# Hacker News 每日资讯 · 2026-06-29

## 今日焦点

> **AI 进医院 · 开放权重模型反击 · Agent 经济模型重思 · 学术诚信崩盘 · 复古工程美学**
>
> - **用 Claude Code 给 MRI 拿"第二意见"** 顶帖 279 分 386 评，全场最炸的讨论，AI 与医生诊断打架谁信谁的争议愈演愈烈。
> - **GLM 5.2 在 Semgrep 安全 benchmark 上爆 Claude** 235 分 88 评，开放权重 + 价格 1/6 的故事让 HN 重新讨论"国产模型该不该用"。
> - **OpenAI Codex 仍未支持 .codexignore** 168 分 110 评，安全黑洞已开两年，社区耐心见底。
> - **布朗大学教授公开痛斥大规模 AI 作弊** 99 分 121 评，"academic integrity is at risk" 成为常驻话题。
> - **Tokenmaxxing 已死，Tokenmaxxing 万岁** 89 分 113 评，Agent 经济从"烧 token 换 KPI"切换到"烧 token 换正确性"。

---

## 今日热榜总览

| 排名 | 标题 | 描述 | 分数 | 评论数 |
|------|------|------|------|--------|
| 1 | [纽约公共图书馆 1880-1920 馆藏菜单](https://news.ycombinator.com/item?id=48707763) | 5000 张老菜单可视化 | 299 | 80 |
| 2 | [用 Claude Code 给我的 MRI 拿第二意见](https://news.ycombinator.com/item?id=48708941) | AI 与放射科医生打架 | 279 | 386 |
| 3 | [GLM 5.2 在我们的 cyber benchmark 上爆了 Claude](https://news.ycombinator.com/item?id=48709670) | 39% vs 32% F1 | 235 | 88 |
| 4 | [Librepods：解放 AirPods](https://news.ycombinator.com/item?id=48710232) | 跨平台 AirPods 协议逆向 | 203 | 60 |
| 5 | [OpenAI Codex 仍无敏感文件排除机制](https://news.ycombinator.com/item?id=48706714) | .codexignore 仍是空头支票 | 168 | 110 |
| 6 | [Show HN: Zanagrams](https://news.ycombinator.com/item?id=48708182) | 字母排列益智小游戏 | 131 | 45 |
| 7 | [波音 747 开始最后的降落](https://news.ycombinator.com/item?id=48675295) | 一代女皇正式退役 | 109 | 121 |
| 8 | [布朗大学教授痛斥课程考试大规模 AI 作弊](https://news.ycombinator.com/item?id=48708991) | 学术诚信全面失守 | 99 | 121 |
| 9 | [1960-2026 历史内存价格图](https://news.ycombinator.com/item?id=48710092) | 半导体价格穿越史 | 90 | 27 |
| 10 | [Tokenmaxxing 已死，Tokenmaxxing 万岁](https://news.ycombinator.com/item?id=48708795) | Agent 烧 token 的经济学 | 89 | 113 |
| 11 | [Daisugi：日本"母树生子树"古老林木技法](https://news.ycombinator.com/item?id=48708859) | 千年可持续林业奇技 | 88 | 32 |
| 12 | [用龙芯 Yeeloong 笔记本跑 OpenBSD](https://news.ycombinator.com/item?id=48709187) | 复古硬件 BSD 折腾日记 | 80 | 17 |
| 13 | [拆解航天飞机 I/O Processor 电路板](https://news.ycombinator.com/item?id=48708700) | 太空硬件考古 | 72 | 14 |
| 14 | [Show HN: DRM-Free Books](https://news.ycombinator.com/item?id=48709186) | 无 DRM 电子书清单 | 48 | 24 |
| 15 | [ISC'26 TOP500 新冠军揭晓](https://news.ycombinator.com/item?id=48710775) | 全球超算榜易主 | 43 | 28 |
| 16 | [Show HN: NanoEuler – C/CUDA 从零写 GPT-2 规模模型](https://news.ycombinator.com/item?id=48710778) | 教学向裸写训练框架 | 26 | 7 |
| 17 | [LLM 能通过镜子测试吗？](https://news.ycombinator.com/item?id=48710414) | 自我意识哲学实验 | 23 | 15 |
| 18 | [Show HN: Bash4LLM+ 零依赖 LLM API 包装](https://news.ycombinator.com/item?id=48710827) | 纯 bash 写 LLM 客户端 | 18 | 10 |
| 19 | [1968 论文：计算机辅助无言儿童语言开发 [pdf]](https://news.ycombinator.com/item?id=48710350) | dang 亲贴的早期 AAC 史 | 16 | 1 |
| 20 | [Staying Awake (2008)](https://news.ycombinator.com/item?id=48678377) | Wendell Berry 经典随笔 | 9 | 3 |

---

## 重点讨论点评

### 🥇 [I used Claude Code to get a second opinion on my MRI](https://news.ycombinator.com/item?id=48708941) — 279分 · 386评

**当 AI 与放射科医生意见相反，普通人该听谁的？**

作者把肩部 MRI 影像扔进 Claude Code（Opus 4.8），让模型在不知道医生结论的前提下做一次盲读。Claude 报告"肌腱完好"，与他门诊医生给出的"III 级撕裂"完全相反；他又把双方报告交给 Claude 仲裁，加入临床体征后模型仍然站在自己一边，结论是"轻度止点性肌腱病，无部分或全层撕裂"。文章以"我现在到底该信谁"作结，没有给答案。

HN 评论区分化激烈：医疗专业派强调放射诊断需要 prior 序列、临床触诊与超声补充，单张 MRI 让模型读图属于"用错工具"；技术派则反驳放射科年误诊率本身就在 3-5% 区间、二次意见在医学里是默认流程；监管派担忧"AI 二次意见"如果被普及到 ChatGPT 入口、会引发大规模延误就诊与医患信任崩塌。**这是今年 HN 上最典型的"AI 介入高风险领域"案例帖**——它既不是炫技、也不是吐槽，而是用第一人称把"不知该信谁"的尴尬摆到台面上。

> *热门评论摘要：* 多位放射科医生指出 MRI 解读高度依赖 T1/T2 序列对比、患者既往史与体格检查，单张图像即便人类专家也会读错；但也有评论反驳说"医学不是不容质疑的圣物，AI 二次意见在统计学上跟人类二次意见同价值"，这种张力正是评论区 386 楼吵不停的根源。

---

### 🥈 [GLM 5.2 beats Claude in our benchmarks](https://news.ycombinator.com/item?id=48709670) — 235分 · 88评

**开放权重的"实战拐点"出现在安全代码审计上**

Semgrep 团队公布内部 IDOR（越权访问）检测 benchmark：智谱开源的 GLM 5.2 拿到 39% F1，**击败 Claude Code 的 32%**；更关键的是单漏洞成本约 $0.17，仅相当于前沿闭源模型的 1/6。结论很直接：在他们这条"安全分析"窄赛道上，开放权重模型第一次拿到了"性价比 + 能力同时领先"的成绩单。

HN 评论的有意思之处在于：**没人质疑能力（这是新现象）**，争论焦点全部跑到了三个新维度——本地部署的硬件门槛（753B 全量需 $120K-$150K 推理硬件）、benchmark 是否被特定 prompt 工程过拟合、以及更尖锐的"该不该把代码安全审计交给一个由中国实验室训练的模型"。前 HN 5 年讨论"开源 vs 闭源"还停留在"能跑就行"，今天的讨论已经是"性价比 + 地缘 + 部署"三角博弈。

> *热门评论摘要：* 一位 Rust 工程师贴出自己用 GLM 5.2 写加密 agent 的实际账单——$20 完成一项任务，对比闭源模型动辄 $100+；另一位则提醒大家 DeepSeek V4 Pro 在他们内部 benchmark 上比 GLM 5.2 还要好，开源赛道内部的迭代速度已经把闭源拉开第二战线。

---

### 🥉 [A way to exclude sensitive files issue still open for OpenAI Codex](https://news.ycombinator.com/item?id=48706714) — 168分 · 110评

**一个 .codexignore 拖了两年，HN 已经不愿意再"善意理解"了**

issue #2847 请求 Codex 支持仓库级与全局级的 ignore 文件（类似 .gitignore，模式如 `.env`、`*.pem`），让团队能确定性地阻止敏感文件被读入或上传到模型。原 issue #205 早在两年前就提过，被关闭并承诺在 codex-rs 中实现，**截至 2025-08-28 仍未落地，issue 重开后又拖了 10 个月**。

社区的怒火不在功能本身（这是个 100 行的 feature），而在于"OpenAI 拿企业级合约的同时却把基础数据卫生留给用户兜底"。多位评论提到他们公司因此禁用 Codex、改用 Aider / Cline / Cursor，因为后者要么默认支持 .ignore 要么有 git-aware 的扫描器。**最伤的一条留言：**"这不是优先级问题，是态度问题——把安全功能拖两年的厂商，将来上市后也不会变。"

> *热门评论摘要：* 多名安全工程师晒出自家流水线被 Codex 上传 `.env` 文件后被 GitGuardian 警告的经历；少数 OpenAI 员工出现回复说"已经在 sprint 内"，但被反问"两年了每个季度都说在 sprint 内"。

---

### 🎓 No.4 · [Professor denounces mass AI fraud on an exam at Brown](https://news.ycombinator.com/item?id=48708991) — 99分 · 121评

**当一门课的"自由作答题"全班用同一种 LLM 腔调答卷**

布朗大学一位教授在 El País 撰文，描述自己课程期末出现的大规模 AI 作弊：答卷中频繁出现重复的 LLM 风格句式、相同的伪引用，他直接把这种现象定义为"学术诚信的系统性塌陷"。HN 评论分两派：教师/家长派认为这是必然结果——大学几十年来过度依赖"写论文"作为评估手段，AI 出现后这一手段失效；技术派则反讨论说现在所有 AI 检测工具假阳性都太高，惩罚机制本身在制造新的不公。

更有意思的是评论里反复出现的一类"诚实声音"：**"我自己读硕士的时候也用 GPT，但我只用来做参考翻译和润色，作业仍然是自己写——但这个边界已经没人能定义了。"** 这种"灰区共识"正在变成 2026 年大学教务办公室最难处理的真问题。

> *热门评论摘要：* 一位长期助教写道："改 200 份学生作业里有 130 份用 LLM，是当我意识到题目本身已经过时了——这不是学生的错。" 这条评论在子线程被顶到第一，比原文章本身更有传播力。

---

### 💰 No.5 · [Tokenmaxxing is dead, long live tokenmaxxing](https://news.ycombinator.com/item?id=48708795) — 89分 · 113评

**Agent 经济的 KPI 从"烧多少 token"切换到"烧得对不对"**

作者把过去一年企业内"按 token 用量考核 AI 使用率"的做法称为 tokenmaxxing 1.0，认为它已经死亡——补贴退坡 + 真实成本回归后，CFO 不会再让员工"为了考核数据空跑 prompt"。但作者预言 tokenmaxxing 2.0 立刻会接棒：当模型迭代到"更多 token → 显著更高正确率"的 compounding correctness 阶段，对于 24/7 跑的 Agent 来说，把 token 花到极致反而是经济理性。

HN 评论把这篇文章当作 2026 年下半年 agent 商业模式的"思维锚定"反复引用。一条尖锐意见：**这本质上是把开发者从"产品工程师"变成"agent 调度运维"**，工作内容从"写代码"变成"调 prompt 配置 + 监控吐 token 的成本",对很多人来说是一次身份重塑。

> *热门评论摘要：* 一位 platform engineer 留言："我们公司去年 LLM 月支出 $400K，今年压到 $90K，但 agent 输出值翻倍——原因是 80% 的预算花在 5% 的'真值得跑'任务上，剩下 95% 任务直接退回写脚本。" 这种"非对称分配"恰好印证作者关于 tokenmaxxing 2.0 的预言。

---

## 社区脉搏

今天 HN 的主题是**"AI 不再是新闻，而是日常基础设施"**。前 10 帖中有 5 帖直接讨论 AI 落地——MRI 二次意见、开源模型反击、Codex 安全黑洞、AI 作弊、Agent 经济——但讨论氛围已经从去年的"惊叹技术"完全切换到"质问后果"。HN 评论区今天的关键词不是 "this is amazing" 而是 "who owns the consequences"。

非 AI 的"硬核怀旧"流量依然稳定：NYPL 老菜单（299 分）、波音 747 退役（109 分）、龙芯笔记本（80 分）、航天飞机电路板（72 分）——这些贴提醒我们 HN 的真实底色仍然是工程师对"造物美学"的执念，AI 只是借走了流量的顶层，没有改变社区的底层趣味。

值得继续关注的趋势：**开放权重模型在窄赛道（安全审计、代码补全、Agent）首次系统性反超闭源**，叠加"地缘 + 部署成本 + benchmark 信任度"的三角讨论，是 6-7 月 HN 上最有可能持续发酵的议题。
