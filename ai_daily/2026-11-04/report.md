# AI 每日报告 · 2026-11-04

## 今日焦点

> **Anthropic RSP 自我迭代预警 · OpenAI 阿布扎比四方协议 · 美中选前 AI 应急组 · 400+ 深伪 App 被曝 · 高盛收紧 Claude Code**
>
> - **Anthropic 更新 Responsible Scaling Policy**：在 SEC 披露中警告模型"接近"自加速 AI 研发阈值，拟引入新一层安全审查。
> - **OpenAI 落地阿联酋**：与阿布扎比签四份协议，覆盖政府服务、能源、主权投资，继 Stargate UAE 后再深化。
> - **深伪 App 风暴**：WIRED 调查 400+ 隐藏滥用深伪功能的 App 与网站，部分藏身 App Store，累计下载 35 万次，苹果紧急下架 19 款。
> - **Goldman Sachs 限制 Claude Code**：仅限工程师使用，理由为"生产力与风险权衡"，首家在前台金融场景收紧代理式编码。
> - **Meituan LongCat-2.5 发布**：1.6 万亿总参数 / 单 token 激活 480 亿的多模态 MoE，中国开源梯队再上一级。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Anthropic 在 SEC 文件警告正接近"AI 自加速研发"阈值，拟修订 RSP | TechCrunch | ⭐⭐⭐⭐⭐ |
| 2 | OpenAI 与阿布扎比签四项协议，覆盖政府/能源/主权投资 | Semafor | ⭐⭐⭐⭐⭐ |
| 3 | WIRED 曝光 400+ 深伪 App，下载 35 万次；苹果下架 19 款 | WIRED | ⭐⭐⭐⭐⭐ |
| 4 | OpenAI 下调融资目标至约 200 亿美元，估值 1.25 万亿，已到账 110 亿 | TechCrunch / WSJ | ⭐⭐⭐⭐ |
| 5 | Goldman Sachs 收紧 Claude Code 使用权限，仅限工程师 | The Decoder | ⭐⭐⭐⭐ |
| 6 | Meituan 发布 LongCat-2.5：1.6T 总参、48B 激活的多模态 MoE | TechNode | ⭐⭐⭐⭐ |
| 7 | OpenAI 与 Anthropic 为美国中期选举组建选举响应团队 | Semafor | ⭐⭐⭐⭐ |
| 8 | OpenAI 发布 LifeVal 基准：3,995 人调研，测日常生活任务能力 | OpenAI | ⭐⭐⭐ |
| 9 | 纽约时报等出版商起诉 Brave，指其绕过付费墙抓取 | The Verge | ⭐⭐⭐ |
| 10 | MIT 权重空间编辑：改写 0.016% 权重把 Qwen MATH-500 从 7.9% 拉到 48.1% | 作者博客 | ⭐⭐⭐ |
| 11 | OpenAI "Grid Protectors" 项目，乔治亚数据中心可应急释放 1 GW 电力 | The Verge | ⭐⭐⭐ |
| 12 | 新发现 Claude 驱动 Windows infostealer，按"价值"排序受害者 | Tom's Hardware | ⭐⭐⭐ |
| 13 | ElevenLabs 研究：2 分钟以上会话中，语音 Agent 比文本 Chat 成功率高 31.7% | ElevenLabs | ⭐⭐⭐ |
| 14 | 中国金融监管警告 AI 投资过度集中（央行副行长肖远企） | Reuters | ⭐⭐⭐ |
| 15 | Palantir CEO Karp：日本应用 AI 建"领土防御"能力 | Commonwealth Magazine | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Anthropic 自曝模型正逼近"AI 自加速研发"阈值

