# GitHub Trending 日报 · 2026-04-29

## 今日焦点

> **Skills 生态爆炸 · Claude Code 第三方代理 · 代码知识图谱 · 开源语音/音乐 · Markdown 现代化**
>
> - `mattpocock/skills` 单日 +7,429⭐ 登顶，AI agent skills 已成显学
> - `ComposioHQ/awesome-codex-skills` +961⭐ 进入榜单，OpenAI Codex 也走"skill 化"路线
> - `abhigyanpatwari/GitNexus` +1,565⭐，浏览器端 Graph RAG 给 AI 编程加上"全局视野"
> - `Alishahryar1/free-claude-code` +1,706⭐，Claude Code 的多后端代理热度持续
> - `microsoft/VibeVoice` 和 `fspecii/ace-step-ui` 一起把开源语音/音乐推上前台

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [mattpocock/skills](https://github.com/mattpocock/skills) | 面向真实工程师的 Claude skills 集合 | Shell | 36,624 | +7,429⭐ | 2,871 |
| 2 | [abhigyanpatwari/GitNexus](https://github.com/abhigyanpatwari/GitNexus) | 浏览器端代码知识图谱与 Graph RAG | TypeScript | 32,551 | +1,565⭐ | 3,695 |
| 3 | [Alishahryar1/free-claude-code](https://github.com/Alishahryar1/free-claude-code) | 通过代理把 Claude Code 接到多种后端 | Python | 17,354 | +1,706⭐ | 2,445 |
| 4 | [microsoft/VibeVoice](https://github.com/microsoft/VibeVoice) | 微软开源的前沿语音 AI | Python | 44,600 | +1,523⭐ | 4,963 |
| 5 | [ComposioHQ/awesome-codex-skills](https://github.com/ComposioHQ/awesome-codex-skills) | 面向 OpenAI Codex CLI 的 skills 清单 | Python | 3,898 | +961⭐ | 248 |
| 6 | [HunxByts/GhostTrack](https://github.com/HunxByts/GhostTrack) | 定位/手机号信息追踪工具 | Python | 10,492 | +976⭐ | 1,481 |
| 7 | [iamgio/quarkdown](https://github.com/iamgio/quarkdown) | 带超能力的 Markdown，论文/演示/网站一套源码 | Kotlin | 11,859 | +797⭐ | 315 |
| 8 | [donnemartin/system-design-primer](https://github.com/donnemartin/system-design-primer) | 系统设计面试经典仓库 | Python | 345,772 | +734⭐ | 55,824 |
| 9 | [public-apis/public-apis](https://github.com/public-apis/public-apis) | 免费公共 API 清单 | Python | 427,993 | +600⭐ | 46,744 |
| 10 | [CJackHwang/ds2api](https://github.com/CJackHwang/ds2api) | 协议转通用 API 的轻量中间件，支持多账号轮询 | Go | 2,274 | +418⭐ | 643 |
| 11 | [davila7/claude-code-templates](https://github.com/davila7/claude-code-templates) | Claude Code 配置与监控 CLI | Python | 26,097 | +347⭐ | 2,611 |
| 12 | [fspecii/ace-step-ui](https://github.com/fspecii/ace-step-ui) | ACE-Step 1.5 AI 音乐生成专业 UI | JavaScript | 1,594 | +263⭐ | 253 |
| 13 | [EbookFoundation/free-programming-books](https://github.com/EbookFoundation/free-programming-books) | 免费编程书清单 | Python | 386,559 | +133⭐ | 66,158 |

---

## 重点项目点评

### 🥇 [mattpocock/skills](https://github.com/mattpocock/skills) — 今日榜首，+7,429⭐

**当 "skill" 取代 "prompt" 成为新的开源单元**

mattpocock 把自己 `.claude/` 目录里那套日常用的工程师 skill 完整开源——`/tdd`、`/diagnose`、`/grill-with-docs`、`/improve-codebase-architecture`、`/grill-me`、`/caveman` 等等，覆盖测试驱动、调试、需求澄清、架构改造和压缩沟通。这些不是花哨的 demo，而是一个有名望的 TypeScript 教学者长期"驯化" agent 的真实产出。

它一夜涨 7.4k 星说明了两件事：第一，"skill" 已经稳定成为 Claude Code/Codex 这类 agent 体系的最小可分享单元——比 prompt 更结构化、比插件更轻量；第二，社区开始更看重"工程方法论"而不是"提示词魔法"。仓库里反复强调的四个痛点（意图错位、术语混乱、反馈回路差、架构腐化）正是 vibe coding 一年后所有人都在补的功课。

可以预期未来几周会出现更多个人/团队公开自己的 `.claude/skills`，并逐步催生 skill 包管理、版本化、组合化的二级生态。

---

### 🥈 [Alishahryar1/free-claude-code](https://github.com/Alishahryar1/free-claude-code) — +1,706⭐

**Claude Code 客户端协议正在被"标准化"**

这个项目把 Claude Code 的 API 请求劫持到本地 `localhost:8082`，再转发给 NVIDIA NIM、OpenRouter、DeepSeek、LM Studio、llama.cpp 或 Ollama。换句话说，它把 Claude Code 当成了一个"前端"，让用户自由替换"后端"。在 Anthropic 官方限额、按 token 计费的现实下，这种打法对学生、独立开发者、小团队极具吸引力。

它今日继续涨 1.7k 星，本质上是在把 Claude Code 的客户端协议事实标准化。一旦"任何模型都能跑 Claude Code"，那么 Claude Code 的护城河就从"模型"转向"客户端体验 + skills 生态"。这恰好与今日榜首的 skills 仓库形成呼应：客户端是壳，skills 是肉，模型可替换。

需要警惕的是，这类代理对 Anthropic 的 ToS 是灰色地带，长期风险在于规则收紧或客户端协议变更。

---

### 🥉 [abhigyanpatwari/GitNexus](https://github.com/abhigyanpatwari/GitNexus) — +1,565⭐

**给 AI 编程补一块"全局结构视野"**

GitNexus 用 Tree-sitter 把 14+ 种语言的代码解析成 AST，构建出一张可在浏览器里交互的代码知识图谱，并暴露 16 个 MCP 工具（影响面分析、多文件改名、blast radius、社区聚类等）给 Cursor、Claude Code、Windsurf 等 agent 调用。它解决的痛点是当下所有 vibe coding 用户最痛的一件事：**agent 改了 `UserService.validate()`，但不知道 47 个函数依赖它的返回类型**。

它的工程取舍很有意思——不是查询时算关系，而是索引时**预先**把结构关系算好，让小模型也能在一次 tool call 里拿到完整上下文。这是对 Graph RAG 的一次具体落地，也是"agent 平台化"的关键基础设施：从单文件级别向项目级别跃升。

---

### [microsoft/VibeVoice](https://github.com/microsoft/VibeVoice) — +1,523⭐

**微软的开源语音前沿模型继续吃星**

VibeVoice 自发布以来一直在榜上，单日还能再 +1.5k 说明它已经成为开源语音生态的事实参考。配合榜单第 12 的 `ace-step-ui`（ACE-Step 1.5 音乐模型的专业前端），今日的语音和音乐两条赛道一起在被推到聚光灯下。

值得注意的是，开源音频生成在 2026 年才真正进入"可用"门槛——VibeVoice 主打 frontier 级语音质量，ACE-Step 主打 Suno 替代品。两者一个是模型，一个是 UI，叠加之后基本可以本地搭出一套不打折扣的语音/音乐生产线。这对内容创作者和小型工作室是非常实质的成本下降。

---

### [ComposioHQ/awesome-codex-skills](https://github.com/ComposioHQ/awesome-codex-skills) — +961⭐

**OpenAI 阵营也学会了"skills"**

Composio 维护的这份清单把 OpenAI Codex CLI 的 skill 生态做了系统化整理，涵盖 PR review、CI 自动修复、Linear/Jira triage、会议纪要转 action items、Notion 集成、Datadog 日志过滤等 50+ 条目。仓库本身只有 3.9k 星但今日 +961，增长速度很快。

把它和今日榜首的 mattpocock/skills 放一起看，趋势非常清楚：Anthropic Claude Code 和 OpenAI Codex CLI 都已经把"skill"当作官方的最小工作单元，社区开始向两边复用同一套 mental model。下一步八成会出现"skill 翻译器"——把同一个 skill 同时编译成 Claude Code 和 Codex 两种 runtime 的格式。

---

## 生态观察

今天的榜单几乎可以用一个词概括：**Skill 化**。

- **AI 编程基础设施层**正在从"会聊天的 IDE 插件"演化成"客户端协议 + skill 生态 + 项目级理解"三件套：mattpocock/skills 是 skill 层，free-claude-code 是协议层，GitNexus 是项目级理解层。这三件事一起涨星不是巧合。
- **多供应商主义**抬头：开发者越来越不愿被绑在单一模型公司，free-claude-code、ds2api 这类"协议转换"项目持续受关注，意味着模型层正在被快速商品化。
- **开源音频**（语音 + 音乐）从沉寂多年到今日双双进榜，是一个值得长期跟踪的拐点。
- **经典清单类仓库**（system-design-primer、public-apis、free-programming-books）依然稳定收割 700/600/100 星——技术热点变快，但基本面阅读需求一点没变。

如果说昨天还在讨论"AI 编程会不会泡沫"，今天的榜单已经在告诉答案：泡沫还没到，因为基础设施才刚开始被组合起来。
