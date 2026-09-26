# AI 每日资讯 · 2026-09-27

## 今日焦点

> **企业级 Agent 商业化爆发 · 中美 AI 治理正面碰撞 · 开源与推理端算力军备赛 · 政策与硬件双重升级**
>
> - **Cognition (Devin) 两年内冲上 10 亿美元 ARR**，估值 480 亿美元，GE Aerospace、Rivian、Exa 已进入付费名单，验证"编码 Agent"为首个可规模化的 Agent 商业形态
> - **DeepSeek 年化营收翻倍至 10 亿美元**，7 月毛利率达 82.9%，同时把 API 价格上调 2.3–4.5 倍，中国头部大模型首次证明"高毛利 + 提价"仍不影响需求
> - **Sanders–Casar《超级智能禁令》法案**在国会提出，要求永久禁止超越人类认知能力的 AI 系统，配套设立内阁级"AI 部"，违规者最高判 20 年
> - **NYC 出台美国首个针对前沿模型的市级监管草案**，OpenAI、Anthropic、Google、Meta、SpaceXAI 将于 10 月 5 日到场听证
> - **xAI Colossus 2 集群装机 11 万张 GB200 + 44 万张 GB300**，12 月底还将追加 66 万张 GB300，单点算力规模首次进入 100 万卡级

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Cognition (Devin) 突破 10 亿美元 ARR，估值 480 亿美元 | The Information | ⭐⭐⭐⭐⭐ |
| 2 | DeepSeek 年化营收翻倍至 10 亿，API 全面涨价，毛利率 82.9% | The Information | ⭐⭐⭐⭐⭐ |
| 3 | Sanders–Casar 提出《超级智能禁令》法案 | 美国国会 | ⭐⭐⭐⭐⭐ |
| 4 | NYC 前沿 AI 监管草案，10 月 5 日五大厂听证 | NYC Council | ⭐⭐⭐⭐ |
| 5 | Anthropic 上诉受挫：Claude 被 D.C. 巡回法院维持列入 DoD 供应链黑名单 | 联邦上诉法院 | ⭐⭐⭐⭐ |
| 6 | Microsoft Copilot 重构为 Home / Code / Autopilot 三件套，转向按用量计费 | Microsoft | ⭐⭐⭐⭐ |
| 7 | xAI Colossus 2 装机 55 万张 Blackwell，年底冲 100 万+ | SemiAnalysis | ⭐⭐⭐⭐ |
| 8 | 阿里 Qwen3.8-Omni-Flash 发布，1M 上下文原生全模态 | 阿里巴巴 | ⭐⭐⭐⭐ |
| 9 | 美团开源 LongCat-2.5-Preview：1.6T MoE，48B 激活，$0.75/$2.95 定价 | 美团 | ⭐⭐⭐ |
| 10 | OpenAI ChatGPT Voice 全面升级，支持插件与模型切换（Astra/Sol/Luna） | OpenAI | ⭐⭐⭐⭐ |
| 11 | Google Project Suncatcher：4 颗 TPU 将于 10 月 1 日搭载 SpaceX 入轨 | The New York Times | ⭐⭐⭐ |
| 12 | Alibaba Qwen-Audio 3.1：ASR 降价 95%、TTS 降 70% | 阿里巴巴 | ⭐⭐⭐ |
| 13 | Heidi 完成 3.4 亿美元融资，估值 9 亿美元 | Blackbird / General Catalyst | ⭐⭐⭐ |
| 14 | OpenEvidence 新一轮 2.5 亿美元融资，估值 150 亿美元 | OpenEvidence | ⭐⭐⭐ |
| 15 | Anthropic Claude 完成九圈 Yang-Mills 玻色化物理计算，成本 $1-2K | Anthropic | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Cognition (Devin) 冲上 10 亿美元 ARR，Agent 商业化拐点确立

