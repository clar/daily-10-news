# AI 行业日报 · 2026-10-25

## 今日焦点

> **开源模型密集更新 · 中国实验室估值重估 · 芯片竞争进入"推理定价"时代 · AI 治理分化加剧 · 机器人推理范式切换**
>
> - **Qwen3.6 27B / MiniMax M3.1 Flash / DeepSeek V4.1 Flash** 一周内接连登陆排行榜，开源阵营迭代节奏追平前沿闭源厂商
> - **Anthropic $900B 估值轮已基本敲定条款，收入年化冲向 $45B**，首次在估值维度超越 OpenAI
> - **DeepSeek 新一轮估值接近 $740 亿**，为明年可能的上海 IPO 铺路，中国 AI 独角兽进入"百亿美元俱乐部"
> - **AMD Helios 机架开始小批出货、Intel Crescent Island 下半年送样**，Nvidia Vera Rubin 的时间差被加速压缩
> - **arXiv 新论文《ARC: A Reasoning Recipe for Robot Foundation Models》** 提出"用推理代替数据"的机器人新路线，挑战 VLA 大数据范式

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Anthropic 敲定 $30B 新一轮融资，估值达 $900B，首次反超 OpenAI | Dealroom / The Decoder | ⭐⭐⭐⭐⭐ |
| 2 | DeepSeek 新一轮融资估值逼近 $740 亿，瞄准 2027 上海 IPO | 聚合媒体 | ⭐⭐⭐⭐⭐ |
| 3 | 阿里 Qwen3.6 27B 10 月 21 日上线，全面升级多模态与长上下文 | llm-stats / LLM Gateway | ⭐⭐⭐⭐ |
| 4 | Anthropic 据报探索 $70 亿收购芯片初创 MatX | aifunding.me | ⭐⭐⭐⭐ |
| 5 | AMD Helios AI 机架 Q3 2026 开始发货，正式进入与 Nvidia 对位竞争 | S&P Global / 市场研报 | ⭐⭐⭐⭐ |
| 6 | arXiv 新论文：机器人基础模型用"推理"替代"数据扩展" | arXiv 2610.12386 | ⭐⭐⭐⭐ |
| 7 | Butterfly Effect 获博裕资本、IDG 领投 $5 亿 C 轮 | aifunding.me | ⭐⭐⭐ |
| 8 | 美国 AI 创业公司占据 9 月末本国 Top 10 融资中的 8 席，一周吸金 $28.6 亿 | AF.NET | ⭐⭐⭐ |
| 9 | Meta Muse Spark、xAI Grok Voice 3.0 本月中旬同周发布 | BenchLM | ⭐⭐⭐ |
| 10 | Intel Crescent Island 数据中心 AI 芯片 H2 2026 开始送样 | Barchart | ⭐⭐⭐ |
| 11 | NVIDIA Nemotron 3.5 Super VL 120B / Liquid AI LFM2.5-24B 开源发布 | BenchLM | ⭐⭐⭐ |
| 12 | 10 月单月 AI 创业总融资回落至 $6.32 亿（10/12-16 周），创近三月新低 | aifunding.me | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Anthropic 以 $900B 估值反超 OpenAI，年化收入冲向 $450 亿

