# AI 行业日报 · 2026-04-28

## 今日焦点

> **MS-OpenAI 解绑 · 中国监管否决 Meta 收 Manus · Anthropic ARR 反超 OpenAI · 机器人融资再热 · GPT-5.5 涨价两倍**
>
> - **微软放手 OpenAI 多云销售**：双方修订协议，OpenAI 模型获准登陆竞争对手云平台，"独家通道"时代正式落幕
> - **北京叫停 Meta 收购 Manus**：中国发改委以违反外商投资规则为由要求撤销交易，AI 出海第一桩"被否"案出现
> - **Anthropic ARR $300 亿首超 OpenAI**：估值升至 $3,800 亿，Google 二次加码最高 $400 亿（首笔 $100 亿到账）
> - **Sereact 拿 $1.1 亿融资**：把"预测后果"塞进机器人推理回路，具身智能赛道资金不停
> - **GPT-5.5 定价 $5/$30**：首次完全重训基座模型，价格较 5.4 翻倍但 Terminal-Bench 2.0 上压过 Claude Mythos Preview

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | 微软-OpenAI 修订协议，OpenAI 可在第三方云销售模型 | CNBC / Reuters | ⭐⭐⭐⭐⭐ |
| 2 | 中国发改委叫停 Meta AI 收购 Manus | 官方公告 | ⭐⭐⭐⭐⭐ |
| 3 | Google 宣布最多 $400 亿投 Anthropic，估值 $3,800 亿 | TechCrunch | ⭐⭐⭐⭐⭐ |
| 4 | Anthropic ARR 突破 $300 亿，反超 OpenAI 的 $250 亿 | The Information | ⭐⭐⭐⭐⭐ |
| 5 | OpenAI 发布 GPT-5.5，1M 上下文，定价 $5/$30 | OpenAI 官方 | ⭐⭐⭐⭐ |
| 6 | Sereact 完成 $1.1 亿融资，做"会预测后果"的机器人模型 | Bloomberg | ⭐⭐⭐⭐ |
| 7 | Anthropic 把 Claude Mythos Preview 列为"战略防御资产"，仅限政府/可信伙伴 | VentureBeat | ⭐⭐⭐⭐ |
| 8 | Amazon 与 Anthropic 续签：最多再投 $250 亿做 AI 基建 | CNBC | ⭐⭐⭐⭐ |
| 9 | 智谱 GLM-5.1（744B MoE/MIT）SWE-Bench Pro 超 GPT-5.4 与 Claude Opus 4.6 | llm-stats | ⭐⭐⭐⭐ |
| 10 | 阿里 Qwen 3.6-Plus 上线，主打 agentic coding，1M 上下文 | 通义 | ⭐⭐⭐ |
| 11 | Nvidia GTC 2026 推 Agent Toolkit，17 家企业（Adobe/Salesforce/SAP）同步接入 | VentureBeat | ⭐⭐⭐⭐ |
| 12 | Google 对外发布企业 AI Agent 套件，正面挑 Anthropic/OpenAI | Bloomberg | ⭐⭐⭐ |
| 13 | EU AI Act 8 月 2 日全面适用倒计时，"不可接受风险"系统将禁 | 欧盟委员会 | ⭐⭐⭐⭐ |
| 14 | Broadcom 与 Google、Anthropic 扩大芯片合作 | CNBC | ⭐⭐⭐ |
| 15 | NeoCognition 获 $4,000 万种子轮，押注"像人一样学习的 agent" | TechCrunch | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · 微软放手，OpenAI 走向"多云时代"

