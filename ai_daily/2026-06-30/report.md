# AI 行业日报 · 2026-06-30

## 今日焦点

> **巨头估值军备 · 模型迭代节奏 · 欧盟监管落地 · 硬件并购暗战 · 企业 Agent 治理**
>
> - **Anthropic $965B 估值反超 OpenAI**：5 月底完成的 $65B H 轮后估值正式超过 OpenAI $852B，全球最贵 AI 独角兽易主。
> - **OpenAI GPT-5.5 全面铺开**：4 月发布的 GDPval 84.9%、OSWorld 78.7% SOTA 模型，进入企业大规模采购周期。
> - **欧盟 AI Act 8 月限期临近**：6 月 16 日 Parliament 通过 Digital Omnibus 修正案延期高风险条款，但透明度与水印规则 8 月 2 日如期生效。
> - **Qualcomm 谈判收购 Tenstorrent**：$8-10B 价位锁定 Jim Keller 团队 + RISC-V AI 芯片，正面狙击 Nvidia/AMD。
> - **Gemini 3.5 Pro 月底 GA 倒计时**：Vertex preview 还未结束，Pichai 承诺的 6 月窗口期只剩最后几小时。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Anthropic 估值反超 OpenAI 成全球最贵 AI 独角兽 | The Information / Bloomberg | ⭐⭐⭐⭐⭐ |
| 2 | OpenAI GPT-5.5 进入企业大规模部署期，GDPval 84.9% SOTA | OpenAI Blog | ⭐⭐⭐⭐⭐ |
| 3 | 欧盟 Parliament 通过 Digital Omnibus，AI Act 透明度规则 8/2 生效 | EU Commission | ⭐⭐⭐⭐⭐ |
| 4 | Qualcomm 早期谈判 $8-10B 收购 Tenstorrent | Reuters | ⭐⭐⭐⭐ |
| 5 | Gemini 3.5 Pro GA 倒计时，2M context + Deep Think 即将开放 | Google Blog | ⭐⭐⭐⭐ |
| 6 | xAI Grok 5 训练进入收尾，Polymarket Q2 发布概率仅 12-33% | xAI / Polymarket | ⭐⭐⭐ |
| 7 | EU Code of Practice on AI Content Transparency 发布 | EU Commission | ⭐⭐⭐ |
| 8 | Microsoft 7/1 全球涨价，捆绑 M365 Copilot 推升级 | Microsoft Partner Center | ⭐⭐⭐ |
| 9 | Meta 把 AI 使用与员工绩效奖金挂钩 | Fortune | ⭐⭐⭐ |
| 10 | Ames Lab DuctGPT 发现无稀土永磁材料新组合 | Nature | ⭐⭐⭐ |
| 11 | Anthropic Project Glasswing 联合 50 家伙伴做防御性网络安全 | Anthropic | ⭐⭐⭐ |
| 12 | OpenAI $122B 融资 case 已 closed，post-money $852B | OpenAI | ⭐⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Anthropic $965B 估值反超 OpenAI

