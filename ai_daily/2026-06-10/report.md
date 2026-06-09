# AI 行业日报 · 2026-06-10

## 今日焦点

> **Mythos 全面公开 · 前沿模型价格腰斩 · Anthropic IPO 倒计时 · Apple 倒向 Gemini · 白宫国安令重塑监管**
>
> - **Claude Fable 5 / Mythos 5 全量开放**：SWE-Bench Pro 80.3% 直接碾压 GPT-5.5 的 58.6%，定价 $10 / $50 per M tokens，较 Mythos Preview 砍半。
> - **Anthropic 6 月 1 日秘密提交 S-1**：在 $65B Series H、$965B 估值之上启动 IPO，ARR 已飙至 $47B 年化。
> - **苹果 WWDC 倒向谷歌**：Siri AI 由定制版 Gemini 驱动，每年向 Google 支付约 $10 亿；Claude 首次作为 iPhone 默认可选模型出现。
> - **特朗普 6 月 2 日签署 AI 国安行政令**：要求前沿模型上线前自愿向联邦提交 30 天，建立国家安全评估框架，进一步压制各州 AI 立法。
> - **半导体单日蒸发 $1.3T**：Broadcom AI 营收小幅不及预期触发崩盘，Nvidia 单日跌 6%、市值蒸发 $7400 亿。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Anthropic 发布 Claude Fable 5 / Mythos 5，SWE-Bench Pro 80.3% | VentureBeat / Anthropic | ⭐⭐⭐⭐⭐ |
| 2 | Anthropic 秘密递交 IPO 招股书，ARR 达 $47B | The Information / Bloomberg | ⭐⭐⭐⭐⭐ |
| 3 | WWDC：苹果 Siri AI 转用 Gemini，年付谷歌 $10 亿 | Business Standard / Bloomberg | ⭐⭐⭐⭐⭐ |
| 4 | 特朗普签署「促进先进 AI 创新与安全」行政令 | The White House | ⭐⭐⭐⭐⭐ |
| 5 | 半导体板块单日蒸发 $1.3T，Broadcom AI 营收不及预期触发 | Intellectia / Reuters | ⭐⭐⭐⭐ |
| 6 | Microsoft 发布 MAI-Code-1-Flash，自研模型摆脱 OpenAI 依赖 | CNBC | ⭐⭐⭐⭐ |
| 7 | Reflection AI 完成 $20 亿融资，估值 $80 亿 | TechFundingNews | ⭐⭐⭐⭐ |
| 8 | Rhoda AI $4.5 亿 A 轮，发布机器人视觉控制平台 FutureVision | Crescendo | ⭐⭐⭐ |
| 9 | Microsoft Foundry 模型目录突破 11,000 个，新增 GPT-5.5、Opus 4.8 | Microsoft | ⭐⭐⭐ |
| 10 | EU AI Act 透明度条款将于 8 月 2 日正式生效 | European Commission | ⭐⭐⭐⭐ |
| 11 | Gemini 3.5 Flash GA，价格 $1.50 / $9.00 per M tokens | Google Cloud | ⭐⭐⭐ |
| 12 | xAI 完成 $200 亿新一轮融资，Grok 4.3 Skills 上线 | AI Business | ⭐⭐⭐ |
| 13 | Stripe 用 Fable 5 在 5000 万行 Ruby 代码库中一天完成两月迁移 | Anthropic | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Anthropic 将 Mythos 拉到大众：Claude Fable 5 / Mythos 5 同步发布