**[The Information](https://www.theinformation.com/)**

Cognition 旗下 AI 编程 Agent Devin 在成立不足两年内跨过 10 亿美元 ARR 门槛，最新一轮融资对公司估值为 **480 亿美元**。目前付费客户已覆盖 GE Aerospace、Rivian、捷克电商 Rohlik、搜索引擎 Exa 等头部企业，Devin 被用于从"跑通任务"升级到"完成完整工程项目"——这是过去两年 Agent 赛道最强的商业化数据点。

从技术形态看，Devin 走的是"长上下文 + 工具调用 + 自主试错"的重型 Agent 路线，反而在企业侧率先跑通 PMF。对比同期 GitHub Copilot、Cursor 这类"辅助编码"产品的 ARR，Cognition 的收入结构显示：**企业更愿意为"能独立完成一个 Jira 卡片"的 Agent 支付订阅费**，而非按行补全。

真正的信号不在于 10 亿本身，而在于 480 亿估值背后的资本共识——市场已经承认，编码是首个能规模化外包给 Agent 的白领岗位。接下来 12 个月，Claude Code、Codex、Gemini CLI 的贴身战会更惨烈；对开发者工具的独立创业公司（Cursor、Windsurf 等）而言，如果不能拿出与 Devin 同级的自主性，就会被前沿实验室的自家 Agent 抢走高价值订单。

**点评：** 编码是所有白领岗位里最容易被 Agent 吃掉的第一块——从 480 亿估值倒推，市场已经把"AI 编码"当成 SaaS 之外的下一个平台级机会。

---

### 🚀 No.2 · DeepSeek 逆势涨价 API 2.3–4.5 倍，毛利率 82.9% 打破"中国模型没利润"神话

**[The Information](https://www.theinformation.com/)**

DeepSeek 年化营收在半年内从约 5 亿美元跳到 **10 亿美元**，同时把 API 价格调涨 2.3 至 4.5 倍，7 月毛利率高达 **82.9%**。这是中国头部大模型公司首次公开呈现"高毛利 + 主动提价 + 需求依然扩张"的组合。

过去 18 个月，中国大模型市场因价格战被认为陷入"零毛利+烧钱"陷阱。DeepSeek 的数据打破了这一叙事——V3、R1 系列在 Coding、Reasoning 上的公开评测持续压制同价位竞品，形成了"性价比 + 品牌"的正循环，从而具备提价能力。相比之下，Kimi、Doubao、Qwen 走的是"通过 To C 补贴 + 云捆绑"路线，DeepSeek 反而更接近 OpenAI 早期"API-first + 定价权"的商业模式。

值得关注的是，这份数据出现在 Trump-Xi AI 会谈之后——中方明显想向外界证明"即使不用 Nvidia B 系列，中国模型公司也能形成盈利闭环"。对海外用户来说，这意味着 Coding、翻译、Batch 推理类工作负载的中国模型使用比例会继续上升。

**点评：** 中国大模型价格战正式结束——真正跑出来的公司敢涨价，反而更多客户还回来。

---

### 🇺🇸 No.3 · Sanders–Casar《超级智能禁令》法案：AI 政策进入"红线立法"时代

**[美国国会](https://www.congress.gov/)**

参议员 Bernie Sanders 与众议员 Greg Casar 联合提出《Superintelligence Prohibition Act》，核心条款包括：**永久禁止**任何在综合认知能力上超越人类的 AI 系统；暂停"前沿模型"训练；设立内阁级 AI 部；违规企业可被解散或高管最高判 **20 年监禁**。

这是继"AI 训练暂停信"之后，第一份把"超级智能禁令"写入正式立法草案的美国联邦级动作。虽然该法案通过概率极低（共和党占多数、Trump 政府整体倾向 light-touch），但它的政治信号极强——AI 治理已从"抽象风险"进入"具体法条"阶段，且左翼开始正面动员。

与此同时，纽约市自己的前沿模型监管草案要求外部评估、人类硬性 kill switch、24 小时事故报告，并允许因绕过安全措施受害者提起私人诉讼。**10 月 5 日 OpenAI、Anthropic、Google、Meta、SpaceXAI 五家将到场听证**，是 xAI 首次以"SpaceXAI"品牌出现在美国监管场景。

**点评：** 从加州 SB-1047 到纽约草案再到 Sanders 议案，美国 AI 立法正在从"州级试点"扩展成"联邦级红线尝试"——法律赶不上模型，但正在赶。

---

### 🏭 No.4 · Microsoft Copilot 重构为 Home + Code + Autopilot：企业市场按用量计费

**[Microsoft](https://www.microsoft.com/)**

Satya Nadella 亲自宣布，Copilot 将拆分为三个 SKU：**Home**（面向员工的工作中枢）、**Code**（低代码应用构建）、**Autopilot**（长驻企业 Agent）。同时废弃 M365 Copilot 时代的 $30/seat/月固定套餐，转向按调用量计费 + FinOps 控制面板。

这个转向对整个 SaaS 行业冲击极大——Salesforce、Workday、ServiceNow 之前均效仿 M365 采用固定席位价，但如果 Autopilot 一个订阅可以替代 3-4 个业务系统的席位，"按人头卖"模型会被系统性瓦解。Nadella 直言，Copilot 目标市场"比整个云还要大几个量级"，明显把 Azure + Copilot 组合定位成新一代平台。

结合前两天 Cognition Devin 10 亿 ARR、Warp $85M HR Agent 融资、Heidi 医疗 scribe 3.4 亿融资，**"垂直 Agent + 按结果计费"正在成为新的 SaaS 商业标准**。

**点评：** SaaS 20 年不变的"按 seat 定价"模型正在被 Agent 拆穿——不是每人一份订阅，而是每个 outcome 一次计费。

---

### 🖥️ No.5 · xAI Colossus 2：单集群冲向百万卡，中美算力鸿沟继续扩大

**[SemiAnalysis](https://www.semianalysis.com/)**

SemiAnalysis 披露 xAI Colossus 2 数据中心已装机 **11 万张 GB200 + 44 万张 GB300**，12 月底目标追加 **66 万张 GB300**，若按期到位，Colossus 2 将成为全球首个 **100 万卡量级的单一 AI 训练集群**。

同期，SemiAnalysis 对中国数据中心的调研指出：中国已建成 1000+ 大型数据中心，交付容量 24 GW，其中字节跳动一家占约 20%；单个 100MW 站点最快 12 个月内交付。**但由于制裁与 HBM 短缺，中国"能力密度"（FLOPs/W）显著落后美国**——同样的 24 GW，若装满 GB300 相当于 3-4 个 Colossus 2，中方目前主要以国产芯片 + H20 组合填充。

xAI 侧同时更新 Grok 5 的训练时间轴：预计年底完成，Colossus 2 是其独占算力。Musk 在推文中放话"Grok 5 将是首个显著体感更聪明的模型"，坐实其对标 GPT-6 Sol 与 Claude Opus 5.5 的野心。

**点评：** 大模型进入"电力工程"阶段——谁能在 12 个月内合法接入 100 万卡，谁就直接跳过下一个模型代际。

---

## 行业观察

今天的信号非常一致：**Agent 已经跨过"技术能不能"的争论，进入"商业能不能规模化"的临床期**。Cognition 10 亿 ARR + Microsoft Copilot 按用量重构 + Warp / Heidi / Ando 一系列垂直融资，都在说明企业级 Agent 已经具备现金流，SaaS 定价模型正在被系统性重写。

竞争格局层面：**OpenAI 与 Anthropic 用旗舰模型（GPT-6 Sol / Claude Opus 5.5）拉高上限，中国厂商用价格与开源拉低下限**——DeepSeek 敢涨价、阿里 Qwen-Omni-Flash 原生 1M 上下文、美团 LongCat 2.5 开源 1.6T MoE，从三个维度分层竞争。开源正在成为中国队的默认战术。

政策线索也开始收紧：Sanders 的超级智能禁令、NYC 前沿模型监管草案、D.C. 巡回法院维持 Anthropic-Pentagon 供应链黑名单、Trump-Xi 高层对 AI 治理表态，说明 **AI 已经进入政治议题主线**。对企业侧影响是：明年开始，"合规准入 + 安全评估 + 事件披露"将变成前沿实验室的固定 CAPEX，一定程度上抬高进入门槛，反过来强化头部效应。

硬件层面依然是 Nvidia 的独角戏：xAI 55 万卡、Google Project Suncatcher 试验太空 TPU、Anthropic 在 Yang-Mills 物理问题上跑通 $1-2K 成本的"科学 Agent"——三条路线看似不同，其实指向同一命题：**当算力足够便宜且 Agent 具备完成完整工作流的能力时，"用算力换人力"会从口号变成资产负债表上的一行数字**。

**关注明日**：OpenAI DevDay 前瞻（预计 10 月）、纽约 10 月 5 日五大厂听证细节、Grok 5 训练是否按期完成、Nvidia GB300 出口白名单最新细则。
