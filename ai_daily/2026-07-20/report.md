# AI 日报 · 2026-07-20

## 今日焦点

> **Fable 5 转入信用点计费 · GPT-5.6 三档下沉抢占中端 · 中国开源模型逼近前沿 · 欧盟"数字总线"落地 · AI 独占 H1 全球风投 86%**
>
> - **Anthropic 今日起 Fable 5 全面切换 usage credits** 定价 $10/$50 per M tokens，Pro/Max 用户告别"50% 免费额度"过渡期。
> - **OpenAI GPT-5.6 Sol 在 Agents' Last Exam 拿到 53.6 分** 领先 Fable 5 达 13.1 分，Terra/Luna 触发端到端价格战。
> - **Moonshot Kimi K3 登顶 Arena Frontend Code Arena** 76% 对战胜率，把开源前沿模型的中美差距缩到"周"级。
> - **欧盟《数字 AI 总线》正式生效** 高风险 AI 义务分批推迟至 2027-12/2028-08，透明度条款 8 月 2 日仍如期启动。
> - **H1 全球风投触及 5100 亿美元历史峰值** 其中 3559 亿美元流向 AI，OpenAI + Anthropic 单季吸金 2170 亿。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Claude Fable 5 免费额度今日到期，转入信用点计费 $10/$50 | Anthropic / DigitalApplied | ⭐⭐⭐⭐⭐ |
| 2 | OpenAI GPT-5.6 Sol/Terra/Luna 三档发布，引入 Ultra Mode 与可编程工具调用 | OpenAI / MarkTechPost | ⭐⭐⭐⭐⭐ |
| 3 | H1 2026 全球风投达 5100 亿美元，AI 独占 86% | Crunchbase | ⭐⭐⭐⭐⭐ |
| 4 | Moonshot Kimi K3 开源模型登顶前端代码竞技场 76% 胜率 | Tech Startups | ⭐⭐⭐⭐⭐ |
| 5 | 欧盟《数字 AI 总线》签署生效，高风险合规窗口延后 | European Council | ⭐⭐⭐⭐ |
| 6 | Google Gemini 3.5 Pro 因编码与长程推理未达预期推迟发布 | Tech Startups | ⭐⭐⭐⭐ |
| 7 | Anthropic 完成 650 亿美元融资，估值 9650 亿美元 | Crunchbase | ⭐⭐⭐⭐ |
| 8 | SpaceX 上市并宣布 600 亿美元收购 Cursor 母公司 Anysphere | Crunchbase | ⭐⭐⭐⭐⭐ |
| 9 | Nvidia 确认 2027 年前 1 万亿美元 AI 芯片需求已锁定 | 24/7 Wall St. | ⭐⭐⭐⭐ |
| 10 | DeepMind 数学推理系统在 IMO 试题上进入全球前 1% | Skycrumbs | ⭐⭐⭐⭐ |
| 11 | JetSpec 推测解码在 MATH-500 上取得 9.64 倍加速 | AIapps | ⭐⭐⭐ |
| 12 | 欧盟 7 月网络安全与 AI 行动计划：2027 年前建成前沿模型评估能力 | EU Commission | ⭐⭐⭐ |
| 13 | Shield AI 完成 15 亿美元 G 轮，估值 127 亿美元同比翻倍 | Crunchbase | ⭐⭐⭐ |
| 14 | Anthropic Claude Sonnet 5 促销价 $2/$10 延续至 8 月 31 日 | Anthropic | ⭐⭐⭐ |
| 15 | Meta Muse Spark 1.1 与 xAI Grok 4.5 加入价格战 | ThursdAI | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Claude Fable 5 免费额度今日到期，进入信用点付费时代

