# AI 每日资讯 · 2026-07-04

## 今日焦点

> **Anthropic 强势追赶 OpenAI · Sonnet 5 免费开放 · Fable 5 出口管制解除 · GPT-5.6 家族仅向政府限量分发 · EU AI Act 全面执法倒计时**
>
> - **Claude Sonnet 5 免费全量开放**：Anthropic 将 Sonnet 5 设为 Free/Pro 用户默认模型，原生 1M token 上下文，促销价 $2/$10 每百万 token，性能接近 Opus 4.8。
> - **Fable 5 出口管制解除**：Fable 5 于 7 月 1 日全球恢复访问，此前被美国商务部停用 20 天。
> - **GPT-5.6 Sol/Terra/Luna 限量预览**：OpenAI 应政府要求，仅面向约 20 家可信合作伙伴开放，Cerebras 上跑到 750 tok/s。
> - **TwelveLabs 融资 $1 亿**：视频 AI 独角兽 Series B 由 NEA、Naver Ventures、Amazon 领投，估值破 10 亿美元。
> - **Nvidia + Valar 核电驱动 AI**：加州核电初创 Valar Atomics 用 Ward 250 反应堆直接为 Blackwell 芯片供电，两家公司签订核电 AI 联合开发协议。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Claude Sonnet 5 成为 Free/Pro 默认模型，1M 上下文，促销价 $2/$10 | Anthropic | ⭐⭐⭐⭐⭐ |
| 2 | Fable 5 出口管制解除，全球恢复访问 | Al Jazeera | ⭐⭐⭐⭐⭐ |
| 3 | OpenAI GPT-5.6 Sol/Terra/Luna 限量预览，Cerebras 上 750 tok/s | OpenAI | ⭐⭐⭐⭐⭐ |
| 4 | Sam Altman 呼吁"AI 新秩序"，暗示 OpenAI 正在被 Google/Anthropic 追赶 | Fortune | ⭐⭐⭐⭐ |
| 5 | Trump AI 行政令 7 月 2 日交付节点：财政部成立漏洞情报中心 | White House | ⭐⭐⭐⭐ |
| 6 | Gemini 3.5 Pro 从 6 月延到 7 月，仍在 Vertex AI 企业预览 | Google | ⭐⭐⭐⭐ |
| 7 | TwelveLabs 融资 $1 亿 Series B，视频 AI 独角兽 | Crunchbase | ⭐⭐⭐⭐ |
| 8 | Nvidia + Valar Atomics 核反应堆为 Blackwell 芯片供电 | Bloomberg | ⭐⭐⭐⭐ |
| 9 | Quantum Systems 融资 $12 亿 Series D，Blackstone 领投国防 AI | Tech Startups | ⭐⭐⭐⭐ |
| 10 | Claude Science 面向药企科研上线 | STAT News | ⭐⭐⭐⭐ |
| 11 | EU AI Act 8 月 2 日全面执法，罚金上限 €3500 万或全球营收 7% | 欧盟数字战略 | ⭐⭐⭐⭐ |
| 12 | Qwen3-Max 登顶中国 AI 模型榜首，Arena-Hard 90.5 | BenchLM | ⭐⭐⭐ |
| 13 | Grok Web 流量 1-5 月下滑 22%，跌幅居所有主流聊天机器人之首 | Forbes | ⭐⭐⭐ |
| 14 | Anthropic 自报营收超过 OpenAI，目标 2029 年盈利 | Fortune | ⭐⭐⭐⭐ |
| 15 | Claude Enterprise 新增管理员分析、模型级授权、开销告警 | Anthropic | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Claude Sonnet 5 免费开放，Anthropic 借"性价比 + 智能体"改写竞争格局

