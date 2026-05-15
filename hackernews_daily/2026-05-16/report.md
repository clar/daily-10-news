# Hacker News 每日热榜 · 2026-05-16

## 今日焦点

> **公共基础设施情怀 · 隐私 vs 政府执法 · 移动端 0-click 漏洞 · AI 增长曲线辩论 · 形式化语言上太空**
>
> - **Project Gutenberg 持续焕新** 484 分 / 138 评，HN 社区集体为"互联网最好的角落之一"鼓掌，但项目正被 LLM 爬虫流量压得喘不过气
> - **DOJ 要求 Apple/Google 上交 10 万车迷 App 用户身份** 237 分 / 131 评，被类比为"要求 Home Depot 上交所有买过撬棍的人名单"，宪法第四修正案讨论再起
> - **Project Zero 揭示 Pixel 10 零点击漏洞链** 265 分 / 112 评，VPU 驱动一个 mmap 处理函数即可拿到 root，安卓内核安全模型再受考验
> - **Wikipedia 套上 Windows XP 桌面壳** 439 分 / 104 评，意外引爆"层级 vs 搜索"的信息架构怀旧讨论
> - **OCaml 写的 CCSDS 协议栈上轨道运行** 209 分 / 49 评，纯函数式语言完成首次在轨后量子密钥轮换演示

---

## 今日热榜总览

