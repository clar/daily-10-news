# AI 日报 · 2026-04-27

## 今日焦点

> **OpenAI 史诗级 1220 亿美元融资 · Google 砸 400 亿"绑定"Anthropic · Cognition 估值翻倍至 250 亿 · Anthropic Mythos 危险模型被攻破 · DeepSeek V4 重写大模型成本曲线**
>
> - **OpenAI 收官 1220 亿美元，估值 8520 亿** Amazon、英伟达、软银三家做主投，AI 资本进入"国家级支票"时代
> - **Google 注资 Anthropic 高达 400 亿美元** 现金加算力，估值锚定在 3500 亿，云厂商版图战正式定型
> - **Cognition (Devin) 谈 250 亿美元估值** 一年内估值 6 倍跳，AI Coding 赛道继续吸金
> - **Anthropic Mythos 模型被未授权访问** 这款"太危险不能公开"的零日漏洞挖掘 AI 在公布当日就漏出
> - **DeepSeek V4 / V4-Pro / V4-Flash 集中发布** 与华为昇腾深度绑定，把闭源前沿模型再压一档价

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | OpenAI 完成 1220 亿美元融资，估值 8520 亿美元 | OpenAI / Bloomberg | ⭐⭐⭐⭐⭐ |
| 2 | Google 拟向 Anthropic 投资 400 亿美元（现金 + 算力） | TechCrunch / Bloomberg | ⭐⭐⭐⭐⭐ |
| 3 | Anthropic Mythos 模型被未授权第三方访问 | Fortune / TechCrunch | ⭐⭐⭐⭐⭐ |
| 4 | DeepSeek 发布 V4-Pro 与 V4-Flash，与华为芯片深度集成 | Fortune | ⭐⭐⭐⭐ |
| 5 | Cognition (Devin) 谈 250 亿美元估值新一轮融资 | Bloomberg | ⭐⭐⭐⭐ |
| 6 | Google 推出全新企业 AI Agent 工具集，对位 Anthropic/OpenAI | Bloomberg | ⭐⭐⭐⭐ |
| 7 | OpenAI 推出"ChatGPT for Clinicians"免费版 | OpenAI | ⭐⭐⭐ |
| 8 | xAI 推出 Grok 4.3，性能逼近 GPT-5.5 | What LLM | ⭐⭐⭐ |
| 9 | Moonshot AI 发布 Kimi K2.6，长上下文进一步拉升 | LLM-Stats | ⭐⭐⭐ |
| 10 | Meta 发布并购 Scale AI 后首款主力大模型 | CNBC | ⭐⭐⭐ |
| 11 | EU AI Act 8 月 2 日全面执法节点临近，企业合规倒计时 | OneTrust / Pearl Cohen | ⭐⭐⭐⭐ |
| 12 | Q1 2026 全球 VC 资金 81% 流向 AI 板块 | Crescendo AI | ⭐⭐⭐ |
| 13 | Era 融资 1100 万美元做"AI 硬件软件平台" | TechCrunch | ⭐⭐ |

---

## 深度点评

### 🏆 No.1 · OpenAI 一笔 1220 亿美元收官，估值锚定 8520 亿