**[TechCrunch](https://www.theneuron.ai/digest/everything-that-happened-in-ai-today-tuesday-november-3-2026/)**

Anthropic 在最新一轮监管披露中罕见地主动承认：公司内部用来触发"AI 显著加速 AI 研究"安全条款的阈值，可能"很快"被跨过。文件同时指出目前没有任何已发布模型越过红线，但 Responsible Scaling Policy (RSP) 需要为此增加一层新的部署与评估流程。

这是继 2025 年 RSP 2.0 之后，Anthropic 首次在 S-1 这种对股东有约束力的公开文件里强调自我迭代风险。放在它正走向 IPO、同时与 Google 签下 5 GW 和与 AWS 签下 1000 亿美元级合约的时间节点，这个披露不是姿态，而是对投资者和监管同时发出的信号——"更强的模型要来了，并且不只是更快，还更像一个自我改进的闭环"。

值得追踪：新版 RSP 的具体门槛（evaluations、第三方红队、红线能力清单）、是否会与英国 AISI / 美国 AISI 的预部署评估挂钩，以及 Claude Opus 下一代是否会被挡在该门槛之后再上市。

**点评：** 当"最谨慎的 Lab"都把自加速风险写进招股书，别的 Lab 早晚要跟进——这不是营销，是行业的监管锚点被 Anthropic 自己向下压了一寸。

---

### 🚀 No.2 · OpenAI 落地阿布扎比：从 Stargate 到主权一体化

**[Semafor](https://www.theneuron.ai/digest/everything-that-happened-in-ai-today-tuesday-november-3-2026/)**

OpenAI 一次性与阿联酋签下四份协议，覆盖政府数字化服务、能源供应、主权财富投资与模型部署。这是继 2024 年 Stargate UAE 算力项目、2025 年与 G42 的深度合作之后，OpenAI 在海湾最彻底的一次"国家级嵌入"。

和竞品比较，这是 OpenAI 第一次把"主权 AI"做成 Full Stack——不只是卖 token，而是把数据中心、能源基建、政务入口、投资回流管道都打包进一张协议网。配合 OpenAI 正在下调的 200 亿美元融资目标（估值仍锁在 1.25 万亿美元），能看出 Altman 的融资逻辑：不再单靠硅谷和大科技公司，而是抓住主权基金这条新的"永久资本"来源。

看点：这份协议会不会被 BIS 出口管制触发审查？以及 Google、Anthropic 的海湾对冲策略会多久跟进。

**点评：** 2026 年最强的"AI 基础设施货币"正在从 H100 换成"主权关系"，谁先把一个国家的能源、数据和政务绑进自己的平台，谁就赢了下一轮。

---

### 🧨 No.3 · 400+ 深伪 App 被曝光：平台治理再度崩盘

**[WIRED](https://www.theneuron.ai/digest/everything-that-happened-in-ai-today-tuesday-november-3-2026/)**

WIRED 调查发现超 400 款 App 与网站内嵌隐藏的滥用型深伪功能，有的伪装成"宠物肖像生成器"等常见工具，累计下载达 35 万次，其中多款上架 Apple 与 Google 商店。被点名后，苹果首批下架 19 款。

这件事的意义不是"又有垃圾 App"，而是在于三个失败点同时发生：（1）平台审核在大规模生成式模型上线后仍沿用静态关键词和 API 文档审核；（2）App 内置模型可本地规避内容审核；（3）这是选前 48 小时被公开的，恰好暴露任何对 2026 美国大选 AI 虚假信息的"入口治理"都极度脆弱。

**点评：** 比 Deepfake 本身更危险的，是我们在 2026 年还在用 2018 年的 App 审核流程去挡它——这件事注定会写进下一版欧盟 AI Act 实施指南的案例库。

---

### 💼 No.4 · 高盛内部收紧 Claude Code：第一家把"代理式编码"降级的大行

**[The Decoder](https://www.theneuron.ai/digest/everything-that-happened-in-ai-today-tuesday-november-3-2026/)**

Goldman Sachs 已将 Claude Code 等代理式编码工具的使用范围限制回"仅工程师"，并撤销对一般业务人员的开放权限，官方口径为"生产力收益与运营风险重新平衡"。

这是今年第一家公开"收紧"而非"扩展"代理式编码权限的头部投行。背景是 AI 编码工具在 2025–26 年从"辅助补全"演进为"自动提交 PR 和运行命令"的代理，而金融机构的审计 / SOX / MNPI 要求本质上和"模型自己调用 shell"不兼容。

值得注意：这与 Anthropic 本周另一起消息呼应——Claude Code 在部分合法逆向工程任务上"过度拒绝"，开发者抱怨 Opus 5.5 加了克隆特定游戏的硬限制。换句话说，Anthropic 一端在收紧模型行为，企业另一端在收紧使用权限，两边都在给代理式编码降温。

**点评：** 2024–25 "全员 Copilot" 的叙事开始出现裂缝，监管敏感行业的"再部门化"是 2027 年值得盯的趋势。

---

### 🚀 No.5 · Meituan LongCat-2.5：中国开源 MoE 继续追到前沿

**[TechNode](https://www.theneuron.ai/digest/everything-that-happened-in-ai-today-tuesday-november-3-2026/)**

美团发布 LongCat-2.5 多模态大模型：总参数 1.6 万亿，每 token 激活约 480 亿，采用稀疏 MoE + 视觉 / 音频联合训练。这是美团继 LongCat 1.x 之后第一个把总参数拉到万亿级的开源模型，也标志着继 DeepSeek、Qwen、Kimi、Zhipu 之后，又一家互联网大厂将基础模型投入"开放参数"赛道。

从架构看，它直接对标 Google Gemini 4 Carbon 与 OpenAI GPT-6.1 Terra 的"便宜 + 快"路线：参数巨大但 active 很稀，部署成本接近 70B dense。配合中国仍在扩张的 10,000 GPU 级国家采购（印度亦跟进），中国 MoE 开源阵营正在抢占"成本/质量"的中段市场。

**点评：** 2026 年真正值得关注的，不是"谁家 SOTA"，而是"开源万亿级 MoE 还要多久把 OpenAI 的推理成本护城河填平"——LongCat-2.5 把这个倒计时又拨快了一格。

---

## 行业观察

今天的消息线把 2026 年 Q4 的 AI 版图切成三块。

**第一块是"安全与监管的回摆"。** Anthropic 把自加速风险写进 S-1，Claude Code 在金融前台被降级，400 款深伪 App 在选前被扒出来，这三件事发生在同一天——不是巧合，是行业从"能力竞赛"向"合规竞赛"换挡的信号。EU AI Act 12 月 2 日的关键节点、美国中期选举、中国央行对 AI 过度投资的警告几乎同频发出。

**第二块是"主权算力"的加速。** OpenAI 的阿布扎比四协议、Anthropic 的 Google 5GW + AWS 1000 亿、印度 10,000 GPU 采购计划，都指向同一个逻辑：算力正在从"企业资产"变成"国家基建"，谁先完成主权绑定，谁先锁定下一代推理基座。

**第三块是"开源 MoE 继续压价"。** LongCat-2.5 的出现意味着中国厂商在稀疏万亿级架构上追平时间窗继续缩短，Google Gemini 4 Carbon 与 OpenAI GPT-6.1 Terra 刚打出的"更便宜更快"的护城河，很快会被中国开源梯队重新定价。接下来值得观察的，是谁会在 Q4 结束前先开放"跨模态 + 超长上下文 + 稀疏推理"的三合一开源 checkpoint——那将是 2027 年成本战的起点。

**数据与来源**：以上信息综合自 [The Neuron 11/3 综述](https://www.theneuron.ai/digest/everything-that-happened-in-ai-today-tuesday-november-3-2026/)、[LLM Stats 新闻](https://llm-stats.com/ai-news)、[AI Startup Funding News 11/2026](https://blog.mean.ceo/ai-startup-funding-news-november-2026/)、[Cubbbix AI Regulation Nov 2026](https://cubbbix.com/blog/ai-regulation-november-2026-global-update) 及 Tom's Hardware、TechCrunch、WIRED 等转述报道。部分数字来自二级来源，已在正文中标注。
