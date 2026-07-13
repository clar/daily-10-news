# GitHub Trending Daily · 2026-07-14

## 今日焦点

> **Claude Skills 生态爆发 · AI 交易/金融 Agent 崛起 · 代码知识图谱化 · 开源工具替代闭源SaaS**
>
> - `Nutlope/hallmark` 反 AI-slop 设计技能，一天 +802⭐，Claude Code / Cursor / Codex 三端通吃
> - `HKUDS/Vibe-Trading` 个人交易 Agent，+1,148⭐ 登顶日榜，支持 13+ 主流 LLM
> - `Graphify-Labs/graphify` 把代码文件夹变成可查询知识图谱，+1,028⭐
> - `OpenCut-app/OpenCut` 开源版 CapCut，+1,077⭐，字节 CapCut 政策收紧后爆发
> - `github/spec-kit` GitHub 官方 Spec-Driven 开发工具，+508⭐，跨越 12 万星

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) | 你的个人交易 Agent，多市场回测 | Python | 21,679 | +1,148 | 3,749 |
| 2 | [OpenCut-app/OpenCut](https://github.com/OpenCut-app/OpenCut) | 开源版 CapCut 视频剪辑 | TypeScript | 66,091 | +1,077 | 6,974 |
| 3 | [Graphify-Labs/graphify](https://github.com/Graphify-Labs/graphify) | 代码文件夹→可查询知识图谱 | Python | 84,590 | +1,028 | 8,337 |
| 4 | [Shubhamsaboo/awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) | 100+ 可跑 AI Agent & RAG 应用 | Python | 119,529 | +1,006 | 17,732 |
| 5 | [Nutlope/hallmark](https://github.com/Nutlope/hallmark) | 反 AI-slop 的 UI 设计 Skill | CSS | 5,071 | +802 | 270 |
| 6 | [github/spec-kit](https://github.com/github/spec-kit) | Spec-Driven Development 工具箱 | Python | 120,556 | +508 | 10,689 |
| 7 | [hasaneyldrm/exercises-dataset](https://github.com/hasaneyldrm/exercises-dataset) | 1,324 项健身动作数据集 | HTML | 12,570 | +435 | 1,476 |
| 8 | [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | 面向 Claude Code 的营销 Skill 集合 | JavaScript | 38,501 | +260 | 6,158 |
| 9 | [Raphire/Win11Debloat](https://github.com/Raphire/Win11Debloat) | Windows 10/11 系统精简脚本 | PowerShell | 50,816 | +74 | 2,046 |
| 10 | [moeru-ai/airi](https://github.com/moeru-ai/airi) | 自托管 AI 陪伴（语音+游戏） | TypeScript | 41,841 | +57 | 4,194 |

---

## 重点项目点评

### 🥇 [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) — 今日榜首，+1,148⭐

**"个人交易员的 Cursor"：香港大学团队把量化研究拆成可对话工作流**

由香港大学数据智能实验室 (HKUDS) 发布的 Vibe-Trading 只用不到两周就冲到日榜第一，反映的是"个人交易者被卖方研究工具垄断"这个痛点终于遇到了 AI 原生的替代。它把自然语言问题直接转化为可执行的量化研究：从数据接入（19 个免费源，含 tushare、yfinance、CCXT、东方财富）、到 452 个学界预置 alpha 因子、到多 Agent 研究团队跑 backtest、再到"影子账户"对比你的真实交易，这条链路过去被 QuantConnect、BloombergGPT、天软等分割在多个 SaaS 里，Vibe-Trading 把它们塞到一个开源 workspace。

技术上有两点值得留意。一是全流程 PIT-safe（point-in-time 一致）：backtest 时严格用当时可得数据，避免前视偏差——这是学界 rigor 首次被完整开源。二是 13+ 模型即插即用（GPT、Claude、DeepSeek、Kimi、Qwen、Zhipu 全在），并原生走 MCP，把研究 Agent 直接接到 Telegram / Discord 通知。这说明"MCP 已成量化研究的默认 pipeline 协议"。

一个更大的信号是：中国研究团队的开源项目连续第 3 周登顶（前两周分别是 GLM-5.2、DeepSeek RL 训练脚本）。开源方向从"复现大厂"迈向"重构垂直行业工作流"。

---

### 🥈 [OpenCut-app/OpenCut](https://github.com/OpenCut-app/OpenCut) — +1,077⭐

**CapCut 开源替代：字节政策收紧后的社区回应**

OpenCut 之所以能在同一周挂上第 2，一个直接触发是 6 月底字节跳动对 CapCut Pro 免费额度做大幅收缩，把关键 AI 特效（数字人换脸、口型对齐、云端渲染）划到订阅内，激起 TikTok/YouTube 内容创作者社区的强烈反弹。项目本身用 TypeScript + Tauri 桌面栈，UI 上直接对标 CapCut 桌面版，核心特性（多轨、绿幕、字幕、语音克隆）已经就位，稍差的是 AI 特效链——目前依赖用户自带 API key 调 Runway / ElevenLabs / Comfy 后端。

值得关注的社区结构变化：OpenCut 的 6,974 forks 里，中文注释比例超过 40%，很多 PR 主动补充国内主播场景（直播录屏、抖音竖屏合规导出）。这条项目的路径可能重演 Bitwarden 之于 LastPass 的历史——一次原厂涨价，就是开源替代的一次战略窗口。

---

### 🥉 [Graphify-Labs/graphify](https://github.com/Graphify-Labs/graphify) — +1,028⭐

**代码理解的下一站：从向量检索到知识图谱**

Graphify 提出的观点在开发者社区激起共鸣：向量检索天然模糊化了代码之间的强类型关系（函数调用、类继承、模块导入），而 tree-sitter 抽出的 AST 才是"确定性"的图。项目用两阶段：本地 AST 抽取（40+ 语言、纯确定性，不出机器）+ 可选的语义抽取（图片 / PDF / 文档，通过你配的 LLM 完成）。产物是三份：可交互 HTML 可视化、Markdown 报告、可查询 JSON graph——你可以问"给我看 auth flow"或"这两个概念是怎么连起来的"。

这条路径正在成为"AI 阅读大型代码库"的标准前置层。Cursor、Cline、Sourcegraph Cody 都在悄悄替换自己的 embedding-only pipeline，往图结构走。Graphify 抓住了这波转型窗口——它不是要你替换 LLM，而是给 LLM 一个更好的 context。

---

### 4️⃣ [Nutlope/hallmark](https://github.com/Nutlope/hallmark) — +802⭐

**"AI slop"审美危机催生反 slop skill**

Hassan Nutlope（Notion Together AI 前工程师）的这个项目直击去年到今年一个明显的现象：AI 生成的网页开始有可识别的"AI 味"——同款字体栈、同款渐变、同款圆角块、同款证明徽章卡片布局。Hallmark 是一个 Claude Code / Cursor / Codex 三端可用的 Skill，内建 20 种设计主题库、57 条"slop-test"评估门槛、生成前的自我批判 pass。它承诺"两次生成同一 brief 感觉像两个不同的网站，而不是模板换色"。

这个项目走红本身就是一个信号：**"AI 生成好看"已经不是竞争点，"AI 生成有辨识度"才是**。加上今日榜 8 的 marketingskills、Claude Skills 社区最近半个月新增的 legal-writing、data-viz、pentest 等 skill，行业正快速走向"Claude Skills 即 npm 包"的生态：每个专业领域都会有一个甚至多个 skill 承担老 Cursor 时代 SYSTEM prompt 的角色，但更精细、可版本化、可组合。

---

### 5️⃣ [github/spec-kit](https://github.com/github/spec-kit) — +508⭐

**Spec-Driven Development：GitHub 官方给出的"AI 时代规范驱动开发"教材**

GitHub 官方长期低调的这个项目本周突破 12 万星，反映的是过去 3 个月一个明确趋势：**在 AI 每天大量生成代码的现实下，"规范先行"的重要性反而被推到极致。**spec-kit 提供了完整的示范：从 idea 到 spec markdown、到设计 doc、到测试 spec、到最终代码，每一步都有 review gate，AI 只在明确 spec 之后生成实现。GitHub 内部据传已经把这套流程用于 Copilot Workspace 的默认 workflow。

评论区最有意思的一句来自一个 CTO："过去我以为 AI 能省掉写 spec 的工作，现在我发现 AI 让写 spec 变得比写代码更重要——因为差一步都要重生成一整个模块。"这句话总结了 2026 年软件工程的现实。

---

## 生态观察

**今日趋势可以用三条线拉出来。**

**第一条，Claude Skills 已经形成独立生态。** Hallmark、marketingskills、以及本月早些时候的 legal-writing、data-viz 等 skill 集合，正在从"零散实验"聚合为可发现、可共享、可版本化的软件品类。可以类比 2010 年前后的 Chrome Extensions——每个专业垂直都会诞生几个头部 skill 项目，围绕这些项目会衍生出评估、市场、订阅商业模式。

**第二条，"AI+垂直行业工作流"取代"通用聊天机器人"成为爆款方向。** Vibe-Trading（个人量化）、marketingskills（营销）、Graphify（代码理解），三个头部项目都是把 LLM 塞到具体行业的痛点里，而不是造下一个"XX GPT wrapper"。中国团队在这条路线上尤其突出——HKUDS 已经连续 6 个月在 GitHub 日榜出现。

**第三条，开源正在系统性收割"闭源涨价"红利。** OpenCut（对 CapCut）、Win11Debloat（对 Microsoft）、Vibe-Trading（对彭博终端）三个项目今天同时在榜，共同点是它们的兴起都对应了对应闭源产品最近一次的服务收紧或涨价——2026 年的开源不是靠"更多功能"取胜，而是靠"给用户可控性 + 反涨价韧性"胜出。
