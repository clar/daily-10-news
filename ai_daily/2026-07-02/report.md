# AI 每日资讯 · 2026-07-02

## 今日焦点

> **Claude Sonnet 5 上线 · GPT-5.6 Sol 分级发布 · Fable 5 全球回归 · Nvidia 数据中心 Q1 破 $75B · 欧盟 AI Act 8·2 分段生效**
>
> - **Anthropic 发布 Claude Sonnet 5**：定价 $2/$10（输入/输出，百万 token），Agent 编码 63.2% 接近 Opus 4.8 的 69.2%，同步取代 Free/Pro 默认模型。
> - **OpenAI 预览 GPT-5.6 Sol/Terra/Luna**：Sol 主打前沿推理与长时程 Agent；Terra 对标 GPT-5.5 但价格减半；Luna 主打最低延迟成本。Sol 仍受美国政府准入名单限制。
> - **Fable 5 7 月 1 日全球回归**：出口管制解除后重新上线；Mythos 5 仅限受审核的美国机构。
> - **Nvidia FY27 Q1 数据中心收入 $75.2B、同比 +92%**；AMD Q1 数据中心 $5.8B、+57% YoY，Lisa Su 上调服务器 CPU 五年 CAGR 至 35%。
> - **欧盟 AI Act 8 月 2 日**：GPAI 处罚权、透明度义务、市场监管机构同步激活；高风险 Annex III 系统合规期推迟至 2027-12。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Anthropic 发布 Claude Sonnet 5，Agent 编码逼近 Opus | TechCrunch / Anthropic | ⭐⭐⭐⭐⭐ |
| 2 | OpenAI 预览 GPT-5.6 家族（Sol/Terra/Luna），面向前沿推理 | OpenAI News | ⭐⭐⭐⭐⭐ |
| 3 | Fable 5 全球重新可用；Mythos 5 仅限美国政府审核机构 | Fable5.app / llm-stats | ⭐⭐⭐⭐ |
| 4 | Nvidia FY27 Q1 数据中心收入 $75.2B，同比 +92% | Silicon Analysts | ⭐⭐⭐⭐⭐ |
| 5 | AMD Q1 2026 数据中心 $5.8B、+57% YoY，上调服务器 CPU 长期预期 | DCD | ⭐⭐⭐⭐ |
| 6 | 欧盟 AI Act 8-2 分段生效，Digital Omnibus 推迟高风险条款到 2027 | AI Act EU | ⭐⭐⭐⭐ |
| 7 | 中国《AI 拟人化交互服务管理办法》7 月 15 日生效 | Bird & Bird | ⭐⭐⭐⭐ |
| 8 | Anthropic 5 月 Series H 融资 $65B，估值 $965B 反超 OpenAI | 综合新闻 | ⭐⭐⭐⭐⭐ |
| 9 | Figure AI Figure 03 量产 1 台/小时，全球部署破 10,000 台 | Meta Intelligence | ⭐⭐⭐⭐ |
| 10 | Tesla Optimus 首线量产延迟至 7 月底/8 月，目标百万级 | KraneShares | ⭐⭐⭐ |
| 11 | DeepMind AI Co-Mathematician 在 FrontierMath Tier 4 拿下 48% | arXiv | ⭐⭐⭐⭐ |
| 12 | Perplexity 完成 E-6 轮融资，估值 ~$21B | AI Business Weekly | ⭐⭐⭐ |
| 13 | 白宫签署《促进先进 AI 创新与安全》行政令 | White House | ⭐⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Anthropic 发布 Claude Sonnet 5：把 Opus 级别的智能塞进 Sonnet 的价格