**[Anthropic Newsroom](https://www.anthropic.com/news)**

7 月 1 日，Anthropic 将 Claude Sonnet 5 设为所有 Free 和 Pro 用户的默认模型，同步进入 Claude Code。核心指标：原生 1M token 上下文、8 月 31 日前促销价 $2/$10 每百万 token（输入/输出），性能"接近 Opus 4.8"。这是 Anthropic 首次把"接近旗舰"的模型直接送到免费用户手中。

价格战意味明显：GPT-5.6 Sol 走的是政府限量、Cerebras 高速路线；Gemini 3.5 Pro 卡在 GA 前的最后调优；而 Anthropic 直接用"更便宜的 Opus 级智能"占领日常用户和 Coding Agent 场景。配合 Sonnet 5"能规划、能用浏览器和终端、能自主长跑"的智能体定位，Anthropic 明显在赌"下一代交互不是聊天，而是任务托管"。

配套动作也一并落地：Claude Enterprise 添加管理员分析、模型级授权、开销告警；Claude Apps Gateway 打通 Amazon Bedrock 与 Google Cloud，加上 SSO、策略、RBAC、按人成本追踪。企业侧交付力已明显补齐。

**点评：** Anthropic 用免费流量做上量、用企业管控做锁定、用智能体做溢价，这套组合拳打得比 OpenAI 现阶段更完整；Sam Altman 谈"AI 新秩序"未必只是外交辞令。

---

### 🚀 No.2 · Fable 5 出口管制解除，20 天禁令改写监管—产业博弈剧本

**[Al Jazeera](https://www.aljazeera.com/economy/2026/7/1/us-lifts-restrictions-on-powerful-ai-models-fable-mythos-anthropic-says)**

美国商务部 6 月 12 日出于国家安全考虑对 Anthropic 最强推理模型 Fable 5 和 Mythos 5 实施出口管制，中断全球服务近 3 周。6 月 30 日管制解除，7 月 1 日 Anthropic 全线（Claude.ai、Claude Platform、Claude Code、Claude Cowork）恢复访问。

这是产业史上第一起"针对单一 AI 模型的临时全球停机"事件，20 天里 Anthropic 官方给出的用户挽留是"降级到 Opus 4.8 + Sonnet 5 提前发放"。表面看模型撑住了短暂缺席，实质上产业得到了一个明确信号：出口管制可以精确到模型 SKU 级别，且政府具有随时开关能力。

配合 6 月 2 日 Trump 行政令要求财政部 7 月 2 日前建立"覆盖前沿模型自愿预发布访问框架"，出口管制—白宫预审—CAISI 十倍扩编（$1500 万 → $1 亿/年）三线合力，实际上把美国前沿 AI 的"发布权"提前置入政府议程。

**点评：** 短期利好 Anthropic（模型复活 + 政府信任），长期利空全行业（模型上线要看政府脸色）；下一次 Fable 级模型停机，可能就是竞争对手而不是 Anthropic 自己了。

---

### 🚀 No.3 · GPT-5.6 家族仅对政府盘点的 20 家伙伴开放，OpenAI 走上"半军管"路线

**[OpenAI · Previewing GPT-5.6 Sol](https://openai.com/index/previewing-gpt-5-6-sol/)**

6 月 26 日 OpenAI 预览 GPT-5.6 家族三款：旗舰 Sol、低成本 Terra、极速 Luna。Sol 在 Terminal-Bench 2.1 上创下新 SOTA，在网络安全领域"漏洞研究和利用"长任务上有明显提升。Cerebras 上 7 月推出 Sol 版本可跑到 750 tok/s，是当前主流服务速度的 15 倍。

关键节点：**限量预览，且合作伙伴名单由 OpenAI 与美国政府共同商定**。这是继 Anthropic Fable 5 遭出口管制之后，OpenAI 主动配合的第一次"政府背书发布"。理由官方说得直白——GPT-5.6 Sol 是"最强网络安全模型"，涉及漏洞挖掘和攻防能力，必须限量。

同时期 Fortune 报道：Anthropic 自报营收已超过 OpenAI，冲击 $470 亿，预计 2029 年盈利，比 OpenAI 早一年。Sam Altman 罕见公开呼吁"AI 世界新秩序"，被解读为对 OpenAI 追赶乏力的焦虑。

**点评：** OpenAI 用"能力—安全—政府"三段绑定守住高端；Anthropic 用"便宜 + 智能体"从底部抢用户。战术层面 Anthropic 目前赢面更大，但一旦 GPT-5.6 全面开放，护城河竞赛将回到模型质量本身。

---

### 🔬 No.4 · TwelveLabs $1 亿 Series B：视频 AI 首个"存量数据变现"独角兽

**[Tech Startups](https://techstartups.com/2026/07/02/venture-capital-startup-funding-roundup-july-2-2026/)**

7 月 2 日 TwelveLabs 完成 $1 亿 Series B，NEA、Naver Ventures、Amazon 领投，估值超过 10 亿美元。核心叙事简单直接：企业沉睡多年的视频素材（会议录像、监控、生产线画面、广告库、体育直播）第一次有了可检索、可总结、可推理的能力。

这轮融资的信号意义高于金额：过去 12 个月视频 AI 大量集中在"文生视频"（Sora、Runway、Kling），投资人开始意识到 B 端更大市场其实是"视频理解"——把已有视频变成结构化知识。TwelveLabs 直接把这个方向做成第一家真正的独角兽，估值锚点也从此建立。

同日 Blackstone 领投 Quantum Systems $12 亿 Series D 国防 AI；Celea Therapeutics $1.8 亿投呼吸疾病 AI。资金结构说明"AI + 传统重资产"（视频、国防、生物制药）是 2026 年下半年 VC 的偏好切换。

**点评：** 生成式 AI 的下半场，"消化存量数据"比"生成新数据"更值钱；TwelveLabs 这轮定价，将带动一批 "vertical understanding" 玩家（法务、医疗、金融）跟进。

---

### ⚡ No.5 · Nvidia + Valar 核反应堆直供 AI 芯片，"电力—算力"绑定进入实操期

**[Bloomberg](https://www.bloomberg.com/news/articles/2026-07-01/nvidia-ai-chip-gets-power-from-valar-s-nuclear-reactor)**

7 月 1 日 Valar Atomics 用 Ward 250 微型反应堆在犹他州直接为一颗 Nvidia Blackwell 芯片供电，短暂托管了一个网站。两家公司同步签署联合开发协议，探索"核电—AI 系统"整体方案。这是第一次"民用小堆"和"主流 AI 芯片"公开做端到端演示。

Blackwell 平台上跑万亿参数模型比上一代节能 25 倍，但即便如此，AI 数据中心 2026 年电力缺口已经是每一家超大规模云厂商的头号痛点。Rubin 平台今年发布，token 推理成本再降 10 倍、MoE 训练 GPU 数量降 4 倍，仍然改变不了"更快电站建设"是行业最刚性瓶颈的事实。

配套背景：Morgan Stanley 近日警告"AI 突破 2026 到来，多数国家没准备好"，其中一半理由是电力和监管。Nvidia 走上"直接跟核电初创绑定"的路径，实际上是把上游能源纳入自家路线图。

**点评：** 未来 24 个月，AI 大厂签的可能不再是 GPU 大单，而是电站长期合约；核电—AI 一体化会成为 2027 年前后的头号叙事。

---

## 行业观察

**Anthropic vs OpenAI 权力更迭正在发生。** Sonnet 5 免费开放叠加 Fable 5 出口管制解除，Anthropic 一周内既拿到用户增量，又完成了监管信任修复。同时期 OpenAI 只能以"限量政府预览 + Cerebras 极速"守住高端叙事。Fortune 关于 Anthropic 自报营收反超 OpenAI 的报道，从财务上确认了 Sam Altman 少见的公开焦虑。

**监管—产业进入"发布前审查"时代。** 6 月 Trump 行政令 30/60 天节点密集触发：7 月 2 日财政部漏洞情报清算所成立，8 月 1 日 CAISI 拿到十倍预算。跨大西洋另一边，EU AI Act 8 月 2 日全面执法，罚金上限 €3500 万或全球营收 7%。发布节奏、模型访问、企业合规同时被政府议程主导。

**下半场资本主题：存量数据 + 电力 + 国防。** 7 月 2 日单日融资清单：视频理解（TwelveLabs）、国防自主系统（Quantum Systems）、生物制药（Celea）。加上 Nvidia—Valar 核电示范，方向清晰——大模型自身估值见顶后，钱在往"AI 落地到硬约束场景"的地方流。

**中国开源仍在压制底部报价。** Qwen3-Max 登顶 BenchLM 中国榜（90.5），DeepSeek V4 保持 $0.14–0.30 输入价的极限低价。虽然美国政府对前沿模型收紧管控，但中国开源阵营通过"够用 + 极便宜"持续吃掉了应用层份额，这是 GPT-5.6 限量策略必须直面的另一头竞争。
