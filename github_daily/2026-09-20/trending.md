# GitHub Trending 每日榜 · 2026-09-20

## 今日焦点

> **Agent Skills 成为新一代基础层 · Computer-Use 生态发力 · Cloudflare 双榜进场 · 本地化 Agent IDE 走热 · 文档管线仍是刚需**
>
> - `cloudflare/security-audit-skill` 单日暴涨 +3,162⭐，成为 Claude Code Skill 生态标杆案例。
> - `trycua/cua` 单日 +1,124⭐，Computer Use 2.0 跨系统操控栈成为 agent-workspace 首选。
> - `addyosmani/agent-skills` 累计 96k+⭐，Google Chrome DevRel 一手构建的 skills 大集合仍在增长。
> - `anthropics/claude-code` +482⭐（累计 146k+⭐），Claude Code 主线 CLI 持续扩张开发者基本盘。
> - `coder/coder` +406⭐，把「Dev Container 给 Agent 用」的定位讲通，主打云端安全沙箱。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) | 多阶段安全审计的 coding-agent Skill | JavaScript | 16,196 | +3,162⭐ | 888 |
| 2 | [trycua/cua](https://github.com/trycua/cua) | Computer Use 2.0：开源驱动 + 跨 OS 集群 | HTML | 24,344 | +1,124⭐ | 1,676 |
| 3 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | AI Agent 生产级工程 Skill 集合 | JavaScript | 96,982 | +547⭐ | 10,235 |
| 4 | [anthropics/claude-code](https://github.com/anthropics/claude-code) | 终端 agentic coding 工具 | TypeScript | 146,684 | +482⭐ | 23,914 |
| 5 | [Open-Dev-Society/OpenStock](https://github.com/Open-Dev-Society/OpenStock) | 开源实时行情 + 公司数据面板 | TypeScript | 15,993 | +477⭐ | 2,081 |
| 6 | [asciimoo/hister](https://github.com/asciimoo/hister) | 自建自己的搜索引擎 | Go | 5,211 | +430⭐ | 217 |
| 7 | [coder/coder](https://github.com/coder/coder) | 面向开发者与 Agent 的安全云开发环境 | Go | 15,597 | +406⭐ | 1,521 |
| 8 | [higgsfield-ai/higgsfield](https://github.com/higgsfield-ai/higgsfield) | 面向大模型训练的 GPU 编排框架 | Jupyter | 4,923 | +314⭐ | 908 |
| 9 | [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) | 知识工作者用 Claude Plugin 开源库 | Python | 25,110 | +280⭐ | 2,992 |
| 10 | [cactus-compute/needle](https://github.com/cactus-compute/needle) | 面向嵌入式设备的自动化基础模型 | Python | 11,581 | +207⭐ | 739 |
| 11 | [ruanyf/weekly](https://github.com/ruanyf/weekly) | 阮一峰科技爱好者周刊 | Markdown | 103,106 | +151⭐ | 4,424 |
| 12 | [docling-project/docling](https://github.com/docling-project/docling) | Gen AI 文档解析与结构化 | Python | 67,005 | +94⭐ | 4,833 |
| 13 | [cloudflare/quiche](https://github.com/cloudflare/quiche) | QUIC + HTTP/3 协议实现 | Rust | 12,003 | +84⭐ | 1,115 |
| 14 | [yynxxxxx/Codex-X](https://github.com/yynxxxxx/Codex-X) | OpenAI Codex 桌面 / CLI 可视化管理器 | Rust | 3,383 | +59⭐ | 443 |
| 15 | [ZuodaoTech/everyone-can-use-english](https://github.com/ZuodaoTech/everyone-can-use-english) | 「人人都能用英语」学习工具 | TypeScript | 37,767 | +31⭐ | 5,205 |

---

## 重点项目点评

### 🥇 [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) — 今日榜首，+3,162⭐

**Cloudflare 亲自下场教社区如何写「生产级 Claude Skill」**

Cloudflare 昨晚开源了他们内部使用的多阶段安全审计 Skill —— 一个 12k tokens 内完成的可复用工作流，包括依赖扫描、密钥泄漏检测、IAM 权限审查、web attack surface enumeration 与最终报告生成。它不是新工具，而是一个把 Cloudflare 内部 pentest playbook 装进 Claude Code Skill 的样板。

单日 +3,162⭐ 说明两件事：一是 Skill 生态正在从「玩具 demo」跨越到「大厂内部实战流程外发」阶段；二是 Cloudflare 明显在下 devrel 大棋——通过 Skill 把开发者拉进 Cloudflare 安全产品的心智地图。这种「把 SOP 打包成 Skill 开源」的模式，可能是接下来半年 GitHub trending 的常态。

---

### 🥈 [trycua/cua](https://github.com/trycua/cua) — +1,124⭐

**Computer Use 2.0：跨 OS 的 Agent 操作栈，24k+ 星只用了 4 个月**

trycua 提供开源的 Computer Use 驱动，可跑在 macOS、Windows、Linux 与 iOS 模拟器上，做到 Anthropic Computer Use / OpenAI Operator 类似的能力，但完全 self-host。今天他们发布了 2.0：新增 CUA-S1 系统一号模型（对应 HN 上今天的 Show HN 帖），把 GUI 操作决策模型抽象成独立组件，其他 LLM 只需要提供高层规划。

热度背后是行业分层的信号：过去半年 Agent 圈都在讨论「先在浏览器里做 Agent 还是先在电脑里做 Agent」，Anthropic Computer Use API 定价高、模型延迟大，trycua 的开源栈给了大量中型公司自建能力的可能。1,676 fork 的比例说明这是一个真正被拿去改造的项目，而不是收藏党热榜。

---

### 🥉 [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — +547⭐

**Google Chrome DevRel 团长 Addy Osmani 把 Skill 生态变成个人平台**

Addy Osmani 的这个 repo 从 8 月开始快速累积到 96k+ 星，涵盖数百个「production-grade」Skill 模板：代码 review、测试生成、文档同步、CI 修复、e2e 补写等。今天再涨 +547⭐，说明流量还没到顶。

它成功的原因是双向的：对开发者来说，能拿来就用的 Skill 比自己去啃 SDK 更省事；对 Anthropic 来说，社区正在自发把 Claude Code Skill 变成事实上的 agent shortcut 层——就像 Chrome DevTools 之于 Chrome。Google DevRel 老兵下场做 Anthropic 生态最大的社区仓库，这个 optics 本身就够耐人寻味。

---

### 🎯 [coder/coder](https://github.com/coder/coder) — +406⭐

**「Dev Container for Agents」讲通了：安全沙箱是 Agent 生产化的最后 1km**

Coder 把定位从「面向 developer 的云 IDE」正式升级为「面向 developer + agent 的安全环境」，主打让 Claude / Codex / Cursor 在受控 workspace 里跑长时间任务，避免污染本地。新加的 agent policy engine 支持从 IAM、网络白名单、文件权限三个维度 sandboxing。

行业上下文：SLA 高的企业越来越不敢让 Agent 直接跑在开发者笔电上，"AI agent 需要一个 dedicated 沙箱" 已经是共识。Coder + Daytona + GitPod + Coderabbit 这条赛道正在被重估，今天 +406⭐ 只是开胃菜。

---

### 🔥 [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) — +280⭐

**Anthropic 官方释出「知识工作插件」库，直指非编码场景**

这是 Anthropic 官方今日新推的 repo，包含面向律师、分析师、研究员、市场人的 Claude plugin 模板。技术上是 Skill + MCP + Artifact 的组合样板，产品上则是 Anthropic 首次把 Claude Code 之外的 knowledge-work 场景系统化开源。

对读者的意义：Anthropic 正在把「Claude Code」的成功外推到白领全域。如果你在写 Skill / Plugin，这个 repo 是 2026 Q4 最重要的模板源。280⭐ 的日增放在其他 repo 平淡，但考虑到它今天才 published，量级已经非常可观。

---

## 生态观察

**Agent Skill 生态正在完成从「玩具」到「基础层」的跃迁。** 榜前 5 里有 4 个直接与 Skill / Plugin 有关，Cloudflare、Addy Osmani、Anthropic 官方三方同日推动，说明这套抽象已经从 Anthropic 单方倡议变成社区共识。

**Computer Use 与 Cloud Dev Env 是 Agent 的两只手。** trycua/cua 和 coder/coder 分别代表「Agent 用户端」与「Agent 沙箱端」的双方向落地，两者共振暗示 Q4 大量 SaaS 都会自建 workspace + computer use 组合。

**Cloudflare 与 Anthropic 分别在做「生态操作系统」。** Cloudflare 通过 Workers + AI + Skill 建自己的开发者操作系统；Anthropic 通过 Claude Code + Skill + Plugin 建 agent 生态操作系统。两者今天各占榜单 2 席，是 2026 下半年最值得盯的两个平台叙事。

**中文与老 IP 项目仍在积累底盘。** 阮一峰周刊、everyone-can-use-english 这类经典中文 repo 继续吃自然流量，佐证内容型 repo 的长尾从不失效。
