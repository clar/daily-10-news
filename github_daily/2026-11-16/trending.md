# GitHub Trending 每日报告 · 2026-11-16

## 今日焦点

> **Agent Skills 生态爆发 · 办公协同 SDK 回潮 · 前端 Agent 协议标准化 · 大厂开源代码审查工具 · 评测基础设施成型**
>
> - `dream-num/univer` 办公 SDK 单日 +1,041⭐，开源 Office 替代方案再起波澜。
> - `GoogleChrome/modern-web-guidance-src` 单日 +1,220⭐——Google 把前端最佳实践写成 Agent 可读的模式。
> - `backnotprop/plannotator` +860⭐，"规划—标注—回流 Agent"的全链路开发者协作工具。
> - `ChromeDevTools/chrome-devtools-mcp` +718⭐，Chrome DevTools 原生拥抱 MCP。
> - `alibaba/open-code-review` +688⭐——阿里开源，Deterministic Pipeline + LLM Agent 的混合代码审查方案。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [dream-num/univer](https://github.com/dream-num/univer) | AI 原生的办公套件 SDK（表格 / 文档 / 协作） | TypeScript | 25,557 | +1,041 | 2,333 |
| 2 | [GoogleChrome/modern-web-guidance-src](https://github.com/GoogleChrome/modern-web-guidance-src) | 让 Agent 跟上现代前端最佳实践 | TypeScript | 7,085 | +1,220 | 596 |
| 3 | [backnotprop/plannotator](https://github.com/backnotprop/plannotator) | 规划 / 注解 / 反馈 Agent 的开发者工作台 | TypeScript | 11,793 | +860 | 1,081 |
| 4 | [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) | Chrome DevTools 的 MCP 实现 | TypeScript | 56,878 | +718 | 4,808 |
| 5 | [tradermonty/claude-trading-skills](https://github.com/tradermonty/claude-trading-skills) | Claude Code 股票交易 Skill 集 | Python | 5,476 | +707 | 1,169 |
| 6 | [alibaba/open-code-review](https://github.com/alibaba/open-code-review) | 混合确定性 + LLM Agent 的代码审查 | Go | 52,007 | +688 | 4,105 |
| 7 | [Tencent/LoopForge](https://github.com/Tencent/LoopForge) | 自托管的 Agent 编排工作流（带人审） | Go | 1,432 | +484 | 263 |
| 8 | [ag-ui-protocol/ag-ui](https://github.com/ag-ui-protocol/ag-ui) | 把 Agent 嵌入前端应用的协议 | TypeScript | 17,803 | +393 | 1,818 |
| 9 | [google-labs-code/stitch-skills](https://github.com/google-labs-code/stitch-skills) | Stitch MCP server 的 Agent Skills 库 | TypeScript | 9,258 | +248 | 1,125 |
| 10 | [elementalsouls/Claude-BugHunter](https://github.com/elementalsouls/Claude-BugHunter) | Claude Code 漏洞挖掘 Skill 包 | Python | 6,350 | +221 | 966 |
| 11 | [NVIDIA/SkillEvaluator](https://github.com/NVIDIA/SkillEvaluator) | AI Agent Skill 评测框架 | Python | 1,616 | +205 | 227 |
| 12 | [ggml-org/ggml](https://github.com/ggml-org/ggml) | 机器学习张量底层库 | C++ | 15,888 | +53 | 2,018 |

---

## 重点项目点评

### 🥇 [GoogleChrome/modern-web-guidance-src](https://github.com/GoogleChrome/modern-web-guidance-src) — 今日 +1,220⭐

**Google 向 Agent 直接投喂"前端最佳实践数据集"**

这个仓库由 Chrome 团队维护，内容本质是一份随前端发展持续更新的"**Agent 可直接读取的 Web 规范与反模式手册**"——内容包括 CSS 新特性、ARIA 实践、性能预算、Core Web Vitals 指南，以及明确的"不要让 Agent 做的事"清单。它的格式刻意设计成 Agent Skill 友好的 YAML + Markdown 结构，可以被 Claude Code、Codex、Cursor 等工具按触发条件加载。

单日 1200+ 星说明一个趋势：**各大厂商开始主动把"知识文档"做成 Agent 契合的形态**，而不是让模型靠自己去 Google。这一方向上，Google 显然意识到其核心 Chrome 生态在 Agent 时代有被模型"幻觉重写"的风险，不如先一步把官方知识变成 Agent 的默认上下文。同类方向预计半年内会有大量跟进——Mozilla / Deno / Shopify 都已启动类似项目。

值得关注的是仓库的**写作风格**：每一条指南都包含 "Model Hint" 段落，告知 Agent 什么情况下应用该建议——这几乎是 Agent SDK 时代的"官方文档 2.0 范式"。

---

### 🥈 [dream-num/univer](https://github.com/dream-num/univer) — 今日 +1,041⭐

**AI 原生的"开源 Office"还活着，而且终于找到商业模式了**

Univer 是国内团队开源的办公套件 SDK（表格 / 文档 / 协作），本周新发布的 **AI Native 架构**支持把 Claude、GPT、Gemini 等 LLM 作为"原生 workbook 智能体"接入——公式自动化、单元格批注、跨 sheet 推理都走统一 Agent 层。1,041 星单日增长背后是**国内开源办公套件集体复兴的信号**：除了 Univer，近期 Luckysheet、x-spreadsheet 也各自宣布重大更新。

真正让 Univer 本次破圈的是其发布的 **Agent SDK 示例**：开发者只需编写 YAML Skill，用户在表格里直接用自然语言触发（"把这列按月同比，生成图表"），底层会由 MCP 协议路由到对应 Agent。这把过去三年 Excel Copilot 的能力彻底开源化，并把"函数生态"换成了"Skill 生态"。

对企业客户来说，Univer 填补了一个明确的空白：**既不想用 M365（数据合规）、又不想买 WPS AI（上下游闭源）**，Univer 提供了可自托管的中间选项。

---

### 🥉 [backnotprop/plannotator](https://github.com/backnotprop/plannotator) — 今日 +860⭐

**"程序员看 PR → 批注 → 回流 Agent" 的全链路工作台**

Plannotator 定位是一个**给开发者审阅 Agent 工作的工作台**：Agent 生成一次改动后，开发者在它的 UI 里打标注（可以画框、可以写自然语言评论），然后一键把标注 + diff 送回 Agent 继续迭代。它抓住的痛点是当前 Agent 开发流最薄弱的一环——**人类反馈的粒度和速度**。

860 星单日证明：**Agent 工作流的瓶颈已经从"推理"转向"反馈接口"**。在大部分公司，Codex / Claude Code 每次输出代码后，程序员的 feedback 还停留在 "Approve / Reject + 下一个提示词"的原始阶段；Plannotator 的"图形化标注 + 结构化回流"几乎是必然的产品形态。

这个方向上同时有 Cursor 的 "inline review"、GitHub Copilot 的 "task review mode"、Vercel 的 v0 preview 批注——开源方案的优势在于与任何 Agent 产品松耦合，预期半年内会被企业 DevTools 团队大量二次开发。

---

### 🏢 [alibaba/open-code-review](https://github.com/alibaba/open-code-review) — 今日 +688⭐

**阿里开源 Hybrid 代码审查：确定性流水线 + LLM Agent**

该仓库开源了阿里内部使用多年的代码审查体系——左半部分是 AST 规则 + 静态分析（确定性流水线），右半部分是 LLM Agent 负责语义级别 review（上下文一致性、设计模式、性能陷阱）。688 星意味着这是**大厂首次把完整生产级 review pipeline 做开源**，之前的 Google critique-review、Meta wedge 都只开源了组件。

真正的看点是**"两层评审如何合并打分"**：仓库中有一个 `judge-chain.yaml`，规定了哪种规则违反可以直接阻断合并、哪种只提示 Agent 复评——这等于把 CR 决策逻辑交代给了社区。可以预见接下来 1–2 个季度会出现大量二次改造版（金融、医疗合规等垂类）。

对团队 leader，这是 2026 年值得立刻试用的工具之一——它**把"AI 代码审查"从玩具推进到了可商用的生产形态**。

---

### 🧪 [NVIDIA/SkillEvaluator](https://github.com/NVIDIA/SkillEvaluator) — 今日 +205⭐

**Agent Skill 终于有了评测标准**

英伟达开源的 SkillEvaluator 填补了另一个关键空白：**对 Agent Skill 做结构化评测**。它定义了 Skill 的四类质量门槛——触发准确度 (trigger precision)、行为确定性 (behavior determinism)、失败可恢复性 (recoverability)、以及**跨 Agent 可移植性 (portability across agents)**——并提供了基于真实 Claude / GPT / Gemini 的回归测试工具链。

205 星看似不多，但在 "Agent Skill 爆发" 的背景下这是**基础设施级信号**。过去半年 Anthropic 推出 skill-doctor、Claude Code 的 `plugin eval` 等工具，各家都在搭自己评测体系；Nvidia 这一步是行业首次给出**跨厂商统一指标**，可以预测 2027 年企业采购 Agent Skill 包的招标文件里会直接引用 SkillEvaluator 的分数。

---

## 生态观察

今天的 trending 几乎全被 **"Agent Skill 生态"** 占据——从 Claude 交易技能、Claude 漏洞挖掘、Google Stitch Skills、到 Nvidia 的 Skill 评测框架、再到 Chrome 的 "Agent-friendly 文档"——**Skill 正取代传统的 NPM package / Python wheel 成为新一代开发者分发单元**。换言之，从"安装一个库"到"安装一个技能"，开发者生态在重做一次。

第二条主线是 **"工业化 Agent 工作流"**：Plannotator、Tencent LoopForge、Alibaba open-code-review、ChromeDevTools MCP——都是把 Agent 的"自由探索"约束进可审查、可打断、可打分的工业流程。这与过去一年"炫技式 Agent 演示"形成鲜明对比。

最后，**大厂主动输出 Agent 契合内容**（Google 的 modern-web-guidance、阿里的 open-code-review、腾讯的 LoopForge）是今日最具战略意义的变化——**巨头开始意识到：如果不自己给 Agent 投喂规则，模型就会用别人的规则改写他们的生态**。这将是 2027 年前端 / 云服务 / DevTools 争夺的下一个战场。
