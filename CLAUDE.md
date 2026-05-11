# 项目说明

本仓库用于存放每日自动生成的资讯报告（AI、加密、美股、GitHub trending、Polymarket）。

## 日期规则（强制）

生成或引用"今日报告"的路径时，**必须**严格遵守以下流程：

1. **以中国时间（UTC+8 / Asia/Shanghai）为准**，不使用 UTC 或本地时区。
2. 在决定日期之前，**必须先执行一次 shell 命令**获取权威日期，不得凭 context、记忆或仓库已有目录推断：
   ```
   TZ='Asia/Shanghai' date +%Y-%m-%d
   ```
3. 该命令输出即为"今日"日期（格式 `YYYY-MM-DD`），用于所有报告目录：
   - `ai_daily/{YYYY-MM-DD}/report.md`
   - `crypto_daily/{YYYY-MM-DD}/report.md`
   - `stock_daily/{YYYY-MM-DD}/report.md`
   - `polymarket_daily/{YYYY-MM-DD}/report.md`
   - `github_daily/{YYYY-MM-DD}/trending.md`
4. 仓库中已存在某个日期的目录**不意味着**那就是今天，可能是历史报告——永远以命令输出为准。

## 执行模式（强制）

生成日报时**默认由主 agent 亲自执行全部 skill**，不使用子 agent，原因：

- 子 agent 不省 token（反而多消耗系统 prompt 和重复加载 skill）
- 子 agent 容易遇到 stream idle timeout、沙箱写文件受限等问题，失败代价高
- 只有在明确"独立 + 重 IO + 并行收益大"场景下才考虑子 agent

**推荐流程（顺序执行）：**

1. `TZ='Asia/Shanghai' date +%Y-%m-%d` 拿日期
2. 逐个运行 5 个 skill（github-trending、ai-daily、crypto-daily、polymarket-analysis、stock-daily），每个完成立刻写文件
3. 全部完成后一次性 `git add` + `commit` + `push`

**遇到问题时的优化策略（按顺序尝试）：**

- 单个 skill 卡住：跳过它，继续下一个，最后单独补
- WebSearch 过多撑爆 context：改用更精准的 1-2 次查询，不要穷举
- 耗时过长：允许部分 skill 使用子 agent 并行（仅限无写文件依赖的），但要在 prompt 里显式传入日期
- 网络失败：重试该单项，不重跑全部

## 分支与提交（强制）

> **直推 `main` 会被 harness 代理以 HTTP 403 拦截**，必须走 "feature 分支 + PR + MCP 合并" 流程。

标准流程：

1. 开工前在 `main` 上 `git pull origin main`，确保基础最新
2. 切到 daily 分支：harness 注入的分支名（如 `claude/practical-babbage-xxxx`）就用它；否则用 `git checkout -b claude/daily-{YYYY-MM-DD}`
3. 写完 5 份报告，`git add` 对应目录 → `git commit` → `git push -u origin <daily-branch>`
4. 立刻通过 GitHub MCP 自动合入 main，**无需人工点击**：
   - `mcp__github__create_pull_request`（base=`main`、head=`<daily-branch>`）
   - `mcp__github__merge_pull_request`（`merge_method=squash`）
5. 合并成功即视为发布完成；如 MCP 返回需要审核/检查未通过，再告知用户人工介入
6. 合并完成后**可以直接删除** daily 分支（无需保留历史，main 已经有 squash 后的提交）

注意事项：

- **永远不要尝试 `git push origin main`**，会浪费时间在 403 重试上
- 如果当前已经在 daily 分支（如 routine 启动时 harness 已 checkout），直接在该分支上 commit/push 即可，不要切回 main
- PR 标题统一格式：`feat: add daily reports for {YYYY-MM-DD}`
- 仓库已开启 GitHub "Automatically delete head branches"，PR squash 合并后 daily 分支会被 GitHub 服务端自动删除，**无需任何额外清理动作**

## Skill 目录

各报告对应的 skill 定义在 `.claude/skills/` 下，报告格式以各 SKILL.md 为准。
