# Hacker News 日报 · 2026-10-26

## 今日焦点

> **更野心的软件 · AI 不是万能 · 开发者反抗审查 · 政府信息透明代价 · AI 代理走向 GUI**
>
> - **"We should be more ambitious with the software we build"** 730 分 · 671 评 — Dan Luu 的檄文把 HN 情绪推到年度峰值
> - **Root shell on Samsung TV** 732 分 · 557 评 — 一条推文揭示的内网级漏洞，连带硬件安全焦虑
> - **A 10-year-old CNN outperforms frontier LLMs for skin cancer diagnosis** 343 分 · 177 评 — 对 LLM 泛用性的最辛辣提醒
> - **Oregon Police charging $2.5M for records about one cop** 309 分 · 78 评 — 公共信息被标价的典型案例
> - **AI use leads UC Berkeley math professor to see 'no point' in grading homework** 172 分 · 252 评 — AI 冲击教育的真实现场

---

## 今日热榜总览

| 排名 | 标题 | 描述 | 分数 | 评论数 |
|------|------|------|------|--------|
| 1 | [Root shell on Samsung TV](https://news.ycombinator.com/item?id=50218633) | 智能电视漏洞再上头条 | 732 | 557 |
| 2 | [We should be more ambitious with the software we build](https://news.ycombinator.com/item?id=50225695) | Dan Luu 檄文引爆讨论 | 730 | 671 |
| 3 | [Cerebras Deploys Trillion-Parameter AI Models](https://news.ycombinator.com/item?id=50227356) | 挑战 Nvidia 推理霸权 | 344 | 127 |
| 4 | [A 10-year-old CNN outperforms frontier LLMs for skin cancer diagnosis](https://news.ycombinator.com/item?id=50233779) | 老 CNN 碾压大模型 | 343 | 177 |
| 5 | [I refuse to accept a censored Internet. Join Me at FOSDEM 27](https://news.ycombinator.com/item?id=50233929) | 开源社区抵制审查 | 326 | 168 |
| 6 | [Oregon Police charging $2.5M for records about one cop](https://news.ycombinator.com/item?id=50234232) | 公共信息被标天价 | 309 | 78 |
| 7 | [Dolly Parton's Imagination Library](https://news.ycombinator.com/item?id=50234474) | 2 亿本童书的慈善项目 | 274 | 49 |
| 8 | [AI use leads UC Berkeley math professor to see 'no point' in grading homework](https://news.ycombinator.com/item?id=50233304) | 高校评分制崩塌中 | 172 | 252 |
| 9 | [JetBrains Thinkrail](https://news.ycombinator.com/item?id=50233294) | AI 代理 GUI 新战场 | 141 | 100 |
| 10 | [Serbia's Vucic concedes election defeat](https://news.ycombinator.com/item?id=50236081) | 学生运动改写历史 | 101 | 39 |
| 11 | [Active incident at Dreamhost forcing password reset](https://news.ycombinator.com/item?id=50231166) | 老牌主机商被迫重置 | 94 | 35 |
| 12 | [Why I Am a Programmer](https://news.ycombinator.com/item?id=50235017) | 老程序员的自白 | 78 | 14 |
| 13 | [Overgrown, when plants invade your abandoned tabs](https://news.ycombinator.com/item?id=50197108) | 浏览器扩展小趣味 | 53 | 13 |
| 14 | [Eunice is almost here](https://news.ycombinator.com/item?id=50235316) | 开发者个人项目预告 | 49 | 42 |
| 15 | [The U.S. Power Grid](https://news.ycombinator.com/item?id=50196623) | 美国电网科普长文 | 48 | 17 |
| 16 | [VCF Southwest 2026, edited on SGI for '90s TV](https://news.ycombinator.com/item?id=50223435) | 复古计算情怀 | 48 | 11 |
| 17 | [What goes into making an animated film?](https://news.ycombinator.com/item?id=50235738) | 迪士尼制片流程揭秘 | 46 | 17 |
| 18 | [Gheist: scaled abuse of stolen GitHub tokens](https://news.ycombinator.com/item?id=50235010) | GitHub 供应链攻击 | 39 | 0 |
| 19 | [Recreate the Apollo Guidance Computer](https://news.ycombinator.com/item?id=50195769) | 复刻登月计算机 | 34 | 2 |
| 20 | [Show HN: Hurston-1 open source TTS (Southern/Afro-English)](https://news.ycombinator.com/item?id=50227330) | 口音多样性新 TTS | 32 | 10 |

---

## 重点讨论点评

### 🥇 [We should be more ambitious with the software we build](https://news.ycombinator.com/item?id=50225695) — 730 分 · 671 评

**Dan Luu 把 HN 的集体焦虑一次点穿**

Dan Luu 的新文章用一贯的"数据+段子"风格，批评当代软件工程普遍"过度满足于一张能跑的 React 界面"。他列举了金融后台、企业 CRM、OS 调度器等地方多年未变的痛点，并追问："这些问题 20 年前就有，为什么没人去啃？"文章用大量基准数据证明：工程师并没有变懒，而是我们的组织结构、投融资方式和激励体系把人才引向了"低风险、易变现"的产品。

HN 评论区几乎是年度最热烈：671 条评论里一半在共鸣，一半在反击。拥护者说"是的，CRUD 不是你的终点"；反对者则指出大部分软件工作本来就是"修管道的管道工"，野心需要客户买单，而客户只愿意为"节省 5% 成本"付钱。还有一派在讨论 Dan Luu 自己提到的"工程文化腐坏"是否可以通过小团队高自主来解决。

> *热门评论摘要：* 最高赞评论调侃"我上一次写出有野心的代码是在那年新冠封控时，公司不敢开会；一开会，野心就死了。"反方最高赞则反问："请先告诉投资人为什么要给我们 3 年时间做一个'可能根本没人买'的东西。"

---

### 🥈 [Root shell on Samsung TV](https://news.ycombinator.com/item?id=50218633) — 732 分 · 557 评

**一条推文暴露的消费电子"糖衣炸弹"**

@log4j（研究员推特账号）用一张截图展示了在 Samsung 智能电视上拿到 root shell 的全过程，起点是一个未签名的 debug menu 入口。这件事技术上没有新花样——过去三年我们见过小米、海信、LG 多次类似漏洞——但它触发了 HN 一贯的"消费电子即监视设备"焦虑。

讨论焦点有三：**（a）** 智能电视在 LAN 内的攻击面远超用户想象，很多设备自带 ADB over Wi-Fi 和未加密 MQTT；**（b）** 固件更新机制几乎没有强制，老机型漏洞永存；**（c）** 相比之下 Apple TV 的封闭策略被重新评价为"不是作恶，是不作恶最低限度"。还有大量用户表示自己把电视断网只接 HDMI 棒，这几乎成了 HN 中产标配。

> *热门评论摘要：* "每一台 smart TV 都应被当成一个未打补丁的 2015 年 Android 平板来对待——因为它就是。"

---

### 🥉 [A 10-year-old CNN outperforms frontier LLMs for skin cancer diagnosis](https://news.ycombinator.com/item?id=50233779) — 343 分 · 177 评

**对 LLM "万能主义"的一次冷水浇头**

Lynch Lab 的一项评测在医学分类任务上对比 2015 年的 ResNet 变体与 2026 年主流前沿 LLM（视觉模型）：老 CNN 在皮肤癌样本上准确率超越最新多模态 LLM 约 7–12 个百分点，且推理速度快一个数量级。文章得出的结论不是"LLM 没用"，而是"把分类任务塞进通用模型是一种资源浪费"。

HN 的反应极其分裂。老派 ML 工程师在欢庆"终于有人证实了我们的直觉"；LLM 阵营则辩解"评测数据集太小、泛化比准确率更重要"；还有一派指出真正值得警惕的是医疗 AI 产品正在用 LLM 招牌向监管机构骗取通过。评论区关于"分类 vs 推理 vs 生成"的分工讨论特别精彩，一度回到 2015 年"深度学习 vs 概率图模型"的味道。

> *热门评论摘要：* "LLM 把所有问题都变成了下一个 token 预测，但医生看皮肤图不是预测下一个像素。"

---

### 🏛️ [Oregon Police Are Charging a Local News Outlet $2.5M for Records About One Cop](https://news.ycombinator.com/item?id=50234232) — 309 分 · 78 评

**公开信息被"合法"地标价成壁垒**

Intercept 的调查揭示：Oregon 当地警署应 FOIA 请求提供一名警官的档案时，报价 250 万美元，宣称是"复印、审查与冗余查询"成本。这笔金额对任何本地媒体都是天文数字，等同于拒绝。HN 的愤怒来自两处——第一是数字离谱，第二是"合法化"的手法：地方立法允许警署基于"复杂度"自定价。

讨论中出现了一个有意思的技术向思路：有律师背景的用户建议把 FOIA 流程做成一个标准化 open-source pipeline，用 LLM 预览去冗余，然后把法律挑战程式化。另一派则泼冷水："这是政治问题，不是工程问题。"该讨论侧面反映 HN 用户对"用技术解政治病"的疲惫情绪在上升。

> *热门评论摘要：* "250 万不是价格，是一个暗语：'滚开'。"

---

### 🎓 [AI use leads UC Berkeley math professor to see 'no point' in grading homework](https://news.ycombinator.com/item?id=50233304) — 172 分 · 252 评

**AI 把家庭作业变成了测谎仪，教授先投降了**

Berkeley 一位数学教授公开宣布放弃给作业打分，理由是无法区分 LLM 完成与学生自己完成。文章一出，HN 评论区爆出 252 条互喷：有家长说"是的，我儿子的 AP 班作业全让 Claude 做了"；有助教说"我们现在只盯课堂测验"；还有一派坚持"大学从来不是靠作业保证能力的"。

讨论里最值得记录的是教育侧的实用建议：**（a）** 现场考试权重重新上升至 70% 以上，**（b）** 口头答辩回归，**（c）** 作业只给"参与分"而非"正确分"。这些做法反而回归 1980 年代欧洲高教惯例。有人也指出，若所有大学把评价放回现场考试，等于反向证明"工作场景中 AI 可用"的合法性——因为学生"做作业用 AI"与成人"做工作用 AI"本就是同一行为。

> *热门评论摘要：* "大学现在面临的真问题不是作弊，而是我们教的东西 90% 并不需要人类再做了。"

---

## 社区脉搏

今天的 HN 是"技术乐观主义"与"文化悲观主义"的罕见双顶：
- **技术线**：Dan Luu 的"我们该更野心"冲到年度前列；Cerebras 把万亿参数部署到自家堆栈的工程细节获得第一梯队关注；JetBrains Thinkrail 预示着 AI 代理从 CLI 迈向 GUI 的下一场战役；Show HN 的 Hurston-1 TTS 则展示开源仍在扩展少数族裔口音维度。
- **文化线**：Oregon 警署 2.5M 账单、Samsung 电视 root shell、FOSDEM 27 反审查倡议——都在反复敲打同一个主题：**权力正在把公共性和消费电子都变成不透明黑箱**，而社区对此的抵抗变得越来越像"自救"而非"倡议"。
- **AI 的两面性**：同一天 LLM 既"被老 CNN 教做人"（医学分类），又"把大学作业评分制逼到墙角"。HN 的集体直觉是：LLM 泛用性被过度营销，但其对社会的冲击已经不可逆。
- **情绪关键词**：野心 / 怀旧（Apollo 复刻、SGI 剪辑）/ 疲惫（技术解政治）/ 警惕（供应链攻击、Dreamhost 事故、Gheist）。
