# GitHub Trending 每日热榜 · 2026-07-19

## 今日焦点

> **3D 基础模型爆发 · Agent CLI 三强争锋 · Skills 生态成形 · 本地优先 MCP · AI 教育大合集**
>
> - `Robbyant/lingbot-map` 单日 +827⭐——**流式 3D 场景重建的 feed-forward 基础模型**首次进入榜单前列，视觉基础模型走向 3D 化。
> - `MoonshotAI/kimi-cli` 与 `anomalyco/opencode`（+334⭐）同框——**Claude Code / Kimi CLI / OpenCode 三强 CLI Agent** 的开源分发战正式打响。
> - `anthropics/skills` 累计 16.2 万⭐、单日 +312⭐——**"Skill"作为 Agent 的可组合能力单元**成为跨厂商共识。
> - `tirth8205/code-review-graph` +356⭐——**本地优先 + 持久化代码知识图谱**成为 MCP 时代的新一层基础设施。
> - `codecrafters-io/build-your-own-x` 单日仍在 +1,131⭐——"从零重造轮子"教程库在 AI 编码时代反而更受欢迎。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [codecrafters-io/build-your-own-x](https://github.com/codecrafters-io/build-your-own-x) | 从零重造你最爱的技术教程集 | Markdown | 528,202 | +1,131 | 49,981 |
| 2 | [Robbyant/lingbot-map](https://github.com/Robbyant/lingbot-map) | 流式数据场景重建的 3D 基础模型 | Python | 12,877 | +827 | 1,340 |
| 3 | [HenryNdubuaku/maths-cs-ai-compendium](https://github.com/HenryNdubuaku/maths-cs-ai-compendium) | AI/ML 研究员成长资源大全 | TypeScript | 6,874 | +462 | 825 |
| 4 | [SigNoz/signoz](https://github.com/SigNoz/signoz) | OpenTelemetry 原生可观测性平台 | TypeScript | 30,772 | +425 | 2,353 |
| 5 | [tirth8205/code-review-graph](https://github.com/tirth8205/code-review-graph) | 本地优先代码知识图谱 for MCP/CLI | Python | 20,134 | +356 | 2,123 |
| 6 | [PostHog/posthog](https://github.com/PostHog/posthog) | 自驱动产品平台 + AI 可观测 | Python | 36,562 | +337 | 3,027 |
| 7 | [anomalyco/opencode](https://github.com/anomalyco/opencode) | 开源编码 Agent | TypeScript | 187,218 | +334 | 23,510 |
| 8 | [anthropics/skills](https://github.com/anthropics/skills) | Anthropic 官方 Agent Skills 仓 | Python | 162,394 | +312 | 19,244 |
| 9 | [ibelick/ui-skills](https://github.com/ibelick/ui-skills) | 面向设计工程师的 Skills 集合 | TypeScript | 4,970 | +242 | 208 |
| 10 | [rohitg00/ai-engineering-from-scratch](https://github.com/rohitg00/ai-engineering-from-scratch) | 从零学习并交付 AI 工程 | Python | 39,075 | +240 | 6,551 |
| 11 | [lyogavin/airllm](https://github.com/lyogavin/airllm) | 用单张 4GB GPU 跑 70B 推理 | Jupyter | 23,311 | +234 | 2,653 |
| 12 | [KnockOutEZ/wigolo](https://github.com/KnockOutEZ/wigolo) | 无 API key 的 AI Agent 本地搜索 | TypeScript | 1,199 | +192 | 83 |
| 13 | [datawhalechina/hello-agents](https://github.com/datawhalechina/hello-agents) | 从零构建智能体中文教程 | Python | 67,050 | +145 | 8,327 |
| 14 | [darkroomengineering/lenis](https://github.com/darkroomengineering/lenis) | 平滑滚动交互库 | TypeScript | 14,567 | +74 | 591 |
| 15 | [upstash/context7](https://github.com/upstash/context7) | 面向 LLM 的实时代码文档平台 | TypeScript | 59,361 | +71 | 2,830 |

---

## 重点项目点评

### 🥇 [Robbyant/lingbot-map](https://github.com/Robbyant/lingbot-map) — 今日榜首级涨幅 +827⭐

**视觉基础模型正在从图片/视频走向 3D 场景**

`lingbot-map` 是一个 feed-forward 结构的 3D 场景重建基础模型，直接接受"流式数据"（连续帧图像 / 深度 / 相机位姿）作为输入，输出稠密 3D 表示——与传统 SLAM / NeRF / Gaussian Splatting 走的"逐场景优化"路线完全不同，属于 **"一次训练、任意场景、前向推理"** 的路线。这条路径由 CVPR 26 前后一批工作开启，本仓库是社区第一个把整个训练 + 推理 + 数据处理管线开源到工程可用程度的项目。

单日 +827⭐ 反映的信号是：**继语言模型、多模态模型之后，"3D 场景基础模型"是资本、机器人、AR/VR 共同押注的下一波**——具身智能、无人机导航、机器人操作、AR 眼镜的语义地图都在等这一层。它对标的是 Meta 的 SPARC、Google 的 CAT4D、NVIDIA 的 InstantSplat，但因为开源和"可 fine-tune"两个属性，社区认为它是这一层"最可能被广泛复用的基座"。

---

### 🥈 [tirth8205/code-review-graph](https://github.com/tirth8205/code-review-graph) — +356⭐

**MCP 时代的"本地代码知识层"开始出现**

这是一个"本地优先 + 持久化 + 面向 AI 编码工具"的代码知识图谱：给整份代码库建增量索引，然后通过 MCP Server / CLI 暴露给 Claude Code、Cursor、Kimi CLI 使用。它做的事看似简单——语义化的 grep + 依赖图 + 类型索引，但价值在于**把"每次问 LLM 都要 grep 一遍"的低效模式，替换成"事先跑好、Agent 就地查"的模式**。

单日 +356⭐ 说明市场对"Agent 的记忆和上下文层"需求变得非常紧迫。Cursor、Codeium、GitHub Copilot 都在往云端拉这层，本仓库则押注**"你的代码库离你越近越好"**——尤其对企业内网 / 合规敏感场景。类似定位的项目本周还有 `KnockOutEZ/wigolo`（本地网页搜索）、`aws/agent-toolkit-for-aws`（AWS 官方 MCP 服务器）——**MCP 生态正在从"协议"进化到"生态位分工"**。

---

### 🥉 [anthropics/skills](https://github.com/anthropics/skills) — +312⭐（累计 16.2 万⭐）

**"Skill" 成为 Agent 生态跨厂商的可组合能力单元**

Anthropic 官方 Skills 仓库单日仍在 +312⭐，累计 16.2 万⭐——它的模式（一个 SKILL.md + 参数 + 说明就构成一个"可加载能力"）**已经被整个生态复制**：今天榜单里的 `ibelick/ui-skills`（面向设计工程师的 skills 集合，+242⭐）就是显式模仿；`MoonshotAI/kimi-cli` 的插件加载协议也在向兼容 Skills 靠拢。

这是一个非常反常的信号：**通常大厂想强推的能力接口都会被生态抵制，但 Skills 却在自发扩散**。原因大概是三点：1）SKILL.md 是纯文本 + 极简 schema，学习成本几乎为零；2）Skills 天然沿着"人类拆任务"的方式组合，比 function-calling 更贴近工程师直觉；3）Anthropic 把仓库放在 MIT 协议下，别的 Agent 抄走就能用。**Skills 有可能成为 Agent 时代的 npm**。

---

### 🖥 No.4 · [anomalyco/opencode](https://github.com/anomalyco/opencode) & [MoonshotAI/kimi-cli](https://github.com/MoonshotAI/kimi-cli) — CLI Agent 三强争夺

`opencode`（18.7 万⭐ · 单日 +334⭐）与 `kimi-cli`（9,454⭐ · 单日 +48⭐）本周同框出现在榜单，加上事实上的行业标杆 Claude Code，**"CLI 是 AI 编码 Agent 的最优载体"** 这个共识已经确立。opencode 走的是"任何模型都能接入"的中立路线，是 GitHub Copilot CLI / Cursor CLI / Aider 的开源答卷；kimi-cli 则是 Moonshot 借 Kimi K3 大势直接对标 Claude Code 的商业化路线——这两条路线在今天的榜单上分别代表着"社区拥抱 Claude 生态"和"中国厂商做自己的分发"。

值得注意的是，两个项目都在 README 里明确支持 **MCP + Skills**：CLI Agent 的"三件套"（长上下文模型 + MCP 工具接入 + Skills 能力包）已经变成事实标准。**未来 3–6 个月的竞争焦点将不再是"谁做 CLI"，而是"谁在 CLI 里绑定了最多有价值的 MCP Server 和 Skills"**。

---

### 📚 No.5 · [codecrafters-io/build-your-own-x](https://github.com/codecrafters-io/build-your-own-x) — +1,131⭐（累计 52.8 万⭐）

**"从零重造"教程库在 AI 编码时代反而更火**

一个存在多年的教程集合仓库，今天仍以 +1,131⭐ 位居榜首。这背后是一种反直觉现象：**AI 越强，程序员越想"自己写一次"来搞清楚原理**。Claude Code、Cursor 让搭一个数据库/操作系统/编译器变容易了，但市场上的招聘、面试、以及"如何面对 AI 时代的技术贬值"的焦虑，反而推着开发者去重刷底层。

同一天入围的 `HenryNdubuaku/maths-cs-ai-compendium`（+462⭐）、`rohitg00/ai-engineering-from-scratch`（+240⭐）、`datawhalechina/hello-agents`（+145⭐，中文教程）都是同一类型——**"AI 时代的学习清单"品类正在全面复兴**，且以 GitHub Markdown 教程的形式，与 Twitter/X 长文、YouTube 长视频形成三角。**教材经济，是 AI 泡沫溢出后最直接的受益品类之一**。

---

## 生态观察

**今日主线：3D 基础模型 + Agent CLI + Skills 生态。** `lingbot-map` 拉开了 3D 视觉基础模型的开源序幕，与语言/多模态基础模型形成"三足鼎立"格局；`opencode`、`kimi-cli` 与 Anthropic Skills 仓的同框出场，说明 **CLI Agent 已经不需要证明自己是主流入口**，问题变成生态分工——谁做协议、谁做工具、谁做能力包。

**次线：本地优先的 MCP 基础设施正在补齐。** `code-review-graph` 的代码知识图谱、`wigolo` 的本地搜索、`aws/agent-toolkit-for-aws` 的 MCP Server 官方集，共同指向一个方向——**"Agent 上下文"这层正在从 Cursor / Copilot 的云端 SaaS，被开源社区拉回到本地**。这是 MCP 协议真正开始改变工程实践的证据。

**冷清区：** 传统前端 / DevTool / 数据库仓库今日几乎没有进入前 15；`tldraw`、`lenis`、`context7` 处于中段。GitHub 的注意力份额被 AI 一侧几乎全部吸走——这与上周、上上周的分布一致。**当"给设计师做的 Skills 仓（ui-skills）"能挤进第 9 名，你就知道 Agent 已经开始蚕食设计师工具生态了**。
