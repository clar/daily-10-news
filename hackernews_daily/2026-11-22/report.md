# Hacker News 日报｜2026-11-22

数据口径：北京时间 05:02 左右读取 [HN 首页](https://news.ycombinator.com/)和[官方热榜 API](https://hacker-news.firebaseio.com/v0/topstories.json)。两处更新不同步，排名、分数、评论数取同一张首页快照；表格节选首页前 20 名中的 19 条，保留原名次。

## 今日焦点

> **黎曼猜想验证 · 本地模型 · 公共软件 · 网络排障**
>
> - **Lean 与 Mathlib 社区确认经典黎曼猜想的形式化证明**：公开了命题比对、可重现构建和独立检查的依据。620分 · 471评。
> - **Inkling 2 Mini 的 5.4 GB 方案**：低内存能否跑得动，与能否胜任你的任务，是两个问题。220分 · 40评。
> - **巴西联邦税务局开源税改计算器**：先公开的是消费税相关实现，不是整套申报系统。595分 · 197评。
> - **显示器接入后网速降了 75%**：同一个网卡直连再复测，才把问题从宽带缩小到本地设备链路。378分 · 194评。

---

## 今日热榜总览

| 排名 | 标题 | 描述 | 分数 | 评论数 |
|---|---|---|---:|---:|
| 1 | [用 5.4 GB 内存运行 Inkling 2 Mini](https://news.ycombinator.com/item?id=50591853) | 技术：更小的内存占用有何代价 | 220 | 40 |
| 2 | [Lean 验证经典黎曼猜想证明](https://news.ycombinator.com/item?id=50589618) | 数学：社区说明四项检查依据 | 620 | 471 |
| 3 | [胰腺癌候选口服药的研究进展](https://news.ycombinator.com/item?id=50582069) | 医学：临床研究不等于获批治疗 | 74 | 17 |
| 5 | [巴西税务局以 MIT 许可开源税改计算器](https://news.ycombinator.com/item?id=50532613) | 公共软件：消费税计算逻辑开放 | 595 | 197 |
| 6 | [用 Go 写 PostgreSQL 扩展](https://news.ycombinator.com/item?id=50591260) | 数据库：用 Go 拓展数据库功能 | 79 | 5 |
| 7 | [我的显示器让下载速度下降 75%](https://news.ycombinator.com/item?id=50587875) | 排障：用直连对照定位链路差异 | 378 | 194 |
| 8 | [Alessandro Masullo 的广义黎曼猜想手稿](https://news.ycombinator.com/item?id=50579568) | 数学：独立人工候选稿仍待核验 | 2345 | 1127 |
| 9 | [热带雨林物种可能比想象中更年轻](https://news.ycombinator.com/item?id=50532417) | 研究：重新估计物种形成时间 | 17 | 8 |
| 10 | [让思维引导身体，再由身体反过来影响自己](https://news.ycombinator.com/item?id=50583028) | 随笔：讨论思维与身体的双向作用 | 13 | 2 |
| 11 | [黎曼猜想 Lean 证明的验证文件](https://news.ycombinator.com/item?id=50590441) | 数学：提供独立复查所需文件 | 56 | 20 |
| 12 | [Show HN：Zero C#，无需运行时或垃圾回收](https://news.ycombinator.com/item?id=50590279) | 项目展示：重新探索 C# 的运行方式 | 86 | 63 |
| 13 | [Thinking Machines Lab 发布 Inkling 2 Mini](https://news.ycombinator.com/item?id=50581260) | AI：官方发布与社区量化是两回事 | 1308 | 270 |
| 14 | [我对自己的艺术网站架构很满意](https://news.ycombinator.com/item?id=50577991) | 技术：复盘个人作品站的技术选择 | 107 | 26 |
| 15 | [GnuPG 远程代码执行漏洞公告](https://news.ycombinator.com/item?id=50587208) | 安全：管理员应关注供应商修复 | 197 | 73 |
| 16 | [Bolt 滑板车变成无障碍地图传感器](https://news.ycombinator.com/item?id=50533517) | 城市：用骑行数据了解道路障碍 | 5 | 3 |
| 17 | [我如何为 Satelital 自制游戏引擎](https://news.ycombinator.com/item?id=50550015) | 游戏：为单一作品定制引擎 | 17 | 2 |
| 18 | [iOS 为什么仍没有非 WebKit 浏览器](https://news.ycombinator.com/item?id=50575644) | 平台政策：纸面开放能否实际落地 | 388 | 224 |
| 19 | [Ask HN：有 15 年经验，在美国失业近两年怎么办？](https://news.ycombinator.com/item?id=50583761) | 社区问答：软件工程师求转岗建议 | 523 | 589 |
| 20 | [确定性模拟测试并不只适合大团队](https://news.ycombinator.com/item?id=50574264) | 工程：让偶发失败可以重复出现 | 57 | 8 |

---

## 重点讨论点评

### 🥇 [Lean 验证经典黎曼猜想证明](https://news.ycombinator.com/item?id=50589618) · 620分 · 471评

**从昨天的候选证明到今天的明确背书，新增的证据是什么？**

[Lean 与 Mathlib 社区联合声明](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/)确认，Alpöge 的工程证明了 Mathlib 中经典黎曼猜想的正式表述。声明列出四项检查：核对命题、复现构建、用独立工具确认所证命题一致，以及用不同实现检查导出的证明。[验证文件](https://math.mit.edu/~drew/grh/)也单独公开。

这一确认的范围是**经典黎曼猜想**，不能直接扩大到所有广义黎曼猜想，也不是对 Masullo 的独立人工手稿背书。可形式验证和能用一篇人可读的论文解释证明思路，也是两个阶段。

> *热门评论摘要：* 读者追问 AI 是否可能碰巧利用证明检查器的缺陷。回应的重点是此次不是只运行了一个检查器，而且还专门比对了该工程真正证明的命题。

### 🥈 [用 5.4 GB 内存运行 Inkling 2 Mini](https://news.ycombinator.com/item?id=50591853) · 220分 · 40评

**把模型装进现有机器，只解决了第一道门槛。**

[社区项目](https://github.com/ShinMegamiBoson/lookatmyquant)与 [Thinking Machines Lab 的官方发布](https://thinkingmachines.ai/news/inkling-2-mini/)不是一回事。前者讨论量化后的低内存方案；标题的 5.4 GB 不宜直接读成所有机器、上下文长度或负载的承诺。

真正有用的对照是同一硬件、同一上下文和任务下的峰值内存、速度和成功率。输出分布更接近原模型，可以作为指标，但不能替代真实任务测试。

> *热门评论摘要：* 有熟悉本地模型的读者指出，项目还列了其他模型的指标，不能把仓库标题的倍数优势套到 Inkling；能跑起来也不能证明实用性。

### 🥉 [巴西税务局开源税改计算器](https://news.ycombinator.com/item?id=50532613) · 595分 · 197评

**税法可以公开阅读，执行税法的代码也可以公开核对。**

[巴西联邦税务局公告](https://www.gov.br/receitafederal/pt-br/assuntos/noticias/2026/novembro/receita-federal-publica-primeiro-codigo-fonte-aberto-no-github-e-amplia-transparencia-da-reforma-tributaria)称，这是该机构首次以 MIT 许可在公共协作环境发布软件，服务于消费税改革。外部开发者能看同一份计算逻辑，更容易发现自己的实现和官方解释到底差在哪。

开放计算器并不等于个人所得税申报系统也已开源。能否真正减少争议，还要看以后税法变化时，公式、版本和测试案例能否同步更新。

> *热门评论摘要：* 高位评论希望更多国家公开公共软件；跟帖则补充，这次涉及消费税和相关业务税计算，不是个人报税工具。区分这两点，才能判断谁会马上受益。

### [我的显示器让下载速度下降 75%](https://news.ycombinator.com/item?id=50587875) · 378分 · 194评

**“换个接法就正常”不是修好，但比反复测公网更接近原因。**

[作者的排障记录](https://blog.tymscar.com/posts/studiodisplayethernet/)里，同一台 Mac 和同一 USB 网卡，直接接电脑时局域网吞吐约 2.3 Gbps，经过显示器时下载约 600 Mbps。换驱动和调整流量控制都会改变结果，说明标题说的显示器只是问题路径的一段。

对读者更可复用的是对照法：保持设备尽量一致，只改一处连接，用本地测速把家庭网络与公网表现拆开。个别组合上的结果不能当作所有同型号显示器都会慢的结论。

## 社区脉搏

今天几条热点都在追问「能不能独立复核」：数学社区公开了对命题和证明的交叉检查，巴西税务局公开了部分计算逻辑，网速帖则用直连和本地测速给出对照。另一个值得注意的信号是，就业求助虽只排第 19，评论却比不少榜首帖子更多，榜单排序不等于社区最想聊什么。
