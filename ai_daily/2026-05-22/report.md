# AI 每日资讯 · 2026-05-22

## 今日焦点

> **算力军备升级 · 顶级人才大迁徙 · AI 攻克数学未解之谜 · 白宫监管摇摆 · Anthropic 即将首次盈利**
>
> - **Anthropic 与 xAI 签 1.25 亿美元/月超级算力合同**，独占 Colossus 1+2，三年合计 400 亿美元，正式与 OpenAI / Google 形成算力三足鼎立。
> - **Andrej Karpathy 加盟 Anthropic 预训练团队**，将主导"用 Claude 加速 Claude 训练"的自我递进研究，被视为 AI 人才战的标志性事件。
> - **OpenAI 内部模型自主攻克 Erdős 80 年单位距离猜想**，由 Tim Gowers 等真人数学家审核通过，AI 首次独立解决一个学科中心难题。
> - **Trump AI 行政令最后时刻被叫停**，"模型发布前 90 天交政府审查"的自愿性框架仍在拉锯中，监管节奏陷入摇摆。
> - **Anthropic Q2 营收预期 109 亿美元、首度季度盈利 5.59 亿**，IPO 传闻和"会计游戏"质疑同步发酵。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Anthropic 与 xAI 签 1.25 亿美元/月算力合同，三年 400+ 亿 | TechCrunch / Axios | ⭐⭐⭐⭐⭐ |
| 2 | OpenAI 模型自主推翻 Erdős 80 年几何猜想，Fields 奖得主验证 | OpenAI / TechCrunch | ⭐⭐⭐⭐⭐ |
| 3 | Andrej Karpathy 加盟 Anthropic 预训练团队 | TechCrunch / CNBC | ⭐⭐⭐⭐⭐ |
| 4 | Google I/O 2026 发布 Gemini 3.5 Flash 和 Spark 个人 Agent | TechCrunch / CNBC | ⭐⭐⭐⭐ |
| 5 | Anthropic Q2 营收预计 109 亿美元，有望首次季度盈利 | CNBC / TechCrunch | ⭐⭐⭐⭐ |
| 6 | Trump AI 行政令签署被推迟，"90 天预审"框架仍在博弈 | CNN / Axios | ⭐⭐⭐⭐ |
| 7 | SpaceX 提交 S-1 招股书，披露 xAI 与 Anthropic 大单 | Axios | ⭐⭐⭐⭐ |
| 8 | OpenAI 年化营收突破 250 亿美元，最快 2026 年底 IPO | 多家 | ⭐⭐⭐⭐ |
| 9 | Microsoft、Google、xAI 同意政府对 AI 模型进行预发布测试 | CNN Business | ⭐⭐⭐ |
| 10 | Gemini 3.5 Flash 在 Antigravity、Gemini Enterprise 全量开放 | Google Cloud Blog | ⭐⭐⭐ |
| 11 | 美国各州层面 1200+ AI 法案缺统一标准 (CA SB 53 / NY RAISE / TX TRAIGA) | Fortune | ⭐⭐⭐ |
| 12 | Fazeshift 完成 2200 万美元融资，AI 应收账款自动化 | 多家 | ⭐⭐⭐ |
| 13 | Orkes 完成 6000 万美元融资，AI 工作流编排 | 多家 | ⭐⭐⭐ |
| 14 | Agentic AI 预计占 2026 年企业 IT 支出 10-15% | Brookings | ⭐⭐⭐ |
| 15 | 加密圈热议 Anthropic 估值或超越 OpenAI | Seoul Economic | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Anthropic 砸 1.25 亿美元/月 锁定 xAI Colossus 全部算力

