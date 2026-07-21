# GitHub Trending 每日报告 · 2026-07-22

## 今日焦点

> **AI Agent 全栈热潮 · 代码智能持续升温 · TypeScript × AI 依然主战场 · Rust 稳步蚕食 CLI · 复古与未来同框**
>
> - `bojieli/ai-agent-book` 一天暴涨 **+4,434⭐**，AI Agent 工程学被开源社区正式立教科书
> - `diegosouzapw/OmniRoute` +2,040⭐，"AI 网关 + 268 供应商配额化路由"成为新基础设施类目
> - `tirth8205/code-review-graph` +1,921⭐，本地优先的代码智能图谱把 MCP/CLI 生态又推一大步
> - `ayghri/i-have-adhd` +1,846⭐，编程 agent 输出的"可读性设计"意外破圈
> - `oblien/openship` +1,556⭐，自托管部署平台再次被 Vercel/Fly 定价刺激上榜

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [bojieli/ai-agent-book](https://github.com/bojieli/ai-agent-book) | AI Agent 设计与工程实践开源书 | Python | 14,278 | +4,434⭐ | 1,337 |
| 2 | [diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute) | AI 网关，268+ 供应商、配额自动降级 | TypeScript | 23,484 | +2,040⭐ | 3,144 |
| 3 | [tirth8205/code-review-graph](https://github.com/tirth8205/code-review-graph) | 本地优先的代码智能图谱（MCP/CLI） | Python | 24,487 | +1,921⭐ | 2,347 |
| 4 | [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) | Agent 输出的 ADHD 友好排版 skill | — | 6,745 | +1,846⭐ | 276 |
| 5 | [oblien/openship](https://github.com/oblien/openship) | 自托管部署平台 | TypeScript | 6,129 | +1,556⭐ | 442 |
| 6 | [chrislgarry/Apollo-11](https://github.com/chrislgarry/Apollo-11) | 阿波罗 11 号原始制导计算机源码 | Assembly | 69,920 | +1,195⭐ | 7,838 |
| 7 | [koala73/worldmonitor](https://github.com/koala73/worldmonitor) | 实时全球情报仪表盘（AI 聚合） | TypeScript | 65,168 | +1,167⭐ | 10,169 |
| 8 | [every-app/open-seo](https://github.com/every-app/open-seo) | 开源 SEO 平台替代 | TypeScript | 6,553 | +850⭐ | 710 |
| 9 | [1jehuang/jcode](https://github.com/1jehuang/jcode) | 代码开发智能 agent harness | Rust | 10,273 | +835⭐ | 1,128 |
| 10 | [AstrBotDevs/AstrBot](https://github.com/AstrBotDevs/AstrBot) | IM × LLM 一体化 Agent 助手 | Python | 37,438 | +416⭐ | 2,610 |
| 11 | [earthtojake/text-to-cad](https://github.com/earthtojake/text-to-cad) | CAD / 机器人 / 硬件 Agent skill 集 | JavaScript | 9,059 | +378⭐ | 1,024 |
| 12 | [DioxusLabs/dioxus](https://github.com/DioxusLabs/dioxus) | Web/桌面/移动全栈 Rust 框架 | Rust | 37,622 | +261⭐ | 1,773 |
| 13 | [tradesdontlie/tradingview-mcp](https://github.com/tradesdontlie/tradingview-mcp) | AI 辅助 TradingView 分析集成 | JavaScript | 4,815 | +219⭐ | 2,172 |
| 14 | [AlexsJones/llmfit](https://github.com/AlexsJones/llmfit) | 支持 268+ 供应商的模型发现工具 | Rust | 30,157 | +194⭐ | 1,841 |
| 15 | [hyprwm/Hyprland](https://github.com/hyprwm/Hyprland) | 动态平铺 Wayland 合成器 | C++ | 37,011 | +88⭐ | 1,861 |

---

## 重点项目点评

### 🥇 [bojieli/ai-agent-book](https://github.com/bojieli/ai-agent-book) — 今日榜首，+4,434⭐

**AI Agent 工程学的第一本"教科书"，开源社区喊了一年终于等到**

这个仓库把 2024-2026 三年内 AI Agent 领域散落在博客、论文、Talks 里的**设计模式、评测方法、失败模式**系统化地整理成一本可阅读的"工程手册"，Python 示例 + 章节 + 术语表。**单日 +4,434⭐** 说明社区对"agent 是玄学"的忍受度已到极限，需要一个大家都能引用的共同教材。

这个爆发也踩中当下的教育空档：LangChain/LlamaIndex 官方文档偏工具、Anthropic/OpenAI cookbook 偏产品、学院派论文偏理论——**"工程实践"这一层长期没人写**。当下大量企业内部 agent 项目在裸奔，一本共识手册的经济价值巨大。

值得关注的是 fork 数（1,337）已经与 star 数呈现健康比例——这不是"点收藏"的项目，而是被大量团队 fork 定制化学习。

---

### 🥈 [diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute) — +2,040⭐

**AI 网关不再是可选项，配额路由成为新的"基础设施类目"**

OmniRoute 定位是**多模型 AI 网关**：支持 268+ 供应商，具备 quota-aware auto-fallback，一次调用可在 OpenAI 超配额时无缝降级到 Anthropic/Google/DeepSeek/Kimi。这与今年 3 月的 LiteLLM 大热同频——**企业不再愿意锁死一家模型供应商**。

同榜的 `AlexsJones/llmfit`（模型发现工具）也是同一类目，一天里两个"268+ 供应商"仓库上榜绝非偶然：**Kimi K3、DeepSeek V4、Qwen 系列开源节奏加速**，本地/自托管路由需求水涨船高。可以预期未来 6 个月这个类目会像 2018 年的"多云管理"一样成为 SRE 必备。

---

### 🥉 [tirth8205/code-review-graph](https://github.com/tirth8205/code-review-graph) — +1,921⭐

**本地优先的代码智能图谱，把 MCP 从"玩具"推向生产**

这个项目把整个代码库变成**一张本地可查询的语义图**：调用关系、符号定义、跨文件依赖、变更影响面全部可查，暴露成 MCP 与 CLI 双接口。Claude/Codex/Cursor 这类 agent 都可以直接调用它做"改这个函数会影响哪些测试？"这类 whole-repo 推理。

这是 MCP 生态在 2026 年下半年爆发的一个具体信号——**MCP server 已从"toy demos"进入"你必须装一个才能用 agent"的阶段**。同类项目还会持续出现，本地 embedding + 语义图 + MCP 会成为 developer tools 的新一层。

---

### 🏅 [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) — +1,846⭐

**"能读的输出" 比 "能生成的输出" 更稀缺**

一个专门优化 coding agent 输出格式的 skill：短段、粗体关键动作、明确 diff、"这里我改了什么 / 你现在做什么" 分块。名字自嘲 ADHD，实则击中所有开发者的通病——面对 agent 冗长输出时的注意力崩溃。

这类项目走红有一个大背景：**Claude Code / Codex CLI 等 agent 密集布道后，用户已开始区分"聪明"和"好用"**。同样能力的模型，输出规范的会赢。skill 生态（.claude/skills, Codex skills）正在把这种"人机协作 UX 层"变成可复用组件。

---

### 🎖 [oblien/openship](https://github.com/oblien/openship) — +1,556⭐

**Vercel/Fly.io 涨价潮催生的第 N 波"自托管部署平台"**

Vercel 与 Fly.io 在 2026 年二季度陆续收紧了免费额度和数据出口费，正好让 openship 这类"自托管替代"再度获得关注。TypeScript、docker-first、支持一键部署 Next/Astro/Node/Python——功能上没有革命性，胜在"你能自己 host"的心理安全感。

值得注意的是，此前同类项目（Coolify、Dokploy）都能获得短期爆红但难持续。openship 是否能靠**多云 + AI runbook**做出差异化，将决定它能否走出上一批的 6 个月周期律。

---

## 生态观察

**今日榜单五条主线交织：** ① 教育与设计模式类项目回潮（`ai-agent-book`、`i-have-adhd`），说明 agent 工程正在从"能跑"进入"能规模化"阶段；② 多模型路由类项目集体上榜（OmniRoute、llmfit），侧面印证开源模型军备竞赛已使"路由抽象层"成为刚需；③ 本地代码智能（code-review-graph）与 MCP 生态深度绑定；④ 复古情怀项目常青（Apollo-11 再次上榜）；⑤ Rust 稳步蚕食 CLI、agent runtime、前端框架三条战线。

一个隐性但重要的信号：**没有一款传统"大公司发布的新框架"进入今日 Top 10**，社区的注意力已彻底从"框架 vs 框架"转向"agent 工作流 vs agent 工作流"——GitHub 的引力中心正在从平台切换到 workflow。