**[OpenAI 官方公告](https://openai.com/index/accelerating-the-next-phase-ai/)**

OpenAI 宣布完成 1220 亿美元承诺资金的融资，投后估值 8520 亿美元。本轮由 Amazon、NVIDIA、SoftBank 共同领衔，微软继续追加，a16z、D.E. Shaw Ventures、MGX、TPG 联合主投。和过去几轮"边谈边融"的节奏不同，这一轮以"一次性敲定 + 阶段性出资"模式锁定，意图很清楚——把未来三年的算力资本一次抽干。

8520 亿美元这个估值已经超过了沙特阿美之外的多数全球能源巨头，把 OpenAI 与 Anthropic、xAI 拉开三个数量级的资金势能。更重要的是这次的投资人组合：Amazon（AWS）+ NVIDIA（GPU）+ SoftBank（资本 + 日韩能源）三方坐定主投，意味着 OpenAI 已经把全球最稀缺的三种生产要素——云、芯片、电力——全部绑成股东。

这对竞争对手的影响在于："纯模型公司"这条路实质上已经走不通了，剩下的赛道全部要拼"基础设施联盟"。

**点评：** OpenAI 这次拿到的不是钱，是把全球 AI 产业链的关键节点都变成了它的股东——这才是真正的护城河。

---

### 🚀 No.2 · Google 加注 Anthropic 400 亿美元，估值锁 3500 亿

**[TechCrunch](https://techcrunch.com/2026/04/24/google-to-invest-up-to-40b-in-anthropic-in-cash-and-compute/)**

Google 计划向 Anthropic 投资最多 400 亿美元，其中 100 亿美元立即注资，按 Anthropic 3500 亿估值入股；剩余 300 亿美元在达成业绩里程碑后分批注入。形式包含现金与 Google Cloud TPU 算力两部分。这是 Google 在 Anthropic 上累计的第三轮重投，使其继 Amazon 之后成为另一关键股东。

这件事的战略意义远远超过金额本身。Google 一边自己推 Gemini 3.x 和 AI Agent 产品集（4 月 22 日刚发了一批针对企业的 Agent 工具），一边在 Anthropic 持续加码——本质上是在做"双轨对冲"：自家模型保住搜索/广告闭环，Anthropic 则用来覆盖 Claude Code、Skills 这种已经赢得开发者心智的赛道。

更要命的是这笔钱里有相当一部分是"算力承诺"，意味着 Anthropic 接下来扩张主力会越来越深地跑在 Google TPU 上——这与 Amazon Trainium 的早期承诺形成结构性冲突。Anthropic 实际上正在变成"两大云厂商共同博弈的中立模型公司"，独立性会持续受压。

**点评：** Google 这步棋的真正目标不是 Anthropic，而是让 OpenAI 在和 Microsoft 的捆绑里失去"唯一前沿模型供应商"的奇货可居地位。

---

### 🚨 No.3 · Anthropic Mythos 模型公布当日即被未授权访问

**[Fortune](https://fortune.com/2026/04/23/anthropic-mythos-leak-dario-amodei-ceo-cybersecurity-hackers-exploits-ai/)**

Anthropic 4 月 7 日宣布的 Claude Mythos Preview——一款官方自评"过于危险不应公开"的网络安全模型——在公布当日就被一群未授权用户接入。该模型据称能够独立发现 OS 与浏览器的零日漏洞，甚至能把多个浏览器漏洞链起来打破渲染层与系统沙箱。

入侵路径相当低级：一名第三方承包商在 Anthropic 的 vendor 环境里有合法访问权，攻击者基于此前从 AI 训练公司 Mercor 泄露出的 Anthropic 命名规律，"猜中了" Mythos 的 API URL。这把 Anthropic 一直引以为豪的"负责任披露 + 受限发布"叙事，撕开了一道 PR 上很难补的口子——你说它危险所以不公开，但你自己的运维边界又守不住。

更深远的影响是关于"前沿模型使用谁的供应链"这件事。Mercor 的训练数据合作、第三方承包商体系，这些过去半年里 AI 公司高速扩张的支撑系统，正在被验证为新的攻击面。可以预期，下半年监管视角会从"模型能不能力封顶"转向"训练与部署链路如何审计"，EU AI Act 8 月执法节点也会强化这个方向。

**点评：** 这次事故证明，前沿模型的安全风险不是来自"模型自身能力跑超控"，而是来自我们这些拿薪水的人类。

---

### 🌊 No.4 · DeepSeek V4 三连发，把开源前沿模型按到地板价

**[Fortune](https://fortune.com/2026/04/24/deepseek-v4-ai-model-price-performance-china-open-source/)**

DeepSeek 在上周五一口气发布 V4、V4-Pro、V4-Flash 三个版本：V4 主打 1.6T 参数的开源前沿能力，V4-Pro 自称在多项评测上比肩闭源顶尖模型，V4-Flash 是更小、更便宜的边缘部署版。三款模型都与华为昇腾芯片做了深度集成，是本轮中国国产链路替代 NVIDIA 的最大一次产品化展示。

DeepSeek 这次发布的真正杀招是定价：V4-Flash 的 token 单价被压到了远低于 GPT-5.5 与 Claude 4.6 Sonnet 的水平，重写了大模型 API 的成本曲线。结合"昇腾 + DeepSeek"这套自主链路，意味着中国国内场景将出现一条"性能不弱于 80% GPT-5.5 但成本只到 1/4"的可用方案。海外开发者也会被这个定价拉走相当一部分价格敏感的 batch / RAG 工作负载。

对 Anthropic 的影响最直接：Claude Code 等工作流型产品依赖大量推理调用，如果 DeepSeek V4 + Skills 兼容生态成熟，"前端用 Claude Code、后端跑 DeepSeek"的混合范式会进一步抬头（参考今天 GitHub 趋势榜上的 free-claude-code）。

**点评：** OpenAI 和 Anthropic 在拼"上限"，DeepSeek 在拼"下限"——大模型市场正在被劈成两个不联通的世界。

---

### 💸 No.5 · Cognition 谈 250 亿美元估值，AI Coding 赛道继续狂飙

**[Bloomberg](https://www.bloomberg.com/news/articles/2026-04-23/ai-coding-firm-cognition-in-funding-talks-at-25-billion-value)**

Cognition（AI 软件工程师 Devin 的母公司）正洽谈一轮新融资，估值 250 亿美元——较 2025 年 9 月的 102 亿美元翻倍多，较 2025 年 3 月的 40 亿美元跳了 6 倍。Devin 的 ARR 从 2024 年 9 月的约 100 万美元，飙到 2025 年 6 月的 7300 万美元。

如此跳变的估值轨迹反映的是赛道整体重估：去年还在质疑 Devin 是 demo 公司的投资人，今年发现 Cursor、Cognition、Codeium、Replit 等都在做"用 Agent 替代真实工程师工作流"的规模化变现。叠加 Cognition 收购 Windsurf 后产品线扩张到 IDE 端，市场把它当成了"OpenAI/Anthropic 之外的第三极候选"在投。

但风险也很明显：Coding Agent 是目前 Claude / GPT 模型能力最直接受益的应用层，Anthropic 自己就在持续把 Claude Code 越做越深，Skills 机制甚至开始让"垂直 Agent 工具"被部分平替。Cognition 这种"应用层独角兽"如果不能在产品差异化（比如长程任务记忆、企业级权限模型）上拉出明显护城河，估值兑现会很难。

**点评：** AI Coding 赛道现在是热钱最密集的应用层，但 Anthropic / OpenAI 自己直接下场做这条赛道的概率正在快速上升。

---

## 行业观察

今天的几条头条把 2026 年 AI 产业的两条主线全部摊开来了：

**第一条线：基础设施战争已经盘整完毕。** OpenAI 拿下 Amazon + NVIDIA + SoftBank 三方支票，Google 用 400 亿"双轨绑定" Anthropic，DeepSeek 用昇腾把中国国产链路打通——三大阵营各自把"模型 + 算力 + 资本"绑死，未来 18 个月不会再有显著的格局变化，剩下都是兑现。

**第二条线：应用层正在从"卖模型"切换到"卖工作流"。** Cognition 250 亿估值、Composio 推 Codex Skills、Anthropic Skills 生态飞轮——投资人和开发者都在用钱投票，承认"价值正在从 token 价格转向工作流粘性"。这也是为什么 Claude Code 的 Skills 机制接下来会变成最具战略意义的产品功能。

**风险面：Anthropic Mythos 事件是个重要分水岭。** 它会让 EU AI Act 在 8 月 2 日执法节点上把"供应链审计"加到首要议程，也会让企业 SOC 团队开始把 LLM 部署边界纳入第三方风险评估范围。前沿模型公司接下来的合规成本，会比过去任何一年都重。

Sources:
- [OpenAI](https://openai.com/index/accelerating-the-next-phase-ai/)
- [TechCrunch — Google to invest up to $40B in Anthropic](https://techcrunch.com/2026/04/24/google-to-invest-up-to-40b-in-anthropic-in-cash-and-compute/)
- [Fortune — Anthropic Mythos leak](https://fortune.com/2026/04/23/anthropic-mythos-leak-dario-amodei-ceo-cybersecurity-hackers-exploits-ai/)
- [Fortune — DeepSeek V4](https://fortune.com/2026/04/24/deepseek-v4-ai-model-price-performance-china-open-source/)
- [Bloomberg — Cognition $25B funding talks](https://www.bloomberg.com/news/articles/2026-04-23/ai-coding-firm-cognition-in-funding-talks-at-25-billion-value)
- [Bloomberg — Google AI Agents](https://www.bloomberg.com/news/articles/2026-04-22/google-releases-new-ai-agents-to-challenge-openai-and-anthropic)
- [Pearl Cohen — EU AI Act guidance](https://www.pearlcohen.com/new-guidance-under-the-eu-ai-act-ahead-of-its-next-enforcement-date/)
