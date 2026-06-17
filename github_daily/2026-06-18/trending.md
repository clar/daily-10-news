# GitHub Trending 每日热榜 · 2026-06-18

## 今日焦点

> **Claude Skills 工程化普及 · Agent 基础设施层成型 · 时间序列基础模型 · MCP 服务正在标准化 · Rust 网络栈"密钥即地址"**
>
> - `mattpocock/skills` 单日 +1,570⭐，13.3 万 star 高位继续爆冲，Matt Pocock 把"给真正工程师用的 .claude 技能"做成了行业模板
> - `Panniantong/Agent-Reach` +1,154⭐，"给 agent 一双能看互联网的眼睛"，Python 端的 agent 工具/记忆栈正在成熟
> - `obra/superpowers` +1,205⭐，agentic skills 框架已被反复 fork 2 万次，证明"骨架化 agent 工程方法论"是真需求
> - `DeusData/codebase-memory-mcp` +718⭐，C 语言写的高性能 MCP 服务器，MCP 生态今天首次有"性能党"作品进入热榜
> - `google-research/timesfm` +712⭐，时间序列基础模型回到榜单，Google Research 在 LLM 之外的另一个"基础模型"赛道持续投入

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [mattpocock/skills](https://github.com/mattpocock/skills) | "Skills for Real Engineers"，来自 .claude 目录 | Shell | 133,433 | +1,570 | 11,596 |
| 2 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic skills 框架 + 软件开发方法论 | Shell | 230,994 | +1,205 | 20,536 |
| 3 | [Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach) | 给 AI agent 一双能看整个互联网的眼睛 | Python | 33,097 | +1,154 | 2,667 |
| 4 | [freeCodeCamp/freeCodeCamp](https://github.com/freeCodeCamp/freeCodeCamp) | 开源编程教育平台 | TypeScript | 449,115 | +764 | 45,088 |
| 5 | [DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) | 高性能代码智能 MCP 服务器 | C | 5,135 | +718 | 479 |
| 6 | [google-research/timesfm](https://github.com/google-research/timesfm) | 预训练时间序列基础模型 | Python | 21,838 | +712 | 2,128 |
| 7 | [Universal-Debloater-Alliance/universal-android-debloater-next-generation](https://github.com/Universal-Debloater-Alliance/universal-android-debloater-next-generation) | 跨平台非 root Android 去广告/精简 GUI | Rust | 7,621 | +465 | 326 |
| 8 | [n0-computer/iroh](https://github.com/n0-computer/iroh) | "IP 会坏，拨号用密钥"——Rust 模块化网络栈 | Rust | 9,622 | +422 | 447 |
| 9 | [meshery/meshery](https://github.com/meshery/meshery) | 云原生（CNCF）管理平面 | TypeScript | 11,002 | +199 | 3,458 |
| 10 | [bytedance/UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop) | 开源多模态 AI Agent 栈（字节跳动） | TypeScript | 36,681 | +148 | 3,700 |
| 11 | [krahets/hello-algo](https://github.com/krahets/hello-algo) | 动画化数据结构与算法教程 | Java | 127,424 | +109 | 15,175 |
| 12 | [penpot/penpot](https://github.com/penpot/penpot) | 开源设计/代码协作工具 | Clojure | 50,053 | +94 | 3,233 |
| 13 | [yairm210/Unciv](https://github.com/yairm210/Unciv) | 文明 V 开源重制（Android/Desktop） | Kotlin | 10,636 | +41 | 1,843 |
| 14 | [continuedev/continue](https://github.com/continuedev/continue) | 开源编码 agent | TypeScript | 33,870 | +38 | 4,693 |
| 15 | [RocketChat/Rocket.Chat](https://github.com/RocketChat/Rocket.Chat) | 任务关键场景的安全沟通 OS | TypeScript | 45,561 | +15 | 13,655 |

---

## 重点项目点评

### 🥇 [mattpocock/skills](https://github.com/mattpocock/skills) — 今日榜首，+1,570⭐

**Claude Skills 已经成为"开发者自带工作流"的事实分发格式**

Matt Pocock 把自己 `.claude/skills` 目录里给"真实工程师"用的技能开源出来，单日 +1,570⭐ 把这个仓库推到了 13.3 万 stars 量级。这不是"又一个 prompt 集合"——它本质上是把 Claude Agent SDK 的 skills 协议当作分发格式，让任何 Anthropic Claude 用户克隆即用。

这个趋势比单个仓库重要：过去两年，工程师社区曾经在"AI 知识"该如何打包上反复试错——Awesome 列表、Cursor rules、Continue 配置、Aider conventions、Claude project files……Skills 用 markdown + 目录结构这种最低门槛的形式，可能成为"开发者带着自己工作流走"的真正标准。注意 `obra/superpowers`（榜眼）和今天热榜上一同出现的多个 skills 仓库都在指向同一方向。

更值得关注的隐含信号：当一个个人开发者的 skills 仓库能稳定占据 GitHub 首页几个月，说明 Anthropic 通过 Claude Code 正在事实上"挟生态以令规则"——开发者把自己的方法论嵌入了 Claude 的运行时，这是任何其他 AI Coding 工具今天都没做到的护城河。

---

### 🥈 [obra/superpowers](https://github.com/obra/superpowers) — +1,205⭐

**agentic skills 框架被 fork 2 万次，方法论正在被工业化**

obra（Jesse Vincent，前 Best Practical / KDE 大佬）发起的 superpowers 仓库以 23 万 stars / 2 万 forks 的体量稳坐 agent 框架第一梯队。它的特别之处不在功能而在"形态"——这不是一个库，而是一个完整的"agentic 软件开发方法论"，把"如何让 agent 帮你工程化地完成长任务"分成可复用的"超能力"模块。

之所以今天再涨 1,205⭐，是因为 superpowers 本周更新了与 Claude Skills 协议的互操作示例。Skills 提供"能力分发"，superpowers 提供"能力编排"，两者拼成 agent 工程的上下游。这也解释了为什么榜单上 6 个 Top-15 项目都和 agent / skills / mcp 相关——这不是巧合，是整个工程生态在 2026 年的主线。

---

### 🥉 [Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach) — +1,154⭐

**"让 agent 看见互联网"的中文社区作品冲上前三**

Agent-Reach 由中国开发者维护，定位是"给 agent 一双能看见整个互联网的眼睛"——本质是 web-browsing / search / scraping 能力的封装层，让 Claude/GPT 系列 agent 可以直接在长任务中调用。33k stars / 2.6k forks 的体量加上单日 +1,154⭐，说明这个垂类（"agent 上网"）至今仍是开发者最痛的中间件。

为什么这种项目能持续上榜？因为虽然 OpenAI / Anthropic / Google 都在做 deep research、web search 内置工具，但**开发者构建自主 agent 时**仍然需要可控的、可自托管的、不会被 rate-limit 的"上网层"。中国开发者在这种"工具中间件"上的供给速度，已经构成 GitHub 中文区的明显特色。

---

### 🛰️ [DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) — +718⭐

**MCP 生态终于有"性能党"作品**

用 **C 语言**写的高性能代码理解 MCP 服务器，把"给 agent 看代码"这件事用最底层的方式做到极致。单日 +718⭐ 把它从 5k 推上了第 5 名。

它的出现填补了 MCP 生态长期的空白：过去一年里，MCP server 主要由 TypeScript / Python 实现，性能往往是瓶颈——尤其是要处理大型 monorepo 时，索引和检索都很慢。C 语言实现意味着可以做到接近 ripgrep 级别的速度，让 agent 真正能在"几十万行代码"的工程上即时回答问题。

MCP 协议 Anthropic 在 2024 年底推出至今，已经度过了"协议存活期"和"应用爆发期"，现在进入"性能优化期"——这个仓库就是标志。

---

### 📈 [google-research/timesfm](https://github.com/google-research/timesfm) — +712⭐

**LLM 之外的另一类基础模型在被持续投资**

TimesFM 是 Google Research 的时间序列基础模型，今天 +712⭐ 重新回到热榜（总 stars 已 21.8k）。它的迭代节奏不像 LLM 那么张扬，但每次小版本更新都能上榜——说明工业界对"通用预测模型"的真实需求被严重低估。

时间序列预测过去几十年是统计学家和 ML 工程师的小众战场，每个行业都要训自己的模型。TimesFM 类似 LLM 之于 NLP，证明了"一个足够大的基础模型可以零样本地做大多数预测任务"。今天能涨星，是因为 v2.5 版本提升了对**更长 horizon、更高频率序列**的支持，金融与零售的实际使用门槛进一步降低。

---

## 生态观察

**主线一：Agent + Skills + MCP 三件套已经吃下半个热榜。** 今天前 15 里有 6 个项目（superpowers、skills、Agent-Reach、codebase-memory-mcp、continue、UI-TARS-desktop）属于这条主线。这是过去 18 个月里第一次出现"agent 工程基础设施"如此集中地占据 GitHub 首页——意味着 2026 年开发者工具的主战场已经不在编辑器、不在 prompt 引擎，而在"agent 怎么稳定完成长任务"的方法论层。

**主线二：基础模型不只是 LLM。** TimesFM（时间序列）、UI-TARS（多模态 GUI agent）今天同时上榜，说明 Foundation Model 的多模态化 / 多领域化在 2026 年正全面铺开。LLM 是入口，但应用层的多样性才决定真正的市场厚度。

**主线三：Rust 工程基础设施。** Universal-Android-Debloater 和 iroh 两个 Rust 项目今天都进了前 10。iroh 的"用密钥而非 IP 地址 dial"代表了去中心化网络栈的延续脉络；UAD 则是终端用户层面"对抗厂商捆绑"的代表。Rust 生态在系统层和工具层的吸引力持续稳固。

**主线四：CNCF 和云原生工具回暖。** Meshery 单日 +199⭐ 重回热榜，是 K8s/服务网格生态的一次能量释放——在过去半年 AI 喧嚣里，这部分基础设施被冷落了，但企业生产仍在持续投入。
