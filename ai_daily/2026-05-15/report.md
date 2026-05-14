# AI 日报 · 2026-05-15

## 今日焦点

> **Android 重做为"智能体 OS" · DeepSeek 估值飙至 450 亿 · 美国政府接管模型预审 · EU AI Act 进入高风险倒计时 · Anthropic Mythos 拿下白宫**
>
> - **Google 将 Gemini Intelligence 嵌入 Android 中枢** 安卓被重构为 agent 操作系统，正面拦截 Apple 的 AI 重启
> - **DeepSeek 首轮融资估值或冲 450 亿美元** 数周内估值从 200 亿翻倍，中国大模型估值天花板被重画
> - **Trump 政府要求 Google/Microsoft/xAI 上线前送审** Center for AI Standards 与三巨头签下预审协议
> - **Anthropic Claude Mythos 进白宫做网络安全** Project Glasswing 首批闭门交付，Amodei 与高层会晤
> - **EU AI Act 高风险条款 8/2 全面生效** 雇佣、信贷、教育、执法领域 90 天倒计时

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Google 把 Gemini Intelligence 装进 Android 中枢，拦截 Apple AI 重启 | CNBC | ⭐⭐⭐⭐⭐ |
| 2 | DeepSeek 首轮融资估值或冲 450 亿美元 | TechCrunch | ⭐⭐⭐⭐⭐ |
| 3 | 美国政府与 Google/Microsoft/xAI 签署模型预审协议 | CNN | ⭐⭐⭐⭐⭐ |
| 4 | Anthropic Claude Mythos Preview 进白宫，启动 Project Glasswing | The Information | ⭐⭐⭐⭐⭐ |
| 5 | EU AI Act 高风险条款 8 月 2 日全面生效，企业进入冲刺期 | EU AI Act Tracker | ⭐⭐⭐⭐ |
| 6 | Bret Taylor 的 Sierra 再融近 10 亿，估值跃至 150 亿美元 | CNBC | ⭐⭐⭐⭐ |
| 7 | AI 创业公司占据美国 VC 市场近半壁江山 | BusinessToday | ⭐⭐⭐⭐ |
| 8 | Oracle 拟筹资 500 亿美元加码 AI 数据中心 | Reuters | ⭐⭐⭐⭐ |
| 9 | Google 警告：黑客用 AI 武器化零日漏洞，相关行动已被阻断 | Fortune | ⭐⭐⭐⭐ |
| 10 | Anthropic 上线 Claude Code Routines、Advisor 工具与 20+ 法律 MCP 连接器 | Anthropic Releases | ⭐⭐⭐ |
| 11 | OpenAI 探索"AI-first 设备"，传闻砍掉传统 App 形态 | The Information | ⭐⭐⭐ |
| 12 | Parallel 完成 2.3 亿美元融资，构建 AI 搜索基础设施，估值 20 亿 | TechCrunch | ⭐⭐⭐ |
| 13 | Anduril 以 610 亿估值融资 50 亿，国防 AI 估值再翻倍 | Bloomberg | ⭐⭐⭐ |
| 14 | NVIDIA Vera Rubin 平台进入量产，下半年 OpenAI 首批 1GW 部署 | NVIDIA Newsroom | ⭐⭐⭐ |
| 15 | Air Street Press 发布 5 月 State of AI 月报：模型路由成主战场 | Air Street | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Google 把 Gemini Intelligence 嵌入 Android 中枢，安卓"从 OS 进化为 Intelligence System"

**[CNBC](https://www.cnbc.com/2026/05/12/google-races-put-gemini-at-center-of-android-before-apples-ai-reboot.html)**

Google 本周公开的方向是把 Gemini Intelligence 直接放进 Android 的核心——不再是一个"长在系统里的助手"，而是接管跨 App 调度、屏幕理解、任务执行的核心层。官方演示场景包括：从 Gmail 抽事件，跨多个购物 App 凑齐购物车，看着客人名单自动生成菜单并下单。

这是对 Apple 即将于 WWDC 重启 Apple Intelligence 的提前压制。Google 的赌注是：当 LLM 不再是单点功能而是 OS 级中间件时，**谁的端侧 + 云端协同栈最完整，谁就锁定终端入口**。安卓的开放性让它可以激进地把 Gemini 钉死在系统层 API、Notification、Intent Bus、屏幕识别上，这是 iOS 在隐私沙盒下短期内无法对齐的。

值得关注的下一步：1) Android 16 的 GA 时间表是否会被这次"intelligence layer"重新切片；2) 第三方 App 怎样"被 Gemini 调度"以及由此产生的开发者 SDK 与分账模式；3) 端侧推理是否切换到 Tensor + Gemma 4 Nano 组合。

**点评：** 这是过去三年里安卓改动最大的一次内核调整——Android 不再是 App 的舞台，而是 agent 的执行环境，搜索流量的二次替代正式开始。

---

### 🚀 No.2 · DeepSeek 首轮融资估值或冲 450 亿美元，中国大模型估值天花板被重画

