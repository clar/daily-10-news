# GitHub Trending 日报 · 2026-09-12

## 今日焦点

> **AI 沟通反抗（ADHD skill）· OSINT 全球态势平台开源 · Agent 方法论走向"技能库" · 桌面级本地代码 Agent · 中国系数学 Agent 项目跑上榜**
>
> - `ayghri/i-have-adhd` +3,440⭐：一个"让 AI 别废话"的 skill 意外爆红，说明"话痨 assistant"已经成社区痛点
> - `bilawalsidhu/gods-eye-view` +3,642⭐：民用 OSINT 三维态势平台上线即冲榜，公共数据可视化门槛被拉低
> - `github/spec-kit` +985⭐：GitHub 官方"规格驱动开发"工具持续加热，总星数破 13.5 万
> - `obra/superpowers` +731⭐：Agent skills 框架跨越 28 万星，agent 开发方法论正在标准化
> - `jihe520/MathModelAgent` +132⭐：数学建模自动化 Agent，中国大学生赛季"科研自动化"应用抬头

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [bilawalsidhu/gods-eye-view](https://github.com/bilawalsidhu/gods-eye-view) | 3D 地球 · 实时航班/船舶/卫星/火点/摄像头 OSINT 面板 | JavaScript | 26,955 | +3,642 | 5,513 |
| 2 | [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) | 让 Claude/Cursor 少说废话的 skill 插件 | Python | 41,608 | +3,440 | 2,356 |
| 3 | [github/spec-kit](https://github.com/github/spec-kit) | GitHub 官方 spec-driven 开发工具集 | Python | 135,743 | +985 | 12,199 |
| 4 | [obra/superpowers](https://github.com/obra/superpowers) | Agent skill 框架（TDD / 计划 / 评审全流程） | Shell | 285,339 | +731 | 25,515 |
| 5 | [nashsu/llm_wiki](https://github.com/nashsu/llm_wiki) | 桌面 App，将文档转成个人知识库 | TypeScript | 18,701 | +640 | 2,134 |
| 6 | [alsk1992/CloddsBot](https://github.com/alsk1992/CloddsBot) | 跨 1000+ 市场自动化交易 Agent | TypeScript | 2,116 | +627 | 280 |
| 7 | [vastsa/PI-Desktop](https://github.com/vastsa/PI-Desktop) | Electron+Rust 本地 AI 代码 Agent 桌面端 | TypeScript | 2,759 | +545 | 216 |
| 8 | [armory3d/armorpaint](https://github.com/armory3d/armorpaint) | 3D 纹理绘制工具 | C | 4,708 | +354 | 533 |
| 9 | [Sonarr/Sonarr](https://github.com/Sonarr/Sonarr) | 电视剧 PVR 智能管理（Newsgroups + BT） | C# | 15,720 | +174 | 1,948 |
| 10 | [alphaXiv/OpenResearch](https://github.com/alphaXiv/OpenResearch) | 多模型并行的研究 Agent | Rust | 1,250 | +156 | 91 |
| 11 | [jihe520/MathModelAgent](https://github.com/jihe520/MathModelAgent) | 数学建模自动化 Agent | Python | 4,844 | +132 | 392 |
| 12 | [melgarafael/DeskcommCRM](https://github.com/melgarafael/DeskcommCRM) | 自托管 CRM · AI Agent + WhatsApp 集成 | TypeScript | 1,308 | +126 | 492 |
| 13 | [jordan-gibbs/hyperresearch](https://github.com/jordan-gibbs/hyperresearch) | Agent 驱动的研究知识库与综述工具 | Python | 2,557 | +118 | 257 |
| 14 | [pascalorg/editor](https://github.com/pascalorg/editor) | 开源 3D 建筑编辑器 · 支持 CLI 与 MCP | TypeScript | 23,564 | +83 | 2,939 |
| 15 | [nab138/iloader](https://github.com/nab138/iloader) | 用户友好的 iOS 侧载工具 | TypeScript | 2,891 | +36 | 201 |

---

## 重点项目点评

### 🥇 [bilawalsidhu/gods-eye-view](https://github.com/bilawalsidhu/gods-eye-view) — 今日榜首，+3,642⭐

**民用 OSINT 平台从"YouTube 视频"变成"每个人都能跑的实时地球仪"**

Bilawal Sidhu（Google 前产品经理、"WorldView" YouTube 系列 500 万 + 播放）与 Sameh Khamis 联合放出的开源三维地球态势平台，一次性集成了实时航班（ADS-B）、船舶（AIS）、卫星（TLE）、地震、火点、公开摄像头等公开数据源，界面模仿情报中心指挥室——同时接入 OpenAI Realtime API，允许用户"用嘴指挥地球仪"锁定物体、切换热成像/夜视等传感器模式。

它今天爆火的意义不在于技术难度（各个数据源都是可获取的），而在于两点：一是把"专业 GEOINT 平台"（Palantir Metropolis / Maxar SecureWatch）的核心用户体验用 JavaScript + 免费公共 API 重新做了一遍，把行业门槛砍到"运行一个 npm dev"；二是背后有一家新公司 Halfpixel 在做托管版——**"YouTube 出圈 → 开源代码涌流 → 商业化托管"** 已经成为 2026 年 vibe-driven 项目的标准路径。

同时今天 EPA 数据中心听证、Anthropic 蒸馏报告都在 HN 头条——公共数据 + 三维可视化，是社会舆论对不透明基础设施的一种直接反抗工具。

---

### 🥈 [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) — +3,440⭐

**社区的沉默抗议：AI 助手请少说废话**

一个只做一件事的 skill：给 Claude/Cursor/Gemini 装上后，强制它 action-first、去掉 "Great question!" 之类的开场白、去掉结尾的 tangential 建议、给出可量化时间估算。作者用 before/after 例子直接对比，把大家平时"AI 越来越啰嗦"的隐性不满转成了可安装的插件。

一天涨 3440 星、总星数上 4.1 万，说明这个不满已经不是小众——它对应的正是 [HN 榜 🥇 数学 AI 帖](https://news.ycombinator.com/item?id=49662371) 里那句话的镜像："AI 给出答案的方式抽空了对话本身的价值"。**当 assistant 变成默认"话痨 + 免责声明机器"，用户会用一个 3KB 的 markdown 文件把它治回去**。这个项目的市场信号是：Claude / Cursor / Copilot 的默认输出风格调优，正在被社区反向定义。

对 Anthropic / OpenAI：如果这类"反 slop skill"继续爆红，官方系统 prompt 需要重构。

---

### 🥉 [github/spec-kit](https://github.com/github/spec-kit) — +985⭐

**GitHub 官方"规格驱动开发"越滚越大，13.5 万星逼近全站前 20**

spec-kit 是 GitHub 官方推出的 spec-driven development 工具集，配合 Copilot Agent Mode 使用，用规格文档来驱动 AI 完成实现——类似"先写严格的 PRD/契约，再让 Agent 逐段实现并回滚"。今天新增 985 星只是常态化增长，但总星数达到 135,743，是过去一个月增速最稳的官方项目之一。

它反映的是 2026 下半年很清楚的一个转向：**"prompt-first" → "spec-first"**。Cursor、Aider、Cline、Cody 都往这个方向走，obra/superpowers 也是同一叙事。GitHub 借官方地位把这个范式变成了默认设置。对企业买家来说，spec-kit 的进展将直接决定 GitHub Copilot Enterprise 在下一季度的 upsell 说服力。

---

### 🤖 [obra/superpowers](https://github.com/obra/superpowers) — +731⭐

**Agent 开发方法论走向"技能库"，star 数已破 28 万**

Prime Radiant 的 Jesse Vincent（obra）主导的 Agent 方法论仓库：一整套 composable "skills"，覆盖测试驱动、系统化调试、设计澄清、计划评审、并行开发。它在多个 Agent 平台（Claude、Cursor、Devin、Gemini）中即插即用，通过 context 自动触发。

28 万星是极高数量——对比一下，同类的官方 spec-kit 才 13.5 万。obra/superpowers 的走红意味着 **agent 开发不再是"提示词工程"，而是"技能仓库工程"**：一批具备"编排+回顾+测试"的 primitives 会成为 agent 生产环境的操作系统层。跟今天的 `i-have-adhd`（一个反向 skill）一起看，社区的 skill 生态已经开始出现"官方 vs 反官方"两派—— 生态开始成熟的信号。

---

### 🎓 [jihe520/MathModelAgent](https://github.com/jihe520/MathModelAgent) — +132⭐

**中国大学生赛季来了：数学建模 Agent 冲上 4844 星**

MathModelAgent 是一个自动化数学建模流程的 Agent：接入文献检索、数据处理、模型选择、Python 数值计算、报告写作，完成美赛/国赛式题目的全流程。今日新增 132 星并不惊人，但总星数已达 4844 且长期在 trending 榜上——契机很明确：每年 9 月是"中国大学生数学建模竞赛"报名与备赛高峰，10-11 月出成绩。

这个项目的存在本身，与今日 [HN 头条数学家反弹 AI](https://news.ycombinator.com/item?id=49662371) 构成的对比很有意思：**学院派数学家担心 AI 抽空数学理解的价值，而工程/应用侧数学早就大规模自动化了**。这个断层未来会持续扩大，学术与工程社区对"AI 与数学"的态度将进一步分化。

---

## 生态观察

- **Agent 分层完成**：过去一年榜单常见"AI Agent 框架 + demo"，今天上榜的清一色是三层——**方法论（superpowers / spec-kit）→ 领域 Agent（Math / OpenResearch / hyperresearch / CloddsBot）→ 反 slop 治理（i-have-adhd）**。生态开始有分工。
- **OSINT + 三维可视化爆发**：gods-eye-view 的 3600+ 涨星意味着"公开数据可视化"从利基走向大众，随之而来的是 GDPR / 反监控话题在明年上升。
- **本地代码 Agent 桌面端起来**：PI-Desktop（Electron+Rust）+545 星，nashsu/llm_wiki +640 星，都指向"我不想再把代码 + 文档给云"的心态。数据主权类项目在缓慢积累势能。
- **传统项目仍有稳定水位**：Sonarr（+174）、armorpaint（+354）说明 GitHub trending 里"实用工具"从未被 AI 完全挤出。
- **中国系项目继续保持有效供给**：MathModelAgent、nashsu/llm_wiki、vastsa/PI-Desktop，三条不同赛道稳定输出。跟 Anthropic 蒸馏报告叙事同框看，中国开发者面对的舆论压力与生产力势能是同时上升的。
