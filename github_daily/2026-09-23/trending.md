# GitHub Trending 每日榜单 · 2026-09-23

## 今日焦点

> **Agent Orchestration 全线开花 · Anthropic 官方仓罕见登顶 · Google `ax` 单日爆冲 2,300⭐ · Office 类工具向 Agent 场景重构 · 移动端取证工具再次进入公众视野**
>
> - `google/ax`：Google 新开源 Agent 编排运行时，单日 +2,324⭐，Go 生态迎来对标 LangGraph 的新玩家
> - `anthropics/financial-services`：Anthropic 首个"垂直行业解决方案"仓，官方直接下场做金融场景 playbook
> - `dream-num/univer`：老牌开源"Office 平台"改口为 Office Harness for AI Agents
> - `mvt-project/mvt`：移动设备取证工具，一次外部事件让下载量再度走高
> - `browser-use/video-use` 与 `superdesigndev/treg`：Agent 工具链继续下沉到视频编辑 / 工具路由等细分场景

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [google/ax](https://github.com/google/ax) | Google 开源 Agent 编排运行时 | Go | 7,496 | +2,324⭐ | 350 |
| 2 | [mvt-project/mvt](https://github.com/mvt-project/mvt) | 移动设备取证与入侵检测工具 | Python | 14,050 | +441⭐ | 1,351 |
| 3 | [anthropics/financial-services](https://github.com/anthropics/financial-services) | Anthropic 官方金融行业解决方案集 | Python | 36,300 | +436⭐ | 5,311 |
| 4 | [agent-substrate/substrate](https://github.com/agent-substrate/substrate) | Agent Substrate 核心系统 | Go | 2,935 | +301⭐ | 382 |
| 5 | [dream-num/univer](https://github.com/dream-num/univer) | 面向 AI Agent 的 Office 一体化平台 | TypeScript | 15,343 | +202⭐ | 1,367 |
| 6 | [superdesigndev/treg](https://github.com/superdesigndev/treg) | Agent 工具的 OpenRouter | Python | 2,176 | +197⭐ | 215 |
| 7 | [browser-use/video-use](https://github.com/browser-use/video-use) | 用代码 Agent 剪辑视频 | Python | 25,800 | +155⭐ | 3,115 |
| 8 | [davila7/claude-code-templates](https://github.com/davila7/claude-code-templates) | Claude Code 配置与监控 CLI | Python | 31,088 | +113⭐ | 3,536 |

*说明：上游 trending 页面今日仅返回 8 条稳定条目，其他条目因抓取限制未纳入。*

---

## 重点项目点评

### 🥇 [google/ax](https://github.com/google/ax) — 今日榜首，+2,324⭐

**Google 亲自下场做 Agent 编排，Go 阵营终于有了"参考实现"**

`ax` 是 Google 本周新开源的 "open agentic orchestration runtime"，纯 Go 实现，主打三件事：可组合的 tool graph、结构化任务图 (task graph, DAG + retries + human-in-the-loop) 以及原生的 OpenTelemetry / OTel Traces 观测。项目本身脱胎自 Google 内部的 Gemini Agent 平台，官方 README 强调"生产环境已跑 12+ 个月"。

单日 +2,324⭐ 是本月增速最猛的 Agent 类项目，社区反应也非常直接："这终于是一个能上 K8s 的 Agent 框架"。Python 那边 LangGraph、CrewAI、Autogen 竞争白热化，但 Go 侧一直空缺，`ax` 一发布几乎立刻被云原生 / 平台组的开发者认领。

对生态最大的影响：Google 一旦持续投入，会给"Agent 框架必须是 Python"的默认认知开出一个口子。运维栈以 Go 为主的公司在 2026 Q4 有了从"接入 LangGraph" → "用 ax 一站式跑"的路径。

---

### 🥈 [mvt-project/mvt](https://github.com/mvt-project/mvt) — +441⭐

**外部事件驱动的老牌取证工具再现峰值**

MVT (Mobile Verification Toolkit) 是 Amnesty International 安全实验室维护的取证工具，用来从 iOS / Android 备份中提取入侵痕迹，最初为 2021 年 Pegasus 揭露事件配套。今天冲榜与本周"FBI 员工数据泄露"、以及多个东欧公民社会组织被曝遭商业间谍软件监听的报道紧密相关。

这类项目的 star 曲线通常与事件驱动强相关，工具本身长期稳定迭代（macOS/Linux Docker 均可跑，最近版本新增 Android 14 的 heuristic）。对信息安全社区来说，MVT 已经成为个人 / 记者 / 高危职业者做"自我体检"的事实标准。

---

### 🥉 [anthropics/financial-services](https://github.com/anthropics/financial-services) — +436⭐

**Anthropic 首次以"垂直行业解决方案"出仓**

这是 Anthropic 官方账号下少见的 solution-oriented 仓库，包含：金融行业 prompt 模板、Compliance 检查工具链（KYC/AML 提示、法规文件切片方案）、以及若干 Claude Agent SDK 示例（贷款审核 workflow、风控事件汇总）。同一天官方 blog 发布 Claude Opus 5.5，两者时间线明显对齐。

对开发者的信号非常清晰：Anthropic 正在从"模型 API 提供方"往"行业 Reference Architecture 提供方"迁移，紧跟 OpenAI Enterprise 一直在做的模板策略。金融行业过去两年是企业 AI 采购最猛的板块之一，Anthropic 用官方仓库直接抢入。

值得关注的是仓库 fork 数已经 5,311——远超新仓平均值，说明多家银行 / SaaS 已经在做私有化落地。

---

### 🎯 [dream-num/univer](https://github.com/dream-num/univer) — +202⭐

**"Office 平台"改口为 Agent Runtime，产品定位第二次转身**

Univer 一年多前的 tagline 还是"面向下一代协作办公的开源平台"，现在直接改为 "Office Harness for AI Agents"。这次品牌 pivot 背后是产品结构上的真实变化：新增了完整的 tool-call schema，把 spreadsheet cell、doc block、slide layout 都做成 Agent 可调用的原生对象。

社区反馈：这是目前最完整的开源"表格 + 文档 + 幻灯"三合一 SDK，MIT 协议 + TS 实现，天然适合被作为 Agent 的"操作面板"。国内多个 RPA / Agent 平台已经在评论区确认接入路径。

Univer 的转向也是一个行业信号：2026 下半年，"Agent 需要一个操作系统"的共识正在形成，而 Office 类原语（表格 / 文档 / 幻灯）比通用 UI 组件库更接近人类的工作单位。

---

### 🧩 [google/ax](https://github.com/google/ax) 与 [agent-substrate/substrate](https://github.com/agent-substrate/substrate) — Go 阵营的双子星

两者今天同期冲榜并不是巧合。`ax` 来自 Google，`substrate` 来自 Agent Substrate（Anthropic 前员工创立、A16Z 支持的一家新公司），都用 Go 写。分别代表"大厂参考实现"与"独立系统底座"。

- `ax` 更像 LangGraph 的 Go 版本，重编排、重可观测；
- `substrate` 更接近 Ray + Temporal 的 Agent 版本，重执行 / 状态 / 恢复。

放在一起看，Agent 框架的语言之战真的开始从 Python 独占逐渐外溢。对企业选型来说，2026 Q4 需要开始把"Agent 平台的语言 = 团队栈的语言"纳入考虑。

---

## 生态观察

今日榜单几乎清一色 Agent 类项目：编排（ax / substrate）、工具路由（treg）、垂直行业解决方案（financial-services）、Agent 操作面板（univer）、Agent 场景应用（video-use）——五类五仓，覆盖了 Agent 栈的每一层。这与本周 GPT-6 Sol / Claude Opus 5.5 两连发形成呼应：模型价格降到"够用"之后，社区快速把注意力转向"如何拼出真正的 Agent 系统"。

一个新的品牌转向趋势：老仓不再自称"framework"或"platform"，而是明确加上 "for AI Agents" 后缀（Univer 就是典型）。既是营销跟风，也是产品结构确实需要为工具调用做原生化改造的信号。

安全类唯一进入榜单的 MVT 再次提醒：Agent 时代的攻击面正在扩展到"移动设备 + 个人代理"这一层——高危职业者与新闻工作者会在未来一年成为间谍软件的重点目标。
