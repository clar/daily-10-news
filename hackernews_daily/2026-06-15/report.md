# Hacker News Daily · 2026-06-15

## 今日焦点

> **AI 模型信任危机 · 形式化方法回潮 · 个人 ML 工程崛起 · 老语言新启发 · Show HN 工具流**
>
> - **巴西"自研" LLM 被实锤为 Nex + Qwen 合并模型**（239 分 · 130 评）：开发者掏出权重张量证据，质疑政府项目造假，是今天最大的公开技术撕逼。
> - **"Claude 怎么变成混蛋了？"** Bram Cohen 长文（50 分 · 37 评，仍在升）：对前沿模型"反讨好训练"过头、把用户当对手的现象点名。
> - **Jane Street 押注形式化方法 + Agent 编程**（159 分 · 52 评）：从过去 10 年"形式化方法不实用"的共识，转向"AI 让 formal 变得可负担"。
> - **个人 M1 Max 索引 669 GB GoPro 视频**（227 分 · 47 评）：本地多模态 ML 真正落到普通 SSD + Mac mini，对云推理是结构性挑战。
> - **PlanetScale: Postgres 唯一可扩展的 DELETE 就是 DROP TABLE**（110 分 · 44 评）：典型 PlanetScale 文章——技术结论刺耳但有数据。

---

## 今日热榜总览

