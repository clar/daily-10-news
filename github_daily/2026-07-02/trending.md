# GitHub Trending 每日榜 · 2026-07-02

## 今日焦点

> **Agent 全家桶继续屠榜 · AI 安全测试双升 · Vibe-Trading 走出 crypto · Facebook 押注 Agent-ready 设计系统 · 网关/多路复用两条基建线**
>
> - `msitarzewski/agency-agents` 今日榜首，+2,097⭐，"一键部署完整 AI Agency"，Shell 脚本编排。
> - `usestrix/strix` +1,195⭐，开源 AI 渗透测试自动化，安全侧最强新星。
> - `HKUDS/Vibe-Trading` +682⭐，个人交易 Agent，从 crypto 圈溢出到通用金融。
> - `facebook/astryx` +714⭐，Meta 首个"agent-ready"设计系统，剑指 LLM UI 生成。
> - `diegosouzapw/OmniRoute` +1,012⭐，231+ 提供商的免费 AI 网关。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | 一键部署"完整 AI Agency"，预设专家 Agent 编排 | Shell | 123,237 | +2,097⭐ | 20,062 |
| 2 | [hasaneyldrm/exercises-dataset](https://github.com/hasaneyldrm/exercises-dataset) | 433 个健身动作数据集（含图/视频） | HTML | 8,339 | +2,203⭐ | 944 |
| 3 | [usestrix/strix](https://github.com/usestrix/strix) | 开源 AI 渗透测试，自动发现并给修复建议 | Python | 29,598 | +1,195⭐ | 3,217 |
| 4 | [microsoft/AI-For-Beginners](https://github.com/microsoft/AI-For-Beginners) | 微软 24 课 AI 入门课程 | Jupyter | 50,377 | +1,086⭐ | 10,250 |
| 5 | [diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute) | 免费 AI 网关，聚合 231+ 提供商 + token 压缩 | TypeScript | 9,468 | +1,012⭐ | 1,459 |
| 6 | [facebook/astryx](https://github.com/facebook/astryx) | Meta 开源"Agent-ready"设计系统 | TypeScript | 2,541 | +714⭐ | 130 |
| 7 | [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) | 个人交易 Agent（LLM 驱动） | Python | 16,477 | +682⭐ | 2,799 |
| 8 | [ogulcancelik/herdr](https://github.com/ogulcancelik/herdr) | Rust 写的终端 Agent 多路复用器 | Rust | 9,558 | +611⭐ | 564 |
| 9 | [0xNyk/council-of-high-intelligence](https://github.com/0xNyk/council-of-high-intelligence) | 18 AI 人格协商决策框架 | Shell | 2,596 | +473⭐ | 243 |
| 10 | [allenai/olmocr](https://github.com/allenai/olmocr) | AI2 PDF 结构化工具，训练数据管线 | Python | 18,241 | +295⭐ | 1,502 |
| 11 | [Mebus/cupp](https://github.com/Mebus/cupp) | 常用密码字典生成工具 | Python | 6,233 | +185⭐ | 2,065 |
| 12 | [refactoringhq/tolaria](https://github.com/refactoringhq/tolaria) | Markdown 知识库桌面管理器 | TypeScript | 18,009 | +160⭐ | 1,223 |
| 13 | [logto-io/logto](https://github.com/logto-io/logto) | 开源 SaaS 身份认证基础设施 | TypeScript | 13,227 | +131⭐ | 903 |
| 14 | [Unclecheng-li/VulnClaw](https://github.com/Unclecheng-li/VulnClaw) | MCP 工具组合的渗透测试 Agent | Python | 1,556 | +123⭐ | 217 |
| 15 | [togatoga/karukan](https://github.com/togatoga/karukan) | Rust 神经日语输入法引擎 | Rust | 564 | +29⭐ | 33 |

---

## 重点项目点评

### 🥇 [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) — 今日榜首，+2,097⭐

**"一键部署一整间 AI Agency"——Sub-agent orchestration 的社区级模板**

agency-agents 的定位很直白：它不是新框架，而是把已有的 Claude Code / Codex / GPT-5.6 Terra 的 sub-agent 系统打包成一套预设的"部门制"角色（产品经理、前端工程师、市场、运营等），配上一系列 Shell 脚本让个人开发者能几分钟建起可运转的小团队。这类"Agent 全家桶"模板不是新概念，但这次冲上榜首说明 Sonnet 5 与 GPT-5.6 Terra 的定价下调让"多 Agent 并行"从财务上真的划算了。

有意思的是它选择 Shell 而不是 Python/TS 作为编排层，这对 CLI 用户友好但对 Windows 用户几乎劝退。评论区已经出现多个 Python fork 请求。加 2,097 星今日排在前 15 的第二（仅次于健身数据集），是当下"个人 Agency"叙事的社区风向标。

---

### 🥈 [usestrix/strix](https://github.com/usestrix/strix) — +1,195⭐

**AI 渗透测试从 PoC 走到"一天 1K⭐"，红队被 Agent 化的临界点**

Strix 主打"给我一个 URL 或者一个 repo，我告诉你漏洞在哪、怎么修"，底层是把开源渗透工具（如 nmap、burp scripts、sqlmap）用 Agent 编排 + LLM 决策整合。相比 VulnClaw（同榜第 14 名，MCP 组合）更成熟：文档、示例、CI 集成都齐全。今日 +1,195⭐，加上 VulnClaw 的 +123⭐，可以看出攻防两侧的开源 Agent 正在同时爆发。

Strix 的意义在于把渗透测试从"高门槛外包服务"降维到"开发者自助工具"。风险和机会同在——一旦这类工具足够成熟，中小 SaaS 的漏洞发现窗口会显著缩短，同时也让恶意方拿到更低的入门门槛。

---

### 🥉 [facebook/astryx](https://github.com/facebook/astryx) — +714⭐

**Meta 开源"Agent-Ready 设计系统"——押注 LLM 生成 UI 的下一阶段**

astryx 是 Meta 首个明确写着 "agent-ready" 的开源项目，核心思路：所有组件都带机器可读的 slot/prop schema、语义化 role、可组合的样式变量，让 LLM 生成 UI 时能"直接选组件而不用凑 CSS"。这实质上是把 React + Tailwind 的组合往更结构化的方向拉。

评论区争论最集中的是"这是不是 Radix + shadcn 的老酒新瓶"——技术层面很像，但 Meta 的加入让企业采购路径出现新可能：如果 Meta 内部产品线大量采用，第三方 SaaS 会跟风。Astryx 的中期意义不在开源社区，而在企业 Agent 生成 UI 的事实标准之争——LLM 时代 UI 组件库的第一次"重定标准"。

---

### 🌐 [diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute) — +1,012⭐

**231+ 模型提供商的"多云网关"，主打 token 压缩降本**

OmniRoute 走的是 OpenRouter / LiteLLM 的老赛道，但两点差异化：一是免费自托管（OpenRouter 中心化），二是内置多种 prompt/token 压缩策略，宣称能节省 20-40% token。1K+⭐ 一天说明 Sonnet 5 与 GPT-5.6 分级发布后，"多模型比价路由"再度成为开发者关注点。

有意思的是网关层今日同时爆的还有 `herdr`（终端 Agent 多路复用，+611⭐），说明"个人开发者的模型/Agent 层聚合"是当下最活跃的基建分支。这一层的商业化很难（免费网关注定卷成本），但作为 open source 项目对社区影响很大。

---

### 📈 [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) — +682⭐

**从 crypto Vibe 到通用交易 Agent——学术组开源"个人交易员"**

HKUDS（港大数据智能研究组）开源，取名 Vibe-Trading，但覆盖股票、期权、期货和 crypto。架构类似 finrobot/OpenBB Agent：接研究、接策略回测、接执行接口。今日 +682⭐ 前 10。

真正吸引社区的不是回测数据（其实很保守），而是它给出了"LLM 直接做交易决策"的完整工程模板——很多 quant 团队一直在私有栈里搭这套，但公开开源版本一直缺。风险显而易见：把 LLM 当决策器直接下单在真实市场极其危险；评论区已经有多位 quant 强调"这是研究/学习工具，别用真钱"。

---

## 生态观察

今日 Trending 榜的 15 个仓库里，有 9 个直接标签"AI Agent"、"渗透 Agent"、"交易 Agent"或"Agent 组件"，另有 3 个是围绕 Agent 的基建（网关、多路复用、设计系统），仅剩 3 个是与 Agent 无关的经典项（健身数据集、身份认证、日语输入法）。这个比例是过去半年 Trending 榜的新高——说明社区对"Agent 化"的实用兴趣已经从"试试看"进入"自己下场"。三个更细的趋势：**（1）安全攻防两侧同时开源化**（Strix、VulnClaw、cupp），这会加速中小 SaaS 的漏洞循环；**（2）网关/多路复用/聚合层依然是最卷的公开赛道**（OmniRoute、herdr），且必然进一步压缩商业 API 的中间毛利；**（3）Meta 开源"Agent-ready 设计系统"**是本轮榜单里最有战略意味的信号——一旦大厂开始定义 Agent 生成 UI 的组件标准，第三方 SaaS 会被强行拉入下一场生态战。