| 排名 | 标题 | 描述 | 分数 | 评论数 |
|------|------|------|------|--------|
| 1 | [Project Gutenberg – keeps getting better](https://news.ycombinator.com/item?id=48150431) | 古腾堡焕新但被爬虫拖垮 | 484 | 138 |
| 2 | [Explore Wikipedia Like a Windows XP Desktop](https://news.ycombinator.com/item?id=48146129) | XP 风格层级浏览维基 | 439 | 104 |
| 3 | [A 0-click exploit chain for the Pixel 10](https://news.ycombinator.com/item?id=48148460) | Pixel 10 VPU 零点击 root | 265 | 112 |
| 4 | [U.S. DOJ demands Apple/Google unmask 100k car-tinkering app users](https://news.ycombinator.com/item?id=48151383) | 排放执法波及 10 万人隐私 | 237 | 131 |
| 5 | [O(x)Caml in Space](https://news.ycombinator.com/item?id=48147058) | OCaml 协议栈上低轨卫星 | 209 | 49 |
| 6 | [Waymo updates 3,800 robotaxis after they 'drive into standing water'](https://news.ycombinator.com/item?id=48151767) | 涉水识别失败大规模召回 | 85 | 72 |
| 7 | [ABC News has taken all FiveThirtyEight articles offline](https://news.ycombinator.com/item?id=48152553) | 538 全部存档下线 | 88 | 41 |
| 8 | [Image-blaster: 3D environments from a single image](https://news.ycombinator.com/item?id=48150069) | 单图生成 3D 场景 SFX | 83 | 14 |
| 9 | [The sigmoids won't save you](https://news.ycombinator.com/item?id=48147021) | Scott Alexander 反驳 AI 平台论 | 62 | 90 |
| 10 | [Meta to receive $3.3B in tax breaks for $10B Louisiana data center](https://news.ycombinator.com/item?id=48152825) | Meta 路州数据中心税收减免 | 48 | 11 |
| 11 | [WinCE64 – Windows CE 2.11 for N64](https://news.ycombinator.com/item?id=48152729) | N64 上跑 Windows CE | 51 | 11 |
| 12 | [The Zulip Foundation](https://news.ycombinator.com/item?id=48152168) | Zulip 转入基金会治理 | 48 | 10 |
| 13 | [I designed a nibble-oriented CPU in Verilog](https://news.ycombinator.com/item?id=48151237) | 自研 4-bit CPU 跑科学计算器 | 48 | 8 |
| 14 | [Judge Bars Kars4Kids from Broadcasting 'Misleading' Ads in California](https://news.ycombinator.com/item?id=48152777) | 神曲广告被加州法院禁播 | 55 | 18 |
| 15 | [Zenith: live local-first planetarium](https://news.ycombinator.com/item?id=48150097) | 本地优先定视场天象仪 | 55 | 12 |
| 16 | [California bill: patches or refunds when online games shut down](https://news.ycombinator.com/item?id=48152994) | 加州拟立法保护停服老玩家 | 38 | 13 |
| 17 | [Palantir has hired 30+ senior UK Government officials](https://news.ycombinator.com/item?id=48153183) | Palantir 大举挖角英政府 | 24 | 1 |
| 18 | [Microscale Thermite Reaction](https://news.ycombinator.com/item?id=48153142) | 哈佛微缩铝热反应演示 | 16 | 4 |
| 19 | [The nuclear-physics infrastructure behind PET scans](https://news.ycombinator.com/item?id=48122172) | PET 扫描背后的核物理 | 18 | 1 |
| 20 | [Hightouch (YC S19) Is Hiring](https://news.ycombinator.com/item?id=48151034) | Hightouch 招聘贴 | 1 | 0 |

---

## 重点讨论点评

### 🥇 [Project Gutenberg – keeps getting better](https://news.ycombinator.com/item?id=48150431) — 484分 · 138评

**互联网的"公共图书馆"在 AI 爬虫时代如何生存**

Project Gutenberg 最新一轮改版获得社区一致好评：移动端响应式重做、关闭样式仍可读、EPUB3 与即将上线的 PDF 输出全部到位。一位用户的评价代表了主流情绪——"互联网最好的角落之一"。这是少数能让 HN 这种平时挑剔的群体集体放下技术批判、转而表达感谢的话题。

但讨论的下半段才是真正的信号：项目维护者 JSeiko 亲自在帖子下解释，最近性能波动来自"大量爬虫流量"——所有人都心知肚明这是 LLM 训练数据抓取潮的连带后果。社区一边夸 Gutenberg 不商业化、不广告化的纯粹运营，一边讨论 ISP 投诉、CDN 缓存、ABuse 报告等防御方案。一个 70 万册公共领域电子书库正在被现代 AI 经济"无意中"碾压。

另一个绕不开的暗线是 Italy 仍然封禁 Gutenberg——2020 年法院一纸禁令，无人维护、无人撤销。当主权与开源公共品冲突时，开源方几乎没有反击工具。

> *热门评论摘要：* "Standard Ebooks 提供了 GitHub 上完整的版本历史，而 Gutenberg 的版本演化对读者是不透明的"——这是 HN 给项目最实际的下一步建议。

---

### 🥈 [DOJ demands Apple/Google unmask over 100k car-tinkering app users](https://news.ycombinator.com/item?id=48151383) — 237分 · 131评

**当排放执法变成大规模身份扒库**

司法部要求 Apple 与 Google 把使用某款"汽车 ECU 调校 App"的 10 万名用户身份全部上交——理由是排放法（Clean Air Act）执法需要。HN 用户立刻把这个案例与 1990 年代的"Pen Register"、2010 年代的"Smartphone Stingray"、近期的 Geofence Warrants 串成一条逻辑线：政府在用最低举证门槛拿到最大数据集，再事后筛选嫌疑人。

最高赞评论用一个干净的类比击穿了官方逻辑：*"这相当于因为有几起入室盗窃案使用了撬棍，就要求 Home Depot、Walmart、Amazon 把所有买过撬棍的美国人名单交出来。"* 法律上，第四修正案"针对特定人/物"的要求被"全量扫荡"模式正面挑战。技术上，App Store 与 Play Store 作为"事实上的身份注册中心"被首次正式调用——下次可能就是 Tor 客户端用户、加密通讯 App 用户。

讨论里另一条暗线：开发者层面的连带后果。一旦"我的 App 装机量 = 我能被强制要求暴露身份的数据集"，独立开发者还要不要做匿名/隐私强保护？很多开发者表示这会改变他们对"应该收集多少用户标识"的默认设定。

> *热门评论摘要：* "如果你的执法策略前提是'获得所有人身份再筛选'，那你其实承认你没有真正的犯罪证据——你只是在做大规模钓鱼。"

---

### 🥉 [A 0-click exploit chain for the Pixel 10](https://news.ycombinator.com/item?id=48148460) — 265分 · 112评

**Project Zero 用两个漏洞拿下 Android 旗舰内核**

Google 自家的 Project Zero 团队公开了一条针对 Pixel 10 的零点击漏洞链：先利用一个补丁不彻底的 Dolby 漏洞（CVE-2025-54957）作为初始入口，再触发 VPU 驱动 mmap 处理函数里的尺寸校验缺陷——通过指定一个超大 buffer，"可以映射任意多的物理内存"——最终在 71 天内被修复前，可在零交互情况下拿到 root。整条链只用了大约两个漏洞。

HN 社区的讨论集中在两点：第一，VPU（视频处理单元）这种"非主流"内核驱动正变成移动安全的新弱点——主流子系统已经被审计过太多遍，攻击者正向显示控制器、相机 ISP、NPU 这些路径迁移。第二，Project Zero 暴露这条链的同时，恰好处于"AI 安全代理"与"政府预审 AI 模型"的舆论高峰期（参考本周 Anthropic Mythos 的争议），证明再前沿的网安模型也跑不过"两个 typo 级别 bug"的复合利用。

社区还有人指出：71 天修复速度对 Google 自家旗舰来说是"合格但不亮眼"，对于"安全设计标杆"定位的 Pixel 是一次实打实的口碑伤害。同样的漏洞链如果落到非 Pixel Android OEM，可能根本撑不到补丁。

---

### 📡 [O(x)Caml in Space](https://news.ycombinator.com/item?id=48147058) — 209分 · 49评

**纯函数式语言完成在轨后量子密钥轮换**

Borealis 是一个完全用 OCaml/OxCaml 编写的 CCSDS 协议栈，于 2026 年 4 月 23 日在低轨卫星上成功启动，运行加密命令-控制链路。作者用一句"C/C++ 严重 CVE 约 70% 来自内存破坏"为 OCaml 上太空背书，然后亮出两个硬数字：包派发延迟从 29ns 降到 9ns，零 GC 开销；以及完成了首次公开的在轨后量子密钥轮换（OTAR）。

HN 评论分两派：一派欢呼"形式化 / 类型安全语言终于在太空交付证据"，把它与 Ada 在波音、Rust 在 Linux 的故事并列，认为这种 demo 比一万篇博客都更有说服力。另一派挑剔："9ns 是好成绩，但 OxCaml 离 Rust 与 Ada 在嵌入式生态的成熟度还有距离"，以及"在轨样本量 = 1，离主流采购决策还远"。

这条新闻的真正价值在于：它是一组"语言安全性 → 关键系统采购"的具体证据，可以被未来 NASA、ESA 的 RFP 引用，逐步动摇 C/C++ 在航天嵌入式领域几十年的默认地位。

---

### 🤖 [The sigmoids won't save you](https://news.ycombinator.com/item?id=48147021) — 62分 · 90评

**Scott Alexander 给"AI 必然平台"派一记反驳**

Astral Codex Ten 这篇长文专门拆解一类怀疑论者的标准武器："所有指数增长最终都会变成 S 形曲线，AI 也不例外。" Scott 的反驳分三步：第一，平台是数学必然性，没错，但"在哪个点平台"才是关键问题；第二，过去 30 年大量"S 形预言"——联合国出生率、太阳能装机、Wharton 2026 年 AI 报告——刚一发布就被现实打脸；第三，怀疑论者要么具体解释"AI 进步的微观动力为什么会在 X 时点失速"，要么干脆采用 Lindy's Law（趋势越长越可能继续）。

HN 评论区分裂得很有意思：90 条评论里既有 AI 加速派对"S 曲线偷换概念"的拍手叫好，也有 AI 怀疑派直接指出"Scott 自己在做 cherry-picking——发改委计划经济和共产主义国家也曾经被 Lindy 加持"，还有务实派提醒"模型架构 + 数据 + 能源任何一条腿断了都会触发平台"。

这条贴子分数不算最高，但评论/分数比超过 1.4，说明真正的"上下文密度"在评论区——这是典型 HN 思辨型讨论，比单纯新闻聚合更有阅读价值。

---

## 社区脉搏

今天的 HN 呈现三股交织的情绪：

**一是"公共品 vs 工业 AI"的对立**。Project Gutenberg 被 LLM 爬虫拖垮、FiveThirtyEight 全部存档下线、Meta 拿 33 亿税收减免在路易斯安那建数据中心——同一天的几个高票贴拼出了一个清晰反差：去中心化、长期主义的公共信息基础设施在被吞食，而集中式 AI 资本扩张在被补贴。社区情绪复杂——既有挫败感，也有"该不该 Self-host 一份镜像"的实操讨论。

**二是隐私与执法边界的再次紧张**。DOJ 要 10 万车迷身份、Palantir 挖空英国政府、加州想立法保护停服游戏玩家——这三条放在一起，HN 看到的是国家与平台合谋的"数据-合规"复合体在加速。曾经"我有什么好怕的"的天真主义彻底退场，取而代之的是"任何 App 注册都是一次未来执法暴露面"的工程思维。

**三是技术怀旧与硬核工程并存的双峰**。Wikipedia XP 桌面、N64 上的 Windows CE、Nibble 4-bit CPU、火星热反应小实验，与 Pixel 0-click、OCaml 上太空、Image-blaster 单图 3D 同台。HN 在 AI 大模型主导新闻周期的当下，仍然顽固地为"小而精的工艺活儿"提供顶级流量——这种二元性本身就是 HN 区别于其他技术社区最稳定的特征。
