# AI 日报 · 2026-06-07

## 今日焦点

> **Anthropic 上市冲击万亿 · 白宫"自愿型"AI 监管落地 · 英伟达进军 PC 生态 · 微软 MAI 自研模型出阵 · Agent 经济撑起新估值**
>
> - **Anthropic 抢跑 IPO**：S-1 已秘密递交，融资轮估值 9650 亿美元反超 OpenAI，公司同期警告"递归自我改进"窗口正在逼近。
> - **特朗普签署 AI 行政令**：建立自愿前沿模型上报机制（部署前最长 30 天审查），同时大幅降低 AI 监管摩擦。
> - **英伟达双线出击**：Vera CPU 全面量产，OpenAI/Anthropic/SpaceX 成为首批客户；RTX Spark Superchip 杀入 Windows on Arm 笔记本市场，AMD/Intel/高通同日股价齐跌。
> - **微软发布 MAI 七模型家族**：MAI-Transcribe-1.5 在转录基准上超过 Gemini 与 OpenAI，MAI-Image-2.5 跻身 Arena 榜首集团，明显加速去 OpenAI 化。
> - **Agent 经济估值狂飙**：Supabase 借 Claude Code 红利获 105 亿美元估值；Coralogix 拿下 2 亿美元押注"agent 监控层"。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Anthropic 9650 亿美元估值秘密递交 IPO，同期警告 AI 递归自我改进 | Fortune / CNBC | ⭐⭐⭐⭐⭐ |
| 2 | 特朗普签署"促进先进 AI 创新与安全"行政令，确立 30 天自愿审查机制 | The White House | ⭐⭐⭐⭐⭐ |
| 3 | 英伟达 Vera CPU 全面量产，OpenAI、Anthropic、SpaceX 首发部署 | Bloomberg / CNBC | ⭐⭐⭐⭐ |
| 4 | 英伟达 RTX Spark Superchip 联手 MediaTek，杀入 Windows on Arm PC 市场 | Bloomberg | ⭐⭐⭐⭐ |
| 5 | 微软 Build 2026 推出 MAI 七模型家族，转录与图像基准击败 OpenAI / Gemini | CNBC | ⭐⭐⭐⭐ |
| 6 | Salesforce 借 Claude Code，将原本 231 天的迁移缩到 13 天，FY26 工程零增员 | Anthropic case study | ⭐⭐⭐⭐ |
| 7 | xAI Grok V9-Medium（1.5T 参数）完成训练，专攻编码，Cursor 数据训练 | TechTimes | ⭐⭐⭐⭐ |
| 8 | Supabase 完成 5 亿美元融资，估值升至 105 亿美元，受益于 vibe-coding 浪潮 | CNBC | ⭐⭐⭐⭐ |
| 9 | 众议员 Obernolte / Trahan 发布《2026 美国伟大 AI 法案》两党讨论稿 | Captain Compliance | ⭐⭐⭐⭐ |
| 10 | Coralogix 获 2 亿美元融资，押注"AI agent 可观测层"，估值 16 亿美元 | TechCrunch | ⭐⭐⭐ |
| 11 | 谷歌发布 Antigravity 2.0，可并行编排多 agent 同时执行任务 | Google Cloud | ⭐⭐⭐ |
| 12 | Gemini 3.1 Flash-Lite 开放 Public Preview，主打超低延迟 + 极致单价 | Google Cloud | ⭐⭐⭐ |
| 13 | OpenAI 更新 GPT-Rosalind 生命科学模型，新增药物发现与生信插件 | Releasebot | ⭐⭐⭐ |
| 14 | Apoha 凭"液体波形数据"AI 走出隐身，获 3600 万美元 A 轮 | Fortune | ⭐⭐⭐ |
| 15 | 联邦 AI 采购合同总潜在金额暴涨 1912% 至 918 亿美元，国防部独吃 98.9% | Brookings | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Anthropic 9650 亿美元估值秘密递交 IPO，同期警告"递归自我改进"窗口逼近

