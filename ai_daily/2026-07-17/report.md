# AI 日报 · 2026-07-17

## 今日焦点

> **Gemini 3.5 Pro 正面亮剑 · 习近平首度出席 WAIC · 华为 Atlas 950 全球首秀 · Fable 5 定价拉锯战 · AI 投资 H1 破 5100 亿美元**
>
> - **Google Gemini 3.5 Pro 今日发布**：抛弃 2.5 Pro 架构从零重建，2M token 上下文 + Deep Think 推理层，对标 GPT-5.6 Sol 与 Anthropic Fable 5
> - **WAIC 2026 今日在上海开幕**：习近平首次亲自出席并作主旨演讲，中方推动"世界人工智能合作组织（WAICO）"落地上海
> - **华为 Atlas 950 SuperPoD 在 WAIC 全球首秀**：8192 张 Ascend NPU 组成单一逻辑计算机，FP8 算力达 8 EFLOPS，剑指 NVIDIA H100/B200
> - **Anthropic 三度延长 Fable 5 免费访问至 7 月 19 日**：Sonnet 5 以 $2/$10 的入门定价试图接住流量，Fable 5 定价 $10/$50 是 Opus 4.8 两倍
> - **OpenAI GPT-5.6 Sol 上线不到两周即触及容量上限**：Altman 警告"增长疯狂"、可能出现"hiccups"，54% token 效率提升换来指数级需求

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Google Gemini 3.5 Pro 今日正式发布，2M 上下文 + Deep Think 推理层 | BigGo Finance / Google | ⭐⭐⭐⭐⭐ |
| 2 | 习近平首次亲自出席 WAIC 2026 并作主旨演讲，力推"世界人工智能合作组织" | CGTN / SCMP | ⭐⭐⭐⭐⭐ |
| 3 | 华为 Atlas 950 SuperPoD 在 WAIC 展出，8192 张 Ascend 950，FP8 8 EFLOPS | Digitimes / Tom's Hardware | ⭐⭐⭐⭐⭐ |
| 4 | Anthropic 第三度延长 Fable 5 免费访问至 7 月 19 日，Sonnet 5 抢占中间市场 | The New Stack / TechTimes | ⭐⭐⭐⭐ |
| 5 | OpenAI GPT-5.6 Sol 需求暴涨触及容量上限，Altman 预警短期"hiccups" | Axios / CNBC | ⭐⭐⭐⭐ |
| 6 | EU AI Omnibus 协议达成：AI 沙盒截止推迟至 2027-08-02，透明度期限缩短至 3 个月 | Consilium / DLA Piper | ⭐⭐⭐⭐ |
| 7 | 全球 2026 H1 风险投资达 5100 亿美元创纪录，AI 占绝对主导 | Crunchbase | ⭐⭐⭐⭐ |
| 8 | Meta 扎克伯格发布 Muse Spark 1.1：1M token 上下文智能体模型，对标 GPT-5.5 与 Opus 4.8 | ThursdAI | ⭐⭐⭐ |
| 9 | 7 月 15 日单日 8 家 AI 初创融资 10.22 亿美元，Neko Health 领跑 7 亿 Series C | Yutori Scouts | ⭐⭐⭐ |
| 10 | Emergent 完成 1.3 亿 Series C，估值达 15 亿美元的"盒装工程团队" | Crunchbase News | ⭐⭐⭐ |
| 11 | 7 月 AI 智能体赛道融资 18 亿美元、12+ 笔交易，估值季环比涨 40% | AI Funding Insights | ⭐⭐⭐ |
| 12 | Altman 承认与 Lutnick、Bessent 就 GPT-5.6 发布进行多轮调整 | Bloomberg / Fortune | ⭐⭐⭐ |
| 13 | 华为公布南韩市场 4Q26 落地计划，Ascend 950PR 以 1/4 成本挑战 H20 | TrendForce | ⭐⭐⭐ |
| 14 | EU 委员会启动 AI 模型第三方评估能力建设，2027 年前可投入运行 | European Commission | ⭐⭐⭐ |
| 15 | ByteDance Seedream 与华尔街资金拥抱中国模型，推动"AI 两极化" | 综合报道 | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Google Gemini 3.5 Pro 今日正式发布——从零重建，直面 GPT-5.6 与 Fable 5

