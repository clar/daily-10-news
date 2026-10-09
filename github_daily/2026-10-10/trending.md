# GitHub Trending 日报 · 2026-10-10

## 今日焦点

> **Agent 技能化成主流 · 逆向工程 Agent 爆红 · PS5 跨平台移植 · AI 工具美学化 · 创意引擎**
>
> - `morluto/rea` 单日 +15,335⭐：首个真正能"从应用行为一路钻到二进制"的 Agent，占据榜首。
> - `boykopovar/AnyPS5` +5,925⭐：把 PS5 可执行文件移植到 Linux/Windows，游戏逆向圈集体围观。
> - `storytold/artcraft` +3,723⭐：Rust 写的创意工艺引擎，面向艺术家/设计师/电影人。
> - **Agent Skills 板块四连爆**：`mattpocock/skills`、`anthropics/knowledge-work-plugins`、`addyosmani/agent-skills`、`twostraws/SwiftUI-Agent-Skill` 同日上榜。
> - `cathrynlavery/diagram-design` +1,744⭐：42 种自包含 HTML/SVG 图解模板，AI 编码工具的"美学化"趋势显形。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [morluto/rea](https://github.com/morluto/rea) | Agent 驱动逆向工程，App 行为穿透到原生二进制 | TypeScript | 44,124 | +15,335 | 6,916 |
| 2 | [boykopovar/AnyPS5](https://github.com/boykopovar/AnyPS5) | PS5 可执行文件移植到 Linux/Windows | C++ | 21,940 | +5,925 | 1,790 |
| 3 | [storytold/artcraft](https://github.com/storytold/artcraft) | 为艺术家/设计师/电影人打造的"工艺引擎" | Rust | 11,271 | +3,723 | 1,695 |
| 4 | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | AI 编码工具专用的 42 种编辑级 HTML/SVG 图解 | HTML | 47,798 | +1,744 | 3,032 |
| 5 | [mattpocock/skills](https://github.com/mattpocock/skills) | 作者自用 Agent 的工程师技能合集 | Shell | 282,567 | +1,696 | 23,674 |
| 6 | [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) | Claude Cowork 用的"知识工作者"插件集 | Python | 28,206 | +714 | 3,244 |
| 7 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | AI 编码 Agent 的生产级工程技能 | JavaScript | 103,939 | +523 | 10,867 |
| 8 | [alibaba/open-code-review](https://github.com/alibaba/open-code-review) | 确定性流水线 + LLM Agent 的代码审查工具 | Go | 45,145 | +323 | 3,262 |
| 9 | [Robbyant/lingbot-map](https://github.com/Robbyant/lingbot-map) | 流式三维重建的几何上下文 Transformer | Python | 17,669 | +109 | 1,949 |
| 10 | [BerriAI/litellm](https://github.com/BerriAI/litellm) | Rust 内核 + Python SDK 的 AI 网关，兼容 OpenAI 格式 | Python | 60,626 | +95 | 12,186 |
| 11 | [twostraws/SwiftUI-Agent-Skill](https://github.com/twostraws/SwiftUI-Agent-Skill) | 面向 Claude Code / Codex 的 SwiftUI 技能包 | - | 5,389 | +88 | 195 |

---

## 重点项目点评

### 🥇 [morluto/rea](https://github.com/morluto/rea) — 今日榜首，+15,335⭐

**"逆向工程的 Cursor 时刻"**

单日新增 1.5 万星，是本周 trending 榜最强的一次"冷启动"。rea 把 Agent 范式从"应用层代码"扩展到了"原生二进制 + 应用运行时行为"：你让它去理解一个 iOS/Android 应用的某个加密逻辑，它会同时在反汇编、hook、动态插桩、符号传播层并行推理。这类工作传统上需要 Ghidra + Frida + IDA + 大量人类经验，rea 的突破点是用 Agent 把这些工具串成一个连贯推理环。

这类项目爆红的技术背景是：（1）大模型已经能处理较长的汇编上下文；（2）Agentic tool-use 配套工具链成熟（MCP、工具调用、OpenAgents 协议）；（3）合规安全审计、游戏逆向、SDK 兼容性验证这些长尾场景的"人力瓶颈"正在被打破。TypeScript 的选择也值得注意——过去逆向工具链以 C/Python 为主，TS 的流行说明"Agent 侧"的工程文化正在把逆向工程"编程化"。

这也必然引发合规与伦理争议：rea 把门槛大幅拉低意味着更多应用会被"全解剖"——未来一年里 iOS/Android 的反逆向机制、DRM 系统、游戏发行商的反作弊产品，都需要重新评估"假设门槛"。

---

### 🥈 [boykopovar/AnyPS5](https://github.com/boykopovar/AnyPS5) — +5,925⭐

**"主机独占"概念的技术性消解**

AnyPS5 直指 PS5 可执行文件的运行时翻译，让 Sony 独占作品在 Linux/Windows 上原生运行。C++ 做底层，走的是和 Wine / Proton 类似的思路，但针对的是 ORBIS（PS5 的 OS）系统调用而非 Win32。它和多年前的 RPCS3（PS3）处于类似生态位，但 PS5 的时间点要早得多——通常主机模拟器要在上市 7–10 年后才出现。

HN/Reddit 上的反应是双重的：模拟器社区欣喜（这意味着游戏保护主义有了新工具），而发行商和 Sony 的法律团队将在未来几周表态。更深层的信号是：开源社区在"运行时翻译"这件事上的能力已经逼近主机硬件的生命周期——这会直接影响到后续主机的 DRM 架构设计（更多走云端验证、更少让可执行文件落地）。

---

### 🥉 [storytold/artcraft](https://github.com/storytold/artcraft) — +3,723⭐

**AI 时代的"反 AI"创作工具**

artcraft 是用 Rust 写的"工艺引擎"（crafting engine），不走大模型路线，而是用 ECS 架构+形状原语+时间线为艺术家、设计师、电影人提供一个"从草图到最终稿"的本地工作台。它和 Blender、TouchDesigner 的区别是：更轻、更编辑化、更专注于非 AI 的手工流程。

它能在 Agent 风潮里仍然冲上 trending，恰恰说明创意社区的"反潮流"诉求：生成式工具普及后，用户对"过程感"、"可控感"的需求反而上升。Rust 的工程质量和插件化架构让它在很多独立创作者眼中成了"下一个 Blender 候选"。

---

### 🏅 Agent Skills 板块：从个人技巧到"工程规范"

**[mattpocock/skills](https://github.com/mattpocock/skills) · [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) · [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) · [twostraws/SwiftUI-Agent-Skill](https://github.com/twostraws/SwiftUI-Agent-Skill)**

同一个主题下四个项目同日上榜，这是 trending 榜近 60 天最明显的"板块效应"。Matt Pocock（TypeScript 大神）和 Addy Osmani（Google / Chrome DevRel）亲自整理技能库，意味着 Agent Skills 已经从"用户自建 prompt"进化为"社区可共享的工程资产"。Anthropic 的 `knowledge-work-plugins` 则把这股趋势官方化——Claude Cowork 这个产品把"插件"做成了类似 VS Code Extension 的生态。

Twostraws（Paul Hudson）的 SwiftUI 技能包是另一个重要信号：技能库正在"场景化"，专门针对某个框架/领域积累。接下来 12 个月值得观察的是："Skill Registry"、"Skill Marketplace"是否会出现，以及谁能率先建立类似 npm 的生态位。

---

### 🏅 [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) — +1,744⭐

**AI 工具开始追求"编辑级美学"**

42 种自包含 HTML/SVG 图解模板，专门为"AI 代码编辑器 / Agent 开发"场景优化。这个项目的爆红标志着一个新趋势：Agent 不再只被评价"能不能工作"，还要被评价"做出来的东西好不好看"。SVG + 内联样式的技术选择意味着图解可以直接被 Agent 生成、嵌入、修改，而不需要外部渲染工具链。

从社区审美来看，这是对一年前"大模型生成的图又丑又崩"问题的集体回应。整齐、信息密度高、tooltip 可读是明确的设计语言。

---

## 生态观察

今日 trending 清晰呈现三条趋势：

1. **Agent 的"下沉"**：从应用层代码（Cursor、Copilot）下沉到了原生二进制（rea）、游戏主机运行时（AnyPS5）、创意工艺（artcraft）——Agent 正在吃掉之前被认为"必须人类"的工具链。

2. **Skill 板块的工程化**：个人分享 → 社区标准 → 公司产品化，Anthropic 入场把节奏明显拉快。接下来 1–2 月的看点是 Skill 治理、Marketplace、版本管理生态。

3. **"反潮流"创作工具的持续在场**：storytold/artcraft 的 Rust 血统和 cathrynlavery/diagram-design 的 SVG 美学化，提示我们——AI 风潮里，"手工精品"反而稀缺溢价。
