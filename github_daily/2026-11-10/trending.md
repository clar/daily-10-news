# GitHub Trending 每日报告 · 2026-11-10

## 今日焦点

> **Agent Skills 井喷 · Meta 开源设计系统 · Sherlock 回潮 · 物理仿真/感知仍热 · LLM Agent 工具链持续放量**
>
> - `anthropics/skills` 190,865⭐，+1,052⭐，Agent Skills 已成为生态第一入口。
> - `meta/astryx` 19,823⭐，+3,324⭐，Meta 发布的 AI Agent 导向开源设计系统一夜起飞。
> - `sherlock-project/sherlock` +4,294⭐ 位居日增第一，老牌 OSINT 工具突然翻红。
> - `vercel-labs/agent-browser` +914⭐，Rust 写的 Agent 浏览器自动化 CLI。
> - `milind-soni/OpenMausBot` +1,589⭐，开源 Grok Bot 替代品带 VM 沙箱。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [anthropics/skills](https://github.com/anthropics/skills) | Claude Agent Skills 公开目录 | Python | 190,865 | +1,052 | 22,435 |
| 2 | [meta/astryx](https://github.com/meta/astryx) | Agent 原生、可定制的开源设计系统 | TypeScript | 19,823 | +3,324 | 1,507 |
| 3 | [sherlock-project/sherlock](https://github.com/sherlock-project/sherlock) | 按用户名跨平台定位社交账号 | Python | 106,897 | +4,294 | 12,374 |
| 4 | [google-deepmind/mujoco](https://github.com/google-deepmind/mujoco) | 多关节接触动力学物理仿真 | C++ | 16,876 | +579 | 1,990 |
| 5 | [anthropics/claude-quickstarts](https://github.com/anthropics/claude-quickstarts) | Claude API 可部署项目模板 | Python | 19,983 | +560 | 3,308 |
| 6 | [garrytan/gbrain](https://github.com/garrytan/gbrain) | OpenClaw/Hermes Agent 用的 Opinionated 大脑层 | TypeScript | 32,100 | +215 | 4,760 |
| 7 | [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) | 面向 AI Agent 的 CLI 浏览器自动化 | Rust | 48,412 | +914 | 3,299 |
| 8 | [ruvnet/RuView](https://github.com/ruvnet/RuView) | 用普通 WiFi 做空间感知 / 生命体征 | Rust | 103,401 | +245 | 13,399 |
| 9 | [ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis) | LLM 驱动的美/A/港股日报系统 | Python | 68,786 | +505 | 56,375 |
| 10 | [homeassistant-ai/ha-mcp](https://github.com/homeassistant-ai/ha-mcp) | 用 Claude/ChatGPT 配置 Home Assistant | Python | 5,906 | +31 | 292 |
| 11 | [milind-soni/OpenMausBot](https://github.com/milind-soni/OpenMausBot) | 开源 Grok Bot 替代 + 沙箱 VM | TypeScript | 19,600 | +1,589 | 2,685 |

---

## 重点项目点评

### 🥇 [sherlock-project/sherlock](https://github.com/sherlock-project/sherlock) — +4,294⭐

**老牌 OSINT 工具在 Agent 时代第二次翻红**

Sherlock 的上一次登顶还是 2020 年前后——按用户名在数百个社交平台上做横向检索，老牌到几乎成了 OSINT 101 的默认教材。它今天突然冲到日增第一，一方面是因为过去一周多起社工 / 诈骗报道让这类工具重新被技术圈分享，另一方面——也是更结构性的原因——Agent 框架正在把它封装成「人物信息采集」的子工具，Sherlock 这类「外部命令化」的 CLI 成为 Claude Skills / Agent Browser 的天然组件。

值得关注的是 Fork 数：106,897 星对 12,374 Fork，这个 Fork/Star 比例在传统工具里极高，意味着有大量「加个平台」或「做个 Agent wrapper」的下游分叉——这是 Agent 生态真实在消费它的信号。

---

### 🥈 [meta/astryx](https://github.com/meta/astryx) — +3,324⭐

**Meta 的「给 Agent 用的设计系统」是今天最被低估的一枪**

Astryx 把过去 10 年前端界习惯的「设计系统给人类设计师用」彻底换了方向，直接给出一套对 AI Agent 友好的组件、token、交互元数据——组件名称、props、可编辑区都以结构化方式暴露，Agent 可以直接 plan 一个 UI 而不需要先 parse 一个 Figma 文件。TypeScript 19,823⭐ / +3,324⭐ 的节奏表明一夜之间被整个前端社区灌了关注度。

这件事的真正意义是：Meta 在 Reality Labs + Agent 这条线一直缺一个「可解释、可组合的 UI 层」，Astryx 可能是 Meta 为了 Llama Agent / Horizon / Ray-Ban Meta 铺设的共同底座。开源发布的时机（紧跟 Muse Ember 端侧模型）也暗示 Meta 正在把 Agent 栈的每一层都公之于众。

---

### 🥉 [anthropics/skills](https://github.com/anthropics/skills) — +1,052⭐

**Agent Skills 已经成为生态门面**

anthropics/skills 几乎每周都在 trending 榜上，但这次 190,865 星的体量本身就是现象——它是 2026 年最被 fork 的开源项目之一（22,435 forks），也是 Claude Code / Claude App / Claude 云端会话共享的「软件基础设施」。生态走到这里，Skill 已经不是 Claude 的专属概念，它逐渐变成了类似 `.editorconfig` 或 `package.json` 这种跨工具的轻协议。

与之配套，`anthropics/claude-quickstarts`（+560⭐）、`homeassistant-ai/ha-mcp`（+31⭐）、`garrytan/gbrain`（+215⭐）同列今日榜，整个列表的 2/3 都与 Agent 生态直接相关。可以合理推论：11 月中旬 Anthropic IPO 效应下，这类官方/社区仓库会继续获得结构性关注。

---

### 🏅 No.4 · [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) — +914⭐

**Vercel 把浏览器做成 Agent 的"stdlib"**

Rust 写的 CLI 工具，核心定位是「让 Agent 像调 bash 一样调浏览器」：命令式 API、确定性 I/O、可组合管道。Vercel-labs 出品直接拉高背书，同时它的 Rust 选择与 Playwright / Puppeteer 的传统 Node 栈拉开差异化，速度更快、二进制单文件可分发。

这与 Claude 的 claude-in-chrome、OpenAI 的 Operator、Google Antigravity 2.0 在产品思路上完全同一方向：都承认 2026 年的 Agent 大多数时间都要「开浏览器」。agent-browser 是开源侧的代表作，48K+ 星意味着它在 7 月发布后 4 个月内已经是这个赛道的实质标准。

---

### 🏅 No.5 · [milind-soni/OpenMausBot](https://github.com/milind-soni/OpenMausBot) — +1,589⭐

**开源 Grok Bot 替代：带 VM 沙箱是真正的差异化**

OpenMausBot 不是又一个「套 Grok API 的壳」，而是提供一个虚拟机环境让机器人在隔离沙箱内跑代码、浏览、调用工具——这与 xAI Grok Bot 的「原生带 VM」思路如出一辙，但代码完全开源。19,600⭐ / +1,589⭐ 的节奏表明这类 Agent + VM 工具正迅速在社区形成共识。

对自托管用户来说，它意味着可以把 Grok 的交互体验独立出来绑到自己的 LLM 后端；对企业来说，更重要的是 VM 隔离比纯 Tool-Use 更安全。预计未来数周 GitHub 上会涌出多款类似「OpenX + 沙箱」项目。

---

## 生态观察

把今天 11 个仓库的话题压一压，基本上就三件事：

1. **Agent 基础设施的层叠正在完整化**。Skills（能力定义）、Astryx（UI 层）、Agent Browser（浏览器 I/O）、gbrain（规划层）、OpenMausBot（VM 沙箱）——分别对应 Agent 栈里最常被提及的 5 个空缺。整条栈在同一天各出一家旗舰项目，这是生态正在收敛的信号。

2. **「老工具的 Agent 化」是一个被低估的分支**。Sherlock、MuJoCo、Home Assistant、ha-mcp 这些原本在各自领域成熟多年的项目，因为「可被 Agent 调用」而再次冲榜——这种「存量项目×Agent」的乘数效应比纯新项目更有生命力。

3. **Rust / TypeScript 继续平分 Agent 客户端生态**。11 个项目里 Rust 3 个、TypeScript 4 个、Python 4 个，Python 退守到「后端 + Skills + 数据」三栖，CLI 与前端层基本被 Rust/TS 接管。

一句话：今天的 trending 榜是一张「2026 年 Agent 技术栈全家福」。
