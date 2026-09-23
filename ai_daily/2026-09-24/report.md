# AI 每日报告 · 2026-09-24

## 今日焦点

> **Sora API 正式停摆 · 联合国安理会首启中美 AI 峰会 · 加州 SB53 倒计时 · 机器人开源生态提速 · Anthropic 系创业者接连套现**
>
> - **OpenAI Sora API 今日全面下线**，Sora 2/Sora 2 Pro 开发者端点终结，官方以"经济性不佳、版权困境未解"给出体面收尾。
> - **联合国安理会 9 月 23 日召开 AI 与国际安全专场**，Sam Altman、Anthropic、DeepSeek、Moonshot 同场同台，中美前沿实验室首次被拉进多边治理桌面。
> - **加州 Frontier AI Safety Act 进入 9 月 30 日决断窗口**，纽森手中的这支笔可能重画美国联邦/州权博弈的分水岭。
> - **Alphabet Intrinsic 在 ROSCon 2026 开源 Intrinsic Core**，Apache 2.0 的 ROS 兼容运行时把大厂级机器人栈直接甩进社区。
> - **前 Anthropic 研究员创业公司 Mirendil 6 个月拟融 10 亿美金**，估值 50 亿美金，AI 顶尖人才价签再次被重新校准。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | OpenAI 正式停用 Sora API，视频生成开发者接口今日关停 | OpenAI Help / TechCrunch | ⭐⭐⭐⭐⭐ |
| 2 | 法国主持联合国安理会首个 AI 与国际安全部长级会议，中美前沿实验室同场亮相 | AI Weekly | ⭐⭐⭐⭐⭐ |
| 3 | 加州 Frontier AI Safety Act 面临 9/30 签署或否决截止日 | Cubbbix / 政策观察 | ⭐⭐⭐⭐⭐ |
| 4 | Alphabet Intrinsic 在 ROSCon 2026 开源 Intrinsic Core（Apache 2.0） | AI Weekly | ⭐⭐⭐⭐ |
| 5 | Mirendil（前 Anthropic 研究员团队）洽谈 10 亿美金融资，估值 50 亿美金，Kleiner 领投 | AI Weekly | ⭐⭐⭐⭐ |
| 6 | AI 云新星 Verda 完成 1.89 亿美元融资，Emergence Capital 领投，估值 ≥10 亿美金 | Bloomberg | ⭐⭐⭐⭐ |
| 7 | AI 药物发现公司 Basecamp Research 完成 1.4 亿美元 C 轮，Nvidia、Anthology Fund 参投 | SiliconANGLE | ⭐⭐⭐⭐ |
| 8 | xAI Grok Bot 周活突破 41.8 万，环比再增 24% | AI Weekly | ⭐⭐⭐ |
| 9 | OpenAI GPT-6 Sol / Luna 上线（9-22），主打低成本与更低幻觉率 | TechCrunch | ⭐⭐⭐⭐ |
| 10 | Nvidia + Microsoft + Anthropic 三方 300 亿美金 Azure 训练协议进入落地阶段 | AI Business / Bloomberg | ⭐⭐⭐⭐ |
| 11 | EU AI Act Article 50 透明度义务与 EU AI Office 执法权已于 8-2 全面激活 | European Commission | ⭐⭐⭐⭐ |
| 12 | Nvidia 收购 Hugging Face 129.3 亿美金交易文件递交 SEC，预计 2027H1 关闭 | Yahoo Finance / SEC 8-K | ⭐⭐⭐⭐ |
| 13 | Anthropic Claude Fable 5.1 缓存读取降价 75%，Enterprise Frontier Safeguards 正式上线 | VentureBeat | ⭐⭐⭐ |
| 14 | Summer 2026 AI Safety Index 覆盖 9 家实验室 37 项指标，评级差距进一步拉大 | Future of Life Institute | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Sora API 今日正式下线：一款开山之作的体面退场

