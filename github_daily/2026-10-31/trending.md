# GitHub Trending 日报 · 2026-10-31

## 今日焦点

> **AI Agent Skills 生态爆发 · 持久化记忆/多代理协作 · 面向 AI 的开发工具链 · "情趣化"的学习与设计工具**
>
> - `obra/superpowers`、`mattpocock/skills`、`anthropics/skills`、`expo/skills` **四条 Skills 仓同时冲榜**，Agent Skills 正在从"实验玩法"变成一个有争夺的标准化栈。
> - `thedotmack/claude-mem` 和 `macro-inc/macro` 把 Agent 的"长期记忆/工作区"做成产品级能力。
> - `pbakaus/impeccable`、`JetBrains/thinkrail` 显示"AI 原生 IDE / 设计辅导"正在正规军化。
> - `HKUDS/DeepTutor`、`Renhuai123/ziwei-doushu` 一边是终身个性化学习，一边是传统命理工程化——Agent 应用触角继续外扩。
> - `lightpanda-io/browser` 持续为 AI/自动化场景提供 Zig 写的无头浏览器——基础设施层也在为 Agent 重写。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [obra/superpowers](https://github.com/obra/superpowers) | Agent 技能框架与软件工程方法学 | Shell | 309,386 | +1,255 | 27,519 |
| 2 | [mattpocock/skills](https://github.com/mattpocock/skills) | 作者的 `.agents` 工程技能集合 | Shell | 307,421 | +889 | 25,870 |
| 3 | [pbakaus/impeccable](https://github.com/pbakaus/impeccable) | 面向编码代理的设计词汇/缺陷检查工具 | Rust | 96,967 | +2,299 | 5,712 |
| 4 | [HKUDS/DeepTutor](https://github.com/HKUDS/DeepTutor) | 终身个性化 AI 辅导 | Python | 51,722 | +2,282 | 6,335 |
| 5 | [togg53192-cmd/jailbreaks](https://github.com/togg53192-cmd/jailbreaks) | 作者整理的 Jailbreak 清单 | — | 10,875 | +2,053 | 1,581 |
| 6 | [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | AI 代理持久化记忆：会话捕获+压缩+再注入 | TypeScript | 106,132 | +1,145 | 9,347 |
| 7 | [Renhuai123/ziwei-doushu](https://github.com/Renhuai123/ziwei-doushu) | 紫微斗数开源起盘引擎（算法+飞化+古籍） | TypeScript | 11,168 | +1,146 | 2,231 |
| 8 | [pingdotgg/t3code](https://github.com/pingdotgg/t3code) | Theo 发起的 T3 系编码代理项目 | TypeScript | 32,686 | +920 | 8,649 |
| 9 | [milind-soni/OpenMausBot](https://github.com/milind-soni/OpenMausBot) | 开源 Grok 式机器人+虚拟机环境 | TypeScript | 8,544 | +899 | 1,193 |
| 10 | [CopilotKit/OpenBot](https://github.com/CopilotKit/OpenBot) | 开源 AI 协作同事：自带浏览器/文件/工具 | TypeScript | 8,742 | +707 | 1,103 |
| 11 | [JetBrains/thinkrail](https://github.com/JetBrains/thinkrail) | JetBrains 轻量 vibe-coding IDE | TypeScript | 6,538 | +717 | 356 |
| 12 | [lightpanda-io/browser](https://github.com/lightpanda-io/browser) | Zig 实现、面向 AI/自动化的无头浏览器 | Zig | 38,302 | +652 | 1,868 |
| 13 | [anthropics/skills](https://github.com/anthropics/skills) | Anthropic 官方 Agent Skills 仓库 | Python | 185,259 | +287 | 21,891 |
| 14 | [macro-inc/macro](https://github.com/macro-inc/macro) | 邮件/聊天/文档/CRM 一体化 AI 工作区 | Rust | 5,844 | +117 | 537 |
| 15 | [expo/skills](https://github.com/expo/skills) | Expo & EAS 的 Agent Skills 集合 | Shell | 3,873 | +108 | 247 |

---

## 重点项目点评

### 🥇 [obra/superpowers](https://github.com/obra/superpowers) — 今日榜首，+1,255⭐

**"Skills 栈"正在从玩法变成行业标准**

Obra 的 `superpowers` 现在接近 **31 万星**、2.75 万 fork，和榜二 `mattpocock/skills`（也在 30 万+）一起把 "AI Agent 的工程技能框架" 做成了去年"dotfiles"级别的组织单位——不是文档，而是**一组可复用的 agent 指令 + 项目方法学 + 工具链入口**。它把过去散落在 `CLAUDE.md`、`.claude/skills/`、Rules、System Prompts 中的碎片，重新集中成"开发者自带的工具箱"。

今天 4 个 skills 相关仓同日冲榜（`superpowers`、`mattpocock/skills`、`anthropics/skills`、`expo/skills`）传递了两个信号：(1) 社区在用 fork 投票选"谁的 skills 更可用"；(2) 大厂（Anthropic、Expo）也进场抢赛道，意味着 skills 的格式/命名/发现机制有可能在未来 6 个月被工具标准化（像 `.editorconfig`/`.nvmrc` 那样）。

对普通开发者的实操意义：现在起花半小时 fork 一个主流 skills 仓并剪出自己的 `.claude/skills/` 已是性价比最高的 agent 升级路径。

---

### 🥈 [pbakaus/impeccable](https://github.com/pbakaus/impeccable) — +2,299⭐

**让 AI 不画出"丑陋 UI"的 lint**

`impeccable` 的卖点非常锋利：它是"**写给编码代理用的设计词汇表**"——内置设计评审（critique）/打磨（polish）/缺陷捕获（flaw detection）三类工具，强约束 AI 生成界面时的间距、层级、对比度、颜色系统，防止代码跑通但审美塌房。本质上是把"设计系统的 lint"内嵌进 agent 的决策循环。

今天 +2,299 的增速说明：开发者对"AI 做产品 = 产出几何正确但视觉灾难"的痛点共识正在爆发。Rust 写的工具 + 极简规范，使得它可以在不同 agent（Cursor、Claude Code、Codex）之间被当作"统一的审美裁判"调用。

---

### 🥉 [HKUDS/DeepTutor](https://github.com/HKUDS/DeepTutor) — +2,282⭐

**个性化 AI 辅导的"开源 Khanmigo 平替"**

香港大学 HKUDS 组的 `DeepTutor` 把"**终身化、按人塑模**的辅导"写成一个可私有部署的项目。核心价值在于：它不是"一次性 Q&A"的 tutor，而是维护长期学习档案、根据遗忘曲线和错题策略规划下一轮内容。这与行业里"面向学习者的 AI 系统 vs. 面向通用对话的 AI 系统"的分叉完全一致。

社区关注度高意味着：教育垂类的开源方案正在从"demo repo"升级到"可以上生产的 pipeline"。该项目的下一个判定节点是：能否吸纳本地 LLM、能否接入 Agent Skills 生态。

---

### 🏅 [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) — +1,145⭐

**长期记忆：Agent "Day-2 问题"的首选解法**

`claude-mem` 的卖点一句话——**捕获、压缩、再注入**：捕获会话活动，让关键事实/判断/状态经过结构化压缩后在未来会话里重新加载，解决 Claude Code 原生"每次 session 都是失忆症"的痛点。10 万+ 星的量级意味着这是本季度"Agent 的持久化记忆"最被认可的事实标准之一。

与之呼应的是 `macro-inc/macro`——把邮件/聊天/文档/日历/CRM 全部纳入"共享 AI 内存"的协作工作区。两者在不同抽象层回答同一个问题：**Agent 需要跨 session、跨团队的共享状态**。看谁最先成为 skills + memory 这条栈里的"默认持久化层"。

---

### 🎯 [lightpanda-io/browser](https://github.com/lightpanda-io/browser) — +652⭐

**Zig 版无头浏览器：AI 自动化的"下一代 Puppeteer"**

Lightpanda 从去年起就被 agent 开发者盯着：它用 **Zig 写、专为 AI/自动化优化**，比 Puppeteer/Playwright 显著更轻量，启动更快、内存更低。今天进榜的意义在于：当 agent 开始大规模调用浏览器完成任务（网页抓取、桌面网页操作、测试），常规 Chromium 的开销就撑不住并发。这是一条"AI 基础设施重写"的典型路径——传统工具因为新负载而被重新实现。

---

## 生态观察

本周 trending 的主旋律只有一个词：**Skills**。四条 Agent Skills 仓同日上榜本身就说明"从模型能力到工程能力"的拐点到了——开发者不再追 benchmark 排行，而是在拼"我拿到的 agent 用了什么样的方法学 / 工具栈"。另一条暗线是**Agent 的 Day-2 问题**（记忆、协作、浏览器、设计审美）正在被社区并行解决——`claude-mem`、`macro`、`lightpanda`、`impeccable` 四条垂直线共同指向"Agent 可以进入工作流了，但没有一个单一方案能覆盖"。再加上 `JetBrains/thinkrail`、`pingdotgg/t3code` 把 vibe-coding IDE 带进 trending，可以预判接下来两个月的 trending 会被这组"AI 原生工具链"占据主位。
