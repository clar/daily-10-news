# AI 每日资讯 · 2026-07-06

## 今日焦点

> **奥特曼向白宫喊价 · Sonnet 5 定义"廉价 Agent" · GPT-5.6 三分家 · Anthropic 开辟制药新赛道 · 中国 GLM-5.2 冲击排行榜**
>
> - **OpenAI 提议向美国政府赠送 5% 股权（约 426 亿美元）**，套用阿拉斯加永久基金模式为国民发红利，同时希望"锁定"其他前沿实验室共同入场。
> - **Anthropic Claude Sonnet 5** 在 Terminal-Bench 上逼近 Opus 4.8，价格仅其 1/3，成为 Free/Pro 默认模型，将 Agent 单位算力成本压到新低。
> - **OpenAI 首次将 GPT-5.6 拆成 Sol/Terra/Luna 三档**，Sol 拿下 Terminal-Bench 2.1 88.8% SOTA，但仅限约 20 家政府背景机构预览，白宫深度介入前沿模型发布节奏。
> - **Anthropic 正式跨进新药研发**，推出 Claude Science 工作台 + 内部"被忽视疾病"药物发现项目，加入与 Google/OpenAI 的三方竞赛。
> - **Z.ai GLM-5.2 在 OpenRouter 反超 Anthropic**，以 1/6 成本获得接近前沿的编程/Agent 能力，被业内称为"迷你 DeepSeek 时刻"。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | OpenAI 拟赠美国政府 5% 股权 (~$42.6B)，仿阿拉斯加永久基金 | Forbes / CNBC / CNN | ⭐⭐⭐⭐⭐ |
| 2 | Anthropic 发布 Claude Sonnet 5：$2/$10 入门价，接近 Opus 4.8 表现 | Anthropic / TechCrunch | ⭐⭐⭐⭐⭐ |
| 3 | OpenAI 预览 GPT-5.6 Sol/Terra/Luna，仅政府白名单可用 | OpenAI / VentureBeat | ⭐⭐⭐⭐⭐ |
| 4 | Anthropic 推出 Claude Science 并成立内部药物发现团队 | CNBC / pharmaphorum | ⭐⭐⭐⭐ |
| 5 | Z.ai GLM-5.2 在 OpenRouter 反超 Anthropic，成本仅 1/6 | Japan Times / Modern Diplomacy | ⭐⭐⭐⭐ |
| 6 | EU AI Act 8 月 2 日全面生效，最高罚金 3500 万欧元或 7% 全球营收 | 欧盟委员会 / DLA Piper | ⭐⭐⭐⭐ |
| 7 | 上半年全球 VC 投资达 $510B，OpenAI+Anthropic 占 43% | The Information | ⭐⭐⭐⭐ |
| 8 | 特朗普签署"促进先进 AI 创新与安全"行政令，成立 AI 网络安全清算所 | White House | ⭐⭐⭐⭐ |
| 9 | Grok 5 训练滞后（1.5 GW Colossus 2 上），Polymarket 押注 Q3 发布概率 3% | Polymarket | ⭐⭐⭐ |
| 10 | NVIDIA GTC 2026：Isaac、Cosmos、GR00T 开源，联合 FANUC/Honda/TSMC 推物理 AI | NVIDIA Newsroom | ⭐⭐⭐⭐ |
| 11 | 联邦 2026 财年 AI 合同金额 $7.2B，同比 +966% | Brookings | ⭐⭐⭐ |
| 12 | Anthropic Claude Fable 5 全球恢复访问，出口管制放开 | Anthropic | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · OpenAI 拟赠美国政府 5% 股权

