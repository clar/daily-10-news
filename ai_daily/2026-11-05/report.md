# AI 日报 · 2026-11-05

## 今日焦点

> **AI 安全攻防战升温 · GPT-6 Astra 自主设计硬件 · ChatGPT 冲击谷歌搜索 · 密码学验证模型身份 · 美国中期选举成 AI 广告战场**
>
> - **OpenAI 雇"曾攻入 Anthropic"的 Cathedral 做红队**：前 DOGE 员工创办的安全公司转阵营，AI 实验室之间的攻防赛被公开化。
> - **GPT-6 Astra 一周"自己设计"一款硬件**：从外壳到电路板再到软件，模型几乎接管了一次完整的产品开发。
> - **ChatGPT 周活 12 亿、"搜索类查询"达 Google 20%**：OpenAI 用自己的定义,但规模冲击已经难以忽视。
> - **Anthropic 放出 FlashProve 研究**：用零知识证明验证"这确实是声明的那个模型",给第三方审计提供新原语。
> - **美国中期 AI 政治广告支出 1.87 亿美元**：近 300 条生成/增强广告,州级披露规则混乱,监管真空被实时放大。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | OpenAI 与前 DOGE 员工创办的 Cathedral 结成安全合作、上调漏洞赏金 | The Neuron | ⭐⭐⭐⭐⭐ |
| 2 | 路透：5 名前员工称 ChatGPT 上线前 OpenAI 内部数据访问过宽、安全评审薄弱 | Reuters | ⭐⭐⭐⭐⭐ |
| 3 | 两名 OpenAI 工程师用 GPT-6 Astra 一周内设计出 Codex 配套硬件 | The Neuron | ⭐⭐⭐⭐⭐ |
| 4 | Anthropic 发布 FlashProve：对模型身份做密码学证明的研究与代码 | Anthropic | ⭐⭐⭐⭐ |
| 5 | OpenAI 披露 ChatGPT 每周 12 亿用户,"搜索类查询"约为 Google 的 20% | OpenAI | ⭐⭐⭐⭐ |
| 6 | 美国 2026 中期选举：AI 生成/增强政治广告支出达 1.87 亿美元 | The Neuron | ⭐⭐⭐⭐ |
| 7 | Revolut 将自托管模型设为默认,AI 编码成本下降约 90% | The Neuron | ⭐⭐⭐⭐ |
| 8 | OpenAI 推出 Grid Protectors：乔治亚新园区可提供最多 1,000 MW 弹性负荷 | OpenAI | ⭐⭐⭐⭐ |
| 9 | Google DeepMind 删除新合同中的"离职后不得公开批评"条款 | The Neuron | ⭐⭐⭐ |
| 10 | Google 学校策略：禁用 Google AI 的学区将同时失去 Google Search 账号 | The Neuron | ⭐⭐⭐ |
| 11 | CrowdStrike Falcon Guardian 新增 "AI Kill Switch",可冻结失控代理 | CrowdStrike | ⭐⭐⭐ |
| 12 | Apple 年报新增风险因素：自主代理可能越权执行未授权交易 | Apple 10-K | ⭐⭐⭐ |
| 13 | Drax 公布 200 亿英镑级北约克郡数据中心项目(Brookfield + Radiant) | The Neuron | ⭐⭐⭐ |
| 14 | OpenAI 发布 Pando:Git 兼容后端已接管主代码库,中位 push 延迟降 ~80% | OpenAI | ⭐⭐⭐ |
| 15 | Anthropic Claude Code 负责人 Cat Wu 离职 | The Neuron | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · OpenAI 把"攻过 Anthropic"的 Cathedral 收编,AI 安全战进入贴身肉搏

