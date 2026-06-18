# GitHub Trending 每日精选 · 2026-06-19

## 今日焦点

> **国产开源模型 GLM-5 登场 · Agent 基础设施大爆发 · 时间序列基础模型 · MCP 工具链下沉**
>
> - `zai-org/GLM-5` 智谱开源 744B/40B-active MoE，开源模型在 Vending Bench 2 上首次拿下榜首
> - `obra/superpowers` 把"agent skills"做成强制工作流，单日 +1,435⭐，agent 编程方法论再加新流派
> - `DeusData/codebase-memory-mcp` 单日 +2,308⭐，Tree-sitter + LSP + SQLite 给 agent 装上 codebase 长期记忆
> - `google-research/timesfm` TimesFM 2.5 把时间序列基础模型砍到 200M 参数 / 16k context，单日 +858⭐
> - `Kilo-Org/kilocode` 全平台 agentic IDE，500+ 模型零加价中转，正面挤压 Cursor 商业模式

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [google-research/timesfm](https://github.com/google-research/timesfm) | 时间序列预测基础模型，2.5 版砍到 200M | Python | 23,065 | +858⭐ | 2,210 |
| 2 | [n0-computer/iroh](https://github.com/n0-computer/iroh) | 用拨号 key 代替 IP，Rust 模块化网络栈 | Rust | 9,994 | +369⭐ | 461 |
| 3 | [freeCodeCamp/freeCodeCamp](https://github.com/freeCodeCamp/freeCodeCamp) | freeCodeCamp 开源课程 | TypeScript | 449,522 | +417⭐ | 45,125 |
| 4 | [obra/superpowers](https://github.com/obra/superpowers) | 强制工作流的 agentic skills 框架 | Shell | 232,356 | +1,435⭐ | 20,638 |
| 5 | [zai-org/GLM-5](https://github.com/zai-org/GLM-5) | 智谱 GLM-5: 744B/40B-active MoE | — | 4,091 | +286⭐ | 428 |
| 6 | [DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) | 158 语言代码知识图谱 MCP | C | 6,956 | +2,308⭐ | 563 |
| 7 | [yifanfeng97/Hyper-Extract](https://github.com/yifanfeng97/Hyper-Extract) | LLM + 超图把非结构化文本变知识 | Python | 1,733 | +124⭐ | 199 |
| 8 | [alibaba/zvec](https://github.com/alibaba/zvec) | 阿里轻量级进程内向量数据库 | C++ | 11,197 | +344⭐ | 648 |
| 9 | [withastro/flue](https://github.com/withastro/flue) | Astro 团队出的 sandbox agent 框架 | TypeScript | 5,474 | +164⭐ | 298 |
| 10 | [Kilo-Org/kilocode](https://github.com/Kilo-Org/kilocode) | 全平台 agentic 编程平台 | TypeScript | 22,063 | +1,339⭐ | 2,703 |
| 11 | [makeplane/plane](https://github.com/makeplane/plane) | 开源 Jira 替代 | TypeScript | 51,802 | +610⭐ | 4,599 |
| 12 | [Kong/insomnia](https://github.com/Kong/insomnia) | 开源跨平台 API 客户端 | TypeScript | 38,654 | +13⭐ | 2,289 |
| 13 | [Universal-Debloater-Alliance/universal-android-debloater-next-generation](https://github.com/Universal-Debloater-Alliance/universal-android-debloater-next-generation) | ADB 跨平台 Android 去膨胀 GUI | Rust | 7,906 | +247⭐ | 338 |
| 14 | [dotnet/aspnetcore](https://github.com/dotnet/aspnetcore) | .NET 跨平台 Web 框架 | C# | 38,091 | +22⭐ | 10,708 |
| 15 | [owainlewis/awesome-artificial-intelligence](https://github.com/owainlewis/awesome-artificial-intelligence) | AI 课程 / 书 / 论文清单 | — | 14,360 | +33⭐ | 2,333 |

---

## 重点项目点评

### 🥇 [DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) — 今日榜首，+2,308⭐

**给 agent 装一颗"长期记忆"，不要再 grep 第 100 次**

这个项目是这周 MCP 生态最直接命中痛点的作品。它不是又一个 LLM，而是一个**结构化分析后端**：用 Tree-sitter 解析 158 种语言、混合 LSP 做语义类型解析、SQLite + 内存索引、文件级 watcher 自动同步。Agent 不再每次 prompt 都重新读一遍仓库，而是用 Cypher-like 查询直接拿调用图、死代码、社区聚类、Git diff 影响面。

性能数据相当激进：Linux 内核 28M LOC 三分钟索引完，查询亚毫秒级，号称比"逐文件搜"省 99.2% token。安装一行脚本自动识别 11 种 agent（Claude Code、Codex、Gemini CLI、Zed…）写好 MCP 配置和 hook。

这条赛道的意义在于：今天的 agent 编程瓶颈已经从"模型不够聪明"变成"模型每次都得重新理解你的代码库"。code memory + MCP 这种组合，未来 6 个月会从今天的"小众工具"变成 IDE 默认配置。

---

### 🥈 [obra/superpowers](https://github.com/obra/superpowers) — +1,435⭐

**把"agent skills"做成强制工作流，而不是建议**

Jesse Vincent（Prime Radiant 创始人）做的 Superpowers 提出了一个明确的方法论假设：当前 agent 之所以不可靠，是因为开发者把 "skill" 当成"建议"，而 agent 经常跳过它们。Superpowers 反过来——把 brainstorming、需求澄清、计划制定、TDD（RED-GREEN-REFACTOR）、code review、git worktree 并行开发**做成强制工作流**，agent 必须按部就班走完。

支持 Claude Code、Cursor、GitHub Copilot 等多平台，MIT 许可。从 232k stars 的存量看，这个仓库已经早就在累积关注度，今天 +1,435 是版本节点带来的二次爆发。

它代表了 agent 编程的一种"反直觉"流派：不是让 agent 更自由，而是把它框死在最佳实践流程里。如果你最近抱怨 Claude Code / Codex 还是会"乱想"，这套强制 workflow 值得抄一下。

---

### 🥉 [zai-org/GLM-5](https://github.com/zai-org/GLM-5) — +286⭐

**国产开源大模型再上台阶，对标前沿闭源模型**

智谱 GLM-5（GLM-5.2 是当前最新）：**744B 总参数 / 40B active MoE**，从 GLM-4.5 的 355B/32B 跳上来一个量级；训练数据 28.5T tokens；引入 DeepSeek Sparse Attention (DSA) 降部署成本；后训练用自研的异步 RL 框架 "slime"。

关键指标：Vending Bench 2（长程经营能力）开源模型里**排第一**，在内部 CC-Bench-V2（前端 / 后端 / 长程任务）显著超过 GLM-4.7，与前沿闭源模型在 reasoning / coding / agentic 上"缩小差距"。BF16 和 FP8 双精度在 HuggingFace、ModelScope 同步开放。

放在今天的全局新闻里看：Claude Fable 5 / Mythos 5 被美国出口管制下架，国内开源前沿模型的战略地位再次被抬高。GLM-5 这个时间点开源，是非常清晰的"国产替代窗口期"信号。

---

### 🎯 [google-research/timesfm](https://github.com/google-research/timesfm) — +858⭐

**时间序列预测的"基础模型"路线在 2026 跑通了**

TimesFM 2.5 是 Google Research 时序基础模型的最新一代：**参数从 500M 砍到 200M、上下文从 2048 拉到 16k**——典型的"更小但更强"路径。架构是 decoder-only，已经被集成进 BigQuery ML、Google Sheets、Vertex Model Garden。

时间序列预测在过去一年是被 LLM 浪潮长期掩盖的领域，但今年从 Amazon Chronos、TimeGPT 到 TimesFM 2.5，"无需为每个数据集单独训练"的零样本预测路线正在成熟。对金融、能源、制造业的 demand forecasting 团队是个明显的工具栈刷新信号。

仓库新增了 Flax 推理、LoRA fine-tuning（HuggingFace Transformers），以及通过 XReg 引入协变量——把这个模型从"演示"变成了真正可用于生产 forecasting pipeline 的工具。

---

### 💡 [Kilo-Org/kilocode](https://github.com/Kilo-Org/kilocode) — +1,339⭐

**Cursor 的"开源 + 零加价"对手出现了**

Kilo Code 是个**多 IDE 全平台 agentic 编程平台**：支持 VS Code、JetBrains、CLI，500+ 模型可中途切换，**provider 原价、零加价**（这是直接挑衅 Cursor 抽佣模式），有专门的 Plan / Ask / Debug / Review 子 agent，CI/CD 里可以 `kilo run --auto` 全自动。

这条赛道今天最大的新闻是 Claude Code、Cursor、Windsurf 都把价格从订阅升级到"按 token 转手加价"。Kilo Code 的杀手锏就是把"我不收你中转加价"写进官网首屏——开源 + 不抽佣 + 多 IDE 兼容是它跟 Cursor 切割市场的三板斧。

22k stars 已经是个不小的体量，433 个 releases 显示迭代速度极快。对自己 hosting 模型 / 用 OpenRouter / 不想被锁在单一编辑器的团队来说，是 Cursor 之外最值得评估的开源替代。

---

## 生态观察

今天 GitHub trending 的主线非常一致：**Agent 工具链全栈下沉**。

- **记忆层**：codebase-memory-mcp（+2,308⭐）抓住了 agent 没有 codebase 长期记忆这个核心痛点；
- **方法论层**：Superpowers（+1,435⭐）把 skill 从"建议"做成"强制 workflow"；
- **IDE 层**：Kilo Code（+1,339⭐）以"开源 + 不抽佣 + 多 IDE"切 Cursor 的市场；
- **模型层**：GLM-5（+286⭐）让中国侧开源前沿模型再升一档，恰逢美国出口管制让 Claude Fable 5 下架。

另一条暗线是**时间序列与垂类基础模型**：TimesFM 2.5、Hyper-Extract（LLM + 超图把非结构化文本变成知识图）、alibaba/zvec（轻量级 in-process 向量库）——这些都不是聊天 chatbot，而是把 AI 嵌进数据管道的工程化工具。这一类工具未来半年的增速可能会超过通用 chatbot 上层应用。

如果只挑一个今天必看的仓库，是 codebase-memory-mcp——它代表了 agent 编程从"会写代码"到"长期理解你的代码库"的范式跳跃，所有做 IDE / coding agent 的团队都需要把它放进路线图。
