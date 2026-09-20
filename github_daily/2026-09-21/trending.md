# GitHub Trending 每日热榜 · 2026-09-21

## 今日焦点

> **Agent Skill 大爆发 · 安全审计工具进入 Skill 化时代 · 开源金融/股票平台异军突起 · GPU 编排层稳步爬升**
>
> - `affaan-m/ECC` — Claude Code Agent 性能优化系统，+837⭐ 冲上榜首
> - `cloudflare/security-audit-skill` — Cloudflare 官方发布"多阶段安全审计 Skill"，+2,375⭐ 全站单日最强
> - `addyosmani/agent-skills` — "生产级 AI Coding Agent 技能包"接近 10 万⭐，Agent Skill 生态迎来收敛期
> - `trycua/cua` — 开源市场行情平台冲上 25k⭐，一天 +1,012⭐
> - `higgsfield-ai/higgsfield` — 容错型高扩展 GPU 编排框架，+461⭐

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Claude Code 与相关工具的 Agent 性能优化 harness | JavaScript | 263,679 | +837 | 39,453 |
| 2 | [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) | 多阶段安全审计的 Coding Agent Skill | JavaScript | 17,953 | +2,375 | 994 |
| 3 | [trycua/cua](https://github.com/trycua/cua) | 开源市场行情/股价洞察平台 | HTML | 25,109 | +1,012 | 1,726 |
| 4 | [Open-Dev-Society/OpenStock](https://github.com/Open-Dev-Society/OpenStock) | 开源版付费股票平台替代品 | TypeScript | 16,745 | +752 | 2,131 |
| 5 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 面向 AI Coding Agent 的生产级技能包 | JavaScript | 97,644 | +729 | 10,292 |
| 6 | [higgsfield-ai/higgsfield](https://github.com/higgsfield-ai/higgsfield) | 大模型训练用容错型 GPU 编排框架 | Jupyter | 5,350 | +461 | 952 |
| 7 | [anthropics/claude-code](https://github.com/anthropics/claude-code) | 终端里的 Agent 编码工具 | TypeScript | 147,086 | +415 | 24,047 |
| 8 | [coder/coder](https://github.com/coder/coder) | 面向开发者与其 Agent 的安全开发环境 | Go | 16,019 | +382 | 1,541 |
| 9 | [vercel-labs/json-render](https://github.com/vercel-labs/json-render) | Generative UI 框架 | TypeScript | 17,262 | +332 | 915 |
| 10 | [anthropics/financial-services](https://github.com/anthropics/financial-services) | Anthropic 金融行业解决方案参考实现 | Python | 35,337 | +236 | 5,247 |
| 11 | [mihail911/modern-software-dev-assignments](https://github.com/mihail911/modern-software-dev-assignments) | Stanford 现代软件开发课作业集 | Python | 4,539 | +174 | 1,009 |
| 12 | [BuilderIO/agent-native](https://github.com/BuilderIO/agent-native) | 构建 Agent 原生应用的框架 | TypeScript | 5,167 | +89 | 484 |
| 13 | [paperless-ngx/paperless-ngx](https://github.com/paperless-ngx/paperless-ngx) | 社区强化版文档管理系统 | Python | 45,527 | +32 | 3,142 |

---

## 重点项目点评

### 🥇 [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) — +2,375⭐

**大厂正式下场做 Skill：安全审计从"工具"进化为"Agent 能力单元"**

Cloudflare 官方发布的 `security-audit-skill` 是一个专为 Claude Code / Coding Agent 使用的 **多阶段安全审计 Skill**，主打"分阶段扫描 + 验证过的发现（verified findings）"。它可以在 Agent 上下文里被显式调用，从代码变更差异触发，跑一条包括：静态分析 → 潜在漏洞验证 → 修复建议的完整流水线，并且把"疑似发现"和"已验证发现"严格分开——这个设计本身就是过去一年 AI 安全审查最痛的点（假阳性泛滥）。

这条榜首告诉行业两件事：其一，**"Skill" 这一封装形式已经出圈**——大型云厂商愿意把自家最贵的能力（安全审计）直接封成 Agent 能用的最小单元，而不是继续做闭源 SaaS；其二，**Agent 的能力扩展正在从"MCP Server"路线滑向"Skill"路线**：Skill 更轻、更本地、更容易嵌进 CI，是 2026 年下半年最明显的开发者工具趋势。

---

### 🥈 [affaan-m/ECC](https://github.com/affaan-m/ECC) — +837⭐

**Claude Code Agent Harness 的性能优化系统，直接杀入前排**

ECC 定位是 **Claude Code / 类似 Agent Tool 的性能优化 harness**——即在 Agent 运行时里插入指令编排、缓存与并发控制层，减少 token 与延迟消耗。总星 26 万说明它的仓库其实很早就有了积累，但今日 +837⭐ 的暴涨来自于 Anthropic Fable 5.1 上线（cache read 降至 1/4）的连锁反应：**只要模型侧改一次定价结构，harness 侧就会跟着重写策略**，这类"Agent 中间件"仓库因此进入新一轮优化窗口。

值得关注的是，ECC 与今日榜单上另两条相关（`anthropics/claude-code`、`addyosmani/agent-skills`）构成了同一条产业链：**Skill 提供能力单元 → Claude Code 提供 Agent 内核 → ECC 提供性能编排层**。这三条一起进榜，说明"Claude Code 生态"作为一个独立技术栈已经形成。

---

### 🥉 [trycua/cua](https://github.com/trycua/cua) — +1,012⭐

**开源版"实时行情 + 个性化提醒"平台，同类项目集体爬榜**

`trycua/cua` 与今日 4 位 `Open-Dev-Society/OpenStock`（+752⭐）几乎是同一天冲榜——两者都是 **开源版收费股票 / 市场行情平台的替代品**：实时价格、告警、公司洞察。这类项目连续爬榜，背后其实是同一件事：**Robinhood / Bloomberg Terminal / TradingView 的订阅费用已经让个人开发者集体反弹**，而 2026 年的 AI 编程工具让"从零复刻一个金融 SaaS"的成本骤降。

从榜单节奏看，"开源版付费 SaaS 替代品"是继"AI 工具"之后最稳定的 GitHub 爬榜品类，且这批项目普遍采用 TypeScript + Next.js + 免费或平价市场数据源。**下一个被开源解构的赛道，可能就是财报分析和量化研究**。

---

### 🚀 [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — +729⭐

**接近 10 万⭐的 Agent 技能包，Skill 生态开始收敛**

由 Google 的 Addy Osmani 维护，`agent-skills` 提供了一整套 **"生产级 AI Coding Agent 技能包"**——从测试生成、代码审查到重构，涵盖典型 Agent 工作流。这份仓库的关键作用不是提供最强的单一 Skill，而是把"什么样的 Skill 才算生产就绪"变成一个公开标准。

它今天再度爬榜，与 `cloudflare/security-audit-skill` 榜首形成呼应——**Skill 生态从"每个人做一个"进入"标准形成期"**：命名规范、目录结构、测试要求都在收敛，头部仓库的示范效应加速。未来 3 个月，Agent 工具的护城河很可能不是模型也不是 IDE，而是"谁的 Skill 库里长住着 Fortune 500 的开发者"。

---

### 🧠 [higgsfield-ai/higgsfield](https://github.com/higgsfield-ai/higgsfield) — +461⭐

**面向大模型训练的容错型 GPU 编排框架，"训练地基"再次热起来**

`higgsfield` 是一个 **容错型、高扩展性的 GPU 编排框架**——为超大规模训练提供 job scheduler + auto-recovery + 分布式 checkpoint 能力。这类"训练地基"的项目在 2025 年 SkyPilot、Ray 之后一度冷清，但 2026 年因为**开源模型持续发力（Qwen、DeepSeek、GLM）+ HBM 供给松动（今日 HN 前排 Samsung 产能翻倍）**，训练/微调侧的工具需求再度抬头。

尤其值得注意的是，它把"故障恢复"作为第一优先，说明目标客户是 **实际跑万卡训练** 的工业级团队——不是单机 finetune 玩家。这条项目上前排是一个信号：**大规模开源模型训练不再是几家实验室的特权，中层玩家（大学、AI 初创）正试图把训练能力自己抓回手里**。

---

## 生态观察

**今天的 GitHub 是"Claude Code 生态日"。** ECC (harness)、agent-skills (skill 标准)、claude-code (核心)、cloudflare/security-audit-skill (企业级 Skill) 四条同时进入 Top 10，第一次能明显感觉到 Anthropic 主导的 Agent 技术栈作为独立生态成型。对比之下，LangChain / LlamaIndex 系今日没有一条爬榜——**Agent 工具的心智份额正在快速重分**。

**开源 SaaS 替代品继续活跃。** `trycua/cua`、`OpenStock` 都是"开源版付费金融平台"，加上一直在榜的 `paperless-ngx`、`coder/coder`，"用开源杀 SaaS"是 2026 年下半年最稳的 GitHub 增长赛道之一。

**训练侧工具复苏。** `higgsfield-ai/higgsfield` 上榜配合 HBM 硬件产能翻倍的新闻，暗示 2027 年会有一波"中型玩家自训"高潮——训练不再只是 OpenAI、Anthropic、Google 三家的游戏。

**冷区：** 前端框架、传统数据库、DevOps 工具今天几乎全线缺席。榜单已经被"AI Agent 生态 + 开源 SaaS 替代品"两条线全面覆盖，Web 与基础设施品类的爬榜窗口进一步收窄。
