# Hacker News 日报 · 2026-10-19

## 今日焦点

> **DeepSeek 把搜索 API 打到 $0.75 · 域名注册商信任崩塌 · 开源硬件新巅峰 · 工程师怀念"软件背后的人" · 反 AI 编程语言**
>
> - **DeepSeek 搜索/抓取 API 上线**（515 分 · 251 评）：$0.75/千次成功请求，HN 一致震惊中国定价把搜索类基础设施打回"数据库原价"
> - **Namecheap 没收并禁用全部域名**（333 分 · 160 评）：一位 sysadmin 的 Reddit 控诉引爆 HN，再度让"去中心化域名"话题回潮
> - **RepRapMicron 开源微米级 3D 打印**（310 分 · 47 评）：精度跨进 μm 时代，RepRap 社区二十年来最硬的一次更新
> - **"Someone behind the software"**（252 分 · 107 评）：Linear 创始人 Karri Saarinen 文章戳中工程师对"软件去人格化"的集体情绪
> - **"我做了个 LLM 用不了的编程语言"**（43 分 · 35 评）：反 AI 浪潮延伸到语法层，HN 讨论从玩笑逐渐变成严肃主张

---

## 今日热榜总览

| 排名 | 标题 | 描述 | 分数 | 评论数 |
|------|------|------|------|--------|
| 1 | [DeepSeek search and fetch – $0.75 per 1000 successful requests](https://news.ycombinator.com/item?id=50138531) | DeepSeek 搜索 API 血洗定价 | 515 | 251 |
| 2 | [Namecheap just seized and disabled all my domains](https://news.ycombinator.com/item?id=50142866) | 域名被注册商单方面没收 | 333 | 160 |
| 3 | [RepRapMicron](https://news.ycombinator.com/item?id=50141076) | 开源微米级 3D 打印机 | 310 | 47 |
| 4 | [Someone behind the software](https://news.ycombinator.com/item?id=50142573) | 工程师呼唤软件的"人味" | 252 | 107 |
| 5 | [Show HN: Zelda timeline for Ocarina of Time remake](https://news.ycombinator.com/item?id=50140769) | 塞尔达时间线补课站 | 149 | 88 |
| 6 | [Java sealed classes and exhaustive pattern matching](https://news.ycombinator.com/item?id=50141579) | Java 终于拿到完整模式匹配 | 120 | 97 |
| 7 | [Hybrid Reasoning Agents: think in latent space, act through text](https://news.ycombinator.com/item?id=50145337) | 隐空间思考+文本行动的 Agent | 104 | 41 |
| 8 | [I electrified my push scooter with a power drill](https://news.ycombinator.com/item?id=50093020) | 电钻改装的电动滑板车 | 100 | 41 |
| 9 | [SIGSALY: Churchill's top secret hotline](https://news.ycombinator.com/item?id=50096110) | 丘吉尔的二战加密电话 | 96 | 31 |
| 10 | [Free Pascal: dynamic packages](https://news.ycombinator.com/item?id=50144066) | Free Pascal 支持动态包 | 88 | 12 |
| 11 | [The Intel 8087 chip: FP addition microcode](https://news.ycombinator.com/item?id=50142449) | 8087 浮点加减微码拆解 | 79 | 23 |
| 12 | [Dogs agree 'bouba' is round, 'kiki' is spiky](https://news.ycombinator.com/item?id=50136979) | 狗也懂 bouba/kiki 效应 | 78 | 55 |
| 13 | [PalmOS Lemmings](https://news.ycombinator.com/item?id=50143536) | PalmOS 旅鼠游戏源码 | 70 | 20 |
| 14 | [There's never been a better time to go into math](https://news.ycombinator.com/item?id=50136150) | 3Blue1Brown 力挺学数学 | 68 | 24 |
| 15 | [Beyond Tetris: other games of Alexey Pajitnov](https://news.ycombinator.com/item?id=50136017) | 俄罗斯方块作者的其他作品 | 49 | 1 |
| 16 | [I built a programming language that LLMs can't use](https://news.ycombinator.com/item?id=50135762) | 反 AI 的 killswitch 语言 | 43 | 35 |
| 17 | [One parser, two bugs: Broadcom WiFi exploit](https://news.ycombinator.com/item?id=50122058) | 跨 eCos/Linux 的 WiFi 漏洞 | 27 | 6 |
| 18 | [Developing for Debugging (2025)](https://news.ycombinator.com/item?id=50131053) | 为可调试性而写代码 | 21 | 0 |
| 19 | [16-bit DIY magnetic core memory](https://news.ycombinator.com/item?id=50098148) | 自制 16 位磁芯内存 | 14 | 2 |
| 20 | [They war-gamed dimming the Sun](https://news.ycombinator.com/item?id=50103988) | 日光减量兵棋推演失败 | 7 | 2 |

---

## 重点讨论点评

### 🥇 [DeepSeek search and fetch – $0.75 per 1000 successful requests](https://news.ycombinator.com/item?id=50138531) — 515 分 · 251 评

**中国再次把一个基础设施品类打成"白菜价"**

DeepSeek 悄悄把搜索/抓取 API 挂上官方文档：每一千次**成功**请求 $0.75（失败请求不计费），上下文直接可接入 V4 系列模型。对照一下目前主流选项——Serper $5/千、Brave Search $3/千、Google Custom Search $5/千——DeepSeek 把价格压到了行业的 1/5 到 1/7，而且在"失败不收费"这一条上做到了比云厂商 SLA 还友好。

HN 的 251 条评论几乎分成三派：Agent 开发者狂喜，终于能把 Deep Research 类工作流做成"打得起"的产品；SEO/爬虫服务商担忧现有商业模式被打穿；少数人质疑数据合规——搜索结果到底来自自建爬虫还是转售第三方。有人把这件事和 DeepSeek R1 当初震动 OpenAI 相比：**定价本身就是产品，中国玩家用"性价比"这把武器已经不只打 LLM，开始横扫上下游**。

更深一层的观察：当搜索 API 便宜到忽略不计，Agent 产品的工程重心会从"节省搜索次数"转向"如何让 Agent 多搜几次再决策"，这反过来会推动模型架构向"多轮工具使用 + 并行搜索"倾斜。整个 Agent 栈的成本结构正在被 DeepSeek 重排。

> *热门评论摘要：* 有开发者直接测算：原本一个 Deep Research 任务 $3-$5 的搜索成本，现在压到 $0.5 以内；另一派担心的是 DeepSeek 显然在用亏损换生态位，一旦结束补贴期，用户被迁移成本锁死。

---

### 🥈 [Namecheap just seized and disabled all my domains](https://news.ycombinator.com/item?id=50142866) — 333 分 · 160 评

**注册商单方面权力，又一次被 HN 翻出来示众**

一名长期 Namecheap 客户在 r/sysadmin 发帖：账户内全部域名在没有事先通知的情况下被没收、锁定、禁用，客服给出的理由模糊地指向"TOS 违规"，但不披露具体条款。帖子被转到 HN 后迅速冲上第二位，160 多条评论几乎一边倒谴责。

技术社区对这类事件的反应其实有一个固定模板：先吐槽注册商霸权，然后讨论 ENS/Handshake 等去中心化域名，再回到"但是浏览器不认"的现实僵局。但今天讨论里出现了几个新东西——一是 EU DSA/DMA 下的透明度要求能否被当作杠杆来倒逼注册商公开判决理由；二是**AI 冒名/诈骗域名爆发之后，注册商的"预防性查封"开始走向过度**：被误杀的概率比过去几年都高。

对工程师而言，这是又一次"关键基础设施单点"的教训。TLS 证书、CDN、注册商、支付通道——每一个都可以在 24 小时内让一个合法业务消失。HN 讨论里有人提醒："把域名注册和 DNS 托管分到两家、把邮件 MX 分到第三家"已经成为新型的 opsec 常识。

> *热门评论摘要：* 多位资深管理员表示类似经历不只一次，建议把高价值域名迁到 Cloudflare Registrar 或 Gandi，并开启 WHOIS 代理和 Registry Lock；也有法律顾问建议直接发 ICANN 投诉。

---

### 🥉 [RepRapMicron](https://news.ycombinator.com/item?id=50141076) — 310 分 · 47 评

**RepRap 社区的"微米时刻"**

RepRapMicron 把开源 3D 打印机的精度从 100μm 级一步跨进 1μm 级，使用柔性铰链 + 压电陶瓷 + 自制控制器，整机设计全部放在 Wiki 公开。HN 技术氛围浓厚的一天，评论聚焦在三个点：成本结构（压电陶瓷和干涉仪才是贵的部分，主体机架其实可以 DIY）、工作尺寸（当前只有毫米级）、以及最有争议的——**这是不是在走 fab lab 的老路**。

有人提到 RepRap 社区 20 年前第一次做 PLA 打印时的争论场面：也是"小尺寸、慢速度、商业设备便宜得多"，但正是那波开源让 3D 打印从 20 万美元降到 200 美元。微米级会不会复制这个曲线？讨论里有半导体工程师指出：**真正能撬动的不是芯片制造（光刻路径不同），而是生物微流控和 MEMS 原型**——这两个领域目前被 "每台设备 50 万美元" 挡在门外，微米级开源打印机可能把实验门槛降到大学实验室和 Hackerspace 可以承受的水平。

> *热门评论摘要：* 多条评论建议把 RepRapMicron 和 OpenFlexure Microscope 结合起来做"桌面级生物工程套件"；另有讨论指出控制器部分可用 Teensy + 商用压电驱动器，总成本可以压到 $3000 以内。

---

### 🏅 [Someone behind the software](https://news.ycombinator.com/item?id=50142573) — 252 分 · 107 评

**对"去人格化软件"的集体不满**

Linear 创始人 Karri Saarinen 的博文谈的其实是一件老事：好软件总有一个"看得见的人"站在后面——愿意写回信、承认错误、让你感觉在跟真人打交道。但在 2026 年这个主题突然再度流行，是因为 AI 客服、Copilot 式更新日志、代码生成 PR 爆炸之后，用户和工程师都在怀念"有人格的软件"。

HN 的 107 条评论既怀旧又现实。怀旧的一面：37signals、Fog Creek 早年、Vim 社区、SQLite——都是"面孔清晰"的工程师文化。现实的一面：当你每天收到几十个 AI 生成的 Issue、PR 和用户反馈，再"有人味"的产品人也会被湮没。更尖锐的观点来自几条高赞评论——**"软件背后的人"其实不是产品力，而是用户信任的一种代偿机制**；当用户不再信任公司的制度性承诺，他们转而相信"那个会回邮件的 Karri"。这个论点把文章从美学升到了组织学。

> *热门评论摘要：* 有人指出 Linear 本身就是这个说法的最好反例——产品体验非常"有人味"，但靠的是上百人的工程文化而非创始人一个人；另一派认为未来小团队工具会靠"创始人直接触达"再卷一轮，就像早期 Pieter Levels 式路径。

---

### 🔧 [I built a programming language that LLMs can't use](https://news.ycombinator.com/item?id=50135762) — 43 分 · 35 评

**反 AI 情绪从社交平台蔓延到语言设计**

作者 Dominik Picheta 开玩笑地做了一门"反 LLM 友好"的语言 killswitch——语法故意设计成模型训练数据里罕见的组合、强依赖程序员自定义运算符、每次编译随机化关键字顺序。表面是玩笑，HN 上 35 条评论里却出现了意外严肃的讨论。

有人支持："保留一个 LLM 搞不定的编程空间，是程序员最后的审美阵地。"反对者认为："这就像 20 年前抵制 IDE 自动补全，最终输给了生产力。"也有人指出一个真问题：**随着模型训练数据扩张，任何'LLM 用不了的语言'都只是一个时间窗口，三个月后 Claude 5 就能学会**。但作者的回应切得很准——这不是对抗，而是迫使模型解决"你永远没见过的语言设计"，等于把 killswitch 当做一个长期对抗 benchmark。

这篇被顶到首页，更像是一个情绪指标：开发者对 AI 的态度正在从"热情拥抱"回摆到"保留一点自主"。前面 Linear 那篇"someone behind the software"是产品端的回摆，killswitch 则是工具端的回摆。两者放在一起看，HN 社区在 2026 年末已经进入"后 AI 热"的反思期。

> *热门评论摘要：* 有评论打趣说："等 Claude 5 搞定了，就改名叫 killswitch-ng，继续加密语法。"也有人认真讨论能不能把这个思路做成教育工具，让学生在没有 AI 补全的环境里重建基础能力。

---

## 社区脉搏

今天 HN 的情绪可以用一句话概括：**"价格战让我兴奋，但自主权让我担心"**。515 分的 DeepSeek 搜索 API 和 333 分的 Namecheap 事件是两个极端——前者展示了基础设施商品化带来的红利，后者展示了基础设施单点带来的风险。工程师既想要便宜的 API，又害怕生态只剩几个"大到不能倒的中间商"。

另一条支线更隐蔽：Linear 创始人那篇文章 + 反 LLM 编程语言 + 3Blue1Brown 的"现在正是学数学最好时代"视频，三条看似无关，却共同指向一种**对"AI 时代中人类工程师定位"的集体焦虑**。HN 的回答仍然是老派的：个人工艺、硬核基础、开源硬件——微米级 3D 打印机被顶到 310 分，不是没有理由。

硬件 geek 文化今天格外浓厚：Intel 8087 微码拆解、SIGSALY 二战加密电话、PalmOS Lemmings、DIY 磁芯内存、电钻改装电动车，一股"从 bit 到铁"的复古味贯穿首页。这类帖子的持续回暖，是 HN 对"软件虚无感"的一种本能对冲。

明天继续追的两条线：DeepSeek 搜索 API 的实测质量与数据来源披露；以及 Namecheap 事件是否被 EFF/ICANN 层面接盘推动政策回应。
