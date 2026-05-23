# GitHub Trending 日报 · 2026-05-24

## 今日焦点

> **Claude Code 生态主导榜单 · "代码知识图谱"成为 Agent 标配 · 安全/金融垂类 Skills 涌现 · 长视频生成回归 · 经典工具仍稳坐高位**
>
> - `multica-ai/andrej-karpathy-skills` 单日 +3,372⭐，CLAUDE.md 已成 Agent 时代"提示词圣经"
> - `colbymchenry/codegraph` 单日 +2,434⭐，"预索引代码图谱"声称为 Agent 节省 35% 成本、减少 70% tool calls
> - `Lum1104/Understand-Anything` 单日 +2,331⭐，把代码库转成可视化知识图谱，多 Agent 通吃 Cursor/Claude/Codex
> - `anthropics/claude-plugins-official` 单日 +2,172⭐，Anthropic 官方插件市场正式爆量
> - `mukul975/Anthropic-Cybersecurity-Skills` 单日 +238⭐，单仓库 754 条安全 Skill，AI 安全 Agent 走向"专科化"

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) | Karpathy 派 CLAUDE.md 模板，主打 Think Before Coding | Markdown | 149,505 | +3,372⭐ | 15,327 |
| 2 | [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) | 为编码 Agent 预索引代码图谱，省 35% 成本 | TypeScript | 19,295 | +2,434⭐ | 1,064 |
| 3 | [Lum1104/Understand-Anything](https://github.com/Lum1104/Understand-Anything) | 把任意代码库转成可交互知识图谱 | TypeScript | 21,313 | +2,331⭐ | 1,902 |
| 4 | [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) | Claude Code 官方插件市场目录 | Python | 26,369 | +2,172⭐ | 2,850 |
| 5 | [rohitg00/ai-engineering-from-scratch](https://github.com/rohitg00/ai-engineering-from-scratch) | "Learn it. Build it. Ship it" 端到端 AI 工程教程 | Python | 13,654 | +1,523⭐ | 2,555 |
| 6 | [yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp) | 经典音视频下载器 | Python | 164,929 | +745⭐ | 13,857 |
| 7 | [trimstray/the-book-of-secret-knowledge](https://github.com/trimstray/the-book-of-secret-knowledge) | 工程师必备清单合集 | Markdown | 223,806 | +628⭐ | 13,423 |
| 8 | [Fincept-Corporation/FinceptTerminal](https://github.com/Fincept-Corporation/FinceptTerminal) | 现代化金融分析与投研终端 | Python | 23,097 | +537⭐ | 3,187 |
| 9 | [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) | Chrome DevTools 作为 MCP 服务给 Agent 用 | TypeScript | 41,309 | +437⭐ | 2,623 |
| 10 | [multica-ai/multica](https://github.com/multica-ai/multica) | 团队协作的"托管 Agent"平台 | TypeScript | 31,886 | +429⭐ | 3,858 |
| 11 | [odoo/odoo](https://github.com/odoo/odoo) | 开源企业级 ERP/CRM 平台 | Python | 51,456 | +386⭐ | 32,529 |
| 12 | [presenton/presenton](https://github.com/presenton/presenton) | 开源 AI 演示文稿生成器 + API | TypeScript | 6,317 | +335⭐ | 1,114 |
| 13 | [dotnet/skills](https://github.com/dotnet/skills) | 微软官方 .NET / C# Skills 包 | C# | 2,734 | +262⭐ | 208 |
| 14 | [mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | 754 条结构化网络安全 Skill | Python | 7,351 | +238⭐ | 1,006 |
| 15 | [NVlabs/LongLive](https://github.com/NVlabs/LongLive) | NVIDIA 长视频生成基础设施 | Python | 1,791 | +79⭐ | 168 |

---

## 重点项目点评

### 🥇 [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) — +3,372⭐

**Karpathy 一句话，开发者改 14.9 万次 CLAUDE.md**

这个仓库本质只有一份 CLAUDE.md：四条主张——"Think Before Coding"、"Simplicity First"、"Surgical Changes"、"Goal-Driven Execution"——分别针对 LLM 编码时最常踩的四个坑：胡乱假设、过度抽象、连带改动、跳过验证。仓库提供两种使用方式：Claude Code 全局插件 + 项目级注入，并把 Karpathy 在多场公开演讲与 X 帖中的"反 LLM 编码反模式"系统化。

为何今天暴涨？两个推力：(1) 5 月 23 日 Karpathy 在 Lex Fridman 节目中再次强调 "specs first, code last"，与本仓库主张高度同频；(2) Anthropic 官方插件市场（同榜第 4）正式开放 publish 通道，CLAUDE.md 的"可分发性"被首次合法化。这个仓库直接受益。

它的存在本身揭示了 2026 H1 一个关键转向——"提示词"正在被升级为"工程产物"：可被版本管理、可被测试覆盖、可被发布到插件市场。Karpathy 不再只是教模型架构师，他在教"如何让模型按工程师的方式思考"。

---

### 🥈 [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) — +2,434⭐

**Agent 不该一次次 grep 整个仓库——它该读一张已经备好的图**

CodeGraph 把代码库预索引成一张 SQLite 本地图，包含符号关系、调用图、目录结构与跨文件引用；通过 MCP 服务暴露给 Claude Code、Cursor、Codex 等 Agent，让它们在执行任务时不再依赖大量 `grep` / `read` 工具调用。官方实测数据：成本降低 ~35%、tool call 数下降 ~70%，覆盖 19+ 编程语言，文件变动通过本地 watcher 自动增量更新。

CodeGraph 的爆发说明 Agent 经济正在从"模型即一切"转向"上下文工程才是 ROI 中心"——同等模型下，谁的检索结构更精确，谁的成本曲线就更陡。值得对照同榜的 Understand-Anything：后者偏 UI 可视化，前者偏 Agent 后端；二者一旦合并就是 IDE 端的下一代 Source Insight。

潜在风险：本地 SQLite 在百万行 monorepo 下的索引大小、跨 worktree 切换的一致性是否能撑住，是未来 30 天必须验证的工程问题。

---

### 🥉 [Lum1104/Understand-Anything](https://github.com/Lum1104/Understand-Anything) — +2,331⭐

**"Day-1 工程师入职"问题首次有了通用解**

这个项目通过多 Agent 流水线（项目扫描器、文件分析器、架构检测器、引导式 tour 生成器）将任意代码库转化为可交互的知识图谱，并提供 Web Dashboard 进行可视化探索与语义搜索。它直接面向"新人加入 monorepo 第一天不知道从哪儿读"的高频痛点。

与 CodeGraph 不同，它的"读者"是人——重点是让工程师肉眼快速建立心智模型，并通过"自动生成的 codebase tour"完成第一次贯穿性阅读。覆盖 Claude Code / Cursor / Codex / Gemini CLI / VS Code Copilot 全栈编辑器，意味着无论团队用什么 Agent，都能接入它生成的图谱。

它和 CodeGraph 的同日双爆有结构意义：开发者正在为 LLM 时代下"代码理解"这件被严重忽视的事补课——过去十年我们做了无数 IDE 智能跳转，却几乎没有"系统级理解 + 自动导览"的开源标准答案。

---

### 🛠️ [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) — +2,172⭐

**Anthropic 第一次开官方插件市场——Claude Code 走向"App Store 化"**

仓库结构非常克制：分为 Anthropic 内部插件 与 社区/合作方插件 两个目录，安装命令统一为 `/plugin install {name}@claude-plugins-official`。包含官方质控、安全审查、文档模板与开发者参考实现，是 Claude Code 半年以来最重要的运行时基础设施。

战略意义：与其让"CLAUDE.md / Skills"在 GitHub 野生分发，不如官方做一个统一发现层，反过来强化 Claude Code 的网络效应。今日 Karpathy Skills、Cybersecurity Skills、.NET Skills 同日登榜，本质就是这个市场开放后的"首发效应"。

对开发者意味着两件事：(1) 写 Skill / 插件本身正式成为可发布的"软件产品"；(2) 未来三个月会出现 Skills 版的"Awesome List 大战"，关键评分维度从 Star 数转向"被实际 Agent 调用次数"。

---

### 🔐 [mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) — +238⭐

**Agent 走向"专科化"：单仓库 754 条结构化安全 Skill**

这个仓库把网络安全工作流（漏洞挖掘、CVE 复现、AppSec 扫描、IR 流程等）拆成 754 条标准化 Skill，每条均按 Anthropic Skills 规范封装。它最直观的价值是给 SOC 团队提供"开盒即用"的 Agent 知识库——一线分析师不必再为每一种攻击模式编写 prompt。

之所以将其纳入今日点评，是因为它示范了"垂直 Skill 包"这一新形态：未来 6 个月内，金融、医疗、法律、CAD 等垂类大概率出现类似的"千级 Skill" 仓库。Anthropic Skills 协议很可能像 npm 之于 JavaScript 那样，成为 Agent 时代的"package 标准"。

警示：单仓 754 条意味着维护与版本管控压力极高——HN 已有评论提醒，Skill 包同样需要 SBOM / 依赖审计标准，否则会出现 npm 当年的"依赖污染"复刻。

---

## 生态观察

今天 GitHub Trending 出现近半年最清晰的"Agent 基础设施单日"——前 4 名（Karpathy Skills / CodeGraph / Understand-Anything / Claude Plugins Official）全部围绕 Claude Code 生态，且互为补全：CLAUDE.md 提供编码哲学、CodeGraph 提供检索后端、Understand-Anything 提供可视化前端、Anthropic Plugins 提供分发市场。这是 Claude Code 第一次"作为平台"而非"作为客户端"出现在开发者讨论的中心。

第二条暗线是**"Skill 包"作为新一类开源产物正式登场**：dotnet/skills（.NET 官方）、mukul975/Anthropic-Cybersecurity-Skills（垂直 754 条）以及 Karpathy 风格通用 Skills 同日上榜——意味着 Skill 已具备语言（.NET）、领域（cybersec）、风格（karpathy）三种切分轴。

老牌仓库依然稳定：yt-dlp、odoo、book-of-secret-knowledge 持续吸量；但增量第一梯队完全被 Agent 类项目占据。NVIDIA LongLive 是少数非 Agent 类的研究型仓库，提示"长视频生成"赛道仍在升温但暂未走出实验室。

明日值得追踪：Claude Plugins Official 是否会接入 Skill 评分/下载统计；CodeGraph 是否被 Cursor 集成；Karpathy 本人是否对这个以他命名的 149k 仓库做出回应（fork? endorse? rename request?）。

---

*数据抓取于 2026-05-24 18:00 UTC+8；来源：github.com/trending（daily 视图）。*
