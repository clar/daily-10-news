# GitHub Trending 日报 · 2026-10-25

## 今日焦点

> **Claude Skills 生态爆发 · AI Agent 安全运行时 · "设计语言为 AI 服务" · 中国本土项目逆势出圈 · 具身智能开源化**
>
> - `cloudflare/security-audit-skill` **+2,271⭐** — Cloudflare 首个官方 Claude Skill 爆红
> - `NVIDIA/OpenShell` **+893⭐** — Nvidia 推出 Agent 安全沙箱运行时，直接对标 E2B
> - `SnailSploit/Claude-Red` **+770⭐** — 攻击面 Skill 库引发安全圈关注
> - `pbakaus/impeccable` **+733⭐** — "给 AI 用的设计系统"概念被 Google 前设计总监带火
> - `Renhuai123/ziwei-doushu` **+635⭐** — 紫微斗数开源算法引擎意外霸榜中文圈

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) | 多阶段安全审计 Claude Skill | JavaScript | 44,409 | +2,271 | 2,763 |
| 2 | [NVIDIA/OpenShell](https://github.com/NVIDIA/OpenShell) | 自主 Agent 的安全私有运行时 | Rust | 19,441 | +893 | 1,930 |
| 3 | [SnailSploit/Claude-Red](https://github.com/SnailSploit/Claude-Red) | 攻击性安全 Skill 精选库 | Python | 8,833 | +770 | — |
| 4 | [pbakaus/impeccable](https://github.com/pbakaus/impeccable) | 让 AI 做出更好设计的设计语言 | Rust | 86,341 | +733 | 5,152 |
| 5 | [Renhuai123/ziwei-doushu](https://github.com/Renhuai123/ziwei-doushu) | 紫微斗数算法引擎与参考数据 | TypeScript | 7,253 | +635 | — |
| 6 | [Nutlope/hallmark](https://github.com/Nutlope/hallmark) | 给 Claude/Cursor/Codex 用的设计 Skill | CSS | 32,068 | +570 | 1,647 |
| 7 | [makecindy/cindy](https://github.com/makecindy/cindy) | 开箱即用的开源 AI Agent | TypeScript | 4,055 | +471 | 582 |
| 8 | [luongnv89/claude-howto](https://github.com/luongnv89/claude-howto) | Claude Code 可视化示例手册 | Python | 44,501 | +442 | 5,487 |
| 9 | [pollen-robotics/microduck](https://github.com/pollen-robotics/microduck) | 开源微型双足机器鸭 | Rust | 10,943 | +381 | 1,405 |
| 10 | [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | 跨会话压缩+注入上下文的 Memory | TypeScript | 102,808 | +274 | — |
| 11 | [jbiaojerry/ebook-treasure-chest](https://github.com/jbiaojerry/ebook-treasure-chest) | 多家中文读书 App 书籍聚合链接 | Python | 22,569 | +220 | 3,187 |
| 12 | [bendlang/bend](https://github.com/bendlang/bend) | 用形式化证明阻挡 AI 犯错的编程语言 | TypeScript | 24,113 | +113 | — |
| 13 | [pollen-robotics/microduck_rl](https://github.com/pollen-robotics/microduck_rl) | Microduck 的强化学习训练环境 | Python | 2,611 | +41 | — |
| 14 | [google-gemini/gemini-cli](https://github.com/google-gemini/gemini-cli) | 把 Gemini 带入终端的开源 Agent | TypeScript | 108,007 | +38 | 14,805 |
| 15 | [aws/agent-toolkit-for-aws](https://github.com/aws/agent-toolkit-for-aws) | 官方 AWS MCP Servers & Skills 集 | Python | 3,106 | +11 | 397 |

---

## 重点项目点评

### 🥇 [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) — 今日榜首，+2,271⭐

**Claude Skills 从社区实验走向大厂官方背书**

Cloudflare 今天开源的 `security-audit-skill` 是其第一个真正意义上的"官方 Claude Skill"——不是 MCP server，不是 workflow，而是直接遵循 Anthropic 10 月初发布的 Skills 规范（`SKILL.md` + 子脚本的目录结构）。该 Skill 内置多阶段流程：代码扫描 → 依赖图分析 → OWASP Top10 自检 → 修复建议 PR → 回归测试。启动后它会先调用 Cloudflare 自有的 Radar/Threat Intel 数据库，再接入项目本身的测试基础设施。

爆火的原因是双重的：（1）这是第一个由 Cloudflare 这类 Tier-1 云厂商正式贡献的 Skill，向整个开源社区发出"Skills 规范已站稳"的信号；（2）它直接把安全扫描变成"写几行命令让 Agent 来做"的形态，让此前只能靠 Snyk/Semgrep 等商用 SaaS 的中小团队有了平替。可以预见未来 2–3 个月，GCP、Azure、Datadog 等大厂都会跟进自己的官方 Skill 包。

---

### 🥈 [NVIDIA/OpenShell](https://github.com/NVIDIA/OpenShell) — +893⭐

**Nvidia 直接下场做 Agent 运行时，和 E2B / Daytona 正面开战**

OpenShell 是一个用 Rust 写的"Agent 专用安全沙箱 shell"：它向上为 Agent 暴露类 bash 接口，向下用 microVM + rootless container 把每条命令隔离在一个受限 namespace 里，并记录完整审计日志。Nvidia 的切入角度相当精明：GPU 云 + Agent 运行时 + 推理服务三位一体，让客户在 Nvidia 的基础设施上跑 Agent 时，不再需要再去自己拼 Kata/Firecracker。

从技术栈看，OpenShell 的 Rust+microVM 组合几乎就是在复刻 E2B 的架构。它选择用 Apache 2.0 协议开源而非厂商专属 SDK，摆明了要把这块变成 commodity——真正值钱的是上面跑的 GPU 账单。E2B、Daytona、Modal 等 Agent 运行时创业公司今天估计正坐在会议室里重新定战略。

---

### 🥉 [SnailSploit/Claude-Red](https://github.com/SnailSploit/Claude-Red) — +770⭐

**红队 Skill 库：Claude Skills 的"暗面"开始形成**

Claude-Red 定位为 "offensive security skills"：一整套面向渗透测试、CTF、红队演练的 Claude Skill 集合，内含子域名爆破、WAF 绕过、二进制符号化分析、恶意 PDF 构造等多个方向。虽然作者在 README 顶部明确声明"仅用于授权测试"，但这个仓库的星数曲线仍然引起了 HN 和 Reddit /r/netsec 的激烈讨论——Skills 的"可编排性"使得组合不同的攻击 Skill 变得前所未有的简单，社区正在用脚投票地测试 Anthropic Trust & Safety 的边界。

与 Cloudflare 官方防御向 Skill 并列登榜说明一件事：**Skills 生态同时打开了攻击者和防御者的工具箱**，并且攻击面的创作者比防御者更有分享动机。这对 Anthropic 的下一步 Skill Marketplace 治理策略提出了直接问题。

---

### 🎨 No.4 · [pbakaus/impeccable](https://github.com/pbakaus/impeccable) — +733⭐

**"为 AI 服务的设计语言"：从 Material 到 Impeccable 的世代切换**

Paul Bakaus（前 Google Chrome DevRel 和 AMP 产品设计师）发布的 Impeccable 不是又一套 UI Kit——它定义了一组"AI 友好的设计约定"：颜色命名用语义而非色号、layout 用相对比例而非像素、交互语义用动词短语标记、组件文档用 YAML 可被 Agent 消费。目标是让 Claude、Cursor、v0 这类 AI 工具生成的页面"开箱就看起来 impeccable"。

这个方向本身比项目本身更有意义。过去 15 年设计系统（Material、Tailwind、Shadcn）都是"写给人的"；而当代码 90% 由 Agent 生成，设计系统的 primary consumer 已经悄悄换成了 LLM。impeccable 和同样登榜的 `Nutlope/hallmark`（+570⭐）走的是同一条赛道——**设计系统正在被重写一遍，这一次读者不是前端工程师，而是 Agent**。

---

### 🧠 No.5 · [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) — +274⭐（累计 102,808⭐）

**跨会话记忆：Agent "持久化"问题的又一次尝试**

claude-mem 的核心机制是：每一次 Claude 会话结束时，自动将关键事件、代码变更、决策理由压缩成结构化 memory artifact，并在下次启动时按需注入上下文。它不依赖 Claude Code 自带的 memory 功能，而是独立运行在用户侧的 CLI/插件，适配面更广。10 万+ Star 本身说明"Agent 的记忆不够用"这个问题远没有被 Anthropic 原生解决。

有意思的是，Anthropic 近期的产品路径（Projects 文件夹、Memory tool、Sub-agents）都在避免做"永久 state"，试图保持"每个会话仍是 stateless"的架构美学；但社区的实际需求是：**我希望昨晚那个 Agent 今天还记得我们改了什么**。claude-mem 的持续热度告诉所有做 Agent 创业的公司：解决记忆问题不是 nice-to-have。

---

## 生态观察

今天的 15 个 trending 项目里，**有 9 个直接服务于 Claude Code / Agent 生态**（Cloudflare Skill、OpenShell、Claude-Red、hallmark、cindy、claude-howto、claude-mem、gemini-cli、aws/agent-toolkit），一个围绕"Agent 友好的设计系统"（impeccable、hallmark），一个是具身智能开源（microduck + microduck_rl）。

- **Claude Skills 规范是今日最大赢家。** Cloudflare 的官方 Skill 把这个规范推进到"大厂背书"阶段；Claude-Red 则说明攻击面 Skill 的生态也在形成。可以预见未来一个月内各大安全厂商都会出官方 Skill。
- **Agent 运行时市场正在被巨头收编。** Nvidia OpenShell、AWS agent-toolkit 同日登榜，两条路径——Nvidia 做 sandbox 运行时、AWS 做 MCP 服务目录——正在从不同方向吞并曾经属于 E2B/Daytona/Modal 的空间。
- **设计系统进入"AI primary consumer"时代。** impeccable 和 hallmark 两个高星项目预示 2027 年的新设计系统标准会被重写，Material 3 和 shadcn 都需要出一个"AI-native"版本。
- **中国本土项目在中文 Spoken Language 过滤之外首次占据高位。** `Renhuai123/ziwei-doushu`（紫微斗数）和 `jbiaojerry/ebook-treasure-chest`（中文电子书聚合）都登上全局榜，说明中文开发者正在不惜用英文 README 争取全球曝光。
- **具身智能继续开源化。** Pollen Robotics 的 `microduck` 和 `microduck_rl` 两个仓库连续登榜，和昨天 HN 上 Dream-1 World Action Model 的热度形成呼应——**可编程机器人 + 开源硬件**是 2026 年底的新一波开发者热点。

今日生态关键词：**Skills 规范化、运行时商品化、设计系统 AI 化、机器人硬件开源化。**
