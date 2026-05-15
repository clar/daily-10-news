# Hacker News Daily Report

Generate a daily Hacker News front-page analysis in Chinese.

## Data Source

- **Primary**: [Hacker News front page](https://news.ycombinator.com/) — the daily top stories ranked by HN's algorithm
- **Firebase API**:
  - Top story IDs: `https://hacker-news.firebaseio.com/v0/topstories.json`
  - Single item: `https://hacker-news.firebaseio.com/v0/item/{id}.json` (returns `title`, `url`, `score`, `descendants` for comment count, `by` for author, `time`)
- Fetch the top 15-20 stories with: title, URL / domain, score, comment count, author

## Analysis Steps

1. **Fetch today's top 20** from the front page (use API to avoid scraping)
2. **Enrich each story**: if the URL points to a long article, briefly read it to grasp the angle
3. **Categorize** into: tech / startup / research / policy / culture / Show HN / Ask HN
4. **Identify themes**: what is the HN crowd debating today — new framework, layoffs, AI release, gov policy?
5. **Pick 3-5 stories** for deep commentary — biggest discussions, signal-rich items, or theme-defining posts
6. **Read comment patterns** when possible — HN comments often contain the real insight; quote / summarize a top comment if it sharpens the analysis

## Report Format

```markdown
## 今日焦点

> **{theme keywords separated by ·, 3-5 items}**
>
> - **{story title}** {one-line takeaway with score / comment count}
> - **{story title}** {...}
> - (3-5 bullet points total)

---

## 今日热榜总览

| 排名 | 标题 | 描述 | 分数 | 评论数 |
|------|------|------|------|--------|
(15-20 rows. **标题 must always link to the HN discussion page** (`https://news.ycombinator.com/item?id={id}`) — readers come here to find the discussion, not the article. 描述 is a ≤25-character Chinese summary capturing the angle, not just restating the title.)

---

## 重点讨论点评

### 🥇 [{title}]({hn_or_article_url}) — {score}分 · {comments}评

**{subheading that frames why this discussion matters}**

{2-3 paragraphs analysis. What's the post about, why is HN debating it, what does the comment section reveal that the headline doesn't}

> *热门评论摘要：* {1-2 sentences paraphrasing the top comment(s) when relevant}

---

### 🥈 [{title}]({url}) — {score}分 · {comments}评

{same structure}

---

(3-5 total "重点讨论点评" entries)

## 社区脉搏

{One short section summarizing the day's HN mood — what's heating up, what got flagged, what's the meta-debate (e.g., AI doomers vs. accelerationists, layoffs vs. hiring, open source vs. corporate)}
```

## Output

Save to: `hackernews_daily/{YYYY-MM-DD}/report.md`

## Notes

- All text in **Chinese**
- **热榜总览表的标题链接必须是 HN 讨论页** (`https://news.ycombinator.com/item?id={id}`)，让读者一键进入评论区；**不要**指向原文 URL
- 重点讨论点评 (🥇🥈🥉…) 的标题链接也优先用 HN 讨论页；如果文章本身才是"主菜"（如长篇研究 / 公告原文），可以指向原文，但要在正文里另行提供 HN 讨论链接
- Score/comments in format `{N}分 · {M}评`
- Distinguish HN's recurring genres: **Show HN** (creator self-post), **Ask HN** (question to the community), **Launch HN** (YC company launch) — call these out explicitly
- Focus on **why the HN crowd cares**, not just summarizing the article — this skill's value is reading the room, not aggregating links
- 3-5 deep commentaries is ideal; don't pad if today's front page is quiet
