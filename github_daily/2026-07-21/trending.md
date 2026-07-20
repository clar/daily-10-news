# GitHub Trending 每日榜单 · 2026-07-21

## 今日焦点

> **MCP 生态爆发式扩张 · Agent Harness 与 Coding CLI 三分天下 · AI 网关成本战全面开打 · 中国项目占据前 15 三席（kimi-cli、ktransformers、AstrBot） · Rust 在 Agent 领域重新出圈**
>
> - `tirth8205/code-review-graph` **+1,876⭐**，MCP 本地化知识图，把 AI 阅读代码的 token 消耗砍 82 倍
> - `1jehuang/jcode` **+612⭐**，Rust 写的 Agent Harness，14ms 首帧、27MB 内存
> - `diegosouzapw/OmniRoute` **+1,300⭐**，聚合 268 个 AI 供应商的开源网关，主打"每月 14 亿免费 tokens"
> - `MoonshotAI/kimi-cli` **+405⭐**，月之暗面同步官方 CLI，与 Kimi Work 桌面端左右手互搏
> - `every-app/open-seo` **+983⭐**，开源版 Semrush，罕见的非 AI 项目挤进前十

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [tirth8205/code-review-graph](https://github.com/tirth8205/code-review-graph) | MCP + CLI 本地代码智能图谱 | Python | 23,029 | +1,876⭐ | 2,270 |
| 2 | [1jehuang/jcode](https://github.com/1jehuang/jcode) | 最智能的代码 Agent Harness | Rust | 9,581 | +612⭐ | 1,078 |
| 3 | [diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute) | 268+ 供应商 500+ 模型 AI 网关 | TypeScript | 21,682 | +1,300⭐ | 2,951 |
| 4 | [rohitg00/ai-engineering-from-scratch](https://github.com/rohitg00/ai-engineering-from-scratch) | AI 工程从零教程 | Python | 40,479 | +846⭐ | 6,717 |
| 5 | [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | 一整个 AI 代理机构在指尖 | Shell | 134,666 | +744⭐ | 21,961 |
| 6 | [kvcache-ai/ktransformers](https://github.com/kvcache-ai/ktransformers) | 异构 LLM 推理灵活框架 | Python | 18,722 | +448⭐ | 1,463 |
| 7 | [jamiepine/voicebox](https://github.com/jamiepine/voicebox) | 开源 AI 语音工作室 | TypeScript | 44,120 | +839⭐ | 5,363 |
| 8 | [topoteretes/cognee](https://github.com/topoteretes/cognee) | 开源 AI 记忆平台 | Python | 28,762 | +249⭐ | 2,741 |
| 9 | [Robbyant/lingbot-map](https://github.com/Robbyant/lingbot-map) | 前馈式 3D 场景重建基础模型 | Python | 14,176 | +554⭐ | 1,480 |
| 10 | [every-app/open-seo](https://github.com/every-app/open-seo) | 开源版 Semrush / Ahrefs | TypeScript | 5,802 | +983⭐ | 643 |
| 11 | [MoonshotAI/kimi-cli](https://github.com/MoonshotAI/kimi-cli) | 月之暗面官方 CLI Agent | Python | 10,212 | +405⭐ | 1,217 |
| 12 | [AstrBotDevs/AstrBot](https://github.com/AstrBotDevs/AstrBot) | AI Agent 助手 & 开发框架 | Python | 37,059 | +330⭐ | 2,575 |
| 13 | [PrefectHQ/fastmcp](https://github.com/PrefectHQ/fastmcp) | Pythonic 方式构建 MCP Server | Python | 26,516 | +77⭐ | 2,163 |
| 14 | [KnockOutEZ/wigolo](https://github.com/KnockOutEZ/wigolo) | 本地优先搜索/爬取/研究 MCP | TypeScript | 2,490 | +695⭐ | 144 |
| 15 | [tokio-rs/topcoat](https://github.com/tokio-rs/topcoat) | 电池已包含的 Rust Web 框架 | Rust | 1,507 | +374⭐ | 40 |

---

## 重点项目点评

### 🥇 [tirth8205/code-review-graph](https://github.com/tirth8205/code-review-graph) — 今日榜首，+1,876⭐

**"给 AI 一张知道该读哪些文件的地图"，中位数 token 节省 82 倍**

这个项目的定位太精准了：不是又一个 code assistant，也不是又一个 MCP server 模板，而是**MCP 生态里最关键的中间层——代码结构感知层**。做法直接——用 Tree-sitter 解析仓库、把符号/引用/依赖关系存进 SQLite，然后暴露一个 MCP 工具给上层 Agent（Claude Code、Cursor、Kimi CLI 都可以调）。Agent 问"这个 PR 会影响哪些文件"时，图谱直接算出"爆炸半径"，只把真正相关的 5-10 个文件塞进上下文，而不是让 Agent 全库扫描。

作者贴出的基准数字非常吸睛：在 6 个仓库上做 code review 类问题，**每问 token 中位数节省 82 倍，大型 monorepo 上最高 528 倍**。这直接击中 2026 年 Agent 时代的头号痛点——上下文成本。1M-token 模型不是万能钥匙，把 500K 无用代码塞进去和塞进 500 行相关代码，同样一个问题成本相差数百倍。

这条项目一天 +1,876⭐ 让它成为 2026 年 7 月最亮眼的 MCP 生态基础设施——它填补的正是 Anthropic MCP 协议缺失的那一块"知识层"，而不是仅仅在做又一个"聊天+工具调用"应用。

---

### 🥈 [1jehuang/jcode](https://github.com/1jehuang/jcode) — +612⭐

**Rust 版 Claude Code：14ms 首帧、27MB 内存，Swarm 多 Agent 协作**

jcode 的定位是 "Agent Harness"（Agent 骨架/宿主环境），而不是又一个聊天式编码工具。作者选 Rust 是有意为之——**性能压制**：单会话 27.8 MB 内存、14 ms time-to-first-frame，这些数字放在 Node.js/Python 主导的现状里显得刺眼。它想说明一件事：Agent 时代的宿主工具本身不该是资源黑洞。

功能上最有意思的是 **Swarm 模式**——多个 Agent 在同一仓库并行工作，自动做冲突解决和相互消息。这直接呼应了 Cursor 上周的博文 "Agent swarms and the new model economics"（今日 HN 也上榜）：**AI 编码从"单 Agent 长时程"转向"多 Agent 并发"**。加上语义向量记忆、跨提供商（Claude / OpenAI / Gemini / Ollama）、浏览器自动化（Firefox）、Agent 甚至能改自己源码——它想成为的是 Claude Code 的"更开放、更快、更硬核"版本。

Rust 在 Agent 生态里 2025 年初还只是零星出现，2026 下半年已经能占到今日榜第二名，可以说 Rust 在 Systems + AI 的双重势位下拿到了它一直等待的应用层入口。

---

### 🥉 [diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute) — +1,300⭐

**"月免费 14 亿 tokens"——AI 网关战场的价格屠夫**

OmniRoute 把 271 个 AI 供应商聚合到一个本地端点（`http://localhost:20128/v1`），支持 26+ 编码 Agent（Claude Code / Cursor / Cline / Copilot 都能一键指过来）。它的杀手锏有三个：**免费 tier 聚合**（90+ 供应商的免费额度整合起来每月约 14 亿 tokens）、**智能路由**（免费 / 便宜 / 高级三档自动切换）、**Token 压缩**（RTK + Caveman 双引擎平均省 89%）。

放在 OpenRouter、LiteLLM 已经在做的赛道里，OmniRoute 用"免费 tier 聚合"这一角度突围。它切中了两类用户：**独立开发者**（用免费额度做原型不心疼）和**成本敏感的中小团队**（把 GPT-5.6 Luna 和 Kimi K2 等便宜模型自动混合，比全走一家 API 便宜 60%）。这也是今日 AI Daily 里 GPT-5.6 三档 + Claude Sonnet 5 促销价 $2/$10 现象的"上游反应"——**大模型价格战下沉到网关层，谁能自动路由到最低价谁赢**。

MIT 协议、无默认 telemetry 是它冲上 +1,300⭐ 的另一层原因——在数据敏感的企业推广时，这两条比"聚合功能"更能过合规。

---

### 🎯 [MoonshotAI/kimi-cli](https://github.com/MoonshotAI/kimi-cli) — +405⭐

**Kimi 的 CLI + Work 双钩战术：抢占开发者桌面入口**

同一天，Moonshot 在 HN 上有 Kimi Work（桌面 Agent），在 GitHub 上有 kimi-cli（终端 Agent），组合出击的意图非常明显——**围住开发者的整个工作面**。kimi-cli 的能力清单没有惊喜：读改代码、执行 shell、抓网页、MCP tool 支持、VS Code 扩展、Zed/JetBrains 通过 ACP 兼容。**惊喜在于时序：** README 已经写了"kimi-cli 正在被 Kimi Code CLI 取代"，意味着这个仓库刚火就要迭代，节奏比 Anthropic 的 Claude Code 还激进。

Moonshot 走的路径是"追赶 + 差异化定价"：功能对齐 Claude Code / Codex CLI 的核心特性，但价格拉到对方的 1/3。放在今日 GitHub Trending 里，能看到中国 AI 应用层项目的三席（kimi-cli #11、ktransformers #6、AstrBot #12）合计 +1,183⭐——**开发者社区对"低价 + 开源 + 功能对齐"三合一的组合已经形成惯性偏好**。

---

### 🚀 [every-app/open-seo](https://github.com/every-app/open-seo) — +983⭐

**罕见的非 AI 项目冲进前 10，SaaS 挑战开源反攻**

在 AI 主题彻底霸占 GitHub Trending 半年多后，一个纯 SEO 工具突然爬到第 10 位，值得单独说一句。Semrush 和 Ahrefs 是 SEO 圈两大付费巨头（订阅 $99-$499/月），open-seo 打出的旗号是"开源替代品"——反向链接分析、关键词研究、rank tracking、爬虫全部开源实现。

这条帖的爆红反映了 2026 年一个持续现象：**AI 让开源社区"重做付费 SaaS"的门槛骤降**。用 LLM 写爬虫、调用免费 SERP API、批量处理关键词——过去需要 20 人研发团队的功能，现在两三人 side project 能做出来 80% 覆盖。Notion 有 AppFlowy、Airtable 有 NocoDB、Semrush 现在有 open-seo——**这条替代赛道未来一年会更拥挤**。

---

## 生态观察

**MCP 生态首次撑起 GitHub Trending 单日**：#1 code-review-graph、#13 fastmcp、#14 wigolo 全是 MCP 主题，加上 jcode / kimi-cli / OmniRoute 全都以 MCP 为一等公民。这说明 MCP 已经从"Anthropic 家的协议"变成了跨厂商 Agent 生态的事实标准，围绕它的**中间层项目正在集中爆发**——不做 Agent 本身，而做"给 Agent 用的知识层、工具层、网关层"。

**Agent Harness 已成显学**：jcode（Rust）、agency-agents（Shell）、AstrBot（Python）、kimi-cli（Python）四条项目都是"承载 AI Agent 的骨架"，不是聊天前端也不是模型本身。这一层过去被 Claude Code / Cursor 独占，现在开源生态正在正面切入。可以预见 2026 下半年会有一波"Claude Code 替代品"井喷。

**中国项目再度回榜**：ktransformers、AstrBot、kimi-cli 组队上榜，加上今日 HN 头条 "China's open-weights AI strategy is winning"，形成呼应。**开源权重路线在开发者社区的接受度已远超商业新闻的判断**。

**Rust 悄悄回归应用层**：#2 jcode、#15 topcoat 均为 Rust 项目，前者 Agent Harness、后者 Web 框架。Rust 走出"Systems only"标签的这一波来自 AI 基础设施场景——性能要求真的高时，Node.js / Python 撑不住。

**非 AI 项目的稀缺回归**：open-seo（#10）、Airport Simulator（不在此榜但今日 HN 第 9）是仅有的两个非 AI 项目。整个开源生态几乎被 AI 全面接管的 2026 年，这种偶尔的"传统项目冲榜"越来越像市场信号——**AI 不能吃掉所有品类**，某些垂直领域（SEO、游戏、开发工具）依然值得独立创业。

---

*生成时间：2026-07-21 · 数据源：github.com/trending · Top 15*
