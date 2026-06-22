# GitHub Trending 日报 · 2026-06-23

## 今日焦点

> **Agentic 视频生产爆发 · Claude Skills 工程化 · 中国开源 Quant 杀回美榜 · MCP 全栈代码理解 · AI 视频编辑器双雄**
>
> - `calesthio/OpenMontage` 全球首个开源 agentic 视频生产系统，+2,935⭐ 登顶。
> - `mattpocock/skills` 工程师 Claude Skills 套件，+2,051⭐，"Real Engineers" 路线印证 skills 范式爆发。
> - `palmier-io/palmier-pro` 给 AI 用的 macOS 原生剪辑器，+2,462⭐，Swift 入榜罕见。
> - `ZhuLinsen/daily_stock_analysis` LLM 多市场量化分析，+1,560⭐，41,896 forks 显示中国开源 Quant 圈高粘性。
> - `DeusData/codebase-memory-mcp` 158 语言通用代码理解 MCP，+1,186⭐，MCP 生态首次出现"杀手 server"候选。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) | 开源 agentic 视频生产系统，12 pipeline / 52 工具 | Python | 11,814 | +2,935⭐ | 1,535 |
| 2 | [palmier-io/palmier-pro](https://github.com/palmier-io/palmier-pro) | macOS 原生 AI 视频剪辑器 | Swift | 7,247 | +2,462⭐ | 500 |
| 3 | [mattpocock/skills](https://github.com/mattpocock/skills) | 工程师 Claude Skills 套件 | Shell | 141,548 | +2,051⭐ | 12,247 |
| 4 | [ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis) | LLM 多市场量化股票分析 | Python | 45,751 | +1,560⭐ | 41,896 |
| 5 | [DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) | 158 语言代码理解 MCP server | C | 11,450 | +1,186⭐ | 846 |
| 6 | [mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | 817 个 Anthropic 安全技能（MITRE 等 6 框架） | Python | 18,623 | +957⭐ | 2,206 |
| 7 | [bytedance/deer-flow](https://github.com/bytedance/deer-flow) | 字节跳动 SuperAgent，研究/编程/创作 | Python | 73,196 | +736⭐ | 9,893 |
| 8 | [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) | Web 抓取与 agent API | TypeScript | 137,191 | +736⭐ | 7,961 |
| 9 | [penpot/penpot](https://github.com/penpot/penpot) | 开源协作设计工具 | Clojure | 52,825 | +730⭐ | 3,383 |
| 10 | [Stirling-Tools/Stirling-PDF](https://github.com/Stirling-Tools/Stirling-PDF) | GitHub 第一 PDF 工具 | TypeScript | 82,834 | +691⭐ | 7,235 |
| 11 | [garrytan/gstack](https://github.com/garrytan/gstack) | Garry Tan 个人 Claude Code 装备包 | TypeScript | 113,085 | +649⭐ | 16,790 |
| 12 | [tursodatabase/turso](https://github.com/tursodatabase/turso) | Rust 重写 SQLite，进程内 SQL | Rust | 21,424 | +538⭐ | 1,084 |
| 13 | [jamiepine/voicebox](https://github.com/jamiepine/voicebox) | 开源 AI 语音工作站，clone/听写 | TypeScript | 32,158 | +508⭐ | 3,929 |
| 14 | [heygen-com/hyperframes](https://github.com/heygen-com/hyperframes) | 写 HTML 渲染视频，agent 友好 | TypeScript | 29,931 | +369⭐ | 2,818 |
| 15 | [JCodesMore/ai-website-cloner-template](https://github.com/JCodesMore/ai-website-cloner-template) | 一行命令 AI 克隆网站 | TypeScript | 17,672 | +63⭐ | 2,742 |

---

## 重点项目点评

### 🥇 [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) — 今日榜首，+2,935⭐

**全球第一个把"视频后期"拆成 12 个 agentic pipeline 的开源系统**

OpenMontage 以"agentic video production"为口号，把传统视频后期切分成 12 条 pipeline、52 个工具——剪辑、调色、字幕、转场、音乐配音、抖动稳定、镜头检测、转码、发布……每条 pipeline 都可以独立被 agent 调用，也可以串成端到端 workflow。这是 OpenAI Sora / Runway / Pika 推出之后，第一个完全开源、可自托管的"后期 agent 框架"。

它今天爆冲 +2,935⭐ 与 HN 上 Heygen Hyperframes（+369⭐）形成有趣呼应：HTML→视频的"模板范式"和 OpenMontage 的"agent 编排范式"代表了 AI 视频生产的两条主流路线。考虑到字节 deer-flow（No.7）同样占榜，多 agent 框架"从聊天进入媒体"已成定局。

短期看点：(1) 与 HeyGen / Synthesia 商业产品的功能差距追多久能填上；(2) 是否能接住 Sora-2 / Veo-3 之类生成模型作为 pipeline 上游；(3) 社区 PR 速度——目前 1,535 forks 显示参与势头充足。

---

### 🥈 [mattpocock/skills](https://github.com/mattpocock/skills) — +2,051⭐

**"Skills" 范式正在取代 dotfiles 成为 2026 工程师的新身份标志**

Matt Pocock 把自己 `.claude/` 目录里的 skills 整理开源，标题 "Skills for Real Engineers"。这与今天榜上同时出现的 garrytan/gstack（No.11，Y Combinator 总裁的 Claude Code 装备）、mukul975/Anthropic-Cybersecurity-Skills（No.6，817 个安全 skill）共同指向一个事实：**Claude Skills 已经成为 2026 工程师炫技的新载体**。

去年的 dotfiles 战争是 vim 配置文件，今年的 dotfiles 战争是 skills 包——这是一种更高维的 "what kind of engineer am I" 表达。skills 不仅是工具调用清单，它本质上是工程师工作流程的可执行抽象，能被同事直接 fork 复用。

更深的信号：高星 skills 仓库正在形成 social proof 飞轮——某 KOL 推出 skills 包 → 工程师 fork + star → 公司团队批量采用 → 形成事实标准。GitHub Skills 是不是要成为"AI 时代的 npm"？今天的三个高分 skills 仓库（mattpocock / garrytan / mukul975）合计 +3,657⭐，足以引出官方层面的目录化探索。

---

### 🥉 [palmier-io/palmier-pro](https://github.com/palmier-io/palmier-pro) — +2,462⭐

**Swift 入榜的稀客：原生 macOS AI 视频剪辑器**

GitHub Trending 上 Swift 项目极为罕见，何况是+2,462⭐ 的单日爆款。palmier-pro 主打"为 AI 而生的 macOS 视频编辑器"——区别于 Web 端的 OpenMontage 与浏览器端的 HeyGen 路线，它把 native macOS UI + AI agent 控制结合，意味着剪辑过程中的素材管理、时间线、预览渲染都享受原生性能。

它登榜的真正意义不在产品本身，而在"native AI 应用"路线的复辟：今年上半年 Web 端 AI app 同质化严重（一堆 Next.js + OpenAI），原生 macOS / iOS 应用因体验更好、付费转化更高，开始重新成为创业焦点。结合 No.1 的 OpenMontage（Web/CLI）与 No.14 的 Hyperframes（agent 模板），AI 视频生产已经形成三条清晰路线——CLI agent、HTML 模板、Native 应用。

---

### 🏅 [DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) — +1,186⭐

**MCP 生态首个"杀手级 server"候选：覆盖 158 种语言的代码理解**

去年 11 月 Anthropic 推出 MCP 协议至今，市面 MCP server 数百但缺乏一个"必装"项。codebase-memory-mcp 直奔最高频痛点：让 Claude Code / Cursor / Codex 等 agent 能在 158 种语言的项目里建立**持久记忆与跨文件关系图**，而非每次重新扫描。用 C 语言实现也意味着 indexing 性能远高于 Python / Node 同类。

考虑到今天榜上同时有 garrytan/gstack（工程师装备包）、mattpocock/skills（skills 套件）这类围绕 Claude Code 的"周边经济"项目，codebase-memory-mcp 有望成为这条工具链的事实标准底座——如果它能保持单日 +1k⭐ 节奏一周以上，下半年 Anthropic 官方很可能将其加入推荐 MCP 列表。

---

### 🎖️ [ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis) — +1,560⭐

**41,896 forks 的中国开源 Quant 项目杀回美榜**

LLM 驱动的多市场股票分析系统，支持实时数据接入。本身定位"散户日常工具"，但 41,896 forks 的数字背后是中国开源 Quant 圈最庞大的群体使用——A 股 / 港股 / 美股全覆盖 + LLM 解读 + Tushare / akshare 数据接入，几乎是 retail trader 必备工具链。

今天能在国际 Trending 拿到 +1,560⭐ 的爆冲，反映两个变化：(1) 美区 retail trader 开始接受非英文项目作为分析底座；(2) 中国开源在"垂直 + 数据 + LLM"组合的工具链产品上已经形成独特竞争力——和昨日 Zhipu GLM-5.2 的爆冲一起，说明中国开源在 2026 Q2 进入第二个高峰。

---

## 生态观察

**今日 GitHub Trending 的三条主线**：(1) **AI 视频生产范式确立**：OpenMontage（agent 编排）+ palmier-pro（native 剪辑）+ Hyperframes（HTML 模板）三种路线同台亮相，下半年大概率出现整合者；(2) **Skills 经济正式成为生态**：mattpocock + garrytan + mukul975 三个 skills 包占今日新增 ⭐ 接近 6,000，Skills 已经从"个人偏好"升级为"行业基础设施"；(3) **中国开源破圈**：daily_stock_analysis + bytedance/deer-flow 双双进入前列，承接 GLM-5.2 的势头。

**冷信号**：Stirling-PDF、firecrawl、penpot 这些传统强榜仓库依然活跃，但增速明显被 AI 类目压制。**结构性观察**：MCP server 首次出现"必装级"候选（codebase-memory-mcp），意味着 MCP 生态从 2025 末的"实验期"进入"基础设施期"。
