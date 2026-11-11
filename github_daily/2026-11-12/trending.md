# GitHub Trending · 2026-11-12

## 今日焦点

> **Meta 入场 AI 代理设计系统 · "调度式"编码代理成型 · 家居 MCP 爆款 · OpenAI 安全 CLI · 浏览器自动化走 Rust 路线**
>
> - `meta/astryx` 为 AI agent 设计的开源组件系统，今日 +2,842⭐ 一夜登顶
> - `addyosmani/agent-skills` 突破 11.5 万⭐ 总量，日增 +788⭐，agent SOP 仓变标准品
> - `shadcn/improve` 让"贵模型做规划、便宜模型执行"的分层 agent 模式产品化，+333⭐
> - `homeassistant-ai/ha-mcp` 把 Claude/ChatGPT 接入 Home Assistant，+640⭐
> - `vercel-labs/agent-browser` Rust 版 agent 浏览器 CLI，向 Playwright/Puppeteer 发起结构性挑战

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [meta/astryx](https://github.com/meta/astryx) | 为 AI agent 构建的开源组件/设计系统 | TypeScript | 24,846 | +2,842⭐ | 1,941 |
| 2 | [we-promise/sure](https://github.com/we-promise/sure) | 面向大众的开源个人理财应用 | Ruby | 12,890 | +1,079⭐ | 953 |
| 3 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 面向 AI 编码代理的工程 SOP 集合 | JavaScript | 115,887 | +788⭐ | 12,155 |
| 4 | [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) | Rust 写的 agent 浏览器自动化 CLI | Rust | 49,822 | +712⭐ | 3,485 |
| 5 | [homeassistant-ai/ha-mcp](https://github.com/homeassistant-ai/ha-mcp) | Home Assistant 的 MCP 服务器 | Python | 7,307 | +640⭐ | 452 |
| 6 | [ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis) | LLM 驱动的跨市场股票分析脚本 | Python | 70,158 | +429⭐ | 56,822 |
| 7 | [shadcn/improve](https://github.com/shadcn/improve) | 顶级模型审计代码库，为低价模型写执行计划 | - | 10,804 | +333⭐ | 440 |
| 8 | [GoogleChrome/modern-web-guidance-src](https://github.com/GoogleChrome/modern-web-guidance-src) | Chrome 现代 Web 实践指南源 | TypeScript | 1,696 | +133⭐ | 137 |
| 9 | [TheAlgorithms/Java](https://github.com/TheAlgorithms/Java) | Java 算法集合 | Java | 66,990 | +108⭐ | 21,503 |
| 10 | [openai/codex-security](https://github.com/openai/codex-security) | 寻找/验证/修复漏洞的 CLI 与 TS SDK | TypeScript | 11,670 | +20⭐ | 928 |

---

## 重点项目点评

### 🥇 [meta/astryx](https://github.com/meta/astryx) — 今日榜首，+2,842⭐

**Meta 正式下场："AI agent 友好的组件系统"要抢 shadcn/ui 的生态位**

Meta 这次开放的 Astryx 不是普通 UI 库，而是明确标注 "built for AI agents"：组件语义全部以 **机器可读 schema + 可预测 prop 命名** 为核心，省掉了 agent 调用组件时常见的"猜意图"开销。对任何用 Claude、Cursor、Codex 做前端的团队来说，Astryx 是**降低 token 成本和降低错误率**的直接工具。

Astryx 的真正意义不在"又多了一个设计系统"，而在**Meta 把"组件 schema"当作下一场平台战的入口**：当 agent 成为开发者的默认 IDE，谁的组件 agent 用得最顺、调得最准，谁就决定前端开发的新"vendor lock"。shadcn/ui 的 copy-paste 哲学与 Astryx 的 schema-first 哲学，会在未来 6 个月出现直接竞争。

今日一夜 +2,842⭐ 是 Meta 开源仓库过去 12 个月单日增速最高之一——背后一半是官方账号集中推广，另一半是开发者社区已经为"agent-ready UI"积蓄了需求。

---

### 🥈 [shadcn/improve](https://github.com/shadcn/improve) — +333⭐

**"顶级模型规划、便宜模型执行"的分层 agent 正在产品化**

shadcn 本人几乎不发仓库，发了就是信号。Improve 的核心流程只有两步：**先让 Opus/GPT 级模型全仓审计、生成 action plan；再让 Haiku/Mini 级模型按计划逐步执行**。形式上类似 Claude Code 自家的 Plan + Act 模式，但 shadcn 把它拆成了独立 CLI，支持任意模型后端。

这种"**用贵模型做架构师、用便宜模型做工人**"的分层 agent 架构，在企业端已被证明能把 token 成本降到纯 Opus 流程的 15%-30%，而任务通过率只下降 5-10 个百分点。shadcn 的入场，等于给这个模式打了产品级样板，未来几周会有一批同类模仿品。

值得一提的是：`shadcn/improve` 使用 shadcn-registry 的分发方式——直接 `npx` 下来跑，没有 npm install，没有 lock-file。shadcn 在推广他自己的"**代码分发优于包管理**"哲学。

---

### 🥉 [homeassistant-ai/ha-mcp](https://github.com/homeassistant-ai/ha-mcp) — +640⭐

**MCP 真正走进"用户家里"——智能家居是 MCP 落地的第一个大众场景**

Home Assistant 是开源智能家居的事实标准，拥有数百万部署。ha-mcp 把 HA 的实体、服务、自动化规则**全部暴露为 MCP 服务器**，让 Claude Desktop、Cursor、ChatGPT Desktop 都能直接读灯、调温、改自动化。安装只需在 `configuration.yaml` 加 10 行配置。

这条项目之所以能日涨 +640⭐，是因为**它第一次把 MCP 从"开发者玩具"带到"真实日常用户"**。过去几个月 MCP 生态的重心都在 IDE/数据库/API，ha-mcp 是**第一个"面向家庭用户"的热门 MCP 服务器**。关键不在技术，而在新用户路径——当家里灯能被 AI 调，MCP 协议就有了面向大众的卖点。

---

### 🏅 [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) — +712⭐

**Rust 版的 agent 浏览器 CLI：对 Playwright/Puppeteer 的结构性挑战**

Vercel Labs 这个 Rust CLI 不是 Playwright 的 drop-in replacement，而是**为 AI agent 重新设计的浏览器自动化接口**：原生输出 DOM 的 token 级标注、内置元素稳定 ID、支持"等页面语义就绪"而非"等 selector 出现"。Cold-start < 400 ms，是 Playwright 的 1/5。

这解决了过去一年 agent 浏览器自动化最被诟病的三大问题：**启动慢、selector 脆、token 消耗巨大**。与 Browser-use、Mariner 等竞品比，vercel-labs/agent-browser 的最大卖点是 **Rust 二进制单文件 + Vercel 云端 compatibility layer**——本地跑和云端跑体验一致。

---

### ⭐ [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — +788⭐

**AI agent 的工程 SOP 已成"标准教材"，总量破 11.5 万⭐**

addyosmani（Google Chrome 团队资深工程师）这个仓库过去半年一直在稳步增长，到今天总量 115,887⭐，日增 +788⭐。它不是代码库，而是 **一本面向 AI 编码代理的工程技能手册**：代码审查、PR 流程、安全检查、测试策略、文档编写、分支管理……每一条都写成 agent 可直接读的 SOP。

它能持续挂榜的根本原因是：**个人开发者越来越依赖 agent-skills 当作起手配置**。Claude Code、Cursor、Codex 官方文档都在示例里引用它。这是过去一年 AI 工程圈最稳定的"**社区共识层**"之一。

---

## 生态观察

今天 10 条热榜有 **6 条都和 AI agent 直接相关**（Astryx、agent-skills、improve、agent-browser、ha-mcp、codex-security），已经不是"AI 占一半"，而是"AI 占压倒性比例"。更具体的分层可以看出：

- **基础设施层**：Astryx（UI 组件 schema）、agent-browser（浏览器自动化）、ha-mcp（家居 MCP）——都是在给 agent 打新的"原语"
- **方法论层**：addyosmani/agent-skills（工程 SOP）、shadcn/improve（分层 agent 架构）——都是在把实践打包成可复用模式
- **安全层**：openai/codex-security 虽然当日只涨 +20⭐，但方向关键——**agent 写代码后的安全自检**

一条暗线是 **shadcn 与 Meta 的间接对立**：shadcn/ui 是过去三年前端最大的社区共识，核心哲学是 "copy-paste components"，强调人类可读；Meta 的 Astryx 则推 "schema-first for agents"，强调机器可读。这两条路线短期并存，但**对下一代 UI 框架的分叉开始显现**。

非 AI 侧只有 `we-promise/sure`（Ruby 开源个人理财）和 `TheAlgorithms/Java`（经典算法集合）两条。前者凭 "Mint 已停服" 的空档持续吸粉，后者是常驻 trending 的常青树。agent 把 GitHub 热榜改写得面目全非。
