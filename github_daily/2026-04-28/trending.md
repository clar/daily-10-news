# GitHub Trending 日报 · 2026-04-28

## 今日焦点

> **Skills 生态爆发 · Claude/Codex 双线竞速 · 智能体记忆基建 · 代码知识图谱**
>
> - `mattpocock/skills` 单日狂揽 +5,551⭐ 登顶榜首，把"工程师私藏 .claude 目录"做成开源标杆
> - `ComposioHQ/awesome-codex-skills` 单日 +637⭐，OpenAI Codex 阵营紧追 Anthropic Skills 模式
> - `abhigyanpatwari/GitNexus` 浏览器内构建代码知识图谱，+1,074⭐，Graph RAG 路线再升温
> - `Alishahryar1/free-claude-code` +2,973⭐，"免费 Claude Code"灰色入口仍在快速吸量
> - `gastownhall/beads` +485⭐，把 Dolt 当智能体长程记忆——agent infra 进入"持久化数据库"时代

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [mattpocock/skills](https://github.com/mattpocock/skills) | 真实工程师的 Claude Skills 集合，直出私人 .claude 目录 | Shell | 29,260 | +5,551 | 2,300 |
| 2 | [Alishahryar1/free-claude-code](https://github.com/Alishahryar1/free-claude-code) | 终端 / VSCode / Discord 三端"免费 Claude Code"入口 | Python | 15,869 | +2,973 | 2,195 |
| 3 | [Z4nzu/hackingtool](https://github.com/Z4nzu/hackingtool) | All-in-one 黑客工具集合 | Python | 66,916 | +1,839 | 7,509 |
| 4 | [abhigyanpatwari/GitNexus](https://github.com/abhigyanpatwari/GitNexus) | 浏览器端代码知识图谱构建器，配合 Graph RAG | TypeScript | 31,345 | +1,074 | 3,584 |
| 5 | [microsoft/VibeVoice](https://github.com/microsoft/VibeVoice) | 微软开源语音 AI | Python | 42,887 | +771 | 4,878 |
| 6 | [ComposioHQ/awesome-codex-skills](https://github.com/ComposioHQ/awesome-codex-skills) | Codex Skills 实战合集，CLI/API 自动化 | Python | 2,675 | +637 | 192 |
| 7 | [gastownhall/beads](https://github.com/gastownhall/beads) | 给编码 Agent 用的图式记忆/任务系统（基于 Dolt） | Go | 22,122 | +485 | 1,455 |
| 8 | [donnemartin/system-design-primer](https://github.com/donnemartin/system-design-primer) | 经典系统设计入门 | Python | 345,075 | +396 | 55,756 |
| 9 | [penpot/penpot](https://github.com/penpot/penpot) | 开源设计协作工具 | Clojure | 46,524 | +283 | 2,791 |
| 10 | [TauricResearch/TradingAgents](https://github.com/TauricResearch/TradingAgents) | 多智能体金融交易框架 | Python | 53,626 | +183 | 9,762 |
| 11 | [davila7/claude-code-templates](https://github.com/davila7/claude-code-templates) | Claude Code 配置模板与监控 CLI | Python | 25,747 | +181 | 2,586 |
| 12 | [CJackHwang/ds2api](https://github.com/CJackHwang/ds2api) | 协议→通用 API 中间件，支持多账号轮转 | Go | 1,799 | +144 | 562 |
| 13 | [deepseek-ai/DeepSeek-V3](https://github.com/deepseek-ai/DeepSeek-V3) | DeepSeek V3 模型仓库 | Python | 103,062 | +60 | 16,697 |

---

## 重点项目点评

### 🥇 [mattpocock/skills](https://github.com/mattpocock/skills) — 今日榜首，+5,551⭐

**当个人 .claude 目录变成开源资产**

Matt Pocock（TypeScript 圈知名教育者）把自己日常使用的 Claude Skills 直接搬出来开源，slogan 写得直白——"Skills for Real Engineers. Straight from my .claude directory."。仓库分四大类：Planning & Design（PRD 转 issue、接口设计问询）、Development（TDD、bug 调查、代码库改进）、Tooling & Setup（pre-commit、安全护栏）、Writing & Knowledge（文档、领域语言抽取）。每个 skill 都是一个可即装即用的提示包。

它在 Anthropic 推 Skills API 不到一年就成为该形态的"标准答案"——今日单日 +5,551⭐ 是榜上最猛的一波资金面，把第二名拉开近一倍。社区情绪非常清楚：玩家不再要 demo 级别的 prompt 模板，而要那种"作者本人天天用的"实战流程。这意味着 Skills 生态正在从"概念验证"跨进"工艺品阶段"，未来 6 个月会出现大量同形态仓库，但能脱颖而出的一定是带有强签名作者背书的那一批。

---

### 🥈 [Alishahryar1/free-claude-code](https://github.com/Alishahryar1/free-claude-code) — +2,973⭐

**"免费 Claude"灰色入口的持续吸量**

这是一个把 Claude Code 接入终端、VSCode 扩展、Discord 三端的"免费"工具，本质上是用某种共享/代理方式让用户绕过订阅。星标增速惊人，但合规性存疑——它能上榜也直接说明 Claude Code 当前的付费门槛与配额限制让大量轻度用户痛苦。

值得关注的不是这个仓库本身，而是它折射的市场缝隙：开发者愿意安装一个匿名作者发的 Python 包来换取 Claude 算力，说明官方限免和 API key 流转的策略需要重新思考。预计 Anthropic 未来若调整 Claude Code 计费或推出免费层，这类仓库会迅速降温。

---

### 🥉 [abhigyanpatwari/GitNexus](https://github.com/abhigyanpatwari/GitNexus) — +1,074⭐

**Graph RAG 终于走到代码理解的"基建层"**

GitNexus 在浏览器里直接对代码库建知识图谱：函数、类、import、依赖全部预先索引，然后通过 MCP 协议把 16 个查询工具暴露给 Claude Code、Cursor、Codex。它要解决的痛点非常具体——agent 改一个函数，常常意识不到下游 47 个调用点会被破坏，于是把"impact analysis"做成一次调用即可返回完整上下文。

这个方向意义很大：当 Skills 提供"做事的工艺"，Knowledge Graph 提供"知道是什么"，二者拼起来才是真正能在大型代码库长程作业的 agent 形态。GitNexus 主打"零服务器、纯客户端"，意味着隐私敏感的企业用户也能用，这是它单日破千星的根本原因。

---

### 4️⃣ [ComposioHQ/awesome-codex-skills](https://github.com/ComposioHQ/awesome-codex-skills) — +637⭐

**Codex 阵营开始抄答案了**

这是 Composio 维护的 Codex Skills 合集，分类几乎与 Anthropic Skills 一模一样——开发工具、生产力协作、写作沟通、数据分析、Meta 工具。最大亮点是与 Composio CLI 的 1000+ 应用集成深度绑定：Skill 不止是提示词，还能直接发邮件、建 GitHub Issue、发 Slack 消息。

它和今日榜首形成镜像格局：mattpocock 是个人作者带 Anthropic Skills 实战，Composio 是公司带 OpenAI Codex 整合。这场"Skills 标准之争"实际上变成了"Anthropic vs OpenAI"在工程层的代理人战。今天双方仓库同时上榜，说明社区已经形成两边下注的避险共识。

---

### 5️⃣ [gastownhall/beads](https://github.com/gastownhall/beads) — +485⭐

**给 Agent 一个真正的数据库式记忆**

Beads 把 Dolt（带版本控制的 SQL 数据库）作为底层，给编码 agent 提供一个图结构的任务/记忆系统。亮点：Hash-based ID 防多 agent 合并冲突、自动生成"已关闭任务的语义压缩摘要"以省 context、原生支持 `relates_to`/`duplicates`/`supersedes` 等图关系。它不是 markdown TODO 增强版，是真在用 SQL+Git 的工艺做 agent 长程记忆。

它和 GitNexus 在思路上同频：Agent 基础设施正在从"prompt 工程"沉到"数据库/图层"。当 agent 要做几小时甚至几天的任务时，靠 in-context 已经支撑不住，必须有结构化、可分支、可合并的外部状态。Beads 的高 fork 比（22k 星 / 1.4k forks，6%）也说明很多团队真在 fork 它接入私有流程。

---

## 生态观察

今天的榜单几乎是"Agent 工程化"的横切面：**Skills 层**（mattpocock、awesome-codex-skills、claude-code-templates）三连发，**记忆 / 知识层**（beads、GitNexus）双双进前 7，**模型 / 基建**（DeepSeek-V3、VibeVoice）作为底座维持热度，**灰色访问**（free-claude-code、ds2api）则反映出付费 agent 服务的市场缝隙。

把这五条线拉直：2026 年 Q2 的开源主战场不再是"哪家模型更强"，而是"如何把模型变成能在真实代码库长跑的工程师"。Skills 给方法、Knowledge Graph 给视野、Beads 给记忆、Templates/CLI 给环境——这是一整套正在快速标准化的栈。值得关注的是榜单中**没有一个传统应用框架**（React、Vue、Spring 等）入榜，注意力已经彻底从"web 工具"迁移到"agent 工具"。

冷门但值得记一笔：`Z4nzu/hackingtool` 和 `system-design-primer` 这种老牌仓库的同步上榜，往往与某种社交媒体大号点名相关，更像是流量噪声而非生态信号。

