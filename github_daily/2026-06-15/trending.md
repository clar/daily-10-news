# GitHub Trending Daily · 2026-06-15

## 今日焦点

> **Agent 安全工具崛起 · 金融基础模型开源 · IPTV 集合长青 · 老牌前端基础设施回潮 · LLM 多供应商抽象层**
>
> - `NVIDIA/SkillSpector` 上线即冲榜（+962⭐）：英伟达开源专扫 AI Agent 技能包安全漏洞的扫描器，16 类、64 种模式。
> - `shiyu-coder/Kronos` 大涨（+238⭐）：声称是"K 线数据上第一个开源 foundation model"，金融时序的 Transformer 路线被点亮。
> - `iptv-org/iptv` 仍是榜首（+1,531⭐）：刚性需求 + 高 churn，常年霸榜不下。
> - `swc-project/swc` 单日 +163⭐：Rust 前端工具链在 React 19/20 周期里被重新评估。
> - `andrewyng/aisuite` +290⭐：吴恩达的多 LLM 统一接口持续吸星，对应"多模型路由"已成行业事实。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [iptv-org/iptv](https://github.com/iptv-org/iptv) | 全球公开 IPTV 频道聚合 | TypeScript | 120,775 | +1,531⭐ | 6,463 |
| 2 | [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) | AI Agent 技能包安全扫描器 | Python | 5,219 | +962⭐ | 398 |
| 3 | [chatwoot/chatwoot](https://github.com/chatwoot/chatwoot) | 开源全渠道客服 / 替代 Intercom | Ruby | 31,185 | +399⭐ | 7,582 |
| 4 | [GorvGoyl/Clone-Wars](https://github.com/GorvGoyl/Clone-Wars) | 100+ 知名网站开源克隆汇总 | Multiple | 35,402 | +337⭐ | 3,182 |
| 5 | [andrewyng/aisuite](https://github.com/andrewyng/aisuite) | 多 LLM 厂商统一接口 | Python | 14,372 | +290⭐ | 1,501 |
| 6 | [Introduction-to-Autonomous-Robots/Introduction-to-Autonomous-Robots](https://github.com/Introduction-to-Autonomous-Robots/Introduction-to-Autonomous-Robots) | 自动机器人入门教科书 | TeX | 2,685 | +276⭐ | 610 |
| 7 | [freeCodeCamp/freeCodeCamp](https://github.com/freeCodeCamp/freeCodeCamp) | 编程教育大全 | TypeScript | 447,141 | +253⭐ | 44,948 |
| 8 | [shiyu-coder/Kronos](https://github.com/shiyu-coder/Kronos) | K 线金融时序 foundation model | Python | 29,884 | +238⭐ | 5,149 |
| 9 | [music-assistant/server](https://github.com/music-assistant/server) | 开源音乐流媒体聚合 | Python | 2,166 | +196⭐ | 437 |
| 10 | [swc-project/swc](https://github.com/swc-project/swc) | Rust 前端编译工具链 | Rust | 33,766 | +163⭐ | 1,401 |
| 11 | [cypress-io/cypress](https://github.com/cypress-io/cypress) | 浏览器端到端测试 | TypeScript | 49,914 | +121⭐ | 3,413 |
| 12 | [puppeteer/puppeteer](https://github.com/puppeteer/puppeteer) | Chrome/Firefox JS 自动化 API | TypeScript | 94,631 | +59⭐ | 9,438 |
| 13 | [Free-TV/IPTV](https://github.com/Free-TV/IPTV) | 免费 TV 频道 M3U 列表 | Python | 16,904 | +52⭐ | 2,543 |
| 14 | [meshery/meshery](https://github.com/meshery/meshery) | 云原生网格管理 | TypeScript | 10,386 | +45⭐ | 3,420 |
| 15 | [pytest-dev/pytest](https://github.com/pytest-dev/pytest) | Python 测试框架 | Python | 14,017 | +8⭐ | 3,177 |

---

## 重点项目点评

### 🥇 [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) — +962⭐

**Agent 安全扫描器："skills as code"的第一层防护**

英伟达开源的 SkillSpector 不是又一款 prompt-injection 玩具，而是把扫描对象明确定位在 **Claude Code / Gemini CLI 等 Agent 平台上以技能（skill / plugin）形式分发的代码包**。它内置 16 类、64 个安全模式，覆盖 prompt injection、数据外泄、特权升级、供应链投毒、过度自主、System Prompt 泄漏、危险代码执行等典型路径，提供静态分析 + 可选 LLM 语义评估两条路。

这条仓库今天突然爆量，本质是回应一个浮上水面的痛点：**Agent 技能包正在变成"新一代浏览器扩展"——分发渠道很多，安全审核几乎没有**。在我刚刚看到的 AI 日报（Anthropic Fable 5 / Mythos 5 被美政府强制下线）背景下，英伟达把"Agent 平台安全"作为基础设施开源出来，对企业落地 Agent 来说是一根真正的钉子。

预测后续几周内会看到 SkillSpector 被各家 Agent 市场（Anthropic Skills、Cursor、Cline 等）以 CI 形式集成；同时它的 64 个模式定义会变成行业事实标准。

---

### 🥈 [shiyu-coder/Kronos](https://github.com/shiyu-coder/Kronos) — +238⭐

**第一只"K 线 Foundation Model"：金融时序版的 GPT**

Kronos 把 OHLCV 蜡烛序列当作专门的"语言"来学，使用两阶段架构：先训一个针对 K 线的 tokenizer，再训一个自回归 Transformer。训练数据来自 **45 家全球交易所**，规模和广度都是同类开源项目里头一次。

这件事的意义不在"它能不能赚钱"——量化圈普遍知道单看价量预测 alpha 边际有限——而在于 **它把"金融时序 + 大模型"这条路彻底搬到了公开领域**。过去顶级买方拿来当成秘密武器的方法（K 线分词、统一基础模型、再下游微调），现在在 GitHub 上可以一键复现。下一波"垂直行业 foundation model" 的复刻潮（医疗、电网、物流）大概会借这套思路。

风险也清晰：金融时序非平稳、有自我反身性，纯监督预训练能给出的信号上限不会高；真正能用的版本可能是在 Kronos 上加 RLHF / 强化学习 + 多模态新闻 + 期权流。但开源 SOTA 起点已经显著抬高。

---

### 🥉 [iptv-org/iptv](https://github.com/iptv-org/iptv) — +1,531⭐

**常青树为什么还在涨：IPTV 的"刚性 + 高 churn"**

`iptv-org/iptv` 已经在 GitHub trending 上长期霸榜，今天再增 1531⭐，总星数突破 12 万。它本身只是一个 m3u 列表的聚合 + 校验工具集合——没有花哨架构、没有 AI 元素，靠的是 **频道列表每天都失效，需要持续维护和重新发现** 这一刚性需求。

它今天上榜的隐藏理由是：**主流流媒体服务（Netflix、Disney+、HBO）这一年内连续涨价 + 区域内容割裂越严重，普通用户和家庭 NAS 玩家越倾向回到"自建 IPTV 客户端 + 公开频道"的链路**。仓库的 fork 数（6,463）也说明大量私人/区域分支在持续维护各自的频道源。这类项目反映的是 **"开源对消费级娱乐基础设施的兜底作用"**，和 AI 无关，但稳定性极强。

---

### 4️⃣ [andrewyng/aisuite](https://github.com/andrewyng/aisuite) — +290⭐

**多 LLM 统一接口：Andrew Ng 的"通用 API"赌注还在赢**

aisuite 给开发者提供一个统一接口去调用 OpenAI、Anthropic、Google、Mistral、Groq、Together 等十几家供应商，写一次代码、切一行参数就能换模型。今天再涨 290⭐，累计已破 1.4 万。在我刚刚整理的 AI 日报里，**Anthropic Fable 5/Mythos 5 被美政府强制下线**——这条新闻直接把"多供应商路由"从优化项变成生存项：单一供应商的合规、配额、突然下线都可能让产品瞬间瘫痪。

aisuite 的吸星速度从某种程度上是 LangChain / LiteLLM 等老牌路由器的"反例"——开发者要的不是另一套 framework，而是**简洁、稳定、低魔法的 multi-provider adapter**。Andrew Ng 的品牌效应让它天然有传播红利，但能持续涨星说明它确实戳到痛点。

后续看点：**aisuite 是否会被 OpenAI 5.6 / Claude Mythos / Gemini 3.5 Pro 同时发布的窗口期进一步推上去**——这正是开发者最需要 A/B 跑多家模型的时刻。

---

### 5️⃣ [swc-project/swc](https://github.com/swc-project/swc) — +163⭐

**Rust 前端工具链的"二次复兴"**

swc 是基于 Rust 的 JavaScript / TypeScript 编译器，定位是 Babel / TSC 的高性能替代品。它的核心客户原本是 Next.js（默认编译器），但近期重新热起来跟两件事相关：**一是 Vite / Turbopack 等新一代构建器持续向 swc 靠拢**；**二是 TypeScript 6.0（Rust 端口）路线让前端社区重新对 Rust-based toolchain 有了兴趣**。

今天 +163⭐ 在重点项目里不算最高，但对一个 33k 星的成熟项目来说是显著上扬。这也是更大趋势的局部投影——**编译器/打包器/Linter 这一栈正在彻底 Rust 化（biome、swc、oxc、turbopack）**。社区从"JS 写一切"的纯粹转向"边缘工具用 Rust、业务逻辑用 TS"已经是事实。

---

## 生态观察

今天的 trending 排布反映了三条主线：

1. **Agent 安全成为基础设施**：SkillSpector 一上线就直冲第二，说明 Agent 平台从"用起来"进入"管起来"的阶段，安全扫描、权限沙箱、技能签名将是接下来 3-6 个月的工具焦点。
2. **垂直行业 Foundation Model 走出实验室**：Kronos 把"K 线即语言"做成开源；和 ai-daily 里讨论的"行业垂直 Agent"一脉相承——通用模型见顶后，资本和注意力转向"行业 + 领域数据 + 中等规模模型"。
3. **基础工具链持续低噪上涨**：swc、cypress、puppeteer、pytest 这些十年老仓库今天都在榜上，说明前端 / 测试 / 自动化等"非 AI 工具"并没有被 LLM 浪潮吸干注意力，反而因为"AI 写代码越多 → 测试和工具链越关键"而获得二次红利。

冷却信号：今天没有看到任何与"通用 chat UI"或"prompt engineering 课程"相关的仓库上榜——这块的注意力红利基本结束。
