# AI 行业日报 · 2026-06-11

## 今日焦点

> **SpaceX/xAI IPO 定价日 · Apple 打开 Siri 第三方 AI 市场 · Anthropic 估值狂飙至 9650 亿 · 监管全球收紧 · Vera 平台量产**
>
> - **史诗级 IPO 今晚定价** SpaceX 含 xAI 业务今晚收市后以每股 $135 定价，估值约 **1.75 万亿美元**，明日纳斯达克挂牌，刷新人类历史最大 IPO 纪录。
> - **iOS 27 终结 ChatGPT 独占** Apple WWDC26 宣布 Extensions 框架，用户可把 **Claude / ChatGPT / Gemini / Grok** 设为 Apple Intelligence 默认模型，Siri 由 Gemini + 私有云算力驱动。
> - **Anthropic 估值碾压 OpenAI** Series H 以 9650 亿美元 post-money 收官，ARR 达 **$47B**（2 月还只有 $14B），秘密提交 IPO 文件、最快 10 月挂牌。
> - **欧盟 AI Act 8 月 2 日全面生效倒计时** 高风险系统义务已在 5 月落地，距通用条款全面适用仅剩 50 余天，合规窗口骤紧。
> - **Anthropic 呼吁全行业暂停** Jack Clark 公开倡议头部实验室协调放缓前沿训练；OpenAI 反对自我设限，转而呼吁建立"国际 AI 监管机构"。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | SpaceX (含 xAI) 今晚定价 $135 / 估值 $1.75 T，明日 SPCX 上市 | CNBC / WEEX | ⭐⭐⭐⭐⭐ |
| 2 | Apple WWDC26：iOS 27 Extensions 开放 Claude/ChatGPT/Gemini 替换 Siri | TechCrunch / AI Weekly | ⭐⭐⭐⭐⭐ |
| 3 | Anthropic 9650 亿估值收官 Series H，ARR 47B，秘密递 IPO | Crescendo / blog.mean.ceo | ⭐⭐⭐⭐⭐ |
| 4 | Claude Fable 5 上线，首款 "Mythos-class" 前沿模型 | Anthropic / Wikipedia | ⭐⭐⭐⭐ |
| 5 | Nvidia Vera CPU 全量产，Anthropic/OpenAI/xAI 首批客户 | NVIDIA Blog | ⭐⭐⭐⭐ |
| 6 | Microsoft Foundry 模型库扩至 11,000+，含 GPT-5.5/Opus 4.8/Gemini | CNBC / Build 2026 | ⭐⭐⭐⭐ |
| 7 | OpenAI 发布 GPT-Rosalind 生命科学专用模型 | Releasebot | ⭐⭐⭐⭐ |
| 8 | GPT-5.5 Instant 向全体 ChatGPT 用户推送 | OpenAI Help Center | ⭐⭐⭐ |
| 9 | Anthropic 公开呼吁前沿实验室协调暂停训练 | Al Jazeera | ⭐⭐⭐⭐ |
| 10 | OpenAI 反提"国际 AI 监管机构"方案 | Gizmodo | ⭐⭐⭐ |
| 11 | EU AI Act 距 8 月 2 日全面生效仅 50 余天 | EU Digital Strategy | ⭐⭐⭐⭐ |
| 12 | Google TurboQuant 算法 (ICLR 2026) 大幅压缩 KV cache | Crescendo | ⭐⭐⭐ |
| 13 | Google 与 SpaceX 签 $920M / 月算力长约 | TechCrunch | ⭐⭐⭐⭐ |
| 14 | MolmoAct 2 机器人模型，速度提升 37× | blog.mean.ceo | ⭐⭐⭐ |
| 15 | 中国 CAC 2 月新规：所有生成式 AI 强制安全审查 | utu.fi Insights | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · SpaceX-xAI 联体上市定价：1.75 万亿美元改写 IPO 历史

