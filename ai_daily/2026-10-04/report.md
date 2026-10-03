# AI 日报 · 2026-10-04

## 今日焦点

> **GPT-6 Sol 掀起价格战 · Anthropic Mythos 全家桶补齐 · Nvidia 锁定 TSMC A16 节点 · EU AI Act 高风险条款推迟 · 中国出口管制复议**
>
> - **OpenAI GPT-6 Sol 开 2026 下半年"腰斩"价格战**：输入 $2 / 输出 $10 每百万 token，是上一代 Sol 系列的一半价格，OpenAI 向 VentureBeat 明确这是"永久价格"而非促销。
> - **Anthropic Claude Opus 5 以半价对标 Fable 5**：7 月 25 日释出，定价 $5 / $25 per MTok，被定位为"接近 Mythos 级能力的低价版本"；至此 Anthropic Fable / Opus / Sonnet 全线补齐。
> - **Nvidia 确认成 TSMC A16 节点首发客户**：Vera Rubin GPU 下半年量产，TSMC 为此将 2026 资本开支上限上调至 $64B。
> - **EU AI Act 高风险条款推迟 1-2 年**：修订法案 (EU) 2026/1744 把 Annex III 类系统推迟到 2027-12-02，Annex I 推迟到 2028-08-02，但最高 €35M / 全球营收 7% 的罚则不变。
> - **美国 BIS 把 H200 / MI325X 等效芯片对华出口转入"逐案审查"**：年初生效的新规在 10 月进入关键执行节点，附加 50% 容量上限与 25% 关税。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | OpenAI GPT-6 Sol / Luna 发布，API 价格腰斩，1.05M context | VentureBeat / DataNorth | ⭐⭐⭐⭐⭐ |
| 2 | Anthropic Claude Opus 5 以 Mythos 级能力对标 Fable 5，定价减半 | Mezha / Threatcluster | ⭐⭐⭐⭐⭐ |
| 3 | Nvidia 锁定 TSMC A16 (2nm + BSPD) 作为 Vera Rubin 首发工艺 | TweakTown | ⭐⭐⭐⭐⭐ |
| 4 | EU AI Act Annex III/I 高风险条款推迟 1-2 年 | JDSupra / timewell | ⭐⭐⭐⭐ |
| 5 | 美国 BIS H200/MI325X 对华"逐案审查 + 25% 关税"进入执行期 | casrai / ecorpit | ⭐⭐⭐⭐ |
| 6 | Q1 2026 全球 VC 创纪录 $300B，AI 占 $188B（63%） | 投资季报 | ⭐⭐⭐⭐ |
| 7 | OpenAI 单季吞下 $122B 融资，Anthropic 考虑 11 月前后 IPO | Digg | ⭐⭐⭐⭐ |
| 8 | xAI 与 SpaceX 完成合并，Grok 更名 "SpaceXAI" 品牌 | tech-insider | ⭐⭐⭐ |
| 9 | Google Gemini 3.1 Pro / Flash-Lite 全面推送到付费订阅 | Google blog | ⭐⭐⭐ |
| 10 | MIT 调研：95% 企业 GenAI 试点未能进入生产 | benchlm.ai | ⭐⭐⭐⭐ |
| 11 | 企业评估重心从"跑分"转向可预测性、延迟预算、单位 token 经济 | ecorpit | ⭐⭐⭐ |
| 12 | Anthropic 游说支出首次超越 OpenAI，联邦 lobbying 同比增 7 倍 | theaireport | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · OpenAI GPT-6 Sol 把工作负载模型价格打到地板，并把 1M context 做成标配

