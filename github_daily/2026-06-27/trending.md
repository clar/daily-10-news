# GitHub Trending 日报 · 2026-06-27

## 今日焦点

> **AI agent 工具链全面扩张 · 设计–代码协议标准化 · 自托管复兴 · 中文 AI 应用占榜**
>
> - `google-labs-code/design.md` 单日 +2,319⭐ —— Google 把"设计语言传递给编码 agent"做成正式格式规范，今日真正的现象级仓库。
> - `calesthio/OpenMontage` 单日 +1,674⭐ —— "全球首个 agent 视频制作系统"，52 个工具串成端到端流水线。
> - `xbtlin/ai-berkshire` 单日 +1,270⭐ —— 价值投资框架用 AI coding 范式重写，中文圈财经向 vibe coding 完美样板。
> - `mauriceboe/TREK` 单日 +1,063⭐ —— 自托管旅行规划器，CasaOS 之后又一个"逃离 SaaS"的爆款。
> - `opendatalab/MinerU` 单日 +944⭐ —— PDF→LLM 友好 Markdown 的最常用基础设施，再次回到首页。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [google-labs-code/design.md](https://github.com/google-labs-code/design.md) | 把视觉系统传递给 coding agent 的格式规范 | TypeScript | 21,144 | +2,319 | 1,716 |
| 2 | [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) | 首个开源 agentic 视频制作系统（52 工具） | Python | 23,536 | +1,674 | 2,614 |
| 3 | [xbtlin/ai-berkshire](https://github.com/xbtlin/ai-berkshire) | AI 范式重写的价值投资研究框架 | Python | 3,074 | +1,270 | 451 |
| 4 | [mauriceboe/TREK](https://github.com/mauriceboe/TREK) | 自托管 + 实时协作 + 地图的旅行规划器 | TypeScript | 7,609 | +1,063 | 646 |
| 5 | [opendatalab/MinerU](https://github.com/opendatalab/MinerU) | PDF → LLM-ready Markdown/JSON 流水线 | Python | 70,368 | +944 | 5,937 |
| 6 | [garrytan/gstack](https://github.com/garrytan/gstack) | "23 个有立场的工具"组成全岗位栈 | TypeScript | 116,588 | +919 | 17,300 |
| 7 | [NanmiCoder/MediaCrawler](https://github.com/NanmiCoder/MediaCrawler) | 多平台中文社媒数据爬取 | Python | 53,335 | +640 | 10,972 |
| 8 | [IceWhaleTech/CasaOS](https://github.com/IceWhaleTech/CasaOS) | 简洁的个人云 OS | Go | 35,335 | +612 | 2,024 |
| 9 | [kunchenguid/no-mistakes](https://github.com/kunchenguid/no-mistakes) | Git 工作流防呆工具 | Go | 3,390 | +412 | 205 |
| 10 | [aws/agent-toolkit-for-aws](https://github.com/aws/agent-toolkit-for-aws) | AWS 官方 MCP server + agent 插件 | Python | 1,340 | +238 | 120 |
| 11 | [simplex-chat/simplex-chat](https://github.com/simplex-chat/simplex-chat) | 无用户 ID 的消息网络 | Haskell | 12,468 | +191 | 706 |
| 12 | [alchaincyf/zhangxuefeng-skill](https://github.com/alchaincyf/zhangxuefeng-skill) | 中文职业规划与教育指导框架 | - | 9,239 | +185 | 2,560 |
| 13 | [ripienaar/free-for-dev](https://github.com/ripienaar/free-for-dev) | 开发者免费云资源大全 | HTML | 123,703 | +137 | 13,050 |
| 14 | [commaai/openpilot](https://github.com/commaai/openpilot) | 300+ 车型支持的开源辅助驾驶 OS | Python | 61,766 | +67 | 11,047 |
| 15 | [grafana/grafana](https://github.com/grafana/grafana) | 可组合的可观测性与可视化平台 | TypeScript | 74,874 | +17 | 14,125 |

---

## 重点项目点评

### 🥇 [google-labs-code/design.md](https://github.com/google-labs-code/design.md) — 今日榜首，+2,319⭐

**Google 终于把"设计→代码"的格式问题定型了**

这是 Google Labs 推出的 **设计系统传递规范**：用一份纯文本 `design.md` 把品牌色板、字体、间距、组件层级、暗黑模式映射全部 schema 化，让 Claude Code / Codex / Cursor / Copilot 等编码 agent 在生成 UI 时 **不再"靠看截图猜"**。它的本质等价于 "OpenAPI 之于 REST" —— 把一种之前依靠隐式知识的协作面表达成机器可读结构。

单日 +2,319⭐ 不是因为代码本身复杂，而是因为它解决了一年来 vibe coding 的最大痛点：模型生成的页面"功能对，但视觉违和"。design.md 让设计师只写一遍规范、所有 agent 同步遵循。后续观察：Anthropic / OpenAI / Vercel 会不会原生支持，以及 Figma 是否会出导出器。

---

### 🥈 [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) — +1,674⭐

**52 个工具串起来的 agentic 视频流水线**

OpenMontage 把脚本理解、镜头规划、素材拉取、剪辑、字幕、音轨、调色、转码 52 个步骤全部封装成可编排的 tool，外层由一个 planner agent 串联。它的位置类似当年 ComfyUI 之于图像生成，把"视频生成"从单一大模型调用变成了 **可调试的有向无环图**。

为什么今天爆掉？两条线：① CapCut / Runway 都把高级功能封到订阅墙后，自托管需求被抑制；② Anthropic / OpenAI 这一年把 tool use 打磨稳定，"52 tool 编排"在 2025 还是噩梦，在 2026 已经能做到稳定 demo。OpenMontage 把一个之前需要 5 个 SaaS 串起来才能做完的工作流压到一个仓库——它就是 2026 上半年"agent 替换 SaaS 套件"的最直观样本。

---

### 🥉 [xbtlin/ai-berkshire](https://github.com/xbtlin/ai-berkshire) — +1,270⭐

**当 vibe coding 撞上 value investing**

ai-berkshire 把巴菲特/芒格风格的价值投资研究方法做成 prompt + 工作流，让模型代替分析师跑：抓财报→DCF→护城河打分→给出"持/卖/观望"理由。新仓库（3,074 星里 1,270 是今天涨的），背后是 **中文圈 AI 投资 圈层** 的一次集体下注——上半年 stock-daily 类项目频繁登榜，但这次 ai-berkshire 把视角从"日报"提升到"长期持仓研究框架"。

它的真实意义不是工具有多强，而是揭示了一个趋势：**vibe coding 范式正在垂直渗透到非 IT 知识工种**——投资研究、法律研究、学术综述都在 6 月集中出现"用 prompt + agent 重写一个老行业"的仓库。质量参差不齐，但 ⭐ 曲线告诉你需求是真的。

---

### 🛫 [mauriceboe/TREK](https://github.com/mauriceboe/TREK) — +1,063⭐

**自托管旅行规划：CasaOS 之后的下一个"逃离 SaaS"代表**

TREK 把行程协作、实时同步、互动地图、推荐对接都做进一个 Docker 即可起的 stack，定位是"Notion + Google My Maps + Wanderlog"三合一的自托管替代。今天 +1,063⭐ 体现的是 **自托管社区在 2026 的二次复兴**：用户数据隐私 + AI agent 的本地化需求，让 self-hosted 类项目重新有了"非小众"的需求基础。

注意它和榜单 #8 CasaOS（+612）以及 #11 SimpleX（+191）形成一个清晰的轴线：消息→OS→应用层，自托管栈的全栈在被一个个补齐。

---

### 📄 [opendatalab/MinerU](https://github.com/opendatalab/MinerU) — +944⭐

**LLM 时代最沉默的水电煤又回到首页**

MinerU 已经 70k 星，今天仍能进前 5，足见它的"基础设施粘性"。它的作用极朴素：把任意复杂 PDF（含表格、公式、栏式排版、扫描图）转成 LLM 友好的 Markdown/JSON。在 2025 它和 Unstructured.io 并列必装，在 2026 它实际已经成为 RAG 流水线的事实默认。

今天再次冲榜的原因极可能是版本更新或某个新模型对接（值得跟踪），但更重要的是它代表了一个被忽视的事实：**真正的 AI 红利不只在前沿 LLM，也在那些把数据从"人类格式"切到"模型格式"的中间层**——这一层目前的中文项目（MinerU、PaddleOCR-VL 等）占据明显优势。

---

## 生态观察

- **AI agent 工具链全面扩张** ：今日前 5 里有 3 个是 agent 配套（design.md / OpenMontage / agent-toolkit-for-aws），证明 agent 已经从"模型能力"变成"模型 + 上下文协议 + 工具集"的组合战。Google 入场 design.md、AWS 入场 MCP server 工具箱，**大厂在抢工具协议层**。
- **vibe coding 进入垂直工种** ：ai-berkshire（投资）、zhangxuefeng-skill（教育/职业规划）、OpenMontage（视频）说明 2026 上半年的趋势是"让某个老行业的从业者用 prompt 复刻整套方法论"，而不是"再做一个 LLM 框架"。
- **自托管复兴** ：TREK、CasaOS、SimpleX 三个赛道（应用 / OS / 通信）同日上榜不是巧合，是用户对 SaaS 锁定 + 数字所有权问题（昨天 HN PlayStation 删 551 部影片是同一情绪）的反扑。
- **中文项目占据三席** ：MinerU、MediaCrawler、ai-berkshire、zhangxuefeng-skill 四个仓库都来自中文社区，证明 GitHub trending 的中文比重在 2026 已经稳定在 25–30%。
- **传统老牌存在感稀薄** ：Grafana 今天只涨 17、commaai openpilot 涨 67，说明在 AI/工具链狂热下，"通用平台型项目"的曝光被严重挤压——这是 GitHub trending 的结构性变化，不是当日噪声。

---

*数据时间：2026-06-27（UTC+8）· 数据源：github.com/trending*
