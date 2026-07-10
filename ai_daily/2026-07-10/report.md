# AI 日报 · 2026-07-10

## 今日焦点

> **三大前沿模型同日公开 · 出口管制"18 天风波"落幕 · AI 融资从模型转向基建 · 欧盟高风险条款推迟两年**
>
> - **GPT-5.6 全家桶登陆公众市场**：OpenAI 在获得政府审查放行后，Sol / Terra / Luna 三档同时开放，Sol 新增 "ultra 模式"，可在单请求内调度子代理。
> - **首次"三家前沿模型同日发布"**：GPT-5.6、Grok 4.5、Sonnet 5 均在 7 月 9 日前后可公开使用，Sol 综合分 86，Grok 4.5 以 1/5 定价打价格战。
> - **Anthropic 双喜临门**：出口管制解除，Fable 5 全球恢复；Sonnet 5 以 $2/$10 入门价直奔 Opus 4.8 性能。
> - **Together AI 8 亿美元 C 轮**：Aramco 领投，NVIDIA 跟投，公有云容量 5 年扩 50 倍，年 booking 已破 11.5 亿美元。
> - **EU AI Act 让步**：独立高风险 AI 系统合规期延至 2027 年 12 月，嵌入式高风险产品延至 2028 年 8 月。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | OpenAI 公开发布 GPT-5.6 Sol / Terra / Luna | CNBC / OpenAI | ⭐⭐⭐⭐⭐ |
| 2 | xAI Grok 4.5 同日上线，宣称 Opus 级性能、5 倍便宜 | The Decoder | ⭐⭐⭐⭐⭐ |
| 3 | Anthropic Sonnet 5 上线，$2/$10 定价至 8/31 | Anthropic | ⭐⭐⭐⭐⭐ |
| 4 | 美国解除 Claude Fable 5 / Mythos 5 出口管制 | CNBC | ⭐⭐⭐⭐ |
| 5 | Together AI 8 亿美元 C 轮，估值破 100 亿 | StartupHub.ai | ⭐⭐⭐⭐ |
| 6 | 欧盟正式敲定 AI Act 高风险条款延期 | Consilium | ⭐⭐⭐⭐ |
| 7 | Kling AI 20 亿美元融资，估值 180 亿 | Crunchbase | ⭐⭐⭐⭐ |
| 8 | Google NanoBanana 2 Lite：4 秒出图，$0.034/千张 | Google | ⭐⭐⭐ |
| 9 | OpenAI 发布 GPT-Live 语音模型，可听说并行 | OpenAI | ⭐⭐⭐ |
| 10 | Crusoe 谈判 30 亿美元融资，估值将翻三倍至 180 亿 | Crunchbase | ⭐⭐⭐ |
| 11 | Menlo Ventures 靠 Anthropic 押注拿下 50 年最大基金 | Crunchbase | ⭐⭐⭐ |
| 12 | Nvidia 推出"AI 工厂"分成模式，绑定新云玩家 | NVIDIA | ⭐⭐⭐ |
| 13 | Taktile 1.1 亿美元由 Goldman Sachs 领投，做 Agent-First 银行 | PYMNTS | ⭐⭐⭐ |
| 14 | Fable 5 复出携新版越狱防护框架 | Anthropic | ⭐⭐⭐ |
| 15 | Terminal-Bench 2.0：Sol 91.9% vs Grok 4.5 83.3% | Artificial Analysis | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · 三家前沿模型同日发布，AI 竞赛进入"周更"时代

