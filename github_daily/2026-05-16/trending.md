# GitHub Trending 每日热榜 · 2026-05-16

## 今日焦点

> **Agent Skills 生态全面爆发 · 个人 AI 助理本地化 · WiFi 信号空间智能 · Anthropic 工具链占据 5 席 · 端侧 TTS / 视频理解齐发力**
>
> - `mattpocock/skills` 一日 +3,155⭐，前端教父把 `.claude/` 目录开源即上榜首
> - `obra/superpowers` 累计 19 万⭐ 仍单日 +1,646，Agentic 开发方法论事实标准化
> - `tinyhumansai/openhuman` +1,272⭐，"Memory Tree" 把 118+ SaaS 同步进本地 SQLite，挑战 ChatGPT/Claude 的云端默认
> - `ruvnet/RuView` +1,865⭐，无摄像头 ESP32 WiFi CSI 测呼吸心率，端侧隐私传感新方向
> - `anthropics/skills` & `K-Dense-AI/scientific-agent-skills` 同日大涨，"Skills"作为 Claude SDK 一等公民已被产业接管

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [mattpocock/skills](https://github.com/mattpocock/skills) | Skills for Real Engineers，来自 .claude 目录 | Shell | 84,740 | +3,155 | – |
| 2 | [ruvnet/RuView](https://github.com/ruvnet/RuView) | WiFi 信号空间智能 / 生命体征监测 | Rust | 57,351 | +1,865 | – |
| 3 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic skills 框架与开发方法论 | Shell | 192,686 | +1,646 | – |
| 4 | [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) | 私有本地 AI 超级助理，Memory Tree 架构 | Rust | 8,897 | +1,272 | – |
| 5 | [supertone-inc/supertonic](https://github.com/supertone-inc/supertonic) | 端侧 ONNX 多语种闪电 TTS | Swift | 5,946 | +712 | – |
| 6 | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) | 科研 / 工程 / 金融现成 Agent Skills | Python | 22,369 | +643 | – |
| 7 | [anthropics/skills](https://github.com/anthropics/skills) | Claude Agent SDK 官方 Skills 示例库 | Python | 135,006 | +625 | – |
| 8 | [joeseesun/qiaomu-anything-to-notebooklm](https://github.com/joeseesun/qiaomu-anything-to-notebooklm) | 多源内容打通 NotebookLM 的 Claude Skill | Python | 2,626 | +465 | – |
| 9 | [oven-sh/bun](https://github.com/oven-sh/bun) | 极速 JS 运行时 + 打包器 + 测试运行器 | Rust | 90,571 | +395 | – |
| 10 | [NVIDIA-AI-Blueprints/video-search-and-summarization](https://github.com/NVIDIA-AI-Blueprints/video-search-and-summarization) | GPU 加速视觉 Agent / 视频摘要 | Python | 1,104 | +305 | – |
| 11 | [influxdata/telegraf](https://github.com/influxdata/telegraf) | 通用指标 / 日志 / 数据采集 Agent | Go | 17,383 | +213 | – |
| 12 | [czlonkowski/n8n-mcp](https://github.com/czlonkowski/n8n-mcp) | n8n 工作流 MCP 服务器 | TypeScript | 20,854 | +68 | – |

---

## 重点项目点评

### 🥇 [mattpocock/skills](https://github.com/mattpocock/skills) — 今日榜首，+3,155⭐

**前端教父把私人 `.claude/` 目录开源，"工程师的真本事"成新流量密码**

Matt Pocock（TypeScript / TS 教程作者）把自己日常使用的 `.claude/skills/` 目录原样开源，定位"Skills for Real Engineers"。仓库瞄准的不是新手，而是已经在用 Claude Code/Cursor 等 Agent 编码工具的中高级开发者——核心痛点是"AI 给出的代码看似能跑、实际架构在缓慢腐烂"。Skills 给出的是 TDD、issue triage、代码诊断、架构改进等一系列"小而可适配"的实战配方，强调不替代开发者判断、只补全 AI 的盲区。

一夜 +3,155⭐ 的真正驱动力，是社区终于愿意承认："AI 写代码不是模型问题，是工作流问题。" Matt 的影响力把这个观念从开发者博客带到了 GitHub 热榜——这也是为何 obra/superpowers、anthropics/skills、K-Dense-AI/scientific-agent-skills 同日一起爆涨：今天市场已经把"Agent Skills"作为开发者新的"package.json"看待。

如果说 2023 年是 "Awesome List" 时代，2025 年是 "MCP Server" 时代，那 2026 年中段已经明显进入 "Skills" 时代——这是一种比配置更结构化、比 prompt 更可复用的开发资产形态。

---

### 🛰️ [ruvnet/RuView](https://github.com/ruvnet/RuView) — +1,865⭐

**用一颗 ESP32 让 WiFi 信号变成"医院级"传感器**

RuView 走的是一条小众但今年突然爆发的路线：用 WiFi 物理层的 Channel State Information（CSI）反推人体活动——隔墙感知位置、呼吸频率、心率甚至姿态识别，**全程不需要摄像头、不需要可穿戴设备、不上云**。硬件门槛是几美元的 ESP32，软件用 Rust 跑在端侧，定位医疗、零售、安防、工业等"光学传感受限"的场景。

它能突然涨 1.8k+ 是因为几个力量叠加：一是 LLM 时代之后市场对"非视频隐私传感"需求暴涨（养老院、儿童监护、办公室出勤等场景被监管反噬）；二是 Rust + 边缘部署的工程范式已经成熟到可以做"传感算法即服务"；三是 OpenAI / Anthropic 在做大模型的同时，留下了大量"模型无法直接解决但需要被 Agent 调用"的真实世界传感空缺，RuView 正好补这一块。

可以预期接下来这种"WiFi + CSI + 端侧推理"会快速进入 Home Assistant、Frigate 等家居自动化生态。

---

### ⚙️ [obra/superpowers](https://github.com/obra/superpowers) — +1,646⭐

**已经 19 万⭐ 的"事实方法论"还在加速**

Superpowers 由 Jesse Vincent 和 Prime Radiant 团队主导，定位是"给编码 Agent 用的软件开发方法论"——强制 Agent 先头脑风暴细化规格、再切成小颗粒可验证任务、过程中跑 TDD 红绿循环、最后做代码评审与并行 Agent 协调。仓库已积累 19.2 万⭐，但今日仍 +1,646——这种"上不封顶"的曲线说明它已经从"流行框架"切换到"基础设施"。

更重要的信号是它的"多平台中立"：同时支持 Claude Code、GitHub Copilot、Cursor、Gemini。当一个 Agent 方法论可以跨工具复用时，它就成为团队选择 AI 编码工具时的"先决条件"——你先有 Superpowers 工作流，再选谁来跑它。这种"反工具捆绑"的设计让 Anthropic、OpenAI、Google 反过来要兼容它，而不是它兼容它们。

Skills 时代的另一面是方法论开始硬资产化：Superpowers 与 mattpocock/skills 一起构成了"AI 编码方法论"这个新的开源品类。

---

### 🧠 [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) — +1,272⭐

**"Memory Tree" 架构：把 118 个 SaaS 同步进本地 SQLite**

OpenHuman 想解决的是当前云端 AI 助理最被诟病的体验问题——"装上之后还得花两周教它你是谁"。它的差异化设计是 Memory Tree：一个本地 SQLite 知识库，每 20 分钟自动同步 118+ 集成（Gmail、Notion、GitHub、Slack 等），把数据压缩成 Obsidian 兼容 wiki 后存在本地。号称"分钟级上下文，不是周级"。

技术栈是 Rust（70%）+ TypeScript 前端，自带 Web Search、代码工具、语音、Token 智能压缩。本质上是把 Notion AI / ChatGPT Memory 的所有体验在本地、私有、开源条件下重做了一遍。在 Anthropic 9500 亿估值与 OpenAI 加速企业化的当下，OpenHuman 一日 +1.2k⭐ 反映了一股反向力量：**开发者社区在寻找"不被云端绑架"的个人 AI 替代方案**。

OpenHuman 的难点接下来会是：118 个集成的认证维护成本，以及 LLM 推理放回本地后性能与电费的平衡。

---

### 🎙️ [supertone-inc/supertonic](https://github.com/supertone-inc/supertonic) — +712⭐

**端侧 ONNX 多语种 TTS，把 ElevenLabs 的护城河挪到 Swift 上**

Supertonic 由韩国 AI 音频公司 Supertone（被 HYBE 收购）开源，主打"端侧多语种 TTS + ONNX 推理"。这次开源最大的意义不是模型本身有多强，而是它选了 Swift 作为示例语言——直接把 Apple 生态作为第一战场。在 Apple WWDC26 即将开放 App Store 接入 AI Agent、Siri 即将由 Gemini 接管的窗口期，一个能在 iPhone 端本地跑、不需要联网、不依赖 ElevenLabs 云的 TTS，是大量 Agent 应用的关键底座。

更宏观看：2026 年的开源 AI 重心正在从"做大模型"转向"做端侧推理 + 工具栈"。Supertonic、OpenHuman、RuView 同一天上榜，背后是同一个共识——**云端 LLM 卷不出新的差异化，差异化在端侧、在传感器、在低延迟、在隐私**。

---

## 生态观察

今天的 GitHub 热榜呈现一个非常清晰的主题——**"Skills" 正在成为 AI 编码工具的新一级公民**。前 12 名里有 5 个直接以 Skills 命名或主打 Skills 概念（mattpocock、obra、anthropics、K-Dense-AI、joeseesun），加上间接相关的 czlonkowski/n8n-mcp，占据榜单近一半。这与 Anthropic 在 Claude Agent SDK 中把 Skills 提升为一等公民、以及 OpenAI 同期推出"Agent Skills"接口的产业动向完全同频。这意味着**接下来几个月，GitHub 上"skills" 这个关键词的 SEO 价值会持续上升**，开源项目要么作为 Skills 资产入库、要么作为 Skills 加载器存在。

第二条暗线是**端侧 + 隐私的"反云端"潮**：RuView（WiFi 端侧传感）、OpenHuman（本地 Memory Tree）、Supertonic（端侧 TTS）、NVIDIA video-search（本地 GPU 视频 Agent）四个项目同台上榜，构成了一个完整的"端侧 AI Agent 栈"。在 Anthropic 与 OpenAI 把估值推向万亿的当下，开源社区给出了一个明确反应：让我们至少保留一个"不上传到任何 API"的替代生态。

第三条信号是**JS 与 Go 的传统基础设施仍然有韧性**：bun 一天 +395⭐、telegraf 单日 +213⭐——这说明哪怕 AI 占据 70% 的舆论流量，运行时与可观测性这种"基础设施工具"仍然是 GitHub 长期的复利曲线。开发者社区从来不是单一方向，但今天的方向比任何一天都更清晰：**从"调模型"到"调 Skills、调端侧、调集成"**。
