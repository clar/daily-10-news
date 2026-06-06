# GitHub Trending 日报 · 2026-06-07

## 今日焦点

> **Agentic skill 框架霸榜 · Agent 记忆系统进生产 · 开源 NotebookLM 升温 · 多平台 agent 阅读器 · 语音/OCR 老兵继续吸星**
>
> - `obra/superpowers` 今日 **+1,008⭐**，agentic skill 框架登顶，把"工程方法论 + skill 包"做成可分发资产。
> - `lfnovo/open-notebook` **+783⭐**，开源 NotebookLM 因 vibe-research 趋势再度爆发。
> - `Panniantong/Agent-Reach` **+700⭐**，让 agent 一键读 Twitter/Reddit/YouTube/GitHub/Bilibili。
> - `CopilotKit/CopilotKit` **+613⭐**，"agent 前端栈"在 React/Angular/Mobile 全平台铺开。
> - `MemPalace/mempalace` **+441⭐**，主打 benchmark 第一的开源 agent 长期记忆系统。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic skill 框架与软件开发方法论 | Shell | 219,615 | +1,008⭐ | 19,540 |
| 2 | [lfnovo/open-notebook](https://github.com/lfnovo/open-notebook) | 开源版 NotebookLM，更高自由度 | TypeScript | 26,571 | +783⭐ | 3,035 |
| 3 | [Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach) | 让 agent 跨平台读取与搜索社媒/视频/代码 | Python | 22,271 | +700⭐ | 1,903 |
| 4 | [CopilotKit/CopilotKit](https://github.com/CopilotKit/CopilotKit) | Agent 与生成式 UI 的前端栈 | TypeScript | 33,173 | +613⭐ | 4,237 |
| 5 | [PaddlePaddle/PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR) | 多语言 PDF/图像 → 结构化数据 OCR | Python | 80,941 | +449⭐ | 10,655 |
| 6 | [MemPalace/mempalace](https://github.com/MemPalace/mempalace) | 基准最强的开源 agent 长期记忆 | Python | 54,247 | +441⭐ | 7,107 |
| 7 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 跨 Reddit/X/YT/HN/Polymarket 的研究 agent | Python | 28,740 | +441⭐ | 2,434 |
| 8 | [microsoft/VibeVoice](https://github.com/microsoft/VibeVoice) | 微软开源前沿语音 AI | Python | 48,451 | +219⭐ | 5,389 |
| 9 | [santifer/career-ops](https://github.com/santifer/career-ops) | 14 种 skill 模式的 AI 求职系统 | JavaScript | 49,283 | +203⭐ | 10,194 |
| 10 | [aquasecurity/trivy](https://github.com/aquasecurity/trivy) | 容器/K8s/代码/云的安全扫描 | Go | 35,992 | +159⭐ | 454 |
| 11 | [openai/whisper](https://github.com/openai/whisper) | 大规模弱监督语音识别 | Python | 101,829 | +155⭐ | 12,439 |
| 12 | [vitejs/vite](https://github.com/vitejs/vite) | 下一代前端工具链 | TypeScript | 81,166 | +73⭐ | 8,274 |
| 13 | [nginx/nginx](https://github.com/nginx/nginx) | 官方 NGINX 仓库 | C | 30,673 | +37⭐ | 7,956 |
| 14 | [sveltejs/svelte](https://github.com/sveltejs/svelte) | 给大众的 web 开发 | JavaScript | 86,964 | +34⭐ | 4,937 |
| 15 | [golang/go](https://github.com/golang/go) | Go 编程语言 | Go | 134,497 | +24⭐ | 19,089 |

---

## 重点项目点评

### 🥇 [obra/superpowers](https://github.com/obra/superpowers) — 今日榜首，+1,008⭐

**Agentic skill 第一次以"工程方法论"姿态登顶 Trending**

`superpowers` 把 skill 不再当成"prompt 模板"，而是一整套包含目录规范、调用约定、子流程契约和实例脚本的 **agentic 工程方法论**。仓库定义了 skill 之间如何串联、如何与 agent 主循环交互、如何让人类工程师审查 skill 输出。配套的 Shell 工具链直接对接 Claude Code、Codex 与 OpenDev 等多端 agent runtime。

它今日新增 1,008 星，恰逢 Anthropic 公开"递归自我改进"白皮书与微软 Build 2026 集体 push agent 工程化。市场需要一个比"prompt + tools"更高层的抽象，把 agent 行为变成可治理、可复用的资产；`superpowers` 押的是这个赛道。值得注意它已经累计 21.9 万星，这是 trending 上极少见的"巨头量级 + 仍在加速"组合，意味着社区认为 skill 工程化的窗口刚刚打开。

---

### 🥈 [lfnovo/open-notebook](https://github.com/lfnovo/open-notebook) — +783⭐

**Vibe-research 的复兴让开源 NotebookLM 二次起飞**

这是开源版的 Google NotebookLM，但在 RAG 层面更模块化：支持自定义 embedding、混合检索、引用回溯，以及把 notebook 嵌入到 agent 工作流里作为长期上下文。它最近一周冲到 26.5K 星，跟今天 HN 主站"Ask HN：你的 GenAI 卧槽时刻"长帖中"用 NotebookLM 做研究是真破圈"的讨论高度相关。

值得关注的是它今天选择把"deep research"流水线也内置进去——把搜索、抓取、清洗、引用打包成一个 notebook lifecycle，跟主力 agent 框架解耦。这种"研究型 notebook + agent 长期记忆"组合正在成为去年 RAG 框架（如 LangChain、LlamaIndex）的下一代替代品。

---

### 🥉 [Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach) — +700⭐

**多平台社媒抓取层在 agent 时代再度走红**

Agent-Reach 让 agent 一次性"读懂" Twitter/X、Reddit、YouTube、GitHub、Bilibili——以统一接口暴露 search、read、subscribe 三类原语，并解决了各家越来越严格的反爬与登录态问题。代码量不大，但因为把"5 个平台 × 三种使用模式"打包成一套 MCP server，今天直接被多个 agent 项目当依赖引入。

在 X API 涨价、Reddit 收紧、YouTube 数据 limit 越来越严的当下，这类"统一阅读层"对 agent 开发者具备显著的 ROI——单一仓库吃掉本来要写六遍的 scraper。这与 #7 `last30days-skill`（跨平台 30 天研究 agent）形成上下游配合。

---

### 🛠️ [CopilotKit/CopilotKit](https://github.com/CopilotKit/CopilotKit) — +613⭐

**Agent UI 层第一次跨出"chat 框"，赢得多端覆盖**

CopilotKit 把 agent 不再只当作侧栏的 chat，而是定义了 generative UI 的组件原语：表单、Kanban、表格、向导都可以由 agent 在运行时生成、修改、订阅状态变化。最新版本覆盖 React、Angular、移动端 RN、甚至 Slack 内置 UI，这种"agent UI 多端发行"格局在前端社区还是少见的。

今天的加速度跟 Microsoft Build 2026 公开演示"agent-first UI"思路高度同步——VS Code、Office、Teams 都被改造成 agent 驱动的工作流。CopilotKit 是当前 OSS 阵营里最完整的"前端栈替代品"，明显在试图把自己装进新一代 SaaS 启动模板。

---

### 🧠 [MemPalace/mempalace](https://github.com/MemPalace/mempalace) — +441⭐

**"基准最强"的 agent 长期记忆系统进入工程化阶段**

mempalace 主打的不是 vector DB，而是 **agent 行为日志 + episodic memory + skill 关联记忆** 三层组合，并发布了对比 mem0、letta、Zep 的公开 benchmark。今天的 441 星增速来自其 v0.4 版本默认开启"latent compression"，把 30 天会话压成不到 1MB 的可回放摘要，对生产环境极有吸引力。

这一波 trending 把 "memory" 与 "skill"（榜首的 superpowers）放到同一天，事实上构成了 agent 工程化的两根支柱：**skill 给能力组合，memory 给状态延续**。当各家都在卷 agent runtime 时，谁能率先把 skill + memory 标准化，就有机会成为下一个 LangChain 级别的事实标准。

---

## 生态观察

今天的 Trending 榜呈现一个**集中的主题**：agent 工程化。前 7 个榜位里有 6 个直接服务 agent 栈——skill 框架（superpowers）、agent UI（CopilotKit）、agent 多平台阅读（Agent-Reach、last30days-skill）、agent 记忆（mempalace）、agent 原生 notebook（open-notebook）。这与 Build 2026 + Anthropic IPO + Salesforce 案例这一周的产业叙事完全一致：开发者正在快速搭出 **skill / memory / UI / 工具接入** 这四层基础设施。

另一头是传统底层项目的稳定脚步：PaddleOCR、Whisper、Vite、Go、NGINX、Svelte 都在榜单里"低速但常驻"——这是 agent 浪潮真正消化掉的能力（OCR、ASR、前端构建）的源头。把今天的榜单分成"agent 化基础设施 + 经典底座"两层来看，叙事是非常清晰的：基础设施层在野蛮生长，经典层在稳定供给。

下一个会先卷出来的位置：**agent 评估/可观测**。今天 trending 里还没出现 "agent eval/observability" 类目的爆款，但 HN 与产业新闻里 Coralogix 拿 2 亿美元已经把信号亮起。下一周这个赛道的 OSS 项目大概率冲榜。
