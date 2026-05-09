# GitHub Trending 日报 · 2026-05-10

## 今日焦点

> **Anthropic 进入金融垂直 · Agent Skills 工程化爆发 · 中文 Agent 教程持续走强 · 3D 与 DevTools 工具回潮**
>
> - `anthropics/financial-services` 一日 +3,077⭐ 登顶，Anthropic 直接下场做投行/股研/PE 垂类 Agent
> - `addyosmani/agent-skills` +2,801⭐，Addy Osmani 把"高级工程师工作流"打包成可装载的 Skill 包
> - `datawhalechina/hello-agents` +1,162⭐，中文 Agent 教程总星已破 4.5w，国内 Agent 学习需求仍在爬升
> - `decolua/9router` +980⭐，"40+ 提供商免费 AI 编码"小工具异军突起，反映模型路由层仍是空白
> - `playcanvas/supersplat` +513⭐，3D Gaussian Splat 编辑器持续吸量，Web3D 工具链成熟度提升

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [anthropics/financial-services](https://github.com/anthropics/financial-services) | Anthropic 官方金融服务参考 Agent、Skill 与数据连接器 | Python | 17,192 | +3,077⭐ | 2,175 |
| 2 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 面向 AI 编码 Agent 的生产级工程 Skill 集合 | Shell | 37,263 | +2,801⭐ | 4,165 |
| 3 | [datawhalechina/hello-agents](https://github.com/datawhalechina/hello-agents) | 从零开始构建智能体（中文系统教程） | Python | 45,625 | +1,162⭐ | 5,523 |
| 4 | [decolua/9router](https://github.com/decolua/9router) | 40+ 提供商免费 AI 编码路由器，支持自动 fallback | JavaScript | 6,407 | +980⭐ | 1,157 |
| 5 | [masterking32/MasterDnsVPN](https://github.com/masterking32/MasterDnsVPN) | 高性能 DNS 隧道 VPN，绕过审查 | Go | 2,421 | +595⭐ | 256 |
| 6 | [bytedance/UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop) | 字节开源多模态 AI Agent 桌面端 | TypeScript | 31,315 | +549⭐ | 3,114 |
| 7 | [rohitg00/agentmemory](https://github.com/rohitg00/agentmemory) | AI 编码 Agent 持久化记忆方案 | TypeScript | 3,339 | +518⭐ | 336 |
| 8 | [playcanvas/supersplat](https://github.com/playcanvas/supersplat) | 浏览器端 3D Gaussian Splat 编辑器 | TypeScript | 6,197 | +513⭐ | 724 |
| 9 | [datawhalechina/easy-vibe](https://github.com/datawhalechina/easy-vibe) | Vibe Coding 2026 现代化编程入门课 | JavaScript | 8,454 | +294⭐ | 855 |
| 10 | [Lordog/dive-into-llms](https://github.com/Lordog/dive-into-llms) | 动手学大模型（中文实战教程） | Jupyter Notebook | 36,454 | +194⭐ | 4,483 |
| 11 | [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) | 让编码 Agent 用上 Chrome DevTools 的 MCP | TypeScript | 38,759 | +159⭐ | 2,451 |
| 12 | [oracle-devrel/oracle-ai-developer-hub](https://github.com/oracle-devrel/oracle-ai-developer-hub) | Oracle AI 数据库与 OCI 开发者资源 | Jupyter Notebook | 758 | +153⭐ | 228 |
| 13 | [rowboatlabs/rowboat](https://github.com/rowboatlabs/rowboat) | 开源带记忆的 AI 协同 Agent | TypeScript | 13,710 | +144⭐ | 1,360 |

---

## 重点项目点评

### 🥇 [anthropics/financial-services](https://github.com/anthropics/financial-services) — 今日榜首，+3,077⭐

**Anthropic 把 Claude 卖进华尔街：11 个垂直 Agent + 6 个行业 Skill 包**

这是 Anthropic 官方仓库，今天直接空降 Trending 榜首，单日涨 3k+。仓库内容并不是新的模型或框架，而是一整套**金融服务行业的参考实现**：11 个 Named Agent（Pitch Agent、Earnings Reviewer、Model Builder、KYC Screener、GL Reconciler 等）+ 6 个行业 Plugin（Investment Banking、Equity Research、Private Equity、Wealth Management、Fund Admin）+ 与 FactSet、S&P Global、Moody's、PitchBook、LSEG 等 11 家数据商的 MCP 连接器。

战略层面的信号比代码本身更重要。Anthropic 这一手等于把 Claude 直接装进了投行分析师、股研团队、PE 风控、财富顾问的真实工作流，**用产品化的"行业模板"代替单纯的 API**。`/dcf`、`/lbo`、`/cim`、`/ic-memo` 这种命令的出现，意味着 Claude 已经从"通用聊天工具"走到"替代分析师 90% 重复劳动"的位置——只是免责声明仍强调"仅供分析师起草，由人类复核"。

对生态的辐射也明显：`addyosmani/agent-skills` 在同一天爆发不是巧合，**Skill 作为 Claude Code/Cowork 的可移植工程资产，正在形成新的开发者生态**。今天的双雄登顶，等于一次官方+社区的联动宣传。

---

### 🥈 [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — +2,801⭐

**Addy Osmani 把"高级工程师工作流"打包成可装载 Skill**

Google Chrome DevRel 元老 Addy Osmani 的新仓库，思路非常清晰：把 spec → plan → build → test → review → ship 这套软件工程闭环写成 7 个斜杠命令 + 21 个核心 Skill + 3 个 Persona（代码审查、测试工程、安全审计），让 Claude / Cursor / Gemini / Copilot 这些 Agent 都能装上"高级工程师的肌肉记忆"。

最值得注意的不是 Skill 本身，而是它的设计哲学：**强调"过程优先于辞藻"**，每个 Skill 都带"反合理化表"（anti-rationalization table）——专门拦截 Agent 那些"我先跳过测试因为时间紧"的偷懒借口，强制要求"可验证证据"（测试通过、构建输出、运行时数据）才算完成。

这其实是 Agent 工程实践的一个分水岭：从"提示工程"进入"流程工程"。配合 Anthropic 当天发布的 financial-services 模板，**Skill 文件正在成为 2026 年最重要的"可分发 AI 工程资产"形态之一**——比 Prompt 重，比 Agent 框架轻，刚好填充团队规范和工具调用之间的空白。

---

### 🥉 [datawhalechina/hello-agents](https://github.com/datawhalechina/hello-agents) — +1,162⭐

**4.5w 星的中文 Agent 系统教程：依然是国内最稳的入门路径**

Datawhale 这个仓库已经积累到 45,625 ⭐，今天再涨 1k+。它不是任何一个 Agent 框架，而是一本完整的中文教科书：16 章覆盖 ReAct/Plan-and-Solve 等经典范式、Coze/Dify 等低代码平台、记忆系统/RAG/上下文工程、多 Agent 通信协议、强化学习直至毕业项目（旅行助手、研究 Agent、模拟小镇）。

它的持续走强反映了两个现实：一是中文世界 Agent 学习需求仍在大量增加，二是**国内开发者更倾向于"系统课程"而非英文圈那种"边看 README 边试错"的工程文化**。同一天 `Lordog/dive-into-llms`（也是中文，3.6w⭐）继续涨 194⭐，`datawhalechina/easy-vibe`（Vibe Coding 中文课）涨 294⭐，三本中文 AI 教科书同时在榜，是国内 AI 教育需求结构化的明确信号。

---

### [decolua/9router](https://github.com/decolua/9router) — +980⭐

**模型路由层的"瑞士军刀"：40+ 提供商免费 AI 编码**

这个仓库在今天的榜单里属于"小品级"突围——一个 JavaScript 路由器，把 40+ 模型提供商打通，提供自动 fallback 和"免费 AI 编码"能力。它解决的是普通开发者最现实的痛点：**模型 API 价格碎片化、限速频繁、可用性参差**。

它能在一日内拿下 +980⭐，反过来说明**官方 SDK 和 LiteLLM、OpenRouter 这类成熟方案没能彻底覆盖业余/学生开发者的"零成本编码"场景**。模型路由依旧是一个有空间的中间层——只是商业化路径比较模糊，多数项目最终会沦为薅羊毛工具或被大厂收编。

---

### [playcanvas/supersplat](https://github.com/playcanvas/supersplat) — +513⭐

**Web 端 3D Gaussian Splat 编辑器：3D 工具链回归 Web**

PlayCanvas 出品的 SuperSplat 不是新项目，但持续在 Trending 出现说明 **3D Gaussian Splatting** 已经从 2024 年的研究热点走到 2026 年的工具产品化阶段。它是纯浏览器、零安装的 Splat 检视/编辑/优化/发布工具，受众是 3D 艺术家和 WebXR/游戏内容创作者。

在 LLM 占据榜单大头的当下，`supersplat` 的存在提醒我们**视觉/3D 这条线并未停滞**——Gaussian Splatting 的工具链成熟度（捕获、编辑、压缩、发布）正快速接近传统三维资产管线。这条赛道一旦和多模态 Agent 融合（"用自然语言修改 3D 场景"），可能成为 2026 下半年值得关注的新方向。

---

## 生态观察

今天的榜单是典型的**"Agent 工程化日"**：Anthropic 官方做行业模板（financial-services）、社区大佬做工程流程（agent-skills）、中文社区做系统教程（hello-agents、easy-vibe、dive-into-llms），三股力量同向叠加。

**两个清晰的趋势**：

1. **Skill 成为新的一级资产**：从"写 Prompt"到"封装 Skill"再到"组合 Agent 工作流"，开发者群体正在把私有工程经验产品化为可分发的 Skill 包。Anthropic 官方仓库 + Addy Osmani 个人仓库同时登顶，说明这条路径已经被双向认可。
2. **模型路由 / 记忆 / 桌面 Agent 仍是中间层蓝海**：`9router`、`agentmemory`、`UI-TARS-desktop`、`rowboat` 全部在前 13——基础模型已被巨头垄断，但**模型上面那一层（路由、记忆、UI、协作）依旧分散**，新项目仍能靠单点功能吸量。

**冷却信号**：纯模型仓库（基础 LLM、训练框架）今天几乎不在榜，反映 2026 年开源世界的注意力已经从"造模型"彻底转向"用模型搭产品"。
