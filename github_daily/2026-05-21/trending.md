# GitHub Trending 中文日报 · 2026-05-21

## 今日焦点

> **Claude Code 生态全榜霸屏 · "Karpathy 效应"再次显灵 · 软件 Agent-Native 化加速 · 本地优先 AI 助手抬头**
>
> - `tinyhumansai/openhuman` 一天暴增 **+3,603⭐**，本地优先 Rust AI 助手主打"私有 + 简单 + 强大"
> - `multica-ai/andrej-karpathy-skills` 一份 `CLAUDE.md` 把 Karpathy 的 LLM 编程观蒸馏成四条原则，**+2,620⭐**
> - `colbymchenry/codegraph` 把代码库预索引成知识图谱给 Claude/Cursor/Codex 用，**+1,910⭐**
> - `obra/superpowers` Agentic skills 框架累计接近 20 万星，今日继续 **+1,776⭐**
> - `HKUDS/CLI-Anything` 自动把任何软件生成 Agent 可用 CLI，**+930⭐**

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) | 本地优先的个人 AI 桌面助手 | Rust | 23,540 | +3,603 | 2,104 |
| 2 | [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) | Karpathy 风格 Claude Code 准则 | Markdown | 140,675 | +2,620 | 14,435 |
| 3 | [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) | 给 AI Agent 用的代码知识图谱 | TypeScript | 9,306 | +1,910 | 576 |
| 4 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic 技能与开发方法学框架 | Shell | 199,947 | +1,776 | 17,832 |
| 5 | [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | 全套 AI 代理"公司"模板 | Shell | 102,779 | +1,714 | 16,942 |
| 6 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) | 研究→写作→评审→修订的学术 Skills | Python | 16,051 | +1,639 | 1,439 |
| 7 | [rohitg00/agentmemory](https://github.com/rohitg00/agentmemory) | AI 编码 Agent 的持久记忆层 | TypeScript | 15,072 | +1,121 | 1,247 |
| 8 | [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | 让一切软件变成 Agent-Native | Python | 38,495 | +930 | 3,661 |
| 9 | [rohitg00/ai-engineering-from-scratch](https://github.com/rohitg00/ai-engineering-from-scratch) | 从零搭 AI 工程的学习路径 | Python | 9,475 | +762 | 1,936 |
| 10 | [rmyndharis/OpenWA](https://github.com/rmyndharis/OpenWA) | 自托管 WhatsApp API 网关 | TypeScript | 4,809 | +726 | 973 |
| 11 | [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) | Anthropic 官方 Claude 插件目录 | Python | 20,734 | +706 | 2,539 |
| 12 | [truelockmc/streambert](https://github.com/truelockmc/streambert) | 跨平台电影/动画流媒体桌面端 | JavaScript | 2,922 | +652 | 244 |
| 13 | [zakirullin/files.md](https://github.com/zakirullin/files.md) | 安静的 Markdown 思考空间 | Go | 2,183 | +468 | 50 |
| 14 | [can1357/oh-my-pi](https://github.com/can1357/oh-my-pi) | 终端 AI 编程 Agent + LSP | TypeScript | 5,372 | +237 | 454 |
| 15 | [opentoonz/opentoonz](https://github.com/opentoonz/opentoonz) | 老牌开源 2D 动画制作软件 | C++ | 6,300 | +206 | 728 |

---

## 重点项目点评

### 🥇 [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) — 今日榜首，+3,603⭐

**本地优先（Local-first）AI 助手抢占"隐私版 ChatGPT 桌面端"心智**

OpenHuman 是一个 Rust + TypeScript 写的桌面端 AI 助手，主打"私密 + 简单 + 强大"，内置 118+ 第三方集成（Gmail / Notion / GitHub / Slack 等），所有工作流数据**在本地加密保存**，可选接 Ollama 跑本地模型。亮点是 **Memory Tree 持久记忆**（灵感来自 Karpathy 的知识库思路）与 **TokenJuice 压缩**（号称 token 用量降低 80%）。

它的爆量并非偶然：随着 OpenAI 完成 1220 亿美元融资、Anthropic 推 Claude Opus 4.7 进金融业，**用户对"我的数据进了谁的训练管线"越来越敏感**。本地优先 AI 助手在 2025 年下半年开始出现一批高质量项目，OpenHuman 是这一波里第一个真正破圈到 trending 榜首的——它对 Karpathy 知识图谱思路的复现，也意味着"个人 AI 操作系统"叙事被新一代独立开发者重新捡起。

---

### 🥈 [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) — +2,620⭐

**今日"Karpathy 效应"双重发酵：Anthropic 招他、社区蒸馏他**

这个仓库就是一份 `CLAUDE.md`，把 Karpathy 公开吐槽过的 LLM 编程毛病蒸馏成 4 条原则：**Think Before Coding / Simplicity First / Surgical Changes / Goal-Driven Execution**。可以直接挂到 Claude Code 项目根目录或经插件安装，也兼容 Cursor `.cursor/rules/`。已经累计 **14 万 star、1.44 万 fork**。

它今日继续涨 2.6k 星，**完美卡在 Karpathy 加入 Anthropic 的新闻发布日**——社区在用最朴素的方式表态："如果他要去训练 Claude，那我们先用他的方法论调教 Claude。"这种"行业大事件 → 立刻反映在 GitHub 涨星曲线"的连锁反应，是 Claude Code 生态正在变成事实标准的征兆之一。

---

### 🥉 [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) — +1,910⭐

**MCP 路线开始进入"工程化基础设施"阶段**

CodeGraph 把代码库预先索引成符号 + 关系 + 调用图的 SQLite 知识图谱，再通过 **MCP server** 暴露给 Claude Code、Cursor、Codex CLI、opencode 等 Agent。19+ 语言、13 个 Web 框架的路由识别、文件 watcher 自动同步。官方 benchmark 给出**省 35% 成本、少 59% token、少 70% 工具调用、快 49% 响应**——这是对"为什么 Agent 拼命读文件还不知道架构"的工程级答案。

CodeGraph 的爆发反映出一个明显趋势：**社区对"裸 Agent 漫游代码库"已经不耐烦了**。从去年的"喂 Agent 整个 repo 让它 grep"，到今年的"先把仓库变成结构化的知识图谱"，工具链正在沉淀新的中间层。这条赛道里 agentmemory（今日 +1,121⭐）、CLI-Anything、Claude Skills 都在做类似的"用工程把 LLM 的 token 浪费降下来"。

---

### 🏅 [obra/superpowers](https://github.com/obra/superpowers) — +1,776⭐

**Skills 范式上位：从"Prompt 工程"到"开发方法学"**

`obra/superpowers` 是 Jesse Vincent 维护的 Agentic Skills 框架，提供一整套结构化的"能力 + 方法学"包，让 Claude/Codex 等 Agent 在工程任务里走相对一致的流程。累计接近 **20 万星**——这个量级在 Shell 项目里非常罕见，说明 Skills 已经从"小众玩法"变成大量团队的默认基建。

今天它仍能涨 1.7k 星，主因有二：一是 Anthropic 官方插件目录 `claude-plugins-official` 同时涨 706⭐，把 Skills 体系上升到 Anthropic 自家背书；二是 `multica-ai/andrej-karpathy-skills` 与 `Imbad0202/academic-research-skills` 这种垂直 Skills 包同时上榜，把"Skills 是 Claude Code 生态的乐高基石"这一叙事推到一个新高点。

---

### 🎖️ [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) — +930⭐

**"软件 Agent-Native 化"：把 GUI 程序自动改造成 Agent 可用 CLI**

香港大学数据科学实验室（HKUDS）放出的 CLI-Anything 通过 7 步自动化流水线（分析 → 设计 → 实现 → 测试规划 → 写测试 → 文档 → 发布），把任意有源码的软件自动改造成 Click 风格 CLI 并附带 SKILL.md 供 Agent 发现。已经在 18+ 专业软件（Blender、QGIS 等）上验证，2330+ 测试通过——例如 Blender CLI 真的生成合法 .blend 文件并调用真正渲染器，而不是 mock。

它的核心论断是："今天的软件服务于人类，明天的用户是 Agent。" 这是一种比 MCP 更激进的路线：不是让 Agent 适配 GUI，也不是给 GUI 包一层 wrapper，而是**把整套软件接口改造成对 Agent 友好的形态**。结合 Google Spark、Anthropic Computer Use 的"Agent 操作真实软件"故事，这类工具未来 12 个月很可能进入企业级软件公司的产品规划。

---

## 生态观察

今天的 trending 榜单出现了一个罕见现象：**前 11 名里有 9 个直接或间接服务于 Agent / Claude Code 生态**。从 Skills（superpowers、karpathy-skills、academic-research-skills、agency-agents）到 Agent 基础设施（codegraph、agentmemory、CLI-Anything、claude-plugins-official）再到本地优先 AI 助手（openhuman）和终端编程 Agent（oh-my-pi），整个榜单呈现出"围绕 Claude / Agent 的工程化生态"高度自我强化。

两条最值得记的线索：

1. **"Karpathy 效应"在 GitHub 上肉眼可见**——他加入 Anthropic 的新闻当天，以他为名的 Skills 仓库继续涨 2.6k，二阶辐射到 openhuman 这种引用其 Memory Tree 思路的项目，再到 Skills 框架本身。一位明星研究员的入职在 24 小时内通过仓库 star 曲线被即时映射出来。
2. **本地优先与"Agent 中间层基建"两个细分赛道同步走强**。OpenHuman 代表前者，CodeGraph、AgentMemory、CLI-Anything 代表后者。两条线都在回答同一个问题：**当 Agent 成为新的"用户"之后，我们到底缺什么基础设施。**

相对冷清的是 Web 前端框架与传统数据库项目——今天榜单几乎没有它们的位置，这与过去两年 GitHub trending 的常态形成鲜明对比。
