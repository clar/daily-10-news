# AI 日报 · 2026-11-23

> 截至北京时间 11 月 23 日 05:00，主要覆盖过去 24 小时。较早发生而本窗口内披露的事项标为「新披露」，窗口外资料标为「背景」。

## 今日焦点

> **推理数据留存 · 韩国考试规则 · AI 芯片迁移 · 物理 AI**
>
> - **OpenRouter 撤销 125 个端点的零数据保留资格。** 这不是 125 起已确认的泄露。平台同时移除了三家未具名的推理供应商。
> - **Novita 披露部分请求被转发至 MiniMax。** 模型名不变，实际处理请求的一方仍可能变化。
> - **韩国教育部长在考试争议后辞职。** 携带不合规设备和已确认利用 AI 作弊是不同口径。
> - **从仿真到实际产线。** 上海 GAMES 研讨会收官，废料分选展示提供了一个可具体检验的场景。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | **OpenRouter 调整供应商与零保留资格**：11 月 22 日公告：移除三家推理供应商，取消 125 个端点的零数据保留资格，其中包含预防性移除；平台称相关发现未显示 OpenRouter 自身被入侵。 | [OpenRouter 公告](https://openrouter.ai/blog/announcements/data-processing-incidents-on-inference-providers/) | ⭐⭐⭐⭐⭐ |
| 2 | **Novita 披露 MiniMax 请求被转发**：11 月 22 日公告：路由配置问题使部分请求发往 MiniMax 官方 API，而非 Novita 自有基础设施。是否曾被第三方留存仍有待核实。 | [Novita 隐私公告](https://novita.ai/blog/minimax-requests-privacy-notice/) | ⭐⭐⭐⭐ |
| 3 | **韩国教育部长在考试争议后辞职**：11 月 22 日，韩国总统接受教育部长崔教镇辞呈。争议涉及为防范 AI 辅助作弊而在全国高考前临时调整的规则；不能据此认定所有违规者均使用了 AI。 | [韩联社](https://www.yna.co.kr/view/AKR20261122024000001)、[韩国国务总理室此前公告](https://www.opm.go.kr/opm/news/press-release.do?articleNo=164260&attachNo=157973&mode=download) | ⭐⭐⭐⭐ |
| 4 | **DeepSeek Harness 推出 0.2.3 预发布版本**：11 月 22 日可见 alpha.2。它是智能体工具链的预发布，不是 DeepSeek 新模型，也不等于稳定版。 | [DeepSeek GitHub](https://github.com/deepseek-ai/deepseek-harness/releases/tag/dsh-v0.2.3-alpha.2)、[发行镜像时间](https://sourceforge.net/projects/deepseek-harness.mirror/files/) | ⭐⭐⭐ |
| 5 | **上海 GAMES 研讨会进入收官日**：11 月 22 日是主办方公布的最后一天；议程聚焦世界模型、物理仿真、空间智能和具身智能。计划编制的白皮书不应写成已发布。 | [GAMES 主办方](https://games-cn.org/games2026/) | ⭐⭐⭐ |
| 6 | **DataBeyond 披露废料分选展示**：新披露：公司 11 月 22 日发布消息，回顾 19 日在 COP31 中国角展示将高光谱识别与机器人拾取结合的分选方案；未披露可横向比较的产线回收率。 | [DataBeyond 新闻稿](https://www.prnewswire.com/news-releases/databeyond-showcases-ai-sorting-solutions-for-circular-supply-chains-at-cop31-302947646.html) | ⭐⭐⭐ |
| 7 | **Baez 拆解 Masullo 的独立证明草稿**：11 月 22 日，数学家 John Baez 梳理其论证路线及已有质疑，并说明自己的判断是暂定的。评议针对 Masullo 的人工撰写稿，不是前一期报道的 Alpöge／Claude 形式化证明。 | [Baez 原文](https://johncarlosbaez.wordpress.com/2026/11/22/masullo-on-the-riemann-hypothesis/) | ⭐⭐⭐ |
| 8 | **Kilat 发布轻量模型训练框架与样例**：11 月 22 日，开发者在 Hugging Face 社区公布支持预训练和微调的实验框架，附 150M 参数样例；不是经独立评测验证的性能突破。 | [开发者发布帖](https://discuss.huggingface.co/t/introducing-kilat-an-open-source-framework-for-building-and-training-lightweight-language-models/192365) | ⭐⭐⭐ |
| 9 | **媒体称亚马逊与 Decart 收购谈判进入后期**：背景（11 月 21 日媒体报道，刊出时刻未核实）：有知情人士称双方进入后期谈判，报道不等于签约。已有合作可查：Decart 曾公布与 AWS 的商业合作。 | [《金融时报》独家报道](https://www.ft.com/content/dc7749dc-0f40-44a6-80bc-7f747d383616)、[新闻摘要与合作时间线](https://www.generalpurpose.com/briefing/2026-11-22) | ⭐⭐⭐⭐ |
| 10 | **国家数据局提出完善词元计量计费标准**：背景：11 月 20 日在世界计算大会提出，并于 21 日发布官方稿。表述是完善计量计费、质量测评标准的方向，不是已实施的统一标准。 | [国家数据局](https://www.nda.gov.cn/sjj/ywpd/sjzg/1121/20261121163827783032901_mobile.html) | ⭐⭐⭐ |

---

## 深度点评

### No.1 · “零保留”要查到实际处理请求的那一层

**[OpenRouter 公告](https://openrouter.ai/blog/announcements/data-processing-incidents-on-inference-providers/) · [Novita 公告](https://novita.ai/blog/minimax-requests-privacy-notice/)**

OpenRouter 的清理行动与 Novita 的公告不是同一件事：前者是路由平台撤销资格的决定，后者是一个供应商对请求处理路径的说明。**不要把公告提及的公司名单等同于被移除的三家公司，也不要把端点数量等同于泄露规模。** 对企业采购更有用的三个问题：谁实际处理请求、故障时是否允许换供应商、处理路径改变后是否能在日志里查到。只看模型名和一个隐私标签不够。

### No.2 · 考场治理需要区分设备、使用与证据

**[韩联社](https://www.yna.co.kr/view/AKR20261122024000001)**

韩国案例最值得看的是规则执行：携带违规设备、在考试中实际使用设备、确认利用 AI 作弊，三者不是同一口径。识别能力只是其中一环；一致的告知、记录、复核和申诉流程决定了技术措施能不能被公正地执行，也比事后用一个总数概括作弊规模更重要。

### No.3 · AI 算力不只卖芯片，也卖跨芯片迁移能力

**[金融时报报道](https://www.ft.com/content/dc7749dc-0f40-44a6-80bc-7f747d383616) · [国家数据局](https://www.nda.gov.cn/sjj/ywpd/sjzg/1121/20261121163827783032901_mobile.html)**

若亚马逊最终拿下 Decart，值得关注的是客户能否以更低的迁移成本把实时视频等工作负载移到 Trainium，而不是传闻中的估值。现阶段可以确认的是既有合作，不是并购完成。评估替代芯片时，比较同一工作负载的总成本、延迟和工程投入，比只看每卡租价更有意义。这也解释了为什么词元的计量与质量标准有价值：不同模型或不同服务的一个词元，不一定代表相同的成本和产出。

### No.4 · 物理 AI 的外部验证要落到工况

**[GAMES 研讨会议程](https://games-cn.org/games2026/) · [DataBeyond 新闻稿](https://www.prnewswire.com/news-releases/databeyond-showcases-ai-sorting-solutions-for-circular-supply-chains-at-cop31-302947646.html)**

上海的议程强调模拟与真实环境之间的联系，废料分选提供了一个具体检验场景。同样是“识别并拾取”，混料组成、传送带速度与污染率一变，结果就可能不同。判断方案是否适合部署，应看同工况下的回收率、纯度、处理量和维护成本，而不是把展示直接当作规模化运营的证据。

## 行业观察

- **看云推理：** 跟踪端点资格复核、实际处理方披露、以及备用路由是否继承原数据政策。这三项比一个隐私徽标更能说明合同是否会在运行中被执行。
- **看智能体产品：** DeepSeek 的预发布属于执行与集成层。对团队来说，先验证关键流程、权限与回滚，再讨论是否升级；不要用模型排行榜替代部署测试。
- **看科研：** 关于黎曼猜想的两份工作采用不同表达形式、经历不同复核路径。关注下一份有实质验证内容的专家说明，不把新的解读文章当作结论更新。
