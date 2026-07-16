# GitHub Trending 日报 · 2026-07-17

## 今日焦点

> **Skills 生态爆发 · 反 AI-slop 觉醒 · 开源剪辑工具 · Kimi K3 编码代理 · Copilot SDK**
>
> - `Nutlope/hallmark` +3,181⭐ · 反 AI-slop 设计 Skill，一日冲上榜二
> - `OpenCut-app/OpenCut` +3,290⭐ · 开源版 CapCut，星海继续暴涨
> - `mattpocock/skills` +2,073⭐ · Matt Pocock 把个人 skill 目录整包放出
> - `Graphify-Labs/graphify` +1,138⭐ · 代码/SQL/文档转可查询知识图谱
> - `Shubhamsaboo/awesome-llm-apps` +935⭐ · 122K 星，仍在稳定增长

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [OpenCut-app/OpenCut](https://github.com/OpenCut-app/OpenCut) | 开源版 CapCut，视频剪辑革命 | TypeScript | 73,918 | +3,290 | 7,476 |
| 2 | [Nutlope/hallmark](https://github.com/Nutlope/hallmark) | 反 AI-slop 设计 Skill（Claude/Cursor/Codex） | CSS | 10,779 | +3,181 | 531 |
| 3 | [mattpocock/skills](https://github.com/mattpocock/skills) | 面向工程师的 skill 目录 | Shell | 174,152 | +2,073 | 14,943 |
| 4 | [Graphify-Labs/graphify](https://github.com/Graphify-Labs/graphify) | 代码/SQL/文档→知识图谱 | Python | 88,948 | +1,138 | 8,691 |
| 5 | [Shubhamsaboo/awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) | 100+ Agent & RAG 可运行应用 | Python | 122,807 | +935 | 18,109 |
| 6 | [hasaneyldrm/exercises-dataset](https://github.com/hasaneyldrm/exercises-dataset) | 1324 条健身动作数据集（含 GIF） | HTML | 14,998 | +697 | 1,798 |
| 7 | [HKUDS/DeepTutor](https://github.com/HKUDS/DeepTutor) | 终身个性化 AI 家教 | Python | 26,828 | +647 | 3,608 |
| 8 | [openinterpreter/openinterpreter](https://github.com/openinterpreter/openinterpreter) | 兼容 Codex 的开源模型编码代理（含 Kimi K3） | Rust | 65,949 | +633 | 5,672 |
| 9 | [PrismML-Eng/Bonsai-demo](https://github.com/PrismML-Eng/Bonsai-demo) | Bonsai 演示项目 | Shell | 1,490 | +323 | 152 |
| 10 | [PostHog/posthog](https://github.com/PostHog/posthog) | 产品分析 + AI 观测平台 | Python | 35,806 | +146 | 2,986 |
| 11 | [ibelick/ui-skills](https://github.com/ibelick/ui-skills) | 设计工程师 Skill 集合 | TypeScript | 4,212 | +141 | 174 |
| 12 | [YimMenu/YimMenuV2](https://github.com/YimMenu/YimMenuV2) | GTA5 Enhanced 实验菜单 | C++ | 1,498 | +122 | 359 |
| 13 | [apache/ossie](https://github.com/apache/ossie) | 跨 BI/AI/分析的元数据规范 | Python | 875 | +81 | 133 |
| 14 | [github/copilot-sdk](https://github.com/github/copilot-sdk) | Copilot Agent 多平台 SDK | Java | 9,629 | +62 | 1,316 |
| 15 | [lobehub/lobehub](https://github.com/lobehub/lobehub) | 7×24 Agent 管理平台 | TypeScript | 80,124 | +51 | 15,612 |

---

## 重点项目点评

### 🥇 [OpenCut-app/OpenCut](https://github.com/OpenCut-app/OpenCut) — 今日榜首，+3,290⭐

**开源版 CapCut，直击字节剪映生态的"性能垄断"。**

OpenCut 用 TypeScript / WebGPU 完全在浏览器里实现视频剪辑，覆盖了 CapCut 90% 以上的核心功能：多轨道时间线、关键帧、色彩分级、Vector Text、常见转场特效。项目自 6 月末上线以来一直稳居 GitHub Trending 前列，本周单日再新增 3,290 星，总数逼近 74K。

它之所以能持续走热，本质在于两件事：一是 CapCut 在企业和创作者市场的付费模型（云导出、水印限制）近半年被越来越多人吐槽；二是 WebGPU 在 Chrome 稳定版全面铺开后，浏览器端做接近原生性能的视频渲染第一次成为可能。**OpenCut 是 2026 年"浏览器 = 桌面"这个趋势最有代表性的项目之一。**

---

### 🥈 [Nutlope/hallmark](https://github.com/Nutlope/hallmark) — +3,181⭐

**"Anti-AI-slop"成为一种审美立场——Hallmark 把它做成 Claude Code / Cursor / Codex 的 Skill。**

Nutlope（Together AI 的 Hassan）把一套"反 AI 视觉垃圾"的设计约束打包成 Skill——对齐规则、色板选择、字体层次、间距、动效节奏——让 AI 编码代理在生成 UI 时不再产出"AI 味浓重"的塑料界面。一天 3,181 星，直接把它送上榜二。

它的意义远远超出 CSS 本身：**这是 Skill 生态第一个明确"审美即约束"的案例**——把主观的、气质层面的判断，写成可以被 LLM 遵循的规则集。今天榜单上的 mattpocock/skills、ibelick/ui-skills 都是同一个逻辑的不同变奏：Skill 正在从"任务型"（写测试、跑 lint）走向"品味型"（配色、动效、写作风格）。

---

### 🥉 [mattpocock/skills](https://github.com/mattpocock/skills) — +2,073⭐

**Matt Pocock 把个人 skill 目录整包放出——"skills-as-shareable-config"进入主流。**

TypeScript 教育界名人 Matt Pocock 把自己在 Claude Code / Codex / Cursor 上使用的 skill 目录整体开源，覆盖 TypeScript 严格模式、React 组件规范、Vitest 测试、shadcn 使用、以及一套完整的 refactor 流程。今天新增 2,073 星，位居榜三。

**这条趋势和 Hallmark、UI-skills 合起来说明了一件事：Claude Code 官方在 6 月推出的 Skills 系统正在被开发者社区大规模消费。** 早期 dotfiles 是一个人 Git 里的 zsh 配置，2026 年的 Skills 是一个人 Git 里的整套 AI 协作约束。今天前 4 名里有 3 名是 Skill 或 Skill 消费者，**"skill economy"作为独立品类正式站上舞台。**

---

### 🕸️ [Graphify-Labs/graphify](https://github.com/Graphify-Labs/graphify) — +1,138⭐

**把代码/SQL/文档转成可查询知识图谱——RAG 之后的"下一层抽象"。**

Graphify 的核心叙事是：给 LLM 一个知识图谱比给它一堆向量检索的片段更有效。它可以摄入代码库、SQL schema、Markdown 文档，然后自动抽取实体、关系、依赖，构建可以被 Cypher / SPARQL 查询的图。集成到 Claude Code / Codex / OpenCode / Cursor 后，Agent 在跨文件重构、schema 迁移、跨系统 API 调用图分析等任务上的表现有明显提升。

**它今天上榜的直接触发点是 6 月末 Anthropic 关于"long context ≠ good retrieval"的博客**——业界开始重新讨论"图 vs 向量"这个古老的话题，而 Graphify 恰好是把这条路做得最完整的开源实现。88K 星、1,138 单日新增，反映了社区对 RAG 之后下一层的强烈期待。

---

### 🤖 [openinterpreter/openinterpreter](https://github.com/openinterpreter/openinterpreter) — +633⭐

**Codex 兼容协议 + Kimi K3 支持——开源编码代理的"两栖生存"。**

Open Interpreter 老项目焕发新生的关键：全面切到 OpenAI 的 Codex 协议、原生支持 Kimi K3 与 DeepSeek V4，同时保持了本地文件读写、shell 执行、python 解释器沙盒的完整能力。今天新增 633 星，与 Kimi K3 昨日在 Hacker News 登顶形成明显联动。

**它的战略地位在于：当 Claude Code / Codex / Cursor 都在做闭源商业代理时，Open Interpreter 提供了一个"我用什么模型都行"的中立层。** 用 Fable 5 就是 Fable 5，用 Kimi K3 就是 Kimi K3——开发者对"锁定"的警惕心，在 2026 年反而给这类中立框架带来了新的增长曲线。

---

## 生态观察

**主线一：Skills 生态已经形成独立品类。** 今天榜单前 4 名里，`Nutlope/hallmark`、`mattpocock/skills`、`ibelick/ui-skills` 三个都是 Skill 项目，加上 `Graphify` 这个 Skill 消费者，Skills 单品类占据了绝对流量。这是 Claude Code 5 月推出 Skills 后第一次看到"分享 skill 比分享 config 更常见"的社区现象——**skill economy 正在形成，未来 3 个月会看到大量垂直 skill 库（DevOps、金融、法务）出现。**

**主线二：反 AI-slop 审美觉醒。** Hallmark 一天 3,181 星，标志着开发者社区对"AI 生成的塑料 UI"的反弹到了临界点。当 LLM 越来越能"写代码"，"写出好代码"的边界就从功能正确转向了审美和一致性。**未来几个月会有更多"anti-slop"的字体、颜色、动画、文案 skill 出现。**

**主线三：浏览器/WebGPU 挑战原生桌面工具。** OpenCut 单日 3,290 星，是 2026 年最响亮的"浏览器就是桌面"的注脚。WebGPU 全量铺开 + WASM 生态成熟，让"复杂桌面软件的开源版跑在浏览器里"变得越来越可行——下一波可能会看到 Figma / Adobe / Autodesk 的开源对手。

**主线四：开源模型带火中立执行框架。** Kimi K3 上榜 HN、Open Interpreter 单日 +633，两个事件同时发生并非偶然。**顶级模型闭源化 + 开源模型能力接近 → 开发者需要能"任意切换 backend"的框架**。Open Interpreter、LM Studio Bionic、Ollama 都是这个链条上的受益者。
