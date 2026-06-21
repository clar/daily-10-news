# GitHub Trending 每日热榜 · 2026-06-22

## 今日焦点

> **AI 视频生产链全面冒头 · LLM token 压缩成新刚需 · MCP 与代码记忆继续吸星 · 开源设计/桌面工具老树新花 · 网络安全 skills 集合获大量收藏**
>
> - `chopratejas/headroom` 一日 +2,617⭐，把 LLM 上下文压缩做成开源刚需。
> - `palmier-io/palmier-pro` Swift 写的"AI 原生" macOS 视频编辑器登顶，+1,829⭐。
> - `tw93/Pake` 老牌"网页变桌面 app" Rust 工具 +1,850⭐，今天又被一波"打包 AI 助手"的需求顶上来。
> - `mattpocock/skills` Matt Pocock 个人工程 skills 集合 +1,441⭐，14 万星里又涨一茬。
> - `bytedance/deer-flow` 字节的 long-horizon agent 框架持续吸星 +415⭐，总星 72k。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [palmier-io/palmier-pro](https://github.com/palmier-io/palmier-pro) | AI 原生 macOS 视频编辑器 | Swift | 4,971 | +1,829 | 377 |
| 2 | [chopratejas/headroom](https://github.com/chopratejas/headroom) | LLM token 压缩 60-95% 工具 | Python | 44,166 | +2,617 | 3,077 |
| 3 | [tw93/Pake](https://github.com/tw93/Pake) | 一行命令把网页打包成桌面 app | Rust | 56,097 | +1,850 | 11,084 |
| 4 | [mattpocock/skills](https://github.com/mattpocock/skills) | 个人工程 skills 集合 | Shell | 139,647 | +1,441 | 12,119 |
| 5 | [penpot/penpot](https://github.com/penpot/penpot) | 开源设计 + 代码协作工具 | Clojure | 52,175 | +1,131 | 3,334 |
| 6 | [DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) | 高性能代码索引 MCP 服务 | C | 10,198 | +1,029 | 771 |
| 7 | [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) | 12 流水线 52 工具的 agentic 视频生产 | Python | 8,545 | +993 | 1,283 |
| 8 | [tursodatabase/turso](https://github.com/tursodatabase/turso) | SQLite 兼容的内嵌 SQL 数据库 | Rust | 20,763 | +543 | 1,061 |
| 9 | [ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis) | LLM 驱动多市场股票分析 | Python | 44,356 | +519 | 41,415 |
| 10 | [mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | 754 个安全 skills for AI agents | Python | 17,615 | +445 | 2,125 |
| 11 | [bytedance/deer-flow](https://github.com/bytedance/deer-flow) | 字节长程 agent 框架 | Python | 72,527 | +415 | 9,827 |
| 12 | [topoteretes/cognee](https://github.com/topoteretes/cognee) | 自托管 AI 记忆 + 知识图谱 | Python | 18,614 | +361 | 1,968 |
| 13 | [smicallef/spiderfoot](https://github.com/smicallef/spiderfoot) | OSINT 自动化威胁情报 | Python | 18,724 | +288 | 3,106 |
| 14 | [koala73/worldmonitor](https://github.com/koala73/worldmonitor) | 实时全球态势监控仪表盘 | TypeScript | 58,025 | +253 | 9,202 |
| 15 | [mikumifa/biliTickerBuy](https://github.com/mikumifa/biliTickerBuy) | 哔哩哔哩抢票辅助 | Python | 3,703 | +56 | 464 |

---

## 重点项目点评

### 🥇 [chopratejas/headroom](https://github.com/chopratejas/headroom) — +2,617⭐

**"上下文越长越贵"这件事终于有人开源解决方案**

Headroom 是一套独立运行在客户端的 LLM token 压缩中间件，宣称在 60-95% 区间压缩对话历史与代码片段，且对下游模型 (Claude / GPT-5.5 / Gemini) 无侵入。今天 +2,617⭐ 是榜单第一，反映的不是"又一个 hack"，而是**主流开发者已经把"长上下文成本"列为生产环境的一级问题**——SpaceX 给 Anthropic 锁 300MW 算力的同一周，开发者群体正在反方向自救。

值得关注的两条线：(1) 它和 `topoteretes/cognee`（开源 AI 记忆 + 知识图谱）形成互补——前者降本、后者增智；两个项目今天都进了 Top 15，说明 RAG + 上下文工程仍是真正的高增长生态位。(2) 项目用纯 Python，无 GPU 依赖，意味着它能直接嵌进任何 IDE 插件 / agent runtime——这是 AI 编码工具从"显卡党"过渡到"日常开发栈"的一种典型征兆。

---

### 🥈 [palmier-io/palmier-pro](https://github.com/palmier-io/palmier-pro) — +1,829⭐

**Swift + macOS 原生的 AI 视频编辑器，第一次把 Apple Silicon 推到舞台中央**

Palmier Pro 是用 Swift 重写的 macOS 视频编辑器，所有 AI 功能（自动剪辑、语义检索、风格迁移）跑在本地 Apple Silicon 上，主打"不上云、不限时、不订阅"。今天首日就拿到 +1,829⭐，背后的语境很清楚：**WWDC 2026 把 Apple Intelligence 重新做了一遍，Siri AI 已经全面接入 Gemini**——开发者群体马上跟进，用 Apple 的本地推理栈做"反订阅"的工具型应用。

跟它撞档的 `calesthio/OpenMontage`（Python，12 流水线 52 工具）也今天进入榜单，但路线截然相反：OpenMontage 是 agentic、跨平台、Cloud-friendly；Palmier 是原生、单设备、隐私优先。这两套路线第一次在 trending 同一天出现，意味着**"AI 视频生产"这个赛道开始分化为云原生 agent 派 vs. 本地原生体验派**，2026 H2 会出现更多围绕这两端的产品。

---

### 🥉 [tw93/Pake](https://github.com/tw93/Pake) — +1,850⭐

**老项目今日复活，是"AI 助手桌面化"的回声**

Pake 是 2022 年就开始火的 Rust 工具，可以把任意网页一键打成轻量级 Tauri 桌面 app。今天它能再涨 +1,850⭐ 并不是因为做了什么大版本——而是因为 **Anthropic Fable 5 下线、Claude 网页客户端用户被迫切走、开发者群体开始批量自建 "Claude / ChatGPT 桌面端"**。Pake 是这种场景下最快的解决方案，跨越 Win / macOS / Linux。

这一波让 56k 星的"老仓库"再次回到首页，本质上反映了一种用户行为：**当云服务被打断时，HN/GitHub 群体的第一反应不是抱怨，而是去找/复活那个最适合"自包装"的工具**。后续可关注：(1) Tauri 2.x 生态下 Pake 是否会被 fork 出"原生 MCP 容器"分支；(2) Rust 桌面工具今年的 trending 频次正在反超 Electron 阵营。

---

### 4️⃣ [mattpocock/skills](https://github.com/mattpocock/skills) — +1,441⭐

**个人工程经验仓被当作"AI 时代的开发者第二大脑"**

Matt Pocock（TypeScript 教育博主）把自己的工程 skills 全部仓库化，今天涨 +1,441⭐，总星 139k 进一步巩固它"最像样的个人工程知识库"地位。它真正爆发的原因不是内容增量，而是**Claude Code / Cursor / Codex 都已经原生支持把这种 skills 仓库当 agent 上下文加载**——`mattpocock/skills` 实际上已经成为"自然语言写工程规范"的事实参考样本。

同榜的 `mukul975/Anthropic-Cybersecurity-Skills`（754 个安全 skills）走的是同一种打法，但聚焦在网安。两者一起反映了趋势：**"Skill repo as a service" 正在取代旧的 dotfiles / awesome-list**，开发者把自己最有价值的提示词、调用模式、SOP 公开仓库化，让 agent 系统直接消费。

---

### 5️⃣ [bytedance/deer-flow](https://github.com/bytedance/deer-flow) — +415⭐

**字节的 long-horizon agent 框架持续吸星，总星 72k 仍在涨**

Deer-flow 是字节开源的"长程任务 agent 框架"，主打多步研究 + 多步编码两个核心场景。+415⭐ 当日增量不算最大，但放在 72k 总星的体量上仍是稳定增长，说明它在 agent 中间件赛道已经完成"事实标准化"——大量国内外项目把 deer-flow 当作 baseline 来对比。

值得注意的是：今天榜单上一共有 4 个 agent / MCP 相关的 Python 项目（OpenMontage、codebase-memory-mcp、cognee、deer-flow）+ 1 个 cybersecurity skills 仓库 + 1 个个人 skills 仓库。**"agent runtime + skill 仓库" 已经是 2026 年 GitHub trending 的主旋律**，相比一年前的"开源大模型"主导有了根本性的位移。

---

## 生态观察

今天的榜单把 2026 H1 的 AI 工具链生态分得很清楚：

**第一层（基础设施）：** Headroom 做 token 压缩、cognee 做记忆、codebase-memory-mcp 做代码索引——这一层在解决"上下文工程"的成本与质量。三个项目今天合计涨星 4,007⭐。

**第二层（agent runtime）：** deer-flow、OpenMontage 这种"多步骤任务执行框架"在持续吸星，但增速已经放缓，意味着该赛道开始进入收敛期，下一步看的是哪几个框架能进入企业级生产案例。

**第三层（skill / 经验仓）：** mattpocock/skills 和 Anthropic-Cybersecurity-Skills 代表了新一类"内容仓库"，它们不是软件，而是给 agent 用的高质量上下文池。值得关注的是这类仓库已经超过传统 awesome-list 的增长曲线。

**第四层（用户层）：** Palmier Pro / Pake / penpot 显示用户层工具仍有空间——尤其在"反订阅、本地优先、隐私优先"这条线上。Apple Silicon 本地推理在 WWDC 2026 后已经被开发者重新拾起。

老项目（Pake、penpot、spiderfoot、turso、deer-flow）今天集体回到榜单，说明 trending 算法正在被"AI Agent 上下文整合"型需求驱动反复点燃。下一周值得继续观察：MCP server 类仓库（codebase-memory-mcp 已经进 Top 6）和"skills 仓库"两条增速是否能保持。
