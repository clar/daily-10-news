# GitHub Trending 日报 · 2026-06-21

## 今日焦点

> **AI Agent 配套基础设施全栈爆发 · MCP 生态走向工程化 · SQLite/Rust 新写法 · Claude Skills 标准库**
>
> - `chopratejas/headroom` 给 Agent 做 60-95% token 压缩，单日 +3,786⭐ 居涨幅榜首。
> - `tw93/Pake` 将网页一键转桌面应用，单日 +2,398⭐，总星突破 5.4 万。
> - `mattpocock/skills` Claude Skill 工程化集合，13.8 万⭐已成事实标准库。
> - `DeusData/codebase-memory-mcp` 给 Agent 喂"代码知识图谱"，把 41 万 token 探索压到 3.4k。
> - `palmier-io/palmier-pro` 首个"为 AI 而生"的 macOS 视频编辑器，AI 在时间线里直接生成/编辑。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [chopratejas/headroom](https://github.com/chopratejas/headroom) | Agent 上下文压缩，60-95% token 减少 | Python | 41,714 | +3,786 | 2,862 |
| 2 | [tw93/Pake](https://github.com/tw93/Pake) | 一行命令把网页打包成桌面应用 | Rust | 54,596 | +2,398 | 10,858 |
| 3 | [mattpocock/skills](https://github.com/mattpocock/skills) | Claude Code skills 工程化集合 | Shell | 138,134 | +1,360 | 11,987 |
| 4 | [DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) | 代码知识图谱 MCP server | C | 9,275 | +1,267 | 702 |
| 5 | [palmier-io/palmier-pro](https://github.com/palmier-io/palmier-pro) | 为 AI 而生的 macOS 视频编辑器 | Swift | 3,247 | +904 | 270 |
| 6 | [tursodatabase/turso](https://github.com/tursodatabase/turso) | Rust 重写的进程内 SQLite | Rust | 20,285 | +774 | 1,040 |
| 7 | [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) | 12 pipelines × 52 工具的视频 Agent | Python | 6,993 | +677 | 1,147 |
| 8 | [Kilo-Org/kilocode](https://github.com/Kilo-Org/kilocode) | Agent 工程一体化开发平台 | TypeScript | 23,321 | +470 | 2,740 |
| 9 | [google-research/timesfm](https://github.com/google-research/timesfm) | 时间序列基础模型（预训练） | Python | 24,502 | +432 | 2,322 |
| 10 | [penpot/penpot](https://github.com/penpot/penpot) | 开源设计/代码协作工具 | Clojure | 51,353 | +424 | 3,296 |
| 11 | [Kong/insomnia](https://github.com/Kong/insomnia) | REST/GraphQL/gRPC API 客户端 | TypeScript | 39,301 | +327 | 2,324 |
| 12 | [withastro/flue](https://github.com/withastro/flue) | Astro 团队的沙盒 Agent 框架 | TypeScript | 6,075 | +313 | 342 |
| 13 | [owainlewis/awesome-artificial-intelligence](https://github.com/owainlewis/awesome-artificial-intelligence) | AI 资源精选合集 | - | 14,756 | +223 | 2,354 |
| 14 | [twentyhq/twenty](https://github.com/twentyhq/twenty) | 为 AI 设计的开源 Salesforce | TypeScript | 50,832 | +140 | 7,413 |
| 15 | [jamiepine/voicebox](https://github.com/jamiepine/voicebox) | 开源 AI 声音工作室 | TypeScript | 30,983 | +140 | 3,833 |

---

## 重点项目点评

### 🥇 [chopratejas/headroom](https://github.com/chopratejas/headroom) — 今日榜首，+3,786⭐

**"Agent 时代的真正瓶颈不是模型，是上下文体积"**

Headroom 把自己定位成"在请求送进 LLM 之前的代理层"，把 tool outputs / logs / RAG chunk / 历史会话全部压缩，目标是 **60-95% token 减少而不影响回答质量**。底层是分类型的压缩流水线：JSON 走 `SmartCrusher`、代码走基于 AST 的 `CodeCompressor`（支持 Python/JS/Go/Rust/Java/C++）、自然语言走名为 `Kompress-base` 的 HuggingFace 模型，KV cache 用 `CacheAligner` 稳定前缀提高命中率。

最有意思的是 **CCR 可逆压缩**：本地保留原文，LLM 需要时按需取回——这意味着 agent 既享受短上下文的速度/成本优势，又不丢"完整事实"。三种部署模式（library / proxy / MCP server）覆盖 Claude Code、Cursor、Codex、Aider 全家桶；甚至有 `headroom learn` 从失败会话挖出修正方案自动写进配置。

这条爆款的真正信号是：**2026 下半年 agent infra 的差异化战场，正从"模型能力"转向"上下文经济学"**。当 Claude/GPT 都向 1M-2M token 进发时，能让 agent 用更少 token 完成同样任务的工具，反而更值钱。

---

### 🥈 [tw93/Pake](https://github.com/tw93/Pake) — +2,398⭐

**老项目今天再起飞：Rust + Tauri 让"把网页装进应用壳子"变成 commodity**

Pake 不是新项目，但今天再次冲上榜单 +2,398⭐，总星累计 **54,596**。它的核心价值简单粗暴：**一行命令把任意 URL 打包成 macOS / Windows / Linux 桌面应用**，基于 Tauri/Rust，相比 Electron 包体小到 5MB 以内。

它最近又上 trending，很可能是因为：(1) 2026 H1 AI 类网页应用激增（Claude / Perplexity / Notion AI），用户想要一个"独立桌面图标 + 独立 dock"而不是放浏览器标签里；(2) 越来越多个人开发者用 Pake 包装自己用 Claude Code/Cursor 生成的小工具，省去打 Electron 包的学习成本。

Pake 出圈的另一面：**它实际上把"前端 + 浏览器 = 桌面 App"这个事彻底 commodity 化了**，未来本地 AI agent 的 UI 壳子可能 80% 都是这种轻量 Tauri 套。

---

### 🥉 [mattpocock/skills](https://github.com/mattpocock/skills) — +1,360⭐（总 138,134）

**Claude Skills 已经形成事实上的"工程实践标准库"**

Matt Pocock（前 TypeScript educator）的这个 repo 总星已经 **13.8 万**，今天再涨 1,360。内容是一组 Claude Code skills，分三类：

- **Engineering Skills**：`/grill-with-docs`、`/tdd`、`/diagnosing-bugs` 等——把 TDD、bug 诊断、文档驱动开发等"硬工程实践"包装成 agent 可执行流程
- **Productivity Skills**：`/grill-me`、`/handoff`、`/teach`——团队协作和知识转移
- **Misc**：边角场景

Matt 在 README 里反复强调"真正工程"对"vibe coding"——这种叙事直接刺中了 senior 开发者对 AI 编码的最大焦虑。**这个 repo 的爆款印证了一个判断：随着 Claude Skills / Agent Skills 在主流 IDE 落地，"skills 库"会成为继 dotfiles / VSCode extensions 之后的下一个个人/团队工程文化载体**。Anthropic 推出 plugins/skills 机制后，这类聚合 repo 必然出现，而 Matt Pocock 凭个人品牌抢到了头位。

---

### 🏅 [DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) — +1,267⭐

**"让 agent 不再 grep 文件"——MCP 生态进入"知识图谱"阶段**

codebase-memory-mcp 用 Tree-sitter（158 种语言）+ LSP 语义层，把整个代码库索引成 SQLite 里的**调用关系图**，暴露 14 个 MCP 工具给 Claude/Cursor 调用。最震撼的数据：

> *"五个结构化查询通过 codebase-memory-mcp 消耗约 3,400 token；同样的探索通过 grep 文件需要约 412,000 token。**99.2% 减少**。"*

对比 28M LOC 的 Linux 内核：3 分钟完成全量索引。普通仓库：毫秒级。

这条爆款延续了 headroom 的同一个主线：**MCP 生态正从"暴露 API 给 Claude"进化到"为 Claude 提供索引结构和探索捷径"**。换句话说，Claude/agent 不需要全文阅读代码，它需要的是一份"地图"。任何能把"代码"这种半结构化数据转成"图"的工具，未来 6-12 个月都会有窗口期。

---

### 🎖️ [tursodatabase/turso](https://github.com/tursodatabase/turso) — +774⭐

**SQLite 的 Rust 重写：内嵌数据库时代的 v2**

Turso 团队明确说这是"用 Rust 重写 SQLite 而非 fork"——保留 SQL 方言、文件格式、C API 兼容，但加上了**并发写（MVCC 的 `BEGIN CONCURRENT`）、CDC、io_uring 异步 I/O、向量搜索、WebAssembly 部署**。

这个项目这两年慢慢爬上来，今天 +774⭐ 跟两件事可能相关：(1) Turso Cloud 商业版的开发者势头持续；(2) "**进程内向量数据库**"成为 RAG/Agent 应用的偏好选择——Chroma/Qdrant 等独立服务的 ops 开销过大，开发者更想要"加一个 SQLite 表"的体验。

Turso 之于 SQLite，就像 Bun 之于 Node.js：**保留生态、重写底层、加现代特性**。今天上榜的几个 repo（headroom、codebase-memory-mcp、Turso）有个隐藏共性：**全是为了让 agent 工作更高效服务的"基础设施重写"**。

---

## 生态观察

今天的 GitHub trending 几乎可以一句话总结："**Agent infra 全栈日**"——前 5 名里 4 个直接服务 agent 工作流：

1. **上下文压缩** (headroom)
2. **代码理解** (codebase-memory-mcp)
3. **Skill 工程化** (mattpocock/skills)
4. **AI 视频编辑** (palmier-pro，MCP server 内嵌)

加上 #8 的 Kilo Code、#7 的 OpenMontage、#12 的 Astro Flue —— **agent 基础设施占了榜单 50%+**。

**两条值得追踪的暗线：**

- **MCP 标准成型**：palmier-pro、codebase-memory-mcp 都把"暴露 MCP server"作为产品差异化卖点。从 6 个月前的 "MCP 是 Anthropic 的协议"变成现在的"MCP 是基础假设"——这是 protocol-level 胜利的明确信号。
- **"为 AI 重做的旧应用"模式爆发**：Twenty（替代 Salesforce）、palmier-pro（替代 Final Cut）、kilocode（替代传统 IDE）——这些 repo 共同卖点是"为 AI 重新设计"，而不是"加 AI 功能"。它们押的是一个更激进的判断：**老软件的 UI/数据模型/工作流根本无法在 agent 范式下使用，必须重写**。

值得对比：传统老牌项目 `penpot` 和 `Kong/insomnia` 今天也在榜单上，但都是温和增长（+424 / +327）——同台对比下，agent infra 类项目的增长曲线明显陡得多。