**[The Decoder](https://the-decoder.com/anthropics-900-billion-valuation-would-make-it-more-valuable-than-openai-for-the-first-time/) · [Dealroom](https://dealroom.co/news/128968-anthropic-agrees-terms-for-30b-round-at-900b-valuation-overtaking-openai/)**

据《金融时报》与《The Information》报道，Anthropic 已基本敲定 $300 亿美元新融资的条款，公司估值达到 $9000 亿美元（pre-money）。这一数字较其 2026 年 2 月的 $3500 亿美元估值几乎翻了近 3 倍，更首次正式超越了 OpenAI 彼时 $8520 亿美元的估值。公司年化收入也从 2025 年底的约 $90 亿美元跃升至接近 $450 亿美元——不到一年时间收入翻 5 倍，是美国 SaaS 史上从未出现过的速度。

与估值并列的，是 Anthropic 内部的战略转向。市场普遍将 Claude Code 与企业 API 视为增长主力：从 Opus 4.5 到 Haiku 5.5 的层级化定价、与 AWS 的 trainium 深度绑定，再到传闻中探索收购芯片初创 MatX（估值 $70 亿美元），Anthropic 正在构建"模型 - 工具链 - 自有算力"的全栈闭环。相较之下，OpenAI 的 AMD/Nvidia 多云算力路线显得更分散。

**点评：** 估值反超本质是收入曲线的斜率问题——Anthropic 的"企业优先、Claude Code 作为切入"路线正把 OpenAI 的 ToC 增长故事比下去；下一步看它能否在不自研推理芯片的情况下，用 MatX + Trainium 把毛利率守住。

---

### 🚀 No.2 · DeepSeek 估值冲向 $740 亿，为 2027 年上海 IPO 铺路

**[综合报道](https://blog.mean.ceo/?p=11147)**

DeepSeek 正在以接近 $740 亿美元估值完成新一轮融资。这是继 Butterfly Effect（$5 亿 C 轮）、Moonshot、智谱等中国模型实验室之后，又一个有望在上海交易所 IPO 的 AI 独角兽。公司明确表示本轮资金将用于下一代推理模型 R2 与 V4 系列的训练算力扩张，以及东南亚市场的本地化部署。

值得注意的是，中国这一轮 AI 融资潮的资本结构正在发生变化：博裕资本、IDG、源码等财务 VC 外，国家大基金、合肥建投等"产业资本"份额明显上升。DeepSeek 若顺利 IPO，将成为自寒武纪之后中国 AI 公司最大的二级市场事件，并直接检验中国投资者对"推理价格战赢家"的定价能力。

**点评：** 中国 AI 的融资叙事正从"模型追赶美国"切换到"推理成本领先 + 本土 IPO 退出"，DeepSeek 的估值其实比技术指标更具行业信号意义。

---

### 🧠 No.3 · 开源阵营一周三连发：Qwen3.6 / MiniMax M3.1 / DeepSeek V4.1

**[LLM Stats](https://llm-stats.com/ai-news) · [LLM Gateway Timeline](https://llmgateway.io/timeline)**

在 10 月 17 日至 21 日短短 5 天内，中国开源阵营连续放出三款旗舰：Alibaba Qwen3.6 27B（10/21）、MiniMax M3.1 Flash（10/19）、DeepSeek V4.1 Flash 1017（10/17）。Qwen3.6 的核心升级在于长上下文窗口（≥1M tokens）与原生多模态；MiniMax M3.1 Flash 则在定价上做激进下探，直接把每百万 output tokens 价格压到 $0.3 以下。

与此同时，欧美开源阵营也不落后：NVIDIA 本月中发布了 Nemotron 3.5 Super VL 120B（MoE，总参数 120B，激活 12B），Liquid AI 推出了 LFM2.5-24B-A2B，EmbeddingGemma 2 也在本月初更新。开源与半开源旗舰的"月更"节奏，意味着企业用户不再需要为前沿能力支付高溢价。

**点评：** 开源 AI 已经进入"推理定价追赶闭源旗舰"的阶段，闭源厂商的护城河将不得不从"模型本身"转移到"工具链 + Agent + 分发"。

---

### 🏗️ No.4 · 芯片战争进入"推理定价"时代：AMD Helios 出货，Intel Crescent Island 送样

**[S&P Global](https://www.spglobal.com/market-intelligence/en/news-insights/research/2025/10/analysts-lift-amds-long-term-revenue-forecasts-after-openai-deal) · [Barchart](https://www.barchart.com/story/news/2266627/intel-sets-sights-on-nvidia-and-amd-with-upcoming-ai-data-center-chip-launch-by-year)**

AMD 的 Helios AI 机架（基于 MI400 系列）已于 Q3 2026 开始小批量出货，并计划在 2027 年全面放量。AMD 与 OpenAI 签署的 6GW 算力协议是其订单基本盘；叠加 Q1 数据中心收入同比+57% 至 $58 亿美元，市场重新给 AMD 定价。Nvidia 本月已开始发货 Vera Rubin，但其 Q4 毛利率指引下调至 71-72%，被视为推理价格战压力的先兆。

Intel 的 Crescent Island（专门针对推理场景）将于 2026 年下半年开始客户送样。虽然 Intel 在训练市场几乎失守，但以 Granite Rapids CPU + Gaudi 3 + Crescent Island 的组合押注"推理服务器"，技术路线上更接近 AMD 而非 Nvidia。推理市场的 TAM 将在未来 3 年从 $300 亿美元扩张到超过 $2000 亿美元，这里才是真正的战场。

**点评：** 训练端 Nvidia 近乎垄断，但推理端是真正的 commodity 战场——价格、功耗、总体 TCO 决定胜负，AMD/Intel 都有机会分走一块。

---

### 🤖 No.5 · 机器人基础模型新范式：《ARC》提出"推理代替数据"路线

**[arXiv 2610.12386](https://arxiv.org/)**

10 月 8 日上传的论文《ARC: A Reasoning Recipe for Robot Foundation Models》提出：当下 VLA（Vision-Language-Action）主流路径——通过收集更多机器人示范数据+更大模型——存在边际收益递减；而将推理（CoT、ToT、规划器）直接融入控制回路，可以在数据量减少 10 倍的情况下保持甚至超过现有性能。该工作得到了 Figure、1X、Physical Intelligence 等前沿机器人实验室的早期背书。

此论文的意义不只在学术层面——它直接挑战了 Nvidia GR00T、Google DeepMind RT-X 等"大模型+大数据"的路线假设。如果"推理替代数据"成立，机器人创业公司的护城河将从"数据采集成本"转向"推理模型质量"，这将显著改变 Figure/1X/Agility 等公司的估值逻辑。

**点评：** 大模型从"把数据喂到饱"切换到"用推理蒸馏数据价值"，这条路径一旦跑通，机器人数据工厂的叙事会被推倒重来。

---

## 行业观察

今天的几条消息，拼起来是一张清晰的"**后训练时代**"地图：

- **估值与权力重排。** Anthropic 以 $900B 反超 OpenAI 并不只是财务事件，而是企业市场定价权向 Anthropic 倾斜的标志。中国侧则由 DeepSeek 独角兽化领跑，产业资本进场，使 IPO 退出窗口首次打开。
- **开源与闭源差距进一步收窄。** 一周之内三个中国开源旗舰、两个欧美开源 MoE 模型齐发，参数规模、上下文、价格都在同时逼近闭源旗舰。企业的采购决策开始从"选哪个闭源 API"变成"自托管还是云托管"。
- **推理市场成为真正战场。** AMD Helios 出货、Intel Crescent Island 送样、Nvidia 毛利指引下调，三家在"推理 TCO"维度首次正面对撞；MiniMax M3.1 Flash、DeepSeek V4.1 Flash 的定价下探，更是直接把这场战争打到应用层。
- **机器人与具身智能换挡。** ARC 论文暗示 Scaling Law 在物理世界的失效，机器人数据飞轮的护城河被重估——下一个 12 个月，Figure/1X/Physical Intelligence 的估值逻辑可能被改写。
- **治理分化已难逆转。** 美国以行业自愿承诺为主、欧盟通用 AI 条款强制落地、中国侧重应用层监管——"一个 AI，三条治理路径"将直接影响大模型厂商的全球产品矩阵与数据合规成本。

今日主题可以浓缩为一句话：**模型的边际价值在下降，而推理算力、企业分发与具身智能的边际价值在上升。**
