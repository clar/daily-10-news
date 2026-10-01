# AI 每日资讯 · 2026-10-02

## 今日焦点

> **算力结盟持续加码 · 代理 AI 融资洪流 · 基准评测商业化 · 欧盟高风险合规落地 · 开闭源竞争重新定义**
>
> - **AMD×OpenAI 6GW 大单继续发酵**：MI450 首批 1GW 预计 2026H2 投产，AMD 向 OpenAI 发行 1.6 亿股认股权证，成为算力史上最大非英伟达绑定协议之一
> - **代理 AI（Agentic AI）融资过去 5 个月已累计 11 亿美元**，几乎翻倍去年同期，Vertical Agents 占比 48% 以上
> - **Vals AI 完成 4000 万美元 A 轮**，a16z 领投，4 亿美元估值，专注独立模型评测——AI 评测正成为千万美元级生意
> - **欧盟 AI Act 高风险条款自 8 月正式适用后进入执法攻坚期**，招聘、信贷、医疗诊断类 AI 系统面临首批合规审计
> - **Oracle 披露与 OpenAI 签订 3000 亿美元五年算力大单**，成为云计算史上最大合同之一；Microsoft Copilot ARR 跨越 370 亿美元

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | AMD 与 OpenAI 6GW 深度绑定，1.6 亿股认股权证分期归属 | ElectronicSpecifier / NextGov | ⭐⭐⭐⭐⭐ |
| 2 | OpenAI 与 Oracle 签订 3000 亿美元五年云算力合同 | Nasdaq / Barchart | ⭐⭐⭐⭐⭐ |
| 3 | 欧盟 AI Act 高风险条款正式适用，首轮合规审计启动 | EU Commission | ⭐⭐⭐⭐ |
| 4 | 代理 AI 融资 5 个月累计 11 亿美元，纵向代理占比过半 | Qubit Capital | ⭐⭐⭐⭐ |
| 5 | Vals AI 完成 4000 万美元 A 轮，a16z 领投独立评测 | CryptoBriefing | ⭐⭐⭐⭐ |
| 6 | LM Arena 1 亿美元种子轮 6 亿美元估值，评测基础设施崛起 | Forbes AI | ⭐⭐⭐ |
| 7 | Microsoft 365 Copilot 付费席位破 2000 万，AI 业务 ARR 370 亿美元 | Microsoft Q3 FY26 | ⭐⭐⭐⭐ |
| 8 | GPT-6 Astra 定位"计算机使用型代理"，首次触及 OpenAI 关键网络安全风险等级 | OpenAI Blog | ⭐⭐⭐⭐ |
| 9 | Anthropic Claude Fable 5.1 / Mythos 5.1 缓存读取价格再降 75% | Anthropic | ⭐⭐⭐⭐ |
| 10 | AWS Bedrock 客户支出环比增长 170%，Amazon Q1'26 云业务同比 +28% | Amazon Q1 FY26 | ⭐⭐⭐ |
| 11 | Forbes AI 50 累计融资 3056 亿美元，OpenAI+Anthropic 占 80% | Forbes | ⭐⭐⭐ |
| 12 | Gemini 3.1 Pro Preview 保持 1M token 输入，SWE-bench 76.2% | Google DeepMind | ⭐⭐⭐ |
| 13 | Meta Llama 5（600B 开源）继续以"递归自改进"叙事扩大场内影响 | Meta | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · AMD×OpenAI 6GW 大单继续发酵——英伟达垄断被撬开一道缝

