# AI 每日资讯 · 2026-07-18

## 今日焦点

> **中国 WAICO 与美国 Pax Silica 阵营对垒 · 开源天花板被 Kimi K3 抬到 2.8T · Google Gemini 3.5 Pro 上量 · Apple 起诉 OpenAI 拉开硬件战 · Meta 挑起 API 价格战**
>
> - **Xi Jinping 揭幕 WAICO**：29 国 AI 合作组织落户上海，直接对标 35 国的 Pax Silica，中国承诺 5 年 5000 名发展中国家 AI 培训名额。
> - **Moonshot 放出 Kimi K3**：2.8 万亿参数 MoE、开源天花板刷新，Frontend Code Arena 竟压过 Claude Fable 5，7 月 27 日放出全部权重。
> - **Google Gemini 3.5 Pro 今日 GA**：2M token 上下文、Deep Think 独占 Ultra 250 美元档、API 1.25/10 美元定价直接进入价格战。
> - **Apple 与 OpenAI 硬件官司升级**：诉状延烧至 Jony Ive 的 io Products，OpenAI 硬件负责人被点名"从每一层"窃密。
> - **Meta Muse Spark 1.1 掀 API 价格战**：$1.25/$4.25 直接砸穿同档位，OpenAI/SpaceXAI 24 小时内被迫跟进。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Xi Jinping 在 WAIC 揭幕 29 国 WAICO 联盟，对标美国 Pax Silica | Al Jazeera / CNBC | ⭐⭐⭐⭐⭐ |
| 2 | Moonshot Kimi K3 发布：2.8T 参数开源 MoE，Frontend Code Arena 首位 | VentureBeat / Tom's Hardware | ⭐⭐⭐⭐⭐ |
| 3 | Google Gemini 3.5 Pro 今日 GA：2M 上下文 + Deep Think | 泄漏文档 / MindStudio | ⭐⭐⭐⭐⭐ |
| 4 | Apple 起诉 OpenAI 与 io Products，指控系统性窃取硬件商业秘密 | CNN / Bloomberg | ⭐⭐⭐⭐ |
| 5 | TSMC Q2 净利润 220 亿美元同比 +77%，全年资本开支上调至 640 亿 | 财报 | ⭐⭐⭐⭐ |
| 6 | Meta Muse Spark 1.1 + Meta Model API 首推付费闭源，$1.25/$4.25 挑起价格战 | Crypto Briefing / New Stack | ⭐⭐⭐⭐ |
| 7 | Anthropic + Blackstone 押注"实施层"下一个万亿业务 | TechCrunch | ⭐⭐⭐⭐ |
| 8 | Thinking Machines 发布首个开源权重模型 Inkling（975B 总参 / 41B 激活） | TechCrunch / Bloomberg | ⭐⭐⭐⭐ |
| 9 | Anthropic 秘密提交 IPO 材料，估值可能突破 1 万亿美元 | Distill Intelligence | ⭐⭐⭐⭐ |
| 10 | Microsoft 培训销售团队"打压 OpenAI 与 Anthropic"，Copilot 反攻大客户 | TechCrunch | ⭐⭐⭐ |
| 11 | 白宫与 OpenAI/Google/Anthropic 敲定前沿模型自愿发布标准 | AIToolsRecap | ⭐⭐⭐ |
| 12 | Nvidia 领投法国语音 AI Gradium 3000 万美元扩融，种子轮累积破 1 亿 | Sifted | ⭐⭐⭐ |
| 13 | 韩国宣布 10 年 8800 亿美元半导体+AI+机器人投资计划 | 韩国政府 | ⭐⭐⭐ |
| 14 | Microsoft 2026 年 7 月补丁日修复创纪录的 570 个漏洞 | Microsoft | ⭐⭐⭐ |
| 15 | 英国人形机器人公司 Humanoid Series A 首关 1.5 亿美元 @ 12 亿 pre | Sifted | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · 中国 WAICO 联盟落地，AI 治理正式进入两极时代