**[The Neuron · November 4, 2026](https://www.theneuron.ai/digest/everything-that-happened-in-ai-today-wednesday-november-4-2026/)**

OpenAI 今天正式宣布与 Cathedral Systems 结成红队合作,后者是由数名前 DOGE(Department of Government Efficiency)成员创办的安全公司。Cathedral 此前曾声称在一次"漏洞赏金测试"中触及 Anthropic 的部分内部系统 —— Anthropic 否认授权,双方公开吵过一轮。现在同一批人换阵营打 OpenAI 自家的防线,OpenAI 同时上调了漏洞赏金额度。

这单事件的象征意义远大于实际意义。头部 AI 实验室之间的"模型安全 / 权重防护 / 代理越权"等边界,过去主要靠 blog 互相喊话,现在变成白盒对抗:同一批攻手,昨天打友商,今天打自己。前 DOGE 背景也意味着他们熟悉大规模内部访问和权限审计的套路 —— 这正是另一条路透稿捅出来的 OpenAI 痛点:五名前员工表示,ChatGPT 2022 年上线前,OpenAI 内部数据访问范围过宽,安全评审"存在但形同虚设",OpenAI 最近一次"security sprint"动员了约 25% 的产品工程师。

**点评:** AI 实验室的护城河以前谈"模型能力"和"算力",现在要加一条"权重和代理行为能不能守得住";Cathedral 这笔交易是把"攻防赛"外包化、职业化的信号枪。

---

### 🚀 No.2 · GPT-6 Astra "一周设计出一台硬件":AGI 自证的第一块样品

**[The Neuron · November 4, 2026](https://www.theneuron.ai/digest/everything-that-happened-in-ai-today-wednesday-november-4-2026/)**

两位 OpenAI 工程师用 GPT-6 Astra —— 9 月上线、OpenAI 自己描述为"能完成大多数人类智力任务"的系统 —— 在一周之内完成了一台用于交互 Codex 的外设设计:外壳建模、PCB 布线、固件都是模型给的,人类主要做的是"审稿"与下厂打样。实际量产原型做了多轮返工,因为 Astra 漏掉了几项制造工艺约束 —— 比如孔位间距与 SMT 可制造性。

这比任何 benchmark 都更能体现"AGI 声明"的分量和局限:
- **分量**:从方案收敛到能跑的硬件,过去是跨学科团队干几个月的活,现在变成一个工程师 + 一个模型的一周;
- **局限**:Astra 仍然不会"主动"核查 DFM(Design for Manufacturing)规则,也不懂物料采购周期 —— 这些是"工业经验",不是"推理能力"。

值得关注的是 OpenAI 同一天推出的 Pando:它把内部主代码库迁到自研的 Git 兼容后端,中位 push 延迟下降约 80%。看似工程优化,其实是在给"自己写自己"的 AGI 场景铺基础设施 —— 代码规模和提交频率都会爆炸。

**点评:** AGI 争议停留在口号阶段没意义,真正的拐点是"模型能不能跑完一段端到端流水线";Astra 这台硬件是行业第一张能摆上桌的样品。

---

### 📊 No.3 · ChatGPT 周活 12 亿,"搜索类查询"冲到 Google 20%

**[The Neuron · November 4, 2026](https://www.theneuron.ai/digest/everything-that-happened-in-ai-today-wednesday-november-4-2026/)**

OpenAI 披露 ChatGPT 当前每周活跃用户达 12 亿,并给出了一个足够刺激的内部口径:"ChatGPT 的搜索类查询量约等于 Google 搜索量的 20%"。这个数字是 OpenAI 自己定义的"搜索类" —— 不是严格意义上的网页搜索 —— 但仍是行业第一次有人敢对 Google 公开喊出"两位数份额"。

对照 Google 自己的 Gemini 牌面:Gemini 3 系列仍然嵌在 Google Search 的 AI Overviews 和 AI Mode 里跑;Gemini 4 Argon 9 月上线主打 1M 输出 token;Pichai 在 Q2 财报说过 3.5 Pro 还在测试。这意味着 Google 把 Gemini 当 Search 的增强,而 OpenAI 直接把 ChatGPT 当 Search 的替代。两种战略今天出现了第一组可量化的碰撞。

另外两条配合读:Revolut 把自托管模型设为默认后,AI 编码成本降约 90% —— 大企业的"长期帐"开始算到自托管那一边;Mistral 据 WSJ 报新发布"Le Chonk",开源阵营继续卡位。

**点评:** 最危险的不是 OpenAI 的 20% 数字真假,而是 Google 现在必须公开辩护"ChatGPT 没有抢我多少搜索",辩护本身就是承认战场已经变了。

---

### 🔐 No.4 · Anthropic FlashProve:给"这真的是 Claude 吗"一个密码学答案

**[The Neuron · November 4, 2026](https://www.theneuron.ai/digest/everything-that-happened-in-ai-today-wednesday-november-4-2026/)**

Anthropic 今天放出了 FlashProve 的研究论文和参考实现:核心是一套可验证推理(verifiable inference)机制,让一次模型调用的输出可以被第三方在不暴露权重的前提下验证"确实来自声称的那个模型"。目前仍处实验阶段,没有产品化计划。

这件事的产业意义比名字低调得多:
- **审计**:监管机构(比如 EU AI Act 下面的通用模型条款)未来要求"对齐评估"或"关键能力评估"时,需要一个办法证明"被评估的是你声称的那个版本",FlashProve 第一次给出了零知识证明路径;
- **代理经济**:下游代理商 / 应用层经常把"我们用的是 Claude Opus"当背书,实际后端能不能换模型省钱,从来没法验证 —— 如果 FlashProve 能商用,"模型身份"将成为一条新的 SLA 维度;
- **对比**:OpenAI 本周的动作偏重攻防(Cathedral 红队、Pando 基础设施、Grid Protectors 电网),Anthropic 偏重"可验证"和"可解释",路线分野继续加深。

**点评:** 这类"看不见但很重要"的研究很少上头条,但"可验证模型身份"几乎是所有 AI 监管和责任框架未来必备的一块积木。

---

### 🗳️ No.5 · 美国中期选举:1.87 亿美元 AI 政治广告砸进监管真空

**[The Neuron · November 4, 2026](https://www.theneuron.ai/digest/everything-that-happened-in-ai-today-wednesday-november-4-2026/)**

研究人员统计 2026 中期选举周期,超过 1.87 亿美元花在了约 300 条 AI 生成或 AI 增强的政治广告上。各州对"是否必须披露 AI 制作"的规则完全不一致 —— 有的州要求广告底部挂水印,有的州只约束候选人自费广告而不管超级 PAC,有的州干脆没有规则。

同一天另一条配合着读:Google 对学校宣布,如果学区关闭 Google 的教育类 AI 功能,学生账号会同时失去 Google Search 访问权。无论 Google 是不是有意的,这种"打包策略"等于在告诉教育系统 ——"你不选我的 AI,就连基础搜索也别用"。监管语境下,这是一个强势平台绑定的典型。

**监管面的其他信号:**
- Apple 在 10-K 风险因素里专门写入"自主代理可能越权执行未授权交易" —— 这是上市公司首次把"AI 代理行为"作为独立风险披露;
- CrowdStrike Falcon Guardian 推出 "AI Kill Switch",可以即时停掉、禁重启或网络隔离失控代理,把企业防线从"模型安全"推到"代理治理";
- Google DeepMind 在员工压力下删除了"离职后不得公开批评雇主"的合同条款 —— 对比 2024 年 OpenAI 的 NDA 争议,行业的自律姿态在被同行迫着升级。

**点评:** 中期选举的 1.87 亿美元是一次压力测试,它验证了一个结论:美国联邦层面在 2026 年底前不会出台统一的"AI 政治广告披露法",州级规则的碎片化会在 2028 年总统周期被放大一倍以上。

---

## 行业观察

今天的主线是**"攻防"**:

- **安全侧的攻防**:OpenAI 买下 Cathedral 补齐红队、路透稿捅出 ChatGPT 上线前的权限漏洞、CrowdStrike 上线 AI Kill Switch、Apple 把代理失控写进年报。AI 安全从"对齐伦理"下沉到"可操作防御",头部公司开始按 SaaS 安全的节奏跑。
- **规模侧的攻防**:ChatGPT 12 亿周活 + 20% 搜索份额的数字,是 OpenAI 对 Google 的一次面对面出牌;而 Revolut 降本 90% 的企业案例,又在暗示开源/自托管会在下一阶段蚕食闭源 API 的收入曲线。
- **监管侧的攻防**:美国 1.87 亿美元 AI 政治广告+州级规则混乱的空窗、Google 用搜索绑架教育 AI、DeepMind 在合同语言上让步、Anthropic 的 FlashProve 给审计开了一条密码学新口 —— 四条线同时拉开,监管会比过去一年明显加速。

一句话收尾:**AGI 的可信度不再取决于某个 benchmark,而是看"模型能自己交付一台硬件""输出能不能被第三方密码学验证""代理能不能被企业一键关停"这三件事能不能同时做到。** 今天,这三件事在同一个 24 小时里都出现了可见进展。