**[AMD and OpenAI announce strategic partnership to deploy 6 gigawatts of AMD GPUs](https://www.electronicspecifier.com/?p=164905)**

AMD 与 OpenAI 的 6 吉瓦合作协议，是过去两年算力史上最具结构性意义的一笔交易，而非一次普通的硬件采购。核心条款是：首批 1 GW 的 AMD Instinct MI450 将于 2026 下半年部署，而 AMD 向 OpenAI 发行高达 1.6 亿股普通股认股权证，按部署里程碑分期归属——这把"大客户"直接变成了"大股东"。

过去 36 个月里，所有讨论"英伟达垄断的裂缝"的分析，最后都归结到一句话："OpenAI 自己想不想裂"。这笔交易给出的答案是明确的"想"。6GW 的量级相当于当前 OpenAI 已部署算力的数倍，意味着从 2027 开始，AMD 可能承载 OpenAI 相当比例的推理与新模型训练负载。考虑到 OpenAI 过去同时与微软 Azure、Oracle（最新 3000 亿美元合同）、Google Cloud、CoreWeave 等签订了并行协议——它在明确地走"多云 + 多芯片"的采购战略。

对 AMD 而言，这是从"陪跑玩家"升格到"同台玩家"的分水岭。AMD 数据中心业务 Q3 收入已达 43 亿美元，MI350 已经验证量产能力；MI450 若能在 OpenAI 工作负载上跑通，则 TAM 面彻底打开。对英伟达而言，CUDA 护城河并没有一夜消失，但"假设每一片 AI 加速器都来自英伟达"的默认叙事正式瓦解。

**点评：** 这不是价格战，这是股权绑定的供应链政治。英伟达要应对的，不是 AMD 的 FLOPS，而是客户主动把算力多元化写进 KPI。

---

### 🚀 No.2 · OpenAI 的"算力三件套"收齐：Oracle 3000 亿、AMD 6GW、Microsoft 优先

**[Oracle Expands AI Database Offerings Through AWS Cloud](https://www.nasdaq.com/articles/oracle-expands-ai-database-offerings-through-aws-cloud-whats-ahead)**

把三份合同并列放在一起看，OpenAI 的算力版图第一次有了完整形状：Microsoft 作为"深度技术合伙人 + 优先供应商"，Oracle 承担 3000 亿美元级别的新建算力资源池，AMD 承担 6GW 的加速器基础供给。这意味着 OpenAI 已经不再是"微软独家依赖"的创业公司，而是在以主权国家级采购体量运作的基础设施买家。

Oracle 一个季度就拿下了 OpenAI、Meta、NVIDIA、AMD 四个超大客户的订单，Larry Ellison 过去 30 年都没拿过这么漂亮的季度；Microsoft Copilot 付费席位过 2000 万、AI 业务 ARR 过 370 亿美元，Accenture 一家就承诺 74 万席位。AI 基础设施的收入兑现曲线，终于开始"看得见摸得着"。

但也要清醒：这些合同大部分是 2026-2030 跨期承诺，兑现要靠电力、变电站、冷却和芯片同步到位。能源瓶颈正在从"配套问题"升格为"主控变量"。

**点评：** 2026 的 AI 竞赛已经从"谁的模型更好"变成"谁能先把千兆瓦插进电网"——这将是 2027 真正的战役。

---

### 🔬 No.3 · 评测基础设施首次迎来"独角兽级"投融资

**[Vals AI Raises $40M Series A Led by a16z](https://cryptobriefing.com/vals-ai-40m-series-a-a16z/)**

Vals AI 以 4 亿美元估值融资 4000 万美元，a16z 领投；几乎同时，LM Arena 以 6 亿美元估值完成 1 亿美元种子轮。这两个数字放在一起只传达一件事：**模型评测正在从公共产品，变成一门严肃的商业生意**。

Vals 的核心产品不再是"做榜单"，而是：Vals Smith（自定义代码基准）、RSI Index（衡量递归自改进能力）、ReverseEngBench（逆向工程基准）、Vals Index 2.0（按 GDP 行业贡献加权）。它们都是企业客户下单的"信息服务"，面向金融、法律、医疗、咨询等专业场景。

这与过去三年的 MMLU/GPQA/SWE-bench 等公共基准形成了鲜明对比。公共基准被模型厂商"打榜竞赛"迅速饱和，很快失去区分力；独立评测则绑定具体业务场景，天然难以作弊、天然能收费。可以预见未来 12 个月内，Scale AI、Surge、Scale Rogue 等公司都会在"企业级评测"赛道加码。

**点评：** 当模型差异收敛，评测本身就是最值钱的差异化服务。a16z 这一笔是押"后训练时代"的核心基础设施。

---

### 🤖 No.4 · 代理 AI 融资过去 5 个月累积 11 亿美元，纵向代理成主流

**[AI Startup Funding: A Complete Roundup for 2026](https://blog.herond.org/ai-startup-funding/)**

2026 前五个月，代理 AI 累计融资 11 亿美元、29 笔交易，是去年同期（5.38 亿美元、9 笔）两倍的资金与三倍的交易量。更关键的是结构：Vertical Agents（纵向代理，聚焦于某一行业例如网络安全、医疗运营、合规）占了 48.3% 的交易量与 54.6% 的资金。

这说明市场情绪已经从"通用型大代理（横向平台）"转向"行业专精代理（纵向嵌入）"。原因无他——通用代理与底层模型高度同构，容易被 OpenAI/Anthropic/Google 一次"原生代理化升级"抢走商业空间（GPT-6 Astra 就是这类"原生代理")；而纵向代理挤占的是具体的业务流程/工单/合规审计，底层模型厂商短期内无法切入。

与此同时，7 月单月代理 AI 融资达 18 亿美元跨 12+ 笔交易，节奏明显加快。

**点评：** 2026 是"代理商业化落地"的分水岭年；"做个 chatbot 挂 API"的项目基本募不到钱，"做工单自动化 / 医疗预授权 / 合规审计"才有估值。

---

### 📜 No.5 · 欧盟 AI Act 高风险条款正式适用——合规时代真正来临

**[The AI Regulation Landscape for 2026](https://cimplifi.com/resources/the-ai-regulation-landscape-for-2026-what-legal-and-compliance-leaders-need-to-know)**

欧盟 AI Act 的"高风险场景"条款自 2026 年 8 月 2 日起正式适用，涉及招聘筛选、信用评估、计算机辅助医疗诊断等直接影响个人利益的场景。进入 10 月，欧盟 AI Board 已经开始对数家头部 HR Tech、FinTech、HealthTech 开展首轮合规审计。

这意味着什么？第一，**模型卡（Model Card）、风险管理档案、人工监督机制、数据治理文档**从"nice to have"变成"必须要有"，一旦缺失，罚款上限可达全球年营业额的 7%。第二，服务于欧洲的美国与中国 AI 厂商必须"自带合规"——这催生了一个全新的"AI 合规 SaaS"赛道。第三，中小企业在"高风险"分类下的生存门槛明显提高，可能加速行业集中度。

中国方面，7 月生效的"AI 拟人化临时办法"也在同步推进；美国则仍是州法+行政令的碎片化状态。三条监管路径的分叉，将成为未来 24 个月跨国 AI 公司战略规划的核心变量。

**点评：** 2025 大家还在喊"自愿安全框架"，2026 已经进入"全球年营业额 7% 罚款威胁"阶段——合规能力从加分项变必修课。

---

## 行业观察

**算力正在成为 AI 行业的"货币"**：从 Oracle 的 3000 亿、AMD 的 6GW、Microsoft Copilot 的 370 亿 ARR 到各家数据中心的电力瓶颈——过去 24 个月的所有重要新闻几乎都在诉说一件事：模型质量差距在收敛，而算力获取、能源获取、芯片多元化正成为新的护城河指标。英伟达的垄断首次出现结构性松动，不是因为技术，而是因为客户不愿意把身家押在单一供应商。

**模型层正在"同质化"，应用层正在"垂直化"**：GPT-6 Astra、Claude Fable 5.1、Gemini 3.1、Llama 5 之间的差距再也不是"谁更聪明"，而是"谁更擅长什么"；企业客户越来越不关心"用哪家模型"，而是关心"这条业务流程 end-to-end 能跑通吗"。这解释了为什么纵向代理的融资占比过半——投资人也在重新定价。

**独立评测与合规正在变成千万美元级生意**：当"用哪个模型"难以靠公开榜单回答时，Vals AI、LM Arena 这类独立评测机构的议价权陡增；当"用了模型会不会被罚"成为董事会议题时，AI 合规 SaaS 的 TAM 也被打开。这些此前被视为"公共产品"或"法律边角"的角色，正在被重新资本化。

**展望下周：**
- OpenAI DevDay（10 月中）会否公布 GPT-6 Astra 的企业版细节与定价
- Anthropic 是否会跟进"企业级代理"产品线，并给出 Claude Fable 的 Agent SDK
- 欧盟 AI Board 首轮合规审计的具体对象与结果——这将定义未来一年的合规基线
- Nvidia 对 AMD 结盟的回应，是否会祭出新一轮大客户锁定协议