**[CNBC · OpenAI proposes U.S. government own 5% stake to address political blowback](https://www.cnbc.com/2026/07/02/openai-proposes-us-government-own-5percent-stake-to-address-political-blowback.html)** · **[Forbes · OpenAI Reportedly Pitches Granting U.S. Government 5% Stake](https://www.forbes.com/sites/siladityaray/2026/07/02/openai-reportedly-pitches-granting-us-government-5-stake/)**

Sam Altman 向白宫抛出的 5% 股权提案，在过去 72 小时内成为业界最大新闻。按 OpenAI 3 月 $852B 的估值计算，这笔股权价值约 $426 亿美元；奥特曼提议将其纳入类似阿拉斯加永久基金的主权工具，长期为美国居民派发"AI 分红"。方案不止针对 OpenAI，Altman 明确暗示"每个前沿实验室都应给美国政府 5%"——Anthropic、Google DeepMind、xAI 尚未表态，但可预见会形成极大的谈判压力。

这一提案实质上是 Altman 主动为 OpenAI 的"政治风险"寻找出口：从 GPT-5.6 被要求政府白名单预览、到白宫刚刚签署的 AI 安全行政令，一系列信号显示白宫正加速把前沿模型纳入国家安全轨道。以股权换监管缓冲（regulatory moat），既能锁定政府作为盟友，也能变相构建"太大不能倒"的护城河，让后来的挑战者（尤其是 Anthropic、xAI）面临同样的政治成本门槛。

短期看，Congress 必然需要立法配合，方案短期落地概率不高；但更值得关注的是——这或许标志着"AI 主权化"从口号进入实际议价阶段。

**点评：** 这不是让利，是买保险。Altman 用 5% 换的是未来 5 年 OpenAI 不被拆分、不被强制开源、不被 antitrust 起诉的"通行证"。

---

### 🚀 No.2 · Claude Sonnet 5：把 Opus 级 Agent 拉进平价区间

**[Anthropic · Introducing Claude Sonnet 5](https://www.anthropic.com/news/claude-sonnet-5)** · **[TechCrunch](https://techcrunch.com/2026/06/30/anthropic-launches-claude-sonnet-5-as-a-cheaper-way-to-run-agents/)**

6 月 30 日发布的 Sonnet 5 在核心 benchmarks 上给出了漂亮的答卷：Agentic Coding 63.2%（Opus 4.8 为 69.2%）、GDPval-AA v2 拿到 1618（超过 Opus 4.8 的 1615）、OSWorld-Verified 计算机使用 81.2%（Sonnet 4.6 为 78.5%）。价格方面，8 月 31 日前 $2/$10（输入/输出，每 M token）的引入价直接把 Opus 级能力打到了 Sonnet 价位。

对企业 Agent 场景意义重大：过去用 Opus 跑长任务往往被 token 成本劝退，现在用 Sonnet 5 就能获得"够用"的规划与工具调用能力。Anthropic 明显在打"Agent 单位任务成本"这场战——不是最强，而是最划算。Claude Code、Bedrock、Vertex 已全面接入，Free/Pro 用户默认切到 Sonnet 5。

配合同期恢复的 Fable 5 全球访问、Mythos 5 对美国部分组织重新开放，Anthropic 把矩阵重新铺齐。相比 OpenAI 被政府"卡脖子"分级发布 GPT-5.6，Anthropic 的定价+可用性策略明显更"开放商业"。

**点评：** Anthropic 正在成为"给企业跑 Agent 的默认选项"，OpenAI 若继续被政府特批限流，会把中端 Agent 市场直接让给 Sonnet 5。

---

### 🧬 No.3 · Anthropic 跨入新药研发，Claude Science 上线

**[CNBC · Anthropic launches AI drug discovery program](https://www.cnbc.com/2026/06/30/anthropic-launches-ai-drug-discovery-program-claude-science.html)** · **[pharmaphorum](https://pharmaphorum.com/news/anthropic-launches-claude-science-pharma-researchers)**

7 月 3 日，Anthropic 同时宣布两件事：(1) 面向研究人员的 Claude Science 工作台正式 beta——聚合 60+ 数据库、支持基因组学/蛋白组学/化学信息学工作流；(2) 成立内部药物发现团队，主攻大型药企不愿投入的"被忽视疾病"，首批合作方包括 Novo Nordisk 和 Allen Institute。项目提供最高 $30,000 使用额度。

这一动作意义远超商业范畴。OpenAI 有 OpenAI for Science、Google DeepMind 有 Isomorphic Labs——Anthropic 是最后一个跨进 AI + 生命科学赛道的前沿实验室。选择"被忽视疾病"作为切入点是聪明的：既避开与传统药企正面竞争，又能积累 wet-lab 反馈数据。生命科学领域是极少数 AI 能真正创造万亿美元级新价值的场景，前沿实验室下场自建 R&D 团队，标志着 AI 公司从"卖 API 给药企"升级为"直接和药企竞争 IP"。

**点评：** 当 Anthropic 开始"用自己的模型做自己的药"，SaaS 型 AI 平台的想象力天花板被再次抬高——它们要卖的不是 token，是分子。

---

### 🇨🇳 No.4 · Z.ai GLM-5.2：迷你 DeepSeek 时刻

**[Japan Times · A cheap Chinese model is catching up with U.S. AI giants](https://www.japantimes.co.jp/business/2026/07/03/tech/china-ai-catch-up/)** · **[Modern Diplomacy](https://moderndiplomacy.eu/2026/07/02/can-chinas-new-glm-5-2-ai-challenge-openai-and-anthropic/)**

GLM-5.2 在 OpenRouter 上的调用量已经超过 Anthropic 系列，Intelligence Index v4.1 拿到 51 分，位列全球第 5，甩开 DeepSeek V4 Pro 与 MiniMax-M3。关键卖点：编程与 Agent 能力接近前沿，价格却是前沿的 1/6，且以开源权重方式提供，允许企业自建部署。

对全球开发者社区的冲击是即时的：过去半年，中国开源模型逐步吃掉了"性价比生态位"，把 OpenAI/Anthropic 逼向"极限性能 + 高价"的顶端。GLM-5.2 的成功让 Silicon Valley 的成本焦虑再度上升——Anthropic 单季 API 收入首次同比放缓，很难不与此有关。

政策端仍是最大变量：GLM-5.2 硬编码了政治敏感话题的过滤器，美国金融/网络安全客户仍受合规掣肘。但对绝大多数亚洲、拉美和欧盟中小型企业来说，价格差异足够压过合规顾虑。

**点评：** 前沿的护城河越来越窄。一年前的 DeepSeek 是意外，一年后的 GLM-5.2 已经是常态——中国"快跟随者"策略在落地成本上开始形成结构性优势。

---

### 🏛️ No.5 · EU AI Act 全面生效倒计时 27 天

**[European Commission · AI Act](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)** · **[DLA Piper AI Laws Tracker](https://intelligence.dlapiper.com/artificial-intelligence/?t=08-enforcement&c=EU)**

8 月 2 日 EU AI Act 将全面生效，三档罚则：(1) 违反禁止性 AI 用途最高 3500 万欧元或 7% 全球营收；(2) 高风险 AI 系统最高 1500 万欧元或 3% 营收；(3) 提供虚假信息最高 750 万欧元或 1% 营收。禁止性用途和 GPAI 义务已于 2025 年 2 月和 8 月分批生效，欧盟委员会已在 2026 年初启动首批正式调查。

对 OpenAI/Anthropic/Google 等 GPAI 提供方而言，最紧迫的合规义务是文档、能耗、系统性风险评估三大类；对企业采购方，则是"高风险清单"分类正在从法条化转向真实执法。多家跨国企业已在 2026 Q2 财报里追加合规准备金。

**点评：** 欧盟的做法明显 vs 美国的"股权换空间"：一个用罚金给行业画界，一个用国家资本入股。未来 3 年，全球 AI 公司将不得不同时管理两套完全不同的政治风险。

---

## 行业观察

**主题一：政治资本正在快速渗入前沿模型层。** 白宫既签行政令又拿 GPT-5.6 分级发布权、又被劝进 OpenAI 5% 股权，一周内三件事共同勾勒出"美国主权基金化前沿 AI"的路线图。欧盟走的是罚金+分类监管，两条路径都会持续挤压前沿实验室的商业自由度。

**主题二：Agent 成本战进入白热化。** Sonnet 5、GPT-5.6 Terra/Luna、GLM-5.2 都在过去 10 天内以"更便宜的中端能力"作为主打卖点。企业 Agent 落地的"每任务美元数"正在指数级下降，2026 下半年的核心竞争已经不是模型智能，而是"能不能长时间稳定跑一整个业务流程"。

**主题三：AI 公司开始纵向一体化。** Anthropic 自建药厂、OpenAI 自建 datacenter 与 chip、NVIDIA 从卖芯片到卖机器人整栈——单纯"卖模型"的商业模式正在成为过去时。垂直资本堆积深度决定谁能吃到下一波价值。

**主题四：中国生态正在成为独立引擎，而不是追赶者。** GLM-5.2 在 OpenRouter 反超 Anthropic 不是偶然，它验证了"开源 + 极致性价比 + 自主生态"路径可以持续输出竞争力。政策脱钩+成本代差正在把全球 AI 生态推向"双极化"。