**[The Information / Crunchbase](https://news.crunchbase.com/venture/record-breaking-funding-ai-global-q1-2026/)**

5 月底 close 的 $65B H 轮，给 Anthropic 锁定了 $965B 的 post-money 估值，正式超越 OpenAI 当前 $852B 的私募估值。两家头部公司估值差超过 $100B，反映出投资者对 Claude 在企业市场的渗透速度，以及 Anthropic 在 Computer Use / Agent / Safety 这条"难但护城河深"路线上的押注收益。

值得注意的是，Anthropic 这一轮估值倍数对应的 ARR 隐含倍数约为 60-70 倍——市场已经把它视为下一个"周期级别基础设施供应商"，而不是与 OpenAI 同框的纯模型公司。Project Glasswing 把 Claude 投入到防御性网络安全研究（限定 50 家伙伴）、以及对 Claude Mythos Preview 的限制访问策略，进一步强化了"高价高门槛 + 行业纵深"的定位。

接下来要关注的是 OpenAI 的反击——GPT-5.6 Sol 的 preview 已经被官方放出，下一个估值锚是它能否在 8 月前发布以撑住 IPO 节奏；同时 Anthropic 的下一个 Sonnet/Opus 版本能否在 Q3 之前推出，决定它能否守住"领先半个身位"的叙事。

**点评：** 估值反超只是开端，真正的考题是 Claude 能否在企业 ARR 上同步反超——否则资本市场迟早会给两家做"估值收敛"。

---

### 🚀 No.2 · OpenAI GPT-5.5 全面铺开，GDPval 84.9% 创纪录

**[OpenAI](https://openai.com/index/introducing-gpt-5-5/)**

虽然 GPT-5.5 正式发布是在 4 月 24 日，但 6 月底进入了企业大规模采购周期——价格 $5/$30 per million tokens（input/output）、1M context、128K max output。OpenAI 官方公布的关键 benchmark：

- **GDPval 84.9%**——44 个职业的 agent 工作能力
- **OSWorld-Verified 78.7%**——真实计算机操作环境
- **Tau2-bench Telecom 98.0%**——复杂客服工作流
- **OfficeQA Pro 54.1%** / **FinanceAgent 60.0%** / **投行建模 88.5%**

值得拉出来单看的是 OSWorld 78.7%——这是 computer use / agent 真实可部署性的最重要指标，意味着 GPT-5.5 已经具备了"替代初级知识工作者执行多步骤任务"的能力。GPT-5.5 的 cached input 价格 $0.50/M tokens，对长上下文 RAG 与 agent loop 极度友好。

**点评：** 比起 5.5 的发布本身，更值得关注的是 OpenAI 已在 Preview 5.6 Sol——这家公司打算把模型版本迭代彻底变成季度节奏。

---

### 🛡️ No.3 · 欧盟 Digital Omnibus 通过，AI Act 8/2 透明度规则如期生效

**[European Commission](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)**

6 月 16 日，欧盟 Parliament 通过 Digital Omnibus 修正案，部分高风险条款延期，但 8 月 2 日的透明度义务和水印要求**如期生效**。配套动作密集落地：

- **6/1**：60 人科学委员会 + Advisory Forum 正式成立
- **6/10**：Code of Practice on Transparency of AI-Generated Content 发布，含官方标签 icon 集
- **12/2**：对 8/2 前部署的 GenAI 系统强制 watermark；同日扩展禁止"nudifier"类应用

对中美 AI 公司的实际冲击：所有在欧盟提供 GenAI 服务的公司，**必须在 8 月 2 日前完成生成内容标签和元数据 watermark**——这不是"建议"，而是硬性条款。OpenAI、Anthropic、Google、xAI 都必须在剩下的 33 天内完成产品端改造。

**点评：** 美国在搞 preemption 还在国会扯皮，欧盟已经把规则刻进了 8 月 2 日的合规倒计时——这是中美 AI 公司今年最贵的一笔合规账。

---

### 🔧 No.4 · Qualcomm $8-10B 谈判收购 Tenstorrent

**[Reuters](https://www.reuters.com/technology/)**

Qualcomm 早期接触 Tenstorrent 的报价区间是 $8-10B。看点有三：

1. **Jim Keller**——AMD Zen、Apple A 系列、Tesla FSD 芯片的总师，给 Qualcomm 带来世界级 CPU/AI 芯片架构能力
2. **RISC-V**——Tenstorrent 是 RISC-V AI 加速器路线最激进的公司，对 Qualcomm 摆脱 ARM 授权依赖意义重大
3. **Nvidia/AMD 之外的第三极**——Qualcomm 在数据中心和 AI training 领域几乎没有积累，这笔收购等于"花钱买入场券"

这笔交易如果成，2026 年 H2 AI 芯片格局将从 "Nvidia 一家独大 + AMD 追赶 + ASIC 散兵" 演变为 "Nvidia + AMD + 高通-Tenstorrent 联合体 + 各家自研 ASIC"。

**点评：** 收购价对 Tenstorrent 而言其实偏低（之前估值峰值接近 $5B 但 ARR 不足以支撑），是 Qualcomm 趁着 AI 芯片估值阶段性回调出手——时机选得相当精准。

---

### 🧪 No.5 · Gemini 3.5 Pro GA 倒计时：2M context + Deep Think

**[Google DeepMind](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-5/)**

Pichai 在 I/O 上承诺的 "next month" GA 已经走到了月底最后一天。Gemini 3.5 Pro 官方确认的两个杀手锏：

- **2M token context window**——量产前沿模型中最大（OpenAI 1M、Anthropic 1M）
- **Deep Think reasoning mode**——专门处理长链推理

但官方 benchmark 和定价**仍未公布**。市场预期价格约 $15/$60 per million tokens（约 Flash 的 10 倍），未确认。Flash 在 Terminal-Bench 2.1、MCP Atlas、GDPval-AA、CharXiv 这些 coding/agent benchmark 上反而超过了 Gemini 3.1 Pro——这意味着 Pro 必须用长上下文 + Deep Think 拉开身位才能定价合理。

**点评：** Google 这次发布节奏比 OpenAI 慢了至少两个月，如果 6 月底再交不出 GA 和 benchmark，市场对 Gemini 3.5 Pro 的预期会迅速回归 "比 Flash 强一点的合理产品"。

---

## 行业观察

**估值游戏进入"千亿俱乐部"内部赛跑。** Anthropic $965B、OpenAI $852B、SpaceX 准备的 $1.75T IPO，AI 与航天双双进入"国家级基建估值"区间。这对二级市场和 LP 的资金分配是结构性冲击——传统软件 SaaS 与小型 AI 应用今年下半年融资压力会显著加大。

**模型层进入"季度迭代"节奏。** OpenAI GPT-5.4 → 5.5 → 5.6 Sol、Google Gemini 3.1 → 3.5、Anthropic Claude 4.x → Mythos，所有头部玩家都把发布节奏压到了 3 个月一档。对开发者意味着 prompt 与 fine-tune 投入的折旧周期被压缩到 90 天，对应用层是"基础能力红利持续"，对 benchmark 公司是黄金窗口。

**监管套利窗口正在关闭。** 欧盟 8 月 2 日透明度合规倒计时只剩 33 天，US 联邦 preemption 议案在国会卡住，州层面 AI 法仍在叠加生效。下半年 AI 产品出海欧盟的成本会显著上升——这对 Anthropic / OpenAI 等已有欧盟主体的玩家相对有利，对中国出海公司是新一轮 compliance tax。

**硬件并购窗口打开。** Qualcomm-Tenstorrent 之后，预期还有更多 AI 芯片二级公司被并购——AMD 之前已经吃掉 ZT Systems，Broadcom 与 Marvell 都在物色 RISC-V 路线标的。Nvidia 的护城河在硬件，但 AI 芯片"第三极"正在拼图。