**[BigGo Finance / Google DeepMind](https://finance.biggo.com/news/6f0c6bb2-795f-4c57-9d09-6db691d7638a)**

Google 今日按计划推出 Gemini 3.5 Pro。与常规迭代不同，DeepMind 彻底放弃了 Gemini 2.5 Pro 的架构，从零重新设计以追赶 OpenAI 的 GPT-5.6 与 Anthropic 的 Fable 5。核心升级包括 2M token 上下文窗口、面向复杂问题的 "Deep Think 推理层"、以及被公司定义为"自主工作流"的原生 Agent 能力。

据泄露的定价信息，API 输入约 $1.25 / 百万 token，输出约 $10 / 百万 token，Deep Think 需订阅 $250/月的 Ultra 计划才能解锁。这个价格明显低于 Fable 5 的 $10/$50，也比 GPT-5.6 Sol 更具"生产就绪"的性价比感——Google 显然想在企业 Agent 场景抢回被 Anthropic 和 OpenAI 拿走的市场份额。

真正值得盯的是 Deep Think 的实际表现：在数学、SVG 生成、图像质量上，DeepMind 承诺"跨越式"提升。如果这次发布能拿下 GPQA / SWE-bench / ARC-AGI 三个关键榜单的头把交椅，Google 将首次在"顶级模型"话题上重新回到牌桌中央。

**点评：** Gemini 3.5 Pro 是 Google 一年内最重要的一次押注——如果 Deep Think 兑现承诺，OpenAI 的"高价 Sol"故事就要重新讲；如果没有，Google 就得开始正视"永远的追赶者"这个定位了。

---

### 🚀 No.2 · WAIC 2026 今日开幕：习近平首度亲临，中国推 "AI 版联合国"

**[SCMP](https://www.scmp.com/tech/article/3360404/xi-jinping-attend-world-ai-conference-first-time-china-elevates-tech-push) / [CGTN](https://news.cgtn.com/news/2026-07-13/Xi-to-attend-and-address-opening-ceremony-of-2026-World-AI-Conference-1OKgsIkkofu/p.html)**

WAIC 2026 上午在上海世博中心开幕。习近平自 2018 年 WAIC 创办以来首次亲自出席，并在开幕式与"全球人工智能治理高级别会议"上发表主旨演讲——中方将 AI 上升为国家最高优先级议题的信号非常明确。

大会规模空前：140+ 论坛、1,400 位嘉宾、1,100 家参展商、300+ 全球首发产品。中方希望本次会议推动"世界人工智能合作组织"（WAICO）总部落户上海，作为对西方主导的 AI 治理框架的对冲。

结合此前 ByteDance Seedream 火出圈、华尔街资金开始追捧中国 AI 模型的现象，2026 上半年的一个核心叙事被再次强化：**AI 已经是货真价实的"两极竞争"**——一极是美国生态（OpenAI/Anthropic/Google/Meta），一极是中国生态（阿里/字节/腾讯/DeepSeek + 华为算力栈）。

**点评：** 当最高领导人亲自站到 WAIC 讲台上，中国 AI 战略就从"发改委/工信部话题"升格为"总书记议程"——接下来一年，中方对芯片、模型出海、治理规则的动作会明显加速。

---

### 🥇 No.3 · 华为 Atlas 950 SuperPoD 全球首秀——8192 张 NPU，FP8 8 EFLOPS

**[Tom's Hardware](https://www.tomshardware.com/tech-industry/semiconductors/chinas-huawei-to-enter-south-korean-ai-chip-market-with-new-atlas-superpods-clusters-pack-8-192-ascend-950-accelerators-per-deployment-reportedly-challenges-nvidia-dominance-with-tripled-inference-performance-of-h20-at-one-quarter-the-cost) / [Digitimes](https://www.digitimes.com/news/a20260302VL209/huawei-ascend-data-center-nvidia-mwc-2026.html)**

配合 WAIC，华为在上海展台首次公开 Atlas 950 SuperPoD 的完整形态：8,192 张 Ascend 950 NPU、UnifiedBus 高速互联、FP8 峰值 8 EFLOPS、低精度 16 EFLOPS——**这是目前中国厂商能拿出的最高规格 AI 训练集群**。华为强调该系统被工程化为"单一逻辑计算机"，训练时通信延迟低于传统松耦合加速器阵列。

在 3 月 MWC 上华为已经展示过 Atlas 950 的样机，但当时缺少完整参数和路线图。本次 WAIC 首秀补齐了三件事：一是完整规格公开、二是 4Q26 出海韩国的商用计划、三是与 NVIDIA H20 的对比数据——Ascend 950PR 在推理任务上宣称 **2.87 倍 H20 性能、四分之一成本**。

对英伟达来说，压力开始从"技术优势"转向"外部管制窗口"：只要美国继续限制 H100/H200 对华出货，华为就有足够时间在国内和东南亚扩大装机量。而对中国 AI 生态而言，Atlas 950 是"上游算力可控"从口号变成 KPI 的关键节点。

**点评：** 华为已经不再只对标 H20 这种降规版，Atlas 950 的目标是 B200 系统级——这是中国 AI 硬件第一次在"整机架构"层面追上世界最前沿，NVIDIA 的"垄断护城河"叙事必须要调整了。

---

### 💰 No.4 · Anthropic Fable 5 三度延长免费访问——一场关于容量、而非价格的拉锯战

**[The New Stack](https://thenewstack.io/fable-5-honeycomb-opus/) / [TechTimes](https://www.techtimes.com/articles/320265/20260712/fable-5-free-through-july-19-anthropic-blinks-again-opus-5-leak-surfaces-cursor.htm)**

Anthropic 本周三度延长 Fable 5 的 Pro / Max / Team / 部分 Enterprise 订阅免费访问至 7 月 19 日 23:59 PT。这已经是自 6 月末原定退出订阅以来的第三次"延期"——**每一次都是在容量恢复的当天临时决定**。

背景是 Fable 5 的成本结构：单独用量计价定为 $10 / 百万输入 + $50 / 百万输出，是 Opus 4.8 的 2 倍、Sonnet 5 入门价 $2/$10 的 5 倍。Anthropic 已多次公开表示"移除 Fable 5 from subscriptions 是容量决策而非永久涨价"，Claude Code 团队工程师也在 GitHub 确认 Fable 5 会在基础设施跟上后回归订阅制。

真正的信号在别处：**Cursor 内部代码库里出现了 Opus 5 的引用**——Anthropic 有意让 Fable 5 承担"极限任务"，同时用 Sonnet 5 抢占中间市场，把 Opus 5 留给下一轮企业级发布。这套三档策略（Fable 5 高端 / Opus 5 主力 / Sonnet 5 走量）如果落地，Anthropic 会形成对 OpenAI 三档（Sol/Terra/Luna）的直接对位。

**点评：** Anthropic 现在最紧张的不是价格，是 GPU——每次"临时延长"背后都是数据中心和 Trainium 装机进度的实时反馈。谁能率先把容量瓶颈踩过去，谁就能把"顶级模型订阅化"这件事重新拿回主导权。

---

### 📈 No.5 · 2026 上半年全球风险投资 5,100 亿美元，AI 独占鳌头

**[Crunchbase](https://news.crunchbase.com/venture/global-startup-exits-ipo-ma-soar-ai-q2-h1-2026/)**

Crunchbase 数据显示，2026 上半年全球风险投资达 **5,100 亿美元**，已经超过 2025 全年（4,400 亿）总额。AI 是绝对主线：仅美国 H1 就录得 4,127 亿美元，AI 交易占据大部分头部融资。

7 月热度不减：**7 月 15 日单日 8 家 AI 公司融资 10.22 亿美元**，覆盖医疗、基础设施、身份、语音、编码、企业自动化和 matching。Neko Health 拿下 7 亿 Series C（Lightspeed 领投）、Emergent 完成 1.3 亿 Series C 达 15 亿估值、"盒装工程团队"叙事在企业市场持续走热。

7 月 AI 智能体赛道单月即录 18 亿美元、12+ 笔交易，**季度环比估值涨 40% 至平均 2.8 亿美元**——这已经是明显的过热区间，但资金还在加码。

**点评：** 5100 亿只是个开始——只要 GPT-5.6、Gemini 3.5 Pro、Fable 5 三大顶级模型的能力提升还在兑现"应用市场重建"的叙事，2026 全年破 1 万亿几乎是板上钉钉的事。风险是估值倒挂：智能体公司 40% 单季度估值涨幅意味着 2027 上半年将迎来第一波估值修正。

---

## 行业观察

**主线一：模型军备赛进入"三档产品线"时代。** 今日 Gemini 3.5 Pro、GPT-5.6 三档（Sol/Terra/Luna）、Anthropic 三档（Fable 5/Opus 4.8/Sonnet 5）以及即将推出的 Opus 5，标志着顶级实验室都统一转向"高端旗舰 + 主力企业 + 廉价走量"的组合拳。谁的中间档能维持性能领先且不烧钱，谁就是未来两年的最大赢家。

**主线二：中美 AI 从"技术差距"进入"生态对撞"。** 习近平亲自出席 WAIC + 华为 Atlas 950 SuperPoD 首秀 + WAICO 落沪计划——中国正在从"追赶模型"转向"另起炉灶做算力+治理体系"。这对美国生态最直接的影响是：中国市场作为"模型 API 主战场"的可能性正在关闭，OpenAI/Anthropic/Google 未来的增量必须在 EU、印度、中东、拉美找回来。

**主线三：容量重新成为估值核心变量。** Anthropic Fable 5 三度延期、OpenAI Sol 触及容量上限——2026 下半年，AI 公司之间的差距不再只是模型能力，而是**"能把这个能力交付给多少企业"**。这也解释了为什么头部公司都在加速自建数据中心（OpenAI Stargate、Anthropic Trainium、Google TPU v6、Meta MTIA）——市场对"算力自持率"的定价将在 Q3/Q4 财报季首次显性化。

**主线四：监管进入"分区分速度"阶段。** EU AI Omnibus 推迟高风险 AI 义务、White House 推动州法优先豁免——欧美监管都在事实上"让步"，为顶级模型的商用留出更长跑道。而中国路线是"官方推 WAICO + 内循环强化"的另一条路径。**未来 12 个月，AI 治理会从"谁最严格"进入"谁最好用"的竞争。**
