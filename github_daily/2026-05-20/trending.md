# GitHub Trending 日报 · 2026-05-20

## 今日焦点

> **Claude Code 生态全面席卷 · Agent 框架持续霸榜 · 私有 / 本地 AI 抬头 · Token 节流成新刚需 · 反指纹浏览器趁势出圈**
>
> - `tinyhumansai/openhuman` 本地"私有超级智能"概念，+3,991⭐ 单日榜首
> - `Imbad0202/academic-research-skills` Claude Code 学术研究 skill 套件，+3,184⭐
> - `multica-ai/andrej-karpathy-skills` 单文件 `CLAUDE.md` 提升 Claude Code 行为，借 Karpathy 入职 Anthropic 热度起飞
> - `colbymchenry/codegraph` 预索引代码知识图谱，"少 token、少调用、100% 本地"，+1,869⭐
> - `CloakHQ/CloakBrowser` 反指纹 Chromium，Playwright drop-in，+1,466⭐

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) | 个人版本地超级智能体 | Rust | 20,829 | +3,991⭐ | 1,834 |
| 2 | [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | 让所有软件 agent-native | Python | 37,614 | +1,027⭐ | 3,604 |
| 3 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) | Claude Code 学术研究 skill | Python | 13,988 | +3,184⭐ | 1,326 |
| 4 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic skill 框架 + 方法论 | Shell | 198,255 | +1,620⭐ | 17,685 |
| 5 | [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) | Anthropic 官方 Claude Code 插件目录 | Python | 20,091 | +127⭐ | 2,501 |
| 6 | [rohitg00/agentmemory](https://github.com/rohitg00/agentmemory) | AI 编程 Agent 的持久记忆 #1 | TypeScript | 14,009 | +1,626⭐ | 1,172 |
| 7 | [CloakHQ/CloakBrowser](https://github.com/CloakHQ/CloakBrowser) | 反 bot 检测 Chromium，30/30 测试通过 | Python | 16,430 | +1,466⭐ | 1,268 |
| 8 | [rtk-ai/rtk](https://github.com/rtk-ai/rtk) | LLM token 消耗减 60-90%，Rust 单文件 | Rust | 50,751 | +667⭐ | 3,096 |
| 9 | [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | 完整 AI 代理人公司框架 | Shell | 101,421 | +983⭐ | 16,772 |
| 10 | [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) | 预索引代码知识图谱，100% 本地 | TypeScript | 6,390 | +1,869⭐ | 427 |
| 11 | [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) | 单文件 CLAUDE.md 优化 Claude Code | — | 137,780 | +1,935⭐ | 14,122 |
| 12 | [humanlayer/12-factor-agents](https://github.com/humanlayer/12-factor-agents) | 生产级 LLM 软件 12 法则 | TypeScript | 21,123 | +733⭐ | 1,593 |
| 13 | [Diolinux/PhotoGIMP](https://github.com/Diolinux/PhotoGIMP) | GIMP 3+ 的 Photoshop 化补丁 | CSS | 10,699 | +930⭐ | 372 |
| 14 | [Alishahryar1/free-claude-code](https://github.com/Alishahryar1/free-claude-code) | 免费用 Claude Code（含语音） | Python | 26,251 | +543⭐ | 3,915 |
| 15 | [microsoft/ai-agents-for-beginners](https://github.com/microsoft/ai-agents-for-beginners) | 12 节课入门 AI Agent | Jupyter | 64,221 | +820⭐ | 21,278 |

---

## 重点项目点评

### 🥇 [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) — 今日榜首，+3,991⭐

**"私有 + 本地 + 极简"——又一次对云端 AI 的反向叙事**

`openhuman` 把自己定位成"私人 AI 超级智能"，Rust 实现、走本地优先路线，主打的是"不上传云、配置简洁、性能强"。它选择在 Google 把 AI Ultra 砍到 $100/月、同时把 Gemini 3.5 Flash API 涨价 3 倍的同一周登顶——这个时间点不是巧合。本地 AI 这条赛道在 2025 末 / 2026 初一度被云厂商压住，过去两周内它正在用"价格反向叙事"重新拿到注意力。

Rust + 本地 + Agent 三个标签叠加，是 2026 年 GitHub 上最稳的"工程审美组合拳"。一句话总结：当 frontier 模型 API 不再变便宜，**用户开始重新关心自己机器上能跑多远**。

---

### 🥈 [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) — +3,184⭐

**Claude Code Skill 第一次出现"垂直行业"形态**

这是一套面向学术研究者的 Claude Code skill 包：从"调研 → 写作 → 评审 → 修改 → 定稿"全流程拆成多个 skill，整套挂进 Claude Code 即可。它的意义不在于 skill 本身有多复杂，而在于**这是 Skill 生态出现"行业专精包"的早期标杆**——之前的 trending skill 多是通用工程方向（review / commit / test runner），现在第一次出现"按职业角色打包"的形态。

配合榜单上的 `anthropics/claude-plugins-official`、`obra/superpowers`、`multica-ai/andrej-karpathy-skills`，今天 4 个顶部项目里有 4 个直接服务于 Claude Code——Claude Code 已经事实上成为开发者侧 AI 工具链的**默认底座**。

---

### 🥉 [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) — +1,935⭐

**借势营销天花板：一份 CLAUDE.md，因为 Karpathy 加入 Anthropic 爆红**

这个仓库的核心其实就是**一份 `CLAUDE.md` 文件**——总结了 Karpathy 在公开访谈、博客、Twitter 里散见的 LLM 编程心得，整理为 Claude Code 项目可直接复制粘贴的指令集。它今天 +1,935⭐ 的直接催化剂是 HN 头条新闻"Karpathy 入职 Anthropic"——社区马上把"他的方法论 + Anthropic 的产品"组合成可用资产。

值得注意的是它 13.7w 总星数，意味着这不是新仓库，而是**借助名人效应翻红的老项目**。在 Claude Code 的 skill 生态里，"以人为单位打包知识"这条路被官方正式承认了。

---

### 🚀 [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) — +1,869⭐

**"少 token、少调用、100% 本地"——Agent 经济学的明显转向**

`codegraph` 把代码库预先索引成知识图谱，挂进 Claude Code / Codex / Cursor / OpenCode 后，**让 agent 在做 RAG 时减少绕路、减少 tool call**。它直接戳到了 2026 年开发者侧 AI 工具的最大痛点：**token 账单**。配合榜单第 8 名的 `rtk-ai/rtk`——一个直接代理 LLM 调用、压缩 token 60-90% 的 Rust 单文件工具——可以看出一个清晰趋势：**Agent 不再以"能力增强"为唯一卖点，"省钱"已经成为独立赛道**。

这和今天 HN 上 Gemini 3.5 Flash 涨价 3 倍的争论形成完美闭环：上游涨价 → 下游工具链开始优化每一次 tool call、每一个 token——这是开源社区对商业模型涨价最直接的回应。

---

### 🕶️ [CloakHQ/CloakBrowser](https://github.com/CloakHQ/CloakBrowser) — +1,466⭐

**反指纹 Chromium 走入开源主流——爬虫与反爬虫的新一轮军备竞赛**

`CloakBrowser` 自称"通过所有 bot detection 测试（30/30）"，并以 **Playwright 的 drop-in 替代**形式出现——这意味着任何用 Playwright 写的自动化 / 爬虫脚本，几乎零成本就能换上这套"隐身 Chromium"。背景是大多数主流网站 2025 年起加大了 fingerprinting 检测、再加上 AI agent 大规模爬数据这一新需求——绕开检测的工具链有了真实付费市场。

需要警惕的是它的**双刃属性**：合规自动化 / 学术爬取 / 浏览器测试是合法用途，但同样的能力也可以用于刷量、抢券、数据剥取。GitHub trending 把它顶到第 7 名，说明社区对这种工具的接受度正在上升——这是值得监管和企业安全团队留意的信号。

---

## 生态观察

今天 GitHub trending 几乎可以一句话概括：**"Claude Code Skill 生态 + Agent token 节流 + 本地优先"三股力量同时发力**。

- **Claude Code skill 占据 4 个 top 名次**（#3、#4、#5、#11），证明 skill 框架已经从"Anthropic 自己玩"变成**社区可持续构造的生产力市场**；
- **token 经济学正式登场**：`codegraph`、`rtk`、`agentmemory` 三个项目都在解同一道题——"如何在不降智的前提下，让 Agent 烧更少的钱"；
- **本地 AI 抬头**：`openhuman` 拿榜首，配合 Gemini 3.5 Flash 涨价的舆论，"逃离云端"成为本周开源圈的潜流；
- **生产级 Agent 方法论**继续走强：`humanlayer/12-factor-agents`、`obra/superpowers` 还在加分——社区已经过了"能跑就行"的阶段，开始追问"如何让 Agent 在生产环境长期稳定"。

一句话总结：**5 月 20 日的 GitHub trending 是 Anthropic 生态的一次集体加冕，也是开源社区对"AI 上游涨价"的一次温和反击。**
