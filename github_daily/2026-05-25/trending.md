# GitHub Trending 每日热榜 · 2026-05-25

## 今日焦点

> **代码知识图谱井喷 · Claude Code 插件生态膨胀 · 「教 AI 写代码」的技能仓爆火 · 从零手搓 AI 工程 · 自托管视觉 NVR**
>
> - `Lum1104/Understand-Anything` 把任意代码变成交互式知识图谱，单日 +3,987⭐ 登顶
> - `colbymchenry/codegraph` 为各家编程 Agent 提供预索引代码知识图谱，+2,993⭐
> - `multica-ai/andrej-karpathy-skills` 单文件改进 Claude Code 行为，+2,555⭐
> - `rohitg00/ai-engineering-from-scratch` 从零构建 AI 工程，+1,836⭐
> - `anthropics/claude-plugins-official` 官方插件目录持续吸量，+1,179⭐

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [Lum1104/Understand-Anything](https://github.com/Lum1104/Understand-Anything) | 把任意代码转成交互式知识图谱 | TypeScript | 25,494 | +3,987⭐ | 2,204 |
| 2 | [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) | 为编程 Agent 预索引代码知识图谱 | TypeScript | 21,816 | +2,993⭐ | 1,213 |
| 3 | [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) | 单文件优化 Claude Code 行为 | — | 151,917 | +2,555⭐ | 15,575 |
| 4 | [rohitg00/ai-engineering-from-scratch](https://github.com/rohitg00/ai-engineering-from-scratch) | 从零学做 AI 工程 | Python | 15,763 | +1,836⭐ | 2,815 |
| 5 | [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) | 官方 Claude Code 插件目录 | Python | 27,206 | +1,179⭐ | 2,904 |
| 6 | [manaflow-ai/cmux](https://github.com/manaflow-ai/cmux) | 面向 AI Agent 的 macOS 终端 | Swift | 18,969 | +634⭐ | 1,447 |
| 7 | [multica-ai/multica](https://github.com/multica-ai/multica) | 开源托管式 Agent 平台 | TypeScript | 32,443 | +584⭐ | 3,902 |
| 8 | [codecrafters-io/build-your-own-x](https://github.com/codecrafters-io/build-your-own-x) | 从零重建你喜欢的技术 | Markdown | 504,225 | +590⭐ | 47,826 |
| 9 | [Alishahryar1/free-claude-code](https://github.com/Alishahryar1/free-claude-code) | 终端/VSCode 访问 Claude Code | Python | 29,113 | +557⭐ | 4,370 |
| 10 | [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) | 面向知识工作者的 Claude 插件 | Python | 13,962 | +486⭐ | 1,730 |
| 11 | [earendil-works/pi](https://github.com/earendil-works/pi) | AI Agent 工具集（CLI/API/TUI） | TypeScript | 53,887 | +444⭐ | 6,437 |
| 12 | [blakeblackshear/frigate](https://github.com/blakeblackshear/frigate) | 本地实时物体检测 NVR | TypeScript | 32,813 | +226⭐ | 3,177 |
| 13 | [shiyu-coder/Kronos](https://github.com/shiyu-coder/Kronos) | 金融市场基础模型 | Python | 25,771 | +96⭐ | 4,494 |
| 14 | [666ghj/MiroFish](https://github.com/666ghj/MiroFish) | 通用群体智能预测引擎 | Python | 62,106 | +179⭐ | 9,727 |
| 15 | [dotnet/skills](https://github.com/dotnet/skills) | 辅助 AI Agent 的 .NET/C# 技能 | C# | 2,941 | +181⭐ | 217 |

---

## 重点项目点评

### 🥇 [Lum1104/Understand-Anything](https://github.com/Lum1104/Understand-Anything) — 今日榜首，+3,987⭐

**「能教会你的图，胜过看起来很厉害的图」——代码可视化的认知转向**

这个 TypeScript 项目的口号一针见血：图表的价值在于「教会你理解」，而非「炫技」。它把任意代码库转化为交互式知识图谱，让开发者能直观地看到模块依赖、调用关系与数据流，单日狂揽近 4000 星登顶。

它的爆火踩中了一个真实痛点：在 AI 辅助编程时代，人类阅读代码的方式正在改变——我们越来越少逐行读、越来越多需要快速把握「整体结构」。当 Agent 帮你写出大量代码后，「我到底拥有了一个什么样的系统」反而成了新难题。Understand-Anything 这类工具，本质上是在为人机协作补上「理解」这一环。它与今日第二名的 codegraph 一起，标志着「代码知识图谱」从研究概念走向开发者日常工具。

---

### 🥈 [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) — +2,993⭐

**给编程 Agent 喂一张「预索引」的代码地图**

codegraph 的定位非常精准：为 Claude Code、Codex、Cursor、OpenCode、Hermes 等主流编程 Agent 提供预先索引好的代码知识图谱。它解决的是当前 Agent 的核心瓶颈之一——上下文理解。Agent 在大型代码库里最大的问题不是不会写，而是「看不全、记不住」，导致改 A 处坏 B 处（恰好呼应昨日 HN 热议的「Constraint Decay」脆弱性）。

通过预索引整个仓库的符号、依赖与调用关系，codegraph 让 Agent 在动手前就拥有一张全局地图，从而显著降低「盲改」风险。它跨多家 Agent 通吃的中立定位，使其成为基础设施层的有力候选——在 Agent 战争中，谁能成为各家共用的「记忆与索引底座」，谁就握住了关键卡位。

---

### 🥉 [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) — +2,555⭐

**一个 CLAUDE.md 文件，承载 15 万星的「最佳实践」信仰**

这个仓库总星数高达 15.9 万，今日再增 2,555——它做的事极简：用一个 CLAUDE.md 文件，依据 Andrej Karpathy 的观察来改进 Claude Code 的行为。它的超高人气说明了一个有趣现象：在 Agent 时代，「如何配置/引导 Agent」本身已成为一门显学，而名人背书（Karpathy 效应）则能让一份提示词工程实践获得病毒式传播。

这也折射出生态的成熟方向：从「造 Agent」到「调教 Agent」。当编程 Agent 的底层能力趋于同质，差异化越来越落在「上下文工程」与「行为规范」上——一份好的 CLAUDE.md/skills 配置，正成为开发者之间互相交换的硬通货。今日榜单上 dotnet/skills、knowledge-work-plugins 的上榜也印证了这一「技能/插件即生产力」的潮流。

---

### 4️⃣ [rohitg00/ai-engineering-from-scratch](https://github.com/rohitg00/ai-engineering-from-scratch) — +1,836⭐

**「学会它，构建它，为他人发布它」——AI 工程教育的持续刚需**

这个 Python 项目主打「从零开始学 AI 工程」，单日 +1,836⭐。它的走红与常青的 build-your-own-x（今日仍在榜，总星超 50 万）一脉相承：在 AI 能力日益黑箱化的当下，开发者对「亲手搭一遍、真正搞懂底层」的渴望不降反升。

值得注意的是它强调的不只是「学」和「建」，还有「为他人发布」——这反映出 AI 工程正从个人探索走向工程化交付。当大量开发者试图从「调用 API」升级为「构建 AI 系统」，这类系统性的从零教程恰好填补了断层。

---

## 生态观察

今天的 GitHub Trending 几乎是一面镜子，照出了 AI 编程生态的两大主线。

**第一条线：从「写代码」到「理解代码」。** 榜首的 Understand-Anything 与第二的 codegraph 共同把「代码知识图谱」推上风口。这背后是 Agent 时代的范式转变——当 AI 能高速产出代码，人类（和 Agent 自身）的瓶颈转向了「理解一个庞大、快速生长的系统」。可视化与预索引正成为人机协作的新基础设施。

**第二条线：从「造 Agent」到「调教 Agent」。** Claude 系生态今天霸榜——官方插件目录、knowledge-work-plugins、Karpathy skills、free-claude-code、multica 托管平台、cmux 终端，乃至微软的 dotnet/skills，全都围绕「如何更好地配置、运行、扩展编程 Agent」展开。底层模型能力趋同后，竞争正下沉到「技能、插件、上下文工程」这一应用层，「skills/plugins 即生产力」成为开发者的新共识。相比之下，纯算法/框架类项目（如金融基础模型 Kronos）的热度明显被 Agent 工程链生态盖过。
