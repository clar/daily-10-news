# GitHub Trending 每日报告 · 2026-04-26

## 今日焦点

> **Claude 生态爆发 · 技能（Skills）共享浪潮 · HuggingFace 开源 ML Agent · API 代理灰色地带 · 学习类经典长青**
>
> - `Alishahryar1/free-claude-code` 一夜暴涨 +3,975⭐ 登顶，本质是把 Claude Code 路由到第三方/本地模型的"白嫖"代理
> - `mattpocock/skills` +857⭐ 把个人 `.claude` 目录开源，引发整个社区"晒技能"的二次创作风潮
> - `huggingface/ml-intern` +1,236⭐ HuggingFace 亲自下场做"读论文、训模型、上线模型"的开源 ML 工程师 Agent
> - `codecrafters-io/build-your-own-x` +1,431⭐ 老牌学习仓库再次抬头，半工龄程序员的"从零造轮子"圣经
> - `Z4nzu/hackingtool` +1,200⭐ 渗透测试工具箱继续吸引大量好奇心驱动型 star

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [Alishahryar1/free-claude-code](https://github.com/Alishahryar1/free-claude-code) | 让 Claude Code 在终端、VSCode、Discord 中"免费"运行 | Python | 11,297 | +3,975⭐ | 1,670 |
| 2 | [mattpocock/skills](https://github.com/mattpocock/skills) | 个人 `.claude` 技能目录开源 | Shell | 19,647 | +857⭐ | 1,643 |
| 3 | [Z4nzu/hackingtool](https://github.com/Z4nzu/hackingtool) | 一站式渗透测试工具箱 | Python | 63,634 | +1,200⭐ | 7,132 |
| 4 | [PostHog/posthog](https://github.com/PostHog/posthog) | 产品分析、会话回放、特性开关一体化平台 | Python | 33,428 | +469⭐ | 2,599 |
| 5 | [davila7/claude-code-templates](https://github.com/davila7/claude-code-templates) | Claude Code 配置与监控 CLI | Python | 25,304 | +78⭐ | 2,524 |
| 6 | [deepseek-ai/DeepEP](https://github.com/deepseek-ai/DeepEP) | 高效专家并行通信库 | Cuda | 9,473 | +189⭐ | 1,193 |
| 7 | [PowerShell/PowerShell](https://github.com/PowerShell/PowerShell) | 跨平台 PowerShell | C# | 53,022 | +68⭐ | 8,295 |
| 8 | [RooCodeInc/Roo-Code](https://github.com/RooCodeInc/Roo-Code) | 编辑器内的 AI 开发团队 | TypeScript | 23,480 | +55⭐ | 3,118 |
| 9 | [huggingface/ml-intern](https://github.com/huggingface/ml-intern) | 读论文、训模型、上线模型的开源 ML 工程师 Agent | Python | 6,144 | +1,236⭐ | 554 |
| 10 | [codecrafters-io/build-your-own-x](https://github.com/codecrafters-io/build-your-own-x) | 通过造轮子精通编程 | Markdown | 495,845 | +1,431⭐ | 46,986 |
| 11 | [CJackHwang/ds2api](https://github.com/CJackHwang/ds2api) | 协议转换中间件，多账号轮询，Docker 部署 | Go | 1,384 | +37⭐ | 445 |
| 12 | [Universal-Commerce-Protocol/ucp](https://github.com/Universal-Commerce-Protocol/ucp) | 通用商务协议规范与文档 | Python | 2,759 | +16⭐ | 347 |
| 13 | [ComposioHQ/awesome-codex-skills](https://github.com/ComposioHQ/awesome-codex-skills) | CLI/API 平台自动化技能精选集 | Python | 1,411 | +174⭐ | 128 |

---

## 重点项目点评

### 🥇 [Alishahryar1/free-claude-code](https://github.com/Alishahryar1/free-claude-code) — 今日榜首，+3,975⭐

**Claude Code 上桌之后，"白嫖代理"正在快速成为一个独立赛道**

这个项目本质是一个轻量级反向代理：拦截 Claude Code 客户端发出的 Anthropic API 请求，转发给 NVIDIA NIM、OpenRouter、DeepSeek、LM Studio、llama.cpp 等替代后端，并把对方的"思考"格式翻译成 Claude 原生的 thinking block。它支持按模型分流（Opus 走一家、Sonnet 走另一家），还附带 Discord/Telegram 远程触发 bot——单从工程完整度看，作者不是随手糊一个 demo。

它能一夜上 +3,975⭐ 是非常典型的"灰色地带流量"特征：Claude Code 用户基数已经膨胀到一定规模，付费成本积累起来不是小数目，社区里"如何降低 token 开销"的讨论早就溢出。但这种代理同时绕过了 Anthropic 的计费链路，存在明显的 ToS 风险，目前看仅作为个人本地开发使用。

更深层的信号是：**Claude Code 本身已经事实上变成了一个开源前端协议**——客户端、技能（skills）、子 agent 的通信结构稳定到足以被第三方 fork、reroute、扩展。今天的榜单上有四个项目都围绕 Claude Code 的扩展生态展开，这件事本身比任何单一项目的 star 数都更值得关注。

---

### 🥈 [huggingface/ml-intern](https://github.com/huggingface/ml-intern) — +1,236⭐

**HuggingFace 终于把"开源 Cursor for ML"这件事给做了**

ml-intern 是一个面向机器学习工程师的开源 Agent，定位是"读论文、训模型、上线模型"。架构上是非常成熟的现代 Agent 范式：单 agentic loop（最多 300 轮迭代）+ 工具路由器（HuggingFace 文档/数据集/repo/沙箱）+ 上下文管理器（170k token 触发自动压缩）+ 死循环检测器，支持 MCP 扩展，session 直接 push 到 HuggingFace 持久化。

放到今年的 ML 工程语境下看，这是 HuggingFace 对 OpenAI Codex / Claude Code 在传统软件领域成功之后的官方回应——把 Agent 从"写代码"扩展到"做完整 ML 项目"。和通用 coding agent 相比，ml-intern 真正的差异在于工具集：它原生集成了 HF 的论文、模型、数据集索引，而不是把这些东西当作普通的网页去爬。

值得 ML 工程师认真看一眼的是它的 **doom loop detector** 和 **170k 触发的上下文压缩策略**，这两点是当前 Agent 类项目最容易翻车的地方，HuggingFace 这套实现可以直接当作参考工程。

---

### 🥉 [mattpocock/skills](https://github.com/mattpocock/skills) — +857⭐

**"晒 .claude 目录"已经从 meme 演变成正式的内容形态**

Matt Pocock 是 TypeScript 圈子里以教学内容著称的工程师，他把自己日常使用的 Claude 技能目录开源，覆盖：规划与设计（对话转 PRD、设计访谈）、开发（TDD 工作流、bug 分诊、架构改进）、工具（git hooks）、写作（文章编辑、术语提取、Obsidian 笔记）。

之所以能在一天内涨 +857⭐，原因不是技能本身有多惊艳，而是因为 **"开源个人技能目录"正在变成新一代开发者博客**——过去是写一篇博客分享某个工作流，现在是直接把可执行的、机器可调用的 prompt + skill 放出来。今天榜单上的 `ComposioHQ/awesome-codex-skills`、`davila7/claude-code-templates` 都是同一现象的不同形态。

这种"工作流即代码"的趋势，对于第三方工具厂商是机会（template marketplace 即将爆发），对于个人开发者则是低成本建立影响力的新通路——以前需要一个完整产品才能立足，现在一个高质量 skills 仓库就能拿到上万 star。

---

### [codecrafters-io/build-your-own-x](https://github.com/codecrafters-io/build-your-own-x) — +1,431⭐

**经典学习仓库的"周期性回涨"，背后是一代人对底层失去耐心的反弹**

这个仓库从 2018 年开始就是 GitHub 上长期排名前列的资源型项目，今天再次出现在 trending 上、单日 +1,431⭐，并不是因为内容更新，而是因为周期性的话题驱动（通常是社交媒体上的"AI 让你不再理解底层"类讨论触发的二次曝光）。

它的核心结构非常简单：按"造一个 X"分类（造一个数据库、造一个 git、造一个浏览器、造一个 OS），每条链接到一系列详细教程。在 AI Agent 写代码越来越容易的今天，**手动复刻底层系统反而成了少数能让人真正理解 trade-off 的方式**——榜单上同时出现 Claude Code 代理、ML Agent 和"造轮子"教程，构成了一个非常典型的当下心态切片。

---

### [Z4nzu/hackingtool](https://github.com/Z4nzu/hackingtool) — +1,200⭐

**安全/红队工具箱的常态化曝光**

这是一个 ALL-IN-ONE 的渗透测试工具集合（信息收集、社工、Web、密码、Wi-Fi、漏洞扩展等），总 star 已经 6.3 万。它能稳定登榜的核心原因之一是**好奇心驱动 star**——大量观众属于"先收藏不一定会用"的群体，加上各种 YouTube/Bilibili 安全频道的循环引流，每隔一段时间就会有一波集中曝光。

工程层面没有特别新意，但作为"安全入门工具索引"它的索引价值依然在，且对教学/比赛场景友好。提一句：里面集成的部分工具的合法使用边界需要使用者自行把握，这类项目真正的争议点从来不是代码，而是分发方式。

---

## 生态观察

今天的榜单有非常清晰的两条主线：

1. **Claude Code 的"事实标准化"**。免费代理、模板 CLI、技能目录、awesome 列表四种形态同时上榜，说明 Claude Code 已经不只是 Anthropic 的一个产品，而是一个被社区接管和扩展的开放生态。这和当年 VSCode 走向"实质上的编辑器协议"是同一种轨迹，只是周期更短。

2. **Agent 工程化 + 模型基础设施**。HuggingFace 推出 ml-intern 是今天最有分量的"严肃工程"消息；DeepSeek 持续输出基础设施级别的 DeepEP 通信库；Roo-Code 维持在编辑器内多 agent 协作方向。这一拨项目共同特征是不再靠 demo 视频驱动，而是靠工程细节（context 压缩、doom loop 检测、专家并行）说话。

冷却的一面：纯 LLM "wrapper"型项目今天几乎没有进入主榜，单纯靠"我做了一个 ChatGPT for X"的获星模式正式终结。能登榜的，要么提供基础设施（代理、通信库、平台），要么提供原生工作流（skills、templates），要么提供学习内容（build-your-own-x）。这是一个相对健康的信号。
