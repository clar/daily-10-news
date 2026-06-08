# GitHub Trending 每日速览 · 2026-06-09

## 今日焦点

> **Claude Code Skill 生态爆发 · 多平台 Agent 检索 · 向量索引内存革命 · 求职/PM 工种 AI 自动化 · 中国教科书数据集**
>
> - `mvanhorn/last30days-skill` 跨 8 大平台的 AI 研究 Agent，单日 +3,558⭐ 登顶
> - `RyanCodrai/turbovec` Rust 写的 TurboQuant 向量索引，10M 文档 31GB → 4GB，+1,730⭐
> - `roboflow/supervision` 计算机视觉工具链，+1,140⭐ 验证 CV 老牌仓库仍在加速
> - `Panniantong/Agent-Reach` "给 Agent 眼睛"，跨平台搜索 +796⭐
> - `santifer/career-ops` Claude Code 求职指挥中心，14 模式，+477⭐

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 跨 Reddit/X/YouTube/HN/Polymarket 的研究 Agent | Python | 34,366 | +3,558⭐ | 2,812 |
| 2 | [RyanCodrai/turbovec](https://github.com/RyanCodrai/turbovec) | Rust 实现的 TurboQuant 向量索引 | Python | 8,746 | +1,730⭐ | 808 |
| 3 | [roboflow/supervision](https://github.com/roboflow/supervision) | 可复用计算机视觉工具库 | Python | 42,309 | +1,140⭐ | 3,781 |
| 4 | [Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach) | 让 Agent 读懂全网内容的"眼睛" | Python | 24,027 | +796⭐ | 2,027 |
| 5 | [refactoringhq/tolaria](https://github.com/refactoringhq/tolaria) | Markdown 知识库桌面应用 | TypeScript | 13,533 | +649⭐ | 951 |
| 6 | [TapXWorld/ChinaTextbook](https://github.com/TapXWorld/ChinaTextbook) | 中国教科书全套数字化 | Roff | 72,954 | +593⭐ | 16,330 |
| 7 | [google/skills](https://github.com/google/skills) | Google 官方 Agent Skill 集合 | Python | 12,350 | +481⭐ | 967 |
| 8 | [santifer/career-ops](https://github.com/santifer/career-ops) | Claude Code 求职指挥中心 | JavaScript | 50,448 | +477⭐ | 10,332 |
| 9 | [CopilotKit/CopilotKit](https://github.com/CopilotKit/CopilotKit) | 面向 Agent 的前端生成式 UI | TypeScript | 34,102 | +398⭐ | 4,303 |
| 10 | [luongnv89/claude-howto](https://github.com/luongnv89/claude-howto) | Claude Code 图文教程 + 模板 | Python | 35,732 | +393⭐ | 4,343 |
| 11 | [openai/plugins](https://github.com/openai/plugins) | OpenAI Plugins 官方仓库 | JavaScript | 2,302 | +296⭐ | 289 |
| 12 | [MemPalace/mempalace](https://github.com/MemPalace/mempalace) | 开源 AI 记忆系统 | Python | 54,896 | +237⭐ | 7,159 |
| 13 | [danielmiessler/Personal_AI_Infrastructure](https://github.com/danielmiessler/Personal_AI_Infrastructure) | 个人 AI 基建框架 | TypeScript | 15,396 | +121⭐ | 2,158 |
| 14 | [phuryn/pm-skills](https://github.com/phuryn/pm-skills) | PM 工作流 100+ Agent Skills 商店 | Mixed | 12,611 | +112⭐ | 1,494 |
| 15 | [Andyyyy64/whichllm](https://github.com/Andyyyy64/whichllm) | 检测本机能跑的最佳本地 LLM | Python | 3,412 | +103⭐ | 201 |

---

## 重点项目点评

### 🥇 [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) — 今日榜首，+3,558⭐

**"AI Agent 主导的全网搜索引擎"，HN/Reddit/Polymarket 全连通**

这个仓库以 Claude Code Skill 为主要分发形式（但兼容 Cursor、Gemini CLI 等 50+ Agent 平台），目标是把"跨平台研究"做成一个 30 秒可调用的标准动作。核心流程是：先做 entity resolution（识别相关的 X handle、subreddit、GitHub 仓库），然后并发抓取 8 个平台的全文（YouTube 字幕、Reddit 评论投票、TikTok 描述、Polymarket 赔率）做语义聚合，最后用 LLM judge 按"社交相关性"排序输出。

它的关键差异化是**"用真实参与度排序，而不是编辑权重"**——HN 和 Polymarket 数据接入意味着研究结果会被"金钱投票"和"硬核工程师讨论"过滤一遍。这种"以社交信号为权威"的设计正是 2026 年信息检索的新范式：传统 PageRank 已经被 SEO 杀死，新一代 Agent 不再相信网页排名，转而相信"谁愿意为这个话题付钱/吵架"。

3,558 颗星单日增长是今年 6 月最高的 Skill 类项目纪录，反映 Claude Code Skill 生态的临界点已经到来。

---

### 🥈 [RyanCodrai/turbovec](https://github.com/RyanCodrai/turbovec) — +1,730⭐

**Google Research 的 TurboQuant 算法终于有了能打的开源实现**

turbovec 把"10M 文档 31GB 内存"压缩到 **4GB**，同时搜索速度还超过 FAISS——尤其在 ARM 架构上领先 12-20%。关键论据是 TurboQuant 的理论保证（量化失真匹配 Shannon 下界）+ 工程上的 SIMD 优化 + filter-aware 检索。

为什么 RAG 圈炸了：1) M 系列 Mac 用户终于能本机跑大规模检索；2) 不需要 train phase，直接在线 ingest 增量数据，对生产环境友好；3) 2-bit 量化让"私有部署 + 全索引常驻内存"在小内存机器上变得可行。LangChain、LlamaIndex、Haystack 都已经做了 adapter。

这是一个非常典型的"Rust+Python binding"项目结构，跟去年 Quantize-AI 走 GGUF 路线相比，turbovec 把"端侧 RAG"和"私有 enterprise RAG"两个市场同时切了一刀。

---

### 🥉 [Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach) — +796⭐

**"给 AI Agent 装上互联网视网膜"——但路线和 last30days-skill 完全不同**

last30days-skill 是 SaaS-skill 化的研究 Agent，Agent-Reach 则走 self-hosted 路线：用户在自己服务器跑一整套"看 Twitter / Reddit / YouTube"的 connector，输出标准化 schema 给上游 LLM。在 last30days-skill 和 google/skills 抢去 Skill 生态注意力的同时，Agent-Reach 把市场切给"自托管 + 可控数据流"的开发者。

值得注意的是它和 CopilotKit、Personal_AI_Infrastructure 在 trending 中同时出现——这三者覆盖了"前端 Agent UI / 后端 Agent infra / 数据感知层"的整套个人 AI 栈。三个不同方向同时火，说明社区在 2026 年中已经开始**自己搭建"独立 LLM Stack"**，绕开大厂的封闭 Agent 平台。

---

### 🎯 No.4 · [santifer/career-ops](https://github.com/santifer/career-ops) — +477⭐

**Claude Code 把求职流程做成了 14 个命令**

这是 Skill 生态成熟期最有意思的应用范例：用 Claude Code + Playwright 把求职从"打开 LinkedIn 手动找"变成 14 个标准化 mode：portal scan、offer scoring、CV 生成、ATS 优化、批量申请、interview prep、LinkedIn 触达。它兼容 Claude、Gemini、OpenCode 三种底层模型。

关键设计是 **human-in-the-loop**：AI 永远只做推荐，最终决定保留给用户。这种"完全自动化以外的克制"才是当前 Agent 产品差异化的核心——市场上已经厌倦了"全自动应聘"的失控感。

它和 phuryn/pm-skills 一起，验证了 Claude Code Skill 正在被"垂直工种"快速吃掉：PM、求职者、研究员、医生、律师都开始把自己的工作流写成 Skill 包。

---

### 🛠️ No.5 · [google/skills](https://github.com/google/skills) — +481⭐

**Google 官方下场做 Agent Skills，是 Anthropic Skill 生态的最大变量**

Google 把官方的 Agent Skills 仓库公开放上来，提供针对 Google Cloud、Workspace、Gemini API 的标准化 skill 模板。这是一个非常清晰的"生态卡位"动作：Anthropic 的 Claude Skill 格式已经成事实标准，Google 的策略不是另起炉灶，而是**直接做兼容版本，把 Gemini 接入相同的协议层**。

这对 Skill 开发者是利好（一份代码两家都能跑），但对 Anthropic 而言是隐忧：Skill 是 Claude Code 当前最强的 lock-in，如果 Google 持续投入兼容版本，最后会变成"协议层 commoditized，模型层正面竞争"。

---

## 生态观察

**主题一：Claude Code Skills 已是事实标准。** Top 15 里有 6 个项目（last30days-skill、google/skills、career-ops、claude-howto、pm-skills、Personal_AI_Infrastructure）直接面向 Claude Code Skill 协议。google/skills 的出现证明协议层正在标准化，Anthropic 的先发优势开始转化为 Skill 软件生态护城河——但同时也意味着模型本身的可替换性在变高。

**主题二：RAG/检索栈进入"端侧革命"。** turbovec 的 4GB / 10M 文档 + 超 FAISS 速度，叠加 whichllm 的"本机 LLM 选型"工具，开发者社区开始把整套 LLM + 检索栈搬到本地。这背后是云端 token 价格上涨 + 隐私合规收紧的双重推力。

**主题三：Agent 不再做"通用助手"，而是切垂直工种。** career-ops 切求职、pm-skills 切产品经理、Agent-Reach 切社媒研究、CopilotKit 切前端 Generative UI。"通用 ChatGPT"的下游已经被各种 Skill 包瓜分。

**主题四：经典工具仍有惊人韧性。** roboflow/supervision（CV 工具链）单日 +1,140⭐，证明非 LLM 类工程仓库依然在涨；中国教科书数据集（ChinaTextbook）+593⭐ 也反映训练数据需求的长期热度。AI 不是唯一变量。
