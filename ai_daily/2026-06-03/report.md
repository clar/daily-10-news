# AI 日报 · 2026-06-03

## 今日焦点

> **Anthropic 抢跑 IPO · Microsoft Build 重塑 Copilot 栈 · Agent 成为操作系统级原语 · EU AI Act 透明度倒计时**
>
> - **Anthropic 机密递交 S-1**：估值 965B 美元、ARR 47B 美元，AI 史上首家冲刺万亿市值的大模型公司，OpenAI 被反超。
> - **Microsoft Build 2026 全家桶**：自研编码模型 **Project Polaris** 8 月起替代 GPT-4 Turbo 成 Copilot 默认，Windows Agent Framework 1.0 以 MIT 协议开源。
> - **GitHub Copilot 改按 AI Credits 计费**：6/1 起所有套餐转向 usage-based，标志 IDE 时代向"用多少付多少"的 agent 经济转身。
> - **五角大楼 96.9 亿美元 Microsoft 合同**：史上最大 MS 政府订单，Pentagon 软件许可全面整合到 Azure + Copilot 平台。
> - **EU AI Act 透明度指南今日截止公众咨询**：6/3 收官，6 月公布最终 Code of Practice；高风险 AI 合规期延至 2027/12。

---

## 热点速览

| #  | 新闻标题 | 来源 | 重要度 |
|----|---------|------|--------|
| 1  | Anthropic 机密递交 IPO 招股书，965B 估值反超 OpenAI | CNBC / Fortune | ⭐⭐⭐⭐⭐ |
| 2  | Microsoft Build 发布 Project Polaris，自研代码模型取代 GPT-4 Turbo | Microsoft Build 2026 | ⭐⭐⭐⭐⭐ |
| 3  | GitHub Copilot 全面转 AI Credits 用量计费（6/1 生效） | GitHub Changelog | ⭐⭐⭐⭐ |
| 4  | 五角大楼授予 Microsoft 96.9 亿美元软件统一合同 | DoD / Microsoft | ⭐⭐⭐⭐ |
| 5  | Windows Agent Framework 1.0 以 MIT 协议开源 | Microsoft Build | ⭐⭐⭐⭐ |
| 6  | Azure Agent Mesh 上线，跨 AWS/GCP/On-Prem 编排 agent | Microsoft Build | ⭐⭐⭐⭐ |
| 7  | Claude Opus 4.8 上 Azure AI Foundry，与 GPT 同列一等公民 | Microsoft / Anthropic | ⭐⭐⭐⭐ |
| 8  | EU AI Act 透明度 Code of Practice 公众咨询 6/3 截止 | European Commission | ⭐⭐⭐⭐ |
| 9  | 美国财政部发布金融业 AI 风险管理框架（FS AI RMF） | U.S. Treasury | ⭐⭐⭐ |
| 10 | Shield AI 完成 15 亿美元 G 轮，估值 127 亿美元（一年涨 140%） | TechCrunch | ⭐⭐⭐ |
| 11 | Office 365 Copilot 全线默认 Agent Mode | Microsoft Build | ⭐⭐⭐ |
| 12 | Foundry Local 通用版上线，Windows/macOS/Linux 端侧推理统一 | Microsoft Build | ⭐⭐⭐ |
| 13 | Colorado AI Act 6/30 正式生效，覆盖高风险系统 | Cooley LLP | ⭐⭐⭐ |
| 14 | 联邦 AI 采购额 72 亿美元（YoY +966%），DoD 主导 1319 单合同 | Brookings | ⭐⭐⭐ |
| 15 | Kimi K2.6 / DeepSeek V4 / Qwen 3.6 持续逼近前沿，开源差距压至日级 | TokenMix / RadarAI | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Anthropic 机密递交 IPO，万亿市值近在咫尺