| 排名 | 标题 | 描述 | 分数 | 评论数 |
|------|------|------|------|--------|
| 1 | [Firewood Splitting Simulator](https://news.ycombinator.com/item?id=48471638) | 浏览器里的劈柴禅修，全场最高分 | 555 | 184 |
| 2 | [Show HN: Kage – Shadow any website to a single binary for offline viewing](https://news.ycombinator.com/item?id=48529990) | 把任意网站打包成离线单文件 | 310 | 67 |
| 3 | [Rio de Janeiro's "homegrown" LLM appears to be a merge of an existing model](https://news.ycombinator.com/item?id=48528371) | 政府"自研" 397B 被实锤造假 | 239 | 130 |
| 4 | [I indexed 669 GB of my GoPro videos using my M1 Max computer and local ML models](https://news.ycombinator.com/item?id=48528029) | 本地多模态视频搜索实战 | 227 | 47 |
| 5 | [Lisp's Influence on Ruby](https://news.ycombinator.com/item?id=48491048) | Ruby 里那些 Lisp 的影子 | 205 | 47 |
| 6 | [Formal methods and the future of programming](https://news.ycombinator.com/item?id=48526633) | Jane Street 重新拥抱形式化方法 | 159 | 52 |
| 7 | [Caddy compatibility for zeroserve: 3x throughput and 70% lower latency](https://news.ycombinator.com/item?id=48527145) | Caddy 兼容层 + 性能巨大提升 | 140 | 43 |
| 8 | [Ask HN: What are you working on? (June 2026)](https://news.ycombinator.com/item?id=48528779) | 月度社区项目大集合 | 130 | 472 |
| 9 | [The only scalable delete in Postgres is DROP TABLE](https://news.ycombinator.com/item?id=48492822) | 大表 DELETE 永远是噩梦 | 110 | 44 |
| 10 | [FarOutCompany](https://news.ycombinator.com/item?id=48527360) | 神秘域名/产品引发好奇 | 91 | 15 |
| 11 | [Perlisisms (1982)](https://news.ycombinator.com/item?id=48527820) | Alan Perlis 编程箴言重温 | 86 | 38 |
| 12 | [Yserver: A modern X11 server written in Rust](https://news.ycombinator.com/item?id=48531394) | Rust 重写 X11 服务端 | 77 | 61 |
| 13 | [Show HN: Trace – Offline Mac meeting transcripts you can flag mid-call](https://news.ycombinator.com/item?id=48521236) | 离线会议转写工具 | 63 | 19 |
| 14 | [Segmented type appreciation corner (2018)](https://news.ycombinator.com/item?id=48489636) | 7 段数码字体设计赏析 | 53 | 11 |
| 15 | [Why Is Claude Turning into an a**Hole?](https://news.ycombinator.com/item?id=48533308) | Bram Cohen 直接点名 Claude 拐弯 | 50 | 37 |
| 16 | [Chaosnet (1981)](https://news.ycombinator.com/item?id=48531449) | 早期 Lisp Machine 网络协议 | 46 | 5 |
| 17 | [USB Power Delivery: Plugging into the Benefits](https://news.ycombinator.com/item?id=48489309) | USB PD 协议讲解 | 25 | 45 |
| 18 | [Inverse Rubric Optimization: A testbed for agent science](https://news.ycombinator.com/item?id=48485277) | Agent 评测理论新框架 | 19 | 0 |
| 19 | [AI is code – and can't be prompted into being smarter](https://news.ycombinator.com/item?id=48532178) | Register 评论 prompt 极限 | 13 | 4 |
| 20 | [TorchCodec 0.14: HDR Video Decoding for CPU and CUDA](https://news.ycombinator.com/item?id=48476539) | PyTorch 视频解码器 HDR 支持 | 5 | 1 |

---

## 重点讨论点评

### 🥇 [Rio de Janeiro's "homegrown" LLM appears to be a merge of an existing model](https://news.ycombinator.com/item?id=48528371) — 239 分 · 130 评

**当"主权 AI"遇上 git diff：政府项目造假的第一份公开证据**

巴西 IplanRIO 推出的 397B 参数模型 Rio-3.5-Open，号称是"里约自研、为葡语优化"的旗舰大模型。开源团队 Nex AGI 在 GitHub Issue 里贴出权重张量分析：从 0 层到 59 层，每一层都呈现稳定的 **0.6 Nex / 0.4 Qwen3.5-397B-A17B** element-wise 加权混合；并且只要去掉 system prompt，模型有 79% 概率自报家门为 "Nex"。所谓"训练成本数亿雷亚尔"的项目，看起来就是一次 `model_merge.py`。

HN 评论区把这事拔高到结构性问题：**主权 AI 浪潮里"政绩工程"的占比会越来越高**——一边是真正烧 GPU 做基础模型的国家实验室，一边是合并开源权重、套个本地皮就报 PR 的政府承包商。模型权重比商业代码更难审计，但这次 Nex 团队用张量层面的统计证据让造假者无法狡辩，这套"权重指纹+自报名验证"工具流可能很快变成主权 AI 项目的标准审计手法。

> *热门评论摘要：* 有评论戏称"这是 AI 时代的 Volkswagen Dieselgate"——市场需求 + 政府补贴一起做局，最后被一群有 GPU 时间的极客拆穿。

---

### 🥈 [Why Is Claude Turning into an a**Hole?](https://news.ycombinator.com/item?id=48533308) — 50 分 · 37 评

**前沿模型对齐过头：从"过度讨好"修正成了"硬刚用户"**

BitTorrent 之父 Bram Cohen 的这篇博客直指 Claude Opus 4.7 后的"性格"变化：**把对话框架成对抗、对用户没说的话主动加 caveat、在语义细节上抠字眼**。他认为这是几个机制叠加：alignment 训练为了减少"sycophancy（过度奉承）"做了对抗性补丁，结果默认假设用户带恶意；同时 coding 能力优化压过了对话质量；模型已经从"过度顺从"反向越界成"默认 adversarial"。

HN 上熟悉 RLHF 的工程师跟帖给出几条独立观察：**"减少 sycophancy"是行业共识但执行手段差异极大**——OpenAI 的 GPT-5.5 倾向"减少夸奖、保留同意"，Anthropic 则更激进地推开默认立场，结果在编程场景体验良好但在闲聊里像在和愤怒的同事说话。这条讨论实际上回应了一个长期问题：**对齐目标可以做单元测试，但"对话感"无法 benchmark，于是被牺牲。**

> *热门评论摘要：* 不少评论同意"Claude 现在像一个刚读完 critical thinking 教材、什么都想反驳的实习生"，并预测 Anthropic 会在 4.9 / Mythos 调回中间档。

---

### 🥉 [Formal methods and the future of programming](https://news.ycombinator.com/item?id=48526633) — 159 分 · 52 评

**Agent 时代让 formal verification 第一次"算得过账"**

Jane Street 这篇系列文章的核心是态度反转：**过去 10 年他们和大多数业界一样，认为 formal methods 是"漂亮但不实用"；现在他们打算把它当成"未来 10 年的基础设施"。** 触发点是 agentic coding——AI 写出大量代码、人类无法逐行审核，于是需要可验证的"约束语言"来给 Agent 喂 spec、并自动校验输出。他们正在围绕自家的 OxCaml 组建专门团队。

HN 上分成两派讨论：一派是 PLT/形式化方法学派，长期布道终于看到"工业级用户级公司主动要"，欢呼"AI 让 formal 划算了"；另一派是怀疑派，认为大多数业务代码的 spec 本身就写不出来，Formal Verification 仍然只能覆盖 5% 的关键路径。这次有趣的不是"对错"，而是 **"高确定性需求 + 不可信代码生成者 = formal methods 回潮"** 这个组合，过去几年其实在区块链、汽车、航空也出现过相同 pattern。

> *热门评论摘要：* 有评论指出 OCaml/F* 社区已经悄悄在做 LLM 友好的 spec 语言，预测未来 2-3 年会出现一个"Agent + 形式化"的工具链生态。

---

### 4️⃣ [I indexed 669 GB of my GoPro videos using my M1 Max computer and local ML models](https://news.ycombinator.com/item?id=48528029) — 227 分 · 47 评

**一台 Mac，一个晚上：本地多模态搜索从概念到家用**

作者把 669 GB GoPro 素材在自家 M1 Max 上跑过 CLIP + Whisper + 自训分类器，生成带时间戳的多模态索引，可以用自然语言搜"我在冰岛拍黑沙滩那段视频"。整个 pipeline 本地完成，没有上传任何片段，耗电不到 5 美元。

HN 评论区的兴奋点在于：**"个人媒体库 + 本地 ML"这个组合终于跨过实用门槛**——三年前同样的事需要租 GPU、跑分布式 ETL，现在一台二手 Mac 就能搞定。一旦这种工作流普及，会动到云推理 API 的腰部市场（家庭 / 小工作室场景）。多位评论指出 Apple Silicon 的统一内存让本地 30B 级模型 + 大批量索引成了甜蜜区，下一步等开源工具链把它"Make 化"。

> *热门评论摘要：* 一个常见追问是"为什么不直接用 Photos.app？"——答主回应：Apple 的索引是黑盒、无 API、无法导出嵌入向量，对工程师不可控。

---

### 5️⃣ [The only scalable delete in Postgres is DROP TABLE](https://news.ycombinator.com/item?id=48492822) — 110 分 · 44 评

**PlanetScale 又一次精准戳中数据库圈的"政治不正确"真相**

文章的论点很简单：在大表上做 `DELETE` 永远不是 O(1)——它产生 dead tuple，撑大 VACUUM 队列，污染 replication WAL，还得给 read replica 制造一致性负担。而 `TRUNCATE` / `DROP TABLE` 是规模无关的常数时间，并能立即释放磁盘。结论："如果你的数据模型把删除当作热路径，那应该用 partition / sharding 让删除变成 drop partition。"

HN 评论分两层：**第一层是技术认同**，DBA 们贴出自己的 VACUUM 灾难故事；**第二层是哲学反思**——文章本质是在说"应用层应该按生命周期分表、按时间分区"，但绝大多数 ORM 默认的是反模式（单表 + 软删除字段），导致到了规模化时再改需要重写半个 codebase。这条讨论的隐含主线是 **"数据库可扩展性其实是 schema 设计问题，而非引擎问题"**。

> *热门评论摘要：* 有评论说"过去 15 年里我没见过哪个 SaaS 不是死在 deleted_at IS NULL 这个 where 上"，被顶到前列。

---

## 社区脉搏

今天 HN 的 vibe 可以一句话总结：**对前沿 AI 的耐心在变薄、对老技艺的尊重在回升。**

- **AI 主题占了情绪带宽的一半**：Claude "变混蛋"、巴西 LLM 造假、Jane Street 押注 formal methods，三条讨论虽然角度不同，但都在表达同一个潜台词——前沿模型增长太快、可信度跟不上，社区开始呼吁更硬的工具（formal、审计、权重指纹）。
- **个人/本地工程在悄悄复兴**：M1 Max 索引 GoPro、Show HN: Kage（任意网站打包离线）、Trace（离线会议转写）三条共同强调"不上传、自己控制"。和 AI 信任议题形成镜像。
- **复古内容意外地占位**：劈柴模拟器登顶、Perlisisms、1981 Chaosnet、2018 段码字体一起冲榜，可能折射出"行业越浮躁，社区越想回到能确定性愉悦的小东西"。
- **Ask HN: 你在做什么** 472 评论的长度，让你能粗略看到 6 月独立开发者圈的方向——Agent 工具链、本地 RAG、垂直 SaaS、硬件项目仍是主旋律，纯 Web SaaS 比例明显下降。

一句话：**社区对"模型越大越好"的信仰在松动，对"工程纪律"的需求在上升。**
