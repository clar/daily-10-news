# GitHub Trending 日报 · 2026-10-23

## 今日焦点

> **Claude Skill 生态爆发 · AI 审计/逆向工具链 · 国产电视去广告 · DeepSeek Harness 生态 · 中文传统玩具项目回潮**
>
> - `cloudflare/security-audit-skill` 今日 +24,074⭐，Cloudflare 开源了带机器可读结论的 Agent 安全审计 Skill，一天登顶。
> - `Gathin23/cleanyourtv` 今日 +19,359⭐，一个下午做出的 Android TV 去广告 + tvOS 风启动器，被国内外媒体连续转载。
> - `morluto/rea` 今日 +9,591⭐，自称「用 Agent 对任何应用/原生二进制做逆向」的 TypeScript 工具，掀起"Agent for RE"话题。
> - `deepseek-ai/DeepInfer` 今日 +6,254⭐，官方发布高性能大规模 DeepSeek 推理框架，与 Harness 生态形成闭环。
> - `peach-mitao/peach` 与 `Renhuai123/ziwei-doushu` 分别代表本地优先媒体系统与紫微斗数引擎，中文开源有「实用 + 文化」双线崛起。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) | 面向 Agent 的多阶段安全审计 Skill，输出可独立验证的机器可读结果 | JavaScript | 39,242 | +24,074 | — |
| 2 | [Gathin23/cleanyourtv](https://github.com/Gathin23/cleanyourtv) | 用 ADB 去广告，给安卓电视装上 tvOS 风格桌面 | Java | 23,695 | +19,359 | — |
| 3 | [peach-mitao/peach](https://github.com/peach-mitao/peach) | Peach 蜜桃：单用户、本地优先的个人媒体系统 | Python | 2,401 | +16,534 | — |
| 4 | [ifixai-ai/iFixAi](https://github.com/ifixai-ai/iFixAi) | 独立审计 AI Agent 的运行结果，可人工或自审 | Python | 33,145 | +12,944 | — |
| 5 | [morluto/rea](https://github.com/morluto/rea) | 用 Agent 逆向任何应用，从行为到原生二进制 | TypeScript | 365,481 | +9,591 | — |
| 6 | [pengchujin/aerial-tv](https://github.com/pengchujin/aerial-tv) | tvOS 风格的国产电视桌面，开机即接管 | Kotlin | 3,031 | +8,094 | — |
| 7 | [Renhuai123/ziwei-doushu](https://github.com/Renhuai123/ziwei-doushu) | 紫微斗数开源排盘引擎，含四化系统与格局库 | TypeScript | 6,298 | +7,252 | — |
| 8 | [Graphify-Labs/graphify](https://github.com/Graphify-Labs/graphify) | 把代码库 + 文档 + SQL schema + PDF 变成可查询知识图谱 | Python | 132,816 | +7,093 | — |
| 9 | [Ebony-Vinyl/dsh-our-free-model](https://github.com/Ebony-Vinyl/dsh-our-free-model) | DeepSeek Harness 插件：无需登录即可免费调用 DeepSeek V4.1/Kimi K3 | JavaScript | 36,671 | +6,655 | — |
| 10 | [stablyai/orca](https://github.com/stablyai/orca) | 用自己的订阅并行跑多个 Coding Agent 的 ADE | TypeScript | 102,646 | +6,584 | — |
| 11 | [mmparko/dsh-purge](https://github.com/mmparko/dsh-purge) | DeepSeek Harness 破甲镜像：含完整分支/73 tag/提交历史 | JavaScript | 1,669 | +6,438 | — |
| 12 | [deepseek-ai/DeepInfer](https://github.com/deepseek-ai/DeepInfer) | DeepSeek 官方大规模推理框架 | Python | 19,797 | +6,254 | — |
| 13 | [jbiaojerry/ebook-treasure-chest](https://github.com/jbiaojerry/ebook-treasure-chest) | 电子书下载链接汇集库（樊登/微信/京东/喜马拉雅等） | Python | 21,671 | +6,174 | — |
| 14 | [DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail) | 让 Agent 像最懒的高级工程师一样思考：少写就是好代码 | JavaScript | 173,322 | +5,956 | — |
| 15 | [deepseek-ai/deepseek-harness](https://github.com/deepseek-ai/deepseek-harness) | DeepSeek Harness：一切皆插件 | TypeScript | 258,115 | +5,064 | — |

---

## 重点项目点评

### 🥇 [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) — 今日榜首，+24,074⭐

**Agent 安全审计官方化：从「生成文字结论」到「生成结构化证据」**

Cloudflare 把内部用于 Workers 平台的多阶段安全审计流程封装成了一个 Claude Skill，发布首日就狂揽两万多颗星。它的最大卖点并非安全知识本身，而是**结构化输出**：每一条 finding 都带有 severity、category、file、line、failure_scenario、以及可被人独立验证的 reproducer。配合 Review 阶段的 verify 子 Agent，产出被称为「machine-readable」而非聊天式结论。

这是 2026 下半年 Skill 生态的典型拐点：模型厂商与基础设施厂商都在用 Skill 这个「子程序抽象」把过去只能写进 prompt 的审查流程显式化、组件化、再分发。Cloudflare 的 Skill 可被任何 Claude Code 项目直接 `/invoke`，意味着**安全审计不再是一个独立的 SaaS 定价点，而是开源的子程序**。

**生态信号：** Agent 工具链进入「Linux pipe」阶段——各家把自己的看家本领做成可组合的 skill/plugin，赢家不是出 LLM 的人，而是出 **接口与可验证产物** 的人。

---

### 🥈 [Gathin23/cleanyourtv](https://github.com/Gathin23/cleanyourtv) — +19,359⭐

**一个下午搓出的「免广告电视」项目，为什么会在 GitHub Trending 爆炸？**

作者自称「在一个下午里用 ADB 搞定了去广告 + tvOS 风格启动器」。项目使用 Java，面向 Android TV 栈，不但卸载预装广告组件，还把桌面重做成接近 Apple TV 的卡片式 UI，开机自动接管主屏。

这一类作品在社区会周期性爆火：它不解决技术前沿问题，但解决**全球数亿家庭的日常生活痛点**——国产/美产电视卖出后的广告收入已经成为厂商的主要利润来源，用户买单后却必须看广告，这是一个积累已久的愤怒。配套出现在今日 #6 的 `pengchujin/aerial-tv`（针对小米/TCL 国产电视）形成了「海外 + 国内双 fork」的组合。

**生态信号：** 消费电子设备「软件自治」正在成为新的开源方向。类似 PostmarketOS、GrapheneOS 之后，Android TV 开始迎来自己的平民越狱时代。

---

### 🥉 [morluto/rea](https://github.com/morluto/rea) — +9,591⭐

**"Reverse Everything with Agents"：逆向工程进入 Agent 时代**

rea 直接把目标定义为：**Reverse engineer anything with agents, from app behavior down to native binaries**。它把 Agent 作为控制面，把 Ghidra/IDA/Frida/radare2 这类传统工具当作 tool-use 节点来调度，核心能力是——根据你给出的目标（APP 行为、协议、固件、原生库），自动生成逆向脚本并逐步验证。

它所体现的是 2026 Q4 一个明显趋势：**凡是过去需要「专家 + CLI 工具」才能完成的工作流，都在被重新封装成 Agent-first 应用**。这类工具的技术护城河并不是算法，而是对一个具体领域（逆向）的"工作流 scaffolding"。rea 的 TypeScript 技术栈也印证了 Agent 工具链向 Node.js/TypeScript 继续迁移的趋势，Python 不再是唯一首选。

**生态信号：** Agent 应用的下一波增长不在 to-C，而在 **「专家工作流 agentize」**——逆向、取证、漏扫、合规、FP&A，每一个都是百亿规模的垂直 SaaS 机会。

---

### 🏗 [deepseek-ai/DeepInfer](https://github.com/deepseek-ai/DeepInfer) — +6,254⭐

**DeepSeek 官方推理框架，与 Harness 生态形成闭环**

DeepInfer 是 DeepSeek 自家下场做的高性能、大规模推理框架，Python 构建，针对 DeepSeek V4 系列模型的 Mo​E 架构做了深度优化。它的发布与 Harness/DeepSeek-Harness（#15）、以及社区"破甲"分支 `dsh-purge`（#11）、"免登录免费模型"插件 `dsh-our-free-model`（#9）形成了明显闭环：**官方推理 + 开源 Harness + 社区插件 + 镜像分发**。

值得注意的是，DeepSeek 走的是和 OpenAI/Anthropic 完全不同的路线：模型权重 + 推理栈 + Harness 全部放出，社区因此可以就地构建自己的 "DeepSeek 发行版"。这解释了为什么 DeepSeek 相关仓库在 10 月连续霸榜——它的发行策略直接让每一个社区插件都能"卷走"一波流量。

**生态信号：** 当头部美系厂商把发布节奏锁进商业管道，开放权重 + 开放 Harness 的玩家正在用「社区裂变」把流量拉回自己手里。

---

### 📚 [Renhuai123/ziwei-doushu](https://github.com/Renhuai123/ziwei-doushu) — +7,252⭐

**传统玄学也开源：紫微斗数引擎意外成为中文热门**

一个基于倪海厦《天纪》体系的紫微斗数排盘引擎，带四化系统、格局知识库、古籍原文。看似是中文圈的小众文化项目，但它一天拿下 7,000+ ⭐，说明 **GitHub 开始承担中文传统文化与民俗数字化的角色**。类似节奏网格化（HN 第 6 位的 Gridification）和 `jiangshan-map`（本榜 #17）、`ebook-treasure-chest`（#13），今天的 Trending 有相当比例是文化/知识型资源。

从代码观察看，它采用 TypeScript，便于前端排盘可视化嵌入——这个取舍可能和「要被小程序/网页端引用」有关。与之匹配的还有 `peach-mitao/peach`（#3）这种"中国家庭数据主权"项目：**中文开源在 2026 下半年明显进入了「生活化 + 工具化」的第二曲线。**

**生态信号：** 开源不再只是技术人圈层的事，而是中文互联网集体回收"内容资产"与"文化资产"的方式。

---

## 生态观察

**三条主线正在交叉：**

1. **Skill / Plugin 生态进入"官方化"**。Cloudflare 的 security-audit-skill、ponytail、graphify、claude-howto、replica-skill 等齐齐在榜——这说明平台方和社区都认识到 **「Skill = Agent 时代的 npm 包」**，谁先把稀缺工作流做成 Skill，谁就先把流量锁在平台内。

2. **开放权重阵营持续"社区裂变"**。DeepSeek 的 DeepInfer / Harness / dsh-purge / dsh-our-free-model 四条链路并发霸榜，说明在美系厂商走向 IPO 和合规的同时，开放权重阵营正在拼"**裂变分发**"而不是"**官方品牌**"。

3. **"工作流 agentize" 开始走出前沿**。rea（逆向）、orca（并行 Agent ADE）、iFixAi（Agent 自审）、ponytail（懒人 Agent）都在用一句话说清楚自己的"工作流原型"。这意味着 **Agent 应用层的差异化不再靠模型能力，而靠「垂直工作流封装 + 可验证产物」**。

**遇冷方向：** 大型通用 Web 框架今日几乎没有新作上榜。前端生态、Rust 新项目、新型数据库都没有明显曝光。这与过去 1 个季度观察一致——GitHub Trending 的流量已经被 AI/Agent/Skill 高度吸走。
