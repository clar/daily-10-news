# GitHub Trending 每日报告 · 2026-07-03

## 今日焦点

> **Agent Skills 生态爆发 · Claude Code 插件化 · AI 渗透测试落地 · Codex ⇄ Claude 互操作 · 垂直 Agent（交易/求职）**
>
> - `usestrix/strix` **今日榜首 +2,167⭐** — 开源 AI 渗透测试工具单日暴涨，DevSecOps 是 2026 下半年最强的落地场景
> - `msitarzewski/agency-agents` **+2,925⭐** — "AI 代理公司"模板站上了 12.5 万 stars，Agent Skills 生态进入模板化竞争
> - `obra/superpowers` **+962⭐** — Agentic 技能开发框架，24 万+ stars 稳居 Skills 元项目头把交椅
> - `openai/codex-plugin-cc` **+448⭐** — OpenAI 主动做 Claude Code 插件，两大 Agent 阵营开始互操作
> - `HKUDS/Vibe-Trading` **+918⭐** — 港大 DS 组的个人交易 Agent，学术圈开始下场做垂直 Agent

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [usestrix/strix](https://github.com/usestrix/strix) | 开源 AI 渗透测试工具 | Python | 32,037 | +2,167⭐ | 3,361 |
| 2 | [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | 专家型多智能体"AI 公司" | Shell | 125,418 | +2,925⭐ | 20,345 |
| 3 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic 技能开发框架 | Shell | 244,348 | +962⭐ | 21,678 |
| 4 | [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) | 个人交易 Agent 系统 | Python | 17,305 | +918⭐ | 2,881 |
| 5 | [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) | 缩略语沟通模式的省 token Skill | JavaScript | 80,763 | +866⭐ | 4,521 |
| 6 | [browser-use/video-use](https://github.com/browser-use/video-use) | Coding Agent 驱动的视频剪辑 | Python | 13,745 | +550⭐ | 1,689 |
| 7 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Claude Code 记忆/技能/安全优化 | JavaScript | 225,148 | +508⭐ | 34,455 |
| 8 | [openai/codex-plugin-cc](https://github.com/openai/codex-plugin-cc) | Claude Code 调用 Codex 的插件 | JavaScript | 22,580 | +448⭐ | 1,376 |
| 9 | [hasaneyldrm/exercises-dataset](https://github.com/hasaneyldrm/exercises-dataset) | 433 项健身动作结构化数据 | HTML | 9,218 | +942⭐ | 1,031 |
| 10 | [santifer/career-ops](https://github.com/santifer/career-ops) | Claude Code 求职 Agent 平台 | JavaScript | 57,755 | +322⭐ | 11,382 |
| 11 | [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) | Chrome DevTools MCP 服务器 | TypeScript | 45,068 | +141⭐ | 2,932 |
| 12 | [langflow-ai/langflow](https://github.com/langflow-ai/langflow) | 可视化 Agent / Workflow 平台 | Python | 150,687 | +74⭐ | 9,394 |
| 13 | [agentskills/agentskills](https://github.com/agentskills/agentskills) | Agent Skills 规范文档 | Python | 21,581 | +47⭐ | 1,374 |
| 14 | [pytorch/pytorch](https://github.com/pytorch/pytorch) | 深度学习框架 | Python | 101,217 | +45⭐ | 28,228 |
| 15 | [actions/checkout](https://github.com/actions/checkout) | GitHub Action 官方 checkout | TypeScript | 8,151 | +5⭐ | 2,527 |

---

## 重点项目点评

### 🥇 [usestrix/strix](https://github.com/usestrix/strix) — 今日榜首，+2,167⭐

**AI 渗透测试第一次以"开源单品"形态站上了单日榜首**

Strix 是一个基于 LLM 的 Web 应用渗透测试工具：自动扫描端点、生成 payload、验证利用性并给出修复建议。它今天登顶的意义远大于其技术本身——**这是 AI Agent 在 DevSecOps 场景第一次赢得主流开发者关注**。昨日 Anthropic 生态里 Cognition 刚发布 Devin Security Swarm（GHSA 漏洞 72% 召回率、$90/次），Strix 则是同类需求在开源侧的自然回应。

背后的产业信号：（1）SOC / AppSec 团队被 CVE 增速压垮，愿意接受"AI 主动发现 + 人工确认"的分工；（2）EU AI Act 8 月 2 日 GPAI 罚款权启动，安全审计工具会跟着走一波"合规刚需"预算；（3）Strix 采用"沙箱可复现"的执行框架，是这一代 Agent 项目区别于"演示型 Agent"的关键工程范式。

值得盯的下一步：Strix 是否会围绕 SARIF / OpenVEX 生成合规报告的能力商业化，如果做，那就是开源版 Snyk。

---

### 🥈 [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) — +2,925⭐

**"AI 代理公司"从概念叙事变成模板超市**

这个项目提供一整套"AI 公司"骨架——CEO、CTO、市场、设计、法务等专家型 Agent 各带独立 persona 与工作流，用 shell + Claude Skills 编排。12.5 万 stars 意味着它已经不是"实验项目"，而是这个领域事实上的教科书模板。今日 +2,925⭐ 也是本周单日最高涨幅之一。

它折射的生态趋势是：**Agent Skills 生态在过去 3 个月从"框架层"（BabyAGI、AutoGen 世代）下沉到了"模板层"**。开发者不再关心"如何构建 Agent"，而是关心"如何 fork 一套现成的 Agent 团队并微调 persona"。这种模板化会带来两个次生效应——（a）Agent 项目的差异化竞争从"能力"转向"人设 / 工作流质量"；（b）Skills 交易市场（付费模板）会在 2026 Q3 出现真正的赢家。

配合 Anthropic 昨日主推"Claude Sonnet 5 作为默认代理模型"，这个赛道会持续拥挤。

---

### 🥉 [obra/superpowers](https://github.com/obra/superpowers) — +962⭐

**Skills 元框架：教开发者"如何写 Skill"**

Superpowers 的定位不是"再造一个 Agent"，而是**为 Agentic 开发提供方法论层**——Skill 如何组织、如何按情境激活、如何做 lifecycle、如何测试。24.4 万 stars（今日 +962）说明它已经成为 Skills 生态的官方教材。

值得注意的是它的"元层"属性：如果说 agency-agents 是 App Store 上的应用，那 Superpowers 就是 Xcode。Anthropic 昨日推出 Fable 5 越狱严重程度评分框架的思路（工程化衡量安全）与 Superpowers 的组织化思路是同源的——**2026 下半年最重要的护城河，是"让别人可以在你的规范上构建 Agent"**。

一个值得盯的指标是它的 CLI（`sp` 命令）在多少衍生仓库里被引用；只要 3–5% 的 Skills 项目开始默认走 Superpowers 规范，它就赢下了标准之战。

---

### 🎯 [openai/codex-plugin-cc](https://github.com/openai/codex-plugin-cc) — +448⭐

**OpenAI 主动做 Claude Code 插件——两大阵营开始互操作**

这个仓库位于 `openai/` 官方 org 下，实现"从 Claude Code 里调用 Codex 完成代码审查 / 任务委派"。上线一周 +448⭐，热度不高但战略意义极强——**这是 OpenAI 官方第一次在 Anthropic 的开发工具生态里"寄生"**。

事件反映的两条信号：（1）Claude Code 已经成为 AI 编码工作流的心智入口，OpenAI 无法回避；（2）OpenAI 用"插件"绕开"整体替换"，是当前市场压力（Anthropic ARR 反超）下的务实之举。类似做法昨日在 Perplexity 已经出现——它同时接入 OpenAI、Anthropic、xAI 甚至 DeepSeek，把"模型无关"作为产品差异化。

如果 Anthropic 反手推出 `anthropic/claude-plugin-codex`（Codex CLI 里内嵌 Claude 调用），就会正式进入"跨阵营互操作时代"，AI Agent 市场的赢家不再是"最强模型"，而是"最强兼容层"。

---

### 🚀 [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) — +918⭐

**学术 lab 下场做垂直 Agent：交易赛道升温**

港大数据智能实验室（HKUDS）近年出品了 LightRAG、AutoAgent 等多个开源明星，Vibe-Trading 是他们首个消费级金融 Agent 项目：调用市场行情 + 新闻 + 情绪信号，给出个性化交易建议并支持 paper trading。+918⭐ 说明"AI 交易"作为 Agent 落地场景，正在从二级市场量化的黑箱产品走向 GitHub 可复现代码。

配合 Bloomberg 上周报道的"个人 AI 财富管理"叙事（AUM $30–100k 中段用户的 robo-advisor 2.0）和 xAI 昨日 Grok Voice ($0.05/min) 的按分钟计费 Agent，2026 Q3 的 Agent 落地格局越来越清楚：**开发工具（Claude Code / Cursor / Devin）—工作流（Superpowers / agency-agents）—垂直业务（Strix 安全 / Vibe-Trading 交易 / career-ops 求职）** 三层同时提速。

---

## 生态观察

**今日 GitHub Trending 的 12 条中，Agent / Skills / Claude Code 相关占 9 条**（strix、agency-agents、superpowers、caveman、video-use、ECC、codex-plugin-cc、career-ops、agentskills、chrome-devtools-mcp），是 2026 年至今相关项目最集中的一天。三个明确子趋势：

1. **模板化替代框架化**——agency-agents / career-ops / ECC 这类"开箱即用的 Agent 团队"取代了 2024–25 年的 AutoGen / LangGraph 讨论。
2. **模型互操作正在到来**——openai/codex-plugin-cc 打头阵，这类 cross-vendor plugin 会成为下半年趋势项目的稳定品类。
3. **垂直 Agent 从 SaaS 变成 GitHub 项目**——strix（安全）、Vibe-Trading（交易）、career-ops（求职）、video-use（视频剪辑）都是垂直落地场景开源化的信号。

pytorch / actions/checkout / langflow 这类基础设施项目虽然仍在榜上，但涨幅远远落后于 Agent 相关项目——说明 2026 Q3 开发者注意力已经完全转向"Agent 应用层"。
