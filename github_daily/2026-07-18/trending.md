# GitHub Trending 每日热榜 · 2026-07-18

## 今日焦点

> **"反 AI slop"设计规范 Hallmark 爆火 · Kimi K3 让 open interpreter 单日 +431 · Copilot SDK 想吃掉整个 IDE 集成层 · DocuSign 开源替代 DocuSeal 上位 · CapCut 开源替代 OpenCut 冲上 7.4 万星**
>
> - `Nutlope/hallmark` +1,486⭐：一套"给 Claude Code/Cursor/Codex 装反 AI-slop 品味"的设计规范，单日暴涨。
> - `codecrafters-io/build-your-own-x` +1,070⭐：527k 巨兽今天又冲 1k 星，"从零复现"始终不过时。
> - `OpenCut-app/OpenCut` +1,077⭐：CapCut 开源替代，剪辑工具赛道进入开源阶段。
> - `HKUDS/DeepTutor` +528⭐：终身个性化辅导系统，教育 Agent 板块再次冒头。
> - `openinterpreter/openinterpreter` +431⭐：为 Kimi K3 优化的 coding agent，开源模型效应立竿见影。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [codecrafters-io/build-your-own-x](https://github.com/codecrafters-io/build-your-own-x) | 从零复现最喜欢的技术 | Markdown | 527,273 | +1,070⭐ | 49,901 |
| 2 | [OpenCut-app/OpenCut](https://github.com/OpenCut-app/OpenCut) | CapCut 开源替代 | TypeScript | 74,808 | +1,077⭐ | 7,541 |
| 3 | [Nutlope/hallmark](https://github.com/Nutlope/hallmark) | 反 AI-slop 设计规范 skill | CSS | 11,960 | +1,486⭐ | 600 |
| 4 | [HKUDS/DeepTutor](https://github.com/HKUDS/DeepTutor) | 终身个性化辅导平台 | Python | 27,325 | +528⭐ | 3,642 |
| 5 | [PostHog/posthog](https://github.com/PostHog/posthog) | 自驱动产品分析平台 | Python | 36,174 | +437⭐ | 3,010 |
| 6 | [openinterpreter/openinterpreter](https://github.com/openinterpreter/openinterpreter) | 面向 Kimi K3 的开源 coding agent | Rust | 66,326 | +431⭐ | 5,701 |
| 7 | [RyanCodrai/turbovec](https://github.com/RyanCodrai/turbovec) | 基于 TurboQuant 的向量索引 | Python | 13,275 | +280⭐ | 1,178 |
| 8 | [PrismML-Eng/Bonsai-demo](https://github.com/PrismML-Eng/Bonsai-demo) | Bonsai 演示项目 | Shell | 1,701 | +279⭐ | 166 |
| 9 | [HenryNdubuaku/maths-cs-ai-compendium](https://github.com/HenryNdubuaku/maths-cs-ai-compendium) | AI/ML 研究工程师资源集 | TypeScript | 6,589 | +248⭐ | 807 |
| 10 | [github/copilot-sdk](https://github.com/github/copilot-sdk) | 集成 Copilot Agent 的多端 SDK | Java | 9,784 | +234⭐ | 1,327 |
| 11 | [docusealco/docuseal](https://github.com/docusealco/docuseal) | DocuSign 开源替代 | Ruby | 17,815 | +152⭐ | 1,769 |
| 12 | [tirth8205/code-review-graph](https://github.com/tirth8205/code-review-graph) | 本地代码智能图谱 MCP | Python | 19,717 | +57⭐ | 2,105 |
| 13 | [anthropics/cwc-workshops](https://github.com/anthropics/cwc-workshops) | Claude on the Web workshop 教材 | TypeScript | 1,572 | +37⭐ | 489 |
| 14 | [protocolbuffers/protobuf](https://github.com/protocolbuffers/protobuf) | Google 序列化协议 | C++ | 71,533 | +18⭐ | 16,191 |

---

## 重点项目点评

### 🥇 [Nutlope/hallmark](https://github.com/Nutlope/hallmark) — +1,486⭐

**"反 AI-slop"品味被打包成一份 Claude/Cursor/Codex 可挂载的 skill**

作者 Nutlope（Together AI 的老玩家）今天把一份"反对 AI slop"的品味手册 hallmark 上线：不是模型也不是框架，而是一份配色 + 版式 + 组件 + 交互反面清单的规范包，声称是给 Claude Code、Cursor、Codex 三家最流行的 AI 代码工具"补上审美"。仓库配了大量对比图——同样一个 landing page 用 hallmark 之前和之后差异明显。

爆火背后是社区共识：**"AI 生成的 UI 全都长一个样"** 这件事已经从段子变成设计师抱怨的正经痛点。hallmark 用"规则化的品味"作为对抗方式，相当于给 vibe coding 强制加了一个 constraint set。这类"AI 时代的设计规范作为可挂载资产"的形态今年会越来越多——它比传统 design system 库轻，也更容易被 LLM 消化。

从技术架构上看，hallmark 采用 CSS + Markdown 双载体，兼容任何能 include 目录的 AI 工具。Nutlope 在 README 里明确说"我们不做组件库，我们做规则"——这条边界让它有别于 Tailwind UI、shadcn。**AI 编码工具的下一个战场是"上下文里能塞什么品味"，hallmark 正好卡在这个位置。**

---

### 🥈 [OpenCut-app/OpenCut](https://github.com/OpenCut-app/OpenCut) — +1,077⭐

**CapCut 开源替代正式上量：视频剪辑的开源阶段到了**

OpenCut 冲上 74k 星、单日 +1,077，标志着一直被认为"太重、生态壁垒太厚"的桌面视频剪辑品类，也进入了 CapCut 引发的替代战。项目提供跨平台桌面客户端（Electron + FFmpeg），核心特性对齐 CapCut 网页版：多轨时间线、AI 字幕、模板、贴纸、导出预设，License 是 GPLv3。

爆火的直接触发点是 CapCut 母公司字节 6 月对 CapCut Pro 的**订阅涨价 + 部分导出限速**，欧美内容创作者集体寻找替代。OpenCut 之前是"能用但小众"的状态，本次事件把它推到 GitHub 首页。

值得关注的是 OpenCut 的社区文档里明确写"AI 特性可选、默认本地推理"——与 CapCut 走向"云端 AI 特性打包收费"完全相反。**"本地优先 + 开源 + 可选 AI"** 这个组合过去三个月已经在浏览器、笔记应用、代码工具上验证过一遍，现在轮到剪辑软件。

---

### 🥉 [openinterpreter/openinterpreter](https://github.com/openinterpreter/openinterpreter) — +431⭐

**Kimi K3 开源发布次日，openinterpreter 直接吃到红利**

openinterpreter 是老牌 coding agent，但它这次刷上榜是因为 README 更新了一条"针对 Kimi K3 优化"的横幅——K3 昨日发布 2.8T 权重、$0.30/M cache-hit 的价格让开源 agent 场景第一次真正有性价比。openinterpreter 团队反应神速，24 小时内把 Rust 端的 prompt template、tool routing、context packing 全部对齐 K3 的 1M 上下文模式，示例演示了在本地跑长上下文 codebase 分析。

这条 trending 背后的信号很清楚：**开源模型只要有 SOTA，围绕它的应用层就会有一次爆发**。K3 昨天发布、openinterpreter 今天冲榜、OpenRouter 侧流量今天翻倍，几乎同步发生。对比 12 个月前 Llama-3 发布时"要等 6 周才有 agent 适配"，今天的适配速度是数量级的加速。这也说明 agent 应用层已经具备"随模型热切"的能力。

---

### 4️⃣ [HKUDS/DeepTutor](https://github.com/HKUDS/DeepTutor) — +528⭐

**教育 Agent 板块再次冒头，港大 HKUDS 出品**

HKUDS 是香港大学做数据挖掘出身的实验室，DeepTutor 定位"终身个性化辅导"：学习者与 Agent 对话时，Agent 会维护跨会话的 knowledge state graph（跟 Anki 的 SRS 系统类似，但基于向量与因果图混合表征），基于该 graph 生成个性化题目、跨主题复习计划和"下一步应学"提示。仓库里带了 K-12 数学、CS 本科课程、语言学习三个 out-of-box 数据集。

DeepTutor 今天冲榜与 **昨天 Google 官宣 NotebookLM 改名 Gemini Notebook** 有直接关系——所有教育 AI 项目都在抢"个性化 + 长期记忆"这个卡位。DeepTutor 走的是学术开源路线，用 arxiv 论文做背书；实际部署主要是学校订阅制 + 免费 API 层。

对 AI 教育创业者的启示：**"跨会话的学习者建模"** 是这波教育 Agent 的最大差异化点，任何单次 chat 打包成课程的产品今年会被 DeepTutor 这类 stateful tutor 挤压。

---

### 5️⃣ [github/copilot-sdk](https://github.com/github/copilot-sdk) — +234⭐

**GitHub 官方发布 Copilot Agent 多端 SDK，杀入 Agent 集成层**

github/copilot-sdk 是 GitHub 昨晚官宣的 Copilot Agent 集成 SDK，覆盖 Java / Kotlin / Swift / .NET，用于把 Copilot Agent 嵌入 IDE、CI/CD、桌面、移动应用。这个 SDK 有别于原来的 Copilot Chat SDK：新版本核心 API 是 `session.attach(context)` + `agent.act(with_tools)`，属于 Anthropic MCP 与 OpenAI Assistants API 之间的第三种设计。

它的战略意义远超 SDK 本身：**GitHub 想在 Anthropic MCP 快速接管开发者 tool routing 生态之前，抢回 IDE 侧的分发权**。Copilot 过去两年在数据侧（代码 telemetry）、模型侧（自研 + OpenAI + Anthropic 混合）都吃到了红利，但工具接入侧一直是被动的。现在推 SDK，等于是"把 Copilot 作为可嵌入 agent runtime"卖给应用开发者。

今日冲榜相当程度上来自 Java 社区——这是 Copilot 长期弱项。GitHub 这一步补齐后，理论上"IDE + Copilot Agent"这条链在 Java/Kotlin/.NET 生态可以完成端到端集成。

---

## 生态观察

**今天 GitHub trending 有四条清晰主线：**

第一，**"AI 时代的品味/规范"作为可挂载资产开始成为新品类**。hallmark 冲榜、DeepTutor 的知识图谱，都在说同一件事：LLM 时代的护城河从"代码"移向"品味 + 规则 + 长期记忆"。这三样都是 skill-shaped、context-shaped 的资产，恰好匹配 Claude Skills、Cursor rules 之类的载体。预计接下来 3-6 个月会出现更多"专门给 LLM 用的规范包"。

第二，**开源模型和开源应用之间的时间差被压缩到 24 小时**。Kimi K3 昨天开源、openinterpreter 今天冲榜；State of Open Source AI 昨天发布、turbovec 今天进榜。基础层与应用层的联动速度是过去 12 个月最大的进化，也解释了为什么这半年 star 曲线越来越 spiky。

第三，**"开源版 X"仍然是 GitHub 上的稳定爆款**——DocuSeal（DocuSign 替代）、OpenCut（CapCut 替代）、DeepTutor（Duolingo Max 替代）都在同一天出现。这说明 SaaS 涨价 + 数据主权担忧 + 本地 AI 可用 三件事叠加，正在系统性推动"开源替代"品类扩张。

第四，**GitHub 官方 Copilot SDK 上榜代表平台方的反击开始**。之前 Anthropic MCP、Cursor 生态、OpenAI Assistants 三家蚕食开发者工作流，今天 GitHub 用 SDK 抢回集成话语权。IDE、Agent runtime、代码索引这条战线接下来会是重头戏。

冷点：**协议层项目关注度持续走低**——protobuf 仅 +18⭐、code-review-graph 只 +57⭐，"通用基础库"叙事对社区吸引力在下降；社区把注意力锁在"具体可用的 Agent / 品味 / 开源替代"上。
