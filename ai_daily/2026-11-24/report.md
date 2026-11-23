# AI 日报 · 2026-11-24

> 截至北京时间 11 月 24 日 05:00（11 月 23 日 21:00 UTC）。以下以窗口内公开发布的消息为准；协议签署不等于交割，研究评测不等于生产验证。

## 今日焦点

> **推理芯片的软件竞争 · 循环架构 · 搜索个人数据授权 · 医疗模型开放权重**
>
> - **英伟达公开宣布黄仁勋复任。** SEC 文件显示董事会在 11 月 22 日已作决定，11 月 23 日对外公布。
> - **亚马逊官宣与 Decart 签约。** 明确购买应用于芯片和推理优化的技术、吸纳团队；不是官宣收购整家公司，也未披露价格。
> - **智谱发布 GLM-5.4。** 共享的 28 层执行两轮，增加推理深度而不增加这一组层的参数；厂商也承认它有时会想得太久。
> - **Google 搜索 AI Mode 开始接入 Wallet。** 用户主动授权、仅可读取；Drive 和 Gemini 应用安排在未来几周接入。
> - **蚂蚁开放两款医疗模型权重。** 独立团队可以自行评测，但公开权重或榜单成绩不构成临床验证。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | **英伟达确认黄仁勋复任**：重新担任总裁、CEO 与董事；临时 CEO Colette Kress 继续担任 CFO。董事会在 22 日作出决定，23 日对外公布。 | [英伟达公告](https://investor.nvidia.com/news/press-release-details/2026/NVIDIA-Board-Reinstates-Jensen-Huang-as-President-CEO-and-Board-Director/default.aspx)、[SEC 8-K](https://www.sec.gov/Archives/edgar/data/1045810/000104581026000090/nvda-20261122.htm) | ⭐⭐⭐⭐⭐ |
| 2 | **亚马逊签约购买 Decart 优化技术并吸纳团队**：涉及 Decart Optimization Stack，仍待满足交割条件，包括监管许可；官方未披露价格。 | [亚马逊公告](https://www.aboutamazon.com/news/company-news/amazon-decart-ai-optimization)、[路透](https://www.investing.com/news/stock-market-news/amazon-to-buy-decarts-ai-chip-optimization-tech-in-latest-ai-talent-grab-5046000) | ⭐⭐⭐⭐ |
| 3 | **智谱发布 GLM-5.4**：首款采用循环 Transformer 的智谱旗舰，重复执行同一组 28 层两次，面向编程及长流程任务；公司指出有过长推理的情况。 | [智谱技术博客](https://z.ai/blog/glm-5.4) | ⭐⭐⭐⭐ |
| 4 | **Google 搜索开始推出 Wallet 个性化连接**：用户主动启用后可查询消费等信息，AI Mode 不能转账、管理或投资资金；Drive 和 Gemini 应用尚在后续推出计划。 | [Google 搜索公告](https://blog.google/products-and-platforms/products/search/google-search-personal-intelligence-apps/) | ⭐⭐⭐⭐ |
| 5 | **蚂蚁阿福开放 LingSante 首批两个医疗健康模型权重**：air-VL 面向多模态理解，flash 面向复杂医学推理；其余权重计划分批开放。 | [蚂蚁集团](https://www.antgroup.com/en/news-media/press-releases/1795402800000)、[flash 模型卡](https://huggingface.co/inclusionAI/LingSante-3.1-flash) | ⭐⭐⭐⭐ |
| 6 | **印度 L&T 拿下金奈 AI 集群多年期订单**：旗下 LTN Compute 将增配英伟达 B300，属于规划中的 1 万块 GPU 集群的一部分；公告并未说本单单独采购 1 万块。 | [L&T 交易所公告](https://nse-bse-announcements.s3.ap-south-1.amazonaws.com/lt/PAM_23112026093338_PressRelease23112026.pdf) | ⭐⭐⭐ |
| 7 | **MIT 披露小模型模拟电路设计研究 SLIC**：小模型借助仿真反馈迭代，在团队测试中接近 GPT-6 Astra；尚不能据此推定量产良率或成本。 | [MIT News](https://news.mit.edu/index.php/2026/ai-driven-technique-could-help-engineers-design-analog-chips-faster-and-less-expensive-1123) | ⭐⭐⭐ |
| 8 | **Appian 发布英国大型企业 AI 开发调查**：200 位受访者中，64% 表示初期开发更快、但测试、集成等后续环节耗时增加；为厂商发布的调查，不等同于全行业净生产率下降。 | [Appian 投资者关系](https://investors.appian.com/node/14611/pdf) | ⭐⭐⭐ |
| 9 | **L&T Technology Services 推出软件定义汽车工具链 SDVault.ai**：面向整车厂和一级供应商的开发、集成与验证，发布不等于已有独立验证的安全收益。 | [LTTS 交易所公告](https://nsearchives.nseindia.com/corporate/LTTS_23112026085541_23112026LTTSPRessreleasesd.pdf) | ⭐⭐⭐ |
| 10 | **Levenza 发布面向企业的个人智能体**：公司宣布全球推出，竞争重点在企业部署；公告不能证明客户实际采用规模或生产效果。 | [Levenza 新闻稿](https://www.globenewswire.com/news-release/2026/11/23/3408386/0/en/levenza-launches-personal-ai-agents-globally-for-the-enterprise.html) | ⭐⭐⭐ |
| 11 | **文远知行披露 WRD 3.0 南昌站辅助驾驶赛结果**：公司称搭载该系统的 AION i60 为该站唯一零接管参赛车辆；公告为北京时间 23 日 06:30，比赛结果不等于道路安全认证。 | [文远知行投资者关系](https://ir.weride.ai/node/9506/pdf) | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · 亚马逊买的是让 AI 芯片更好用的软件

**[亚马逊公告](https://www.aboutamazon.com/news/company-news/amazon-decart-ai-optimization)**

继周末的谈判报道后，亚马逊 23 日首次明确已签协议，购买 Decart 优化软件背后的专有技术，并吸纳三位联合创始人及研究、工程团队。交易尚待监管许可等交割条件，亚马逊没有公布定价。

算力竞争不只是卖多少芯片。客户如果需要重新处理算子、工具链和部署，换到一款便宜的芯片也未必能降低成本。优化软件有机会把迁移工作变成可重复的流程，让 Trainium 的纸面性能更容易变成客户可测的结果。

接下来应比较同一模型、相同服务质量下的端到端延迟、吞吐和工程投入，而不是只比较芯片租价或单项内核成绩。

**点评：** 自研芯片能不能抢到外部客户，要看它能否接住客户已有的模型，而不仅是跑自家的演示。

---

### 🚀 No.2 · GLM-5.4 用更多计算换更深推理

**[智谱技术博客](https://z.ai/blog/glm-5.4)**

GLM-5.4 对同一组 28 层执行两轮，权重共享。增加的是执行深度，不是这组层的参数。智谱同时指出，新模型有时会在推理中花过长时间。

这意味着循环模型可以减少对单纯堆参数的依赖，却不意味着省下的参数会等比例变成更快或更便宜的服务。对于长编程任务，关键是做对同一件事需要多少时间、计算和人工介入。

接下来值得关注外部团队在统一推理预算下的对比，尤其是任务完成时间的长尾、失败后的重试，以及复杂任务的总成本。

**点评：** 参数量变小不等于使用成本变低。拿同一批真实任务对照任务成功率与总耗时，才看得出架构优势。

---

### 🔎 No.3 · 搜索接入 Wallet，扩大的是数据边界

**[Google 搜索公告](https://blog.google/products-and-platforms/products/search/google-search-personal-intelligence-apps/)**

Google 搜索的 AI Mode 开始推出 Wallet 连接。用户必须主动启用；即使启用，Wallet 也是只读，搜索无法转账或投资。Drive 与 Gemini 应用是未来几周的计划，不能算作已经同时上线。

好处是无需再手动整理一堆消费或文档信息；代价是原本分散在不同应用的数据，可能被带入同一次搜索回答。只读避免了模型直接动账，但不能代替对调用范围和数据来源的解释。

接下来要看回答能否明确标注实际使用了哪个连接、撤销授权后如何处理历史上下文、用户能否只在指定的查询中调用连接。

**点评：** 比“能连多少应用”更重要的是，用户能不能看见它这一次到底用了什么。

---

### 🩺 No.4 · 医疗模型开放，让外界可以验证，而不是自动获得信任

**[蚂蚁集团公告](https://www.antgroup.com/en/news-media/press-releases/1795402800000)**

LingSante 首批公开的是 air-VL 和 flash，分别覆盖多模态理解与复杂医学推理。开放权重给研究者提供了独立测试的入口；公告中的排名则来自同时推出的评测平台，不等于独立临床试验。

重要的不是模型答对了多少道题，而是在哪些情况应当表达不确定、什么时候转给医生，以及换地区、医院和文档标准后是否仍可靠。

值得跟踪的是第三方能否在不同数据与流程上复现结果，以及是否公开评估错误分类和人类复核的作用。

**点评：** 开放权重降低了质疑和验证的门槛，不会降低临床证据的门槛。

## 行业观察

今天三条主线都指向同一个问题：模型或系统到底改善了哪一步。芯片优化要证明降低了迁移成本，循环模型要证明提高了任务完成效率，个人数据连接和医疗模型则要证明结果可追溯、能被复核。采购和采用的判断标准，正在从功能清单转向可核查的实际结果。