**[TechCrunch](https://techcrunch.com/2026/05/06/deepseek-could-hit-45b-valuation-from-its-first-investment-round/)**

DeepSeek 正在与多家全球投资人洽谈历史性的"首轮"融资，估值从几周前的 200 亿美元一路抬到 450 亿美元，并且仍未关账。"首轮"二字尤其值得玩味——DeepSeek 此前完全靠幻方资本自有现金跑出全球前三梯队的模型，现在愿意接外部资本，意味着它准备进入数据中心扩张和海外发行的下一阶段。

这背后是两件事在同步发生：一是中国大模型在编码 / 数学 / 推理基准上对 GPT-5.5 形成连续追赶（5 月初已有报道指出 DeepSeek V4 Pro 在代码任务上超过 GPT-5.4），二是美元基金对"中国能跑出独立 AI 供应链"的判断重估。450 亿美元的估值如果真的成型，DeepSeek 将一举成为非美系最贵的 AI 公司。

**点评：** 这一轮不是简单的融资，而是中国 AI 在国际资本视野中第一次拿到"主权级独立基础设施"溢价；接下来要看 Anthropic、xAI 等是否被迫上调下一轮估值。

---

### 🚀 No.3 · 美国政府与 Google/Microsoft/xAI 签下"模型上线前送审"协议

**[CNN Business](https://www.cnn.com/2026/05/05/tech/microsoft-google-xai-government-test-ai-models)** · **[CNBC](https://www.cnbc.com/2026/05/05/ai-oversight-trump-google-microsoft-xai.html)**

新设立的 Center for AI Standards and Innovation（CAISI，前身是 NIST 旗下的 AI Safety Institute）宣布与三家头部模型公司签订协议，**所有前沿模型在公开发布前必须先交政府评估**。同时 Anthropic 此前已与 Pentagon 错过一轮交易（5 月 1 日新闻），合作清单调整为 8 家 Big Tech。

注意 Trump 政府这次的逻辑与拜登时期的 EO 14110 截然不同——它把 AI 看作国家战略资产，所以预审是"国家安全协查"，而不是"安全 / 伦理评估"。这就解释了为什么 xAI 也愿意签：评测内容偏军事 / 网络安全 / 双重用途 / 跨境合规，而非偏见、版权等政治议题。这种监管口径转换会让欧盟的 AI Act 看上去越来越像另一条平行宇宙的法律。

**点评：** 真正的 AI 治理战场已经从"是否要监管"切换到"谁握有 pre-launch 评估权"——美国版的"软强制"开始成型。

---

### 🚀 No.4 · Anthropic 把 Claude Mythos 送进白宫，Project Glasswing 锁定网络安全细分赛道

**[The Information](https://www.theinformation.com/)** · **[YouTube Recap](https://www.youtube.com/watch?v=oMRCR6KqZac)**

Anthropic 在本周公开了 Claude Mythos Preview，专门强化在大型代码库中识别漏洞与安全缺陷的能力，并以 Project Glasswing 计划面向少数关键基础设施合作伙伴定向交付。Dario Amodei 本周也现身白宫，与 Trump 政府高层就 Mythos 与国家网络安全直接对话——这一动作很大程度上是在修复 Anthropic 在 5 月初被 Pentagon "冷处理"的关系。

Mythos 与早些时候 OpenAI GPT-5.5 在 32 步端到端攻防演练上的较量，意味着 Anthropic 正放弃"通用 AGI 一条路打到底"的叙事，转向**用 Claude 系列做垂直纵深**：法律（20+ MCP 连接器、12 个 practice-area 插件）、网络安全（Mythos）、Coding（Routines / Advisor）。这一打法可能比通用模型竞速更适合当下监管和企业现金流。

**点评：** Anthropic 押注"特化模型 + 强 alignment + 政府关系"的三角护城河，是头部公司里第一个明确放弃单一通用旗舰策略的玩家。

---

### 🚀 No.5 · EU AI Act 高风险条款进入 8/2 倒计时，欧洲企业进入冲刺合规期

**[EU AI Act Tracker](https://artificialintelligenceact.eu/)** · **[Secure Privacy](https://secureprivacy.ai/blog/eu-ai-act-2026-compliance)**

距离 2026-08-02 仅 79 天，EU AI Act 第三阶段的高风险 AI 条款将正式可执行——覆盖雇佣、信贷、教育、执法、关键基础设施等领域。从 IAPP / OneTrust 的报道可以看出，欧洲 GC 与合规岗已经从"读法条"切换到"配资源"：风险分类、技术文档、人类监督机制、训练数据治理、上市后监测全部要写进 ISMS。

更重要的是它和 CAISI 的预审在底层逻辑上**互斥**：欧盟侧关心的是基本权利和透明度，美国侧关心的是国家安全和威胁建模。对跨国大厂而言，未来几个月会被迫做"双轨产品"——技术报告、阻断措施、披露文档都要两份，且互不替代。

**点评：** 8 月 2 日之后，"是否合规"不再是 PR 问题，而是能否在欧洲销售、能否签政府订单的硬门槛；中后台合规支出会成为今年 AI 公司财报里的新科目。

---

## 行业观察

今天的主线非常清晰：**AI 已经走完"模型即产品"阶段，进入"模型即基础设施"阶段**。三件事互相印证——Google 把 Gemini 钉进 Android 系统层，OpenAI 与 NVIDIA 锁定 10GW Vera Rubin 部署，Oracle 拟为 AI 数据中心举债 500 亿；前端入口、芯片栈、电力 / 房地产同时被重置，没有人再讨论"参数规模"，只讨论"分发面、推理成本、合规许可"。

第二条暗线是**国家化**：CAISI 把模型预审权抓在手里，Anthropic 进白宫，Pentagon 与 8 家 Big Tech 签订协议，DeepSeek 用 450 亿美元估值表明非美 AI 自成体系。AI 公司的董事会议程里，"政府关系"已经升级为与"算力供应链"同等级别的战略议题。

第三条值得跟踪的方向是**模型生态分化**：Anthropic 走垂直特化，DeepSeek 走主权级独立栈，Google 走端侧深度集成，OpenAI 探索"AI-first 设备"——四种路线第一次清晰可见。下一季度的财报与 Code interpreter / Agent 路由（如本周 Air Street 报告提及的多模型路由）市场份额将给出第一个答案。
