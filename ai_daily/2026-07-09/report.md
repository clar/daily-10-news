# AI 每日新闻报告 · 2026-07-09

## 今日焦点

> **Fable 5 转付费 · 中国模型吞下美企 46% token · Gemini 3.5 Pro 再度跳票 · xAI×Cursor 联合模型 · EU AI Act 简化包落地**
>
> - **Fable 5 结束免费期**：即日起以 API 标准价 $10/$50 per M tokens 计费，是 Opus 4.8 的 2 倍，Pro 用户需买信用点。
> - **中国模型渗透美企**：CNBC 确认美国企业 AI token 用量中 30-46% 流向中国模型，GLM-5.2 以 SWE-bench Pro 62.1% + $1.40/$4.40 价格重击西方定价。
> - **Gemini 3.5 Pro 无期限延后**：Google 承认 token 效率与编码性能达不到企业测试预期，仍锁死在 Vertex AI 有限预览。
> - **xAI + Cursor 首个联合模型**：Musk 与 Anysphere（被 SpaceX 60 亿收购后）合作发布首款代码专用模型。
> - **EU AI Act 简化包终局**：欧洲议会 6/16 通过、理事会 6/29 终审，高风险 AI 义务推迟，透明度规则 8 月生效。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Anthropic Fable 5 结束免费期，转付费信用点模式 | Anthropic / ThursdAI | ⭐⭐⭐⭐⭐ |
| 2 | CNBC 报道美企 30-46% AI token 用量流向中国模型 | CNBC | ⭐⭐⭐⭐⭐ |
| 3 | Google Gemini 3.5 Pro 无期限延后，token 效率不达标 | Google / buildfastwithai | ⭐⭐⭐⭐ |
| 4 | GLM-5.2 SWE-bench Pro 62.1%，价格仅为西方 1/5 | Zhipu AI / BenchLM | ⭐⭐⭐⭐⭐ |
| 5 | xAI 与 Cursor 发布首款联合训练模型 | AIToolsRecap | ⭐⭐⭐⭐ |
| 6 | Together AI 完成 $800M C 轮，Aramco Ventures 领投 | Crunchbase | ⭐⭐⭐⭐ |
| 7 | EU AI Act 简化包通过，高风险条款延后 | European Council | ⭐⭐⭐⭐ |
| 8 | 联合国警告 AI"灾难性风险"，推动全球治理框架 | UN News | ⭐⭐⭐ |
| 9 | 伊利诺伊州州长 Pritzker 签署 AI 监管法案 | WTTW | ⭐⭐⭐ |
| 10 | Trump 突然取消 AI 行政令签署仪式 | buildfastwithai | ⭐⭐⭐ |
| 11 | OpenAI GPT-5.6 获商务部广泛发布许可 | Commerce / OpenAI | ⭐⭐⭐⭐ |
| 12 | 2026 H1 全球创投融资突破 $510B，AI 主导 | Crunchbase | ⭐⭐⭐⭐ |
| 13 | Anthropic 6 月营收首度超越 OpenAI | AIToolsRecap | ⭐⭐⭐⭐ |
| 14 | Google NanoBanana 2 Lite：4 秒生图 $0.034/千张 | Google | ⭐⭐⭐ |
| 15 | Peregrine Tech $250M D 轮，估值 $6.8B | Crunchbase | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Fable 5 免费期结束，Anthropic 拉高顶级模型价格锚

