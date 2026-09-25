# GitHub Trending 日报 · 2026-09-26

## 今日焦点

> **企业级 Agent 管理平台崛起 · Google 加入开源 Agent Runtime 战场 · "Agent Memory"进入主流工具箱 · Claude Plugins 官方目录首日冲榜 · Skills 生态继续吸星**
>
> - `paperclipai/paperclip` 单日 +1,853⭐，"Agent 管理"从概念变成办公室日常工具。
> - `google/ax` 单日 +1,386⭐，Google 官方 Agent Orchestration Runtime 上线即打榜第一天。
> - `vectorize-io/hindsight` 单日 +1,652⭐，"Agent Memory that Learns" 补齐 agent runtime 最缺的一块拼图。
> - `dream-num/univer` +1,048⭐，把 Excel/Docs/Slides/PDF 装进一个 runtime，直击 Agent Office 场景。
> - `rohitg00/ai-engineering-from-scratch` +1,181⭐，AI 工程教程仍在吃"从头造车"的红利。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [paperclipai/paperclip](https://github.com/paperclipai/paperclip) | 办公室最流行的开源 Agent 管理平台 | TypeScript | 84,765 | +1,853 | 15,219 |
| 2 | [vectorize-io/hindsight](https://github.com/vectorize-io/hindsight) | 会学习的 Agent Memory | Python | 29,740 | +1,652 | 3,144 |
| 3 | [google/ax](https://github.com/google/ax) | Google 官方 Agent Orchestration Runtime | Go | 11,441 | +1,386 | 551 |
| 4 | [rohitg00/ai-engineering-from-scratch](https://github.com/rohitg00/ai-engineering-from-scratch) | 从零到部署的 AI 工程教程 | Python | 57,430 | +1,181 | 10,015 |
| 5 | [dream-num/univer](https://github.com/dream-num/univer) | Agent 版 Office 全家桶 runtime | TypeScript | 18,383 | +1,048 | 1,562 |
| 6 | [mattpocock/skills](https://github.com/mattpocock/skills) | 面向真实工程师的 Skills 合集 | Shell | 269,693 | +588 | 22,725 |
| 7 | [obra/superpowers](https://github.com/obra/superpowers) | Agent Skills 框架与研发方法论 | Shell | 291,633 | +465 | 26,108 |
| 8 | [NVIDIA/Model-Optimizer](https://github.com/NVIDIA/Model-Optimizer) | 量化/蒸馏/NAS 一体化优化库 | Python | 4,441 | +360 | 649 |
| 9 | [pbakaus/impeccable](https://github.com/pbakaus/impeccable) | 让 AI 更懂设计的语言 | JavaScript | 71,163 | +326 | 4,310 |
| 10 | [anthropics/skills](https://github.com/anthropics/skills) | Anthropic 官方 Agent Skills 仓库 | Python | 178,276 | +231 | 21,106 |
| 11 | [derv82/wifit3](https://github.com/derv82/wifit3) | 跨平台 USB-only Wifite 重写 | Python | 889 | +168 | 85 |
| 12 | [androoAGI/starnet](https://github.com/androoAGI/starnet) | 像素风桌面 Agent Harness | JavaScript | 450 | +118 | 87 |
| 13 | [kelseyhightower/kubernetes-the-hard-way](https://github.com/kelseyhightower/kubernetes-the-hard-way) | 手把手拉起 K8s 集群 | Documentation | 50,115 | +105 | 15,916 |
| 14 | [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) | Anthropic 官方 Claude Code 插件目录 | Python | 36,898 | +62 | 4,152 |
| 15 | [shy3130/tick-stock-panel](https://github.com/shy3130/tick-stock-panel) | 集成 LLM 的中文股票量化面板 | Python | 5,120 | +31 | 1,253 |

---

## 重点项目点评

### 🥇 [paperclipai/paperclip](https://github.com/paperclipai/paperclip) — 今日榜首，+1,853⭐

**"Agent 管理"从 Slack 群工具变成开源 SaaS 级平台**

Paperclip 是一个 TypeScript 单体，主打"公司内部的 agent 统一管理台"：企业员工可以在里面注册自己训好的 agent、给同事共享 workflow、把 agent 请进 project space 参与协作。今日单日新增 1,853 颗星，累计突破 8.4 万，是最近三个月增速最猛的企业级 AI 平台之一。它的走红踩中了 Dataiku 昨天刚发布 Agent Management 的时点，同期 Anthropic 也宣布 Accenture 加入其安全评估体系——**"Agent 治理"正在成为 2026Q4 最热的企业软件品类**。

Paperclip 的独特之处是它做了非常干净的 workspace 抽象：一个 agent = 一个 pull request-able 单元，可以走 review 流程、可以按角色分权限、还能挂 audit log。GitHub 星星涨得最快的是它上周新加的 "Agent-of-Agents" 编排模式——用一个 orchestrator agent 去 review 下属 agent 的输出，构建"多层 QA"。这与 Claude 5.5 声称的 26% 自动化研发比例形成呼应：**Agent 不再是单点工具，而是可编制的团队成员**。

对比商业替代品（Salesforce Koa、Microsoft Copilot Studio），Paperclip 的开源身位让它在 self-hosted 场景内几乎零竞争，这也是它能在企业 IT 圈子里病毒式传播的核心原因。

---

### 🥈 [google/ax](https://github.com/google/ax) — +1,386⭐

**Google 亲自下场做 Agent Runtime，Go 生态首次拥有"官方"版 orchestrator**

`google/ax` 是 Google 昨晚开源的 Agent Orchestration Runtime，Go 实现，深度集成 Gemini + 任意 OpenAPI 工具。虽然只有 1.1 万星，但今天单日 +1,386，且 forks 已经过 500——**开源速度快得罕见，是本季度 Google 除了 Vertex AI SDK 之外最大的一次开源投入**。

Ax 的架构文档里透露了不少东西：它按 Google 内部 Bard/Gemini agent runtime 的架构复刻，走 event-loop + tool-driver + state store 三段式，天然支持长任务恢复、多 agent 合作、以及 hyper-parallel tool execution。它的核心差异化是"in-band eval"：每个 tool call 都可以内联一段 eval prompt，让 orchestrator 决定是否 rollback——这与 Anthropic Claude Code 的做法思路一致，说明 orchestrator 层的最佳实践正在收敛。

Go 生态之前的 agent runtime 选择寥寥（langchaingo、eino），Google 亲自入场几乎立即改变格局。如果 Ax 能吃到 CNCF 的分发效应，未来 6 个月它可能取代 Python 版 LangGraph 成为 kubernetes-native agent 部署的默认选择。

---

### 🥉 [vectorize-io/hindsight](https://github.com/vectorize-io/hindsight) — +1,652⭐

**"Agent Memory that Learns"——把 agent 的失误变成参数，长期学习不再依赖 fine-tune**

Hindsight 定位很直接：给 agent 补一层可持续学习的 memory。区别于传统 vector memory 的"存 + 查"，Hindsight 会在每次任务结束后跑一段 self-critique，把"这次哪里做错了/哪里做对了"结构化写回 memory，同时更新一个"决策倾向"的权重表。下一次遇到相似 context 时，agent 优先复用带正向权重的经验，反面案例则作为 few-shot 反例注入 prompt。

这个思路并不新（AutoGPT 时代就有），但 Hindsight 的工程实现足够克制：只用 SQLite + 一个 Python 服务，可以嵌入任何 LangGraph / OpenAI Assistants / Claude Code 环境。今天 1,652 的单日增星意味着社区终于承认——**"记忆"是 agent 从 demo 走向生产的必需品**，而"每晚 fine-tune 一次"这条路对 90% 的团队都不现实。

值得一提的是，Hindsight 的作者团队原本来自 Vectorize，公司主打 RAG-as-a-service。这个项目开源后，vector search 市场正在被迫从"检索"扩展到"经验管理"——一个新品类正在成形。

---

### 🏅 [dream-num/univer](https://github.com/dream-num/univer) — +1,048⭐

**把 Office 装进 Agent Runtime：中国团队做出的"Agent 版 WPS"**

Univer 由中国团队 dream-num 主导，用 TypeScript 实现了一个统一 runtime，覆盖 Spreadsheet、Docs、Slides、Canvas、PDF、Relational Table。今日高速上榜的原因是最新版本正式支持 "Agent Runtime" 模式：agent 可以像人一样打开一个工作簿、编辑单元格、跑公式、导出 PDF；所有操作都是 event-based，可以被 replay、审计、rollback。

比起把 agent 塞进 SaaS 的做法，Univer 走的是"给 agent 造工具"这条路——它意识到 agent 需要的不是"我调用 Excel API"，而是"我拥有一整个 Office 环境"。这与本周 Anthropic Skills、Google Ax、Paperclip 的方向一致，即**agent 的能力边界正在从 API 调用扩展到"完整 workspace 操作"**。

对开源社区的意义是：多年来"WebOffice"品类几乎被商业闭源方案垄断，Univer 是第一款既完成产品化、又完成 agent 化的开源基座。可以预见接下来 6 个月，会看到大量基于 Univer 的垂类 SaaS 出现。

---

### 📘 [rohitg00/ai-engineering-from-scratch](https://github.com/rohitg00/ai-engineering-from-scratch) — +1,181⭐

**"从头造车"的教程仍然吃香，反映初学者对"知其所以然"的渴望**

Rohit Gupta 的教程仓库覆盖从 tokenizer、attention 到 RAG、agent、eval 的端到端 Python 实现，全部不依赖商业框架。它今天 +1,181 的关键是新加了一章 "从零实现 Agent Runtime"，与 Google Ax、Paperclip 的走红形成话题联动。

这类"重复造轮子式教程"往往有一个悖论：越是 SaaS 化的时代，越有一批工程师需要理解底层。当前 AI 圈的另一侧是"unbundled AI"叙事——把 API 拆开、把框架推翻、亲手写一遍再上生产。这个 repo 在此氛围下继续增长，说明**AI 工程正在从"套 SDK"进入"读 spec"阶段**。

对企业招聘的隐含意义：面试题正在从"你用过 LangChain 吗"回归到"你能实现一次自回归采样吗"。

---

## 生态观察

**主题一：Agent 治理与运行时"双爆发"。** Paperclip、Google Ax、Univer、Hindsight 四大热门项目共同指向同一个趋势——**agent runtime 正在从概念走向企业标配**。管理平台（Paperclip）、编排层（Ax）、记忆层（Hindsight）、工具层（Univer）四层拼图今天几乎在同一天亮相。

**主题二：Skills 系统仍在吸星，但增速放缓。** obra/superpowers、mattpocock/skills、anthropics/skills 三个大项目累计已超 70 万星，但单日增速较 8 月峰值下降近 60%。这暗示"Skills"作为分发单位可能已经过了叙事峰值，接下来的战场是"Skills 的编排"，而非"Skills 的数量"。

**主题三：Google 开源速度上台阶。** 从 Gemma、A2A protocol、到今天的 Ax，Google 在 Agent 时代拿出了远比 Google Brain 时代更激进的开源姿态，明显是为了在 model + runtime 双线堵住 Anthropic 与 OpenAI 的入口。

**主题四：中国 AI Infra 项目走出小众圈子。** Univer 与 tick-stock-panel 同日上榜说明"中文 AI infra"的品牌溢价正在形成，海外开发者对中国团队的技术深度不再抱刻板印象，这是过去三年首次。

---

*报告日期：2026-09-26 · 数据快照：github.com/trending 早间抓取*