**[CNBC: Microsoft and OpenAI amend partnership terms](https://www.cnbc.com/)** · **[Bloomberg coverage](https://www.bloomberg.com/)**

周一披露的修订条款核心一条：**OpenAI 的模型现在可以在 Azure 之外的云上销售**。这是 2019 年 Microsoft 投资 OpenAI 以来最重要的边界重划——独家算力+独家渠道这条护城河在双方之间正式被填平。配合 4 月 24 日 Google 宣布最多 $400 亿入股 Anthropic，整个"模型供应商-云厂商"格局已从"绑定一对一"切换到"多云任选+股权交叉"的网状结构。

短期最大受益方是 AWS、GCP、Oracle Cloud——它们终于可以把 OpenAI 模型作为一级公民直接卖给企业客户。中长期最值得关注的是 Microsoft：失去渠道独占后，它的 AI 商业故事必须靠 Copilot 应用层和自研模型（Phi、MAI 系列）说服股东继续投钱。OpenAI 这边则获得渠道自由+议价权，但代价是与 MSFT "命运共同体"叙事的弱化——投资人需要重新评估 OpenAI 的"独立性溢价"是利好还是利空。

**点评：** 当模型公司开始在多个云上同价售卖，"模型即水电"的商品化进程进入下半场；下一个分水岭会出现在 Anthropic 是否复制此举——若 Claude 也跨出 AWS/GCP，就意味着 LLM 厂商集体向"中立基础设施"角色靠拢。

---

### 🚀 No.2 · 北京一刀：Meta AI 收购 Manus 被否

**[Reuters/Caixin via 官方公告]** · **[techfundingnews 综合](https://techfundingnews.com/)**

4 月 27 日，中国国家发改委以"违反外商投资规则"为由叫停 Meta AI 对中国 AI 创业公司 Manus 的收购。这是中美 AI 资本流动近期最具标志性的"被否"事件——之前 OpenAI 和 Anthropic 的中国合作多以"自我审查"形式终止，而本次是监管端首次明确出手。

被否的不是技术，是结构。Manus 在 agentic browsing 与多步骤任务自动化上有一定声誉，被 Meta 收购意味着核心团队、客户数据与技术 IP 整体出境，这在当前数据安全与"关键技术外溢"语境下几乎无法通过审批。配合中国 9 月开始执行的合成内容标识、AI 服务备案与"安全评估/审计"要求，可以判断接下来两年中国 AI 公司被海外大厂直接并购的窗口将基本关闭，更多会以"技术授权+合资"形式出现。

**点评：** AI 时代的"芯片三角"开始延伸到模型与人才——监管否决买不来 GPU 之外，也会越来越频繁地否决"买不到的算法团队"；中国 AI 创业者的退出路径正被强制重构为本土 IPO 或战略合作。

---

### 🥇 No.3 · Anthropic 单季暴涨：ARR $300 亿首次反超 OpenAI

**[TechCrunch: Google to invest up to $40B in Anthropic](https://techcrunch.com/2026/04/24/google-to-invest-up-to-40b-in-anthropic-in-cash-and-compute/)** · **[Roborhythms: Anthropic Revenue 30B](https://www.roborhythms.com/anthropic-revenue-30-billion-2026/)**

Anthropic 披露：Run-rate revenue 从 2025 年底的约 $90 亿飙升至当前 $300 亿，单季节奏惊人。同期 OpenAI ARR 约 $250 亿——这是 Anthropic 在历史上首次在季度营收维度反超 OpenAI。背后两条曲线：一是企业客户数量在 2 月到现在不到两个月里翻倍，年化付费 $100 万以上的客户超过 1,000 家；二是 Claude Code 与 Skills 在开发者市场形成口碑级渗透。

Google 这次最多 $400 亿投资（首笔 $100 亿，估值 $3,800 亿，剩余与里程碑挂钩）配合 Amazon 此前最多 $250 亿的算力承诺，让 Anthropic 实质上成为"AWS+GCP 双云加持"的旗舰资产。这种"多金主+多云"结构与 OpenAI-MSFT 修约后的格局形成镜像，AI 巨头正在演化出两套不同治理范式：OpenAI 走"逐渐独立 IPO"路线，Anthropic 走"多金主战略合作"路线。

**点评：** 收入反超是一个分水岭事件，但更值得复盘的是模式之争——Anthropic 的"先服务企业、后做 ChatGPT"路径如今显示出现金流优势，对所有还在 ToC 烧钱的模型公司是直接警示。

---

### 🛠 No.4 · GPT-5.5 上线：第一款完全重训的 5.x 基座，价格翻倍

**[OpenAI 官方](https://openai.com/index/introducing-gpt-5-5/)** · **[VentureBeat](https://venturebeat.com/ai/openais-gpt-5-5-is-here-and-its-no-potato-narrowly-beats-anthropics-claude-mythos-preview-on-terminal-bench-2-0)**

GPT-5.5 于 4 月 23 日上线，是自 GPT-4.5 以来 OpenAI 第一款"完全重训的基座模型"，1M 上下文、定价从 GPT-5.4 的 $2.5/$15 直接跳到 $5/$30——这是 5.x 系列单次最大涨幅。基准上它在 Terminal-Bench 2.0（agentic 多步推理与工具使用）以微弱优势压过 Anthropic 的 gated 模型 Claude Mythos Preview，但在 Humanity's Last Exam（无工具）上 GPT-5.5 Pro 43.1% 落后于 Claude Opus 4.7（46.9%）和 Mythos Preview（56.8%）。

值得拆开两层读：第一，**OpenAI 把价格抬上去说明算力成本端依然在涨**，配合 Greg Brockman "我们在向 compute-powered economy 迁移、2030 年达到 30GW"的表态，这次涨价是基础设施成本传导的开始；第二，**Anthropic 把 Mythos Preview 划为"战略防御资产"**——只给政府和少数可信伙伴，理由是网络安全风险——这是头部实验室第一次以"安全"为由对最强模型实施配额制。两件事合起来意味着前沿模型正在分化成"商用版"和"国家级版"两个市场。

**点评：** 当最强模型变成"配给品"，价格更贵的中等强度模型（GPT-5.5、Opus 4.7）才是真实战场；下一阶段竞争焦点不再是 leaderboard 上的几个百分点，而是给企业的总持有成本（TCO）。

---

### 🤖 No.5 · Sereact $1.1 亿：让机器人"先想清楚后果再动"

**[Bloomberg: Sereact Raises $110M](https://www.bloomberg.com/news/articles/2026-04-27/ai-startup-sereact-raises-110-million-for-robots-that-predict-consequences)**

德国具身智能公司 Sereact 完成 $1.1 亿融资，主打把"后果预测"模型化——机器人在执行抓取/搬运/装配前，先用世界模型评估这个动作会让物体/环境进入哪个状态，再决定是否执行。这种思路区别于纯端到端 VLA（Vision-Language-Action）路线，更像 model-based RL 在工厂场景的回归。

配合 Nvidia GTC 2026 上推出的企业 Agent Toolkit（Adobe/Salesforce/SAP/ServiceNow 等 17 家首批接入），可以看出本月**软件 agent 和具身 agent 是同一波叙事**：都在解决"行动前要不要先三思"的工程问题。具身赛道的资金窗口仍然敞开，但筛选逻辑已经从"会动"卷到"动得明白"。

**点评：** "可解释、可预测的机器人决策"会成为下一年具身公司分胜负的关键——演示视频不再有溢价，工厂良率才是议价筹码。

---

## 行业观察

今日五条主线把 2026 年 Q2 的 AI 产业骨架拼了出来：**资本端**（Google $400 亿入 Anthropic、Amazon 续签 $250 亿、Sereact $1.1 亿）说明"AI 算力+模型+具身"的三段式投资不仅没冷却，还在加速；**渠道端**（MS-OpenAI 解绑、Anthropic 多云）让"模型即商品"成为既成事实，渠道独占叙事退场；**监管端**（中国否决 Meta-Manus、欧盟 AI Act 8 月 2 日生效倒计时）让跨境并购与高风险 AI 系统首次面临实质成本。

最值得记下的两个反转：**Anthropic ARR 反超 OpenAI**——商业化叙事被重写，"先 ToC 烧钱后变现"不再是唯一答案；**最强模型不再公开发布**（Claude Mythos Preview gated）——这是 LLM 时代第一次出现"前沿模型变战略物资"的官方表态，未来 6 个月可能催生类似芯片出口管制的"模型出口管制"政策讨论。

冷信号也别错过：Nvidia GTC 把 17 家 SaaS 龙头一起拉上 Agent Toolkit，意味着"AI 杀掉 SaaS"的极端叙事正在被"SaaS 老厂全面 agent 化"取代——ServiceNow $6 亿 agent 收入、Salesforce $1.7 亿且 YoY +800%——SaaS 公司已不是被颠覆方，而是 agent 时代最先吃到红利的群体。

