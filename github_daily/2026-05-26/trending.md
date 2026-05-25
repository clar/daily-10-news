# GitHub Trending 每日热榜 · 2026-05-26

## 今日焦点

> **代码知识图谱崛起 · Agent Skills 生态爆发 · Claude Cowork 插件化 · 安全技能标准化**
>
> - `Lum1104/Understand-Anything` 把任意代码转成可交互知识图谱，今日 +5,625⭐ 登顶
> - `colbymchenry/codegraph` 预索引代码图谱省 token，本地化服务多家 Agent，+3,171⭐
> - `multica-ai/andrej-karpathy-skills` 一份 CLAUDE.md 提炼 Karpathy 编码心得，+2,753⭐
> - `anthropics/knowledge-work-plugins` 官方 Claude Cowork 插件库，+1,448⭐
> - `mukul975/Anthropic-Cybersecurity-Skills` 754 个安全技能映射五大框架，+999⭐

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [Lum1104/Understand-Anything](https://github.com/Lum1104/Understand-Anything) | 代码转交互式知识图谱 | TypeScript | 30,829 | +5,625 | 2,551 |
| 2 | [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) | Agent 用本地代码知识图谱 | TypeScript | 24,792 | +3,171 | 1,367 |
| 3 | [rohitg00/ai-engineering-from-scratch](https://github.com/rohitg00/ai-engineering-from-scratch) | 从零学 AI 工程 | Python | 18,385 | +3,167 | 3,132 |
| 4 | [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) | Karpathy 编码心得 CLAUDE.md | — | 154,803 | +2,753 | 15,860 |
| 5 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Agent harness 性能优化系统 | JavaScript | 192,244 | +2,052 | 29,761 |
| 6 | [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) | Claude Cowork 知识工作插件 | Python | 15,323 | +1,448 | 1,852 |
| 7 | [mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | 754 个安全 Agent 技能 | Python | 9,161 | +999 | 1,131 |
| 8 | [manaflow-ai/cmux](https://github.com/manaflow-ai/cmux) | AI 编码 Agent 的 macOS 终端 | Swift | 19,462 | +598 | 1,469 |
| 9 | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | 给 AI「品味」防生成水文 | Shell | 19,622 | +542 | 1,650 |
| 10 | [Fincept-Corporation/FinceptTerminal](https://github.com/Fincept-Corporation/FinceptTerminal) | 现代金融分析终端 | Python | 23,843 | +345 | 3,279 |
| 11 | [shiyu-coder/Kronos](https://github.com/shiyu-coder/Kronos) | 金融市场基础模型 | Python | 26,005 | +243 | 4,516 |
| 12 | [anthropics/claude-cookbooks](https://github.com/anthropics/claude-cookbooks) | Claude 使用范例集 | Jupyter | 43,989 | +218 | 5,045 |
| 13 | [paperless-ngx/paperless-ngx](https://github.com/paperless-ngx/paperless-ngx) | 自托管文档管理系统 | Python | 41,300 | +151 | 2,742 |
| 14 | [Axorax/awesome-free-apps](https://github.com/Axorax/awesome-free-apps) | 免费应用精选清单 | JavaScript | 4,456 | +141 | 228 |
| 15 | [moeru-ai/airi](https://github.com/moeru-ai/airi) | 自托管语音 AI 伴侣 | TypeScript | 39,681 | +32 | 4,021 |

---

## 重点项目点评

### 🥇 [Lum1104/Understand-Anything](https://github.com/Lum1104/Understand-Anything) — 今日榜首，+5,625⭐

**「能教会你的图」胜过「让你惊艳的图」**

这个项目的口号一针见血：graphs that teach > graphs that impress。它把任意代码库转成可交互的知识图谱，你可以在里面探索、搜索、提问。在 LLM 已经能读懂单文件的今天，开发者真正缺的是「整库级别的结构理解」——谁调用谁、模块如何耦合、改这里会牵动哪里。

它一天涨近 6000 星，说明痛点踩得极准：Agent 时代「让 AI 理解代码库」从锦上添花变成刚需。与第 2 名 codegraph 同属「代码图谱」赛道，两者一起冲榜，标志着这个细分方向正在从概念走向工具化爆发。

---

### 🥈 [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) — +3,171⭐

**预索引、省 token、100% 本地——Agent 工程的降本三件套**

codegraph 把代码库预先索引成知识图谱，供 Claude Code、Codex、Cursor、OpenCode、Hermes Agent 直接调用，主打「更少 token、更少工具调用、全本地」。它解决的是当下 Agent 编码最现实的成本痛点：每次让 Agent grep 一遍代码库都在烧 token 和上下文，预索引能把这部分开销前置、复用。

它能多家 Agent 通吃，恰恰反映了一个趋势——工具开始抽象在「具体 Agent」之上，开发者不想被某个 harness 锁死。本地化卖点也踩中企业对代码不出网的合规焦虑。

---

### 🥉 [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) — +2,753⭐

**一份 CLAUDE.md，把大神的「踩坑经验」变成可复用规则**

这个仓库把 Andrej Karpathy 关于 LLM 编码陷阱的观察，浓缩成一份能直接改善 Claude Code 行为的 CLAUDE.md。它今日大涨，时间点耐人寻味——正值 Karpathy 确认加盟 Anthropic、负责重建预训练研究的新闻发酵，社区的「Karpathy 信仰」直接转化成了星标。

更深一层，它代表了「skills/规则文件」这一品类的成熟：与其每次手把手纠正 Agent，不如把领域专家的隐性知识固化成配置。`taste-skill`（给 AI 品味防水文）、`Anthropic-Cybersecurity-Skills` 都是同一逻辑的不同切面。

---

### 4️⃣ [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) — +1,448⭐

**Claude 从「写代码」走向「干所有知识工作」**

Anthropic 官方开源的这套插件库，主要面向知识工作者在 Claude Cowork 中使用——不是给程序员的，而是给做文档、做分析、做研究的白领。它的上榜信号很强：Anthropic 正把 Claude 的主战场从「编码 Agent」扩展到「通用知识工作平台」。

结合今日热榜里大量 Claude Code/Skills 项目，可以看出一个清晰的平台战略：用开源插件+技能生态把开发者和知识工作者都吸进 Claude 生态，再用 Cowork 这样的产品收口。

---

### 5️⃣ [mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) — +999⭐

**754 个安全技能，映射五大框架——Agent 安全能力开始标准化**

这个仓库把 754 个结构化的网络安全技能映射到五个主流安全框架，专供 AI Agent 调用。它的走红说明，安全这个高门槛领域正在被「技能化」：把专家流程拆成可被 Agent 编排的标准单元。

这与本周 Anthropic 把新模型 Mythos 定位于网络安全应用的方向一致——AI + 安全是 2026 年最被看好的落地场景之一，而「技能库」就是连接通用模型与垂直专业能力的中间层。

---

## 生态观察

今天的 GitHub Trending 几乎被一个主题统治：**Agent 工程的工具化与标准化**。两条主线清晰可见——

一是**代码知识图谱**（Understand-Anything、codegraph 双双爆发）：当 Agent 编码成为常态，「让 AI 高效理解整个代码库」成了省 token、提准确率的关键基础设施，这个赛道正从论文走向产品。二是**Skills/规则文件生态**（karpathy-skills、taste-skill、cybersecurity-skills、knowledge-work-plugins）：社区找到了驯服 Agent 的最优解——把专家经验固化成可复用的技能与配置，而非每次重新调教。

值得注意的是 Anthropic 官方仓库（knowledge-work-plugins、claude-cookbooks）持续在榜，叠加海量第三方 Claude 工具，整个生态的引力中心明显在向 Claude 倾斜。金融类（FinceptTerminal、Kronos）和自托管工具（paperless-ngx、airi）则是稳定的长尾热度，未受 AI 主线挤压。
