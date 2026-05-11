# GitHub Trending 日报 · 2026-05-11

## 今日焦点

> **Claude 生态全面爆发 · AI Agent Skills 工程化 · 金融垂直场景 · 多模型路由 · 国内开源教育**
>
> - `anthropics/financial-services` Anthropic 官方下场做金融领域 reference impl，+1,479⭐ 仅次于综合榜首
> - `addyosmani/agent-skills` 把 "Skills" 写法变成行业事实标准，单日 +1,092⭐
> - `affaan-m/everything-claude-code` Claude Code 配套生态聚合，存量已破 17 万⭐
> - `decolua/9router` 多家模型免费聚合路由，单日 +806⭐ 反映用户对"成本套利"的强需求
> - `bytedance/UI-TARS-desktop` 字节多模态 Agent 桌面端开放栈，+656⭐ 稳坐 GUI Agent 第一梯队

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [anthropics/financial-services](https://github.com/anthropics/financial-services) | 金融服务场景的 Claude 参考实现 | Python | 18,614 | +1,479⭐ | 2,400 |
| 2 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 面向 AI Coding Agent 的工程化 Skills 集合 | Shell | 38,268 | +1,092⭐ | 4,245 |
| 3 | [affaan-m/everything-claude-code](https://github.com/affaan-m/everything-claude-code) | Claude Code 周边/插件/配置聚合 | JavaScript | 177,961 | +1,011⭐ | 27,492 |
| 4 | [decolua/9router](https://github.com/decolua/9router) | 多家 AI 编程模型免费聚合路由 | JavaScript | 7,184 | +806⭐ | 1,227 |
| 5 | [datawhalechina/hello-agents](https://github.com/datawhalechina/hello-agents) | Agent 原理与实战教程（中文） | Python | 46,400 | +756⭐ | 5,590 |
| 6 | [bytedance/UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop) | 字节多模态 AI Agent 桌面端开源栈 | TypeScript | 32,010 | +656⭐ | 3,178 |
| 7 | [datawhalechina/easy-vibe](https://github.com/datawhalechina/easy-vibe) | 面向新手的现代编程入门课 | JavaScript | 9,055 | +642⭐ | 891 |
| 8 | [playcanvas/supersplat](https://github.com/playcanvas/supersplat) | 3D Gaussian Splat 编辑器 | TypeScript | 6,729 | +604⭐ | 762 |
| 9 | [CloakHQ/CloakBrowser](https://github.com/CloakHQ/CloakBrowser) | 反检测 Chromium，Playwright 兼容 | Python | 4,544 | +567⭐ | 359 |
| 10 | [HKUDS/AI-Trader](https://github.com/HKUDS/AI-Trader) | 全自动 Agent-Native 量化交易 | Python | 15,451 | +255⭐ | 2,517 |
| 11 | [jundot/omlx](https://github.com/jundot/omlx) | Apple Silicon 上的连续 batching LLM 推理服务 | Python | 13,221 | +187⭐ | 1,132 |
| 12 | [lsdefine/GenericAgent](https://github.com/lsdefine/GenericAgent) | 自演化 Agent，主打降低 token 消耗 | Python | 10,475 | +170⭐ | 1,193 |

---

## 重点项目点评

### 🥇 [anthropics/financial-services](https://github.com/anthropics/financial-services) — +1,479⭐

**Anthropic 亲自下场，把"垂直领域 reference 实现"提到与基础工具同等的地位**

这是今天最值得关注的一条信号。一年前 Anthropic 还以"基础模型 + API + Claude Code"为主要叙事，今天直接由官方发布金融服务领域的参考实现仓库——意味着模型厂商正在把"行业模板"列为一级产品。仓库里覆盖了风控、合规审计、研报生成、客服 copilot 等典型金融场景，每个场景都给出 Skills、prompt、评测和审计日志的完整模板。

更关键的是节奏：在 Claude 4.7 发布、Skills 机制成为新一代 agent 写法标准之后，官方用一个高合规要求的行业打样，等于在告诉 ISV 和银行内部团队"标准答案长这样"。这对国内一众"金融大模型"项目是一次正面挤压——大家原本各自摸索 prompt 和 RAG，现在有了官方对照系。预计未来两周会看到 medical-services、legal-services 之类的同类 repo 出现。

---

### 🥈 [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — +1,092⭐

**Skills 正在像 npm 包一样被工程化、被收藏、被复用**

Addy Osmani（Google Chrome 团队的前端权威）下场做这个仓库本身就是个事件——他过去十年的几个仓库（如 `essential-image-optimization`、`learning-jsdesignpatterns`）几乎是前端开发者必读。这一次他把目光锁定在 AI Coding Agent 的 "skill" 写法上：仓库给出了一套"生产级"模板，把 skill 当作可复用工程资产去版本化、测试、文档化。

这背后是一个明显趋势：自从 Claude Code 推出 Skills 以后，提示词不再以"咒语"形式散落在 Discord 截图里，而是开始变成可仓库化、可代码评审、可发布订阅的资产。今日榜单上还有 `affaan-m/everything-claude-code`，两者一上一下卡在 1000+ 增量，说明社区已经从"惊叹"过渡到"标准化"。

---

### 🥉 [affaan-m/everything-claude-code](https://github.com/affaan-m/everything-claude-code) — +1,011⭐

**17 万星的体量说明 Claude Code 周边已是顶级生态**

这是一个聚合型仓库：插件、skills、subagent 模板、settings 样例、hooks 写法、各种工作流的最佳实践全收。17 万⭐、27k fork 的体量意味着它已经是 awesome-list 中的"国民级"项目，类似 `awesome-react` 之于 React。

值得注意的是：Cursor、Continue、Aider 都有自己的拥趸，但生态聚合型 repo 的体量明显落后 Claude Code 一个数量级。这说明一件事——以"在终端 + 自带 Skills/Hooks/MCP"为差异点的工具，更容易催生"代码即配置"的社区资产，而 IDE 类工具的扩展更分散、难以聚合。

---

### 4️⃣ [decolua/9router](https://github.com/decolua/9router) — +806⭐

**模型路由 = 当下最大的成本套利窗口**

定位很务实：聚合 OpenAI、Anthropic、Google、字节、DeepSeek、Qwen、Kimi 等多家模型，做免费/低价路由 + auto-fallback。看似工具向，但增量曲线很激进——一周前还是几百星，今天单日 +806⭐ 冲进 top 10。

它能跑起来的根本原因有两个：一是各家模型的 API 行为差异已经被社区抹平得足够好（OpenAI 兼容接口几乎成事实标准），二是个人开发者对"哪个模型现在便宜/限时免费"的敏感度被 Claude Code、Cursor 这些工具放大了。同类项目还有 `LiteLLM`、`OpenRouter`、`one-api`，但 9router 主打"配置极简、可托管在用户自己机器"，正好戳中开发者隐私 + 成本的双重诉求。

---

### 5️⃣ [bytedance/UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop) — +656⭐

**字节的 GUI Agent 桌面栈持续蓄力，已是中文区第一梯队**

UI-TARS 是字节去年发布的多模态 GUI 操作模型，desktop 这个 repo 把模型 + 调度 + agent infra 打包成一个可本地跑的桌面端开源栈。今天 +656⭐ 不算爆发，但已经累积到 32k⭐，是 GUI Agent 方向上和 OpenAI Operator、Anthropic Computer Use 同档的本土对手。

值得观察的是：GUI Agent 这条线在 2026 年明显从"demo 跑通"进入"产品化落地"阶段，UI-TARS-desktop 直接对标的是给 ISV 提供自托管的桌面自动化栈，而不是 SaaS。这一定位和国内大量"内部数据不能出网"的客户高度契合，所以增长曲线会比海外友商更稳。

---

## 生态观察

今天榜单基本可以用一句话总结：**Claude 生态的"工程化"已经压过了"惊叹期"**。前三位有两个来自 Anthropic 官方/Claude 周边，第四位是为弥补 Claude 成本而生的多模型路由——这意味着 Claude Code/Skills 已经不只是开发工具，而是一个有插件市场雏形的平台。

另一条暗线是 **Agent 方向的两极分化**：上层是 `agent-skills`、`everything-claude-code` 这种"组装乐高"式的应用层，下层是 `omlx`、`GenericAgent` 这种死磕推理效率和 token 消耗的基建层。中间的"通用 agent framework"反而不再上榜，LangChain 时代正式过去了。

国内开源教育这条线也在延续：`datawhalechina` 一天上两个（`hello-agents` 和 `easy-vibe`），节奏稳定。3D 方向唯一上榜的 `supersplat` 提醒大家：Gaussian Splat 已经从研究 demo 变成可视化工具链的一环，预计明年会出现"3DGS 编辑 SaaS"这一品类。
