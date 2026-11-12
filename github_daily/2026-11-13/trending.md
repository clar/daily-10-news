# GitHub Trending 日报 · 2026-11-13

## 今日焦点

> **AI agent 生态全面接管榜单 · "Agent Skills"范式成为开源新共识 · AI 原生设计系统首次登顶 · 本地 LLM 推理引擎百花齐放 · Codex 转向安全赛道**
>
> - `meta/astryx` 以 +1,789⭐ 登顶，AI 原生设计系统首次打败通用 agent 项目。
> - `we-promise/sure` +974⭐，个人理财 app Maybe Finance 开源分叉继续冲榜。
> - `addyosmani/agent-skills` +812⭐，Addy Osmani 力推的"skill 工程"范式 star 破 11 万。
> - `GoogleChrome/modern-web-guidance-src` +799⭐，Google 下场教 AI agent"怎么写现代 Web"。
> - `openai/codex-security` +663⭐，OpenAI Codex 产品线首次公开安全漏洞发现/修复 SDK。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [meta/astryx](https://github.com/meta/astryx) | 面向 AI agent 的开源设计系统 | TypeScript | 26,442 | +1,789 | 2,048 |
| 2 | [we-promise/sure](https://github.com/we-promise/sure) | 开源个人理财应用 | Ruby | 13,850 | +974 | 1,028 |
| 3 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 面向 AI coding agent 的工程 skill 集 | JavaScript | 116,627 | +812 | 12,205 |
| 4 | [GoogleChrome/modern-web-guidance-src](https://github.com/GoogleChrome/modern-web-guidance-src) | 教 coding agent 遵循现代 Web 实践 | TypeScript | 2,797 | +799 | 190 |
| 5 | [openai/codex-security](https://github.com/openai/codex-security) | 代码漏洞发现与修复 CLI / SDK | TypeScript | 12,362 | +663 | 975 |
| 6 | [Alishahryar1/free-claude-code](https://github.com/Alishahryar1/free-claude-code) | 免费使用 Claude Code 等编码 harness | Python | 69,230 | +461 | 10,751 |
| 7 | [pookjw/HermesEnabler](https://github.com/pookjw/HermesEnabler) | 在 Apple Watch 上启用爱马仕表盘 | Objective-C | 1,506 | +300 | 138 |
| 8 | [CopilotKit/OpenBot](https://github.com/CopilotKit/OpenBot) | 开源 AI 同事，自带浏览器/文件/工具 | TypeScript | 11,543 | +291 | 1,428 |
| 9 | [ggml-org/llama.cpp](https://github.com/ggml-org/llama.cpp) | C/C++ LLM 推理引擎 | C++ | 134,510 | +287 | 25,506 |
| 10 | [QwenLM/qwen-code](https://github.com/QwenLM/qwen-code) | 终端里的开源 AI 编码 agent | TypeScript | 29,767 | +151 | 3,392 |
| 11 | [nodejs/node](https://github.com/nodejs/node) | JavaScript 运行时 | JavaScript | 123,583 | +133 | 38,053 |
| 12 | [nvm-sh/nvm](https://github.com/nvm-sh/nvm) | Node.js 版本管理脚本 | Shell | 95,999 | +107 | 10,757 |
| 13 | [ashhart/TensorFold](https://github.com/ashhart/TensorFold) | Metal/CUDA/Vulkan 三端 LLM 推理引擎 | Zig | 1,919 | +94 | 391 |

---

## 重点项目点评

### 🥇 [meta/astryx](https://github.com/meta/astryx) — 今日榜首，+1,789⭐

**AI 原生设计系统正式进入主流开发者视野**

Meta 开源的 Astryx 一夜之间冲上榜首，它不只是一个组件库，而是"为 AI agent 生成 UI 而优化"的设计系统：所有组件都附带了结构化的 JSON schema、语义化标签以及受控状态机，使得 Claude、Codex、Gemini 等 agent 在生成前端代码时能直接产出"符合 design token"的 UI，而不是千奇百怪的 Tailwind 组合。

Astryx 的关键创新是 token-first 架构：颜色、间距、动效、无障碍属性都是一等公民，agent 可以在生成过程中显式指定 "medium density + high contrast + brand blue" 这种语义维度，而不是直接写死像素值。这从根本上解决了 AI 生成 UI 的两个顽疾：风格漂移（同一个产品里 agent 两次生成的卡片高度不一）、品牌污染（agent 把 Material Design 塞进你 brand guide 里的问题）。

对生态的意义：Shopify Polaris、GitHub Primer、Adobe Spectrum 之后，Astryx 可能代表 Meta 在企业设计系统这一仗上的正面入场。更重要的是，它正在定义"AI-friendly design system"这个新品类的标准接口——后续 Anthropic / Vercel 推出竞品时，schema 兼容性会是关键战场。

---

### 🥈 [we-promise/sure](https://github.com/we-promise/sure) — +974⭐

**个人理财应用的"维基式分叉"再度证明其生命力**

Sure 是 Maybe Finance 开源版本的社区分叉（原项目关停后由 we-promise 组织维护），提供自托管的个人净资产追踪、投资组合管理、账户聚合等功能。今日爆增 974⭐ 的背景是：昨天 HN 一篇"离开 Mint/Simplifi 自托管理财 90 天复盘"的热帖把 Sure 作为首选推荐。

Sure 的技术栈选择很值得玩味——Rails 8 + Hotwire + Postgres，几乎是"反时代"的；但在 agent 泛滥的 2026，"少依赖、少 JS、服务端渲染"反而让它在非技术用户里有极强的部署吸引力。它在 YouTube 上已经形成了一个"自托管理财教程"子文化，这类社区驱动的滚雪球效应是 star 增长真正的燃料。

本仓库的"社区分叉胜过原厂商"也是 2026 年开源生态的一个新信号：Anthropic Claude Skills、Hashicorp OpenTofu、Open Finance 等多个赛道都出现了"商业版关停→社区分叉繁荣"的循环。

---

### 🥉 [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — +812⭐

**"Skill 工程"范式进入 11 万⭐ 俱乐部**

Google Chrome 布道师 Addy Osmani 的 agent-skills 仓库今日破 11 万 star，这是 AI coding agent 周边生态里第一个达到此级别的"方法论"仓库（而非工具/库）。仓库内容是围绕 Claude Code / Codex / Cursor 等 coding harness 的 skill YAML 模板、hook 脚本、评估套件，以及"skill 怎么写"的大量教程。

Agent-skills 的爆红反映出一个关键趋势：开发者正在从"学会提示工程"转向"学会写 skill"——前者是一次性对话技巧，后者是可复用、可版本化、可团队共享的工程资产。Anthropic 的 Skills SDK、OpenAI 的 Managed Agents、Google 的 Antigravity Orchestrator 都在推动"skill 工程"成为一个独立于 prompting 的新岗位技能。

如果说 2024 是 "AI engineer" 元年，2025 是 "agent engineer" 元年，那么 2026 的下半场显然是 "skill engineer" 的元年——而 Addy 的仓库正是这个新职种的 canonical reference。

---

### 📘 [GoogleChrome/modern-web-guidance-src](https://github.com/GoogleChrome/modern-web-guidance-src) — +799⭐

**Google 下场定义"AI agent 应该怎么写现代 Web"**

Google Chrome 团队本周开源了 modern-web-guidance-src——一个专门给 AI coding agent 读的"现代 Web 最佳实践"知识库。内容包括 Interop 2026 的推荐特性、Core Web Vitals 2.0 的指标优化、CSS Container Queries 的使用模式、Web Components 和 SSR 的协同范式等等，所有章节都以 agent 友好的 markdown + 结构化 YAML frontmatter 组织。

这个仓库的"Chrome 官方"身份非常重要：过去 AI agent 写的前端代码经常依赖已经过时的 jQuery、CSS-in-JS、client-side 渲染范式——因为训练数据里充满了 2020-2022 的 Stack Overflow 答案。Google 这次是直接把"权威"文档塞进 agent 的 skill library，期望改变 Claude / Codex / Gemini 在 web 领域的生成偏好。

从战略上看，这是 Google 对抗"AI 生成代码质量下降"叙事的一次正面回应，也在争夺"谁来定义 AI 时代的 web 标准"——Chrome 团队明显不打算把这个话语权让给任何第三方 agent 厂商。

---

### 🔒 [openai/codex-security](https://github.com/openai/codex-security) — +663⭐

**OpenAI Codex 正式切入 AppSec 赛道**

Codex-security 是 OpenAI 本周低调发布的一个新品牌下产品——基于 Codex 模型的安全漏洞发现、验证与修复 CLI/SDK，内置 CVE 数据库对齐、OWASP Top 10 规则引擎和"可解释修复建议"。相比 Snyk、GitHub Advanced Security 等传统 AppSec 工具，它的最大差异是"生成式修复"——不仅告诉你哪里有 SQL injection，还能直接提交 PR 修掉并给出单元测试。

这个发布很值得玩味。过去 OpenAI 旗下的所有 Codex 相关项目都走"开发者生产力"品类，这是首次切入"安全"这个独立赛道。考虑到 Anthropic Claude Code 近期也加入了 security-review skill，前沿模型厂商正在迅速吃掉 AppSec 工具链的中段市场。

对企业的实际影响：Snyk、Veracode、Checkmarx 这些传统玩家的护城河不再只是"漏洞数据库完整性"，还要比"修复质量"和"假阳性率"。预计 2027 将出现第一波"安全扫描 + 自动修复 PR"产品整合潮，老牌 AppSec 公司要么被收购，要么快速 AI 化。

---

## 生态观察

**今日榜单 13 个仓库里，有 8 个与 AI agent 直接相关（agent 本体 4 个、agent 工具链 2 个、AI 生成友好资产 2 个）。** 2026 年 Q4 的 GitHub Trending 已经完全被 agent 生态接管，纯语言/框架/工具类项目只剩 nvm、node、llama.cpp 三个"背景常驻"。

**几个有价值的子趋势：**
- **"AI-friendly resource"** 成为独立品类：Chrome 的 modern-web-guidance、Meta 的 Astryx、Addy 的 agent-skills，都是"不供人读，供 agent 读"的新型开源项目。
- **本地推理引擎多语言化**：llama.cpp（C++）和 TensorFold（Zig）同列榜单，Zig 在系统级 AI runtime 的渗透率继续上升。
- **"商业版关停→社区分叉繁荣"** 模式再度奏效：Sure 复刻了 OpenTofu / Forgejo 式的社区接力叙事。
- **Codex 品牌延伸**：OpenAI 正在把 Codex 从单一 agent 拆成"Codex Code / Codex Security / Codex Review"等子产品线，与 Anthropic 的 Claude skill 形态形成对称竞争。

**冷门但值得盯紧的一条：** HermesEnabler 让 Apple Watch 启用爱马仕表盘，技术上是逆向工程案例，背后反映的是"反订阅/反软件锁"运动在消费电子领域继续扩散——这与 Show HN 上"$300 embroidery machine DIY app"是同一个精神源流。
