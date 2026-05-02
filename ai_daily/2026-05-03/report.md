# AI 行业日报 · 2026-05-03

## 今日焦点

> **国防 AI 站队 · Anthropic 估值反超 · OpenAI 多云分发 · 中国开源 V4 浪 · EU AI Act 强制临近**
>
> - **五角大楼绕开 Anthropic** 与 OpenAI、Google、MS、Nvidia、AWS、SpaceX、Reflection 七巨头签署机密网络部署协议，AI "护栏" 之争演变为商业代价。
> - **Anthropic 拟以 9,000 亿美元估值募资**，单日反超 OpenAI 的 8,520 亿，叠加 Google 承诺 400 亿美元投资，与 OpenAI 进入"双巨头"对峙。
> - **OpenAI 模型登陆 AWS**，正式打破"独宿 Azure" 的蜜月期，多云分发开始改写 AI 基础设施格局。
> - **DeepSeek V4 Preview 发布**，专门针对 Claude Code / OpenClaw 等 Agent 工具做了优化，中美开源生态出现"工具兼容层"互通。
> - **EU AI Act 高风险条款** 8 月 2 日强制生效已无悬念，5 月谈判仅剩"如何过渡"的细节。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | 五角大楼与 7 家 AI 巨头签机密网络部署协议，独缺 Anthropic | CNN / Defense News | ⭐⭐⭐⭐⭐ |
| 2 | Google 承诺投资 Anthropic 至多 400 亿美元，估值 3,500 亿 | TechCrunch | ⭐⭐⭐⭐⭐ |
| 3 | Anthropic 与投资人洽谈 9,000 亿美元估值新一轮融资 | CNBC | ⭐⭐⭐⭐⭐ |
| 4 | OpenAI 模型登陆 AWS，正式打破 Azure 独家分发 | OpenAI 官方 | ⭐⭐⭐⭐ |
| 5 | Anthropic 推出 Claude Connectors，原生连 Adobe/Blender/Ableton | Anthropic | ⭐⭐⭐⭐ |
| 6 | DeepSeek 发布 V4-Pro / V4-Flash Preview，原生兼容 Claude Code | Al Jazeera / CNBC | ⭐⭐⭐⭐ |
| 7 | EU AI Act 高风险条款 8 月 2 日强制生效进入倒计时 | Computerworld | ⭐⭐⭐⭐ |
| 8 | GPT-5.5 在 Intelligence Index 领先 3 分，输出 Token 少 72% | Artificial Analysis | ⭐⭐⭐⭐ |
| 9 | Mistral 完成 7.22 亿欧元股权 + 8.3 亿美元债权融资 | Bismarck Brief | ⭐⭐⭐ |
| 10 | xAI 11 位创始团队全部离职，Musk 启动二次重建 | Multiple | ⭐⭐⭐ |
| 11 | Perplexity ARR 突破 4.5 亿美元，估值 212 亿美元 | TSG Invest | ⭐⭐⭐ |
| 12 | Q1 2026 基础模型创业融资额超过整个 2025 年 | Crunchbase | ⭐⭐⭐ |
| 13 | Nvidia 暗示 OpenAI / Anthropic 是其最后两笔大额股权投资 | PYMNTS | ⭐⭐⭐ |
| 14 | Alpha Compute 504 卡 B200 集群 5 月 8 日加拿大投产 | GlobeNewswire | ⭐⭐⭐ |
| 15 | 阿里 Qwen 3 MoE 上线，token 价 $0.38/M，按需激活专家 | TechXplore | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · 五角大楼绕开 Anthropic：AI 安全分歧让出 7 家大厂订单

