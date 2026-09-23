# GitHub Trending 每日报告 · 2026-09-24

## 今日焦点

> **Agent 编排框架三雄争锋 · Office 场景 Agent 化 · Claude Code 生态持续扩张 · 金融科技开源逆袭 · 移动取证/代码情报 MCP 上位**
>
> - `google/ax` 一日暴涨 **+1,542⭐**：Google 正式加入 Agent 编排框架战场，直击 LangGraph、Substrate、LlamaIndex。
> - `dream-num/univer` 单日 **+1,140⭐**：把 Office/PDF 塞进 Agent Runtime，"AI 原生 Office"新范式。
> - `anthropics/financial-services` **+665⭐**：Anthropic 自己下场做行业解决方案，官方 Cookbook 升级为"官方参考产品"。
> - `browser-use/video-use` **+745⭐**：视频编辑首次进入 Coding Agent 工作流。
> - `obra/superpowers` **+485⭐**：**29 万星** 的 Agentic Skills 元框架继续吸血，Skills 生态出现"框架的框架"。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [anthropics/financial-services](https://github.com/anthropics/financial-services) | Anthropic 金融行业 Agent 参考实现 | Python | 36,904 | +665 | 5,374 |
| 2 | [google/ax](https://github.com/google/ax) | Google 开源 Agent 编排运行时 | Go | 8,974 | +1,542 | 428 |
| 3 | [davila7/claude-code-templates](https://github.com/davila7/claude-code-templates) | Claude Code 配置和监控 CLI | Python | 31,468 | +393 | 3,574 |
| 4 | [BuilderIO/agent-native](https://github.com/BuilderIO/agent-native) | 面向 Agent 的应用框架 | TypeScript | 6,506 | +135 | 584 |
| 5 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic Skills 元框架 | Shell | 290,653 | +485 | 26,007 |
| 6 | [dream-num/univer](https://github.com/dream-num/univer) | Agent 原生 Office Runtime | TypeScript | 16,284 | +1,140 | 1,432 |
| 7 | [Open-Dev-Society/OpenStock](https://github.com/Open-Dev-Society/OpenStock) | 开源实时行情/交易平台 | TypeScript | 18,781 | +379 | 2,283 |
| 8 | [agent-substrate/substrate](https://github.com/agent-substrate/substrate) | Substrate Agent 核心系统 | Go | 3,464 | +560 | 410 |
| 9 | [strands-agents/harness-sdk](https://github.com/strands-agents/harness-sdk) | 生产级 Agent Python/TS SDK | Python | 7,818 | +96 | 1,199 |
| 10 | [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | "让所有软件都变成 Agent Native" | Python | 49,889 | +41 | 4,599 |
| 11 | [superdesigndev/treg](https://github.com/superdesigndev/treg) | Agent 工具的 OpenRouter | Python | 2,677 | +502 | 240 |
| 12 | [pbakaus/impeccable](https://github.com/pbakaus/impeccable) | AI Harness 能力设计语言 | JavaScript | 70,296 | +287 | 4,269 |
| 13 | [mvt-project/mvt](https://github.com/mvt-project/mvt) | 移动设备取证与入侵检测 | Python | 14,457 | +546 | 1,381 |
| 14 | [DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) | 亚毫秒响应的代码智能 MCP | C | 44,532 | +266 | 3,635 |
| 15 | [browser-use/video-use](https://github.com/browser-use/video-use) | 用 Coding Agent 编辑视频 | Python | 26,466 | +745 | 3,163 |

---

## 重点项目点评

### 🥇 [google/ax](https://github.com/google/ax) — 今日榜首，+1,542⭐

**Google 终于把自己的 Agent 编排框架推到了 GitHub 主战场**

`ax` 是 Google 官方开源的 Agent 编排运行时，用 Go 编写，强调**多 Agent DAG 编排、可观测性、以及和 Vertex/GKE 的 first-class 集成**。这不是一个"另一款 LangGraph"，而是 Google 内部 Gemini Agent 产品体系（Astra、Cyber、Agent Builder）的一个下探版本，本质上是"把内部生产 Agent 栈标准化后开源"的策略。

真正让它一天冲进 1,500+ 星的原因有三：一是 Google 刚在 3 月 GTC DC 和 Microsoft、NVIDIA 深化合作，官方现在处于"必须交付跨云 Agent 故事"的窗口；二是 Go 语言选型让它天然区别于 Python 系框架，直接吸走了大量 Kubernetes / 平台工程社区的关注；三是 README 里明确点名了 LangGraph、CrewAI、Substrate 作为对比对象——Google 不再遮遮掩掩。

这条趋势 24 小时内值得盯的：ax 的插件模型是否会正面挑战 MCP，还是选择"生态兼容"路线。如果是后者，Anthropic 的 MCP 仍将是事实上的中层协议标准。

---

### 🥈 [dream-num/univer](https://github.com/dream-num/univer) — +1,140⭐

**"AI 原生 Office"：把 Excel / Word / PPT / PDF 塞进一个 Agent Runtime**

Univer 早期是纯粹的开源电子表格引擎，但近三个月完成了一次彻底重构，把自己变成了 **"Office Harness for AI Agents"**——一个统一的表格、文档、幻灯片、PDF 运行时，暴露给 Agent 一个稳定的可编程接口。今天的爆量增长和 GPT-6 Sol/Luna 主打"更适合企业 Agent 场景"的定价变化几乎同步。

背后的信号是：企业级 Agent 场景里，"读懂文件"和"输出文件"是最高频的两个能力，但目前每家 Agent 框架都在各自重造轮子。Univer 押注的方向是**做一层跨 Office 应用的统一 sandbox，让所有 Agent 框架都可以用同一个 runtime 接管这些格式**。对比 Copilot、Gemini for Workspace 这类闭源方案，Univer 是目前最完整的开源等价物。

对开发者而言，这类"底层 runtime"的战略意义远高于 Prompt 模板类项目——如果 Univer 站稳，未来一大批"AI 原生表格"的初创产品会直接构建在它上面。

---

### 🥉 [anthropics/financial-services](https://github.com/anthropics/financial-services) — +665⭐

**Anthropic 官方下场做行业方案，官方 Cookbook 时代结束**

这个仓库是 Anthropic 自己维护的**金融行业 Agent 参考实现**：包含合规审查、风控问答、投研摘要、财报解析等常见工作流的完整可运行代码，全部基于 Claude Fable 5.1 与 EFS（Enterprise Frontier Safeguards）。仓库快速冲上 3.6 万星，说明企业客户在 Fable 5.1 缓存降价 75% 之后，正在**大规模尝试从 POC 迁移到生产**。

Anthropic 过去更倾向把示例放在 `anthropic-cookbook` 这类通用仓库，如今开出行业专属 repo，说明公司正在推行"半 vertical 化"战略：官方给出行业模板，第三方在其之上构建产品。这一步和它同期投资 Basecamp Research（生物医药）、Anthology Fund（Anthropic × Menlo）的动作构成一致节奏。对比 OpenAI 的"通用 API + 少量行业蓝图"策略，Anthropic 明显在往更重的**行业陪跑者**路线走。

---

### 🎬 [browser-use/video-use](https://github.com/browser-use/video-use) — +745⭐

**Coding Agent 的下一站：视频**

`browser-use` 项目原本是通过让 Agent"看屏幕操作浏览器"打开局面的，如今推出的姐妹项目 `video-use` 把同一套模式搬到了视频编辑——**让 Coding Agent 用 Python 脚本操作视频剪辑、时间线拼接、字幕生成、镜头选择**。今日暴涨 745 星背后的助推事件很明确：OpenAI Sora API 今日全面下线，一大批依赖 Sora 的开发者需要一个**"开源 + 本地跑通"** 的视频工作流替代。

`video-use` 的架构选择很聪明：它不试图和 Sora 竞争生成质量，而是抓住"**剪辑与合成的确定性任务**"——让 Agent 学会调用 ffmpeg、moviepy、Runway API、Kling API 等真实工具，而不是让模型自己生成像素。这与 Cursor、Windsurf 在代码领域的路径几乎一致：**Agent 不重造 IDE，而是把 IDE 变成它的手**。

---

### 🛠️ [obra/superpowers](https://github.com/obra/superpowers) — +485⭐

**当 29 万星的 Skills 框架成为"框架的框架"**

`superpowers` 是 Jesse Vincent 维护的 Agentic Skills 元框架——一套用来写、评估、调度 Claude Code / OpenAI Agent 使用的"Skills"的系统。29 万星的绝对量级已经让它跻身 GitHub 全球 top 30 项目之列，今天仍能挤上 trending 说明它继续保持着**社区飞轮**的增长态势。

`superpowers` 最近的关键变化是与 Anthropic 官方 Skill 体系的**双向兼容**：一个 Skill 既可以在 Claude Code、Claude API 里跑，也可以在 superpowers 的调度器里跑，甚至可以直接被打包成 MCP tool。这种"运行时无关"的 Skill 抽象正在成为 2026 秋季 Agent 生态的一个隐形共识：**Skill = 可执行的 Prompt + 工具集 + 评估集**，而不是任何一家框架的私有格式。

配套值得关注的是 `superdesigndev/treg`（+502⭐）——它把自己定位为"**Agent 工具的 OpenRouter**"，形成"Skills + 工具路由"的组合拳。整个方向已经很清晰：Agent 世界正在标准化底层构件，形成类似 Web 早期的"HTML + HTTP + DNS"三层清晰分离。

---

## 生态观察

**主题一：Agent 编排框架战争进入 2.0。** google/ax（Go, +1,542⭐）、agent-substrate/substrate（Go, +560⭐）、strands-agents/harness-sdk（Python/TS, +96⭐）、BuilderIO/agent-native（TS, +135⭐）四家同日入榜。Go 系框架的集中出现说明**平台工程社区**开始入场——Agent 编排不再只是 AI 团队的事，正被 SRE / 平台团队接管。这将极大改变 2027 年生产环境 Agent 的部署方式。

**主题二：Office / 生产力软件的"Agent 原生"重写。** univer（+1,140⭐）、CLI-Anything（+41⭐）、impeccable（+287⭐）三个方向共同指向一件事：**旧的 GUI-first 应用要么被 Agent 化，要么被替换**。Univer 的 runtime 打法可能会成为下一代 Excel / Notion 类产品的底层选择。

**主题三：Anthropic 生态持续扩张。** anthropics/financial-services（+665⭐）、davila7/claude-code-templates（+393⭐）、obra/superpowers（+485⭐）——三个不同层次的 Anthropic 相关项目同时占据前 10。Claude Code + Skills + 官方行业方案的**三段火箭**结构已经清晰，接下来是等类似 Vercel / Supabase 那样的第三方 SaaS 逐一被吸入这个生态。

**主题四：安全与代码情报成为 MCP 的第一批"杀手应用"。** mvt-project/mvt（+546⭐）和 DeusData/codebase-memory-mcp（+266⭐）分别代表移动取证和代码智能两条线。前者反映 iOS/Android Pegasus 类间谍软件的持续高发（尤其是记者、活动人士群体），后者说明 MCP 已经从"官方演示"进入"真正吃 CPU 的服务器实现"的阶段。C 语言 MCP 服务器有 44K 星，说明性能敏感的开发者已经在认真押注 MCP 协议。

**主题五：金融科技开源崛起。** Open-Dev-Society/OpenStock（+379⭐）连续在榜。当 Bloomberg Terminal / Refinitiv 每人每年 2 万美金的成本继续抬升时，开源实时行情 + AI 分析工作流的组合，正在成为 SMB 券商和量化个人的下一站选择。