**[CNBC — OpenAI to publicly release GPT-5.6](https://www.cnbc.com/2026/07/08/openai-expanding-gpt-5point6-ai-model-release-ending-government-limits.html)**

7 月 9 日，OpenAI 正式向公众开放 GPT-5.6 三个版本——Sol（前沿推理/长时代理）、Terra（性能对标 GPT-5.5 但成本减半）、Luna（速度和成本最低）。三个月前，白宫签发的 AI 网络安全令要求前沿模型在发布前 30 天供政府审查，Sol 因此在 6 月底只对"少数受信合作方"开放；本次上线意味着首个走完官方红队流程的一线模型。同一天，xAI 上线 Grok 4.5，Anthropic 的 Sonnet 5 也在早些时候可用——这是 AI 史上**第一次三家前沿实验室在同一天拥有可公开访问的新一代前沿模型**。

从跑分看，Sol 综合分 86，Grok 4.5 为 82，Sol 在 Terminal-Bench 2.0 上以 91.9% 大幅领先 Grok 4.5 的 83.3%；但价格差距同样惊人——Sol 定价 $5/$30，Grok 4.5 只要 $2/$6，且 xAI 声称 Grok 4.5 在 SWE Bench Pro 上比 Opus 4.8 少用 4.2 倍 token。Sol 独家的"ultra 模式"允许在单请求内启动子代理，直接把"代理编排"下沉到模型层。

值得关注的是 GPT-5.6 引入"最高推理档"，等同于给 Sol 一个"想到累"的开关。这是继 o1 之后 OpenAI 在"扩推理时间即扩智能"路线上再走一步——但已经不是新剑，而是老兵新甲。

**点评：** 当三家前沿模型同日发布成为可能，一个时代结束了——"下一代模型"不再是稀缺事件，而是季度节拍；真正的护城河从模型参数转向能不能拿到政府红队通行证，以及每千 token 是 $30 还是 $6。

---

### 🚀 No.2 · Anthropic "18 天风波"落幕：出口管制解除 + Sonnet 5 强势入市

**[Axios — Anthropic's Fable 5 is back after Trump admin lifted export controls](https://www.axios.com/2026/07/01/anthropic-fable-5-back-online-trump-export-controls-lifted)**

7 月 1 日，美国商务部解除 Claude Fable 5 和 Mythos 5 的出口管制，Anthropic 立刻在全球范围重新部署 Fable 5，同时正式发布 Claude Sonnet 5——"迄今最具代理性的 Sonnet 模型"，能自主构建计划、操作浏览器/终端、执行多步任务。定价上，Sonnet 5 以 8 月 31 日前 $2/$10 的入门价切入市场，性能"接近 Opus 4.8"。

这场 18 天的停摆始于 6 月 12 日：Amazon 研究员公开了一份报告，展示如何绕过 Fable 5 的护栏让其识别软件漏洞、甚至给出利用代码，随后白宫援引"国家安全权限"要求 Anthropic 断开这两款模型的对外访问。Anthropic 用不到三周时间上线了"新版行业越狱防护框架"，并在恢复公告中着重强调了"更强的网络安全护栏"。

从竞争层面看，Sonnet 5 在 Grok 4.5、GPT-5.6 之前抢到市场空窗，$2 输入价拿到"近 Opus"性能，是 Anthropic 应对"两家同日发布"的最直接武器；而 Fable 5 的重新可用意味着在 Claude Code / Claude.AI 上，Anthropic 已经补齐前沿→中端→高性价比的完整梯队。

**点评：** Amazon 揭护栏破洞、政府 18 天叫停、Anthropic 补上安全模块再上线——一整套流程走完，前沿实验室与政府的"红队舞步"正式跳出了标准动作。

---

### 💰 No.3 · Together AI 8 亿 C 轮 & Menlo 靠 Anthropic 押注拿下 50 年最大基金

**[StartupHub.ai — Four of every five dollars went to AI infrastructure](https://www.startuphub.ai/ai-news/ai-news/2026/ai-infrastructure-week-july-6-2026)**

7 月 1 日，Together AI 完成 8 亿美元 C 轮，由 Aramco Ventures 领投，NVIDIA、Vista Equity、General Catalyst 跟投。公司披露 Q2 年度 booking 已破 11.5 亿美元，融资将用于**5 年内把公有云容量扩 50 倍**——这是把开源模型托管从"选项"变成"云原生新品类"的一次重资本表态。

同一周，Crusoe 传出与投资人商谈 30 亿美元融资，估值将从 60 亿翻三倍至 180 亿；Kling AI（视频生成）拿下 20 亿美元，General Atlantic 领投，估值 180 亿；Menlo Ventures 靠一笔早期 Anthropic 押注拿下 50 年基金史上最大规模的新募资。

行业数据也在验证叙事：本周 80% 的 AI 融资都进了基础设施；美国以外的 AI 融资占比降到 12%——资本流向已经完全被"美国+算力+基座"三个词绑定。

**点评：** 当风投的 IRR 靠一笔 Anthropic 押注定义、Aramco 石油钱进 Together AI、油和 GPU 用同一张 P&L 表——AI 基建已经完成从科技资产到全球宏观资产的身份转变。

---

### 🇪🇺 No.4 · 欧盟 AI Act 让步：高风险条款推迟两年，行业松了一口气

**[Council of the EU — Green light to simplify AI rules](https://www.consilium.europa.eu/en/press/press-releases/2026/06/29/artificial-intelligence-council-gives-final-green-light-to-simplify-and-streamline-rules/)**

6 月 29 日欧盟理事会终审通过"Digital Omnibus"简化包，7 月正式生效：原本 2026 年 8 月 2 日强制生效的高风险 AI 系统条款——独立系统延至 **2027 年 12 月 2 日**，嵌入式高风险 AI 产品延至 **2028 年 8 月 2 日**。8 月生效的仅剩透明度义务（AI 生成内容标注、聊天机器人身份披露）。同时新增了一条禁止性条款：明确禁止 AI 生成非自愿性内容和 CSAM。

对全球厂商而言，这次让步的意义远大于条款本身：欧盟第一次在 AI 立法上因"合规准备不足"公开调整时间表，说明"欧洲式重监管"的自信正在被"实施可行性"打折。这对 Anthropic、OpenAI 等美国厂商是明确利好——原本 8 月要交的合规文件推迟 16 个月，可以把资源转投模型迭代。

另一边，美国 3 月已发布"州法优先联邦轻监管"框架，越来越像"欧盟收紧透明度、美国收紧安全审查、中国收紧准入"的三向分化。

**点评：** 欧盟第一次向 AI 行业"低头"，本质是承认"合规滞后于模型迭代"；接下来两年，谁的合规成本更低，谁就赢一半。

---

### 🎙️ No.5 · GPT-Live 与 NanoBanana 2 Lite：多模态战线开辟"秒级+便宜"新赛道

**[LLM-Stats — AI Updates July 2026](https://llm-stats.com/llm-updates)**

除了 Sol，OpenAI 顺势发布 GPT-Live 语音模型，能"听说并行"，把 30 秒延迟压到子秒级，直接对标 ElevenLabs 和 Retell AI 的实时电话代理场景。Google 那边，NanoBanana 2 Lite 以 4 秒出图 + $0.034/千张的定价把 T2I 拉到"和 API 调用一样便宜"的量级。

这两个动作共同指向：**基础模态开始被"按秒/按次"计价工具化**。当 T2I 单价低于云函数调用成本，"是否用 AI"就从预算讨论变成默认调用，只有推理链更长的场景（视频生成、Agent 编排）还留有 API 溢价空间。

**点评：** 前沿模型比拼智能，边缘模态比拼延时和单价——2026 下半年的商业化增量，恐怕主要在"秒级+便宜"这一格里。

---

## 行业观察

**7 月 9 日会成为一个记录日**——三家前沿实验室在同一天可公开访问新一代模型，之前从未出现过。当"下一代模型"变成周期性事件，护城河已经从"模型强度"转移到三个新坐标：**政府红队通行证**（Sol 花 40 天走完流程）、**每 token 边际成本**（Grok 4.5 比 Sol 便宜 5 倍）、**代理能力落地**（Sonnet 5 定位"最具代理性"、Sol 的 ultra 模式）。

**Anthropic 的 18 天风波和欧盟延期通过**共同勾勒出监管的新样式：不是拦下模型，而是把"模型可发布状态"变成一个持续的、企业和政府共同定义的状态机——Fable 5 停机 18 天再上线，是这个状态机的第一次公开演练。

**融资端最值得警觉的是"结构性重心"**：本周 80% 的 AI 融资进了基础设施，Together AI 的 8 亿、Crusoe 的 30 亿、Kling 的 20 亿都是"重资本+高毛利"模式，而应用层的融资只有 Taktile 1.1 亿这样的中盘案例。资本正在拒绝为"套壳应用"付溢价，转而集中赌那些能给 GPT-5.6/Grok 4.5/Sonnet 5 供电或供水的公司——这背后是资本对"未来 12 个月内 AI 应用能否跑通 unit economics"的谨慎观望。
