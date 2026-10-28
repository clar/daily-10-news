# GitHub Trending 日报 · 2026-10-29

## 今日焦点

> **Agent Skills 继续吃榜 · AI 原生 IDE / 工作区井喷 · 设计系统进入"反模板"阶段 · WiFi 感知爆红 · 中国网盘生态持续活跃**
>
> - `obra/superpowers` 这类"Agent Skills 方法论"仓库继续顶住 30 万+ 星基本盘，每日仍能收 1,000+⭐。
> - `Nutlope/hallmark` 与 `pbakaus/impeccable` 两个"反 AI 风味 UI"的设计 skill 同时上榜。
> - `JetBrains/thinkrail` 作为 JetBrains 的新 AI 原生 IDE 发布第一天即进入前列。
> - `ruvnet/RuView` 用 WiFi 信号做人体感知的开源项目再度冲榜，代表非摄像头传感的持续热度。
> - `nightly-labs/openbot` 一类"本地 Agent 工作区"打包了 Codex / Claude / Grok，Agent 多后端融合正在成为新品类。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [JetBrains/thinkrail](https://github.com/JetBrains/thinkrail) | AI 原生轻量 IDE，可自适应开发流 | TypeScript | 4,986 | +1,075⭐ | 254 |
| 2 | [elayadesign/ai-design-skills](https://github.com/elayadesign/ai-design-skills) | 面向编码 Agent 的设计 skill 集合 | — | 11,037 | +1,938⭐ | 790 |
| 3 | [obra/superpowers](https://github.com/obra/superpowers) | Agent skill 方法论框架 | Shell | 307,390 | +1,096⭐ | 27,345 |
| 4 | [HKUDS/DeepTutor](https://github.com/HKUDS/DeepTutor) | 终身学习个性化 AI 导师系统 | Python | 47,872 | +2,376⭐ | 5,941 |
| 5 | [macro-inc/macro](https://github.com/macro-inc/macro) | 整合邮件/文档/CRM 的共享 AI 记忆团队工作区 | Rust | 5,386 | +106⭐ | 518 |
| 6 | [Nutlope/hallmark](https://github.com/Nutlope/hallmark) | 让编码 Agent 产出不"generic AI 味"的设计 skill | CSS | 40,628 | +2,109⭐ | 2,108 |
| 7 | [pbakaus/impeccable](https://github.com/pbakaus/impeccable) | 编码 Agent 的 UI 质量复核设计词汇表 | Rust | 92,501 | +1,471⭐ | 5,469 |
| 8 | [makecindy/cindy](https://github.com/makecindy/cindy) | 开箱即用的开源 AI Agent | TypeScript | 8,043 | +740⭐ | 940 |
| 9 | [nightly-labs/openbot](https://github.com/nightly-labs/openbot) | 本地桌面 Agent 工作区，支持 Codex/Claude/Grok | TypeScript | 3,191 | +1,053⭐ | 313 |
| 10 | [togg53192-cmd/jailbreaks](https://github.com/togg53192-cmd/jailbreaks) | 作者汇总的全部 LLM 越狱 prompt | — | 7,018 | +1,478⭐ | 1,007 |
| 11 | [hmjz100/LinkSwift](https://github.com/hmjz100/LinkSwift) | 从 8 家国内网盘提取直链下载 | JavaScript | 34,414 | +1,380⭐ | 2,432 |
| 12 | [expo/skills](https://github.com/expo/skills) | 面向 Expo 项目的 Agent skill 集 | Shell | 3,543 | +216⭐ | 224 |
| 13 | [ruvnet/RuView](https://github.com/ruvnet/RuView) | WiFi 信号做空间感知/生命体征监测 | Rust | 100,980 | +596⭐ | 13,158 |
| 14 | [xiaolai/the-craft-of-selfteaching](https://github.com/xiaolai/the-craft-of-selfteaching) | 自学工程方法论的中文 Jupyter 教材 | Jupyter Notebook | 18,472 | +295⭐ | 17,883 |

---

## 重点项目点评

### 🥇 [HKUDS/DeepTutor](https://github.com/HKUDS/DeepTutor) — +2,376⭐

**从"AI 聊天"到"AI 导师"的方法论级尝试**

DeepTutor 的目标不是再做一个 chatbot，而是把"长期学习路径 + 个性化诊断 + 多轮知识追踪"做成一个开源框架，用户的学习档案跨会话持续保存。这正好对标最近教育赛道两条互相竞争的叙事——"**AI 老师替代课堂**" vs "**AI 老师辅助老师**"：DeepTutor 把宝押在后者，更像是 Khanmigo 风格的组件化开源版本。社区关心的核心其实是数据层——学习档案到底是本地的、SQLite 的，还是云端的；港城大团队目前采用的是本地文件 + 可选云同步，这对自建教育实验平台的用户来说是刚需。

### 🥈 [Nutlope/hallmark](https://github.com/Nutlope/hallmark) — +2,109⭐

**反"AI 味"UI：设计系统进入 Agent-aware 时代**

Hallmark 的切入点很犀利：所有编码 Agent 默认产出的 UI 都带着一股"模板味"（圆角 + 柔和渐变 + glass morphism），hallmark 把一组设计语言、组件约束和"审美拒绝清单"打包成 skill，让 Agent 在生成界面时主动绕开这些模板。它和 `pbakaus/impeccable` 组成了今日榜单上两个最鲜明的"反模板"信号。这其实回答了社区过去几个月的一个担忧：**Agent 规模化输出 UI 的最大问题不是不像，而是太像**。设计系统正在从"规范"演变为"反规范"——用来让 Agent 产出有差异化的东西。

### 🥉 [JetBrains/thinkrail](https://github.com/JetBrains/thinkrail) — +1,075⭐

**JetBrains 发布的 AI 原生轻量 IDE，第一天就冲榜**

Thinkrail 不是传统 JetBrains IDE 的插件，而是**另起炉灶的轻量壳**：以 Agent 对话 + 多后端 LLM 为中心，再把 JetBrains 擅长的代码索引 / 重构能力嵌进去。TypeScript 作为主语言、容量小、启动快，是 JetBrains 对 Cursor / Zed / Windsurf 的直接回应。社区讨论的热点：**JetBrains 这是在革自己 IDE 的命，还是在给旗舰 IDE 做"外延"？** 从仓库的 roadmap 和 PR 密度看，更像前者——"轻 IDE + 深度 Agent"将成为 JetBrains 2026 新战线。

### 🏭 No.4 · [obra/superpowers](https://github.com/obra/superpowers) — +1,096⭐

**30 万⭐ 的 Agent 方法论，仍能保持每天 1,000+⭐ 的进榜**

Superpowers 已经成为 Agent Skill 的"方法论级事实标准"——30+ 万⭐ 的仓库每天仍能新增 1k⭐ 本身就是生态现象。它的价值在于把"skill 命名约定 + skill 调度流程 + 可组合性"写成了一套可以直接 fork 的目录结构，很多公司内部的 agent 配置都是从这个结构开始改的。它和榜单上 `elayadesign/ai-design-skills`、`expo/skills`、`Nutlope/hallmark` 的流行实际上是同一现象的放大：**skill 已经取代 prompt-template 成为新一代 Agent 组件格式**。

### 📡 No.5 · [ruvnet/RuView](https://github.com/ruvnet/RuView) — +596⭐

**非摄像头传感的开源化：WiFi 信号做人体感知**

RuView 把 Wi-Fi CSI 信号的"人体感知 / 心跳监测 / 存在检测"做成了一个 Rust 库 + 可部署样板，隐私叙事和开源硬件复兴叠加之后冲到 10 万⭐。它代表的是一类新的"**非摄像头 CV**"：不用镜头、不采集图像、但能知道空间里有没有人、呼吸频率是否正常。这对医疗、养老、安防场景的意义比 CV 本身更大——因为合规门槛显著降低。社区目前最大的争议是"Wi-Fi 感知的隐私问题会不会比 CV 更难说清"：你可以关掉摄像头，但很难关掉 Wi-Fi。

---

## 生态观察

- **Agent Skills 已经是独立品类**：从 `superpowers`、`ai-design-skills`、`hallmark`、`impeccable`、`expo/skills` 到 `openbot`，skill 几乎垄断了今日榜单——Agent 组件化已经完成从"提示词"到"skill 包"的迁移。
- **"反 AI 风味"设计崛起**：Hallmark / Impeccable 把 Agent 产出的"模板味 UI"视为问题，这是过去一年 Agent 落地 UI 积累的真实痛点。
- **本地 Agent 工作区在抢夺"桌面入口"**：Openbot、Cindy、Macro 三个仓库各自定位不同，但都在抢同一件事——"**本地那一层聚合所有后端 Agent 的 UI/数据**"。
- **非 CV 传感 + 开源硬件延续热度**：RuView 继续冲榜，与过去几周 Hadrian / Instrumental / The Grid 的硬件复兴叙事呼应。
- **中文开发者仓库稳定输出**：`LinkSwift`、`the-craft-of-selfteaching` 常驻榜单，代表 GitHub Trending 的中文用户基本盘仍然稳固，网盘 / 教育 / 工具类是常青赛道。
- **"越狱"类仓库再度上榜**：`jailbreaks` 这类项目回榜，说明模型安全策略的收紧已经触发社区的对抗性回潮，Agent 安全评测将是下一个热点。