**[CNBC / TradingKey](https://www.cnbc.com/2026/06/03/spacex-ipo-stock-price-roadshow-musk.html)**

今晚收市后是马斯克帝国上市的关键时刻。SpaceX 将以每股 **$135** 固定价定价，发行 5.556 亿股，募资约 750 亿美元，承销商超额配售选择权再追加 112 亿。按完全摊薄计算，估值锁定在 **1.75–1.77 万亿美元** 区间，一举超越沙特阿美 2019 年 256 亿美元募资的纪录，成为人类历史上最大 IPO。

更重要的是 S-1 把公司切成三段：连接（Starlink）、太空（Falcon/Starship/Starshield）、**AI（xAI、Grok、X 平台、数据中心）**。这意味着 xAI 不再单独估值，而是作为整体一部分被打包进公募市场。短期看，这给二级市场提供了首个"AI + 卫星 + 防务"复合敞口，Goldman、摩根士丹利等承销团已圈定主流共同基金。长期看，这把马斯克从私募估值游戏里彻底解放——他获得了与 OpenAI 私募 + Anthropic 私募抗衡所必需的公开市场再融资通道。

**点评：** xAI 借着火箭一起上市，是 2026 年最骚的资本结构操作——把烧钱 AI 业务装进现金流强劲的航天平台里，公募投资者别无选择只能接受估值溢价。

---

### 🚀 No.2 · Apple WWDC26：iOS 27 Extensions 杀死单一 AI 供应商时代

**[TechCrunch](https://techcrunch.com/2026/06/09/wwdc-2026-everything-announced-on-siri-ai-os-27-apple-intelligence-and-more/) / [AI Weekly](https://aiweekly.co/node/2611)**

6 月 9 日 WWDC26 主旨演讲做了两件事：第一，**承认自研 Siri 失败**，转身与 Google 签约用 Gemini 给新 Siri 提供基础能力，并通过 Private Cloud Compute 隔离用户数据，Google 拿不到原文；第二，**开放 Extensions**——iPhone 用户可以在"设置 → Apple Intelligence"里把 Claude、ChatGPT、Gemini 或 Grok 设为系统级默认 AI，覆盖写作工具、总结、Siri 调度等所有 Apple Intelligence 功能。

这是 Apple 在 AI 时代第一次明确放弃"垂直一体化"原则。两年前 ChatGPT 是 iOS 18 唯一被点名的合作方，Sam Altman 站台；今年规则变成了"AI 市场化分发"，类似浏览器选择器。Anthropic 是最大赢家——iPhone 装机量瞬间为 Claude 打开了消费级最大入口，原先靠 API 和 Claude.ai 网站的高质量企业流量，现在叠上了 20 亿台终端的潜在订阅基础。

**点评：** Tim Cook 用一场发布会把"Apple Intelligence"变成"Apple AI Store"——Apple 不打造最好的模型，但要做最大的渠道商，这是软件帝国能想到的最稳的位置。

---

### 💰 No.3 · Anthropic 9650 亿估值收官，反超 OpenAI 成最高估值私募 AI 公司

**[Crescendo AI / Mean.ceo Funding Report](https://www.crescendo.ai/news/latest-ai-news-and-updates)**

5 月底关闭、6 月初对外披露的 Series H 让 Anthropic 私募估值蹿升到 **9650 亿美元**（post-money），超越 OpenAI 同期私募估值，成为全球最贵的独立 AI 公司。同期披露的关键数字更夸张：

- **运行率收入 (ARR) 从 2 月的 $14B 跳到 $47B**，236% 增长仅用 4 个月；
- **Q2 2026 预计实现 5.59 亿美元运营利润**，是公司有史以来首个正利润季度；
- **企业客户贡献 80% 收入**——这是与 OpenAI 最大的结构差异，OpenAI 的消费级订阅占比仍超 40%；
- **高盛、摩根大通、摩根士丹利已组团**承销 IPO，最快 10 月挂牌。

这意味着 AI 产业的资本权力格局再次翻转。一年前还是 OpenAI 单极，现在 Anthropic 用 Claude Opus 4.8 + Sonnet 4.6 + 新发布的 Fable 5 三梯队稳住了开发者市场份额，并把 Cursor、Replit、Vercel、Notion 等明星 SaaS 的底层模型几乎全部锁死。

**点评：** Anthropic 的 4 个月 3 倍 ARR 增长不是模型订阅红利，而是 Claude Code + Managed Agents 这类"代码 + 自动化"用例的爆发——这是 AI 真正进入企业生产环境的转折点。

---

### ⚖️ No.4 · Anthropic 呼吁全行业暂停 vs OpenAI 要"国际监管机构"——安全派路线分裂

**[Al Jazeera](https://www.aljazeera.com/economy/2026/6/5/anthropic-urges-ai-labs-to-pause-warns-humans-risk-losing-control) / [Gizmodo](https://gizmodo.com/openai-joins-anthropic-in-call-for-international-ai-watchdog-2000769442)**

6 月 5 日 Jack Clark 与研究院负责人 Marina Favaro 联名撰文，公开呼吁前沿实验室协调"暂停"高能力模型训练，理由是"对齐研究跟不上能力增长"。这是顶级实验室首次公开提出真正意义上的"产业自愿减速"提议。

OpenAI 当天给出截然不同的回应：**反对企业自我设限**，主张由"民主政府而非私营公司"设规，并联合 OpenAI、Anthropic、Google DeepMind、Microsoft 呼吁设立国际 AI 监管机构。背景是 3 月白宫《AI 国家政策框架》强调联邦先发制人 (federal preemption)，州级法规（科罗拉多 6 月底 AI 法、欧盟 8 月 AI Act 全面适用、中国 CAC 强制注册）持续加码，企业被迫在"自愿放缓"和"被规则驯化"之间选边。

**点评：** Anthropic 在估值最高点喊"暂停"，本质是用安全叙事再次拉开与对手的品牌差距——既能拿政府订单，又能让前沿对手承担道义成本。

---

### ⚡ No.5 · Nvidia Vera CPU 全量产，Anthropic/OpenAI/xAI 首批锁定

**[NVIDIA Newsroom](https://nvidianews.nvidia.com/news) / [NVIDIA Blog](https://blogs.nvidia.com/blog/nvidia-gtc-taipei-computex-2026-news/)**

Nvidia 在 Computex 2026 / GTC Taipei 宣布 **Vera CPU 进入全量产**，秋季交付，首批客户名单一字排开：**Anthropic、OpenAI、xAI（SpaceX）、Dell、Oracle、CoreWeave**——几乎覆盖全球前 6 大算力采购方。Vera 是 Vera Rubin 平台的 CPU 部分，官方数据称 token 吞吐速度比 x86 快 1.8 倍。同时 Spectrum-X Ethernet Photonics（CPO 共封装光学）也进入量产，第三代 MGX 机架 + 800V 直流供电组合成新一代 "AI factory" 蓝图。

更值得关注的是 **Google 与 SpaceX 5 日刚签下 $920M / 月** 的长期算力合约——这一方面说明 Google 自家 TPU 集群无法覆盖 Gemini 推理高峰，另一方面也意味着 SpaceX 的天基/地基数据中心战略已经吃到了头部 AI 公司的订单。Nvidia + SpaceX + 三大 AI 实验室构成一条"芯片—基础设施—模型"的资本闭环。

**点评：** 把 OpenAI、Anthropic、xAI 三个看似互斥的客户全部塞进 Vera 量产首发名单，Nvidia 在向资本市场宣告：模型层卷得越凶，黄仁勋赚得越多。

---

## 行业观察

**资本拐点已至：** SpaceX/xAI 公开市场上市 + Anthropic 估值反超 OpenAI 双事件叠加，标志 AI 产业从"少数私募估值游戏"切换到"主流二级市场配置"。下半年最重要观察变量是 Anthropic 10 月 IPO 路演定价，以及 OpenAI 是否被迫提前申报。

**渠道权力重新分配：** Apple iOS 27 Extensions 是分水岭——一旦消费者可以自由切换默认 AI，模型公司的护城河从"产品质量"重新回到"分发与数据循环"。Anthropic 借此获得 iPhone 入口，是其今天估值的最大隐藏期权。

**监管同步落地：** 欧盟 AI Act 8 月 2 日全面适用、美国白宫 3 月框架、中国 CAC 2 月新规、科罗拉多 6 月底 AI 法——四套规则在 6–8 月集中生效，所有跨国 AI 部署 SaaS 都将面临一次实质性合规压测，预计 Q3 引发一轮强监管驱动的产品下架与 SKU 重组。

**算力供应继续吃紧：** Vera 全量产 + Google-SpaceX 算力长约 + Spectrum-X CPO 出货意味着 AI 数据中心进入"工厂化扩张"阶段，但下游需求（GPT-5.5 推送、Claude Fable 5、Gemma 4 开放权重、Apple Intelligence Extensions）依然在指数式增长，2026 下半年 H 系列 / B 系列 GPU 仍将处于绝对短缺状态。

**安全叙事政治化：** Anthropic 的"暂停"提议与 OpenAI 的"国际监管"提议表面是路线之争，本质是头部公司在欧盟、美国联邦、白宫三方监管真空里抢占规则话语权。预计 Q3 一份联名版本的 "Frontier AI Safety Charter" 会出现，主导者大概率仍是 Anthropic。
