# Hacker News 日报 · 2026-10-29

## 今日焦点

> **Apple git 仍信任被吊销 CA · Gemini 4 Carbon 发布 · 指纹库偷偷"合成生物武器" · 新 MacBook Pro PROLED XDR · AI 做"真人税务工作"评测**
>
> - **Apple's git 仍信任被攻陷的 eMudhra 根证书**（991 分 · 371 评）：PKI 吊销链条在企业生态里断得比想象快。
> - **Gemini 4 Carbon**（711 分 · 582 评）：Google 旗舰直接升到 "Carbon" 代号，评论区正打成一片。
> - **"Why is this fingerprinting script creating bioweapons?"**（581 分 · 132 评）：浏览器指纹 SDK 被发现里面藏了合成生物学提示词。
> - **MacBook Pro PROLED XDR + 触控屏**（448 分 · 762 评）：Apple 终于加触控屏，HN 讨论量冲上第一。
> - **Dayjob: Tax**（170 分 · 101 评）：AI Agent 在 50 份真实税务作业上的新 benchmark。

---

## 今日热榜总览

| 排名 | 标题 | 描述 | 分数 | 评论数 |
|------|------|------|------|--------|
| 1 | [Apple's git still trusts the compromised eMudhra certificates](https://news.ycombinator.com/item?id=50271640) | Apple 未撤销被攻陷 CA | 991 | 371 |
| 2 | [Gemini 4 Carbon](https://news.ycombinator.com/item?id=50276792) | Google 发布 Gemini 4 旗舰 | 711 | 582 |
| 3 | [Why is this fingerprinting script creating bioweapons?](https://news.ycombinator.com/item?id=50276998) | 指纹库里嵌生物武器 prompt | 581 | 132 |
| 4 | [Start Doing Graph Theory](https://news.ycombinator.com/item?id=50208960) | 开放式图论教学网站 | 538 | 119 |
| 5 | [MacBook Pro with PROLED XDR Display and Touch](https://news.ycombinator.com/item?id=50276940) | Apple 新 MBP 加触控屏 | 448 | 762 |
| 6 | [The Grid, a factory-scale robot that builds PCBs on demand](https://news.ycombinator.com/item?id=50243060) | PCB 工厂级机器人上线 | 381 | 188 |
| 7 | [CNC Stone Carving](https://news.ycombinator.com/item?id=50274409) | CNC 做哥特石雕的工作流 | 356 | 109 |
| 8 | [Dayjob: Tax – evaluating AI agents on 50 professional tax assignments](https://news.ycombinator.com/item?id=50275626) | AI Agent 真人税务 benchmark | 170 | 101 |
| 9 | [Leak Exposes 41,000 Homeland Security Workers](https://news.ycombinator.com/item?id=50280864) | 国土安全部 4.1 万员工泄漏 | 166 | 57 |
| 10 | [AlpineBSD](https://news.ycombinator.com/item?id=50274251) | Alpine 风格的 BSD 新发行 | 152 | 137 |
| 11 | [Gaussian Splats Part 3: There's Always a Bigger Scene](https://news.ycombinator.com/item?id=50209269) | 高斯点云大场景实践 | 90 | 18 |
| 12 | [The Agent SDK (Cursor)](https://news.ycombinator.com/item?id=50273731) | Cursor 推出 Agent SDK | 84 | 101 |
| 13 | [Formlabs Studio 1 $699 Resin Printer](https://news.ycombinator.com/item?id=50281044) | Formlabs 消费级树脂机 | 60 | 59 |
| 14 | [Show HN: SlideBySide](https://news.ycombinator.com/item?id=50276883) | 不共享屏幕的"同屏"演示 | 45 | 21 |
| 15 | [The case of the 9 bit AES key](https://news.ycombinator.com/item?id=50280722) | AES 密钥"少了一位"排错 | 41 | 13 |
| 16 | [Spiders Spin 'Silk Dope' into Nature's Toughest Material](https://news.ycombinator.com/item?id=50277755) | 蜘蛛丝蛋白"胶体"研究 | 34 | 1 |
| 17 | [The tragedy of losing your Wikipedia page](https://news.ycombinator.com/item?id=50247342) | Wikipedia 页面被删的代价 | 24 | 37 |
| 18 | [Oseberg Tapestry Fragments](https://news.ycombinator.com/item?id=50276883) | 维京船葬挂毯研究 | 13 | 0 |
| 19 | [Rubber Duck I've Ever Had](https://news.ycombinator.com/item?id=50242358) | 作者的 LLM "橡皮鸭"心得 | 12 | 5 |

---

## 重点讨论点评

### 🥇 [Apple's git still trusts the compromised eMudhra certificates](https://news.ycombinator.com/item?id=50271640) — 991分 · 371评

**旧 CA 还在 Apple 工具链里挂着——现代 PKI 的"长尾"问题**

eMudhra 这家印度 CA 之前已经被主流浏览器从信任链里拔掉，但作者发现，Apple 自带的 `git`（以及由此衍生的 Xcode 工具链）在校验 HTTPS 证书时仍然信任这组根证书。换句话说，一个 2026 年的 macOS 开发机，走 `git clone` / `git fetch` 时仍然可以被一个被社区公认不可信的 CA 接受。帖子引爆讨论的点，不是"Apple 又忘打补丁"，而是**系统工具链和浏览器用的信任池不是同一个**——这类"子生态还在用旧根"的问题，正在成为企业 PKI 架构里被反复踩的坑。

HN 评论区把焦点推到了"CA 吊销的真实工程成本"上：吊销 CA 不是修 Chromium 的 bundle 就完事，还要同步 macOS keychain、各发行版 ca-certificates、JDK/Node 的内置池、各种自带 git 的工具。只要有一条支线落后，攻击者就能找到可用的签发链路。

> *热门评论摘要：* 多位安全从业者指出，这种问题常见于把 git / curl 和系统信任池解耦的厂商（Apple、JetBrains、各类打包工具），**真正的修复要么是统一指向 OS 池，要么要有 CA 事件的自动化拉新机制**，否则总会落下几个工具至少一两年。

---

### 🥈 [Gemini 4 Carbon](https://news.ycombinator.com/item?id=50276792) — 711分 · 582评

**Google 正面押注"Carbon 级" Gemini：评论区更关心能不能用，而不是能不能看**

Gemini 4 Carbon 的官方 blog 定位是"下一代旗舰"，HN 评论区 580+ 条，绝大多数不在吵 benchmark，而在吵三件事：**价格、API 可用性、以及 Google 内部到底是不是用它去给 Workspace / Android 做底层替换**。有开发者第一时间贴出成本对比：如果 Carbon 真的能在编程 / Agent 场景替代 GPT-6.1 Terra 和 Claude Sonnet，那意味着 Google 终于回到"价格 + 质量"双优的象限；但也有工程师直接贴出 429 截图，表示配额仍然很紧。

另一条高频讨论：**Google 的"品牌噪声"**。从 Gemini 1 到 4 Carbon 中间插入了 Pro / Advanced / Thinking / Deep Think / Flash / Nano / Carbon 等等后缀，HN 社区普遍认为这套命名系统已经比 OpenAI 更难懂，开发者在选型时成本更高。

> *热门评论摘要：* 高票评论调侃"**Gemini 的最大竞争对手是 Gemini**"——不是模型不行，而是产品矩阵让客户每三个月就要重新读一遍文档。

---

### 🥉 [Why is this fingerprinting script creating bioweapons?](https://news.ycombinator.com/item?id=50276998) — 581分 · 132评

**浏览器指纹库里藏了合成生物学 prompt——反指纹攻防进入 LLM 层**

作者在逆向一个主流浏览器指纹 SDK（nullpt.rs 系列的最新一篇）时，意外发现脚本的某个"异常样本池"里塞了大量看起来像合成生物学任务的 prompt。看完全文后结论较为明确：**这是作者故意用极端 OOD prompt 来触发反指纹引擎（LLM-based）的异常行为**——他想测试当前基于 LLM 的 WAF / fingerprint 过滤器会不会对这类 payload 过敏。

HN 讨论围绕两条线：一是"指纹 vs 反指纹"进入 LLM 时代，WAF 不再只是正则表达式，而是模型推理；二是 bio-safety filter 的误伤率——一旦过度拦截，就反而给攻击者一张可利用的"识别码"。

> *热门评论摘要：* 有安全研究员指出，这类对抗样本会把 LLM 内置的"拒答"行为暴露给前端 JS，**只要能观测到一次拒答，就等于拿到一个新的指纹维度**，这正是作者想展示的攻击面。

---

### 🏭 No.4 · [The Grid, a factory-scale robot that builds PCBs on demand](https://news.ycombinator.com/item?id=50243060) — 381分 · 188评

**硬件 Agent 时代的真实样本：PCB 现在真能"一按下单，机器从铜板到成品"**

CircuitHub 的 "The Grid" 是一台覆盖整条 PCB 工艺（镀铜、光刻、钻孔、SMT、测试）的一体化工厂机器人，整条线被封装成 API，用户在浏览器下单后，中间无人介入。HN 讨论在意的几个点：**成本是否真的碾压常规代工厂、残次品率、从订单到交付的 lead time**；评论区贴出了几组对比数据，结论是对小批量（10-100 片）确实有价格 / 时间优势，但在大批量仍然打不过深圳。

更深层的 HN 情绪是"美国硬件复兴"——这是最近两个月里 HN 第 N 条"工厂机器人回美国"的高分帖，与 Hadrian、Machina Labs、Instrumental 等公司共同构成同一叙事。

---

### 🧾 No.5 · [Dayjob: Tax – evaluating AI agents on 50 professional tax assignments](https://news.ycombinator.com/item?id=50275626) — 170分 · 101评

**Benchmark 从"考试题"走到了"真人税务作业"**

Surge HQ 把 50 份真实的 CPA 税务作业（含附件、客户往来邮件、不完整数据）喂给当前主流 Agent（Claude、GPT-6.1、Gemini），用的是"**结果交付是否可被 CPA 签字**"而不是单纯准确率。排行结果比 GSM / MMLU 这类 benchmark 更难看：顶级模型通过率仍远低于 50%，一旦涉及跨州 / 外币 / K-1 这类情形就全线崩盘。

HN 讨论的焦点在：**专业 benchmark 的真正门槛是"流程保真度"而不是"题干理解"**。有税务从业者评论说，这类 benchmark 比考试题更能揭示 Agent 的真实瓶颈——不是不会算，而是不会把客户给的 PDF、邮件、Excel 组合成一个合法的工作底稿。

> *热门评论摘要：* 多位工程师建议把这类"职业任务"做成行业标杆 benchmark，**让"税务 / 法务 / 医疗"的 Agent 都不得不先过 real-work 评测**，而不是秀 LMArena 分数。

---

## 社区脉搏

- **安全信任池议题重新发酵**：Apple git / eMudhra 事件冲上第一，叠加国土安全部 4.1 万员工泄漏，HN 本周对"CA 吊销"、"OPSEC 卫生"这类基础话题热情明显回升。
- **Gemini 4 Carbon 冲击 Claude / GPT 阵营**：评论区没有去年那种"Google 又慢又贵"的调侃，而是认真讨论 Agent / Codex 切换成本，这是 Google 这代模型第一次被 HN 当成"真选项"而不是"候选"。
- **AI benchmark 范式转移**：Dayjob: Tax、Cursor Agent SDK、再加 AI 做 Wikipedia 页存废讨论，HN 整体情绪在从"看模型分数"转向"看模型能不能干真人工作流"。
- **硬件回潮**：MacBook Pro PROLED XDR、The Grid、Formlabs Studio 1、CNC 石雕——这是近两个月 HN 硬件主题的最高密度之一，社区对"做实物"的兴趣在肉眼可见地回暖。
- **指纹 / 反指纹进入 LLM 时代**：bioweapons prompt 的梗被 581 分推上首页，说明反指纹社区已经开始系统化地把 LLM-based 过滤器当成攻击面之一。