**[OpenAI Help Center](https://help.openai.com/en/articles/20001152-what-to-know-about-the-sora-discontinuation)** · **[TechCrunch](https://techcrunch.com/2026/03/24/openai-discontinue-sora-video-app)** · **[Axios](https://www.axios.com/2026/03/24/openai-discontinue-sora-video-app)**

OpenAI 在今日（9 月 24 日）正式关停 Sora 2 及 Sora 2 Pro 的 API 端点，这是继 4 月 26 日 Sora 消费者应用下线之后的最后一步。今年 3 月 24 日 OpenAI 已经预告了这一天，理由主要是三条：单帧推理成本长期高企、收入始终追不上算力开销，以及肖像权/版权诉讼包袱越来越沉。

对生态而言，这不是"视频模型不行了"，而是"OpenAI 决定把视频这块产品收缩回内部"。真正取而代之的，是它把资源全部倒向 Agent 与代码这两个能付真金白银的场景——GPT-6 Sol / Luna 就在 9-22 才刚刚拉起以 Agent 为主轴的定价体系。Runway、Pika、LumaLabs、Kuaishou 可灵、字节即梦几家反而将在接下来的一个季度里享受一段没有 OpenAI 陪跑的窗口期。

需要关注的：一是所有存量客户是否顺利完成迁移，Sora 内容导出上限 9 月内到期；二是 OpenAI 是否会以完全不同的产品形态（比如 Agent SDK 内的多模态子模块）回归视频赛道。

**点评：** 认赔离场往往比继续硬撑更需要企业级别的克制。Sora 的收摊说明 2026 的 AI 产品经济学正在收紧——只烧算力、无法把用户价值折成 ARR 的方向，第一个被砍。

---

### 🚀 No.2 · 联合国安理会首开 AI 专场：多边治理终于坐进同一间会议室

**[AI Weekly](https://aiweekly.co/ai-news-today)** · **[Global Call for AI Red Lines - Wikipedia](https://en.wikipedia.org/wiki/Global_call_for_AI_red_lines)**

9 月 23 日，法国主持的 15 席安理会部长级会议以"AI 与国际安全"为唯一议题召开。这是安理会史上首次以 AI 为主线议题，也是**首次让美国 OpenAI/Anthropic 与中国 DeepSeek/Moonshot 出现在同一桌讨论前沿模型的红线**。会议直接对接 9 月启动的"Global Call for AI Red Lines"倡议，试图在生物、核、认知战三条底线上形成不受地缘冲突干扰的最小共识。

这场会议本身不会产出有约束力的决议，但它释放了两个信号：其一，AI 治理的重心正在从"技术团体自律 + 双边协议"上移到"联合国框架下的多边协议"，其二，中美前沿实验室已经默认必须承担一部分"半国家责任"，无论他们的 CEO 情不情愿。

**点评：** AI 曾经躲在硅谷会议室里谈治理，如今被架到了纽约东河边。这不是外交表演——这是 2027 年任何一份前沿模型 System Card 都必须回应的第一份问卷。

---

### 🏛️ No.3 · 加州 SB53：纽森的这支笔可能重画美国 AI 联邦/州权分水岭

**[Cubbbix Regulation Tracker](https://cubbbix.com/blog/ai-regulation-september-2026-global-update)** · **[Transcend AI Regulation Overview](https://transcend.io/blog/ai-regulation)**

Frontier AI Safety Act（SB 53 系列）已经送到纽森州长桌上，他必须在 9 月 30 日之前签字或否决。这份法案的关键条款包括强制风险评估披露、SSP（System Safety Plan）备案、以及对训练超过特定 FLOPs 的模型强制第三方评估。

法案背后是一场清晰的地缘博弈：联邦层面因参议院分歧迟迟没有推出统一 AI 法案，加州、纽约、科罗拉多等大州开始各自为政。若纽森签字，加州将成为**全球第二个具备实际处罚牙齿的前沿 AI 法域**（欧盟已于 8 月 2 日激活）；若否决，硅谷会松一口气，但联邦层面会更紧迫地推动 preemption 立法。

值得同步注意的是，科罗拉多 SB24-205 的审计细则也在本季度落地，AI 合规团队 Q4 会异常忙。

**点评：** 2026 已经不是"是否监管"的问题，而是"谁先出手、谁定义标准"的问题。加州这一枪要么打醒美国国会，要么直接把加州变成 AI 版的 CCPA。

---

### 🤖 No.4 · Intrinsic Core 开源：谷歌把机器人栈从 Robot-as-a-Service 拉回开源常识

**[AI Weekly](https://aiweekly.co/ai-news-today)**

Alphabet 旗下 Intrinsic 在 ROSCon 2026（多伦多）宣布，将其内部机器人运行时 Intrinsic Core 以 Apache 2.0 协议开源。Intrinsic Core 支持硬件无关的实时控制、位姿估计、抓取规划、仿真 / 标定服务，以及原生的 Intrinsic-ROS 驱动。这意味着任何一家机器人初创公司，都可以在**同一天**得到一套接近 Google 内部标准的机器人栈起点。

这次开源发生在 Figure、1X、Physical Intelligence（Pi）迅速拉开身位、真实机器人 Foundation Model 全面进入商业化的窗口期。Intrinsic 显然是在用"开源打法"换社区的模型和数据反哺，同时向 ROS 社区宣示 Google 系机器人栈的正统地位。

**点评：** 大模型的开源仗还没打完，机器人栈的开源仗又开一枪。真正稀缺的不再是"能跑的运行时"，而是"能被跑通的数据集"和"能被信任的安全策略"。

---

### 💰 No.5 · Mirendil：Anthropic 出身的团队再次证明"顶尖研究员就是硬通货"

**[AI Weekly](https://aiweekly.co/ai-news-today)** · **[Basecamp Research 融资背景](https://siliconangle.com/2026/09/23/ai-drug-discovery-startup-basecamp-research-raises-140m/)**

成立仅 6 个月、由前 Anthropic 研究员创办的 Mirendil，正在与 Kleiner Perkins 领投的投资方洽谈 10 亿美元融资，估值 50 亿美元。团队 20 人，全部来自 Anthropic、xAI、DeepMind、OpenAI。同一日 AI 医药初创 Basecamp Research 完成 1.4 亿美元 C 轮，由 S32 领投，Nvidia 与 Anthropic × Menlo 的 Anthology Fund 跟投——**Anthropic 系资本-人才双向流动**成为 2026 年 AI 生态最具辨识度的图案。

对市场而言，这类"高估值 / 无产品"的融资再现，说明 2026 秋季的资金氛围仍偏 risk-on，同时也说明现有大厂研究员的机会成本（相对期权池）已经达到临界点。9 月早些时候的另一大数据点是：Cognition 20 亿美金融资、估值 480 亿美金；Mistral 30 亿欧元融资。

**点评：** 顶尖研究员的边际产出还没被 Scaling Law 追平之前，"人"仍然是 AI 产业最贵、也最容易 IPO 的资产类别。

---

## 行业观察

**主题一：产品经济学与算力经济学开始短兵相接。** Sora 的谢幕、OpenAI 主推 GPT-6 Sol/Luna 的定价策略、Anthropic Fable 5.1 缓存读取降价 75%，都是同一个方向：模型厂商在有意压缩长上下文和 Agent 场景下的边际成本，而砍掉那些看不到 ARR 的实验产品。视频、语音、图像这些烧钱重灾区，接下来大概率会看到更多"收缩到内部工作流"的动作。

**主题二：治理主战场正在从欧盟走向多边。** EU AI Act Article 50 已经实打实落地、罚款最高 1500 万欧元或 3% 全球营收；美国州法（加州 SB53、科罗拉多 SB24-205）齐头并进；联合国安理会开始"直接面对"前沿实验室。2027 年若要在美国、欧盟、中国同时部署一款前沿模型，其合规文档量会比 2025 翻一倍不止。

**主题三：机器人和生物医药正在成为下一波"AI 原生"融资的主战场。** Intrinsic Core 开源、Basecamp Research EDEN 280 亿参数医学基础模型、Figure/Pi 的持续爆量融资，说明纯语言模型之外的两条主线——**物理 AI**与**生命科学 AI**——正在快速成为顶级 VC 押注的第二增长曲线。Nvidia 同时收购 Hugging Face + 支持 Basecamp + 深化 Anthropic 合作的三段动作，把它自己变成了这场基础设施战争中唯一同时押三条战线的选手。

**主题四：Anthropic 生态开始横向繁殖。** 从 Fable 5.1 的企业级安全架构 EFS，到 Anthology Fund 跟投 Basecamp，再到 Mirendil、Cognition 这类"离职即融资"团队，Anthropic 正在悄悄建立类似早期 PayPal Mafia / OpenAI Mafia 的第三代 AI 人才网络——2027 年 AI 独角兽榜单里，"前 Anthropic 员工"很可能会是最常见的 tag。
