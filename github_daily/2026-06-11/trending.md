# GitHub Trending 日报 · 2026-06-11

## 今日焦点

> **Agent Skills 大爆发 · Claude Code 生态吃下半个榜单 · WiFi 感知与 AI 短视频回潮 · 反审查工具回归**
>
> - `mvanhorn/last30days-skill` 单日 +2,561⭐ 暴涨，Reddit/X/YouTube/HN 跨平台研究 Skill 成为今日 No.1 增量
> - `obra/superpowers` 老牌 Agentic Skills 框架 +1,205⭐ 反弹至榜单第 7，总星数已突破 22 万
> - `addyosmani/agent-skills`、`phuryn/pm-skills`、`google/skills` 三家"Skills 市场"同时上榜——Anthropic Skills 范式被全行业模仿
> - `harry0703/MoneyPrinterTurbo` +1,471⭐ 借 GPT-5.5 Instant 推送再爆发，AI 短视频赛道二次起飞
> - `ruvnet/RuView` Rust 写的 WiFi 信号→空间智能项目 +439⭐ 进榜，空间感知正成为开源新热点

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 面向 AI 编码 Agent 的生产级工程 Skills 集合 | Shell | 51,604 | +781⭐ | 5,694 |
| 2 | [phuryn/pm-skills](https://github.com/phuryn/pm-skills) | PM Skills 市场，100+ agentic skills/commands/plugins | — | 14,753 | +775⭐ | 1,616 |
| 3 | [refactoringhq/tolaria](https://github.com/refactoringhq/tolaria) | Markdown 知识库桌面端管理器 | TypeScript | 14,862 | +618⭐ | 1,026 |
| 4 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 跨 Reddit/X/YouTube/HN/Web 的研究型 AI Skill | Python | 39,006 | +2,561⭐ | 3,149 |
| 5 | [soxoj/maigret](https://github.com/soxoj/maigret) | 输入用户名扫描 3000+ 站点做 OSINT 档案 | Python | 31,963 | +261⭐ | 2,336 |
| 6 | [x1xhlol/system-prompts-and-models-of-ai-tools](https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools) | 各家 AI 编码工具的 system prompt 大全 | — | 139,492 | +397⭐ | 34,589 |
| 7 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic Skills 框架与软件方法论 | Shell | 223,537 | +1,205⭐ | 19,871 |
| 8 | [masterking32/MasterDnsVPN](https://github.com/masterking32/MasterDnsVPN) | 带 ARQ 的高级 DNS 隧道 VPN，反审查 | Go | 5,162 | +351⭐ | 500 |
| 9 | [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) | LLM 驱动的高清短视频自动生成 | Python | 84,938 | +1,471⭐ | 12,127 |
| 10 | [maziyarpanahi/openmed](https://github.com/maziyarpanahi/openmed) | 开源医疗 AI | Python | 2,261 | +535⭐ | 242 |
| 11 | [luongnv89/claude-howto](https://github.com/luongnv89/claude-howto) | Claude Code 可视化教程与 agent 模板 | Python | 36,501 | +204⭐ | 4,411 |
| 12 | [activeloopai/hivemind](https://github.com/activeloopai/hivemind) | 多 Agent 共享大脑层 | TypeScript | 799 | +47⭐ | 49 |
| 13 | [ruvnet/RuView](https://github.com/ruvnet/RuView) | WiFi 信号转空间智能与生命体征监测 | Rust | 72,857 | +439⭐ | 9,724 |
| 14 | [roboflow/supervision](https://github.com/roboflow/supervision) | 通用计算机视觉工具链 | Python | 43,538 | +699⭐ | 3,867 |
| 15 | [google/skills](https://github.com/google/skills) | Google 官方产品的 Agent Skills 集合 | Python | 13,246 | +238⭐ | 1,007 |

---

## 重点项目点评

### 🥇 [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) — 今日榜首，+2,561⭐

**"跨平台搜索 Agent"成为 Claude Skills 商店里最性感的赛道**

这是一个 Claude Code Skill：给定一个话题，它会在过去 30 天的 Reddit、X、YouTube、Hacker News、Google 搜索结果上做并行抓取与摘要，输出结构化的趋势报告。今天单日 +2,561⭐ 让它在 24 小时内跳到 3.9 万总星，是过去一周 Skills 类项目里最猛的增量。

它走红的逻辑值得拆解：第一，**Anthropic 6 月初把 Claude Skills 列入官方 Marketplace**，社区第一次有了搜索类 Skill 的发行渠道；第二，传统"通用 Web 搜索 Agent"（LangGraph、CrewAI）配置复杂，而 Skills 只需要一个 SKILL.md 加 `WebFetch`/`WebSearch` 调用，门槛骤降；第三，"过去 30 天"这种时间窗口约束既贴合"市场研究 / 竞品扫描"等高频商业用例，又避开了 LLM 知识截止日期的固有缺陷。整体看，这是 Skills 范式落地的**首个明星单品**。

---

### 🥈 [obra/superpowers](https://github.com/obra/superpowers) — +1,205⭐

**22.3 万星总数的老牌 Skills 框架今天反弹回榜单第 7**

obra（Jesse Vincent，Anthropic 前 DevEx 负责人）维护的 superpowers 是 Claude Code Skills 概念最早的开源实现，今天 +1,205⭐，把总星推到 **22.35 万**——已经是 GitHub Shell 类项目顶部。它能反弹是因为今天 Anthropic 同时上了 Fable 5 模型与 Managed Agents 公测，而 superpowers 是社区里最完整的"长寿命 Agent + 工程方法论"模板。

更深一层的信号是：**Skills 与 framework 的竞争路线开始分化**。superpowers 走的是"哲学 + 自带工具链 + 沙箱约束"的重路线（接近一个 SDK），而今天榜单上的 addyosmani/agent-skills、phuryn/pm-skills、google/skills 走的是"Marketplace + 单文件 Skill"的轻路线。两条路线都在涨，但社区可能会在 Q3 出现一次合并潮，类似当年 prompt template 仓库与 LangChain 的关系演化。

---

### 🥉 [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — +781⭐ · 今日 No.1

**前 Chrome DevEx 负责人 Addy Osmani 把"前端工程军规"打包成 Skills**

Addy Osmani 这个名字对前端社区是金字招牌（Chrome Web Platform 多年 lead，著有《Learning JavaScript Design Patterns》）。他这个 repo 把 React/Vue/Astro 项目里常见的"代码审查、性能审计、可访问性扫描、构建优化"的 SOP，全部按 Anthropic Skills 规范编排好，可以 `git clone` 后直接被 Claude Code 调用。

这件事的信号意义比技术意义更大——**Skills 不再只是 hobby 项目，而是头部工程师把多年经验沉淀的载体**。预计未来两周会看到更多"作者本人就是细分领域权威"的 Skills 仓库出现（数据库性能、Rust 重构、Postgres 运维等）。这意味着 Claude Skills 正在跑通"专家知识资产化"的产品市场契合，类似 Stack Overflow 早期的"高 reputation 答主"出现。

---

### 4️⃣ [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) — +1,471⭐

**AI 短视频赛道借 GPT-5.5 Instant 推送再爆发**

国人开发者 harry0703 的 MoneyPrinterTurbo 已经是老朋友——给定话题，自动生成短视频脚本、TTS、配字幕、剪辑、加 BGM，一键产出 TikTok / Douyin 风格的 60 秒视频。它今天 +1,471⭐ 的直接原因是 OpenAI 把 GPT-5.5 Instant 推送给全部 ChatGPT 用户，社区在测试新模型短视频脚本质量是否值得替换 GPT-4o——repo README 第一时间加了 GPT-5.5 model 选项。

更宏观地，今天与之前对应的"YouTube 短视频投放、TikTok 算法变更、Meta Reels 货币化下调"几条新闻叠加，AI 短视频被重新视为"剩余红利赛道"。MoneyPrinterTurbo 的中文用户已经把它当成抖音矩阵号的标配生产线，开源版本周更新带动每次模型升级都会有一波星标暴涨。

---

### 5️⃣ [ruvnet/RuView](https://github.com/ruvnet/RuView) — +439⭐

**Rust 写的"WiFi → 空间智能"框架进入主流视野**

ruvnet 的 RuView 把家庭 WiFi 路由器的 CSI（Channel State Information）信号转化为室内人员位置、姿态甚至心率/呼吸频率的时间序列。这并不是新概念（MIT、清华、Carnegie Mellon 都做过类似研究），但用 Rust 写出可在 RPi 5 / 中低端 NUC 跑通的实现是首次开源。

今天 +439⭐ 把它推到 7.28 万总星。背景是 WWDC26 上 Apple 公开演示了 Vision Pro 2 的"无标定房间扫描"——空间感知突然成为消费级故事。RuView 的迷人之处在于它**完全不需要摄像头**，因此可以走"隐私感知"的差异化路线，对监控、银发养老、智能家居都是直接可用的基础设施。这类"硬件友好的小型空间计算 stack"是 2026 下半年值得密切观察的赛道。

---

## 生态观察

**Skills 范式集中爆发：** 今天 15 名榜单里有 **6 个 Claude Skills 项目**（addyosmani、phuryn、mvanhorn、obra、luongnv89、google），合计今天净增 5,764 星——这是 Anthropic 5 月推出 Skills 规范后首次在 GitHub Trending 上形成"半个榜单都被同一范式占据"的现象。生态从"prompt 仓库"和"LangChain 模板"切换到"Skill 包"的趋势已经确立。

**反审查工具悄然回归：** MasterDnsVPN（DNS 隧道 + ARQ 重传）+351⭐ 进入榜单 8，反映出近期多国（俄罗斯、巴基斯坦、土耳其）网络管制升级带来的真实工具需求。Go 实现且支持 Linux/OpenWRT 路由器固件，是个被严重低估的项目。

**AI + 短视频赛道二次起飞：** MoneyPrinterTurbo +1,471⭐ 与去年 7 月那波"AIGC 视频"热度对比，本轮变化在于**用户从猎奇转向真实变现**——大量中文开发者已经把这套流水线对接到 TikTok / Douyin 矩阵号商业模型，star 增长更多来自付费用户的镜像验证。

**冷门赛道亮点：** roboflow/supervision +699⭐ 表明传统 CV 仍有稳定增长基本盘；RuView 的 WiFi-as-Sensor 思路与 maziyarpanahi/openmed 的医疗 AI 互补，构成"物理世界 AI 应用"的小型趋势线。
