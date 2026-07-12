# Hacker News 日报 · 2026-07-13

## 今日焦点

> **Terry Tao 用 coding agent 重写老代码 · Claude Code 33k token 前置开销引质疑 · geohot 反 LLM 炒作宣言 · 数字疲劳催生纸质阅读复兴 · 爱尔兰数据中心占电 23%**
>
> - **[Old and new apps, via modern coding agents](https://news.ycombinator.com/item?id=48884815)** Terry Tao 用 coding agent 重造二十年前的数学工具，387 分 111 评创当日最高热度
> - **[Claude Code sends 33k tokens before reading the prompt](https://news.ycombinator.com/item?id=48883275)** 实测 Claude Code 硬编码消耗 33k token 才开始读用户输入，OpenCode 只需 7k
> - **[I love LLMs, I hate hype](https://news.ycombinator.com/item?id=48883343)** geohot 一篇文章把 HN 拉进 LLM"实用主义 vs 布道派"的又一轮辩论
> - **[Irish datacenters now guzzle 23% of the country's electricity](https://news.ycombinator.com/item?id=48884322)** AI 用电挤爆爱尔兰电网，公共讨论从产业向能源政策倾斜
> - **[How to read more books](https://news.ycombinator.com/item?id=48882056)** 225 分 128 评，"如何读回一本纸质书"这类反算法帖子占据 HN 高位

---

## 今日热榜总览

| 排名 | 标题 | 描述 | 分数 | 评论数 |
|------|------|------|------|--------|
| 1 | [Old and new apps, via modern coding agents](https://news.ycombinator.com/item?id=48884815) | Terry Tao 讲 agent 重写老代码 | 387 | 111 |
| 2 | [Claude Code sends 33k tokens before reading the prompt](https://news.ycombinator.com/item?id=48883275) | Claude Code 前置开销实测 | 361 | 202 |
| 3 | [I love LLMs, I hate hype](https://news.ycombinator.com/item?id=48883343) | geohot 反炒作宣言 | 256 | 142 |
| 4 | [How to read more books](https://news.ycombinator.com/item?id=48882056) | 反算法的纸质阅读方法论 | 225 | 128 |
| 5 | [Don't you mean extinct?](https://news.ycombinator.com/item?id=48881830) | 图形引擎老兵的媒体考古 | 168 | 95 |
| 6 | [Chromium 148, Math.tanh is now fingerprintable](https://news.ycombinator.com/item?id=48884853) | 数学函数暴露 OS 指纹 | 139 | 55 |
| 7 | [Irish datacenters now guzzle 23% of the country's electricity](https://news.ycombinator.com/item?id=48884322) | AI 电力挤爆爱尔兰电网 | 134 | 86 |
| 8 | [LARP – Revenue infrastructure for serious founders](https://news.ycombinator.com/item?id=48882569) | Launch HN：财务基础设施 | 105 | 26 |
| 9 | [Tiny Emulators](https://news.ycombinator.com/item?id=48884395) | 网页版复古 8bit 模拟器 | 90 | 3 |
| 10 | [Migrating a production AI agent to GPT-5.6: 2.2x faster, 27% cheaper](https://news.ycombinator.com/item?id=48882716) | GPT-5.6 生产迁移实测 | 77 | 15 |
| 11 | [Why write code in 2026](https://news.ycombinator.com/item?id=48861923) | AI 时代还要不要手写代码 | 76 | 125 |
| 12 | [Automation Without Understanding](https://news.ycombinator.com/item?id=48882554) | arXiv：不懂机制的自动化 | 76 | 37 |
| 13 | [Against Usefulness](https://news.ycombinator.com/item?id=48882956) | 反效用主义随笔 | 67 | 17 |
| 14 | [Mechanistic interpretability applying causality theory](https://news.ycombinator.com/item?id=48883090) | 因果理论解剖 LLM | 67 | 58 |
| 15 | [I Learned to Read Again](https://news.ycombinator.com/item?id=48883238) | 数字疲劳后的重读经历 | 60 | 19 |
| 16 | [Deir El-Medina Strikes](https://news.ycombinator.com/item?id=48822234) | 古埃及第一次记载罢工 | 50 | 7 |
| 17 | [The One-Step Trap (In AI Research)](https://news.ycombinator.com/item?id=48883415) | Sutton：单步陷阱警告 | 35 | 7 |
| 18 | [So you want to learn physics (2021)](https://news.ycombinator.com/item?id=48827126) | Susan Rigetti 物理自学路线 | 23 | 3 |
| 19 | [Ask HN: What Are You Working On? (July 2026)](https://news.ycombinator.com/item?id=48884984) | 月度项目分享贴 | 22 | 35 |
| 20 | [The State of MCP Security](https://news.ycombinator.com/item?id=48884647) | MCP 安全白皮书 | 13 | 0 |

---

## 重点讨论点评

### 🥇 [Old and new apps, via modern coding agents](https://news.ycombinator.com/item?id=48884815) — 387分 · 111评

**顶级数学家承认"我让 AI 重写了 20 年前那些 Fortran/MATLAB 代码"**

菲尔兹奖得主 Terry Tao 在博客里详述用 coding agent（未指名，但从上下文推断是 Claude Code + Codex 混用）批量翻译他 2000 年代堆积的科研代码——从物理仿真、数论小工具到给学生的示例脚本，全部 port 到现代 Python/Rust。他强调 agent 的价值不在于"新代码更快"，而在于让"因为语言过时被埋葬的旧想法"重新可运行、可验证。

HN 评论区被这句话点燃——因为 Tao 不是 AI 布道派，他谨慎、以数学严谨著称，这类背书比 OpenAI 官方发布还有说服力。争论集中在两点：其一，agent 生成的旧代码翻译版本是否真的可信（Tao 说他会单元测试并做 spot-check）；其二，普通程序员是否也应该借机会做一次自己代码库的"文物挖掘"。

> *热门评论摘要：* 有评论指出 Tao 的用法很符合他的方法论——"AI 不是替代思考，而是打通了历史沉没成本"；也有人反驳，Tao 有能力校验、普通开发者 port 完就无人 review 才是真风险。

---

### 🥈 [Claude Code sends 33k tokens before reading the prompt; OpenCode sends 7k](https://news.ycombinator.com/item?id=48883275) — 361分 · 202评

**"你付的账单里 80% 是 harness 开销"引发 202 条讨论**

一位开发者对 Claude Code 与 OpenCode 做了对照实验：拦截 outgoing HTTP 请求，实测发现 Claude Code 每次会话启动会先发送约 33k tokens 的系统提示、工具定义与工作区元数据；OpenCode 只发送 7k。作者的观点很尖锐：Anthropic 的官方 CLI 在为"用户体验"付账，但账单最终转嫁到用户 API bill 上。

HN 争论热点：（1）33k 是否包含 prompt cache 命中的 token？作者回应：即使命中 cache，冷启动那一次仍要计费；（2）Claude Code 的复杂功能（例如自动 file 索引、hooks 系统）是否值得这个开销；（3）Anthropic 定价是否应该在 CLI 层做"harness 免费"补贴。有 Anthropic 员工在评论区半官方回应，承认开销大但强调将在下个版本引入"lightweight mode"。

> *热门评论摘要：* 排名第一的评论指出，Claude Code 33k 里有大量是每次都不变的 tool schema，理论上完全可以走 prompt cache 打折 90%——所以真正问题是"开发者是否理解自己在为哪部分买单"，透明度而非绝对值才是核心矛盾。

---

### 🥉 [I love LLMs, I hate hype](https://news.ycombinator.com/item?id=48883343) — 256分 · 142评

**geohot 又一次点燃"实用主义 vs 布道派"的年度辩论**

George Hotz（geohot）这篇短博客几乎每个季度都会以类似标题重复一次，但每次都能上 HN 首页——因为他既有黑客声望，又对 LLM 泡沫极度警惕。这次的核心论点：LLM 在辅助编码、学习、辅助阅读上确实好用；但"AGI 明年到"、"编程职业消失"这类叙事都是让二级市场炒作的话术，工程一线的实际生产力增益是 20-40%，而不是 10 倍。

HN 评论区呈现"三分格局"：三分之一支持 geohot 的清醒；三分之一反驳说他低估了 agent-based workflow 的复合效应；剩下三分之一在讨论 tinygrad 本身。有意思的是不少 Anthropic/OpenAI 前员工在评论区匿名下场，一边同意 geohot、一边指出内部对"生产力提升"的度量方式与外部报道的 10x 说法有巨大 gap。

> *热门评论摘要：* 一条被广泛引用的评论：过去十年每次技术革命的第一阶段都是"炒作>实际"，第二阶段是"实际>炒作"——LLM 在 2023-2025 处于第一阶段，2026 开始进入第二阶段，geohot 的立场刚好卡在过渡期，所以两派都能拿他说事。

---

### 4️⃣ [Irish datacenters now guzzle 23% of the country's electricity](https://news.ycombinator.com/item?id=48884322) — 134分 · 86评

**AI 电力焦虑第一次以国家电网数据形式出现在 HN 首页**

The Register 引用爱尔兰能源监管署 CRU 的数据：截至 2026 Q2，全国数据中心用电已占 23%，较 2023 年的 17% 大幅上升，且过去 12 个月新增负荷 100% 来自 AI 训练与推理集群。都柏林一些区已经暂停批准新增算力接入。文章附了图表，显示总用电增速已超过全国 GDP 增速。

HN 讨论罕见地跳出了纯技术圈：（1）爱尔兰的数据中心为什么这么密集——历史上是税收+海底光缆+温和气候的组合；（2）绿色电力承诺 vs 实际煤/气电填补的现实缺口；（3）欧盟 AI Act 的能源披露条款是否会先于美国立法生效。也有评论提到"如果 2028 年 GPT-7 训练要 5GW，一个爱尔兰都不够用"。

> *热门评论摘要：* 有当地读者留言，都柏林郊区的居民电费涨了 30%，公众开始把"电价"与"AI"这两个话题挂钩——这在美国还很少发生，但在爱尔兰、荷兰、新加坡已经是政治议题。

---

### 5️⃣ [How to read more books](https://news.ycombinator.com/item?id=48882056) & [I Learned to Read Again](https://news.ycombinator.com/item?id=48883238) — 反算法阅读小气候

**HN 首页同时容纳两篇"重返纸质阅读"的自述，这不是巧合**

两篇文章几乎同时上榜，累计 285 分 147 评。共同论点：短视频 + LLM 对话让人失去连续阅读能力，需要重新训练——从 20 分钟无手机纸书开始。评论区表现出的社区情绪比文章本身更值得关注：许多资深 HN 用户（早年 Reddit /r/books 移民）承认自己已"两年读不完一本书"。

这个话题在过去一年多次登上 HN 首页，但每次评论峰值都在攀升。可以观察到一个转变：2023 年这类文章的评论多是"要用 X 工具管理书单"（工具论），2026 年评论主要是"要与算法对抗"（政治论）。HN 社区自认理性、抗炒作，但在个体注意力这件事上正走向集体反思。

> *热门评论摘要：* 一条高赞评论直接给出解决方案："每天早上第一个小时不碰任何屏幕，就能读完一本 300 页的书用不到两周"——这不是新方法，但 HN 用户在 2026 集体愿意公开这么做，本身是信号。

---

## 社区脉搏

**AI 讨论从"能不能"转向"公不公"。** 今天 HN 首页 20 条里有 7 条与 AI 相关，但没有一条是"发布"或"炒作"型：都在讨论 harness 效率、能源代价、生产力回报、幻觉治理。这是 AI 话题在 HN 语境下的成熟标志——不再讨论产品有没有意思，而讨论"账单谁买、代价谁付、benchmark 谁定"。

**geohot 效应重现。** 每次一位有黑客声望的独立工程师出来给 LLM 泼冷水，评论区就会分裂为清醒派与信徒派——不是因为观点新，而是因为 HN 社区对"内部人反炒作"有极高信任回声。这次 geohot 的文章之后，Terry Tao 那篇"AI 帮我重写 20 年前代码"反而成为反例——一位大师说"有用但要监督"比布道者说"AGI 来了"更有分量。

**能源与硬件话题回归。** 爱尔兰 23% 用电、Chromium 148 fingerprint、Flash-MSA sparse attention 三条硬技术条目同天上榜，说明 HN 对"底层如何真正跑起来"的兴趣在恢复。过去两年被 LLM 应用层挤压的"系统程序员"文化正在缓慢反弹。

**Show HN / Launch HN 冷清。** 当日头部 Show/Launch 只有 LARP（105 分）和 Adaptive Recall（11 分），Kode Dot（8 分），流量明显被 AI 生态圈的深度长文抢走。副产品是——今天不是发布产品的好日子。

**古典气质回潮。** Susan Rigetti 的物理自学指南、古埃及第一次罢工、纸质阅读方法论、旧游戏引擎考古——一整天 HN 首页"考古"占了 5-6 条。当技术圈过速时，社区会自发选择放慢，这在过去十年 HN 上出现过至少三次相似周期。

---

*数据来源：Hacker News Firebase API，抓取时间约上海时间 2026-07-13 上午。*