**[CNBC](https://www.cnbc.com/2026/06/01/anthropic-ipo-s1-prospectus.html) · [Fortune](https://fortune.com/2026/06/01/anthropic-confidentially-files-ipo-965-billion-valuation/) · [TechCrunch](https://techcrunch.com/2026/06/01/anthropic-files-to-go-public/)**

6 月 1 日，Anthropic 向 SEC 机密递交 S-1，距离它刚完成 H 轮 650 亿美元融资、把估值推到 9650 亿美元仅 5 天。这把 OpenAI（3 月底估值 8520 亿美元）抛在了身后，让 Claude 母公司一举成为 AI 历史上第一家正式排队上市的前沿实验室。

更耀眼的是收入曲线：ARR 已从一年前的 100 亿美元飙到 470 亿美元，几乎四倍增长，与 OpenAI 拉开了"复利级差距"。市场普遍认为，只要二级市场不出大事，挂牌即破万亿是基本盘——这意味着 IPO 当天 AI 会诞生一家市值堪比 Meta 的新公司。

但风险同样写在脸上：自由现金流仍然为负、训练算力支出（包括 Anthropic 自己披露的多年期 TPU 协议）会持续吞噬利润、监管层对超大规模 AI 公司公开上市后的信息披露要求几乎没有先例。如果 SEC 在公司治理、安全披露、数据合规上提出额外要求，挂牌时间可能滑到 2027。

**点评：** 这不只是融资动作，是 AI 行业"成熟期"的开关被按下——一旦 Anthropic 站上公开市场，再融资能力、估值锚、人才股权都会进入新维度，OpenAI 必须跟进，否则就是在被动让出资本叙事。

---

### 🚀 No.2 · Microsoft Build：自研模型 + 开源 Agent 框架双管齐下，Copilot 栈彻底重排

**[Build Fast with AI](https://www.buildfastwithai.com/blogs/ai-news-today-june-2-2026)**

Microsoft Build 2026 在 6 月 2 日抛出三颗深水炸弹：

1. **Project Polaris** —— 自研代码模型，8 月起接替 GPT-4 Turbo 成为 GitHub Copilot 默认模型，跑在 Azure 自研 Maia 200 加速器上，并保留三个月 OpenAI 模型回退期。
2. **Windows Agent Framework 1.0** —— MIT 协议开源，覆盖 PC、Cloud PC 与边缘设备，自带特权操作的人类审批队列。
3. **Azure Agent Mesh** —— 跨 Azure/AWS Bedrock/Google Cloud/本地系统统一编排 agent，Entra ID + Purview 做身份和审计。

这套组合拳的真实含义是：Microsoft 在系统性"去 OpenAI 化"。Copilot 这条价值数百亿美元的护城河里，OpenAI 的位置正在被替换为"OpenAI + Anthropic + 自研 + 任意开源"的多模型池，而 Azure AI Foundry 已经把 Claude Opus 4.8 与 Sonnet 4.6 当成一等公民同框上架。

对开发者而言，这是去年 Copilot 改为 AI Credits 计费的逻辑闭环——既然你按用量付钱，那 Microsoft 就有动力把每一次 token 调用替换成成本更低、毛利更高的自有模型。Polaris 不是替代 GPT-4 Turbo，是替代"按调用付给 OpenAI 的钱"。

**点评：** OpenAI-Microsoft 联盟正在从蜜月期切换到对手期，Build 2026 是双方关系结构性松动的明确信号，2027 年的 Copilot 大概率会是"以 Microsoft 为中心、OpenAI 作为可选项"的格局。

---

### 🧱 No.3 · GitHub Copilot 改按 AI Credits 计费：开发工具进入 token 经济

**[GitHub Changelog](https://blog.mean.ceo/ai-agents-news-june-2026/)**

6 月 1 日起，所有 Copilot 套餐统一切到 GitHub AI Credits 按量计费，并新增用户级预算控制。这件事看似只是计费调整，实际是开发者工具行业的"AWS 时刻"——从过去 IDE 时代的"每月 19/39 美元订阅"，正式转向"按 token 付费 + 预算护栏"的云原生定价。

为什么必须这么做？Copilot 已经从"代码自动补全"演化成"在 Workspace 里跑一整夜 SRE agent 监控生产系统"。前者每月调用 10 万 token，后者一晚就是百万级。原本的统一订阅价彻底压不住成本结构，特别是 Polaris、Claude 4.8、GPT-5.5 多模型并行的情况下。

边际影响极大：（1）企业 procurement 模式将完全重写，要从"买席位"变成"管预算"；（2）大量 SaaS 工具会跟进，把订阅价改成"基础订阅 + 量价分离"；（3）Anthropic、OpenAI 的 API 毛利空间被进一步压缩，因为 GitHub 现在可以在后端无缝替换最便宜的模型。

**点评：** Token 经济从 API 用户蔓延到了 IDE 用户，下一站是 SaaS 用户。"按席位卖软件"这个延续 30 年的范式，正式被 agent 时代冲垮。

---

### 🛡️ No.4 · EU AI Act 透明度 Code of Practice 截止 + 高风险合规延期

**[European Commission](https://digital-strategy.ec.europa.eu/en/news/ai-act-enforcement-gets-independent-expert-support) · [Latham & Watkins](https://www.lw.com/en/insights/ai-act-update-eu-resolves-to-change-rules-and-extend-deadlines)**

今天（6/3）是欧盟委员会透明度 Code of Practice 公众咨询的最后一天，最终版预计 6 月内公布。同时 5/7 政治协议确认了几件大事：高风险 AI 系统（Annex III）合规义务从 2026/8/2 推迟到 2027/12/2；合成内容机器可读标识义务延至 2026/12/2；非自愿亲密内容的 AI 生成与操纵被列入新禁项（2026/12/2 生效）。

欧盟也同步搭起了执法骨架：60 位独立专家组成的 Scientific Panel 与 Advisory Forum 上线，专注通用 AI 模型、系统性风险与跨境市场监督——这意味着 EU AI Office 终于不再是"纸上立法、无人执法"。

对前沿实验室是一波喘息时间，但对欧洲本土合规咨询、第三方评估机构是高确定性的增长窗口。从产品角度，下半年所有部署到欧盟市场的合成内容必须支持 C2PA 风格的水印——这是 OpenAI、Google、Meta 必须上的项目。

**点评：** 欧盟给了行业延期，但条件是"换更严的禁项 + 真正的执法机构"，这是典型的布鲁塞尔式妥协——慢一点、但更硬。

---

### 💰 No.5 · 五角大楼 96.9 亿美元 Microsoft 合同：政府 AI 采购的范式重置

**[Federal News Network](https://federalnewsnetwork.com/reporters-notebook/2026/01/ai-may-not-be-the-federal-buzzword-for-2026/) · [Brookings](https://www.brookings.edu/articles/where-does-federal-ai-spending-stand-in-2026/)**

DoD 与 Microsoft 签下 96.9 亿美元的软件统一合同，覆盖 Microsoft 365、Azure 与 Copilot 全线服务，估计节省 4.22 亿美元——这是 Microsoft 史上最大政府订单。背后是更大的趋势：2026 年联邦 AI 采购金额从 2024 年的 7 亿暴增到 72 亿（+966%），潜在合同上限 918 亿（+1912%），DoD 一家拿下 1319 单。

这件事告诉行业三件事：（1）政府 AI 不再是"试点"，而是按千亿规模做长期采购；（2）"超大企业平台 + 整合 agent"才是政府能接受的形态，单点 SaaS 越来越难独立中标；（3）地缘安全语境下，自主可控的云栈（Azure Government、AWS GovCloud）和自有模型是必须项——这反向加固了 Microsoft Polaris 的战略意义。

**点评：** AI 行业的钱不只来自 VC 和企业 SaaS 订单，2026 年起政府是和云大厂同等量级的现金牛，而且锁定期更长、单笔更大。

---

## 行业观察

今天的几条线索拼起来，是 AI 行业进入"基础设施级整合期"的清晰画面：

1. **资本叙事完成代际切换。** Anthropic 把 IPO 推到桌面意味着前沿 AI 公司估值锚正在从一级市场过渡到二级市场。下一步是 OpenAI 的快速跟进，以及 xAI、Mistral、Cohere 的估值重定价。
2. **模型层加速去中心化，但应用层加速集中化。** 模型供给端越来越多（Claude/GPT/Gemini/Polaris/Llama 5/Kimi K2.6/DeepSeek V4），但分发端在 Microsoft、Google、AWS、GitHub 四家手里收紧——agent 编排平台才是兵家必争。
3. **计费从"席位"变成"token + 预算"。** GitHub Copilot 的 6/1 切换不是个例，它是接下来 18 个月所有 SaaS 的模板：基础订阅打底 + agent 用量超额计费。
4. **监管节奏与商业节奏正式同步。** 欧盟透明度 Code of Practice、Colorado AI Act 6/30 生效、美国财政部 FS AI RMF 同时落地，AI 合规第一次成为产品发布同等优先级的工作流。
5. **资本支出的"重力锚"正在形成。** Anthropic 多年期 TPU 订单、Meta 480 亿美元 GPU 投入、Microsoft 自研 Maia 200——前沿 AI 公司的资产负债表正在变得越来越像电信公司，而不是软件公司，这是 IPO 前必须解释清楚的故事。

接下来 7 天值得盯的事：OpenAI 是否官宣跟进 IPO、Gemini 3.5 Pro 发布窗口、Code of Practice 终稿、Nvidia Q1 财报后的算力需求指引。
