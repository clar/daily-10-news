# GitHub Trending 每日报告 · 2026-11-08

## 今日焦点

> **Agent Skills 大爆发 · AI 代码审计官方化 · AI 浏览器 Agent · 上下文压缩 · 社会化开源社群**
>
> - `cloudflare/security-audit-skill` 单日 +2,088⭐，成为"官方背书的 Agent Skill"典型案例。
> - `anthropics/skills` 和 `mattpocock/skills`、`google/skills` 同日入榜，Skill-as-a-Package 已形成事实标准。
> - `vercel-labs/agent-browser` 为 AI Agent 提供 Rust 原生浏览器控制层，开源 Agent 浏览器赛道升温。
> - `milind-soni/OpenMausBot` 开源对标 Grok Bot，+1,986⭐，一键自建"AI 虚拟人"热度显著。
> - `ranxianglei/billion-context` 用上下文压缩在单会话节省约 5x token，长会话经济学吸引眼球。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) | 多阶段安全审计 Agent Skill，产出结构化发现 | JavaScript | 65,605 | +2,088⭐ | 4,261 |
| 2 | [milind-soni/OpenMausBot](https://github.com/milind-soni/OpenMausBot) | Grok Bot 的开源替代，含机器人虚拟机 | TypeScript | 16,897 | +1,986⭐ | 2,391 |
| 3 | [sherlock-project/sherlock](https://github.com/sherlock-project/sherlock) | 用用户名跨平台定位社交账号 | Python | 100,346 | +1,819⭐ | 11,858 |
| 4 | [zed-industries/zed](https://github.com/zed-industries/zed) | 高性能、多人协作代码编辑器 | Rust | 94,243 | +1,119⭐ | 11,551 |
| 5 | [mattpocock/skills](https://github.com/mattpocock/skills) | 作者个人 agents 目录汇集的工程 Skill 集 | Shell | 317,634 | +1,111⭐ | 26,572 |
| 6 | [google/skills](https://github.com/google/skills) | Google 产品与技术的 Agent Skills | Python | 23,351 | +449⭐ | 1,950 |
| 7 | [anthropics/skills](https://github.com/anthropics/skills) | Anthropic 官方 Agent Skills 开源库 | Python | 188,732 | +386⭐ | 22,247 |
| 8 | [astral-sh/ruff](https://github.com/astral-sh/ruff) | Rust 写的高速 Python linter/formatter | Rust | 50,958 | +350⭐ | 2,628 |
| 9 | [prometheus/prometheus](https://github.com/prometheus/prometheus) | 监控系统与时序数据库 | Go | 67,432 | +325⭐ | 11,001 |
| 10 | [meta/astryx](https://github.com/meta/astryx) | 面向 Agent 的可定制设计系统 | TypeScript | 14,439 | +185⭐ | 1,179 |
| 11 | [ranxianglei/billion-context](https://github.com/ranxianglei/billion-context) | 长会话上下文压缩插件 | TypeScript | 4,578 | +185⭐ | 366 |
| 12 | [mbillow/localthings](https://github.com/mbillow/localthings) | 本地局域网控制三星家电 | Python | 1,038 | +184⭐ | 111 |
| 13 | [tailwindlabs/tailwindcss](https://github.com/tailwindlabs/tailwindcss) | utility-first CSS 框架 | TypeScript | 98,435 | +181⭐ | 7,103 |
| 14 | [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) | 面向 AI Agent 的浏览器自动化 CLI | Rust | 46,773 | +180⭐ | 3,204 |
| 15 | [dsx-ai-factory/nvke](https://github.com/dsx-ai-factory/nvke) | 裸机 GPU Kubernetes 管理平面 | Go | 533 | +125⭐ | 86 |

---

## 重点项目点评

### 🥇 [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) — 今日榜首，+2,088⭐

**Cloudflare 首次把"安全审计"打成一个官方 Agent Skill**

这是 Cloudflare 把内部安全工程经验封装成 Agent Skill 的结果：一个多阶段审计工作流（扫描 → 验证 → 报告），每条发现都带有机器可读的 verdict 字段（CONFIRMED / PLAUSIBLE）和复现脚本。它直接匹配 Claude Code / Cursor 等 Agent 的工具调用协议，开发者只要把目标仓库路径交给 Agent，就能自动得到一份对标 pentester 的报告。

今日 +2,088⭐ 的增速在非 LLM 核心框架里罕见，核心原因是 Cloudflare 的品牌加持 + Agent Skill 这一形态正处于"杀手级范式"的 S 曲线早期。它也验证了一件事：**Agent 时代的开源单元不是"库"，而是"可被 Agent 调度的 Skill 包"**。随着 Anthropic、Google、Vercel 都在同期扩展自己的 skills 生态，这种标准化、可组合的 skill 正在复刻 Docker 镜像之于微服务的角色。

---

### 🥈 [milind-soni/OpenMausBot](https://github.com/milind-soni/OpenMausBot) — +1,986⭐

**开源 Grok Bot 替代，自带"机器人虚拟机"**

OpenMausBot 直接把自己定位为 xAI Grok Bot 的开源对标：一个可自托管的 AI 虚拟角色平台，内置轻量 VM 供机器人执行代码、浏览和多步推理，预设角色模板可用 YAML 一键换皮。它与早期的 AutoGPT / BabyAGI 不同——目标是"多角色、长周期、可商用的自建 AI 伙伴"，而不是单次 Agent 运行。

近两天爆红的直接触发因素是 xAI 近期把 Grok Bot 的"虚拟人"功能限制在订阅用户，OpenMausBot 刚好填补开源替代空白。更深层的信号是：**去中心化 AI 伙伴**在 Reddit、X、Discord 的创作者社区内成为明确需求，社区希望摆脱大厂的内容政策约束。TS 栈 + 可移植 VM 的选择也让它有机会被嵌入到各种社群机器人。

---

### 🥉 [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) — +180⭐（新发布）

**Vercel 入局 AI 浏览器 Agent 层**

Vercel Labs 开源的 Rust CLI，面向 AI Agent 提供细粒度浏览器控制：读取 DOM、点击、表单填写、脚本注入、截图，输出结构化 JSON 供模型消费。相比 Playwright/Puppeteer，它针对 Agent 的调用模式做了专门优化——操作幂等、错误自动修正、显式的"waiting 状态语义"——并且和 Vercel AI SDK 的 tool-use 协议天然对齐。

它赶上的是 2026 年的"浏览器 Agent 军备竞赛"：OpenAI Operator、Anthropic Computer Use、Google Project Mariner 都在推"Agent 自己用浏览器"的愿景，但官方工具都是服务型闭源。Vercel 的切入点是开发者可本地跑、能嵌入任意 Next.js 项目的开源方案，直接在应用侧和闭源方案抢流量。本周发布就上榜，说明"开源 Agent 浏览器"的开发者需求已然成熟。

---

### 🏅 No.4 · [anthropics/skills](https://github.com/anthropics/skills) · [google/skills](https://github.com/google/skills) · [mattpocock/skills](https://github.com/mattpocock/skills) — 合计 +1,946⭐

**Skills 生态今天三馆同日入榜**

今天最有信息量的现象，是三个 `*/skills` 仓库在同一天登上 trending：Anthropic 官方、Google 官方、以及个人工程师 Matt Pocock 的汇编库。再加上第一名的 Cloudflare 安全审计 skill，可以断言：**Agent Skill 包已经成为 2026 Q4 最活跃的开源原语**。

三者有互补定位：Anthropic 提供 Claude Code / Agent SDK 的参考实现；Google 推与 Workspace、Cloud、Firebase 的集成 skill；Matt Pocock 的仓库则更面向日常软件工程习惯（git 工作流、测试、重构）。Skill 的"可发现、可组合、可声明依赖"的特性正在被 package manager 化——npm / PyPI 之后，Agent Hub / Skill Registry 的雏形呼之欲出。

---

### 🧠 No.5 · [ranxianglei/billion-context](https://github.com/ranxianglei/billion-context) — +185⭐

**把长会话 token 砍掉 5 倍的上下文压缩插件**

来自中国独立开发者的上下文压缩插件，核心思路是"分层摘要 + 关键事实抽取 + 原文按需召回"，宣称在长会话中 token 使用量平均降至原来的 20%。相比前几个月流行的 "RAG 掺入历史"方案，它更接近 Claude 原生的 Memory Compaction 行为，但完全在用户侧实现、不依赖特定模型。

这种工具的流行反映两个压力：一是前沿模型的上下文费用虽然每 token 便宜了，但 Agent 工作流里高频 1M-token 级别调用让总账单失控；二是开发者越来越希望"自己掌握上下文"而不是交给模型内部黑盒压缩。该项目的爆红也说明**上下文经济学正在成为 Agent 中间件市场的新战场**。

---

## 生态观察

今天的 GitHub Trending 可以用一句话概括：**"Agent Skills" 正在成为 2026 Q4 最标准化的开源原语。**

- **横向扩张**：Cloudflare（安全）、Anthropic（通用）、Google（产品）、Matt Pocock（工程）在同一天入榜，skill 的"竖直领域包"分布已经开始。
- **纵向深入**：Vercel 的 agent-browser、OpenMausBot 的 Bot VM、billion-context 的上下文压缩，说明 Agent 中间件层（浏览器、运行时、上下文管理）也在同步成熟。
- **传统工程不冷**：Zed（+1,119⭐）、Prometheus、Ruff、Tailwind 仍在榜上，说明核心开发工具的迭代热度没有被 AI 噱头掩盖。
- **去中心化反弹**：OpenMausBot 的开源替代、localthings 的"本地局域网控制家电"同期入榜，反映了社区对大厂云锁定的持续反击。

一个值得长期关注的信号是：skill-as-a-package 若真能标准化（像 Docker 镜像那样可以 pull / version / depend / compose），那么 2027 年的"Agent 应用市场"将会直接跳过今天的 ChatGPT Store / Claude App 生态，重构为一个更接近 npm 的开发者市场。
