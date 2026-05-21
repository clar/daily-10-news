# GitHub Trending 每日榜单 · 2026-05-22

## 今日焦点

> **Claude Code 生态全面爆发 · Agent Skills 大规模收录 · 代码知识图谱新范式 · 自托管 AI 平台再起 · 个人 IP 驱动开源**
>
> - `anthropics/claude-plugins-official` 官方插件目录单日 +891⭐，Claude Code 正式步入"插件市场"阶段
> - `colbymchenry/codegraph` 单日暴涨 **+4,222⭐**，本地代码知识图谱挑战 RAG
> - `multica-ai/andrej-karpathy-skills` Karpathy 跳槽 Anthropic 加持下，单日 +2,590⭐
> - `Imbad0202/academic-research-skills` 学术研究 skills 全家桶单日 +2,502⭐
> - `obra/superpowers` 突破 20 万星，agentic skills 框架已成事实标准

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) | 本地预索引代码知识图谱，Claude Code 加速器 | TypeScript | 13,231 | +4,222 | — |
| 2 | [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) | Karpathy 风格的 Claude Code 配置全家桶 | — | 143,032 | +2,590 | — |
| 3 | [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) | 学术研究 skills（写作 / 综述 / 同行评审） | Python | 18,109 | +2,502 | — |
| 4 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic skills 框架 + 软件方法论 | Shell | 201,442 | +1,572 | — |
| 5 | [rohitg00/ai-engineering-from-scratch](https://github.com/rohitg00/ai-engineering-from-scratch) | AI 工程从零教程，Learn-Build-Ship | Python | 10,660 | +1,318 | — |
| 6 | [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) | Anthropic 官方维护的 Claude Code 插件目录 | Python | 22,272 | +891 | — |
| 7 | [rmyndharis/OpenWA](https://github.com/rmyndharis/OpenWA) | 开源自托管 WhatsApp API 网关 | TypeScript | 5,376 | +704 | — |
| 8 | [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | 让任意软件变成 agent-native CLI 平台 | Python | 39,079 | +644 | — |
| 9 | [multica-ai/multica](https://github.com/multica-ai/multica) | 开源托管 Agent 平台，"让 Agent 成为团队成员" | Go | 30,682 | +511 | — |
| 10 | [can1357/oh-my-pi](https://github.com/can1357/oh-my-pi) | 终端 AI 编码 Agent，强化编辑/工具调用 | TypeScript | 5,820 | +483 | — |
| 11 | [antoinezambelli/forge](https://github.com/antoinezambelli/forge) | 自托管 LLM tool-calling Python 框架 | Python | 1,460 | +449 | — |
| 12 | [trimstray/the-book-of-secret-knowledge](https://github.com/trimstray/the-book-of-secret-knowledge) | 经典 CLI/Web/Hack 经验合集 | — | 222,366 | +429 | — |
| 13 | [teng-lin/notebooklm-py](https://github.com/teng-lin/notebooklm-py) | NotebookLM 非官方 Python 接口 | Python | 14,349 | +182 | — |
| 14 | [dotnet/skills](https://github.com/dotnet/skills) | .NET / C# 给 AI 编码 Agent 的 skills | C# | 2,164 | +179 | — |
| 15 | [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) | Chrome DevTools 的 MCP server | TypeScript | 40,455 | +132 | — |

---

## 重点项目点评

### 🥇 [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) — 今日榜首，+4,222⭐

**"本地代码知识图谱"成为 Claude Code 的标配中间件**

CodeGraph 单日暴涨 4,222 星，跃居 trending 榜首。它把仓库的依赖关系、函数调用图、类型签名、跨文件引用等用本地图数据库（基于 Neo4j-like 索引）预先构建出来，让 Claude Code、Cursor 等 Agent 编辑器在大型代码库里能**用图遍历替代 RAG embedding**。结果是：跨文件重构、影响分析、API 升级类任务的成功率显著提高。

这件事标志着 Agent 编程范式的下一步进化：**从"全文索引 + embedding RAG"转向"AST + Graph"的结构化检索**。Cursor、Continue、Claude Code 都在面临同一个瓶颈 —— context window 再大也装不下百万行仓库，而 embedding 在符号级别准确度天花板已经触顶。CodeGraph 的爆红说明社区共识正在形成：未来的 Agent IDE 不会是"更大的模型"，而是"更结构化的索引"。

---

### 🥈 [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) — +2,590⭐

**Andrej Karpathy 跳槽 Anthropic 撞上 Claude Skills 风口**

这个仓库精心提炼了 Karpathy 在多年公开演讲、博客、X 帖中的"编码哲学"，封装成一份可直接加载的 Claude Code skills 配置：偏好渐进式构造、优先用最小工具链、用"教育式注释"解释非显然代码。**项目本身已经过 14 万星**，但叠加 Karpathy 周二宣布加盟 Anthropic 的新闻，今天单日 +2,590⭐ 爆发增长。

这是一个有趣的"名人 IP + 工具生态"叠加现象：以前我们把"Karpathy 风格"看作个人审美，现在它变成了一个可机器复用的人格配置文件。Skills 机制让任何技术人都可以"复刻"一位顶尖工程师的工作偏好 —— 而当这位工程师本人刚刚加入 Anthropic，这种复刻就成了 Claude Code 生态的一次集体投票。

---

### 🥉 [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) — +2,502⭐

**学术研究全流程 skills 化：Claude Code 进军研究生工作流**

这个仓库把博士生 / 研究员日常的工作流 —— 文献检索、综述写作、同行评审、修改稿响应、答辩准备 —— 全部封装成 Claude Code skills。可以一条命令"开始一篇综述"或"按导师反馈逐条改稿"，并自动生成可复现的引用记录。

它单日 +2,502⭐ 的增长说明两件事：第一，**学术圈正在从"用 ChatGPT 偷偷润色"快速跨入"公开承认用 AI Agent 跑流程"的阶段**；第二，**Claude Skills 的范式比传统 "GPT Wrapper" 更受欢迎** —— 因为 skill 是可版本控制、可审计、可复制的 Markdown 文件，符合学术圈对透明度的核心要求。

---

### 🏅 [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) — +891⭐

**Anthropic 官方下场维护"App Store"——Claude Code 商业化的关键一步**

Anthropic 终于亲自下场维护"官方插件目录"，意味着 Claude Code 不再只是一个 CLI 工具，而是开始走 VS Code / Chrome 当年走过的路 —— **构建一个由官方背书、社区贡献、可发现可分发的插件生态**。

这一步背后是清晰的商业逻辑：当 plugins 数量足够多时，开发者的"切换成本"指数级上升，Claude Code 就会真正变成程序员的默认 IDE 入口 —— 一个可以收订阅费、可以分发其他 Anthropic 产品（如 Claude Skills Marketplace）的渠道。从今天 +891⭐ 的增速看，社区正在用脚投票认可这条路。

---

### 🎖️ [obra/superpowers](https://github.com/obra/superpowers) — +1,572⭐（突破 20 万星）

**Agentic skills 框架成为事实标准**

Obra 的 superpowers 项目今天突破 **20 万星**，依旧保持单日 4 位数增长。它是一个 shell-first 的 agentic skills 框架，强调"软件开发方法论"而不仅仅是工具集 —— 把 TDD、git 工作流、debugging 规范全部 codified 成 skill。

它的爆红是过去半年 GitHub 上最重要的"范式跃迁"：当一个 shell-first、文本驱动的方法论框架能在 6 个月内累计 20 万星，说明开发者社区对"工程方法论可机器执行化"达成了空前共识。**Skills 已经从 Anthropic 推的概念，变成了跨工具、跨语言的开发者公约。**

---

## 生态观察

今天的 trending 几乎被 **Claude Code / Agent Skills 生态** 完全占领：榜单 15 个项目里至少 **10 个直接服务于 Agent 编程工作流**（CodeGraph、karpathy-skills、academic-skills、dotnet/skills、superpowers、CLI-Anything、multica、forge、oh-my-pi、claude-plugins-official）。这是 GitHub 历史上罕见的"单一生态主导热榜"现象，说明 2026 年 Q2 已经形成一个**新的开发者基础设施层**。

另一个值得注意的趋势是 **"反 SaaS + 自托管"**：OpenWA（自托管 WhatsApp）、multica（自托管 Agent 平台）、forge（自托管 tool-calling）连续上榜，反映出开发者对 SaaS 锁定的疲劳，以及对"自己掌控数据和模型路由"的强烈偏好。结合最近 Anthropic-xAI 算力大单、Google 广告 AI 化等大背景，**"自托管 + 本地模型 + Skills"** 正在成为对抗大厂中心化的事实方案。

最后，**名人 IP 驱动开源** 是今天最戏剧化的看点：Karpathy 加盟 Anthropic 的新闻当天，他的"风格"被自动算成了流量货币 —— 这种现象未来几个月还会重演，技术人个人品牌的"Skill 化"将是新的开发者 KOL 玩法。
