# GitHub Trending 日报 · 2026-10-09

## 今日焦点

> **Agent 玩转逆向工程 · Claude 技能/插件生态扩张 · 游戏主机"跨端跑"再成现象级 · Python 工具链为 Agent 让路 · 设计工具向 AI 原生靠拢**
>
> - `morluto/rea` 把 Agent 推进到"从行为反推二进制"，一天 **+7,744⭐**
> - `boykopovar/AnyPS5` PS5 可执行文件自动跨平台移植，一天 **+4,640⭐**
> - `storytold/artcraft` Rust 写的创作者引擎突然冲榜，**+2,510⭐**
> - `mattpocock/skills` + `cathrynlavery/diagram-design` + `thedotmack/claude-mem` + `anthropics/knowledge-work-plugins` 四连击，**Claude 生态**占据 Trending 近半席位
> - `ayghri/i-have-adhd` 一个专治"Agent 冗长输出"的 skill 冲上 Python 第 3，**+915⭐**

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [morluto/rea](https://github.com/morluto/rea) | Agent 驱动的反向工程，从行为到二进制 | TypeScript | 25,062 | +7,744⭐ | 2,786 |
| 2 | [boykopovar/AnyPS5](https://github.com/boykopovar/AnyPS5) | PS5 可执行文件自动跨平台移植到 Linux/Windows | C++ | 15,300 | +4,640⭐ | 1,211 |
| 3 | [storytold/artcraft](https://github.com/storytold/artcraft) | 面向艺术家/设计师/影视的创作引擎 | Rust | 7,691 | +2,510⭐ | 1,056 |
| 4 | [mattpocock/skills](https://github.com/mattpocock/skills) | 工程师用 Claude skill 合集 | Shell | 280,990 | +1,770⭐ | 23,553 |
| 5 | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | 为 AI 编辑器定制的 42 种图示 HTML/SVG | HTML | 46,227 | +1,163⭐ | 2,943 |
| 6 | [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) | 让 Agent"把答案放前面"的 ADHD 友好 skill | Python | 55,776 | +915⭐ | 3,186 |
| 7 | [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | 跨会话压缩与注入持久记忆 | TypeScript | 98,398 | +662⭐ | 8,632 |
| 8 | [liquidslr/system-design-notes](https://github.com/liquidslr/system-design-notes) | 《System Design Interview》全书笔记 | — | 24,557 | +398⭐ | 4,595 |
| 9 | [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) | Claude Cowork 的开源知识工作插件 | Python | 27,480 | +309⭐ | 3,191 |
| 10 | [EpicGames/raddebugger](https://github.com/EpicGames/raddebugger) | 原生多进程图形化调试器 | C | 8,089 | +283⭐ | 391 |
| 11 | [IAmTomShaw/f1-race-replay](https://github.com/IAmTomShaw/f1-race-replay) | F1 比赛可视化与数据分析 | Python | 6,674 | +216⭐ | 880 |
| 12 | [earthtojake/text-to-cad](https://github.com/earthtojake/text-to-cad) | 给 Agent 添加 CAD 能力 | Python | 18,460 | +162⭐ | 1,833 |
| 13 | [Tracer-Cloud/opensre](https://github.com/Tracer-Cloud/opensre) | 开源 AI SRE Agent 工具包 | Python | 11,652 | +107⭐ | 1,705 |
| 14 | [smicallef/spiderfoot](https://github.com/smicallef/spiderfoot) | OSINT 自动化威胁情报 | Python | 23,187 | +88⭐ | 3,715 |
| 15 | [bmad-code-org/BMAD-METHOD](https://github.com/bmad-code-org/BMAD-METHOD) | AI 驱动的敏捷开发方法论 | Python | 53,952 | +50⭐ | 6,074 |

---

## 重点项目点评

### 🥇 [morluto/rea](https://github.com/morluto/rea) — 今日榜首，+7,744⭐

**Agent 开始动"反向工程"这块硬骨头**

rea 的卖点非常锋利：**从一个 app 的行为出发，让 Agent 一层层下钻到 native 二进制**——API 调用、函数边界、符号恢复、调用图重建都交给 LLM 协同的 Agent 系统。这把过去只有 Ghidra、IDA、Binary Ninja 配人类专家才做得了的工作，第一次用"自主 Agent + 开源工具链"的组合推上了可用门槛。

它一天拿 7,744⭐ 的原因有三：**第一**，逆向工程社区长期需要可编程、可扩展的 Agent 层；**第二**，TypeScript 实现大幅降低了二开门槛；**第三**，它正好踩在"**Claude/GPT-6 具备跨工具 reasoning**"的能力拐点上。短期看，游戏破解、恶意软件分析、CTF、硬件固件审计都会是它的早期用户。

**真正值得关注的二阶效应**：当 rea 可以把 PS5 二进制里的函数拆到可读层级，再配合榜单第 2 名 AnyPS5——"从反编译到跨平台可执行"的闭环已经在社区内形成雏形。

---

### 🥈 [boykopovar/AnyPS5](https://github.com/boykopovar/AnyPS5) — +4,640⭐

**"把游戏主机变成通用计算平台"的新一轮尝试**

AnyPS5 的核心承诺是：**自动把 PS5 可执行文件适配到 Linux 和 Windows**。考虑到 PS5 的 BSD 内核与 x86-64 架构，这件事在技术上并非不可能，但工程量极大。15K⭐ 的瞬时规模以及今日 4.6K 的净增，说明这是一个用户基础极为广泛的"愿望型"项目。

HN/Reddit 上针对该项目的典型质疑有两点：一是**合法性**——商业游戏的二次分发显然有法律风险；二是**完成度**——真实能跑的游戏列表是什么。但也因为它正好叠加了 rea 这类 Agent-driven 反向工程工具的能力曲线，社区气氛更乐观。

**可能后果**：如果核心能力稳住，这类项目会**倒逼主机厂商加强在线执行环境**，PS5 Online-only、强绑定设备签名等防御机制预计会加码。

---

### 🥉 [storytold/artcraft](https://github.com/storytold/artcraft) — +2,510⭐

**"创作者引擎"赛道有了新 Rust 候选**

artcraft 定位是"**面向艺术家、设计师、影视创作者的 crafting engine**"——描述模糊但 Rust 实现、设计者背景清晰、文档和 Demo 质量比较高。短期能冲 2.5K⭐ 一方面是 Rust 社区的放大效应，另一方面是它主打的"**生成式 + 向量工具 + 时间线一体**"工作流在当下非常稀缺（Figma 偏 UI、Blender 偏建模、Adobe 偏企业版权）。

它所在的赛道正在变得拥挤：Figma Make、Adobe Firefly Workbench、Canva Create AI 都在抢"**AI-native 创作者引擎**"的入口。artcraft 用开源 + 本地可跑 + Rust 性能作为差异化，更接近"**创作者的 Blender**"路线。

---

### 🧰 Claude Skills/Plugins 四连击 — 生态外溢

**[mattpocock/skills](https://github.com/mattpocock/skills) +1,770⭐ · [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) +662⭐ · [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) +309⭐ · [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) +915⭐**

今天的 Trending 真正的"隐藏主角"是 **Claude 的 skill / plugin 生态**。四个来自不同作者、不同角度的 repo 同时在榜：Pocock 的工程师 skill 合集已经是 280K⭐ 的"事实标准"；claude-mem 把跨 session 持久记忆做成 TypeScript 包；Anthropic 官方的 knowledge-work-plugins 则把 Cowork 的生态**完全开源**；i-have-adhd 则是一个只有几十行 YAML 的 skill——"**先把结论放前面**"——却收获了 Python 第 3 名。

这是 2026 Q4 的真正信号：**模型层逐渐商品化之后，Claude 的护城河正迁移到"skill + plugin + 记忆 + Cowork"的生态层**，而且是以 Anthropic 主动开源的方式推进。GPT-6 的 Intelligent UI 想对冲的，正是这个护城河。

---

### 🧠 [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) — +915⭐

**一个 skill 文件，一天进 Python 第 3**

它的本质就是一段 markdown：告诉 Claude 不要先讲背景再给结论，而是**把答案第一段讲完，其余的放后面**。这种"用自然语言规则改变 Agent 行为"的 skill，正在成为开发者社区消费 AI 的新"语法糖"。

一天冲 900+⭐ 不是因为代码本身复杂，而是因为它**揭示了一个新的 UX 范式**：Agent 的默认人格可以被用户用一行配置快速改写，这是浏览器扩展、Dotfiles、Prompt Engineering 三者的融合。

---

## 生态观察

- **Agent 从"写代码"扩散到"读代码/读硬件"**：rea、AnyPS5、text-to-cad、opensre、BMAD-METHOD 共同指向**Agent 处理非一次性任务**（逆向、CAD、SRE、工程规划）的能力拐点已到。
- **Claude 生态正式"溢出"到 Trending**：skills、plugins、memory、knowledge-work 四类项目同一天进榜，表明**生态产品化成熟度**已经越过 2024 年的 LangChain 时期——现在是真正可以直接用的工程组件。
- **游戏/消费类项目的流量回暖**：AnyPS5、f1-race-replay、artcraft 三个在很不同方向上出圈的项目都和 "消费者感知" 挂钩。GitHub Trending 本季开始出现**"开发者 ↔ 普通用户"双向流动**的趋势。
- **Rust 继续稳住"重交互 + 性能敏感"**：artcraft 是 Rust，但 Trending 整体 Python/TS 占比反而更高——这反映出"**Rust 做工具内核，Python/TS 做 Agent 层**"的工程分工正在稳定下来。
- **Classic 项目再被激活**：spiderfoot（23K⭐）、BMAD-METHOD（53K⭐）、black（41K⭐）之所以回榜，是因为**AI Agent 把它们当作工具链调用**——老工具的 API 价值被重新估值。
