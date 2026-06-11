# GitHub Trending 日报 · 2026-06-12

## 今日焦点

> **Agent Skills 生态全面占榜 · Apple 自研容器引擎 · 医疗 AI 开源破圈 · Agent 安全治理工具兴起**
>
> - `addyosmani/agent-skills` +3,275⭐ —— Addy Osmani 把"工程师级 agent 技能"系统化，今日 Skills 类项目第一
> - `apple/container` +2,419⭐ —— Apple 用 Swift + 轻量 VM 直接做 Linux 容器，绕过 Docker for Mac
> - `phuryn/pm-skills` +1,944⭐ —— PM 角色的 Skills Marketplace，证明非工程师也开始把工作流"agent 化"
> - `obra/superpowers` +1,323⭐ —— Jesse Vincent 的 Skills 框架累计星数突破 22 万，已经是事实标准
> - `NVIDIA/SkillSpector` +308⭐ —— NVIDIA 亲自下场扫描 agent skill 安全漏洞，标志着这条生态进入治理阶段

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 面向 AI 编码 Agent 的工业级工程技能集 | Shell | 54,586 | +3,275 | 5,933 |
| 2 | [apple/container](https://github.com/apple/container) | Mac 上用轻量 VM 跑 Linux 容器的官方工具 | Swift | 32,227 | +2,419 | 905 |
| 3 | [phuryn/pm-skills](https://github.com/phuryn/pm-skills) | PM Skills Marketplace，100+ agent 技能 / 命令 / 插件 | — | 16,158 | +1,944 | 1,682 |
| 4 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic Skills 框架与开发方法论 | Shell | 224,753 | +1,323 | 19,980 |
| 5 | [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | 一键部署"AI 代理机构"，多专家 Agent | Shell | 111,480 | +1,235 | 18,246 |
| 6 | [soxoj/maigret](https://github.com/soxoj/maigret) | 通过用户名在 3000+ 网站搜集人物档案 | Python | 32,573 | +665 | 2,386 |
| 7 | [refactoringhq/tolaria](https://github.com/refactoringhq/tolaria) | Markdown 知识库桌面管理器 | TypeScript | 15,365 | +604 | 1,059 |
| 8 | [masterking32/MasterDnsVPN](https://github.com/masterking32/MasterDnsVPN) | 基于 DNS 隧道的高级 VPN（含 ARQ 与负载均衡） | Go | 5,657 | +510 | 518 |
| 9 | [maziyarpanahi/openmed](https://github.com/maziyarpanahi/openmed) | 开源医疗 AI 工具集 | Python | 2,722 | +427 | 267 |
| 10 | [x1xhlol/system-prompts-and-models-of-ai-tools](https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools) | 主流 AI 工具系统 prompt 与模型清单 | — | 139,843 | +369 | 34,615 |
| 11 | [TapXWorld/ChinaTextbook](https://github.com/TapXWorld/ChinaTextbook) | 中国教材整理仓库 | Roff | 73,913 | +345 | 16,537 |
| 12 | [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) | AI agent skills 安全扫描器 | Python | 2,590 | +308 | 208 |
| 13 | [chatwoot/chatwoot](https://github.com/chatwoot/chatwoot) | 开源全渠道客服平台 | Ruby | 30,329 | +191 | 7,503 |
| 14 | [kenn-io/agentsview](https://github.com/kenn-io/agentsview) | 本地优先的 coding agent 会话分析 | Go | 1,600 | +98 | 172 |
| 15 | [restic/restic](https://github.com/restic/restic) | 快速安全的增量备份程序 | Go | 34,132 | +33 | 1,784 |

---

## 重点项目点评

### 🥇 [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — 今日榜首，+3,275⭐

**Google Chrome 团队的 Addy Osmani 把"工程师 SOP"翻成 Agent 可执行的 Skill 包**

Addy Osmani（Chrome DevTools / Web Performance 圈无人不晓的工程师）昨天放出了这个项目。仓库里把"如何写 RFC"、"如何做 code review"、"如何 incident postmortem"、"如何 perf-profile 一个 SPA"等 60+ 高级工程实践，封装成可被 Claude Code / Cursor / Copilot 直接挂载的 Skill 包。每个 Skill 都附带 Critic Prompt（"用户给我这个产出后我应当如何反过来挑刺"）。

它今天能拿到 +3,275⭐ 的核心原因有三：一是 Addy 自己的影响力（Web 圈"教科书写作者"地位）；二是 6 月初 Claude Code、Cursor 都把 "Skills" 升级为顶级抽象，开发者立即在找"工业级现成包"；三是 README 里给了 "import-into-Claude-Code" 一键脚本，模板化抄走的门槛极低。

这条赛道已经形成清晰梯队：obra/superpowers（22 万星，方法论顶层）→ msitarzewski/agency-agents（角色化机构层）→ addy 的 agent-skills（资深工程师 SOP 层）→ phuryn/pm-skills（PM 工作流层）。**Skills 不再是工程师玩具，它正在变成职业能力的可移植"运行时"**。

---

### 🥈 [apple/container](https://github.com/apple/container) — +2,419⭐

**Apple 自家用 Swift 写的 Mac 原生 Linux 容器工具，公开亮相即热榜第二**

apple/container 是 Apple 官方放出来的命令行工具：在 Apple Silicon Mac 上用 Hypervisor.framework 起轻量 VM，每个容器一台 microVM。和 Docker Desktop 走 QEMU/Linuxkit 不同，apple/container 用的是原生 Virtualization framework，启动时间 < 300ms，内存占用比 Docker Desktop 小一个数量级；并且**完全免 Docker Desktop 许可**，企业使用零费用。

这是 Apple 在 WWDC 周后释出的"工程师礼物"——也是它继续收紧 macOS 容器化生态的明确动作。之前 Asahi Linux 项目刚被 macOS 27 Beta 阻断启动（昨日 HN 第 7 名），今天 Apple 给出"我们自己的容器方案"。**两者放在一起的含义很清晰：Apple 不再容许第三方 Linux 进入裸机，但会给你一个官方虚拟化通道**。

短期受益最大的是 CI/CD 厂商（GitLab Runner、CircleCI macOS 套件），他们终于有了一条不依赖 Docker Desktop 商业 license 的合规路径；潜在压力对象是 Docker Inc. 自身——Docker Desktop 的 Mac 用户基本盘正在被官方工具直接挖走。

---

### 🥉 [phuryn/pm-skills](https://github.com/phuryn/pm-skills) — +1,944⭐

**第一个出圈的"PM 专用 Skills 市场"，把产品经理工作流也 Agent 化**

phuryn/pm-skills 是模仿 addy/agent-skills 的姊妹仓库：里面是 100+ 个 PM 工作场景的可挂载 Skill，例如 "User Interview Synthesis"、"OKR Drafting"、"Feature Spec → Eng Handoff"、"Competitive Battlecard Generation"。每个 Skill 同样附带 Critic Prompt 和示例输出，可直接挂到 Claude Code 或者 Notion 的 Agent 插件。

今日它和 agent-skills 并列在 Trending 前三，传递出非常明确的信号：**Skills 框架的扩张方向不是技术深度，而是职能广度**。前一个月 Skills 仓库还集中在 Web、DevOps、Security；今天 PM 这条线起来后，下一波合理预测会是 marketing-skills、sales-skills、legal-skills，对应美国大厂 6 月开始的"AI 替代中层管理"叙事。

值得对照的是 obra/superpowers 仓库已经突破 22 万星——这是开源生态历史上少见的"方法论 + 工具集"双高位项目，说明 Skills 不只是 GitHub 上的潮流，而是 2026 年下半年企业内培训的实际抓手。

---

### 🔥 [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) — +308⭐

**NVIDIA 第一次亲自下场做 Skill 安全审计，治理工具入场**

NVIDIA 的 Trust & Safety 团队上线了 SkillSpector：一个静态扫描器，专门检查 agent skill 包里的 prompt injection、shell-out 风险、过度权限、数据外泄路径。支持 Claude Skills 格式、OpenAI Custom GPT 格式、LangChain Tool 格式三大主流定义。

今天它能挤进 Trending 前 12，本身就是个信号：**Skills 生态已经大到 NVIDIA 觉得"必须有人管"**。前一周 Anthropic Mythos 1 限定到 50 家 Glasswing 合作方做"防御性安全研究"，今天 NVIDIA 把 skill 治理拉到开源层面——硬件厂商在 AI Agent 链路里的角色已经远远超过"卖 GPU"。

可以预见的下一步：6 月底 NVIDIA GTC Taipei 上 SkillSpector 会被并入 NeMo Guardrails / NIM 平台，成为企业部署 Skills 时的默认合规组件；Apache 2.0 license 意味着它也会出现在 EU AI Act 8/2 合规清单里的"推荐工具"位。

---

### 🩺 [maziyarpanahi/openmed](https://github.com/maziyarpanahi/openmed) — +427⭐

**开源医疗 AI 工具集，从研究爱好者圈跳到主流**

openmed 是把医疗影像分割、临床 NER、报告生成、用药推荐等 30+ 任务整合到统一 Python pipeline 的开源项目，今日新增 427⭐ 是过去 60 天平均日增的 8 倍。作者 Maziyar 之前以 HuggingFace 中文/波斯语模型出名，这次把 medical AI 做成"开箱即用"。

之所以突然爆发，一个直接催化是 Apple WWDC 2026 提到 HealthKit + Apple Intelligence 的私人医疗助手未来形态，开发者集体在找"端侧可跑的医疗 LLM";二是 EU AI Act 8/2 全面适用前，医疗器械软件（MDR Class IIa+）合规模型很缺开源样板，openmed 在 README 里直接列出每个模型的 CE 标识状态——这种"合规即文档"的写法非常稀缺。

medical AI 历来是开源最弱、合规最强的领域；openmed 这次上榜值得作为"垂直 + 合规导向"开源新模板。

---

## 生态观察

今天的 Trending 是一面镜子：

- **Skills 类项目占据前 5 名中的 4 席**（agent-skills / pm-skills / superpowers / agency-agents），日累计新增星数超过 7,700。这是过去 12 个月里"AI 工作流"语义最确定的一次共识——大家不再讨论"要不要 Agent"，而是讨论"我的 Skill 包是什么"。
- **基础设施侧**，Apple 用 container 项目正面进入开发者工具市场，意图是把 macOS 上的 Linux 工作负载收编到自家虚拟化栈。Docker Inc. 的 Mac 客群正在被官方工具挖走。
- **治理与垂直**侧，NVIDIA SkillSpector 和 openmed 同时出现，说明 Skills/Agent 生态已经从"野生发布"过渡到"安全 + 合规 + 行业"三轴并行。EU AI Act 8/2 deadline 在背后扮演了无形推手。

冷却的板块也很明显：纯 LLM 推理引擎（vLLM / llama.cpp 类）今天基本无新作品上榜；前端框架几乎缺席（Svelte / Solid 系都没出现）。**AI 工程的注意力已经从"模型层"全面下移到"工作流层"——这是 2026 下半年最重要的开源结构变化。**
