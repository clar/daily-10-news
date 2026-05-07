# GitHub Trending 日报 · 2026-05-08

## 今日焦点

> **Anthropic 入场金融 · DeepSeek 终端 Agent · Skills 生态成熟 · Vectorless RAG · 推理加速**
>
> - `anthropics/financial-services` Anthropic 官方放出金融服务工具集，单日 +1,367⭐
> - `Hmbown/DeepSeek-TUI` Rust 编写的 DeepSeek 终端 coding agent 一夜爆红，+5,787⭐
> - `addyosmani/agent-skills` "AI Coding Agent 工程化 Skill 库"持续霸榜，+3,058⭐
> - `VectifyAI/PageIndex` 反向操作——不用向量也能做 RAG，文档索引推理范式继续升温
> - `z-lab/dflash` Block Diffusion + Flash Speculative Decoding，推理侧学术工程双热

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [anthropics/financial-services](https://github.com/anthropics/financial-services) | Financial services tools and resources | Python | 11,259 | +1,367⭐ | 1,465 |
| 2 | [Hmbown/DeepSeek-TUI](https://github.com/Hmbown/DeepSeek-TUI) | Coding agent for DeepSeek models that runs in your terminal | Rust | 18,460 | +5,787⭐ | 1,395 |
| 3 | [z-lab/dflash](https://github.com/z-lab/dflash) | DFlash: Block Diffusion for Flash Speculative Decoding | Python | 3,433 | +654⭐ | 243 |
| 4 | [InsForge/InsForge](https://github.com/InsForge/InsForge) | Postgres backend with auth/storage/AI gateway, built for coding agents | TypeScript | 8,795 | +459⭐ | 728 |
| 5 | [LearningCircuit/local-deep-research](https://github.com/LearningCircuit/local-deep-research) | Local deep research tool supporting multiple LLMs/search engines | Python | 6,163 | +564⭐ | 544 |
| 6 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | Production-grade engineering skills for AI coding agents | Shell | 32,741 | +3,058⭐ | 3,792 |
| 7 | [VectifyAI/PageIndex](https://github.com/VectifyAI/PageIndex) | 📑 PageIndex: Document Index for Vectorless, Reasoning-based RAG | Python | 29,459 | +953⭐ | 2,486 |
| 8 | [vercel-labs/open-agents](https://github.com/vercel-labs/open-agents) | An open source template for building cloud agents | TypeScript | 4,999 | +160⭐ | 631 |
| 9 | [docusealco/docuseal](https://github.com/docusealco/docuseal) | Open source DocuSign alternative | Ruby | 15,516 | +899⭐ | 1,403 |
| 10 | [decolua/9router](https://github.com/decolua/9router) | Unlimited free AI coding connector with multi-provider auto-fallback | JavaScript | 4,425 | +249⭐ | 971 |
| 11 | [PriorLabs/TabPFN](https://github.com/PriorLabs/TabPFN) | ⚡ Foundation Model for Tabular Data | Python | 6,756 | +233⭐ | 666 |
| 12 | [aaif-goose/goose](https://github.com/aaif-goose/goose) | Open source extensible AI agent — install/execute/edit/test with any LLM | Rust | 44,434 | +431⭐ | 4,549 |
| 13 | [Augani/openreel-video](https://github.com/Augani/openreel-video) | Browser-based video editor, open source CapCut alternative | TypeScript | 1,570 | +208⭐ | 242 |

---

## 重点项目点评

### 🥇 [Hmbown/DeepSeek-TUI](https://github.com/Hmbown/DeepSeek-TUI) — 今日榜首，+5,787⭐

**DeepSeek 进军终端，coding agent 战场再添 Rust 选手**

`DeepSeek-TUI` 一夜冲上 18K 星，是今日整个榜单单日增量最高的项目，相当于新一波 DeepSeek 浪潮在 coding agent 形态上的具象化。它用 Rust 写了一个跑在终端里的 DeepSeek 编码代理，定位上对标 Claude Code、Aider、Goose 这一档——但绑定了 DeepSeek 自家模型，强调本地化、低延迟、可脚本化。

它的爆发说明两件事：第一，"在终端里跑 agent"已经从 Claude Code 时代的尝鲜变成默认范式，新模型一发布社区就会自发生成对应的 TUI；第二，Rust 重新成为 agent 工具链的优选语言（goose 也是 Rust），与早期一窝蜂 TypeScript / Python 的格局明显不同——大家开始在意启动时间、内存占用和单二进制分发。

---

### 🥈 [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — +3,058⭐

**Skills 已经长成独立生态，工程化最佳实践开始下沉**

这个项目已经累积 32K 星，今日还能 +3,058，说明 Skills（Anthropic 在 Claude Code / Agent SDK 里推出的能力封装机制）正从"协议"演变成"运动"。仓库的定位是"production-grade engineering skills"——把代码审查、安全审查、API 设计、依赖管理这种公司级实践打包成可复用的 skill，供任何 coding agent 加载。

值得注意的是它的语言是 Shell——大量 skill 本质是命令组合 + 提示词约束，工程师写 skill 不再需要写代码，只需要写约定。这种"低门槛 + 高复用"的模式，让 skill 库的增长速度远超传统库/框架。今日热榜上同时出现 `anthropics/financial-services`，恰好印证了官方也在朝同一个方向推进。

---

### 🥉 [anthropics/financial-services](https://github.com/anthropics/financial-services) — +1,367⭐

**Anthropic 把 Claude 直接送进金融行业的工作流**

Anthropic 官方账号下的新仓库，主语言 Python，单日 +1,367⭐，11K 总星数说明它发布时间不长但势头猛。从 README 走向看，这是 Anthropic 为金融服务行业准备的工具/skill 集合——很可能涵盖估值、合规、报告生成、风险建模等场景的标准化封装。

意义在于战略层面：Anthropic 不再只发布通用模型/SDK，而是开始按垂直行业（先是金融）打包"能立刻用起来的 agent 资产"。这是从"卖工具"到"卖组合"的关键一步，也是和 OpenAI、Google 在企业市场短兵相接的信号。配合 Agent Skills 协议，"行业 skill 包"很可能成为下一年的主流分发形态。

---

### [VectifyAI/PageIndex](https://github.com/VectifyAI/PageIndex) — +953⭐

**Vectorless RAG：把文档当树读，而不是当向量切**

29K 总星说明这个项目早就被关注，今日继续 +953。它的核心反共识：传统 RAG = 切块 + embedding + 向量检索，PageIndex 反过来——不切块、不做 embedding，而是建一棵基于推理的文档索引树，让 LLM 在树上"翻页"找答案。

这个方向之所以再次升温，是因为长上下文模型（200K+）+ 强推理能力已经让"先精确定位再精读"比"先粗暴召回再 rerank"更划算。如果配合 Claude/GPT 的 prompt cache，每次查询的成本反而比向量库低。RAG 这个赛道在 2026 年正在从 vector store 之争转向"索引结构 + 推理调度"之争。

---

### [z-lab/dflash](https://github.com/z-lab/dflash) — +654⭐

**Block Diffusion 进入推理加速主战场**

dflash 把 block diffusion（块扩散）和 flash speculative decoding 拼到一起做推理加速，论文/工程一起放出来后单日 +654，对一个学术性较强的项目来说是高热度。它的卖点是：不再用传统的"小模型起草、大模型验证"的 speculative decoding，而是用扩散方式同时草拟一整块 token，再统一验证。

推理加速这条线在 2026 年特别拥挤——MTP、EAGLE、Medusa、各种 KV 优化已经卷过一轮。dflash 的出现说明社区开始往"完全不同的草拟方式"探索，扩散模型从图像/视频生成卷到 LLM token 草拟，是一个很有意思的跨界融合信号。

---

## 生态观察

- **AI Coding Agent 已彻底主导榜单**：今日 13 个项目里超过一半与 coding agent / AI 工程相关（DeepSeek-TUI、agent-skills、open-agents、9router、goose、InsForge），跨 Rust / TypeScript / Shell / JS 四种语言生态。
- **Skills 协议事实标准化**：Anthropic 官方仓库 + 社区 agent-skills 双爆，"skill 包"将很可能成为 2026 年下半年最主要的 AI 资产分发形态。
- **垂直行业 + AI 开始硬碰硬**：`anthropics/financial-services` 是关键信号，下一波看点是法律、医疗、教育的官方 skill 包。
- **推理侧学术热度回归**：dflash、TabPFN 同时上榜，说明大家在"模型能力封顶"的语境下重新关注效率、专用结构和小数据基础模型。
- **Rust 在 agent 工具链稳定崛起**：DeepSeek-TUI、goose 都是 Rust，这是一个值得长期跟踪的语言层趋势。
