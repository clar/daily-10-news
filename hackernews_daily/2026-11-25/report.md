# Hacker News 日报｜2026-11-25

数据口径：北京时间约 04:58 读取 [HN 官方首页](https://news.ycombinator.com/news)及[官方热榜 API](https://hacker-news.firebaseio.com/v0/topstories.json)。两处刷新不同步，排名和计数统一采用同一张首页快照。表格为节选，保留原名次。

## 今日焦点

> **浏览器里的 Linux · 智能体利益冲突 · DNS 治理 · AI 编程交付**
>
> - **《2035 提前到来》**：浏览器里的 Linux 从命令行演示做到了图形程序可交互。890分 · 333评。
> - **智能体究竟为谁办事？** 托管平台与用户的目标并不总一致，讨论焦点是透明度和问责。785分 · 335评。
> - **Quad9 撤出法国**：上周还在讨论阻断 DNS 的代价，如今服务方已公布退出安排。275分 · 148评。
> - **Jetty Pro**：AI 能快速生成初版，但开发者原以为一两天的项目做了三个半月。211分 · 83评。

---

## 今日热榜总览

| 排名 | 标题 | 描述 | 分数 | 评论数 |
|---|---|---|---:|---:|
| 1 | [Ternary Bonsai 2.5 27B](https://news.ycombinator.com/item?id=50633922) | AI：让更大模型适合本地运行 | 35 | 0 |
| 3 | [喷雾瓶](https://news.ycombinator.com/item?id=50598555) | 设计：观察日常机构如何工作 | 238 | 68 |
| 4 | [Jetty Pro](https://news.ycombinator.com/item?id=50630462) | 开发：一个 AI 辅助的桌面工具 | 211 | 83 |
| 5 | [装进行李箱的意大利折叠自行车](https://news.ycombinator.com/item?id=50610820) | 工业设计：缩小随车携带体积 | 44 | 25 |
| 6 | [把网页应用变成 AI 智能体可验证的操作](https://news.ycombinator.com/item?id=50632998) | AI：让网页操作结果可检查 | 26 | 4 |
| 7 | [Launch HN：Versine，面向收付款的 MCP（YC F26）](https://news.ycombinator.com/item?id=50634426) | 初创发布：把支付操作接入助手 | 7 | 1 |
| 8 | [2035 提前到来](https://news.ycombinator.com/item?id=50624497) | 系统：在浏览器运行 Linux 图形应用 | 890 | 333 |
| 9 | [Cloudflare 掩盖了底层基础设施的短板](https://news.ycombinator.com/item?id=50632883) | 架构：便利层会不会遮住依赖 | 99 | 69 |
| 10 | [一个 USB-C 口同时分出 USB 3 和 USB 2](https://news.ycombinator.com/item?id=50629106) | 硬件：探索两代 USB 的数据线路 | 93 | 68 |
| 11 | [用闲置算力训练本地模型](https://news.ycombinator.com/item?id=50629231) | AI：把本机空闲资源用于训练 | 116 | 34 |
| 12 | [从 CUDA 和 Jax 到 TorchTPU：凯莱图求解经验](https://news.ycombinator.com/item?id=50633424) | 工程：迁移计算框架的实际代价 | 16 | 0 |
| 13 | [Grafana 为多个版本发布安全更新](https://news.ycombinator.com/item?id=50633159) | 安全：核对部署版本并及时更新 | 68 | 14 |
| 16 | [Show HN：基于列式存储的 Postgres 只读副本 Mason](https://news.ycombinator.com/item?id=50630294) | 项目展示：把分析查询移出主库 | 58 | 6 |
| 17 | [Quad9 在法国停止 DNS 服务](https://news.ycombinator.com/item?id=50625384) | 网络治理：退出服务的实际影响 | 275 | 148 |
| 18 | [大模型智能体究竟为谁工作？](https://news.ycombinator.com/item?id=50627340) | AI：讨论用户与平台的利益冲突 | 785 | 335 |
| 19 | [Show HN：Brickie，在自己的 AWS 账户部署沙箱](https://news.ycombinator.com/item?id=50629936) | 项目展示：运行环境由用户控制 | 12 | 0 |
| 20 | [向性能工程师 Brendan Gregg 取经](https://news.ycombinator.com/item?id=50626413) | 性能：学习怎样问出正确的问题 | 200 | 34 |
| 21 | [你的城市需要多少个无线网状网络节点？](https://news.ycombinator.com/item?id=50609483) | 工具：根据条件估算覆盖所需节点 | 9 | 0 |

---

## 重点讨论点评

### 🥇 [2035 提前到来](https://news.ycombinator.com/item?id=50624497) · 890分 · 333评

**浏览器里的 Linux，开始从“能启动”往“有人愿意试”迈进。**

[开发者 Farid Zakaria](https://fzakaria.com/2026/11/23/2035-came-early)介绍，TryNix 换用把 Linux 内核编译成 WebAssembly 的引擎，仍模拟用户程序，但能在网页里运行图形应用和音频，也能联网。作者在不同负载上报告约 2 到 32 倍提速；嵌套运行 Firefox 的演示仍花了一个多小时，说明提升并不均匀。

它最扎实的用途未必是替代桌面系统，而是降低复现门槛。教程、软件试用或故障复现，可以用链接给人一份环境，不必让读者先在自己的机器上装一遍。

### 🥈 [大模型智能体究竟为谁工作？](https://news.ycombinator.com/item?id=50627340) · 785分 · 335评

**把助手接入支付、邮件和文件之前，该先知道它在哪些地方不能代表你。**

[Michael Harley 的文章](https://michaelharley.net/posts/2026/11/01/llm-agents-work-for-their-parent-companies-not-for-you/)把注意力放在托管平台与用户之间可能存在的利益冲突。不能由此认定每次输出都偏袒厂商；实际要追问的是，谁定默认选项、推荐依据是否可见、哪些数据会传出去、操作能不能撤回。

> *热门评论摘要：* 有读者借鉴专业顾问的保密和利益冲突规则，建议 AI 产品也明确自己在代表谁。这是一项治理主张，不是现有法律义务的陈述。

### 🥉 [Quad9 在法国停止 DNS 服务](https://news.ycombinator.com/item?id=50625384) · 275分 · 148评

**从争论到退出，最先承受切换成本的是普通用户。**

[Quad9 官方说明](https://quad9.net/news/blog/quad9-service-deactivation-in-france/)指出，撤出决定和版权封锁纠纷有关。上周 HN 主要争论解析层是不是合适的执法位置；今天的变化是服务方执行退出，使用该解析器的人可能遇到中断。

其中一个难题和技术本身有关：IP 地址的位置不总等于用户的位置，按地址划分会误判。退出和在境内精确执行一批域名的封锁是两个不同问题，不能把前者做得到当成后者已解决。

### [Jetty Pro](https://news.ycombinator.com/item?id=50630462) · 211分 · 83评

**初版写出来，才暴露出原来没算进去的产品工作。**

[John Siracusa 的复盘](https://hypercritical.co/2026/11/23/jetty-pro)写道，他原以为一两天就能借编程助手做出一个自己用的文件夹面板，三个月半后才写下这篇进度说明。这是一个人的开发经历，不是 AI 编程效率的普遍统计；但它提醒读者，生成代码、决定细节和把工具打磨到长期可用，是不同工作。

## 社区脉搏

昨天热榜聚焦独立浏览器引擎和开发文档的存续，今天延续了同一个问题：谁控制工具和基础设施？TryNix 让软件更易分享，Quad9 的退出暴露了看不见的网络依赖，智能体讨论则把控制权问到了产品默认设置和用户授权上。
