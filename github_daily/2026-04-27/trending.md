# GitHub Trending 日报 · 2026-04-27

## 今日焦点

> **Agent Skills 浪潮 · Claude Code 生态外延 · Computer-Use 基础设施 · Agent 长程记忆 · 攻防工具复兴**
>
> - `mattpocock/skills` 一夜 +2,507⭐ 登顶，Claude Skill 工程化进入"个人风格分发"阶段
> - `Alishahryar1/free-claude-code` +1,694⭐，把 Claude Code CLI 接到本地/免费模型的代理需求被点燃
> - `ComposioHQ/awesome-codex-skills` +518⭐，OpenAI Codex 阵营也学着搞 Skills 化包管理
> - `trycua/cua` +200⭐ 与 `gastownhall/beads` +133⭐，Computer-Use 与 Agent 长程记忆基础设施双线推进
> - `Z4nzu/hackingtool` 老项目 +1,724⭐ 反弹，Agent 时代的攻防自动化值得关注

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [mattpocock/skills](https://github.com/mattpocock/skills) | 真实工程师在用的 Agent Skills，从作者的 .claude 目录直接掏出来 | Shell | 22,949 | +2,507⭐ | 1,875 |
| 2 | [Z4nzu/hackingtool](https://github.com/Z4nzu/hackingtool) | All in one 黑客工具集合 | Python | 65,233 | +1,724⭐ | 7,314 |
| 3 | [Alishahryar1/free-claude-code](https://github.com/Alishahryar1/free-claude-code) | 在终端、VSCode 插件或 Discord 里免费跑 Claude Code | Python | 13,266 | +1,694⭐ | 1,921 |
| 4 | [codecrafters-io/build-your-own-x](https://github.com/codecrafters-io/build-your-own-x) | 从零复刻你最爱的技术，掌握编程 | Markdown | 496,696 | +1,074⭐ | 47,072 |
| 5 | [abhigyanpatwari/GitNexus](https://github.com/abhigyanpatwari/GitNexus) | 客户端代码知识图谱，提供交互式代码探索与 Graph RAG Agent | TypeScript | 30,052 | +667⭐ | 3,464 |
| 6 | [openclaw/openclaw](https://github.com/openclaw/openclaw) | "龙虾派"个人 AI 助手，跨任意 OS 与平台 | TypeScript | 364,508 | +620⭐ | 74,643 |
| 7 | [ComposioHQ/awesome-codex-skills](https://github.com/ComposioHQ/awesome-codex-skills) | 自动化工作流的 Codex skills 精选集 | Python | 1,898 | +518⭐ | 156 |
| 8 | [PostHog/posthog](https://github.com/PostHog/posthog) | 一体化开发者平台：产品分析、会话回放、错误追踪、特性开关 | Python | 33,771 | +338⭐ | 2,626 |
| 9 | [trycua/cua](https://github.com/trycua/cua) | Computer-Use Agent 的开源基础设施：沙箱、SDK、benchmark | HTML | 14,321 | +200⭐ | 895 |
| 10 | [gastownhall/beads](https://github.com/gastownhall/beads) | 给 Coding Agent 的"内存升级"——基于 Dolt 的依赖图任务系统 | Go | 21,608 | +133⭐ | 1,436 |
| 11 | [home-assistant/core](https://github.com/home-assistant/core) | 把本地控制和隐私放在第一位的开源家庭自动化 | Python | 86,438 | +52⭐ | 37,356 |
| 12 | [curl/curl](https://github.com/curl/curl) | 多协议 URL 数据传输的命令行工具与库 | C | 41,498 | +50⭐ | 7,153 |
| 13 | [microsoft/typescript-go](https://github.com/microsoft/typescript-go) | TypeScript 原生 Go 端口的开发暂存仓库 | Go | 25,142 | +38⭐ | 916 |

---

## 重点项目点评

### 🥇 [mattpocock/skills](https://github.com/mattpocock/skills) — 今日榜首，+2,507⭐

**TypeScript 教父把自己的 .claude 目录公开了**

Matt Pocock 是 TypeScript 教学圈最有影响力的内容创作者之一。他这次直接把"实战工程师在用的 Claude Skills"从自己的 `.claude` 目录里掏出来开源——内容覆盖从对话拆需求成 PRD、TDD 流程化、到代码架构改进等具体任务。这种"个人 dotfiles 风格的 Skills 分发"形态，正在和过去一周热度居高不下的 `awesome-claude-skills` 类整理仓互相强化。

它能一夜暴涨 2,500+ 星的核心原因，是 Anthropic 的 Skills 机制把"如何使用 Claude"从单纯的 system prompt 工程，变成了"可分发、可组合、可被 LLM 自动调用"的运行时模块。当顶级开发者开始批量贡献自己的工作流，Skills 就具备了类似早年 Vim/Emacs 配置生态的扩散动能：你不需要从零调教，只需要 fork 一份"别人证明过有效"的工作流。

可以预期下周还会有更多名人开发者把 `.claude/skills` 拿出来公开——Skills 正在变成新一代的 dotfiles。

---

### 🥈 [Alishahryar1/free-claude-code](https://github.com/Alishahryar1/free-claude-code) — +1,694⭐

**Claude Code 太好用，所以有人开始想办法不付钱用它**

这个仓库本质是一个透明代理：拦截 Claude Code CLI/VSCode 扩展发往 Anthropic 的请求，转发给免费/本地的 LLM 提供方——NVIDIA NIM 免费档（40 RPM）、OpenRouter、DeepSeek，以及 Ollama、LM Studio 等本地方案。

这个项目能爆，反而是 Claude Code 产品力的反向证明：Claude Code 的命令面板、文件 diff、TodoWrite、Skills 等交互层做得太好，以至于即使后端模型换成开源模型，用户也依然想保留这个"前端"。换句话说，**Claude Code 正在变成 Agent IDE 的事实标准**，模型只是它的可替换组件。

这条赛道短期内会面临 Anthropic 的反制（可能是协议层校验、设备绑定、或更激进的 Skills 服务端化），值得持续盯。但它也提示自托管 Coding Agent 圈：与其重新造一个 IDE 壳子，不如直接做 Claude Code 兼容协议。

---

### 🥉 [Alishahryar1/free-claude-code](https://github.com/ComposioHQ/awesome-codex-skills) — +518⭐

**OpenAI Codex 学着 Anthropic 搞 Skills 包管理**

Composio 这家做 Agent 工具集成的公司，推出了一份 Codex Skills 精选集——把"Codex 该如何完成某类任务"打包成模块化指令包，配合 Composio CLI 一键调用 Slack、GitHub、Notion 等 1000+ 应用。仓库名直接致敬"awesome-claude-skills"，意图非常明显：**Skills 化的 Agent 工作流分发，正在成为各家平台必须跟上的标准。**

值得注意的是，OpenAI 在 GPT-5 时代主要把工具能力封装在 Custom GPTs 与 Assistants API 里，但那些方案对开发者并不友好——版本控制差、本地不可分发、与 IDE 隔离。Composio 这种第三方插件的快速崛起，说明社区正在用脚投票，要求 OpenAI 在 Codex 端给出和 Claude Skills 对等的"文件即模块"开放路径。

---

### 🏅 [trycua/cua](https://github.com/trycua/cua) — +200⭐

**Computer-Use Agent 的"水电煤"基础设施**

cua 提供了一整套让 AI Agent 自主控制电脑的底层组件：macOS 后台自动化的 Cua Driver、跨 OS 的 Agent Sandbox、多 Agent 协调的 CuaBot、benchmark 工具 Cua-Bench、macOS VM 管理 Lume。它瞄准的是"看屏幕、点按钮、完成任务"这一类无需专用 API 即可工作的通用智能体。

Anthropic Computer Use 与 OpenAI Operator 都把"屏幕级操作"推到了产品层，但底层执行环境（怎么安全地给 Agent 一台机器、怎么回滚状态、怎么拿到客观分数）目前没有清晰赢家。cua 选择以 macOS 为主战场，避开了 Windows/Linux 拥挤的虚拟化赛道，错位竞争。如果 Claude Code/Codex 接下来继续把 Computer Use 嵌入终端工作流，cua 这种横向基础设施层的价值会放大。

---

### 🏅 [gastownhall/beads](https://github.com/gastownhall/beads) — +133⭐

**Coding Agent 长任务记忆问题的工程化方案**

Beads 把"Agent 在长任务里到底记得什么"这个问题，从 markdown 计划升级成了基于 Dolt（Git 风格的版本化数据库）的依赖图任务系统。它的卖点很硬：自动判断任务就绪、基于 hash ID 的无冲突协作、语义级记忆压缩——目标是让 Agent 在跨天、跨 session 的长程任务中保持一致。

它的爆款契机和 `beads`、`gitnexus` 这一类"给 Agent 加外挂记忆"的项目同源：Claude Code/Codex 等 Agent 在"几百轮对话内"已经够用，但要走向"几周一个 epic"就必须把记忆从 prompt 里搬出来。Dolt 这种带版本的存储后端是巧妙选择——天然 fit "Agent 改一改、可回滚、可 review"的工作模式。

---

## 生态观察

今天榜单的主旋律毫不含糊：**Claude Skills 正在快速形成生态飞轮**——从 mattpocock 的个人配置，到 Composio 学着给 Codex 做对位产品，再到 Free-Claude-Code 这种"我只想要前端但模型自由"的逆向需求，都在围绕"AI Coding Agent 的工作流标准化"这一主题展开。

底层基础设施这一层也在同步推进：cua 解决"Agent 怎么用电脑"，beads 解决"Agent 怎么记事情"，GitNexus 解决"Agent 怎么读代码"——这三件事过去一年都被各家产品自己内部硬编码，今天开始有专业化、可独立分发的开源组件出现。这意味着 2026 年的 Coding Agent 拼图，已经不再是"哪家模型更强"，而是"哪家把这些外接组件拼得更好"。

老牌项目 `hackingtool`、`build-your-own-x`、`curl`、`home-assistant` 同时在榜，更像是榜单基本盘——但 `hackingtool` 一日 +1,700 星的反弹值得留意，**Agent 时代的红蓝队工具复兴**可能是接下来一个隐形主题。