**[Al Jazeera](https://www.aljazeera.com/news/2026/7/17/chinas-xi-jinping-launches-new-ai-alliance-what-is-it) · [CNBC](https://www.cnbc.com/2026/07/17/x-china-ai-summit-risks-security.html)**

Xi Jinping 昨日亲自出席上海 WAIC 大会——这是 9 年 WAIC 历史上首次由最高领导人开场——正式宣布"世界人工智能合作组织"（WAICO）落地，创始 29 国清一色为全球南方阵营：印尼、巴西、马来西亚、南非、塞内加尔、俄罗斯、巴基斯坦，联合国秘书长 Guterres 亦到场站台。北京同步承诺 5 年内向发展中国家提供 5000 个 AI 培训名额，并把中国国产的 AI 天气预警系统免费开放给 30 国。

这一动作的地缘博弈意味极浓——它与美国主导的 Pax Silica（已签约 35 国）正面对垒。Pax Silica 走的是"高性能出口管控 + 芯片配额"路线，WAICO 反其道走"低成本开源模型 + 培训援助"，恰好卡在了 Kimi K3、DeepSeek 系列打开局面的窗口期。分析人士普遍判断，中方会把 WAICO 作为 UN AI 治理谈判桌上的谈判筹码，未来一年内的 AI 全球规则议题将不可避免地被卷入。

对企业侧看点也很明确：中国把"开源大模型 + 免费公用事业"打包成外交礼物，短期利好国内做 Global South 场景的推理云服务商与教育合作方，长期则可能挤压美方闭源 API 在这些国家的商业空间。

**点评：** WAICO 与 Pax Silica 已经把两阵营的 AI 生态基本切开；今后新模型的性价比曲线，将取决于你是想收 GDP 前二十的钱，还是收后一百三十国的钱。

---

### 🚀 No.2 · Kimi K3 用 2.8 万亿参数把"开源天花板"直接拉高

**[VentureBeat](https://venturebeat.com/technology/chinas-moonshot-ai-releases-kimi-k3-the-largest-open-source-model-ever-rivaling-top-u-s-systems) · [Tom's Hardware](https://www.tomshardware.com/tech-industry/artificial-intelligence/moonshot-releases-2-8-trillion-parameter-kimi-k3) · [Simon Willison](https://simonwillison.net/2026/Jul/16/kimi-k3/)**

7 月 16 日发布、7 月 27 日全权重开放的 Kimi K3 已经登顶"史上最大开源模型"：2.8 万亿总参数、896 专家池、每 token 只激活 16 个（1.8%），架构继承自 Kimi Delta Attention + Attention Residuals，原生 1M token 上下文，自带视觉与常驻推理模式。关键成绩：GDPval-AA v2 排第三（仅次 Claude Fable 5 Max 和 GPT-5.6 Sol Max）、AA-Briefcase 排第二反超 GPT-5.6、Frontend Code Arena **在盲测中直接击败了 Claude Fable 5** 拿下第一。GPQA Diamond 93.5%、Terminal-Bench 2.1 88.3%、BrowseComp 91.2% 均为开源新高。

价格上更加"击穿"：$0.30/M cache-hit 输入、$3/M 未命中、$15/M 输出，对比 Fable 5 的 $10/$50、Sonnet 5 的 $2/$10（月末涨到 $3/$15），K3 在长上下文场景的实际成本可能只有闭源前沿的三到五成。

对开源生态最大的信号是"美国计算封锁没有阻止 SOTA 前进"。K3 训练用的是国产/海外混合算力，Moonshot 在没有 H100 完整供货的情况下仍造出了 2.8T 权重——这对下一轮出口管制博弈的说服力已经在削弱。同时它也让 Meta 的开源霸主地位彻底动摇：Meta 本周刚刚被迫把 Muse Spark 转闭源，而 Moonshot 却把 Llama 家从未做到过的开源天花板抬到新高。

**点评：** 前沿模型开源的战场已经从"美国是否愿意开"变成"中国能否持续供得起"，K3 至少让下一年 12 个月的开源 SOTA 曲线继续向上。

---

### ⚡ No.3 · Google Gemini 3.5 Pro 今日 GA，直接进价格战

**[Distill Intelligence](https://www.distillintelligence.com/briefings/ai-leaders-2026-07-17) · [MindStudio](https://www.mindstudio.ai/blog/google-vs-openai-vs-anthropic-momentum-2026-narrative)**

按泄露的发布计划，Gemini 3.5 Pro 今日（7/17）转 GA：2M token 上下文、Deep Think 推理模式独占 $250/月 Ultra 订阅、API 定价 $1.25 输入 / $10 输出。Google 官方尚未官宣具体日期，但 API 层已经开始灰度。上下文窗口继续维持 Google 的独家优势（Anthropic Sonnet 5 长上下文 200K、OpenAI Sol 系列 1M），2M 主打企业级 codebase / 长文档场景。

值得注意的是定价 —— 这直接把 Google 拉进了 Meta Muse Spark 1.1（$1.25/$4.25）挑起的价格战阵营。输入侧 Google 与 Meta 完全对齐，输出侧凭长上下文 + Deep Think 单独收溢价，属于典型的"入口白菜价、能力档次差异化收钱"。

叠加 Google Cloud Next '26 上刚发布的 Gemini Enterprise 统一 Agent 平台，Google 想传达的信号很清楚：不打模型 benchmark 榜战（Fable 5 已经拿走这一面旗），而是主打"上下文最长 + Agent 平台最完整 + API 价格最合理"这条组合拳。

**点评：** Gemini 3.5 Pro 说明 Google 已经放弃与 Claude / GPT 拼单点 benchmark，转身押平台与价格；这是过去两年内 Google 第一次拿出真正"打折"的商务姿态。

---

### 💥 No.4 · Apple 起诉 OpenAI + io Products：AI 硬件战撕破脸

**[CNN](https://www.cnn.com/2026/07/10/tech/apple-openai-devices-lawsuit) · [Bloomberg](https://www.bloomberg.com/news/articles/2026-07-10/apple-sues-openai-for-trade-secret-theft-in-blockbuster-case) · [TechCrunch](https://techcrunch.com/2026/07/13/the-wildest-allegations-in-apples-trade-secrets-lawsuit-against-openai/)**

诉状 7 月 10 日提交、经过一周挖料后本周继续发酵。Apple 声称 OpenAI 从技术员到硬件负责人 Tang Tan（前 iPhone/Apple Watch 硬件掌门人）"从每一层"系统性窃取商业机密：前 Apple 工程师 Chang Liu 下载了数十份未发布产品的详细文档；OpenAI 面试环节要求候选人"带 Apple 实物零件来做 show and tell"；甚至有一份印有 "Need to Know" 标签的内部文件被 OpenAI 发给新员工，教他们"如何避开被立即劝退（walkout）的程序"。诉状同时把 Jony Ive 的 io Products 列为共同被告。

这场官司实质是 2024 年 Apple ↔ OpenAI 合作蜜月的彻底破裂。Apple 押注 Vision Pro 之后的下一款设备为"AI 原生硬件"，OpenAI 也在准备 2026 年发布消费级 AI 音箱与 Ive 团队设计的可穿戴设备，两条硬件产品线开始正面撞车。分析师普遍认为诉讼将拖慢 OpenAI 硬件发布节奏，同时给 Apple 自研生成式 AI 争取时间。

**点评：** 两年前"合作"、今天"互告"——AI 与消费电子的估值天花板正在收敛，Apple 已经把 OpenAI 视为主线业务级别的战略对手，而不是 Siri 的外挂。

---

### 💰 No.5 · Meta Muse Spark 1.1 + Meta Model API 挑起价格战

**[Crypto Briefing](https://cryptobriefing.com/meta-ai-pricing-strategy-developers/) · [The New Stack](https://thenewstack.io/openai-spacexai-meta-price-war/)**

Muse Spark 1.1 于 7 月 9 日进入 public preview，同步 Meta 首个"付费闭源"API——$1.25/M 输入 + $4.25/M 输出，比同档 GPT-5.6 Terra 便宜约 25%。24 小时内 OpenAI 与 SpaceXAI（Grok 4.5）纷纷跟进降价。Meta 这一步的战略含义是它承认 **"给开源大模型免费无止境"已经不可持续**，转身走"付费闭源 + 免费低阶开源"两条腿。

推理效率而非 benchmark 榜首成为新的战场坐标。K3 拿开源天花板、Sonnet 5 拿 benchmark 天花板、Meta 拿定价地板——三种打法组合下，2026 年 H2 的 API 单价可能整体再下沉 30-50%。这对下游 SaaS/Agent 应用是巨大红利，但对 OpenAI 的 IPO 估值叙事却是重大压力：一旦价格战常态化，$25-33B 的 ARR 增速能否续命就成问题。

**点评：** Meta 转身收钱、Google 打折促销、OpenAI 面临 Apple 官司 + IPO 窗口窄化，这个季度的钱袋子逻辑正在改写：谁 tokens 卖得最多不再重要，谁 tokens 单位成本最低才是新的王座。

---

## 行业观察

**竞争格局的三条主线在同一天集中显影：**

第一，**"两阵营"化**正式落地——WAICO vs Pax Silica、开源 vs 闭源、中式治理 vs 美式治理、发展中国家 vs 发达国家算力供给，这些切分线过去 12 个月一直在移动，今天以 29 vs 35 的具体数字锁定。未来 6 个月 UN AI 治理谈判的每一个提案，都可能被贴上阵营标签。

第二，**开源的领导者从 Meta 换成 Moonshot**。Meta 转闭源、Thinking Machines 主打"可定制而非最强"、Anthropic/OpenAI 从未真正开源，2.8T 的 Kimi K3 成为开源社区新旗帜。中国出口开源大模型 + 便宜推理算力，将成为下一年 Global South 市场的默认组合。

第三，**API 定价加速下沉**。Sonnet 5 的 $2/$10、Muse Spark 的 $1.25/$4.25、K3 的 $0.3 cache-hit、Gemini 3.5 Pro 的 $1.25/$10——本季度头部模型 API 均价至少下降 30%。这直接把 AI 应用层的毛利与推理层的毛利同时压薄，Agent / SaaS 生态今年 Q4 会看到大规模的商业模式重构。

**监管与硬件同时进入下一阶段：** 白宫下周将公布与三大前沿实验室敲定的自愿发布标准，Apple 用官司为自研 AI 硬件争取时间，Anthropic 与 Blackstone 押注"AI 实施层"下一个万亿美元赛道——这些都指向同一个结论：模型层的战局在收敛，接下来的估值增量将从模型转移到"分发（硬件/平台/实施）"这条链。
