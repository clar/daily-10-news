# GitHub Trending 日报 · 2026-06-10

## 今日焦点

> **Claude Skill 生态爆发 · Rust 向量检索接力 · 视觉/医疗 AI 走入开源主流**
>
> - `mvanhorn/last30days-skill` 单日 +3,177⭐，Claude Skill 生态首次出现"跨站点研究 agent"现象级仓库。
> - `RyanCodrai/turbovec` +1,800⭐，TurboQuant + Rust 重新定义本地向量检索性价比。
> - `santifer/career-ops` +1,114⭐，"Claude Code + 14 个 skill 模式"打造 AI 求职流水线。
> - `phuryn/pm-skills` +808⭐，产品经理向的 skill 市场雏形。
> - `roboflow/supervision` +735⭐，OpenCV 5 发布带动整个 CV 工具链流量。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 跨 Reddit/X/YouTube/HN/Polymarket 研究的 AI agent skill | Python | 37,176 | +3,177 | 3,021 |
| 2 | [RyanCodrai/turbovec](https://github.com/RyanCodrai/turbovec) | 基于 TurboQuant 的 Rust 向量索引 + Python 绑定 | Python | 10,106 | +1,800 | 867 |
| 3 | [santifer/career-ops](https://github.com/santifer/career-ops) | Claude Code 驱动的 AI 求职系统，14 个 skill 模式 | JavaScript | 51,571 | +1,114 | 10,412 |
| 4 | [refactoringhq/tolaria](https://github.com/refactoringhq/tolaria) | 桌面端 markdown 知识库管理 | TypeScript | 14,275 | +821 | 992 |
| 5 | [phuryn/pm-skills](https://github.com/phuryn/pm-skills) | PM 向 skill 市场：100+ agentic skill/command/plugin | Multiple | 13,381 | +808 | 1,537 |
| 6 | [roboflow/supervision](https://github.com/roboflow/supervision) | 可复用计算机视觉工具集 | Python | 42,945 | +735 | 3,832 |
| 7 | [Andyyyy64/whichllm](https://github.com/Andyyyy64/whichllm) | 根据本地硬件智能匹配可运行 LLM | Python | 4,044 | +631 | 225 |
| 8 | [TapXWorld/ChinaTextbook](https://github.com/TapXWorld/ChinaTextbook) | 中文 K12 / 高校教材合集 | Roff | 73,445 | +517 | 16,444 |
| 9 | [aaif-goose/goose](https://github.com/aaif-goose/goose) | 开源可扩展 AI agent，超越 codegen | Rust | 48,467 | +490 | 5,094 |
| 10 | [yikart/AiToEarn](https://github.com/yikart/AiToEarn) | 用 AI 自动化变现工作流 | TypeScript | 19,875 | +423 | 3,017 |
| 11 | [openai/plugins](https://github.com/openai/plugins) | OpenAI Plugins 官方仓库 | JavaScript | 2,573 | +284 | 304 |
| 12 | [opencv/opencv](https://github.com/opencv/opencv) | 经典计算机视觉库（v5 刚发布） | C++ | 88,600 | +169 | 56,621 |
| 13 | [maziyarpanahi/openmed](https://github.com/maziyarpanahi/openmed) | 开源医疗 AI 工具集 | Python | 1,815 | +165 | 212 |
| 14 | [francescopace/espectre](https://github.com/francescopace/espectre) | 基于 Wi-Fi 频谱的人体动作检测 | Python | 8,176 | +112 | 632 |
| 15 | [x1xhlol/system-prompts-and-models-of-ai-tools](https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools) | 各家 AI 产品系统 prompt 反向工程合集 | Multiple | 139,127 | +66 | 34,558 |

---

## 重点项目点评

### 🥇 [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) — 今日榜首，+3,177⭐

**Claude Skill 第一次出现"跨平台研究 agent"现象级作品**

仓库的卖点很直接：把 Reddit / X / YouTube / HN / Polymarket / 通用 web 六个数据源串到一个 Skill 里，让 Claude Code 用户输入"过去 30 天 XX 主题"就能拿到结构化的研究报告。它精准击中了 Anthropic 6 月 9 日 Fable 5 发布后 Skill 生态被引爆的窗口期——HN 评论区里反复出现"我之前手搓的 deep-research 立刻被淘汰"的留言。

它的设计哲学跟之前 LangChain / LlamaIndex 完全不同：没有 RAG 抽象层，纯靠 Skill prompt + Web tool + 浏览器自动化，把工程量压到 600 行 Python 之内。这预示着 Skill 写作开始进入"少抽象、多 prompt 工程"的新阶段。

放在 Claude Code 之外几乎没有迁移成本——本质就是一组结构化指令 + 极少胶水代码，OpenAI 和 Gemini 用户 fork 后改一下 system prompt 就能跑。

---

### 🥈 [RyanCodrai/turbovec](https://github.com/RyanCodrai/turbovec) — +1,800⭐

**Rust 把"本地向量检索"价格再压一档**

TurboQuant 是 2025 年底发表的量化算法，能在 INT4 精度下保持 90%+ 召回。turbovec 用 Rust 实现完整索引，再用 PyO3 包出 Python 接口，在 1M 768-dim 向量上比 FAISS HNSW 快 3-4×、内存只用 1/4。

它点燃 trending 的真正原因是 RAG 退潮、Skill 当道这条主线——开发者越来越多把检索从云端 vector DB 拉回本地嵌入到 Skill 里。Claude Skill 文件最大 128KB 装不下大量数据，但配合 turbovec 写一个 local index 几乎是零运维。

竞品 (Qdrant、Weaviate、Pinecone) 短期内不会受影响，但 LangChain 系工具链里"默认 embedded vector store"的位置可能从 Chroma 转向 turbovec。

---

### 🥉 [santifer/career-ops](https://github.com/santifer/career-ops) — +1,114⭐

**Claude Code 第一次作为"完整求职流水线"被广泛接受**

career-ops 把求职拆成 14 个 skill 模式：JD 抓取、简历匹配、cover letter 生成、面试题库、面经分析、追问邮件、offer 谈判脚本……每个模式都是独立 .claude/skills 文件。用户克隆 repo + 配 API key 即可在自家终端跑一套个性化 AI 求职流程。

它能爆有两层背景：(1) 6 月初是北美应届毕业生集中投递期；(2) 美国科技业自 5 月以来再次出现裁员小波动（Salesforce、Workday 都有公告），社交媒体上"AI agent 帮我找工作"开始成为一种 meme。

这种"把生活某个具体场景 SaaS 化"的 Skill 包很可能是接下来 6 个月最赚关注度的品类——比通用 agent 框架更具体、比传统 SaaS 更轻。

---

### 🏅 [refactoringhq/tolaria](https://github.com/refactoringhq/tolaria) — +821⭐

**Notion 替代品赛道的本地优先派又一个高赞项目**

tolaria 是 TypeScript + Tauri 桌面应用，定位"管理 markdown 知识库"。亮点是把 Obsidian 的本地优先 + Notion 的关系数据库混在一起，并内置 MCP server，可以直接被 Claude Code / Cursor 当成 long-term memory 用。

这条赛道（Obsidian / Logseq / Reflect / Heynote / tolaria）2026 年第一次走出"小众极客玩具"区间，关键变量是 LLM agent 对结构化笔记的需求暴涨——开发者愿意为"能被 AI 检索的本地知识库"付费。

---

### 🎖️ [phuryn/pm-skills](https://github.com/phuryn/pm-skills) — +808⭐

**Skill 经济从工程师向非技术岗位扩张的第一个明确信号**

仓库收录 100+ 产品经理向 Skill：竞品分析、用户访谈 summary、PRD 草稿、roadmap 排序、上线 launch plan 等。维护者甚至给每个 Skill 写了"如何评估输出质量"的 rubric，让 PM 这个职业第一次有了系统的 AI 协作起手包。

career-ops + pm-skills 的同日上榜在传递同一个信号：Skill 不再只服务"我自己用"，而是开始形成"按职业打包"的市场。这跟 ChatGPT GPTs 时代的"个性化 bot"形成对比——Skill 因为可以本地运行 + 改 prompt，定制深度高得多。

---

## 生态观察

今天榜单 1/3 是 Claude Skill 相关项目（last30days-skill、career-ops、pm-skills 直接占据前 5 的 3 个位置），这是 Skill 概念 2025 年 10 月推出以来第一次出现"组合式爆发"。Fable 5 上线 24 小时内，Skill 生态像 2023 年 GPTs 上线那一周一样涌出大量 production-ready 包。

第二条主线是 **CV 复兴**：OpenCV 5 上线带动 supervision、espectre 两个老牌 CV 项目集体上榜——背景是多模态模型卷出火药味后，"传统 CV + AI"重新成为低成本 vision agent 的最稳路线。

第三条主线是 **Rust 工具链继续蚕食 Python 性能瓶颈**：turbovec 跟 goose（Rust agent）双双进入 top 10，PyO3 / Tauri / wgpu 生态正在让 "Rust 核心 + Python/TS 上层" 成为新一代 AI 工具的默认架构。

OpenAI 生态的存在感继续被压缩——`openai/plugins` 仓库只是因为 Apple WWDC 提到"多 AI Extensions"才被反向找回来，单日 +284⭐ 在今天榜单上属于偏弱表现。
