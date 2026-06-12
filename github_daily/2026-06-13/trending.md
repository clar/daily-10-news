# GitHub Trending 每日速读 · 2026-06-13

## 今日焦点

> **Agent Skills 生态全面接管 trending · Apple Container 1.0 正式发布 · 医疗 AI 本地化加速 · PM 工具进入 Agent 化 · 老牌 IPTV 持续长尾**
>
> - `addyosmani/agent-skills` 一日 +2,660⭐ 直接登顶，把"高级工程师工作流"封装给 AI Agent
> - `apple/container` 1.0 正式 release，Apple Silicon 上的轻量 VM 容器方案
> - `obra/superpowers` 持续吸星 +1,276⭐，Agent 方法论框架累计 22.5 万星
> - `maziyarpanahi/openmed` 本地化医疗 AI 新秀，HIPAA 合规 + iOS/MLX 加速
> - `phuryn/pm-skills` PM 也要 Agent 化，100+ skills 直接接入 Claude Code

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 给 AI 编码 Agent 的工程级 skills 包 | Shell | 56,706 | +2,660 | 6,111 |
| 2 | [apple/container](https://github.com/apple/container) | Mac 上跑 Linux 容器（轻量 VM） | Swift | 35,001 | +3,513 | 974 |
| 3 | [obra/superpowers](https://github.com/obra/superpowers) | Agent 方法论 + skills 框架 | Shell | 225,955 | +1,276 | 20,080 |
| 4 | [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | 完整 AI Agency，多领域专家 Agent | Shell | 112,348 | +1,040 | 18,334 |
| 5 | [phuryn/pm-skills](https://github.com/phuryn/pm-skills) | PM Skills 市场，100+ 产品管理工作流 | — | 16,937 | +823 | 1,736 |
| 6 | [maziyarpanahi/openmed](https://github.com/maziyarpanahi/openmed) | 本地化医疗 AI，HIPAA 合规 + MLX 加速 | Python | 3,173 | +517 | 303 |
| 7 | [masterking32/MasterDnsVPN](https://github.com/masterking32/MasterDnsVPN) | 高级 DNS 隧道翻墙 | Go | 5,985 | +401 | 538 |
| 8 | [mattermost/mattermost](https://github.com/mattermost/mattermost) | 开源团队协作平台 | TypeScript | 37,609 | +391 | 8,711 |
| 9 | [refactoringhq/tolaria](https://github.com/refactoringhq/tolaria) | Markdown 知识库桌面 App | TypeScript | 15,729 | +369 | 1,075 |
| 10 | [iptv-org/iptv](https://github.com/iptv-org/iptv) | 全球公开 IPTV 频道集合 | TypeScript | 118,003 | +142 | 6,300 |
| 11 | [microsoft/PowerToys](https://github.com/microsoft/PowerToys) | Windows 生产力工具集 | C | 134,313 | +104 | 8,063 |
| 12 | [LMCache/LMCache](https://github.com/LMCache/LMCache) | 最快的 LLM KV cache 层 | Python | 8,620 | +17 | 1,288 |
| 13 | [music-assistant/server](https://github.com/music-assistant/server) | 开源媒体库管理器 | Python | 1,759 | +6 | 422 |

---

## 重点项目点评

### 🥇 [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — 今日榜首，+2,660⭐

**Addy Osmani 亲自下场做 skills，宣告"Agent 工程化"进入 2.0 阶段**

Google Chrome team 资深工程师 Addy Osmani 把"高级工程师的判断力"——拆需求、写规范、TDD、code review、安全加固、CI/CD——拆成 24 个独立 skill，按 Define → Plan → Build → Verify → Review → Ship 六段组织，让 AI Agent 走完整个 SDLC 而不是只生成代码片段。整个仓库以 7 个 slash command（`/spec` `/plan` `/build` `/test` `/review` `/code-simplify` `/ship`）作为入口，兼容 Claude Code、Cursor、Gemini CLI、Windsurf。

这条仓库一天涨 2,660 星不是偶然。过去一周 Anthropic 给 Claude Code 上线 nested sub-agent、OpenAI 收购 Ona、obra/superpowers 持续累计 22 万星——Agent 不缺模型、不缺执行环境，缺的是**"该怎么做事"的工程方法论**。Addy 在 Twitter 的影响力 + Google Chrome team 的工程背景，让这一仓库一夜成为该领域的"事实标准候选"。

更值得关注的信号：这是一个**Shell + Markdown** 的仓库，没有 Python 也没有 SDK——skills 本质上是结构化的提示词与流程。这意味着 Agent skills 的核心壁垒是**方法论 + 经验沉淀**，不是代码——开源社区在这件事上的边际成本极低、复刻速度极快，未来几周大概率会有大量"针对 X 行业的 skills 包"涌现。

---

### 🥈 [apple/container](https://github.com/apple/container) — +3,513⭐

**Apple Container 1.0 正式发布，Mac 上的容器方案终于不再依赖 Docker Desktop**

WWDC 2026 周末，Apple 把 `container` 从预览版推进到 1.0 release——这是它登顶今日 trending 涨星数（+3,513）的直接原因。它的方案是为每个容器启动一个**轻量级虚拟机**（基于自研 Containerization Swift package），而不是像 Docker Desktop 那样跑一个总的 Linux VM。镜像兼容 OCI 标准，可以无缝复用既有 Docker 镜像，但执行模型完全不同。

为什么 macOS 开发者会蜂拥而至？Docker Desktop 自 2022 年收费以来，Mac 上的容器开发体验一直在退化——OrbStack 改善了不少但仍是商业产品。Apple Container 直接由 Apple 维护、随 macOS 升级、并且专为 Apple Silicon 优化（每个容器一个 VM 听起来重，但在 M 系列上启动速度 < 1 秒）。1.0 release 意味着 API 稳定、可以进生产 dev 环境。

战略层面，这是 Apple 对**"开发者从 Mac 流向 Linux"**的反击——Apple Silicon、Container、Xcode、Swift Build 现在构成了一个完整的"开发者主机"方案，无需任何 third-party VM 软件。这种"系统级开发者堆栈"的争夺，是 macOS vs Windows 11（WSL）真正的下一战。

---

### 🥉 [obra/superpowers](https://github.com/obra/superpowers) — +1,276⭐

**Agent 方法论框架累计 22.5 万星，"先思考再写代码"成为新规范**

`superpowers` 由前 Anthropic 工程师 obra 主导，是 Agent 方法论这条赛道上累计影响力最大的项目——总星 22.5 万、Fork 2 万。它和今日榜首 `agent-skills` 互为竞品：两者都把"高级工程师工作流"做成可复用 skill，但 superpowers 的差异化是**"先思考再写代码"** 的强制流程——Agent 接到任务后会先反问需求、再做设计、再 TDD（RED-GREEN-REFACTOR）、再用 subagent 执行、最后 review。

`superpowers` + `agent-skills` 同日双双登榜的现象，说明 Agent 工程化已经进入"方法论之争"阶段——这条赛道从去年的"我能不能写代码"，已经演变成"我能不能写**对**的代码"。社区里这两种风格大概率会共存：superpowers 更适合 0-1 探索性项目，agent-skills 更像企业级 SDLC 流水线。

值得开发者警惕的一点：当 Agent skills 高度同质化、命令几乎都叫 `/spec` `/build` `/test` `/review`，谁能赢取决于**真实使用反馈的迭代速度**——这就是 Addy Osmani 个人品牌 + Twitter 流量入场的真正威胁。obra 需要尽快证明 superpowers 在复杂任务上的 ROI 优势。

---

### 4️⃣ [maziyarpanahi/openmed](https://github.com/maziyarpanahi/openmed) — +517⭐

**本地化医疗 AI 新秀：HIPAA 合规 + Apple Silicon MLX 加速，瞄准院内部署**

OpenMed 把医疗 NER（疾病/药品/解剖结构识别）、HIPAA 18 种 PII 检测、12 种语言去标识化全部封装在一个 Python 框架里，提供 1,000+ 专门的生物医学模型，全部支持 CPU / CUDA / Apple Silicon (MLX) 本地运行，并提供 OpenMedKit 原生 iOS/macOS 集成。"Turn clinical text into structured insight with one line of code" 是它的卖点。

它今天能进 trending 涨 500+ 星，背后是医疗 AI 的一个新现实：**HIPAA / GDPR / 数据主权要求让"上传到 OpenAI"变得不可行**——医院、保险、药企必须找本地化方案。Apple Silicon 加上 MLX 让 M 系列 Mac mini 成为低成本本地推理节点，这正是 OpenMed 重点优化的方向。

把它和今天 HN 上"《Don't You Just Upload It to ChatGPT?》"的讨论放一起看很有意思——专业领域对 AI 的需求是"可控、可审计、本地化"，而不是"最强模型"。OpenMed 这类**针对监管行业的开源 vertical AI 框架**会成为 2026 H2 的明确赛道。

---

### 5️⃣ [phuryn/pm-skills](https://github.com/phuryn/pm-skills) — +823⭐

**PM Skills Marketplace：产品经理也要 Agent 化**

68 个产品管理 skill 分布在 9 个 plugin 里（discovery / strategy / execution / market research / analytics / GTM / marketing / utilities / AI shipping），加上 42 条 chained workflow，把 Teresa Torres、Marty Cagan、Alberto Savoia 这些经典 PM 框架塞进 Claude Code 的 slash command 里。`/discover` `/strategy` `/write-prd` 一行命令产出 PRD、OKR、竞品分析、launch 策略。

这是个非常有意思的信号：今日 trending 前 5 名里有 4 个是 skills 包（agent-skills / superpowers / agency-agents / pm-skills），说明 Agent 已经从"开发者工具"延伸到**"任何知识工作者的工作流"**。PM 通常被认为是"AI 难以替代的角色"——但 phuryn 的赌注是：PM 工作的 70% 是结构化的（市场调研、PRD、OKR、roadmap），完全可以靠 Agent + 框架库自动化。

战略观察：如果 skills 化能在 PM、UX、运营、HR 等专业角色上复刻，那 Claude Code / Cursor 这类原本面向"开发者"的 IDE，可能升级为**"专业角色操作系统"**——这是过去一年最有想象力但讨论最少的趋势。

---

## 生态观察

**今日 trending 几乎被一类东西占据：Agent Skills 包。** Top 5 里 4 个是 skills/methodology 仓库（agent-skills / superpowers / agency-agents / pm-skills），合计涨星 5,800+。Agent 已经从"模型可用"过渡到"工作流可复用"——下一战是**谁的 skills 包能成为事实标准**。这场战争的关键不是代码、不是模型，而是**"沉淀谁的工作经验"**：Addy Osmani 用 Google Chrome team 背书工程方法论，phuryn 用 Teresa Torres / Cagan 背书 PM 方法论——背书人本身就是核心 IP。

**Apple 用 container 1.0 把"开发者主机"叙事推进一个台阶。** 这是 macOS 自 Apple Silicon 以来最重要的开发者侧动作——配合 WWDC 上 Xcode 26、Swift Build、AFM 模型整合，Apple 正在拼一个"M 系列 Mac 即开发者全栈环境"的故事。Linux 党看到 container 1.0 应该警惕：未来 2 年 Mac 上做 cloud-native 开发可能不再需要 Docker、不再需要 minikube、甚至不再需要 Linux VM。

**Vertical AI 框架开始批量出现。** OpenMed 是医疗 NER 的本地化方案，配合本周 Anthropic Claude Code、Codex、Cursor 等都在做 vertical skills 包，说明开源社区已经把"通用大模型 + 垂直 skills 层"当成默认架构。下半年大概率会看到 OpenLegal、OpenFinance、OpenEdu 这类对应版本。

**冷却中：** 大型 LLM 推理框架今日表现平淡（LMCache 仅 +17，vLLM、SGLang 都未进前 15），社区注意力从"推理性能"转移到"Agent 工作流"——这是赛道成熟化的典型信号。