**[Anthropic 官方通告](https://www.anthropic.com/news/redeploying-fable-5) · [DigitalApplied 定价指南](https://www.digitalapplied.com/blog/claude-fable-5-usage-credits-july-7-pricing-guide-2026)**

从今天（7 月 20 日）开始，Anthropic 结束了自 6 月 9 日 Fable 5 首发以来的"50% 每周额度包含期"过渡安排。Pro、Max、Team、Enterprise 用户此前可在计划限额的一半份额里免费调用 Fable 5，而现在这部分调用全部转入 usage credits 计费——输入 $10/百万 token、输出 $50/百万 token，与 Fable 5 API 层保持一致。此前 Anthropic 已经在 7 月 7 日推迟一次，把窗口延到 7 月 19 日，今天是最终切换日。

这次转轨的信号比价格本身更值得关注。Fable 5 于 6 月 9 日发布，仅 3 天就被美国商务部以出口管制为由暂停海外访问，直到 6 月 30 日豁免松绑、7 月 1 日全球恢复上线。Anthropic 用一次"送 20 天再上闸"的方式把用户导入 Fable 5，同时靠 Sonnet 5 的低价（$2/$10 促销延续到 8 月 31 日）稳住中端 API 流水。对比 OpenAI GPT-5.6 Sol $5/$30 的定价，Fable 5 明显是走"最难的长任务、最贵的信用点"路线，而不是与 Sol 正面价格对撞。

对开发者的实际影响：如果你的工作负载依赖多小时以上的 agentic 任务链（Anthropic 官方宣称 Fable 5 能撑住"days-long"任务），今天开始每个 token 都在花钱，务必检查预算告警；如果只是普通对话或代码补全，切回 Sonnet 5 是最经济的选择。

**点评：** Anthropic 用"免费—禁运—复出—收费"的四步节奏完成了一次教科书级的高端模型定价拉升，现在能不能守住 Agents' Last Exam 榜二的位置，就看 Sol Ultra 的凶猛程度了。

---

### 🚀 No.2 · GPT-5.6 三档发布，OpenAI 用 Terra/Luna 打价格战

**[OpenAI 官方发布](https://openai.com/index/gpt-5-6/) · [MarkTechPost 技术评论](https://www.marktechpost.com/2026/07/09/openai-releases-gpt-5-6-a-three-tier-model-family-with-programmatic-tool-calling/)**

7 月 9 日 OpenAI 一次性亮出 GPT-5.6 的 Sol / Terra / Luna 三档，重构了自家产品线的命名方式：数字代表代际，Sol/Terra/Luna 代表可独立演进的能力档位。定价上 Sol $5/$30、Terra $2.50/$15、Luna $1/$6，Terra 官方对标"GPT-5.5 同级性能、价格减半"。Sol 端还引入了 Ultra Mode（多 agent 并行协调）、Max 推理档、可编程工具调用（在内存里跑 JS 组合调用），以及 30 分钟最短生命的显式 prompt cache。

Agents' Last Exam 榜单上 Sol 拿到 53.6 分——这是一个覆盖 55 个专业领域、评估长任务能否"做完"而非"答对"的基准——比 Fable 5 高出 13.1 分。Terra 和 Luna 的意义在于中低端的定价穿透力：Terra 直接把主流 SaaS 里的模型替换成本压到 $2.50 输入价，Luna 更是把 API 价格带回了 GPT-4 早期水平，联合 Meta Muse Spark 1.1、xAI Grok 4.5 一起把整个推理市场推入价格战。

值得观察的是 ChatGPT Work agent——OpenAI 把 Codex 演化成"完成整份工作而非回答问题"的 superapp，直接与 Anthropic 的 Fable 5 长任务路线正面对撞。

**点评：** OpenAI 用"一颗旗舰堵住 Anthropic + 两颗腰部大规模降价"的组合拳锁住企业市场，Anthropic 现在必须靠 Fable 5 的绝对能力护城河来抵消 Terra 的性价比冲击。

---

### 🥉 No.3 · Moonshot Kimi K3 登顶前端代码竞技场，开源前沿的中美差距按周计

**[Tech Startups 报道](https://techstartups.com/2026/07/17/top-tech-news-today-july-17-2026-anthropic-apple-google-meta-moonshot-ai-nvidia-more/)**

北京 Moonshot AI 上周发布开源权重新模型 Kimi K3，在 Arena.ai Frontend Code Arena 头对头对战中拿到 76% 胜率，直接夺走该榜首位。这是继 Qwen、DeepSeek 之后，中国开源模型第三次在编码与 agent 任务上正面挑战闭源前沿，而且节奏在明显加快——GPT-5.6 Sol 发布仅 8 天后就有一个开源竞品在同类基准上占位。

对全球开发者的意义：开源前沿模型不再是"追平主流的次优选"，而是能在特定垂直（前端代码、Agent 工具调用）领先闭源同类的现实选项。对企业采购者，Kimi K3 是继 Qwen3 Coder 之后又一个"能自托管、能改权重、能规避出口管制"的一线选择，进一步压缩了闭源模型可收取的能力溢价。

同时值得注意，Google 的 Gemini 3.5 Pro 因内部测试中编码与长程推理未达预期被推迟，只以"企业限量预览"形式存在。开源和闭源在编码这个战场上的角色，正在肉眼可见地互换。

**点评：** 当一款免费开源模型在编码 Arena 上打赢所有闭源前沿时，"用最好模型的成本"这句 SaaS 定价假设第一次被击穿——Fable 5 和 Sol 的溢价空间将由长任务、多模态、企业安全三件事继续守护，纯代码这块正在被开源吃掉。

---

### ⚡ No.4 · 欧盟《数字 AI 总线》生效，高风险合规窗口整体推迟

**[欧洲理事会新闻稿](https://www.consilium.europa.eu/en/press/press-releases/2026/06/29/artificial-intelligence-council-gives-final-green-light-to-simplify-and-streamline-rules/) · [Technology.org 8 月 2 日启动解读](https://www.technology.org/2026/07/17/eu-ai-act-what-actually-applies-on-2-august-2026/)**

欧盟"简化 AI Act"的 Digital Omnibus 于 6 月 29 日获理事会最终批准，7 月 8 日签署，进入《官方公报》即生效。核心变化：Annex III 独立高风险 AI 系统的合规义务从原本 2026 年 8 月推迟至 **2027 年 12 月 2 日**；嵌入受 Annex I 监管产品的 AI 义务延至 **2028 年 8 月 2 日**；透明度条款依然按原计划 **8 月 2 日**（下周日）生效。

同期 Article 5 新增禁止"AI 生成的非合意亲密影像"，与儿童性虐待材料并列——自 2026 年 12 月 2 日起适用。此外，欧盟委员会推出 7 月 Cybersecurity + AI 行动计划，2027 年前建成 EU 内部的前沿模型评估能力，为第三方评估提供官方基础设施。

对本土与海外企业：8 月 2 日仍必须准备好基础模型透明度报告和数据训练来源披露；但如果你之前把 2026 Q3 定为"高风险系统上市死线"，现在多了 16 个月，可以把资源腾出来做产品迭代。

**点评：** 欧盟这次"减速"是承认了监管跑得比市场快的现实，但透明度条款如期生效意味着开源模型和商业模型都必须公开训练数据画像——短期不痛，长期是给模型溯源留了一根随时可以拧紧的螺栓。

---

### 💰 No.5 · H1 全球风投触 5100 亿美元史高，AI 独吞 86%

**[Crunchbase 半年数据](https://news.crunchbase.com/venture/global-startup-exits-ipo-ma-soar-ai-q2-h1-2026/) · [Crunchbase 北美记录](https://news.crunchbase.com/venture/na-startup-funding-ma-shattered-records-ai-q2-q2-2026/)**

Crunchbase 数据显示，2026 年上半年全球初创融资总额达到 5100 亿美元，已超过 2025 年全年 4400 亿——半年跑赢全年。AI 公司拿走 3559 亿美元，占比 **86%**；仅 OpenAI 和 Anthropic 两家单季吸金 2170 亿美元，占 H1 全部初创融资的 **43%**。Anthropic 单季完成 650 亿美元融资，投后估值 9650 亿美元，即将踏入万亿俱乐部；SpaceX 以 1.77 万亿美元估值 IPO 融资 750 亿美元，一周后宣布 600 亿美元收购 Cursor 母公司 Anysphere——这是史上最大规模的初创并购交易，也是史上最大规模的 VC 支持 IPO。

层级之下，Shield AI 完成 15 亿美元 G 轮（更大 22.5 亿一揽子中的股权部分），估值 127 亿美元，同比翻倍 140%。国防、Agent、编码工具三条主线明显吸走了 AI 生态里的"非模型"资金。

值得警惕的是集中度：AI 生态里的 43% 资金流向了两家公司，这意味着投给"下一个 Anthropic"的钱在急剧减少。对创业者，"能被 OpenAI/Anthropic 收购或整合"正在变成事实上的退出策略。

**点评：** 当两家公司拿走 43% 的钱，AI 已经不是资本市场，是"两个国家 + 无数附庸"的封建结构——SpaceX 收购 Cursor 揭示了另一条路径：模型层封顶后，钱开始堆向工具与基础设施的"下一层护城河"。

---

## 行业观察

**竞争格局：** GPT-5.6 三档发布 + Fable 5 转付费 + Kimi K3 登顶，三件事同一周发生，标志着大模型市场进入"分层竞争"阶段——Sol vs Fable 5 拼旗舰能力，Terra/Luna vs Sonnet 5 vs Kimi K3 拼中端性价比，Nvidia 的 Rubin 提前和 DSX 液冷则从算力层再挤压一次单位推理成本。

**趋势加速：** Agent 是全场共识关键词。GPT-5.6 Ultra Mode、ChatGPT Work、Fable 5 的 days-long 任务能力、Kimi K3 的 agent 榜单表现，都在把行业从"聊天问答"推向"完成整块工作"。Agents' Last Exam 这个 55 领域基准正在事实上取代 MMLU 成为新一代 benchmark。

**监管方向：** 欧盟走了"表面简化、底层加固"的路径——延后高风险义务但保留透明度和 AI 评估能力；同期美国 SpaceX 收购 Cursor、Anthropic 融资超 9000 亿美元，几乎没有反垄断阻力，中美监管在 AI 集中度问题上的态度差正在扩大。

**下一个观察点：** 8 月 2 日欧盟 AI Act 透明度条款生效实操细节；Anthropic Fable 5 转付费一周后的实际调用量下降幅度（会决定 Sonnet 5 促销是否延长）；以及 Kimi K3 是否能守住 Arena 榜首超过一个月。