**[Fortune: Anthropic warns AI could soon build itself without human involvement](https://fortune.com/2026/06/05/anthropic-ai-pause-development-recursive-self-improvement/)**

Anthropic 在 6 月 1 日秘密递交 S-1 招股书，配合刚刚关闭的 650 亿美元 H 轮（投后 9650 亿美元），首次在公开市场估值上正式反超 OpenAI（3 月时 8520 亿美元）。如果 IPO 顺利定价，这将是史上规模最大、估值最高的科技 IPO，万亿美元已经被多家投行作为"基础情景"。

与此同时，公司在 6 月 5 日发布罕见的政策长文，明确警告"递归自我改进"（recursive self-improvement, RSI）的窗口可能比多数机构预期更近：当前公司内部 80% 以上合并代码由 Claude 撰写，每季度交付代码量较 2025 年初翻 8 倍，Claude 独立完成任务的时长每 4 个月翻一倍。Anthropic 罕见地呼吁"全球暂停"在没有可验证安全保障的情况下追求 RSI 的工作。

时间点的微妙在于：恰好卡在 IPO 静默期之前，把"前沿能力 + 安全担忧"打包讲给了未来的二级市场。这是当年 OpenAI"先讲恐怖故事再卖产品"叙事的升级版，也意味着 SEC 路演里"安全"将是核心估值锚之一。

**点评：** 9650 亿美元是当下，递归自我改进是远期看涨期权——Anthropic 用一份"恐慌报告"把这两件事一起卖给了华尔街。

---

### 🚀 No.2 · 特朗普政府发布行政令，确立"自愿前沿模型上报 + 30 天预审"机制

**[The White House: Promoting Advanced Artificial Intelligence Innovation and Security](https://www.whitehouse.gov/presidential-actions/2026/06/promoting-advanced-artificial-intelligence-innovation-and-security/)**

6 月 2 日签署的行政令是本届政府对 AI 监管态度的一次明显转向。一方面继续延续"去监管/促创新"路线，要求 OMB 评估联邦补贴可否倾斜到 AI 漏洞检测；另一方面首次要求前沿厂商在面向公众发布前最长 30 天，自愿向联邦提交模型副本与评估，并设立"AI 网络安全清算中心"协调漏洞披露。

行政令同时要求司法部长把"AI 加持的网络犯罪"列为优先起诉，并把对 AI 的国防/情报采购视为战略产业政策的一部分。配套数据相当惊人——2026 年截至目前，联邦 AI 已确认拨款 72 亿美元（同比+966%），潜在合同总盘子 918 亿美元（+1912%），国防部独占 98.9%。

值得注意的是：此举刚好与 6 月 4 日两党议员 Obernolte / Trahan 推出的《2026 美国伟大 AI 法案》讨论稿形成"行政 + 立法"双线压力，前沿厂商今年的合规和华盛顿政府关系预算会出现结构性跳升。

**点评：** 表面上是"自愿"，实际是把所有头部厂商绑上了一张白宫的牌桌——拒绝合作的厂商在政府采购里基本无路可走。

---

### 💎 No.3 · 英伟达双线出击：Vera CPU 量产首发 OpenAI/Anthropic/SpaceX，RTX Spark 杀入 Windows PC

**[CNBC: Nvidia's new PC chips represent Huang's bid to win at every layer of AI stack](https://www.cnbc.com/2026/06/02/nvidias-new-pc-chips-are-ceos-bid-to-own-every-part-of-ai-stack.html)**

黄仁勋在 6 月 1-2 日完成了对计算栈的两次同步打击。其一，Vera CPU 进入全面量产，OpenAI、Anthropic、SpaceX 成为首批客户，意味着英伟达不再仅仅是"GPU 提供方"，而是接管了数据中心一侧整套 CPU+GPU+互联+网络的"全栈"——AMD 与 Intel 在数据中心 x86 的最后一块阵地正式被撕开口子。

其二，与 MediaTek 合作的 RTX Spark Superchip 直接踩入 Windows on Arm 笔记本市场，Dell、HP、联想首批跟进。当日 AMD、Intel、高通三家股价同步下跌。黄仁勋还把 PC CPU 长期市场目标喊到 2000 亿美元，相当于把"AI PC"重新定义为英伟达自家的增长曲线。

对面 AMD 的反击是 MI500 系列与 Helios 系统，号称对比 MI300X 性能提升 1000 倍，准备对标英伟达 NVL72（72 颗 Rubin GPU）。但客户名单与生态密度上，AMD 至少落后 2 年。

**点评：** 英伟达正在把"GPU 公司"重写为"AI 算力垄断公司"——数据中心 + PC + Arm 三线齐下，AMD/Intel 的护城河被压成 18 个月内的窗口期。

---

### 🛠️ No.4 · 微软 MAI 七模型家族出阵：转录、图像、代码全面挑战 OpenAI 与 Gemini

**[CNBC: Microsoft unveils new AI models to lessen reliance on OpenAI](https://www.cnbc.com/2026/06/02/microsoft-unveils-new-ai-models-lessen-reliance-on-openai-lower-costs.html)**

Build 2026 把"agent-first"从口号变成产品。微软一口气推出 MAI 七模型家族：MAI-Thinking-1（推理）、MAI-Code-1-Flash（代码生成）、MAI-Transcribe-1.5（语音转写，已超越 Gemini 与 OpenAI 同类）、MAI-Image-2.5（图像生成，Arena 榜单跻身第一梯队），以及面向多步工具调用的 agent 专用变体。

更关键的是 Agent 365 正式 GA：跨云的 agent 发现与治理控制面，覆盖 AWS 与 Google Cloud。这把"shadow AI"治理需求直接变成微软的订阅生意，重定义了 CIO 采购清单。

微软对 OpenAI 的依赖结构正在被改写——从"独家算力 + 模型供货方"，变成"多模型多 agent 平台主"，OpenAI 沦为众多 IP 之一。本周 OpenAI 也被迫加速在 ChatGPT Enterprise 内放出更多 agent 与转录工具，但叙事主动权已被 Build 抢去。

**点评：** 微软不再装作"OpenAI 的好朋友"——MAI 家族是给市场看的、Agent 365 是给 CIO 看的、Vera 客户名单是给华尔街看的，OpenAI 的"独家"光环正在被三面拆解。

---

### 📈 No.5 · Salesforce 案例 + Supabase 估值：Claude Code 把 Agent 经济推上下一台阶

**[CNBC: Vibe-coding lifts Supabase to $10.5 billion valuation](https://www.cnbc.com/2026/06/04/database-startup-supabase-raises-500-million-10point5-billion-valuation.html)**

Anthropic 公开的 Salesforce 案例显示，一项原本估时 231 天的迁移在 Claude Code 上 13 天交付，提速近 18 倍；Benioff 在公开场合证实 Salesforce 在 FY26 工程与客服 0 招聘，销售岗 +20%。这是大公司首次正式把"AI 替代工程招聘"写进财报口径，对 SaaS / IT 服务行业的人头模型是一次直接冲击。

下游同步爆发：Supabase 以 105 亿美元估值拿下 5 亿美元（GIC 领投，Accel、Coatue、Stripe 跟进），其增长曲线被高管直接归因于"Claude Code 是 2026 年 Supabase 数据库最大贡献方"。同期 Coralogix 拿下 2 亿美元，押注的就是"无数 agent 跑起来后总要有人盯着"——agent 监控层成为新基础设施叙事。

XAI Grok V9-Medium 也选在编码主战场加注，1.5T 参数 + 显式用 Cursor 真实开发者数据训练，将在 6 月中旬开打。

**点评：** AI 编码已经从"工具升级"演变成"组织重构"——估值、招聘、基础设施都跟着重排，所有围绕开发者的 SaaS 必须重新讲故事。

---

## 行业观察

今天的市场逻辑是清晰的"两条主线"。第一条线是 **资本市场**：Anthropic 的 IPO 与"递归自我改进"叙事把估值锚从 ARR 拉到"超级智能期权"，给后续 OpenAI、xAI 的 IPO 路演定下了节奏；同时 Supabase、Coralogix、Apoha 等中游标的估值集体跳涨，Q1 2026 已 2555 亿美元的 AI 融资几乎肯定要再创新高。

第二条线是 **政策与基建**：白宫行政令 + 两党法案讨论稿 + 联邦采购合同 918 亿美元，意味着前沿 AI 从"创业故事"正式被纳入"产业政策 + 国防优先"的双轨监管。这反过来让微软的 Agent 365、英伟达的 Vera 客户名单、Anthropic 的 IPO 时点都更像有意为之的政策协同。

中长期看，**算力 → 模型 → agent → 治理** 四层都在 Q2 末同步重洗：英伟达拿走了底层算力，OpenAI 与 Anthropic 在模型层进入资本市场对垒，微软抢下了 agent 治理面，而国会和白宫则把规则写进合同里。下一两个月可关注的三件事：OpenAI 的 S-1、xAI Grok V9-Medium 实测分数、以及国会能否把《2026 美国伟大 AI 法案》推进到正式立法。
