# GitHub Trending 日报 · 2026-11-11

## 今日焦点

> **Agent-ready 设计系统 · Skills 生态爆发 · Rust 工具链再现神作 · Home Assistant × MCP · OSINT 老将复燃**
>
> - `meta/astryx` 单日 +3,111⭐，一个"面向 agent 友好"的开源设计系统横空出世，一天登顶。
> - `anthropics/skills` + `addyosmani/agent-skills` + `mattpocock/skills` 三大"Skills"仓库同时登榜，社区正在围绕"**可组合提示库**"重构 AI 工程范式。
> - `vercel-labs/agent-browser` Rust 浏览器自动化 CLI +775⭐，agent 操作真实浏览器的"去 Selenium 化"浪潮继续。
> - `homeassistant-ai/ha-mcp` +792⭐，MCP 成为智能家居社区的新粘合剂，呼应 HN 上今日"智能家居脱网自治"的大讨论。
> - `sherlock-project/sherlock` +2,387⭐，经典 OSINT 工具重回热榜，背后是本周多起"数字身份泄露"事件。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [meta/astryx](https://github.com/meta/astryx) | 面向 agent 的开源设计系统 | TypeScript | 22,627 | +3,111⭐ | 1,808 |
| 2 | [sherlock-project/sherlock](https://github.com/sherlock-project/sherlock) | 社交账号 OSINT 工具 | Python | 108,871 | +2,387⭐ | 12,653 |
| 3 | [anthropics/skills](https://github.com/anthropics/skills) | Agent Skills 官方公共仓库 | Python | 192,245 | +1,676⭐ | 22,637 |
| 4 | [mattpocock/skills](https://github.com/mattpocock/skills) | 面向工程师的 Skills 集合 | Shell | 320,841 | +1,223⭐ | 26,904 |
| 5 | [homeassistant-ai/ha-mcp](https://github.com/homeassistant-ai/ha-mcp) | Home Assistant MCP 适配器 | Python | 6,593 | +792⭐ | 427 |
| 6 | [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) | Rust 版浏览器自动化 CLI | Rust | 49,152 | +775⭐ | 3,446 |
| 7 | [anthropics/claude-quickstarts](https://github.com/anthropics/claude-quickstarts) | Claude API 快速启动模板 | Python | 20,457 | +530⭐ | 3,468 |
| 8 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 生产级工程 skills | JavaScript | 115,100 | +465⭐ | 12,094 |
| 9 | [google-deepmind/mujoco](https://github.com/google-deepmind/mujoco) | 多关节接触物理仿真 | C++ | 17,319 | +453⭐ | 2,144 |
| 10 | [ranxianglei/billion-context](https://github.com/ranxianglei/billion-context) | 单会话上下文压缩插件 | TypeScript | 6,268 | +374⭐ | 527 |
| 11 | [tokio-rs/topcoat](https://github.com/tokio-rs/topcoat) | 集成式 Rust Web 应用框架 | Rust | 6,763 | +192⭐ | 297 |
| 12 | [we-promise/sure](https://github.com/we-promise/sure) | 开源个人财务应用 | Ruby | 11,867 | +184⭐ | 884 |

---

## 重点项目点评

### 🥇 [meta/astryx](https://github.com/meta/astryx) — 今日榜首，+3,111⭐

**"Agent-ready design system" 是一次关键词卡位**

Meta 开源一个面向 agent 的设计系统，一天内冲到热榜榜首。它的卖点不是组件库本身（TypeScript、Figma 同步、暗黑模式等都已是行业标配），而是一组**AI agent 可直接读取与生成**的元数据：组件语义、交互约束、可用变体、生成式修改白名单。换句话说，它是第一个把 "coding agent 想生成某个 UI，但组件规则必须被遵守" 当作一等公民来设计的系统。

社区的热情更多来自于时机：在 Anthropic Claude、OpenAI、Vercel v0 已经把 "LLM 生成前端" 卷到白热化的 2026 末，"设计系统 → agent 协议" 成了一个空位。Meta 放出这套东西，既是对标 shadcn/ui 的"社区事实标准"，也是一次产品层面的"让你把 agent 的生成结果交给我们托管"的入口战争。

**深层信号：** 大厂第一次把"agent 消费"写进自己 open source 的核心叙事——下一阶段的组件库竞争不再是组件丰富度，而是"**LLM 看得懂多少** / **LLM 犯错多难**"。

---

### 🥈 Skills 生态三雄齐发：[anthropics/skills](https://github.com/anthropics/skills) + [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) + [mattpocock/skills](https://github.com/mattpocock/skills)

**"Skill" 正在成为 agent 时代的新一代 npm 包**

同一天前 10 中出现三个 Skills 仓库，这个现象本身就很说明问题：

- `anthropics/skills` 是官方仓，现在 192K⭐，已经不单纯是 Claude Code 的配件，而是事实上的 **"agent skill 规范仓"**。
- `addyosmani/agent-skills`（Google Chrome 团队）聚焦生产级工程 skill——测试、重构、性能回归自动化。
- `mattpocock/skills`（著名 TypeScript 布道者）以最接地气的方式打包工程师日常知识。

三个仓库共同指向一个判断：**Prompt 工程时代结束，Skill 工程时代开始**。模型能力已经足够强，收益不再来自"更会写 prompt"，而来自"准备好可复用、可审查的技能包"。这对企业而言是一个新的 ROI 模型：Skills 既是版本控制友好的提示库，也是组织知识的物化形式。

**深层信号：** Skills 仓的集中爆发，意味着开源社区正在**把 agent 能力自身也开源化** —— 2026 年的 Rails 不会是一个 Web 框架，而是一组被 star 几十万次的 skills 合集。

---

### 🥉 [homeassistant-ai/ha-mcp](https://github.com/homeassistant-ai/ha-mcp) — +792⭐

**智能家居社区把 MCP 当成"脱离云端大厂"的护城河**

今日的 HN 第一名是「Smart home devices should work without the internet」，而 Home Assistant 社区在用一个具体的工程回应：把 MCP 接入 HA，让任何本地跑着的 LLM（甚至是 M 芯片上的 llama.cpp）都能作为智能家居的"调度中枢"。

意义在于：过去 Amazon/Google 掌控的"语音 → 设备"链条，现在被切成两段 —— 语音/意图层由本地 LLM 消化，设备控制由 HA 完成，云厂商被从关键路径上移除了。对隐私敏感的用户、以及因为厂商关停而失去原有生态的"硬件遗孤"，这是一个相当实用的解决方案。

**深层信号：** MCP 正在变成 **"反云绑定" 的工具**——它一开始的目标是统一企业工具接入，却在社区端被拿来做"把大厂从我家踢出去"的武器。这是一个很有趣的 adoption 错位。

---

### 🏅 [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) — +775⭐

**Rust CLI 版本的 Playwright-for-Agent**

Vercel 做了一个 Rust 写的、专门为 agent 设计的浏览器自动化 CLI。相比 Playwright，它更小、更快，核心优化点是**可复现的会话快照** + **低 overhead 的 trace**——这两项正好是 agent 操作真实网页时最痛的地方。

今天它上榜，和另一条潜在新闻形成呼应：Claude Code / OpenAI Operator / Google Project Mariner 等 computer-use agent 在过去一个月同时放出大更新，社区需要一个"干净、无浏览器 UI"的底层驱动层。Rust 的选型暗示了对**长时间运行 agent 服务**的性能/稳定性诉求。

**深层信号：** Playwright 从测试工具变成 agent 基础设施的那一刻可能已经过去了——以后 agent 用的是"agent-browser"，Playwright 回到它测试工具的本业。

---

### 🎖️ [sherlock-project/sherlock](https://github.com/sherlock-project/sherlock) — +2,387⭐

**OSINT 经典工具回潮**

一个存在多年的经典 OSINT 工具，忽然单日 +2,387⭐ 冲到榜单第二，几乎可以确定是由近期的"数字身份泄露/人肉事件"或某条热门教程推动。Sherlock 的原理简单直接：输入用户名，在上百个平台上同时查找，提醒你"你的用户名是否被反查"。

它今天重上热榜其实是一个很有价值的隐喻：**在 LLM 能一分钟写出一个新爬虫的 2026 年，经典 OSINT 工具仍然有不可替代的价值**——因为它已经做完了那件"困难但一次性"的工作：维护一份高质量的站点签名库。

---

## 生态观察

今天 GitHub trending 的主题极其清晰：**Agent 消费层的基础设施正在成型**。

- **设计系统、Skills 仓、Browser CLI、MCP 适配** 四个方向同时出现在前 10 —— 这是一个"地基在被灌混凝土"的信号。2027 年真正会被赚到的钱，大概率就在这一层。
- **大厂 vs 社区**：Meta 入场设计系统、Vercel 入场 agent-browser、Google 入场 agent-skills，但同时 Home Assistant 社区用 MCP 完成"反云端"的技术主权建设——两条叙事线并存，构成今年年底最健康的开源图景。
- **Rust 继续吃系统工具层**：agent-browser 和 topcoat 两个 Rust 项目同日上榜，并不意外，但强化了"长时间运行的 agent 服务 ≈ Rust 服务"的刻板印象。
- **怀旧项目微反弹**：sherlock、we-promise/sure、mujoco 这些"做了多年的老项目"也在今日分走一杯羹，说明社区在 AI 疲劳之后开始回归"稳定、扎实、会用十年"的工具偏好。

一句话总结：GitHub 的热榜正在从"下一个 AI 玩具"切换到"Agent 基础设施中标赛"。
