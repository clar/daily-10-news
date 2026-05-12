# Daily Reports Orchestrator

Run all six daily report skills (github-trending, ai-daily, crypto-daily, polymarket-analysis, stock-daily, hacker-news), then commit and publish via PR — one command end-to-end.

## When to invoke

User says "跑一下今日全部日报" / "生成今天的日报" / "/daily-reports" / "daily-reports" / "把所有 daily skill 跑一遍" or similar batch requests.

If they only name a subset (e.g. "只跑 stock 和 crypto"), do NOT use this orchestrator — invoke those skills directly.

## Mandatory pre-flight

1. **Get authoritative date (China timezone)** — never trust context or directory listings:
   ```
   TZ='Asia/Shanghai' date +%Y-%m-%d
   ```
   Bind the output as `{DATE}` and use it for every downstream path.

2. **Check current git state**:
   ```
   git status && git branch --show-current
   ```
   - If on a harness-injected `claude/...` branch → use it as-is
   - Otherwise → `git pull origin main` then `git checkout -b claude/daily-{DATE}`
   - **Never push to main** (HTTP 403 enforced); always PR-merge

## Execution sequence (main agent, sequential)

Per project CLAUDE.md: main agent runs all skills directly. Do not spawn sub-agents for this — token savings are illusory and failure cost is high.

Run each skill in order; after each, write the report file immediately, then proceed:

| # | Skill | Output path |
|---|-------|-------------|
| 1 | `github-trending` | `github_daily/{DATE}/trending.md` |
| 2 | `ai-daily` | `ai_daily/{DATE}/report.md` |
| 3 | `crypto-daily` | `crypto_daily/{DATE}/report.md` |
| 4 | `polymarket-analysis` | `polymarket_daily/{DATE}/report.md` |
| 5 | `stock-daily` | `stock_daily/{DATE}/report.md` |
| 6 | `hacker-news` | `hackernews_daily/{DATE}/report.md` |

Use TodoWrite to track the 6 skill runs + the commit step as 7 items. Mark each complete the moment its file is written.

## Resilience rules

- **Single skill fails or hangs** → skip it, continue to the next, retry the failed one at the end
- **WebSearch context bloat** → use 1-2 targeted queries per skill instead of exhaustive sweeps
- **Network errors** → retry that specific skill only, not the whole batch
- **Partial success** is acceptable: commit whatever reports succeeded; note skipped ones in the PR body

## Commit + merge (after all skills done)

```
git add github_daily/{DATE} ai_daily/{DATE} crypto_daily/{DATE} \
        polymarket_daily/{DATE} stock_daily/{DATE} hackernews_daily/{DATE}
git commit -m "feat: add daily reports for {DATE}"
git push -u origin <current-branch>
```

Then via GitHub MCP (no manual `gh` calls):

1. `mcp__github__create_pull_request` — `base=main`, `head=<current-branch>`, title `feat: add daily reports for {DATE}`, body listing each report with a one-line takeaway
2. `mcp__github__pull_request_read` (`get_status`, `get_check_runs`, `get_review_comments`) — verify no blockers
3. `mcp__github__merge_pull_request` — `merge_method=squash`

GitHub auto-deletes the head branch on squash merge. No local cleanup needed.

## Output to user

End with one or two sentences:
- PR # and merge commit SHA
- Names of any skipped/retried skills (if any)
- File paths of all six reports

Do NOT paste report contents back; they're in the repo.