**[TechCrunch](https://techcrunch.com/2026/06/30/anthropic-launches-claude-sonnet-5-as-a-cheaper-way-to-run-agents/) · [Anthropic Newsroom](https://www.anthropic.com/news)**

Anthropic 于 6 月 30 日上线 Claude Sonnet 5，并从 7 月 1 日起将其设为所有 Free 与 Pro 用户的默认模型。定价方面，8 月 31 日之前推广价 $2 / $10（输入/输出，百万 token），比 Sonnet 4.6 更便宜。Claude Code 也同步启用 Sonnet 5 为默认模型，并开放原生 1M 上下文窗口。

在实际能力上，Sonnet 5 在 Agent 编码基准拿下 63.2%，介于 Sonnet 4.6 的 58.1% 与 Opus 4.8 的 69.2% 之间；在部分知识工作基准上甚至反超 Opus 4.8。这意味着 Anthropic 用一款"降价 30%~40%、能力却只差 Opus 6 个点"的模型，把整个中端 Agent 推理市场重新定价。对 SaaS 与开发者工具生态来说，这是过去 12 个月最重要的价格信号——之前必须调 Opus 才能跑通的复杂多步 Agent 工作流，现在可以在 Sonnet 5 上批量化。

值得关注的两个后续变量：一是 Sonnet 5 上线后 Opus 4.8 的使用份额会如何被侵蚀，二是 OpenAI GPT-5.6 Terra 是否会跟进"半价对标上一代旗舰"策略。Anthropic 5 月刚以 $965B 估值完成 Series H，估值反超 OpenAI 私募估值——用产品和资本节奏同时压制对手。

**点评：** Sonnet 5 不是"新版本"，是 Anthropic 对 Agent 定价权的一次夺回；GPT-5.6 若不在 Terra 上跟进降价，OpenAI 的 Agent 中端会被抽干。

---

### 🚀 No.2 · GPT-5.6 家族分级发布：Sol 只给"政府 vetted"客户

**[llm-stats](https://llm-stats.com/llm-updates) · [OpenAI News](https://openai.com/news/)**

OpenAI 本周同时上线 GPT-5.6 三兄弟：Sol（前沿推理 + 长时程 Agent）、Terra（对标 GPT-5.5 但价格减半）、Luna（最快最便宜的入门层）。Sol 号称在合成基准上超过 Mythos 5 与 Fable 5，但和后者不同——Sol 目前仍锁定在"美国政府审核过的伙伴"名单，没有公开发布时间。

这是 OpenAI 首次公开采用"能力分级 + 客户分级"的组合发布：顶级模型不再对所有 API 客户开放，而是走类似出口管制的白名单。背后既有安全部长办公室的合规压力，也有 OpenAI 自身在超算容量分配上的取舍——Sol 每次推理消耗远超 Terra/Luna，普适性上线只会拖累其他产品的 SLA。

与此同时，同一批出口管制解除也让 Fable 5 于 7 月 1 日全球重新上线（3 月被封锁后回归），Mythos 5 则仅限美国政府 vetted 机构使用。整个前沿模型市场从"公开可比"进入"分层可见"阶段，评测机构未来能看到的旗舰模型样本会明显收窄。

**点评：** "旗舰白名单化"是本轮最重要的结构性变化——公开 leaderboard 的信息价值正在被人为压缩，投资人和 CIO 只能靠 tier-1 客户口碑判断真实前沿。

---

### 💰 No.3 · Nvidia 数据中心 Q1 破 $75B、AMD 数据中心 +57%：Agent 需求把 CPU 也拉起来

**[Silicon Analysts](https://siliconanalysts.com/analysis/nvidia-ai-accelerator-market-share-2024-2026) · [DCD](https://www.datacenterdynamics.com/en/news/amd-posts-q1-2026-data-center-revenue-of-58bn-forecasts-120bn-server-cpu-income-by-2030/)**

Nvidia FY27 Q1 数据中心收入达 $75.2B、同比 +92%；AMD Q1 2026 数据中心收入 $5.8B、同比 +57%。AMD 上调服务器 CPU 三到五年 CAGR 预期从 18% 直接翻到 35%，理由是"agentic AI 应用对推理侧 CPU 计算的需求远超预期"，将 2030 年市场规模上修至 $120B+。

这里关键的变化是：过去两年市场把 AI 需求几乎完全等同于 GPU / accelerator，但 Agent 化推理（多轮 tool use、长上下文、编排层）实际把 CPU 计算量也一并放大。AMD Epyc 与 Instinct 的双轮增长第一次跑赢单一 GPU 叙事。Nvidia 依然占据 AI 加速器约 75-80% 份额，但相较 2024 年 87% 的峰值，主机厂加速自研（Trainium 3、TPU v7、MI400）+ AMD 追赶的结构性缓释开始显现。

对二级市场，这份数据意味着 AI 资本开支叙事在 2026 下半年仍能持续——只要 hyperscaler 保持每季度上调 capex 指引，Nvidia $54B Q3 指引就有兑现基础。风险变量在电力：多个数据中心的 2027 落地时间点被电网批复推迟。

**点评：** "Agent 化"是 AMD 唯一能追上 Nvidia 叙事的入口——CPU 承接编排层与轻量推理，是 AMD 未来 18 个月最大的估值反弹逻辑。

---

### 🏛️ No.4 · 欧盟 AI Act 8 月 2 日分段生效 + 中国 7 月 15 日 AI 拟人化服务办法：合规大分岔

**[EU AI Act](https://artificialintelligenceact.eu/) · [Bird & Bird](https://www.twobirds.com/en/insights/2026/china/china's-new-regulations-on-ai-anthropomorphic-interactive-services)**

欧盟 AI Act 将在 8 月 2 日进入"部分强制执行"阶段：GPAI 模型提供方的处罚权、Article 50 透明度义务、成员国市场监管机构同步激活；但根据 5 月 7 日达成的 Digital Omnibus 临时协议，高风险 Annex III 系统的强制合规日期从 2026-08-02 推迟到 2027-12-02，给企业多出 16 个月缓冲。GPAI 供应商仍有一年"调整期"才会真正被处罚。

中国这边节奏更快：网信办联合五部门于 4 月 10 日发布的《AI 拟人化交互服务管理办法》将于 7 月 15 日正式生效，涵盖虚拟陪伴、AI 聊天机器人、情感响应助手等全部品类，明确要求实名与心理健康提示。国务院同时明确正在起草综合性 AI 法。字节跳动因 AI 生成内容标识不到位收到网信办首个正式警告，标志国内进入"标签合规"实质执法阶段。

对全球厂商，两地节奏形成分岔：欧盟给基础模型侧的时间余量在拉长（Omnibus 让步），但对下游 App 层的透明度和标识要求正在硬化；中国相反，先从下游产品的场景合规切入，再向上补基础模型立法。这直接影响 Anthropic、OpenAI、xAI 在 EMEA/APAC 的产品部署路线。

**点评：** "推迟高风险 + 加强透明度"是欧盟在保产业竞争力和保安全之间的现实妥协；产品经理短期最痛的是 Article 50 标识义务，而不是 Annex III。

---

### 🤖 No.5 · Figure 03 量产破 1 台/小时，Optimus 首线推迟：人形机器人进入 hyperscaler 阶段

**[Meta Intelligence](https://www.meta-intelligence.tech/en/insight-physical-ai) · [KraneShares](https://kraneshares.com/humanoid-robotics-in-2026-the-race-from-pilot-to-platform/)**

Figure AI 在 BotQ 工厂宣布 Figure 03 达到 1 台/小时的下线速度，全球部署突破 10,000 台。BMW 斯巴坦堡工厂过去 11 个月部署两台 Figure 02，累计参与生产 30,000+ 辆 X3、搬运 9 万+ 冲压件、每台 1,250 小时净工时——第一次给出可量化的 unit economics。Boston Dynamics 电动 Atlas 也开始首批小规模部署。

Tesla 一侧节奏则明显偏慢：1 月宣布把 Fremont 一条 Model S/X 线改造为 Optimus 一代量产线（设计年产能百万台），但 Q1 电话会 Musk 已把量产起点从 Q2 推迟到"7 月底或 8 月"。虽然 Tesla 累计出货已号称超 5 万台，但绝大多数是内部工厂 pilot。

产业进入"从原型到平台"的关键转折，Goldman Sachs 预测 2035 年市场规模 $38B。真正的分水岭是 unit economics：Figure 通过 BMW 站点级数据证明每小时净贡献可覆盖机器人折旧；Optimus 仍缺少同等级别的可披露 pilot 数据。

**点评：** Figure 的 BMW 数据是本轮人形机器人最关键的一次"财务化"；Optimus 若在 Q3 财报里拿不出对等的每小时经济性，估值叙事会被明显重排。

---

## 行业观察

今天的信息面呈现三个同时演进的主线：**（1）模型定价权重排**——Anthropic 用 Sonnet 5 直接把 Agent 中端市场降价一档，OpenAI 用 GPT-5.6 三分级 + 白名单尝试重构溢价结构；**（2）资本 + 硬件的正反馈**——Nvidia/AMD 数据中心增速把 hyperscaler 与 Anthropic/OpenAI/xAI 的融资合理化，Q1 全球 VC 有 63% 流向四家 AI mega-round；**（3）监管开始"分层"**——欧盟推迟高风险条款保产业竞争、加固透明度义务；中国先从拟人化交互和内容标识入手做前台约束。三线合流的结果是：2026 下半年 AI 竞争已经不再是"谁的模型分数更高"，而是"谁能在监管边界内、以正确定价把 Agent 卖给企业"。这对第二梯队（Perplexity、Mistral、Cohere）意味着必须尽快找到自己的分层定位，否则会在 Sonnet 5 与 Terra 的价格夹击下失去入口。