**[VentureBeat](https://venturebeat.com/technology/anthropic-brings-mythos-to-the-masses-with-claude-fable-5-its-most-powerful-generally-available-model-ever)**

昨天（6 月 9 日），Anthropic 把内部代号 Mythos 的下一代模型完整开放，分两个版本：面向通用市场的 Claude Fable 5、以及移除部分安全护栏、面向网络安全与生物安全用例的 Claude Mythos 5。两者底层同一权重，定价均为输入 $10 / 输出 $50 per M tokens——较 Mythos Preview 直接砍半，但仍是 OpenAI GPT-5.5 的两倍以上。

性能上 Fable 5 重写了前沿天花板：SWE-Bench Verified 95.0%、SWE-Bench Pro 80.3%（GPT-5.5 仅 58.6%）、Cognition FrontierCode Diamond 29.3%（Opus 4.8 13.4%、GPT-5.5 5.7%）。Stripe 在内测中用它在 5000 万行 Ruby 代码库内一天完成原本需要 2 个月、5 人团队的迁移工作——这是过去 12 个月里第一份让大型企业 CTO 普遍承认「确实是阶跃」的真实案例。

Pro / Max / Team / Enterprise 用户即日起到 6 月 22 日免费试用，意图明显——在 GPT-5.5 落地 45 天后用免费窗口直接抢市场份额。

**点评：** Anthropic 把「定价/能力」这道题做到了 OpenAI 在 GPT-4o 时代才有的统治力，更关键的是给 IPO 路演讲清了一个故事——前沿模型可以年降本 50%、同时性能跃迁两个台阶。

---

### 🚀 No.2 · Anthropic 秘密递交 IPO，从 $65B 融资到 $47B ARR 只用 4 个月

**[CNBC / Bloomberg](https://www.cnbc.com/2026/06/01/microsoft-and-google-take-on-anthropic-and-openai-in-ai-coding-models.html)**

6 月 1 日，Anthropic 向 SEC 秘密递交 S-1，跟 OpenAI 同期开启上市路径。背景是 5 月底刚刚关闭的 $65B Series H，post-money 估值 $965B，首次超越 OpenAI 上一轮 $852B。更生猛的是营收曲线：2 月 Series G 关闭时 ARR 还是 $14B，5 月已经飙到 $47B 年化——4 个月 3.4×。

驱动因素一是 Claude Code 把 Stripe、Shopify、Booking.com 这些超大型 codebase 拿下；二是企业用户用 Mythos Preview 替换 GPT-4o 的迁移潮；三是 AWS Bedrock 与 Vertex AI 双渠道分发的复合效应。考虑到今天 Fable 5 的发布卡位，Q2 数据出来时 ARR 可能再翻一倍。

**点评：** 这是一份连 OpenAI 都会眼红的招股书。如果年内挂牌，Anthropic 大概率成为美股史上最大 IPO，估值会推高到 $1.2T+。

---

### 🎯 No.3 · 苹果 WWDC：Siri 押注 Gemini，Claude 成 iPhone 默认可选项

**[Business Standard](https://www.business-standard.com/amp/technology/tech-news/wwdc-2026-apple-unveils-siri-ai-gemini-powered-apple-intelligence-more-126060900042_1.html)**

6 月 8 日 Cupertino，库克亲自宣布 Siri 重命名为 "Siri AI"，云端智能由定制版 Gemini 在苹果 Private Cloud Compute 内运行，年付谷歌约 $10 亿。同时苹果推出 "Multi-AI Extensions" 框架，用户可以把 Claude、ChatGPT 接入 iOS 27 系统级 Action，Claude 首次出现在 iPhone 默认选项里。

这是 Apple Intelligence 自 2024 年首发以来最大的策略转弯——自研基础模型阵地彻底失守，转而把 14 亿 iPhone 的入口拍卖给最高出价者。Gemini 拿下默认权，Claude 拿到可选权，OpenAI 在 iPhone 的存在感被显著稀释。

反垄断风险也在浮现：5 月份就有律师警告这交易会成为「下一个 Microsoft 反垄断案」，DOJ 正在评估。

**点评：** 苹果用 $10 亿/年买回了几年时间，但代价是把消费 AI 主导权交给了谷歌；Claude 则用「可选项」身份避免了与 Gemini 正面冲突，可能是最大的隐性赢家。

---

### 📜 No.4 · 特朗普 6 月 2 日签署 AI 国安行政令：前沿模型必须提前 30 天上报

**[The White House](https://www.whitehouse.gov/presidential-actions/2026/06/promoting-advanced-artificial-intelligence-innovation-and-security/)**

行政令名为「Promoting Advanced Artificial Intelligence Innovation and Security」，核心三条：(1) 要求前沿模型开发商在向合作方开放前自愿向联邦提交至多 30 天；(2) 指令国安各机构在 90 天内建立 AI 风险评估框架；(3) 延续 12 月 14365 号令的精神，进一步限制各州独立立法权（加州 SB-1047 阴影下尤其敏感）。

这与 3 月「National Policy Framework for AI」一脉相承——白宫正在把 AI 治理彻底「国家安全化 + 联邦化」，把 EU AI Act 那种合规框架排除在外。配合即将 8 月 2 日全面生效的 EU AI Act 透明度条款，美欧监管路线分歧将进一步加大。

**点评：** 这条令对 Anthropic IPO 是好消息（联邦背书 = 合规护城河），对开源派（Meta、Mistral）是坏消息（30 天延迟会拖慢 Llama 与 Mistral 下一代迭代）。

---

### 💸 No.5 · 半导体单日蒸发 $1.3T：Broadcom 一次小幅不及预期，引爆 AI 估值泡沫

**[Intellectia](https://intellectia.ai/blog/semiconductor-stocks-selloff-june-2026)**

本周 Broadcom 公布最新季度 AI 营收，仅小幅低于预期，但在已经过热的预期面前足以触发踩踏：Nvidia 单日跌 6%、市值蒸发 $7400 亿；AMD、台积电、Marvell、Coherent 全部双位数下挫，AI 芯片板块单日蒸发 $1.3T。

背景是 Nvidia 自己 FY26（截至 2026 年 1 月）已经做到 $215.9B 营收（+65%），数据中心年化 $120B，所有人都在赌 FY27 至少再翻一倍。Broadcom 的数据等于第一次告诉市场——「客户的资本开支不是没有上限」。

**点评：** AI 基建估值进入「需要持续证明的阶段」，下一份 hyperscaler capex guidance（7 月开始的财报季）将决定 Nvidia 是回弹还是开启二次下跌。

---

## 行业观察

今天的主线是 **前沿模型代际更替 + 资本市场提示风险** 的同步上演。Anthropic 用 Fable 5 在能力与价格两个轴同时压制 OpenAI，并把 IPO 节奏卡在峰值，财务侧的 $47B ARR 与产品侧的 SWE-Bench Pro 80% 共同构成它向公开市场要钱的最强论据。

苹果的转向是另一条隐线——大模型层的红利正被快速集中到 Anthropic / Google / OpenAI 三家，所有「平台公司」（Apple、Microsoft、Meta）都在重新思考是否还要自研基础模型。Microsoft MAI-Code-1-Flash 与 Apple-Gemini 交易看似方向相反，本质都是「在前沿之外找一条够用的路」。

监管层正在二元化：白宫国安令把美国 AI 推向「国家冠军 + 联邦护栏」，EU AI Act 8 月 2 日全面生效则保持透明度合规路径。Anthropic 同时满足两套话术（联邦认证 + 安全研究身份），是当前监管套利最干净的玩家。

半导体单日 $1.3T 的回撤提示：模型能力的指数曲线（Fable 5 一年涨 30+ 个百分点）与算力资本开支的线性扩张之间，可能正出现错配。下半年最值得跟踪的不是新模型，而是 hyperscaler 的 capex 修正幅度。