**[TechCrunch](https://techcrunch.com/2026/05/20/anthropic-will-pay-xai-1-25-billion-per-month-for-compute/) · [Axios](https://www.axios.com/2026/05/20/anthropic-spacex-compute)**

随着 SpaceX 提交 S-1 招股书，Anthropic 与 xAI 之间的"世纪算力合同"终于浮出水面：Anthropic 将以 **每月 12.5 亿美元** 的固定价租用 Colossus 1 数据中心**全部 300 兆瓦、22 万张 NVIDIA GPU（H100/H200/GB200 混编）**，合同至 2029 年 5 月，总价超 **400 亿美元**；同时即将扩张至 Colossus 2。

这笔交易颠覆了 AI 产业既有的算力供给格局。过去 18 个月，市场普遍认为 OpenAI 绑定微软、Anthropic 绑定 AWS+Google。但 AWS 自研 Trainium 进度迟滞、Google TPU 优先内部使用，Anthropic 急需"政治中立 + 现货充足"的第三方算力。Colossus 既有 GB200 现货，又能在 Memphis 接入南方电网的便宜电价，是当下唯一能消化 Claude Pro / Max 暴涨流量的硬通货。

更微妙的是，**这是 Anthropic 公开向 Elon Musk 的 xAI"输血"**。表面看是竞争对手互利，深层来看，Anthropic 用一份长合同把 xAI 推上 IPO 跑道，而 xAI 则换得现金流稳定模型训练投入 —— 双方默契对抗 OpenAI 算力护城河。

**点评：** 当 Claude 的最大算力供应商变成"竞争对手的兄弟公司"时，AI 行业的敌我界限已彻底重构 —— 算力，而非模型，正在定义 2026 年的真竞争格局。

---

### 🚀 No.2 · OpenAI 模型自主推翻 Erdős 80 年单位距离猜想

**[OpenAI 官方](https://openai.com/index/model-disproves-discrete-geometry-conjecture/) · [TechCrunch](https://techcrunch.com/2026/05/20/openai-claims-it-solved-an-80-year-old-math-problem-for-real-this-time/)**

OpenAI 周三宣布：一款**未经数学专项训练**的通用推理模型，独立给出了对 Erdős 1946 年提出的"平面单位距离问题"长期猜想的反证，构造出了一族比"正方形网格"更优的点阵排布，并完成完整可验证证明。**Fields 奖得主 Tim Gowers 及多位外部数学家审稿确认。**

这是 AI 首次在没有人类提示策略、没有专门 scaffold 的情况下，**独立解决一个学科核心未解难题**。模型使用了代数数论中的高阶工具完成构造，过程中体现出"自发的研究品味"——选对了变换族、选对了证明路径。

意义有两层：第一，AI 进入了"原创发现"区间，比"刷竞赛题"和"形式化辅助"高一个量级；第二，OpenAI 在产品端被 Anthropic / Google 紧逼的当口，用基础研究的"硬通货"重新定义自己的护城河 —— 数学发现可以直接转化为生物、材料、密码学的发现链路。

**点评：** 这不是 AGI 的烟雾弹，而是真正的拐点信号 —— 如果一款模型能在 Erdős 猜想上做对一次，那么蛋白质设计、密码学构造、芯片新算法上的第二次第三次只是时间问题。

---

### 🧲 No.3 · Karpathy 加盟 Anthropic 预训练团队，"用 Claude 训练 Claude"

**[TechCrunch](https://techcrunch.com/2026/05/19/openai-co-founder-andrej-karpathy-joins-anthropics-pre-training-team/) · [CNBC](https://www.cnbc.com/2026/05/19/anthropic-hires-openai-cofounder-andrej-karpathy-former-tesla-ai-lead.html)**

OpenAI 联合创始人 Andrej Karpathy 周二在 X 上宣布，本周入职 Anthropic 预训练团队，并将牵头一个全新方向：**让 Claude 来加速 Claude 自己的预训练研究**。这是 AI 工程自动化最具象征意义的"自递归"实验。

Karpathy 的标志意义远大于工程价值。过去三年，OpenAI 主导的"前 OpenAI 系叙事"被打破：Ilya Sutskever 自立门户做 SSI、Mira Murati 创办 Thinking Machines，如今 Karpathy 又选择竞争对手 Anthropic。**OpenAI 的人才品牌正在被稀释**，而 Anthropic 正从"OpenAI 旁支"变成"AI 安全派 + 顶级研究员聚集地"。

Karpathy 自己强调：他相信"未来几年是 LLM 前沿研究最具塑形性的窗口期"，这是一句押注 —— 押注下一代飞跃不会在产品层发生，而在预训练和数据工程的微观重构里。

**点评：** 顶级研究员的脚投票，比任何 benchmark 都更有信息量；Anthropic 不只要追上 OpenAI，更要做"研究员心目中那家公司"。

---

### 📱 No.4 · Google I/O 2026：Gemini 3.5 Flash + Spark Agent 全线押注 Agentic AI

**[TechCrunch](https://techcrunch.com/2026/05/19/with-gemini-3-5-flash-google-bets-its-next-ai-wave-on-agents-not-chatbots/) · [CNBC](https://www.cnbc.com/2026/05/19/google-ai-ultra-gemini-spark-omni.html)**

Google I/O 2026 没有发布 Gemini 4 旗舰模型，而是反向选择 **"小而快"路线**：Gemini 3.5 Flash 在编码和 Agent benchmark 上超过 Gemini 3.1 Pro，运行速度 **4 倍于同级前沿模型**。配套推出的 Gemini Spark 是 7×24 小时跑在 Gemini App 里的个人 AI Agent，先向 AI Ultra 订阅用户开放。

Google 的战略意图清晰：**不再用"通用大模型"和 OpenAI 拼参数，而是用"Agent 调用经济学"重构竞争**。Flash 的低 latency、低成本让 Agent 任务可以"长链路、多步骤、低单价"，正是 Anthropic 用 Sonnet 打的同一张牌，但 Google 多了 Workspace / Search / Android 整套分发。

Spark 是 Google 把 Gemini 从"输入框"扩展到"后台守护进程"的关键一步 —— 即便用户不主动唤起，AI 也会管理日程、邮件、研究任务。这是 Apple Intelligence 一直没做成的事，Google 借 Android 14.1 直接推到几亿设备上。

**点评：** Google 不再追前沿模型分数，而是用"Flash + 全平台分发"打 Agent 普及战 —— 这条路一旦跑通，OpenAI 的"模型即产品"叙事将被彻底颠覆。

---

### 💰 No.5 · Anthropic 即将首次盈利 vs SpaceX 大单的"会计魔术"质疑

**[CNBC](https://www.cnbc.com/2026/05/20/anthropic-revenue-explosive-growth-ipo-profitable-quarter.html) · [TechCrunch](https://techcrunch.com/2026/05/20/anthropic-says-its-about-to-have-its-first-profitable-quarter/)**

Anthropic 内部数据显示 Q2 营收预计 **109 亿美元**（Q1 为 48 亿，环比 2 倍以上），**预计运营利润 5.59 亿美元**，将是公司成立 5 年来首个季度盈利。如果属实，估值有望突破 OpenAI。

但 _Where's Your Ed At_ 等媒体迅速指出：所谓"利润"只是 **训练成本入账、剔除股权激励** 后的口径；且 SpaceX 合同前两个月有折扣价，恰好压住 Q2 支出。**这不一定是真盈利，更像是 IPO 路演前的"漂亮报表"**。

无论真假，市场反应已经很明确：Anthropic 已经从"OpenAI 的更安全的影子"变成"营收增速更快、客户更黏的对手"，企业 API 市场的份额拉锯仍将继续。

**点评：** 把"会计利润"包装成"商业模式跑通"是 AI 公司 IPO 老剧本，但 Q2 这份数据至少说明一件事 —— 企业愿意为 Claude 付的钱已经追上了 OpenAI 的脚步。

---

## 行业观察

今天的几条新闻拼成一张完整的 2026 AI 行业图：**算力垄断重排**（Anthropic-xAI 大单）、**基础研究破局**（OpenAI 攻克 Erdős）、**顶级人才再分配**（Karpathy 跳槽）、**Agent 路线确立**（Google Spark）、**商业模式落地**（Anthropic 盈利）。这五件事同时发生在 72 小时内，标志着 AI 行业从"模型军备竞赛"转向"全要素卡位战"——谁握住更便宜的算力、更聪明的研究员、更黏的 Agent 入口、更稳健的现金流，谁就能在 2027 年的下一轮卡位中胜出。

监管端则呈现耐人寻味的"自愿协商"状态：Trump 行政令推迟、CA/NY/TX 各州法案纷飞，企业既不想被"90 天预审"卡脖子，又不愿被各州碎片化合规拖死，最终大概率走向"联邦自愿框架 + 州级强制条款"的混合模式。**接下来 90 天，监管谈判将和算力大单一样塑造 AI 产业的下一阶段格局。**
