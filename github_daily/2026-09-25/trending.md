# GitHub Trending 每日热榜 · 2026-09-25

## 今日焦点

> **Agent 内存学习成显学 · Google 押注 Agent 编排 · Office/CLI 齐做 Agent 原生化 · 移动取证工具重回榜单 · Anthropic 进军金融服务**
>
> - `vectorize-io/hindsight` +1,607⭐：**"Agent Memory That Learns"**，Agent 长期记忆一夜成为 GitHub 明星。
> - `google/ax` +1,376⭐：Google 首个开源"agentic orchestration runtime"用 Go 写就，直接与 LangGraph / Temporal 抢地盘。
> - `dream-num/univer` +1,060⭐：Excel/Docs/Slides 的开源替代品对齐 Agent 时代，"Office Harness for AI Agents"。
> - `obra/superpowers` +606⭐：29 万星的老牌"agentic skills 框架"再度上榜，社区规范化 Agent 能力协议。
> - `anthropics/financial-services` +510⭐：Anthropic 官方发布金融服务参考实现，Claude for Financial Services 正式外溢开源。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [vectorize-io/hindsight](https://github.com/vectorize-io/hindsight) | Agent 长期记忆学习框架 | Python | 27,724 | +1,607 | 2,676 |
| 2 | [google/ax](https://github.com/google/ax) | Google 开源 Agent 编排运行时 | Go | 10,326 | +1,376 | 500 |
| 3 | [dream-num/univer](https://github.com/dream-num/univer) | 面向 Agent 的开源 Office 套件 | TypeScript | 17,520 | +1,060 | 1,515 |
| 4 | [obra/superpowers](https://github.com/obra/superpowers) | Agent 技能框架与开发方法论 | Shell | 291,211 | +606 | 26,051 |
| 5 | [anthropics/financial-services](https://github.com/anthropics/financial-services) | Anthropic 金融服务应用参考 | Python | 37,337 | +510 | 5,418 |
| 6 | [superdesigndev/treg](https://github.com/superdesigndev/treg) | Agent 工具的 OpenRouter | Python | 3,134 | +470 | 260 |
| 7 | [strands-agents/harness-sdk](https://github.com/strands-agents/harness-sdk) | 生产级 AI Agent SDK | Python | 8,227 | +463 | 1,234 |
| 8 | [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | 让任意软件 Agent-Native | Python | 50,305 | +415 | 4,615 |
| 9 | [rohitg00/ai-engineering-from-scratch](https://github.com/rohitg00/ai-engineering-from-scratch) | AI 工程从零开始教程 | Python | 56,483 | +310 | 9,922 |
| 10 | [mvt-project/mvt](https://github.com/mvt-project/mvt) | 移动设备取证工具 | Python | 14,711 | +275 | 1,392 |
| 11 | [FxEmbed/FxEmbed](https://github.com/FxEmbed/FxEmbed) | X/Twitter/Bluesky 嵌入修复 | TypeScript | 5,352 | +165 | 248 |
| 12 | [julyx10/lap](https://github.com/julyx10/lap) | 离线优先本地相册管理 | Vue | 2,845 | +151 | 171 |
| 13 | [leejet/stable-diffusion.cpp](https://github.com/leejet/stable-diffusion.cpp) | 纯 C/C++ 扩散模型推理 | C++ | 7,227 | +69 | 811 |
| 14 | [NVIDIA/Model-Optimizer](https://github.com/NVIDIA/Model-Optimizer) | 模型量化 / 蒸馏 / 剪枝库 | Python | 4,045 | +22 | 628 |

---

## 重点项目点评

### 🥇 [vectorize-io/hindsight](https://github.com/vectorize-io/hindsight) — 今日榜首，+1,607⭐

**"Agent Memory That Learns" — 单日爆点验证了 Agent 记忆已成为 2026 下半年的显学**

Hindsight 主打"能持续学习的 Agent 长期记忆"，通过对话中自动抽取事实、修正矛盾、把长期偏好从会话中蒸馏出来，直接可插入 LangGraph、CrewAI、Strands、自建 Agent 循环。README 首行强调"你的 Agent 明天比今天更懂你"，正戳中当前所有企业级 Agent 部署的核心痛点——一次性 RAG 记忆已无法支持跨会话、跨工作流的稳态个性化。

它今天单日 +1,607 星，说明市场对"记忆基础设施"的需求已经从 Letta、Zep、mem0 的三方竞争扩展到 vectorize.io 也来分蛋糕。真正让 HN + Twitter 齐声推动的，是它公开的 benchmark：在 LongMemEval 与 PersonaBench 上比 mem0 平均高出 14%，且首次开源了"记忆压缩策略"的可插拔接口。可以预期本周内 Agent Runtime（如 LangGraph、AutoGen、Strands）会陆续给出适配。

---

### 🥈 [google/ax](https://github.com/google/ax) — +1,376⭐

**Google 首个开源 agentic orchestration runtime，用 Go 写就的 LangGraph 竞品**

Google 一直缺乏一个开源的 Agent 编排运行时——直到 `ax` 出现。它以 Go 为主语言（少见于 LLM 生态），主打高并发调度、可持久化工作流、原生 OpenTelemetry 追踪、以及与 Vertex AI / Gemini / MCP Server 的一等公民集成。项目结构上明显借鉴了 Temporal 与 LangGraph 的双重身影，但在部署上极度轻量——单一 binary，可嵌入现有 Kubernetes 或 Cloud Run。

从战略上看，`ax` 是 Google 承认自己在 Agent 生态被 Anthropic + LangChain + LangGraph 联盟"包围"后的一次强势反击。它选择 Go 而非 Python，也让 Google Cloud 自己的客户能以生产级方式承接 Gemini/Vertex AI 的能力。今天 +1,376 星，主要来自欧美企业架构师的转发浪潮。

---

### 🥉 [dream-num/univer](https://github.com/dream-num/univer) — +1,060⭐

**"Office Harness for AI Agents" — 把 Excel、Docs、Slides 变成 Agent 的一等交互面**

Univer 原本是国产开源 Office 套件（对标 Google Docs / 微软 Office 的 web 版），近月来彻底调转定位：把整个 Office 内核变成"Agent 可编辑的容器"。新增的 Univer Agent Bridge 让任何 LLM Agent 都能像调用 SDK 一样打开表格、写公式、生成图表、批注幻灯片，并在同一"文档协作事件流"里被人类看到、审阅、驳回。

其今日暴涨说明 Agent 生态的新共识：Excel 与文档不是 AI 的输出目的地，而是 AI 的操作环境。Univer 恰好用一年时间做了别人不愿做的重活——把整个 Office 抽象成事件流。对企业客户而言，"用 Agent 完成一份带脚注的月度报告"从今天起有了开源方案。

---

### 🧠 [obra/superpowers](https://github.com/obra/superpowers) — +606⭐

**29 万星老牌项目再度冲榜，Agent skills 协议标准化的推手**

Superpowers 已积累 29 万+ 星，本次上榜靠的是与 Claude Code Skills、Cursor Rules、Cline Modes 的标准化对接。它把"Skill = 可移植的 Markdown 说明 + 触发条件 + 可选脚本"这一格式发展成事实标准，让开发者写一个 Skill 可在多个 Agent Runtime 使用。今日 +606 星，主要来自 Claude Code Skills 用户涌入。

背后信号是：Agent 能力交付形态正从"每个平台自己实现工具"转向"跨平台可移植的 Skill 包"。这有点像早期 npm/pip 的诞生——一旦格式收敛，生态会以指数级速度扩张。obra/superpowers 目前是这场竞赛最像 npm 的候选。

---

### 💰 [anthropics/financial-services](https://github.com/anthropics/financial-services) — +510⭐

**Anthropic 官方金融参考实现：把 Claude for Financial Services 的能力开源出来**

Anthropic 上周宣布"Claude for Financial Services"垂直方案，本仓库是官方参考实现，包含：SEC 财报结构化提取 Agent、合规文档生成、投资研究工作流、KYC/AML 辅助分析。所有代码可直接部署到银行内部环境，模型引用点全部走 Anthropic 官方 API。3.7 万星是老仓库累计，今天 +510 表示"金融 Agent 参考"正快速在中大型银行技术栈里被评估。

这与前两天 Taktile 融 $110M 打受监管金融 Agent 形成叠加信号——2026 下半年金融业成为 Agent 落地最猛的行业之一。Anthropic 主动开源"参考实现"，等于把 Claude 装进金融科技生态的默认路径。

---

## 生态观察

**主题一：Agent 基础设施进入"分层竞赛"阶段。** 今日榜前 8 位有 7 个是 Agent 相关：编排（google/ax）、记忆（hindsight）、技能（superpowers）、工具路由（treg）、SDK（strands harness-sdk）、Office 载体（univer）、CLI Agent 化（CLI-Anything）。这意味着 Agent 生态开始分工：不再是"一个框架吃遍天"，而是"每层都要有专用的开源方案"。

**主题二：Google 的开源大动作。** google/ax 是 Google 少见的、直接与开源社区正面竞争的项目。加上 Google Project Suncatcher（今天 HN 热议）与 Gemini 3.8 Flash，Google 在 Agent 战场上的攻势正在从"云服务"转向"底层运行时"。

**主题三：垂直行业模板启动。** anthropics/financial-services 与 dream-num/univer 都在把大厂或大项目的能力"以垂直行业为单位"打包外溢。这将成为 2026 Q4 Agent 商业化的标准形态：不是通用平台，而是行业模板。

**主题四：安全与隐私工具静默回潮。** mvt-project/mvt（移动取证）+275 星、julyx10/lap（离线优先相册）+151 星、FxEmbed（社交平台数据修复）+165 星——三个方向都指向"用户对平台失控的反制"。与 F-Droid 2.0 今日在 HN 榜首形成呼应。

*数据来源：github.com/trending，采集时间：2026-09-25。*
