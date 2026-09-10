# Hacker News 日报 · 2026-09-11

## 今日焦点

> **数学家怒怼 OpenAI · Shopify 回归原生 · Rust 进 Microsoft Tier-1 · Cognition SWE-2 挑战头部模型 · Forgejo 严重 RCE**
>
> - **[More questions about whether researchers can trust OpenAI with unpublished math](https://news.ycombinator.com/item?id=49639408)** — 526 分 · 535 评。数学家质疑将未发表证明交给 OpenAI 审阅是否安全。
> - **[Shopify moves back to Native from React Native](https://news.ycombinator.com/item?id=49643982)** — 637 分 · 430 评。RN 十年生态迎来最大规模"回炉"。
> - **[Rust is tier-1 language at Microsoft](https://news.ycombinator.com/item?id=49643546)** — 566 分 · 307 评。Rust 首次和 C++/C# 平起平坐。
> - **[Cognition launches SWE-2, rivaling Fable 5.1 and GPT-Astra](https://news.ycombinator.com/item?id=49645443)** — 326 分 · 133 评。Devin 团队第二代 SWE 特化模型上线。
> - **[Forgejo <=16.0.3 Critical RCE](https://news.ycombinator.com/item?id=49645907)** — 127 分 · 48 评。开源 Git 前端出现远程代码执行漏洞。

---

## 今日热榜总览

| 排名 | 标题 | 描述 | 分数 | 评论数 |
|------|------|------|------|--------|
| 1 | [Shopify moves back to Native from React Native](https://news.ycombinator.com/item?id=49643982) | Shopify 弃 RN 回归原生 | 637 | 430 |
| 2 | [Rust is tier-1 language at Microsoft](https://news.ycombinator.com/item?id=49643546) | Rust 升级 MS 一级语言 | 566 | 307 |
| 3 | [Questions about trusting OpenAI with unpublished math](https://news.ycombinator.com/item?id=49639408) | 数学家质疑 OpenAI 保密 | 526 | 535 |
| 4 | [Cognition launches SWE-2 model](https://news.ycombinator.com/item?id=49645443) | Devin 出 SWE 特化二代 | 326 | 133 |
| 5 | [Hitachi launches CO2 heat pump water heaters](https://news.ycombinator.com/item?id=49627634) | 光伏友好热泵热水器 | 270 | 213 |
| 6 | [NASA color trick unveils rock art on Earth](https://news.ycombinator.com/item?id=49645437) | 火星滤色技术看岩画 | 233 | 36 |
| 7 | [Don't let anyone take away your big box of cables](https://news.ycombinator.com/item?id=49645393) | 极客的线材囤积哲学 | 228 | 179 |
| 8 | [Neki (PlanetScale)](https://news.ycombinator.com/item?id=49645686) | PlanetScale 出 PG 托管 | 182 | 73 |
| 9 | [Silicon Valley Transforming the Military-Industrial Complex](https://news.ycombinator.com/item?id=49645754) | 硅谷改写军工复合体 | 133 | 249 |
| 10 | [Forgejo <=16.0.3 Critical RCE](https://news.ycombinator.com/item?id=49645907) | Forgejo 曝严重 RCE | 127 | 48 |
| 11 | [Music Theory for the 21st-Century Classroom](https://news.ycombinator.com/item?id=49647134) | 免费音乐理论教材 | 123 | 60 |
| 12 | [The part of Navier-Stokes no one is talking about](https://news.ycombinator.com/item?id=49650326) | 形式化方法重讲 N-S | 95 | 76 |
| 13 | [JEP 544: Ahead-of-Time Code Compilation](https://news.ycombinator.com/item?id=49647404) | JDK 引入 AOT 代码编译 | 58 | 23 |
| 14 | [OpenAI Agents API](https://news.ycombinator.com/item?id=49649213) | OpenAI 官方 Agents API | 49 | 44 |
| 15 | [Proof of Capture (open-source)](https://news.ycombinator.com/item?id=49649222) | 隐写术版内容真伪证明 | 33 | 28 |
| 16 | [What happens when a GPU writes memory](https://news.ycombinator.com/item?id=49615922) | GPU 写内存底层机制 | 30 | 1 |
| 17 | [NTSB Update on B-767 Runway Excursion](https://news.ycombinator.com/item?id=49650418) | NTSB 迈阿密 767 事故 | 29 | 20 |
| 18 | [Bodily Oddities](https://news.ycombinator.com/item?id=49649789) | 人体奇异统计集锦 | 20 | 16 |
| 19 | [Show HN: Vertumnus – market produce posters](https://news.ycombinator.com/item?id=49604581) | 农贸市场时令海报 | 15 | 6 |
| 20 | [Recursion into Madness](https://news.ycombinator.com/item?id=49603335) | 递归让人抓狂的历程 | 8 | 0 |

---

## 重点讨论点评

### 🥇 [Shopify moves back to Native from React Native](https://news.ycombinator.com/item?id=49643982) — 637 分 · 430 评

**十年跨端叙事的裂缝：Shopify 决定"分手"React Native**

Shopify Engineering 官方博客承认，其在 2020 年后陆续迁移到 React Native 的移动客户端将在 2026-2027 年迭代中回归 iOS/Android 原生。给出的理由涵盖启动性能、Metal/Vulkan 加速、包体、Long-lived 分支的维护负担，以及"跨端团队与专业客户端团队之间的技能错配"。此前 Shopify 长期是 RN 生态最重要的商用背书之一（甚至资助过 Meta 的 Hermes 项目），因此这次表态被视为 RN 商业化路径的一次关键裂缝。

评论区分裂成三派：一派认为 RN 一直只是"90% 够用"的骗术，Shopify 只是终于承认；一派为 Meta / Callstack 辩护，指出 Bridgeless + New Architecture 已经解决大部分性能问题；第三派把矛头指向 React 本身，认为"跨端"是错误抽象——App 不是网页，UI 应该长在平台自己的框架里。

> *热门评论摘要：* 一条高赞评论直指要害："Shopify 不是抛弃 RN 的第一家，只是最有话语权的一家；真正的问题是，Meta 已经用 Threads / Instagram / Facebook 混合栈默许了 RN 无法承担高端体验。"

---

### 🥈 [Rust is tier-1 language at Microsoft](https://news.ycombinator.com/item?id=49643546) — 566 分 · 307 评

**Rust 走完从"实验"到"官方语言"的最后一公里**

Rust Foundation 转载 Microsoft 官方声明：Rust 正式成为 Microsoft 的 Tier-1 语言，与 C++ 和 C# 享有相同的内部工具链、CI、SDK 支持等级。这意味着未来 Windows、Azure、Office 内部服务都可以合规地新写 Rust 代码，而不需再走"特批"通道。此前 Windows 内核在 2023 年首次引入 Rust，Azure 已在多个高并发服务中大规模使用。

HN 讨论集中在两个层面：一是编译时间、异步生态成熟度、以及缺乏正式 ABI 的老问题是否会阻碍大规模内部推广；二是这是否会加速 C++ 的"体面退场"——尤其在美国 CISA 强推"内存安全语言"的政策压力下。

> *热门评论摘要：* "这不是 Rust 赢，而是 C++ 输——微软内部的存量 C++ 代码库还会继续跑几十年，但新代码从这一天起，写 Rust 才是默认选项。"

---

### 🥉 [More questions about whether researchers can trust OpenAI with unpublished math](https://news.ycombinator.com/item?id=49639408) — 526 分 · 535 评

**当学术信任遇上闭源大模型：数学家的一次公开表态**

Andreas Thom 在 Mathstodon 上抛出了这样一个问题：如果研究者把未发表证明或未公开定理喂给 OpenAI 的模型，OpenAI 是否会将其纳入训练集？如果模型某天"复现"出这个定理，那算不算学术不端？这条帖子被搬上 HN 后引爆 535 条评论。

问题不是新问题（GitHub Copilot 早在 2021 年就有类似争议），但数学社区的敏感度更高——数学圈的信任机制建立在"证明公开归属"上，任何"证明泄漏"都可能改变优先权。OpenAI 的用户协议在"是否用付费 API 输入训练"这件事上多次调整，且历史上有过被质疑的行为，这让 HN 的技术社区也开始重新审视自己对闭源大模型的信任边界。

> *热门评论摘要：* "OpenAI 的隐私政策措辞可以在一夜之间改变，而你交给它的证明再也拿不回来了——这不是概率问题，而是不对称风险。"

---

### 🏅 [Cognition launches SWE-2 model, rivaling Fable 5.1 and GPT-Astra](https://news.ycombinator.com/item?id=49645443) — 326 分 · 133 评

**Devin 团队第二代：SWE 特化模型正式加入头部战队**

Cognition（Devin 的母公司）发布 SWE-2，这是其继 SWE-1 之后的第二代软件工程特化模型，官方宣称在 SWE-Bench Verified 上与 Claude Fable 5.1 和 GPT-Astra 拉近到"±3 分区间"，同时推理延迟显著更低。SWE-2 强调对"多文件重构 + 长上下文调试"的原生支持，训练数据混合了 Devin 内部 workflow trace。

HN 讨论氛围比过去的 Devin 事件（"演示造假门"）平和许多，但仍有明显分裂：一部分开发者认为 Cognition 终于交出了"和演示视频匹配"的产品；另一部分则质疑 Bench 分数无法证明真实工程价值，"SWE-Bench Verified 早已经被过拟合"。同时也有 Windsurf、Cursor 用户对比说 SWE-2 是"目前最好用的 agent 后端之一"。

> *热门评论摘要：* "重要的不是 SWE-2 是否'和 Fable 5.1 一样强'，而是它证明了特化模型能在垂类打赢通用模型，这才是 agent 生态未来的方向。"

---

### 🔒 [Forgejo <=16.0.3 Critical RCE](https://news.ycombinator.com/item?id=49645907) — 127 分 · 48 评

**开源 Git 前端的紧急告警：所有自托管实例需立即升级**

Forgejo（Gitea 的社区 fork）官方安全公告披露 16.0.4 修复了一个严重的远程代码执行漏洞：攻击者可以通过精心构造的 Git 请求触发服务器端命令注入，影响所有 16.0.3 及更早版本。由于 Forgejo 是 Codeberg 及众多欧盟公共部门自托管 Git 服务的默认选择，影响面被认为大于普通开源工具。

HN 讨论迅速指向两个方向：一是"这类漏洞在 Git 前端上并不罕见（GitLab / Gitea / cgit 都曾出过 RCE），关键是升级窗口"；二是抱怨 Forgejo 与 Gitea 分叉后维护资源被稀释，"社区分裂让每个分支的安全响应速度都变慢了"。

> *热门评论摘要：* "如果你的公司在跑 Forgejo，请假设你已经被扫过了——立刻升级，然后审计 access log。"

---

## 社区脉搏

今天的 HN 情绪线可以概括为一个反差：**大公司都在"回归 old school"**。Shopify 弃 RN 回归原生、Microsoft 把 Rust 提到与 C++ 平起平坐、Java 21 发布 AOT JEP、开发者热议"珍藏一箱线材"的老派工程师文化——所有热帖背后都有一个共同的问号：*我们过去十年追求的抽象层，现在还成立吗？*

与此同时，**对 AI 的信任裂缝在扩大**。数学家质疑 OpenAI 保密性、Cognition SWE-2 的 Bench 数字被谨慎评估、Costs of War 长文批判硅谷正在改写军工复合体——HN 观众正在从"AI 加速主义"里冷静下来，开始追问代价。

安全侧 Forgejo RCE、NTSB 迈阿密 767 事故调查也提醒社区：无论 AI 说得多热闹，底层基础设施出问题时，还是要看有多少个 real engineers 半夜起来打补丁。**今天的 HN 是"祛魅日"**：对跨端、对大模型、对新范式，都少了一份滤镜。