**[Anthropic Newsroom](https://www.anthropic.com/news) · [ThursdAI July 2026](https://thursdai.news/releases/2026-07)**

7 月 8 日起，Fable 5 不再包含在 Claude Pro 订阅中，而是通过信用点购买按 API 标准价 $10/M 输入、$50/M 输出计费——这个价格是 Opus 4.8（$5/$25）的整整两倍。同时期新默认模型 Sonnet 5 仍以 $2/$10 优惠价撑到 8 月 31 日，构成非常清晰的三层价格阶梯：Sonnet 5 抓走量、Opus 4.8 做主力生产、Fable 5 定位"顶级理性外挂"。

这次定价的意义远不止一次涨价。过去 18 个月里，Anthropic 一直用免费/低价方式让 Claude Pro 用户"上瘾"于顶级模型，但 6 月单月营收首次超越 OpenAI 之后，公司显然判断已经有足够的定价权把大用户往付费上引。信用点模式还有一个隐藏效果——把重度用户的账单从固定订阅切成变动成本，Anthropic 拿到了更好的单位经济学。

值得警惕的是，这个定价窗口恰好撞上 Google Gemini 3.5 Pro 跳票、OpenAI GPT-5.6 仍在 20 家政府协调伙伴的白名单内——顶层竞品供给受限，Anthropic 敢涨。一旦 Gemini 3.5 Pro 或 GPT-5.6 广泛发布，$50/M 输出这个锚点会不会松动，是下个季度最值得盯的变量。

**点评：** Anthropic 用"限时优惠 → 免费默认 → 强制付费"三段式跑通了 Claude 用户的商业化闭环；顶级模型价格战会不会在 Q3 打响，取决于 Google 能不能兑现 Gemini 3.5 Pro。

---

### 🚀 No.2 · CNBC：美企 46% AI token 已流向中国模型

**[buildfastwithai · July 8 Stories](https://www.buildfastwithai.com/blogs/ai-news-today-july-8-2026)**

CNBC 拿到的企业 API 网关抽样数据显示：美国企业内部消耗的 AI token 中，30-46% 已经流向中国厂商的模型——DeepSeek V4 Pro、GLM-5.2 和 Qwen3.7 Max 三家占大头。触发点是价格差：GLM-5.2 在 SWE-bench Pro 上跑到 62.1%（与前沿西方模型可比），而定价仅 $1.40/$4.40 per M tokens，是 Anthropic/OpenAI 的 1/5 到 1/10。

这个数字之所以震撼，在于它推翻了一个默认假设：即"美国企业出于合规和地缘政治顾虑不会用中国模型"。实际上，工程团队面对 5-10 倍的成本差异时，选择用中国开源模型跑非敏感 workload（代码生成、内容分类、文档摘要），把敏感 workload 留给 Claude/GPT。这种"分级路由"正在成为主流架构。

政策层面几乎必然反应：Trump 取消 AI 行政令签署仪式的原因目前未公开，但一种猜测是需要重新评估中国模型使用的国安含义。真正的问题是：如果限制企业调用中国模型 API，会不会反过来倒逼这些模型的开源权重版本被大规模私有部署——那只会让追踪更难。

**点评：** 中国开源模型的"性能追上 + 价格砸穿"组合拳，第一次把美国前沿实验室的定价权顶到了墙角；接下来是政策上的贸易措施 vs 市场上的架构选择的正面博弈。

---

### 💥 No.3 · Google Gemini 3.5 Pro 无期限延后：巨头也会跌跤

**[buildfastwithai · July 8](https://www.buildfastwithai.com/blogs/ai-news-today-july-8-2026) · [LLM-Stats](https://llm-stats.com/ai-news)**

Google 在 7 月 8 日的官方公告中承认，Gemini 3.5 Pro 从 6 月被推迟至今仍无确定发布日期，理由是"token 效率"以及"企业测试者反馈的编码性能差距"。这已经是三个月内第二次跳票，此前 Google 已经把 3.5 Pro 定位为对标 Opus 4.8 和 GPT-5.6 的旗舰。

延期本身不新鲜，但重要的是市场解读：在 Anthropic 涨价、OpenAI 政府门禁、xAI/Cursor 联合、中国模型渗透这四条战线同时开火的时刻，Google 缺席意味着 Q3 顶级模型市场事实上进入"三家半"格局——Anthropic、OpenAI、中国厂商完整供给，Google 只有 Gemini 2.5 Pro 和 NanoBanana 撑门面。企业客户如果在 Q3 做 vendor 选择，Google 天然出局。

值得一提的是 NanoBanana 2 Lite——Google 在图像生成端反倒卷价格：4 秒生图、$0.034/千张，同时质量超越初代。这透露出内部产品线的分化：语言旗舰陷入研发困境，多模态则用极端定价抢市场。

**点评：** Google 正在承受"Bard → Gemini"品牌重塑之后最尴尬的一次延期，如果 Q3 拿不出旗舰级 LLM，2026 年年终评分很难说服股东；NanoBanana 定价战是唯一亮点。

---

### ⚖️ No.4 · EU AI Act 简化包终审通过，高风险条款延后

**[European Council](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) · [Lexology](https://www.lexology.com/library/detail.aspx?g=25bf031c-432c-45ac-a363-614e1c315e07)**

6 月 29 日，欧盟理事会给 AI Act 简化包盖章，紧随欧洲议会 6 月 16 日的通过。核心动作有两个：一是**高风险 AI 系统的合规义务被 defer**（推迟），业界喘一口气；二是**透明度规则将于 2026 年 8 月生效**，标注 AI 生成内容、披露训练数据来源等条款要求所有落地欧盟市场的 foundation model 遵守。

这次简化不是"放松"，而是"分级"——欧盟承认自己没有能力在 2026 年内建立起对所有高风险 AI 系统的评估基础设施（该能力被官方规划到 2027 年运营），所以先把义务往后推，转而在透明度和事后审计上加压。这对 Anthropic、OpenAI 是好消息（合规成本推迟），对本地欧洲 AI 生态是坏消息（政策保护降低）。

同时值得注意：19 May 2026 发布的"高风险 AI 分类"公众咨询将于 7 月 23 日结束——这份分类目录一旦定稿，会直接决定哪些 API 用途需要额外备案，是 Q4 最需要跟踪的欧洲监管文件。

**点评：** 欧盟从"全面管制"转向"分级 + 透明度优先"，本质上是承认了自己在落地能力上的短板；短期利好美系巨头，长期看治理框架的中心正在从欧洲转移。

---

### 🚀 No.5 · Together AI 拿下 $800M C 轮，中东资本进场

**[Crunchbase Venture News](https://news.crunchbase.com/venture/global-startup-exits-ipo-ma-soar-ai-q2-h1-2026/)**

Together AI 完成 $800M C 轮融资，由 Aramco Ventures 领投——这是沙特阿美旗下资本第一次以主要角色进入美国前沿 AI 基础设施战局。Together AI 的定位是"开源模型的商业化托管平台"，客户主要是需要低成本推理 Llama、Qwen、DeepSeek 系列开源模型的企业。

这一笔的信号意义在两个方向：其一，中东主权财富基金进入 AI infra 的节奏加速——继此前 G42、MGX、Public Investment Fund 各自布局之后，Aramco Ventures 是"石油资本 → AI 资本"最直接的一次身份转换；其二，开源模型托管商正在被资本重估——市场判断顶层模型的差异化会缩小，而**跑推理的赢家**才是能吃下大部分企业 AI 支出的角色。

Q2 数据也印证了这个趋势：全球 H1 创投融资突破 $510B，超过 2025 全年，AI 拿走了大头；SpaceX 上市估值 $1.77T + 收购 Anysphere（Cursor 母公司）$60B 两笔就重塑了资本市场的 AI 加权。

**点评：** 中东资本正在系统性地把美国 AI infra 变成他们的"另类石油"资产；开源推理托管商是这一轮资金浪潮下一波最明显的受益者。

---

## 行业观察

**今日的核心矛盾是"顶层紧、底层松"**。顶层，前沿模型的价格锚被拉高（Fable 5 双倍于 Opus 4.8），且供给收窄（Gemini 3.5 Pro 跳票、GPT-5.6 白名单）；底层，中国开源模型以 1/5 到 1/10 的价格吞掉 46% 美企 token，把整个中低端市场砸穿。这种双向撕裂在中期会产生一个非常明确的战略选择：**要么加入顶层拿定价权，要么下沉到 infra 层做推理托管拿量**——夹在中间的中型 API 提供商最难受。

**监管拉力正在系统性转向"透明度优先"**。欧盟 AI Act 简化包把高风险条款延后、把透明度条款提前，本质是"事后可审计"取代"事前严禁"；美国这边 Trump 取消签署仪式虽然原因不明，但方向大概率是保持竞争力优先。伊利诺伊州法案是州级立法的又一次前哨，接下来要看的是加州 AB2013 后续修订版会不会跟进。

**中东资本 + 中国开源 = 2026 下半年最大变量**。前者提供无上限资金（Aramco $800M 只是开始），后者提供低成本供给（GLM-5.2、Qwen3.7 Max、DeepSeek V4 Pro）。当二者在 Q3 汇合到"用中东资金跑中国开源模型托管"的商业模式时，硅谷的护城河模型（融资 → 训练 → 卖 API）会第一次遇到结构性挑战。

---

**数据来源：**
- [Anthropic Newsroom](https://www.anthropic.com/news)
- [ThursdAI July 2026 Releases](https://thursdai.news/releases/2026-07)
- [buildfastwithai · AI News July 8 2026](https://www.buildfastwithai.com/blogs/ai-news-today-july-8-2026)
- [LLM-Stats · AI News](https://llm-stats.com/ai-news)
- [Crunchbase · H1 2026 Venture Data](https://news.crunchbase.com/venture/global-startup-exits-ipo-ma-soar-ai-q2-h1-2026/)
- [European Commission · AI Act](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)
- [AIToolsRecap · AI News July 2026](https://aitoolsrecap.com/Blog/AINewsJuly2026.aspx)
- [BenchLM · Chinese Models Ranking](https://benchlm.ai/best/chinese-models)
- [UN News · Global AI Governance](https://news.un.org/en/story/2026/07/1167862)
- [WTTW · Illinois AI Bill](https://news.wttw.com/2026/07/06/pritzker-signs-landmark-ai-regulation-bill-aims-mitigate-risks)