**[CNN Business — Pentagon strikes deals with 7 Big Tech companies after shunning Anthropic](https://www.cnn.com/2026/05/01/tech/pentagon-ai-anthropic)**

国防部确认与 OpenAI、Google、Microsoft、Nvidia、AWS、SpaceX 与 Reflection 七家公司签署机密网络部署协议——Anthropic 因坚持其 AI 武器化使用的安全护栏被川普政府从名单中拉黑。但白宫近期"重新打开了与 Anthropic 的沟通窗口"，原因是 Anthropic 近期连续公布若干技术里程碑。

这是 2026 年 AI 政商关系的标志性事件：**安全立场第一次明确换算成具体的商业代价**。过去 18 个月，"安全派"还能在估值与社会舆论上占便宜，但当美国国防部决定真金白银下场买单时，规则变了——拒绝在某些场景"摘掉护栏"的代价是直接出局。

值得注意的是 Reflection 的入选：一家成立不到三年的 startup 与超大公司同台，背后是新一轮"国家队"AI 初创扶持的影子。这预示后续国防 AI 招标可能更多让"接受任意定制"的中型创业公司分一杯羹。

**点评：** 当"AI 安全"开始有商业代价，所有顶层 AI 公司都将被迫对自己的红线重新定价。Anthropic 这次没让步——但下一次会不会让，是真正的看点。

---

### 🚀 No.2 · Google 砸 400 亿、Anthropic 估值冲 9,000 亿，"双寡头"格局成型

**[TechCrunch — Google to invest up to $40B in Anthropic](https://techcrunch.com/2026/04/24/google-to-invest-up-to-40b-in-anthropic-in-cash-and-compute/)** · **[CNBC — Anthropic in talks at $900B valuation](https://www.cnbc.com/2026/04/29/anthropic-weighs-raising-funds-at-900b-valuation-topping-openai.html)**

Google 承诺向 Anthropic 投入至多 400 亿美元（首期 100 亿、达成绩效后追加 300 亿），同时 Anthropic 已与投资人洽谈以 9,000 亿美元估值新一轮融资——直接超过 OpenAI 上一轮的 8,520 亿。Anthropic 的 ARR 已达 300 亿美元。

这个组合拳意味着两件事：**第一**，Google 已彻底放弃"自己的模型必须独占"的执念，转向"Gemini + Anthropic 双注"策略，与 Microsoft 在 OpenAI 上的"独栋押注"形成对照；**第二**，资本市场对 Anthropic 的"安全 + 编程能力 + 企业客户"三重叙事买单——尤其是 Claude Opus 4.7 在 SWE-bench Pro 上 5.7 分领先 GPT-5.5 的事实，已经被 Wall Street 转化成估值溢价。

OpenAI 的反应将耐人寻味。在 Nvidia 已暗示其 300 亿美元投资 OpenAI 是"最后一笔"的语境下，OpenAI 必须自证其在 IPO 前能维持估值锚——这或许解释了 GPT-5.5 选择上 AWS、迅速扩张分发的紧迫性。

**点评：** "双寡头"格局已经确立，但真正决定终局的不是估值数字，而是谁先把 Token 收入做到稳定盈利——Anthropic 暂时领先一步。

---

### 🤝 No.3 · OpenAI 模型登陆 AWS：MS-OAI 蜜月期正式终结

**[OpenAI Blog — Introducing GPT-5.5](https://openai.com/index/introducing-gpt-5-5/)**

OpenAI 正式宣布 GPT-5.5 等模型通过 Amazon Web Services 对企业客户开放——这是 OpenAI 首次承认 Microsoft 不再是其唯一云端分发渠道。AWS 加入意味着相当数量已建立 AWS-only 数据栈的企业，可以原生集成 GPT-5.5 而无需跨云。

技术上不复杂，但商业上巨震：**Microsoft 多年用 130 亿美元换来的"独家分发权" 正式作废**。市场普遍认为，这是去年 OpenAI 与 MS 续签合作时争来的一项关键松绑——OpenAI 用让出股权换回了"灵活分发"的自由度。

副作用是 GPT-5.5 之后的版本与 Microsoft Copilot / Office 之间的"绑定优势"将逐步弱化，其他云厂商（尤其 Google Cloud 和 Oracle）大概率会用类似条款挖走 GPT-5.5 在企业市场的部分份额。Bedrock 之于 OpenAI 的价值，类似于"在敌方阵地里建了个驻外使馆"。

**点评：** 一个最大的"封闭式 AI" 厂商，被市场的力量逼着走向了"分发 commoditization"。这件事 12 个月后会被引用为"AI 平台战的拐点"。

---

### 🇨🇳 No.4 · DeepSeek V4 兼容 Claude Code：中美开源工具链开始互通

**[CNBC — DeepSeek releases preview of V4](https://www.cnbc.com/2026/04/24/deepseek-v4-llm-preview-open-source-ai-competition-china.html)**

DeepSeek 上周末发布 V4-Pro / V4-Flash 双版本预览。本次的最大亮点不是模型本身的 benchmark（V4 在 agent / 知识 / 推理任务上"对标国内最佳"），而是 **官方明确声明对 Anthropic Claude Code 与 OpenClaw 等 Agent 工具做了优化**——这是中国开源大模型首次主动"贴近"美国主流工具链。

这意味着开发者可以用同一套 Claude Code workflow 切换底层模型：白天 Claude Opus 4.7、夜里 DeepSeek V4-Flash。对企业用户而言，这是 Token 成本和数据合规策略可调的关键基础。

战略含义更深：**当中国开源模型主动适配西方工具链时，"模型作为商品"的趋势便由现实而非口号确立**。模型被 commoditize 后，谁掌握开发者 harness（Claude Code、Cursor、Devin 等）才是新世界的入口。Anthropic 心情应该很复杂——一方面 Claude Code 普及度更高了，另一方面"用 Claude Code 跑 DeepSeek"会扭走部分 Token 收入。

**点评：** 中美 AI 之争从"模型代差"演变为"生态嵌入"，DeepSeek 找到了一条非常高明的弯道：寄生于对方的工具链生态。

---

### 🇪🇺 No.5 · EU AI Act 8 月强制临近：监管不再是纸面威慑

**[Computerworld — EU lawmakers fail to agree on watered-down AI Act](https://www.computerworld.com/article/4164963/eu-lawmakers-fail-to-agree-on-watered-down-ai-act-talks-pushed-to-may.html)**

欧盟成员国与欧洲议会就放宽 AI Act 的修订未能达成一致，谈判已推迟到 5 月。**最关键的事实**：如果 8 月 2 日前没有新方案，AI Act 关于"高风险 AI 系统"的强制义务将按原文生效。

意味着什么？所有在欧盟提供"高风险 AI"产品的厂商（医疗、招聘、信贷决策、教育评分等场景），届时必须满足完整的 conformity assessment、技术文档、人工监督与透明度披露要求。OpenAI / Anthropic / Google 已经在做合规准备，但**中型 SaaS 厂商和欧洲本地创业公司距离"合规就绪"仍有一定距离**——技术标准本身要到 12 月才会完整发布。

更现实的挑战是 GPAI（通用 AI 模型）义务自 2025 年 8 月起就已生效，但执法只是缓慢启动。本次若 8 月强制启用高风险条款，欧洲将出现 AI 监管的"双层悬崖"：合规企业获得明确边界，不合规企业要么离开欧洲市场，要么吃下罚款。

**点评：** EU AI Act 第一次在金融市场层面变成"具体定价"——比法律风险更可怕的是合规成本，初创公司应当立即评估自己有多少业务在"高风险"红线上。

---

## 行业观察

**今日的三个结构性变化：**

1. **AI 估值进入双寡头时代**：Anthropic 9,000 亿美元 + OpenAI 8,520 亿美元，市场已经把"两超 + N 强"当作前提条件——xAI 创始团队尽数出走、Mistral 加杠杆建数据中心，都是"第二梯队加速跟跑"的副产物。
2. **分发去独占化**：OpenAI 上 AWS、Anthropic 已在 AWS+GCP+Azure 全开，未来"模型独家"将仅在敏感政府客户场景下出现，企业 AI 已经事实上 commoditize。
3. **政府客户 vs. 安全立场的冲突彻底浮出水面**：Pentagon × Anthropic 事件不会是孤例——欧洲、英国、日本国防客户都会面临类似抉择，AI 公司必须制定"分级红线"，否则会反复在重大订单上吃亏。

**短期看点**：5 月底前后 EU AI Act 谈判结果、OpenAI 是否会反击式宣布超大规模融资、Anthropic 9,000 亿轮的最终领投方（Google 是否包揽）、DeepSeek V4 正式版的 benchmark 数据。

Sources:
- [CNN Business — Pentagon strikes deals with 7 Big Tech companies](https://www.cnn.com/2026/05/01/tech/pentagon-ai-anthropic)
- [TechCrunch — Google to invest up to $40B in Anthropic](https://techcrunch.com/2026/04/24/google-to-invest-up-to-40b-in-anthropic-in-cash-and-compute/)
- [CNBC — Anthropic at $900B valuation talks](https://www.cnbc.com/2026/04/29/anthropic-weighs-raising-funds-at-900b-valuation-topping-openai.html)
- [OpenAI — Introducing GPT-5.5](https://openai.com/index/introducing-gpt-5-5/)
- [Anthropic — Claude Opus 4.7 announcement](https://www.anthropic.com/news/claude-opus-4-7)
- [CNBC — DeepSeek V4 preview](https://www.cnbc.com/2026/04/24/deepseek-v4-llm-preview-open-source-ai-competition-china.html)
- [Computerworld — EU AI Act talks pushed to May](https://www.computerworld.com/article/4164963/eu-lawmakers-fail-to-agree-on-watered-down-ai-act-talks-pushed-to-may.html)
- [Artificial Analysis — GPT-5.5 leading model](https://artificialanalysis.ai/articles/openai-gpt5-5-is-the-new-leading-AI-model)
- [Crunchbase — Q1 2026 AI funding](https://news.crunchbase.com/venture/foundational-ai-startup-funding-doubled-openai-anthropic-xai-q1-2026/)
- [PYMNTS — Nvidia signals final investments](https://www.pymnts.com/artificial-intelligence-2/2026/nvidia-signals-final-investments-in-openai-and-anthropic/)
