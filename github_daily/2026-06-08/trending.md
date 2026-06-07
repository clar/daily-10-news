# GitHub Trending 日报 · 2026-06-08

## 今日焦点

> **Agent Skills 爆款日 · 向量检索新王 · Postgres 原生编排 · NotebookLM 开源化 · 开发者工具下沉到设计层**
>
> - `Leonxlnx/taste-skill` 一夜 +1,104⭐：用 Agent Skill 修正 AI UI"千篇一律"，正面回应 LLM 设计审美危机。
> - `NousResearch/hermes-agent` +1,117⭐：消费级 personal agent 持续吸金，已 18.5 万星。
> - `RyanCodrai/turbovec` +1,533⭐ 单日涨幅榜首：Rust + TurboQuant 把 1000 万向量塞进 4 GB 内存。
> - `mvanhorn/last30days-skill` +1,097⭐：跨 Reddit/X/YouTube/HN/Polymarket 的"30 天主题速览" agent skill。
> - `microsoft/pg_durable` +314⭐：把 durable execution 塞进 Postgres，干掉 Redis + 消息队列 + 工作流编排三件套。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [RyanCodrai/turbovec](https://github.com/RyanCodrai/turbovec) | Rust 向量索引，10M 向量 4 GB 装下 | Python | 7,047 | +1,533 | 690 |
| 2 | [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) | "陪你成长"的个人 AI agent | Python | 185,843 | +1,117 | 31,964 |
| 3 | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | 让 AI 生成的 UI 有"审美" | Shell | 36,498 | +1,104 | 2,639 |
| 4 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 跨平台 30 天话题研究 agent skill | Python | 30,722 | +1,097 | 2,573 |
| 5 | [lfnovo/open-notebook](https://github.com/lfnovo/open-notebook) | NotebookLM 开源替代 | TypeScript | 27,182 | +555 | 3,089 |
| 6 | [TapXWorld/ChinaTextbook](https://github.com/TapXWorld/ChinaTextbook) | 中国小初高大学教材 PDF 汇总 | Roff | 72,415 | +355 | 16,235 |
| 7 | [aaif-goose/goose](https://github.com/aaif-goose/goose) | 开源可扩展 AI agent | Rust | 47,445 | +338 | 5,005 |
| 8 | [microsoft/pg_durable](https://github.com/microsoft/pg_durable) | Postgres 原生 durable execution | Rust | 1,434 | +314 | 31 |
| 9 | [Crosstalk-Solutions/project-nomad](https://github.com/Crosstalk-Solutions/project-nomad) | 离线生存知识 + 本地 AI 计算机 | TypeScript | 29,679 | +304 | 2,939 |
| 10 | [openai/plugins](https://github.com/openai/plugins) | OpenAI 插件官方仓库 | JavaScript | 2,008 | +262 | 270 |
| 11 | [refactoringhq/tolaria](https://github.com/refactoringhq/tolaria) | Markdown 知识库桌面应用 | TypeScript | 12,822 | +242 | 906 |
| 12 | [ggml-org/llama.cpp](https://github.com/ggml-org/llama.cpp) | C/C++ 本地 LLM 推理基座 | C++ | 115,298 | +197 | 19,295 |
| 13 | [yikart/AiToEarn](https://github.com/yikart/AiToEarn) | "用 AI 挣钱"内容工具集 | TypeScript | 18,720 | +180 | 2,903 |
| 14 | [opencv/opencv](https://github.com/opencv/opencv) | 老牌计算机视觉库 | C++ | 88,051 | +89 | 56,597 |
| 15 | [HunxByts/GhostTrack](https://github.com/HunxByts/GhostTrack) | 手机号 / 位置追踪 OSINT 工具 | Python | 13,711 | +21 | 1,833 |

---

## 重点项目点评

### 🥇 [RyanCodrai/turbovec](https://github.com/RyanCodrai/turbovec) — 今日榜首，+1,533⭐

**用 TurboQuant 把"百万级 RAG 必须配集群"这条共识捅了一刀。**

turbovec 的卖点用一句话就能让所有做 RAG 的人停下来：1000 万文档向量原本要 31 GB float32，turbovec 压到 4 GB，且无需训练 codebook。它建立在 Google 去年发表的 TurboQuant（data-oblivious 量化）算法之上，配合 NEON / AVX-512 手写 SIMD kernel，在 ARM 上比 FAISS 快 12–20%。

它能一夜爬到 +1,533⭐ 的真实原因不是"又一个向量库"——而是 2026 年本地优先 + 隐私敏感的 RAG 场景已经成为新主流：local-first 写作工具、桌面 agent、企业内部知识库都在拒绝把向量丢到 Pinecone / Weaviate 的托管服务。turbovec 提供的 LangChain / LlamaIndex / Haystack / Agno 框架集成，意味着它一开始就奔着"FAISS 替代品"去定位的。

值得关注的工程信号是"no training phase"——以往 PQ/IVFPQ 系列需要先用代表性样本训练 codebook，对增量场景非常不友好；turbovec 让 add-as-you-go 成为默认行为，这才是它在 agent 时代被秒赞的关键。

---

### 🥈 [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) — +1,117⭐

**已经 18.5 万星仍单日 +1,117⭐，Hermes Agent 现在是消费级"私人 AI"的事实代名词。**

Hermes 的产品策略一贯偏哲学：他们不卖"高分基准"，卖"你的 agent 会跟你一起成长"。这一阶段更新把 long-term memory、人格留存、多设备同步整合进单一开源仓库，并且明确支持把 Claude / GPT / Llama 作为底层模型来回切——这种"自带身份、自由换大脑"的架构正中"反厂商锁定"的开发者下怀。

把它放到本周更大的背景里：Anthropic 秘密 IPO 估值 965 B、Apple WWDC 即将开放多模型 Extensions，"个人 AI"作为应用层 SKU 的窗口期刚刚打开。Hermes Agent 是这一波里唯一一个把"persona ownership"做成开源仓库主线的项目，所以它的星数还在加速。

---

### 🥉 [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) — +1,104⭐

**给 AI 写"审美"——这是对"LLM 生成 UI 全是模板"焦虑的正面回应。**

taste-skill 是一组写成 SKILL.md 的 Agent Skills，专门修正 Claude / Codex / Cursor 等 coding agent 在生成 React/Tailwind 界面时的"模板化倾向"。用户通过三个旋钮（DESIGN_VARIANCE、MOTION_INTENSITY、VISUAL_DENSITY）调整风格，并可在 soft / brutalist / minimalist 等子皮肤间切换。

它能炸榜的原因有两层：第一，它精准踩在 HN 今天头条"LLM 让我的工程能力贬值"那篇文章的情绪上——开发者不甘心被同质化，所以一个"教 AI 不要 slop"的工具立刻有共鸣；第二，它是 **Anthropic Agent Skills 体系生态扩散的标志性项目**，证明 SKILL.md 已经从 Anthropic 内部规范长成了一个跨 IDE、跨厂商的事实格式（项目主页里 Claude、Codex、Cursor 同时被列为目标）。

值得追踪：今天 trending 榜上 #3、#4 都是 SKILL 类项目（taste-skill / last30days-skill）。这是 Agent Skill 作为"AI 时代 npm 包"的第一周。

---

### 🏅 [microsoft/pg_durable](https://github.com/microsoft/pg_durable) — +314⭐

**Microsoft 把 Temporal 那一套塞进 Postgres——一次"反基础设施栈复杂化"的反击。**

pg_durable 解决的是一类被工程师诟病很久的问题：每个公司都在用 Redis 当 queue、用 Celery / Sidekiq / Temporal 当 orchestrator、再用 Postgres 当状态库——三层基础设施，配置成本与故障域都不可控。这个扩展把 durable execution 全部塞进 PG，函数定义、checkpoint、retry 全部在数据库内完成。

更值得关注的是它是 **Microsoft 自家 Azure HorizonDB 服务的开源副本**：意味着这不是社区玩具，而是产品级实现。配合 2026 年 Postgres 生态持续吞并周边（pgvector、pg_graphql、pg_cron），"Postgres 即应用平台"的叙事再添一块拼图。

只有 1,434 星却单日 +314 说明它刚发布、传播曲线刚开始；如果一周后能稳住增量，这会是今年最重要的 Postgres 扩展之一。

---

### 🎖️ [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) — +1,097⭐

**Agent Skill 不只是用来写代码——它正在成为"研究助手"的封装格式。**

last30days-skill 的工作流很直接：给它一个主题（比如"过去 30 天的 AI 监管"），它会跨 Reddit、X、YouTube、HN、Polymarket、Web 做 fan-out 检索，对来源做对抗式 verification，最后输出带引用的综合报告。这本质上是把"Deep Research"做成可以 npm-style 分发的 SKILL.md。

它与 #3 taste-skill 同日双双登顶印证了一个趋势：**Agent Skill 正在变成一种新的开源单元**，比 prompt 模板更结构化、比 SDK 更轻量。开发者不再 fork "应用"，而是 fork "skill 包"——这跟早期 npm / pip / HomeBrew 的传播曲线非常像。如果 Anthropic 在 WWDC 后跟进推出 Skill Registry，这会是今年最重要的开发者基础设施事件。

---

## 生态观察

今天 trending 的主轴非常清晰：**Agent Skills + 本地 RAG 基础设施 + Postgres 一切化**，三条线并行，且都跟 LLM 时代下"工程师如何重新拿回话语权"这一情绪相关：

- **Agent Skills 体系起飞**：taste-skill、last30days-skill 一日双榜，且都来自非大厂作者，是开源个人开发者第一次在 Anthropic 的格式规范上拿到流量奖励——这一周可以视作 SKILL.md 的"npm 时刻"；
- **本地优先 RAG 抬头**：turbovec 一夜 +1,533、open-notebook 持续涨、project-nomad 把"离线 AI + 知识库"打包成生存包，意味着用户对托管 vector DB 与云端 RAG 的耐心在结构性下降；
- **Postgres 吞噬一切**：pg_durable 让"workflow orchestrator 是不是该消失"重新成为议题；
- **传统 CV 框架在退潮**：OpenCV 仍在榜但仅 +89⭐ 已经远低于 agent 类项目，2026 年的 trending 几乎不再奖励"基础库维护"，只奖励"agent 时代新基础设施"。

唯一与 AI 无关、却仍能上榜的项目是 ChinaTextbook（教材 PDF 汇总）与 GhostTrack（OSINT）——前者是中国教育系统刚性需求，后者是周期性安全工具流量。它们的存在反向印证：今天的开发者注意力，99% 在 AI 应用层与基础设施层之间。
