# GitHub Trending 日报 · 2026-09-10

## 今日焦点

> **Agent Skill 框架大爆发 · 中国团队 AI Native 工具入榜 · 图表/CAD/编辑器工具化 · 交易 Agent 站稳 10 万⭐ · 端侧编码 Agent 崛起**
>
> - `ayghri/i-have-adhd` +4,624⭐ 登顶——"让编码 Agent 别再把答案埋起来"的 skill 一夜爆火。
> - `cathrynlavery/diagram-design` +2,286⭐ 冲上前列，38 种编辑器级 SVG 图表模板专供 Claude Code / Codex / Pi。
> - `affaan-m/ECC` +1,151⭐，Agent harness 性能优化系统，覆盖 Claude Code、Cursor 等主流工具。
> - `Tencent/teamai-cli` +563⭐ 首日入榜，腾讯"让每支团队都 AI Native"的 CLI 首次开源。
> - `vastsa/PI-Desktop` +393⭐——Electron + Rust 的本地优先 AI 编码 Agent 桌面端。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) | 阻止编码 Agent 埋答案的 skill | Python | 34,405 | +4,624⭐ | 2,018 |
| 2 | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | 38 种编辑器级图表模板 | HTML | 36,516 | +2,286⭐ | 2,304 |
| 3 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Agent harness 性能优化系统 | JavaScript | 255,119 | +1,151⭐ | 38,219 |
| 4 | [liquidslr/system-design-notes](https://github.com/liquidslr/system-design-notes) | 系统设计面试笔记 | — | 17,953 | +910⭐ | 3,401 |
| 5 | [obra/superpowers](https://github.com/obra/superpowers) | Agent skill 框架与开发方法论 | Shell | 283,990 | +690⭐ | 25,412 |
| 6 | [freestylefly/awesome-gpt-image-2](https://github.com/freestylefly/awesome-gpt-image-2) | GPT-Image2 工业级提示词引擎 | JavaScript | 29,991 | +612⭐ | 2,898 |
| 7 | [Tencent/teamai-cli](https://github.com/Tencent/teamai-cli) | 腾讯团队 AI Native CLI | TypeScript | 2,924 | +563⭐ | 182 |
| 8 | [openai/plugins](https://github.com/openai/plugins) | OpenAI 插件仓库 | JavaScript | 6,165 | +505⭐ | 825 |
| 9 | [vastsa/PI-Desktop](https://github.com/vastsa/PI-Desktop) | 本地优先 AI 编码 Agent 桌面端 | TypeScript | 1,629 | +393⭐ | 152 |
| 10 | [rohitg00/ai-engineering-from-scratch](https://github.com/rohitg00/ai-engineering-from-scratch) | AI 工程从零学起 | Python | 53,648 | +382⭐ | 9,368 |
| 11 | [TauricResearch/TradingAgents](https://github.com/TauricResearch/TradingAgents) | 多 Agent LLM 金融交易框架 | Python | 103,895 | +367⭐ | 19,968 |
| 12 | [pascalorg/editor](https://github.com/pascalorg/editor) | 开源 3D 建筑编辑器 (CLI+MCP) | TypeScript | 22,873 | +171⭐ | 2,893 |
| 13 | [earthtojake/text-to-cad](https://github.com/earthtojake/text-to-cad) | CAD/CAE/CAM Agent skill 库 | Python | 15,010 | +97⭐ | 1,560 |

---

## 重点项目点评

### 🥇 [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) — 今日榜首，+4,624⭐

**"让编码 Agent 别把答案埋起来"——一句吐槽做成的 skill，直接冲上榜首。**

这是一个针对 Claude Code / Codex / Cursor 等编码 Agent 的 **skill 包**：核心逻辑是要求 Agent 在每次输出时把 **最终结论、关键代码块、下一步动作** 放在顶部，而不是先做 3 屏"我准备做什么"的碎碎念。作者写在 README 里的一句话戳中了几乎所有重度 Agent 用户："I don't need your think-aloud, I need the diff."

+4,624⭐ 一夜的增速在 2026 年 skill 生态里是罕见的顶级传播事件——它的价值不是技术复杂度（几乎是纯 prompt 工程），而是 **把用户群体最普遍的痛点用一句非常有梗的 slogan 表达出来**。这也和最近半年 Anthropic Skills、Cursor Rules、Claude Code Plugins 生态的普及有直接关系：**skill 已经变成 Agent 时代的"vim plugin"，任何一个精准解决痛点的 100 行 markdown 都可能爆红。**

对生态的信号：Agent skill 已经从"专家玩具"变成"普通开发者的日常配置"，未来 6 个月这类小而精的 skill 会形成一个类似 npm 的分发生态。

---

### 🥈 [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) — +2,286⭐

**"No shadows. No Mermaid slop." — 38 种编辑器级 SVG 图表模板专供 AI 编码工具。**

作者提供了 **38 种编辑级图表类型**（timeline / flow / matrix / dependency / annotated diagrams 等），每种都是自包含 HTML+SVG，可直接被 Claude Code、Codex、Pi 等工具在 artifact 里渲染出版级质量。作者 Cathryn Lavery 明显在向 Mermaid 的"糙美学"开战——README 里明确写"No Mermaid slop"。

爆红原因是 2026 年 AI 生成图表的普及：Claude Artifacts、ChatGPT Canvas、Codex Diagrams 都在推 SVG-first 输出，但**默认模板通常很丑**。Diagram-design 提供了一套 opinionated 且现代化的模板库，让 Agent 输出图表能有"设计师做过一遍"的质感。这也说明 **Agent 视觉输出正在成为独立赛道**，从"能画"到"画得漂亮"是下一波竞争点。

---

### 🥉 [affaan-m/ECC](https://github.com/affaan-m/ECC) — +1,151⭐

**Agent harness 性能优化系统：给 Claude Code、Codex、Cursor、Opencode 共用的"发动机调参"。**

ECC 的定位很有野心——它不是绑定单一 IDE 或 Agent 框架，而是提供跨工具的 **skills / instincts / memory / security / research-first workflow**。25 万⭐ 的存量说明它已经在开发者社区经营了很久，但 +1,151⭐ 的单日新增源于最近发布的 **v2 版本**：把 memory 从静态文件升级为按上下文自动淘汰的 LRU，以及 **research-first mode**——强制 Agent 在写代码前先在指定 sources 里查找上下文。

真正的信号：**Agent harness 层正在标准化**。过去每个 IDE/Agent 都在造自己的记忆/技能系统，现在开始出现能跨平台复用的中间层，就像早年 LangChain 那种整合位置。ECC + obra/superpowers（前 5）代表两种路线：一个偏"配置文件即优化"，一个偏"方法论即框架"。

---

### 🇨🇳 [Tencent/teamai-cli](https://github.com/Tencent/teamai-cli) — +563⭐

**腾讯首次把 AI Native 团队 CLI 开源，也是近半年国内大厂在 GitHub Trending 少见的正规入榜。**

teamai-cli 定位是"让每个团队都能 AI Native"——本质是一个统一的 team-level Agent 调度和 workflow CLI，能把内部工具、Slack/飞书通知、代码库操作、AI 模型调用绑成脚本化 workflow。虽然 README 目前偏简，但 **仓库 2,924 总星 / 563 单日新增 + 只有 182 forks**，说明它是一夜之间被曝光而不是长期积累。

对生态的意义：**2026 年国内大厂在 AI 开源上的策略明显转向"面向企业协作"的中间件**——不是模型（那已经饱和），而是 workflow 和团队调度。腾讯此举与阿里 Qwen Code、字节 Trae、百度 AppBuilder 并列，形成中国"Team-level Agent 工具链"这个新赛道。

---

### 🖥️ [vastsa/PI-Desktop](https://github.com/vastsa/PI-Desktop) — +393⭐

**本地优先的 AI 编码 Agent 桌面端：Electron 前端 + Rust 核心 + Pi Agent Harness + 用户可安装插件。**

PI-Desktop 是一个把 **Cursor / Claude Code 的体验做成 Electron 桌面 App** 的开源项目——Rust host 处理模型调用、文件系统操作、安全沙盒；Electron 提供 UI；plugin 系统让用户自安装 skill。总星 1,629 但一夜 +393⭐，是新项目起步爆发的典型信号。

它折射出两个趋势：一是 **"Cursor-like 但开源本地" 的诉求越来越强**——开发者厌倦订阅费和数据隐私；二是 **Rust 在 AI Agent host 层的地位加固**——继 Zed、Warp、Rig 之后，又一个把 Rust 作为核心引擎的编码 Agent。这批工具最大挑战是 **本地小模型的可用性**——他们能否用 Qwen 3.8-32B、Llama 4-70B、DeepSeek Coder V4 本地版本，做到接近 Claude Fable / GPT-6 的效果，将决定这条路线能否规模化。

---

## 生态观察

**今日 GitHub Trending 三大主线：**

1. **Agent Skill 生态已经进入"日常配置"阶段。** 前 6 名里有 4 个都是 skill / harness / prompt 库（`i-have-adhd`、`superpowers`、`ECC`、`diagram-design`）。skill 已经从"你需要会写 markdown"降级为"你只需要 star 一个仓库然后引用"，未来会催生类似 Homebrew / npm 的 skill 分发工具。
2. **"AI Native 团队工具"是中国团队的新阵地。** Tencent teamai-cli 首日入榜、freestylefly/awesome-gpt-image-2 稳居第 6 位——中国团队正在跳过"造模型"的正面战场，切入 **企业协作和 prompt 工程** 两个更快见收入的中间层。
3. **本地/桌面 AI Agent 冉冉升起。** PI-Desktop、pascalorg/editor、text-to-cad 三个项目都强调 "local CLI + MCP tools"，说明 **模型足够小 + Anthropic MCP 协议成熟** 之后，开发者开始规模化把 Agent 装进桌面工具和垂直编辑器。

**降温的一条：** 传统 LLM 训练框架、vector DB、RAG 相关仓库今天几乎没进榜——这说明 2026 年"底层 AI 库"的窗口期基本关闭，注意力全部转向了 **skill / workflow / UI 层的应用整合**。
