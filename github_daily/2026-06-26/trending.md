# GitHub Trending Daily · 2026-06-26

## 今日焦点

> **Agentic 工程占据半壁江山 · Apple Container 持续吸量 · Claude Code 生态扩张 · 视频/SEO/旅游 SaaS 自托管化 · 安全技能库爆发**
>
> - `calesthio/OpenMontage` 单日 +3,553⭐，把"视频制作"做成 12 条 pipeline + 52 个工具的 agentic 系统
> - `google-labs-code/design.md` +1,407⭐，Google Labs 推出"给 coding agent 看的视觉身份规范"
> - `apple/container` +1,366⭐，Mac 上的轻量 Linux 容器项目继续抢占 Docker Desktop 份额
> - `JCodesMore/ai-website-cloner-template` +1,021⭐，"AI 克隆任何网站"模板化套件升温
> - `mukul975/Anthropic-Cybersecurity-Skills` +600⭐，817 条 MITRE/NIST/D3FEND 对齐的安全技能库

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|------------|-------|
| 1 | [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) | 开源 agentic 视频制作系统（12 pipeline / 52 tool） | Python | 21,974 | +3,553 | 2,467 |
| 2 | [google-labs-code/design.md](https://github.com/google-labs-code/design.md) | 给 coding agent 看的视觉身份规范格式 | TypeScript | 19,052 | +1,407 | 1,640 |
| 3 | [apple/container](https://github.com/apple/container) | Mac 上的轻量级 Linux 容器虚拟机 | Swift | 43,169 | +1,366 | 1,266 |
| 4 | [JCodesMore/ai-website-cloner-template](https://github.com/JCodesMore/ai-website-cloner-template) | AI 克隆任意网站的模板 | TypeScript | 20,358 | +1,021 | 3,003 |
| 5 | [garrytan/gstack](https://github.com/garrytan/gstack) | 23 条 Claude Code 集成的高管/设计/工程工作流 | TypeScript | 115,754 | +836 | 17,159 |
| 6 | [mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | 817 条 MITRE/NIST/D3FEND 安全技能库 | Python | 21,170 | +600 | 2,441 |
| 7 | [opendatalab/MinerU](https://github.com/opendatalab/MinerU) | 把复杂文档转成 LLM-ready 数据 | Python | 69,501 | +524 | 5,878 |
| 8 | [shanraisshan/claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice) | Claude Code 从入门到 agentic 最佳实践 | HTML | 60,478 | +450 | 6,059 |
| 9 | [IceWhaleTech/CasaOS](https://github.com/IceWhaleTech/CasaOS) | 个人云 / 自托管面板 OS | Go | 34,770 | +202 | 1,990 |
| 10 | [xbtlin/ai-berkshire](https://github.com/xbtlin/ai-berkshire) | Claude Code 多 agent 对抗式价值投资研究框架 | Python | 1,797 | +201 | 292 |
| 11 | [alibaba/page-agent](https://github.com/alibaba/page-agent) | JS 内嵌的页面级 GUI agent，可自然语言控网页 | TypeScript | 19,770 | +196 | 1,705 |
| 12 | [Free-TV/IPTV](https://github.com/Free-TV/IPTV) | 免费 TV 频道 M3U 播放列表 | Python | 18,187 | +141 | 2,676 |
| 13 | [mauriceboe/TREK](https://github.com/mauriceboe/TREK) | 自托管的实时协同旅行规划平台 | TypeScript | 6,585 | +112 | 602 |
| 14 | [every-app/open-seo](https://github.com/every-app/open-seo) | Semrush / Ahrefs 的开源替代 | TypeScript | 2,470 | +57 | 294 |
| 15 | [aws/agent-toolkit-for-aws](https://github.com/aws/agent-toolkit-for-aws) | AWS 官方 MCP server / skill / plugin 套件 | Python | 1,115 | +15 | 113 |

---

## 重点项目点评

### 🥇 [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) — 今日榜首，+3,553⭐

**视频制作领域第一个真正"agentic 工作流"开源系统**

OpenMontage 把传统的"非线性剪辑（NLE）"概念彻底拆解成 12 条独立 pipeline + 52 个工具，由 Anthropic Claude/OpenAI 等 LLM 编排：剪辑、配色、转场、字幕、配乐、合规审查每一步都是 agent 可调用的能力。这种结构允许用户用自然语言下指令（"剪一个 2 分钟版本，去掉所有静音段，加配乐 lofi"），系统自动调度 pipeline 完成。

这是过去 6 个月"agentic 工程"潮流真正落地到创作工具的标志事件。和 Adobe Premiere 收购 Firefly 之后向 AI Suite 进化的方向不同，OpenMontage 走的是**"工具拆解化 + 编排开放化"**路线——这意味着它的真正护城河不是模型，而是 52 个工具的 schema 设计和 12 条 pipeline 的组合空间。

短期看，这种开源系统不会撼动 Premiere，但它会激活一批"轻量级创作 SaaS"开发者，把视频从"手工艺术"推向"提示工程"。是今日最值得收藏的 repo。

---

### 🥈 [google-labs-code/design.md](https://github.com/google-labs-code/design.md) — +1,407⭐

**Google 用一份 Markdown 规范把"视觉身份"喂给 coding agent**

`design.md` 是 Google Labs 提出的一种文本格式：用结构化的 Markdown 描述品牌的颜色、字体、间距、组件规则等。目的是让 Claude Code、Codex、Cursor 这类 coding agent 在生成前端代码时**自动遵守视觉一致性**，而无需开发者反复在 prompt 里写"主色 #1a73e8、字体 Inter"。

这是一个非常 Google 风格的"先建立标准、再做工具"动作。看起来简单，但实际上把"设计系统"从"组件库"层下沉到了"agent 可消费的元规范"层。值得对比的是 Figma 的 Dev Mode 和 Anthropic 的 Skills——它们都在解决"如何让 AI 一次性产生符合公司视觉规范的代码"。

当今天的 LLM 已经能写大段前端，最大瓶颈反而是**"风格收口"**。`design.md` 是这一瓶颈的 Schema 级答案，今天上榜不意外。预测下一步：Vercel / Tailwind 会推出自己的"标记"扩展，Figma 也很可能官方支持导出 design.md。

---

### 🥉 [apple/container](https://github.com/apple/container) — +1,366⭐

**Apple 持续输血"Mac 上的 Linux 容器"，Docker Desktop 的护城河又少一寸**

Apple 官方的 `container` 项目自 2025 年底开源以来，每月都会因为新增功能再上一次 trending。今天的爆发与最新版引入"GPU 直通"和"VFIO 透传 USB"有关——这让 Mac 上跑 ML 训练镜像和硬件 IoT 镜像第一次有了原生体验。

战略上看，Apple 在用 `container` 做两件事：（1）把 Docker Desktop 在 Mac 上的付费墙逐步瓦解；（2）让 macOS 成为"AI 工程师工作机"的事实标准——一台 MacBook Pro M5 + container 就可以同时跑 K8s 集群和本地推理模型。和今天 Apple 全线涨价新闻并读，这是苹果同时举的"加价 + 开源吸量"组合拳。

技术细节上：`container` 不是 Docker 兼容层，而是直接复用了 Apple Virtualization Framework，启动开销已经追平 Linux 上的原生 containerd。开发者社区给出的反馈是"OrbStack 之外终于有了官方选项"。

---

### 🛡️ [mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) — +600⭐

**817 条对齐 MITRE / NIST / D3FEND 的"AI agent 安全技能库"**

仓库结构是把 817 条网络安全任务封装成 Anthropic Skill 格式，覆盖侦察、横移、提权、缓解、合规等全周期，并明确对齐了 MITRE ATT&CK、NIST CSF、D3FEND 三大框架。其爆红时机非常微妙——OpenAI 同周刚发布 GPT-5.5-Cyber 并采取"窄分发"策略，把网络安全模型限制在 9 家可信厂商。

社区给出的潜台词是清晰的：**"既然官方模型对个人封锁了，那我们用开源 Skill + 开源模型自建"**。这是过去两个季度"Skill 化运动"（把能力包装成可直接被 Claude / Codex 调用的 schema）在安全垂直的代表性输出。对中小安全团队来说，把这 817 条直接挂到 Claude Code 上，等于一夜之间获得一支自动化红蓝队助手。

---

### 📈 [xbtlin/ai-berkshire](https://github.com/xbtlin/ai-berkshire) — +201⭐

**"Buffett 哲学 + Claude 多 agent 对抗"成为投资研究新框架**

ai-berkshire 把价值投资的核心步骤（行业判断、护城河识别、估值、风险）拆成多个相互对抗的 agent：bull、bear、devil's advocate、moat scout、long-tail risk—— 每个 agent 独立给出意见后由 judge 综合。整体逻辑接近 Anthropic 多 agent 论坛模式（Constitutional AI + Debate）。

它今天上榜揭示了一个有趣信号：**"AI 投资研究"不再走"扔大堆财报让 LLM 总结"老路，而开始走"对抗式多 agent"路径**。这与上周 Polymarket 等预测市场社区讨论 LLM agent 自主下注的趋势遥相呼应。对个人投资者来说，这是一个比 ChatGPT 写 SWOT 高一档的工具样本。

如果说 OpenMontage 代表创作工具被 agent 重写，那 ai-berkshire 代表的就是金融研究被 agent 重写。两条曲线都指向同一个方向：**单 agent → 多 agent 协作编排**。

---

## 生态观察

**今天 GitHub trending 的 15 个仓库中有 8 个直接以 Claude Code / agent / Anthropic Skill 为关键词，比例超过 50%**——这是 2026 上半年最高的"agentic 集中度"之一。从 Garry Tan 的 `gstack`（116K⭐）、Claude Code best practice 长青榜、AWS 官方 MCP 套件，到 OpenMontage 这种垂直爆款，都在说明同一件事：

**"框架/库"时代正在被"Skill/Workflow"时代取代**。开发者关心的不再是"用什么库写代码"，而是"我的 agent 该装哪 50 条 Skill、按哪 12 条 pipeline 编排"。

另外两条值得注意的副线：（1）**自托管 SaaS 替代品**继续走强（open-seo 替代 Semrush、TREK 替代 TripIt、CasaOS 替代 NAS 商业方案），说明在通胀 + 订阅疲劳 + AI 自动化部署的三重因素下，"自己跑一个"的可行性正在快速上升；（2）**Apple 生态的开发者动能在抬升**（`apple/container` 持续上榜），M 系列芯片 + macOS 容器化的体验已经接近 Linux 工作站。

值得跟踪的下一波趋势：能否出现一个开源的"AI 视频代理 + design.md + Skill 库"的全栈组合？OpenMontage 已经走到一半。
