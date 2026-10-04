# Hacker News 日报 · 2026-10-05

## 今日焦点

> **本地推理突围 · 隐私抵抗 · 社区悼念 · 数据中心公民监督 · DIY 工程浪漫**
>
> - **Qwen 3.8 Flash Next 跑在 4090 上**：125B 参数、100 token/s，524 分 261 评 —— 本地推理第一次兑现"消费级硬件跑前沿模型"的承诺
> - **移除 macOS 27 的 Apple Intelligence**：219 分 127 评 —— 社区对内嵌 AI 的抵抗情绪与"磁盘空间"同时发酵
> - **Bob Cringely 去世**：782 分 168 评 —— 老 geek 们集体回忆 PBS 时代的技术启蒙
> - **Google 数据中心耗水曝光**：改错的红框暴露了内布拉斯加小镇的真实水电数据，公民监督再立一功
> - **ASIC Puzzle 结果公布**：Jane Street 的硬件谜题吸引了 HN 工程师群体的集体解谜

---

## 今日热榜总览

| 排名 | 标题 | 描述 | 分数 | 评论数 |
|------|------|------|------|--------|
| 1 | [Tell HN: Bob Cringely 去世](https://news.ycombinator.com/item?id=49949438) | 社区悼念元老 | 782 | 168 |
| 2 | [Qwen 3.8 Flash Next 在 RTX 4090 跑 100T/s](https://news.ycombinator.com/item?id=49953495) | 消费级跑 125B | 524 | 261 |
| 3 | [关闭 macOS 27 的 Apple Intelligence](https://news.ycombinator.com/item?id=49957116) | 回收磁盘空间 | 219 | 127 |
| 4 | [Google 数据中心水电数据因误涂泄露](https://news.ycombinator.com/item?id=49957068) | 公民监督胜利 | 152 | 194 |
| 5 | [Show HN: Glashütte Trash Clock](https://news.ycombinator.com/item?id=49930439) | 垃圾造摆钟 | 151 | 20 |
| 6 | [全球灯塔地图](https://news.ycombinator.com/item?id=49933461) | 可视化小玩具 | 149 | 64 |
| 7 | [Show HN: 本地照片 / 视频帧 AI 搜索](https://news.ycombinator.com/item?id=49952111) | macOS Spotlight 替代 | 130 | 62 |
| 8 | [Jane Street ASIC Puzzle 答案](https://news.ycombinator.com/item?id=49934078) | 硬件谜题解法 | 63 | 24 |
| 9 | [胶片扫描流水线自动化](https://news.ycombinator.com/item?id=49946148) | 35mm DIY | 55 | 38 |
| 10 | [Bill Draper 去世](https://news.ycombinator.com/item?id=49953288) | VC 元老辞世 | 53 | 12 |
| 11 | [Neanderthals Among Us 书评](https://news.ycombinator.com/item?id=49947565) | 考古与基因 | 48 | 43 |
| 12 | [Homa：AI 集群不再用 TCP (视频)](https://news.ycombinator.com/item?id=49957117) | RDMA 新协议 | 36 | 6 |
| 13 | [用 AI 规模化保持艺术 (视频)](https://news.ycombinator.com/item?id=49951891) | 创作者讨论 | 35 | 10 |
| 14 | [页表内存消耗](https://news.ycombinator.com/item?id=49916753) | 内核性能 | 30 | 2 |
| 15 | [想要个自定义域名邮箱](https://news.ycombinator.com/item?id=49956092) | 自建邮件血泪 | 28 | 30 |
| 16 | [学术研究激励机制](https://news.ycombinator.com/item?id=49956035) | 论文内卷 | 20 | 10 |
| 17 | [Show HN: Build with Python 入门课](https://news.ycombinator.com/item?id=49956771) | 可视化编程 | 17 | 3 |
| 18 | [宣布鸟类灭绝的中位等待时间：36 年](https://news.ycombinator.com/item?id=49948738) | 保护生物学 | 13 | 7 |
| 19 | [Infidel Goes Wild](https://news.ycombinator.com/item?id=49943637) | 冒险游戏考古 | 12 | 0 |
| 20 | [听鲸鱼的人](https://news.ycombinator.com/item?id=49932350) | 海洋生物声学 | 9 | 1 |

---

## 重点讨论点评

### 🥇 [Tell HN: Bob Cringely has died](https://news.ycombinator.com/item?id=49949438) — 782分 · 168评

**一代 geek 的集体告别**

Bob Cringely —— 本名 Mark Stephens —— 的离去让 HN 短暂安静了下来。对 40 岁以上的开发者而言，PBS 系列 *Triumph of the Nerds*、*InfoWorld* 后页的 "Notes from the Field" 专栏，几乎就是他们对硅谷早期历史的第一印象来源。相比 Steve Jobs/Gates 那些"主角视角"的回忆录，Cringely 的叙述方式是"小道消息 + 工程师八卦 + 轻度幽灵化"——这才是真正塑造了硅谷文化基因的话术。

评论区大量开发者分享"我是因为看了 Triumph of the Nerds 才入行的"类似的回忆，有人直接提到他对 Xerox PARC、Apple II、OS/2 事件的二手记录如何成为他们"真正理解计算机历史"的入口。少数人指出 Cringely 后期的预测（PBS *Nerd TV*、*The Mother of All Demos* 周年纪念）逐渐偏离主流，但没人反驳他对早期硅谷"氛围"的还原力。

> *热门评论摘要：* "他是那种让你第一次意识到——计算机不是魔法、是一群古怪但聪明的人造出来的——的作者。"

---

### 🥈 [Qwen 3.8 Flash Next on RTX 4090 at 100 T/s](https://news.ycombinator.com/item?id=49953495) — 524分 · 261评

**本地推理终于兑现"消费级"承诺**

Strata 项目把 Alibaba Qwen 3.8 Flash Next（125B MoE，激活约 15B）压到单张 RTX 4090（24GB VRAM）上，并在 Q4 量化下跑到 100 token/s。这是本年度最有象征意义的本地推理突破：**125B 规模的旗舰开源模型第一次能在非专业卡上做到接近 Claude Sonnet 速度的输出**。

评论区分裂成两派：工程派逐行讨论 KV cache 压缩、expert routing 的内存复用策略，以及 flash-attention v4 对消费卡的实际加速；产品派则在争论"这意味着什么"—— 有人说这是家庭 agent 的起点，有人说推理成本下降至此会直接威胁 OpenAI 中端定价。少数评论指出 Q4 量化带来的能力退化在复杂推理和代码任务上仍可感知，不要神化。

> *热门评论摘要：* "我们已经走到'小模型跑在小硬件'→'大模型跑在小硬件'的阶段。下一步是什么？'大模型跑在手机'——而这可能只需要 18 个月。"

---

### 🥉 [Improper redaction reveals Google data center water/electricity usage](https://news.ycombinator.com/item?id=49957068) — 152分 · 194评

**公民监督再立一功**

内布拉斯加州林肯市公布 Google 数据中心的监管文件时，使用了"遮罩"而非真正的像素级删除——结果用 PDF 工具一键选中就能看到原始数字。社区立刻复算出：**该数据中心单日用水约 500 万加仑、年耗电量超过 2.5 TWh**，相当于整个林肯市普通家庭用水量的两倍、用电量的三分之一。

评论区的愤怒不是对数据本身，而是对"遮罩文化"：Google 以商业机密为由要求政府封存环境数据，而政府接受这种话术。众多评论把这件事与 Microsoft 在爱尔兰、Amazon 在俄勒冈的类似保密条款放在一起对照——AI 时代的基础设施扩张正在吃掉社区的实际资源，而社区却无权知情。

> *热门评论摘要：* "这不是技术问题——是政治问题。如果 AI 建设需要这么多水和电，公众至少有知情权。"

---

### 🏅 [Turn off Apple Intelligence on macOS 27](https://news.ycombinator.com/item?id=49957116) — 219分 · 127评

**AI 嵌入 vs. 用户抵抗**

RemoveMacAI 本质上是一个脚本工具链，用来关闭并清理 macOS 27 内置的 Apple Intelligence 组件，可回收 7–15 GB 磁盘空间。看起来是小事，但评论区演变成了一场"内嵌 AI 的边界"大讨论：很多开发者抱怨 Apple Intelligence 在后台跑 embedding、索引用户数据，CPU/磁盘占用显著，而默认开启、没有真正的"全关闭"开关。

有人对比 Windows Recall 的隐私风波，认为 Apple 虽然做了 Private Cloud Compute 的技术承诺，但在"用户选择权"这条线上并没有本质差异。另一批人则认为"关掉 AI 等于回到 2010 年"——反对的是哲学问题，不是实现问题。

> *热门评论摘要：* "我不反对 AI，我反对的是别人替我决定什么时候让 AI 看我的文件。"

---

### 🎖️ [Show HN: Glashütte Trash Clock](https://news.ycombinator.com/item?id=49930439) — 151分 · 20评

**浪漫工程主义的小胜利**

艺术家 Niklas Roy 用捡来的垃圾造了一个 30 分钟摆动周期的机械摆钟，机构全靠纸板、金属废料和重力——完全没有电。虽然评论数不算多，但 HN 社区对这类"把物理学变成艺术"的项目一向偏爱。文章里详尽记录了钟摆周期计算、擒纵机构选型、空气阻力调参的过程。

这类项目在 HN 的高分，反映了一个被忽视的侧面：**当技术世界被 AI 和融资新闻轰炸时，一个精巧、无电子元件的手工项目仍然能静静地拿到 150+ 分**。社区的审美底盘始终是"工程浪漫"。

---

## 社区脉搏

今天的 HN 情绪可以用两个关键词概括：**致敬**与**抵抗**。

**致敬**体现在两位元老的离世——Bob Cringely 和 Bill Draper——都在首页获得了高热度讨论。Cringely 代表的是硅谷文化叙事者的一代，Draper 则是风险投资业的奠基者之一。两条讣告加起来超过 800 分，社区在集体整理一段正在远去的历史。

**抵抗**则体现在三条平行叙事上：（1）本地推理（Qwen 3.8 + Strata）展示了社区对"主权算力"的持续追求；（2）移除 Apple Intelligence 的工具暴露了对"内嵌 AI 默认开启"的强烈反感；（3）Google 数据中心水电数据的意外泄露引发了对基础设施保密文化的愤怒。三条合起来，社区的态度非常清晰：**AI 可以用，但使用方式必须交回用户手里**。

副线上，Jane Street ASIC Puzzle 的解法贴、35mm 胶片扫描自动化、垃圾摆钟——这类"低密度高技术"内容依然稳稳进入前 20，说明 HN 的审美底盘没有被 AI 议题吞没。社区仍然热爱"做一件漂亮的工程"。

明日关注：Qwen 3.8 的量化与推理 benchmark 后续、Google 内布拉斯加数据中心的监管回应、以及 Apple 是否会对"关闭 Apple Intelligence"开出正式路径。
