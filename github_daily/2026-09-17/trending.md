# GitHub Trending 每日榜单 · 2026-09-17

## 今日焦点

> **Coding Agent 生态大爆发 · 前沿 MoE 端侧化 · Cloudflare 安全 Skill · 阿里开源代码审查工具 · 研究型 Agent 崛起**
>
> - `alibaba/open-code-review` **一夜 +3,215⭐**，Go 写的高并发代码审查工具正式开源，直逼 Sourcegraph 老阵地。
> - `JustVugg/colibri` **+1,532⭐**，用纯 C、零依赖运行前沿 MoE 模型，端侧推理再度出圈。
> - `cloudflare/security-audit-skill` **+1,249⭐**，Cloudflare 官方 Coding Agent 安全审计 Skill 首发即热榜。
> - `affaan-m/ECC` **+1,046⭐**，Agent 性能优化基础层（skills / memory / security）在 Coding Agent 生态里成为"隐性刚需"。
> - `alphaXiv/OpenResearch` **+1,036⭐**，把 Coding Agent 变成 Research Agent 的开源框架首次进入主榜。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [alibaba/open-code-review](https://github.com/alibaba/open-code-review) | 阿里级并发的开源代码审查工具，混合架构 | Go | 31,657 | +3,215⭐ | 2,249 |
| 2 | [JustVugg/colibri](https://github.com/JustVugg/colibri) | 纯 C 零依赖运行前沿 MoE 模型 | C | 34,974 | +1,532⭐ | 3,671 |
| 3 | [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) | Coding Agent 多阶段安全审计 Skill | JavaScript | 7,021 | +1,249⭐ | 412 |
| 4 | [abue-ammar/tinycast](https://github.com/abue-ammar/tinycast) | 极轻量 macOS 快捷启动 + 剪贴板 | Swift | 5,548 | +1,136⭐ | 264 |
| 5 | [NationalSecurityAgency/ghidra](https://github.com/NationalSecurityAgency/ghidra) | NSA 开源软件逆向框架 | Java | 77,729 | +1,059⭐ | 8,593 |
| 6 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Coding Agent 的 skills/memory/security 底座 | JavaScript | 260,203 | +1,046⭐ | 38,946 |
| 7 | [alphaXiv/OpenResearch](https://github.com/alphaXiv/OpenResearch) | 把 Coding Agent 变 Research Agent | Rust | 4,360 | +1,036⭐ | 270 |
| 8 | [ever-co/ever-gauzy](https://github.com/ever-co/ever-gauzy) | 开源商业管理平台 (ERP/CRM/HRM/ATS) | TypeScript | 7,272 | +771⭐ | 1,085 |
| 9 | [Lakr233/vphone-cli](https://github.com/Lakr233/vphone-cli) | 虚拟手机命令行工具 | Swift | 13,315 | +444⭐ | 1,586 |
| 10 | [jamiepine/voicebox](https://github.com/jamiepine/voicebox) | 开源 AI 语音工作室（克隆 / 听写 / 创作）| TypeScript | 54,333 | +409⭐ | 6,785 |
| 11 | [roboflow/supervision](https://github.com/roboflow/supervision) | 通用可复用计算机视觉工具库 | Python | 50,572 | +292⭐ | 4,812 |
| 12 | [anthropics/claude-code](https://github.com/anthropics/claude-code) | Claude 终端 Agentic Coding CLI | TypeScript | 145,468 | +155⭐ | 23,473 |
| 13 | [supabase/supabase](https://github.com/supabase/supabase) | Postgres 开发平台 | TypeScript | 109,667 | +118⭐ | 14,030 |
| 14 | [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) | Claude 知识工作者插件仓库 | Python | 24,267 | +96⭐ | 2,921 |
| 15 | [ankitects/anki](https://github.com/ankitects/anki) | 智能间隔重复卡片程序 | Rust | 30,828 | +50⭐ | 3,208 |

---

## 重点项目点评

### 🥇 [alibaba/open-code-review](https://github.com/alibaba/open-code-review) — 今日榜首，+3,215⭐

**阿里内部代码审查系统正式开源，直接冲击 Sourcegraph / GitHub 代码智能阵地**

Go 语言实现，宣称"经过阿里级并发验证"，采用"混合架构"——静态规则 + AI 反馈 + 人工工作流可插拔。这类工具过去一年一直由 CodeRabbit、Cursor Review、Greptile 等闭源商业产品占据，阿里这次以完整企业级实践 + 开源许可切入，一夜之间收获 3200+ ⭐，速度是本季最快之一。

三点值得关注：
- **中国大厂开源节奏在明显加速**，尤其是"工程基础设施 + Agent 化"这类工具，天然适合中国团队"卷规模、卷成本"的路子；
- **代码审查赛道从此有了"参考实现"**，会加速商业产品从"专有服务" 卷向"更好的开发者体验 + 集成"；
- **Go 而非 Rust**——阿里选择了"稳定 + 团队人手足" 的技术栈，也说明这类工具的性能瓶颈其实不在语言层。

---

### 🥈 [JustVugg/colibri](https://github.com/JustVugg/colibri) — +1,532⭐

**"前沿 MoE 模型 + 纯 C + 零依赖"，llama.cpp 之后的新一波端侧推理竞赛**

colibri 主打"在你现有硬件上运行前沿 MoE 模型"——纯 C 实现，零依赖，专门针对 DeepSeek / Qwen MoE 系列做了推理优化。GitHub 上已经积累到 3.5 万 ⭐，今日 +1,532 说明社区对"新一代端侧推理引擎"的关注度依然巨大。

它和 llama.cpp / MLX / gguf 的区别在于**明确瞄准 MoE 路由的稀疏加速**——传统 dense 推理引擎在 MoE 上性能损失严重，这块过去半年一直是端侧推理的短板。作者选择完全 C 实现，几乎默认要在嵌入式和低功耗设备上跑，方向和 llama.cpp 略有分野。

---

### 🥉 [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) — +1,249⭐

**Cloudflare 官方 Coding Agent Skill 首发，Skill 生态开始形成"官方标准"**

Cloudflare 把内部使用的多阶段安全审计流程封装成一个 Coding Agent Skill：结构化 prompt + 独立验证阶段 + 结构化 finding 输出，开源出来。JavaScript 实现，直接可用于 Claude Code / Cursor Skills。1249 ⭐ 是 Cloudflare 品牌 + Skill 生态爆发的双重结果。

**这条更大的信号是：Skill 已经从 Anthropic 的实验特性变成大厂对外发布的"品牌资产"**。Cloudflare 出手，之后大概率有 Datadog、Snyk、Sentry 跟进——**Skill 会成为 SaaS 服务对 AI Agent 时代做"官方 API"的新形态**。

---

### 4️⃣ [affaan-m/ECC](https://github.com/affaan-m/ECC) — +1,046⭐

**26 万 ⭐ 的老仓库突然回暖：Coding Agent "基础层" 需求正在被单独抽出**

ECC 定位是"给 Coding Agent 提供 skills / memory / security 的性能优化系统"——本质上是把过去嵌入到具体 Agent 里的三个横切能力抽成独立层。26 万 ⭐ 的历史存量 + 今日 1046 ⭐ 的增量，说明它抓住了一个真实的架构痛点：**当所有人都在造 Agent，Agent 之间共享的记忆、技能和安全策略必须能独立于 Agent 存在**。

这与 alphaXiv/OpenResearch 是同类信号：**Coding Agent 的"骨架"（skills / memory / security / research）正在被单独商品化**，接下来 6 个月的关键战场是谁能做出这些"横向能力层"的事实标准。

---

### 5️⃣ [alphaXiv/OpenResearch](https://github.com/alphaXiv/OpenResearch) — +1,036⭐

**"把 Coding Agent 变成 Research Agent"——Agent 应用形态正在从代码扩散到研究**

Rust 实现，明确定位"给 Coding Agent 加上一层研究能力"——文献检索、跨源综合、假设生成、实验设计。这是 Agent 应用形态的一次重要横向拓展：**过去两年 Coding Agent 是主战场，2026 年下半年开始，Research Agent、Data Agent、Design Agent 逐步分化**。

值得关注的是它选了 Rust——性能敏感 + 组合式架构，说明作者预期这套东西未来会跑在生产环境里、被大量并行调用。

---

## 生态观察

**主题一：Coding Agent 生态从"应用层"走向"基础层"**。今日榜单里 open-code-review、security-audit-skill、ECC、OpenResearch 四个项目都不是"再造一个 Coding Agent"，而是"给现有 Coding Agent 加能力"。**Agent 之间共享的 skills / memory / security 正在被单独抽象成新的商品**。

**主题二：中国大厂开源节奏在加速**。阿里 open-code-review 一夜 3200+ ⭐，Xiaomi Mimo（HN 今日热榜）直播 post-training，Lakr233/vphone-cli 稳居榜单——中国开发者对高质量开源基础设施的输出速度明显上升。

**主题三：端侧推理进入 MoE 时代**。colibri 一夜 1500+ ⭐，说明社区对"在自己硬件上跑前沿 MoE"的需求仍然旺盛，llama.cpp 之外的分支开始出现。

**主题四：Skill 从 Anthropic 实验特性变成"官方 API 新形态"**。Cloudflare 首发企业级 Skill 上榜，可以预期一批 SaaS 公司会跟进——这将是 Anthropic Skill 生态最重要的一次外部认证。

**主题五：安全 / 逆向工程的常青流量**。NSA Ghidra 一夜 1059 ⭐、cloudflare 安全 Skill 1249 ⭐——AI 时代的攻防工具在 GitHub 上依然是稳定的高流量赛道。