**[OpenAI launches GPT-6 Sol and Luna, cuts API prices in half (DataNorth)](https://datanorth.ai/news/openai-launches-gpt-6-sol-and-luna)**

**[GPT-6 Sol / Luna Released: Features & Benchmarks (ComputingForGeeks)](https://computingforgeeks.com/gpt-6-sol-luna-released-features-benchmarks/)**

9 月 22 日 OpenAI 发布的 GPT-6 Sol / Luna 系列，到了 10 月已经基本把中端工作负载的"价格天花板"推翻一次。GPT-6 Sol 定价 $2 input / $10 output per million tokens，是上一代 GPT-5.6 Sol 的 50%；缓存输入再打 10 折，Batch / Flex 再打 5 折；OpenAI 向 VentureBeat 明确表示这是**永久价格**而不是上线促销。两款模型都把 context 推到 1.05M tokens，最大输出 128K，并把 reasoning effort 从 none 到 max 做成可切换参数，覆盖 Fast / 常规 / 深度思考三档。

真正的杀伤力不在"便宜"，而在于**把"便宜 + 1M 上下文 + agentic 工具调用"打包成一个 SKU**。之前 enterprise 为了拿到 1M context 普遍要走定制或 Mythos 级别模型；现在 $2 输入价格直接把这条护城河填平，直接压缩 Anthropic Opus 5 和 Google Gemini 3 Flash 的中端份额。

**点评：** 价格永久腰斩不是防守动作，是把推理成本当作新的分发渠道——谁的 token 更便宜，谁就有权利定义 agent 工作流的默认后端。接下来一个月，Anthropic 要么跟进降价，要么用 Mythos 级能力做"溢价叙事"，没有中间路线。

---

### 🚀 No.2 · Anthropic 补齐 Mythos / Fable / Opus / Sonnet 全家桶，Opus 5 用"半价 Fable"回敬 GPT-6

**[Anthropic 发布全新模型 Claude Opus 5 (Mezha)](https://mezha.ua/en/news/anthropic-predstavila-novu-model-claude-opus-5-313576/amp/)**

**[Anthropic Launches Claude Opus 5 Amid Cybersecurity Concerns (Threatcluster)](https://threatcluster.io/cluster/anthropic-releases-opus-5-with-close-to-fable-5s-capabilitie-dfa4825d)**

7 月 25 日 Anthropic 释出 Claude Opus 5，定价 **$5 / $25 per MTok**，官方口径是"能力接近 Fable 5 的前沿智能，价格只有一半"。至此 Anthropic 在 6-7 月完成了罕见的 **4 次 tier 事件**：6/9 开出 Mythos 级 Fable 5、6/30 发布 Sonnet 5、7/1 Fable 5 短暂出口管制下架后恢复、7/25 Opus 5 补位，官方第一次让每一个 tier 都对齐到当代架构。

Opus 5 真正的产品定位非常清晰：**在 Fable 5 不可用（出口管制 / 预算）或者不划算（纯 code 用例）时的默认替代**。它承接长时程 agentic coding、深度研究、多工具调用，并保留 Mythos 配套的安全分类器——这与 Fable 5 的"分类器可移除"版本 Mythos 5 形成明确的责任切分。

**点评：** Anthropic 这次的产品节奏首次表明它懂得"价格段位"而不是只会"能力段位"——用 Opus 5 应对 GPT-6 Sol、留 Fable 5 守住 agentic coding 高地、Mythos 5 承接政府 / 安全客户。IPO 窗口前把产品矩阵拉直，是对投资人最直接的话术。

---

### 🏭 No.3 · Nvidia 把 Vera Rubin 押在 TSMC A16，TSMC 把 2026 capex 推到 $64B

**[Nvidia rumored to be the first customer for TSMC's most advanced A16 process node in 2026 (TweakTown)](https://tweaktown.com/news/107720/nvidia-rumored-to-be-the-first-customer-for-tsmcs-most-advanced-a16-process-node-in-2026/index.html)**

A16 是 TSMC 的 2nm + 背面供电（BSPD）组合节点，之前只给了 AMD 一笔 AI chip 订单；10 月的最新消息是 Nvidia 下一代 Vera Rubin GPU 已选择 A16 作为**首发客户**，并与 TSMC 一同锁定下半年量产档期。TSMC 为了承接这波需求，把 2026 全年 capex 指引上调到 **$60B–$64B**，Jensen Huang 公开确认 Nvidia 已经在 2025 年取代 Apple 成为 TSMC 最大客户。

这不是单纯的制程竞争。A16 的 BSPD 把供电路径从背面走，让芯片正面能塞更多逻辑 / cache，直接决定 Vera Rubin 在推理单位成本（$ per 1M tokens）上的下一次下降幅度。Nvidia 用 A16 回应的，正是 GPT-6 / Opus 5 向 API 价格施加的下行压力：**在上游用更先进节点把每 token 边际成本再压一轮**。

**点评：** AI 行业的真正竞争正在从 "下一个 benchmark" 迁移到 "下一个 fab 节点"。A16 决定明年谁可以把 Opus / Sonnet 级智能跑进 $1 per MTok 以下，这是对非头部云厂商最大的生死线。

---

### 🏛 No.4 · EU AI Act 高风险条款推迟 1-2 年，但罚则保持原样

**[EU AI Act × Export Control 的叠加合规 (timewell.jp)](https://timewell.jp/en/columns/eu-ai-act-export-control-overlap)**

8 月 2 日 EU AI Act 到达一般适用日之后，修正法案 **(EU) 2026/1744** 把 Chapter III Sections 1-3 的高风险落地义务推迟：Annex III 系统推到 **2027-12-02**，Annex I 系统推到 **2028-08-02**。但最高 **€35M 或全球营收 7%** 的罚款额度维持不变；Annex III 列表中的八类高风险 AI，与欧盟出口管制中的"网络监控物项"重叠度极高，一旦从欧盟再出口到敏感目的地还要再过一道 Dual-Use (2021/821) 出口许可。

节奏上 EU 承认了"产业喘息"诉求，但保留了罚款与出口管制的双把柄——换言之，中大型美中模型厂进欧盟的边际合规成本并没有下降，只是把时间线拉长。

**点评：** 对企业选型来说，这意味着 2026-2027 继续按**"假装 Annex III 已经生效"** 来准备就是正解；把合规成本按时间折现算回来，推迟并不便宜。

---

### 🌏 No.5 · 美国对 H200 / MI325X 等效芯片对华出口转"逐案审查 + 25% 关税"

**[What changed: the AI chip export control landscape in 2026 (CASRAI)](https://casrai.org/wp/?p=2848)**

1 月 13 日 BIS 发布的终稿规则，把 **NVIDIA H200 / AMD MI325X 等效**芯片对华出口从"推定拒绝"下调到 **case-by-case review**，并新增 50% 容量上限、强制终端用途认证、25% 关税。10 月的焦点是执行层面的第一轮节奏：美方对终端用户名单、认证模板、关税叠加规则正在收紧，中国的采购节奏则同步从"抢量"转向"分流" ---- 一部分头部客户已经转向国产等效加速卡+小批量 B40/B50 的混合方案。

和 EU AI Act 推迟形成了鲜明对比：**监管在欧洲延后，在美中之间却在加速落地**。企业做跨境 inference 的部署成本，正在被这两条曲线合力推高。

**点评：** 今年剩下三个月，看哪些厂商先在"推理资产跨地域部署"做出干净的架构——跑赢对手的，不是模型质量，而是地理拓扑。

---

## 行业观察

- **"价格战 + 制程战"双循环**：GPT-6 Sol 的腰斩与 Nvidia A16 的押注不是两条独立新闻，而是同一个闭环——API 侧降价迫使底层算力继续优化，底层算力优化又让 API 可以继续降价。Anthropic 和 Google 要么在 Q4 跟进降价，要么用更高 tier 的产品差异化叙事避战。
- **监管节奏双速**：欧盟选择"推迟高风险落地 + 保留罚则"换取产业时间，美国选择"案例审查 + 关税"精细化管控。中国厂商的回应正从"替代"转向"算力拓扑再规划"，这对云厂与模型厂的全球部署架构提出新要求。
- **企业采纳悖论**：MIT 95% GenAI pilot 失败率与 Q1 $188B 投资形成了资金侧与落地侧的巨大断层。市场在 2026 Q4 开始看到采购部门从"追 benchmark"转向"追 unit economics 与可预测性"——这是今年剩余时间最值得追踪的买方拐点。
- **Anthropic IPO 窗口**：Opus 5 补齐产品矩阵、游说支出首次超越 OpenAI、产品侧和政治侧两线对齐，11 月前的 IPO 节奏正在抬头；若真发生，将是 2026 年 AI 一级市场最大的流动性事件。

---

> 数据与新闻引用自 DataNorth、Mezha、Threatcluster、TweakTown、JDSupra、CASRAI、theaireport.ai、tech-insider 及 benchlm.ai 等公开资料。
