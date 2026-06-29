# GitHub Trending 日报 · 2026-06-30

## 今日焦点

> **去标识化通讯 · AI Agent 工厂 · 价值投资 Agent · 视频编辑 Agent · 隐私基建复兴**
>
> - `simplex-chat/simplex-chat` 无用户 ID 的去标识化即时通讯爆冲 +1,611⭐
> - `ripienaar/free-for-dev` SaaS 免费层清单狂揽 +1,971⭐，连霸榜多日
> - `msitarzewski/agency-agents` "AI Agency 模板"成 GitHub 新一代 boilerplate +1,221⭐
> - `xbtlin/ai-berkshire` 巴菲特价值投资多 agent 框架 +1,397⭐
> - `browser-use/video-use` 用 coding agent 编辑视频，浏览器自动化下一站 +976⭐

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [ripienaar/free-for-dev](https://github.com/ripienaar/free-for-dev) | SaaS/PaaS/IaaS 免费层清单 | HTML | 126,678 | +1,971⭐ | 13,256 |
| 2 | [simplex-chat/simplex-chat](https://github.com/simplex-chat/simplex-chat) | 无用户 ID 即时通讯网络 | Haskell | 16,508 | +1,611⭐ | 954 |
| 3 | [xbtlin/ai-berkshire](https://github.com/xbtlin/ai-berkshire) | AI 多智能体价值投资研究框架 | Python | 6,563 | +1,397⭐ | 862 |
| 4 | [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | 完整的 AI Agency 专家 agent 模板 | Shell | 118,792 | +1,221⭐ | 19,460 |
| 5 | [browser-use/video-use](https://github.com/browser-use/video-use) | 用 coding agent 编辑视频 | Python | 11,894 | +976⭐ | 1,569 |
| 6 | [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) | 个人化 AI 交易 agent | Python | 15,051 | +840⭐ | 2,685 |
| 7 | [altic-dev/FluidVoice](https://github.com/altic-dev/FluidVoice) | macOS 本地离线语音转文字 | Swift | 4,347 | +836⭐ | 272 |
| 8 | [commaai/openpilot](https://github.com/commaai/openpilot) | 300+ 车型的开源辅助驾驶 OS | Python | 62,749 | +465⭐ | 11,111 |
| 9 | [cupy/cupy](https://github.com/cupy/cupy) | GPU 版 NumPy & SciPy | Python | 11,803 | +352⭐ | 1,082 |
| 10 | [0xNyk/council-of-high-intelligence](https://github.com/0xNyk/council-of-high-intelligence) | 18 个 AI persona 多模型协商决策 | Shell | 1,848 | +323⭐ | 199 |
| 11 | [refactoringhq/tolaria](https://github.com/refactoringhq/tolaria) | Markdown 知识库桌面客户端 | TypeScript | 17,484 | +249⭐ | 1,205 |
| 12 | [soxoj/maigret](https://github.com/soxoj/maigret) | 3000+ 网站用户名 OSINT 情报 | Python | 34,336 | +191⭐ | 2,595 |
| 13 | [veracrypt/VeraCrypt](https://github.com/veracrypt/VeraCrypt) | 强加密磁盘卷管理 | C | 10,458 | +187⭐ | 1,231 |
| 14 | [Unclecheng-li/VulnClaw](https://github.com/Unclecheng-li/VulnClaw) | AI agent 渗透测试自动化 | Python | 1,106 | +105⭐ | 170 |
| 15 | [logto-io/logto](https://github.com/logto-io/logto) | SaaS / AI app 鉴权基础设施 | TypeScript | 12,615 | +77⭐ | 862 |

---

## 重点项目点评

### 🥇 [simplex-chat/simplex-chat](https://github.com/simplex-chat/simplex-chat) — +1,611⭐

**全球第一个完全无用户 ID 的即时通讯协议，今日大爆**

SimpleX Chat 的核心创新是：不仅"不需要电话号码"，而是从协议层就**不存在用户标识符**——每个会话是一组临时单向消息队列，服务端无法关联任何两个用户。这套方案在隐私圈被讨论了快 3 年，但今天集中爆发的原因是上周美国最高法院 geofence warrant 判决 + 一百万护照泄露事件叠加推动。

它和 Signal / Session 的差异在于：Signal 仍然需要手机号注册（虽然只用于 onboarding），Session 用 onion routing 但有内部 ID。SimpleX 用 PQXDH (post-quantum key exchange) 做端到端加密、用 SMP 协议做消息分发，理论上是当前最强的"无元数据"通讯方案。

这一波 trending 也反映了 Haskell 在系统级隐私软件领域的复兴——除 SimpleX 外，Pact 智能合约语言、Cardano 节点也都是 Haskell。

---

### 🏢 [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) — +1,221⭐

**"AI Agency 即开即用模板"——开发者市场的新型 SaaS-template**

这个仓库提供了一个完整的多 agent 模板：包括 CEO/CTO/CMO/Designer/Engineer 等 12 个专家 agent，每个 agent 配了角色 prompt、专用工具与工作流。开发者 fork 之后，可以直接拿来给客户做"AI 咨询服务"，也可以当成 Claude Code / Cursor 多 agent workflow 的脚手架。

这种"组织模板"型仓库的趋势源自 2026 年企业咨询行业对 AI 的大规模采购——很多中小咨询公司在卖"AI 部门"服务，agency-agents 就是给他们的 starter kit。同时 Anthropic、OpenAI 都在推 multi-agent SDK，这类模板正好填了"应用层 best practice"的空白。

值得注意：今日新增星数仅 +1,221，但累计星数 118K（fork 19K），说明这是一个长期累积型项目，今日突然爆发可能与某个高影响力 KOL 的推文有关。

---

### 💰 [xbtlin/ai-berkshire](https://github.com/xbtlin/ai-berkshire) — +1,397⭐

**用多 Agent 复刻巴菲特投研流程：财务分析师 + 行业研究员 + 风险官 + 终审决策官**

ai-berkshire 把价值投资的传统分工抽象成 5-8 个 LLM agent：宏观分析、行业研究、财务建模、风险评估、组合配置、终审决策。每个 agent 之间通过结构化报告交换信息，最终输出投资建议 + 持仓建议。仓库提供 Polygon.io / Yahoo Finance / SEC EDGAR 的数据接入模板。

这套架构在 finance + AI 圈热度极高的原因：(1) HKUDS/Vibe-Trading 同日 +840⭐，(2) Bloomberg AI Analyst Agent 在 6 月刚发布企业版，导致开源派必须给出"零成本替代方案"。

这种"模拟金融机构内部分工"的多 agent 框架正在变成一个独立的子赛道——明确比单 LLM 输出投资建议要可解释、可审计、可回溯。

---

### 🎬 [browser-use/video-use](https://github.com/browser-use/video-use) — +976⭐

**Browser-use 团队从浏览器自动化扩展到视频编辑**

Browser-use 之前以"用 LLM agent 自动控制浏览器"出名（GitHub 累计 60K+⭐），video-use 是同团队的新作：把 CapCut / Premiere 等视频编辑器抽象成可被 LLM agent 操控的工作流，用户用自然语言描述需求 → agent 直接操作时间线、转场、字幕、调色。

这一步对 vibe-coding → vibe-editing 是关键节点：之前 video AI 集中在生成（Sora / Runway），video-use 解决的是**后期编辑自动化**，与 Adobe / DaVinci 等专业软件直接竞争。一旦该方案能稳定跑通 1080p 长视频，YouTube / TikTok 创作者的工作流将被根本改写。

---

### 📞 [altic-dev/FluidVoice](https://github.com/altic-dev/FluidVoice) — +836⭐

**号称"最快的 macOS 本地语音转文字"，开源对标 Wispr Flow**

FluidVoice 用 Whisper Large v3 + Apple Neural Engine 优化，号称在 M3 Pro 上做到 4x 实时转录、延迟 <300ms。最关键的卖点是**完全本地**：所有音频不离开设备，对律师、医生、记者、企业内部使用极度友好。

爆发原因可能与 Wispr Flow 涨价到 $24/月有关——FluidVoice 开源 + Swift 原生 + Apple Silicon 优化，定位精准。同时配合本周 Apple Neural Engine 论文（HN 也上榜），开源生态对 ANE 的利用进入新阶段。

---

## 生态观察

**Agent 模板与协议正在 commoditize。** agency-agents、ai-berkshire、Vibe-Trading、council-of-high-intelligence、VulnClaw 五个 multi-agent 项目同日上榜，说明 2026 年的 GitHub 趋势主线是"agent 应用层模板批量生产"——LLM 已经够强，价值正在向"如何编排 agent"转移。

**隐私基础设施迎来"再发明潮"。** SimpleX、VeraCrypt、Maigret（虽然是 OSINT，反向使用即隐私防御）同日上榜，呼应了 HN 上 geofence warrant 判决 + 护照泄露事件。监控时代的反弹正在变成实实在在的代码贡献量。

**Apple Silicon 本地化方向持续受关注。** FluidVoice + ANE 论文 + tolaria（本地笔记软件）共同指向同一个用户群：把 AI 跑在本地 Mac 上、不依赖云端订阅。这与 HN 端 Qwen 3.6 本地 LLM 的讨论相互印证，是一个跨平台共识。

**Vibe-coding 的边界继续扩展：vibe-trading / vibe-editing / vibe-research 全部出现。** 这种"用自然语言操控专业软件"的范式正在从写代码扩展到投资、剪辑、研究等几乎所有专业领域，是 2026 年 H2 最值得跟踪的 product paradigm 转移。
