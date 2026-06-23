# GitHub Trending 日报 · 2026-06-24

## 今日焦点

> **agentic 视频生产 · Claude Code 工具链卷土重来 · 长视野 agent harness · 自托管 AI 平台 · MCP 代码知识图谱**
>
> - `calesthio/OpenMontage` 一夜 +3,590⭐，号称世界首个开源 agentic 视频生产系统，12 条 pipeline + 52 个工具。
> - `palmier-io/palmier-pro` macOS 端 AI 视频编辑器 +1,631⭐，对标 Final Cut + AI agent。
> - `DeusData/codebase-memory-mcp` +1,299⭐，把代码库索引成知识图的 MCP server，成为 Claude / Cursor 通用底座。
> - `mukul975/Anthropic-Cybersecurity-Skills` +1,040⭐，把 6 大安全框架映射成 817 条 agent 技能，紧跟 OpenAI Glasswing/Daybreak 风口。
> - `garrytan/gstack` +1,012⭐，YC 总裁亲撰的 23 条 Claude Code 高管工作流，又一次把 Claude Code 推上热搜。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) | 首个开源 agentic 视频生产系统，12 pipeline / 52 工具 | Python | 15,460 | +3,590 | 1,845 |
| 2 | [palmier-io/palmier-pro](https://github.com/palmier-io/palmier-pro) | macOS 端为 AI 而生的视频编辑器 | Swift | 8,386 | +1,631 | 551 |
| 3 | [DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) | 把代码库索引成知识图的 MCP server | C | 12,801 | +1,299 | 927 |
| 4 | [ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis) | LLM 驱动的多市场股票分析与新闻聚合 | Python | 46,969 | +1,121 | 42,360 |
| 5 | [jamiepine/voicebox](https://github.com/jamiepine/voicebox) | 开源 AI 语音克隆与创作工作室 | TypeScript | 33,089 | +1,042 | 3,993 |
| 6 | [mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | 817 项 agent 安全技能 + 6 大框架映射 | Python | 19,611 | +1,040 | 2,280 |
| 7 | [garrytan/gstack](https://github.com/garrytan/gstack) | 23 条 Claude Code 高管向工具链 | TypeScript | 114,011 | +1,012 | 16,879 |
| 8 | [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) | 自适应 agent 框架 | Python | 200,875 | +933 | 35,827 |
| 9 | [JCodesMore/ai-website-cloner-template](https://github.com/JCodesMore/ai-website-cloner-template) | 用 AI 编码 agent 克隆任意网站模板 | TypeScript | 18,494 | +827 | 2,799 |
| 10 | [bytedance/deer-flow](https://github.com/bytedance/deer-flow) | 长视野 agent harness：研究 / 编码 / 创作 | Python | 73,868 | +741 | 9,966 |
| 11 | [shanraisshan/claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice) | Agentic engineering 实战指南 | HTML | 59,380 | +329 | 5,978 |
| 12 | [koala73/worldmonitor](https://github.com/koala73/worldmonitor) | AI 驱动的全球地缘情报仪表盘 | TypeScript | 59,043 | +279 | 9,281 |
| 13 | [byoungd/English-level-up-tips](https://github.com/byoungd/English-level-up-tips) | 进阶英语学习指南 | Markdown | 54,479 | +151 | 5,584 |
| 14 | [revfactory/harness](https://github.com/revfactory/harness) | 设计领域 agent 团队的"元 skill" | HTML | 7,424 | +123 | 1,045 |
| 15 | [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) | Claude Code 官方高质量插件目录 | Python | 30,817 | +66 | 3,358 |

---

## 重点项目点评

### 🥇 [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) — 今日榜首，+3,590⭐

**视频生产正在被 agent 全面重写**

OpenMontage 把"视频制作"建模成一组可编排的 agent 任务：剪辑、调色、字幕、配音、转场、版权检测、合规审核都拆成独立 pipeline（共 12 条）和工具（52 个），用一个统一的 orchestrator 串起来。它的卖点是"全开源 + agent-native"——你不需要 Premiere、不需要 Topaz、不需要 ElevenLabs 单独付费，全部由开源模型 + 自家工具链拼起来。

爆榜逻辑很清楚：palmier-pro 同日上榜（macOS AI 视频编辑器），voicebox 上榜（语音合成），三者共同指向**"视频制作 = AI agent 工作流"**正在成为 2026 H2 的开源主线。Adobe / Final Cut 的工具栈第一次面对一个完整的开源替代品集群。

trending 排名第一意味着这条赛道的注意力被锁定，下一步看谁先解决"长视频时序一致性"和"版权安全合规"这两个大问题。

---

### 🥈 [palmier-io/palmier-pro](https://github.com/palmier-io/palmier-pro) — +1,631⭐

**macOS 上的"Final Cut + Cursor"组合**

palmier-pro 是 Swift 写的 macOS 原生 AI 视频编辑器，定位非常清晰——把 Final Cut 的时间轴 + Cursor 的"AI 共驾"塞进同一个 app。它和 OpenMontage 形成上下游：OpenMontage 解决"管道与工具"，palmier-pro 解决"工作面与人机协作"。

值得注意的是 **Swift 这种小众语言冲到 trending 第二**，说明 macOS 原生开发者社区在 AI 工具上有强需求。palmier-pro 也是少见的"既有云端 agent 又有本地原生界面"的双栈架构，撞上苹果今天宣布收编 Swift Package Index，时间窗口完美。

---

### 🥉 [DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) — +1,299⭐

**MCP 进入"知识图层"，Claude / Cursor 通用底座成型**

这是一个 C 语言写的 MCP server，把任何代码库索引成知识图（symbol graph、引用关系、变更历史），然后通过 Model Context Protocol 暴露给 Claude Code / Cursor / Windsurf 等编码 agent。它的关键贡献是**性能**——C 写的索引器加上增量更新，把大仓库的 cold start 时间打下来。

MCP 生态在过去一个季度迅速从"少量官方 + 少量小工具"演化成"agent ↔ 工具"的事实标准接口。codebase-memory-mcp 抓住的是其中最有黏性的一层："让 agent 能像人一样记住整个代码库"。在 The Coming Loop 这种焦虑文章登顶 HN 的同一天，这种"让 agent 在长 loop 里保持上下文一致"的工具自然就成了刚需。

---

### 🏅 [mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) — +1,040⭐

**安全 agent skills 集中爆发，正面响应 OpenAI Daybreak / Anthropic Glasswing**

仓库把 NIST CSF、MITRE ATT&CK、OWASP、CIS、ISO 27001、PCI-DSS 6 大主流安全框架映射成 **817 条 Claude Skills**，让安全工程师可以直接把整套合规与威胁建模工作流装进 Claude Code 用。今天 OpenAI 同步发 GPT-5.5-Cyber 与 Patch the Planet，安全赛道在前沿模型公司层面正式开打，这套社区 skills 是开发者层面的对接。

它的爆榜，再次验证一个规律：**只要 Anthropic 或 OpenAI 在某个垂直方向发新产品，社区 24 小时内就会涌现配套 skills / plugins / MCP server**。安全是下一个 90 天最热的赛道。

---

### 🎖️ [garrytan/gstack](https://github.com/garrytan/gstack) — +1,012⭐

**YC 总裁亲自下场写 Claude Code 高管工作流**

gstack 是 YC President Garry Tan 整理的 23 个 Claude Code 高管工具，包括日程整理、投资备忘录生成、行业研究 brief、邮件草拟、面试纪要等。能在第一天就 +1,012⭐ 是因为它**用最有影响力的"人设"为 Claude Code 背书**——把 Claude Code 从"开发者工具"重新定义为"知识工作者通用 OS"。

这也解释了为什么今天 trending 榜上有 3 个 Claude Code 相关项目（gstack、claude-code-best-practice、claude-plugins-official）。Anthropic 在 IPO 前的开发者生态战已进入"高管 / 知识工作者破圈"阶段，从工程师人群破壁到 C-suite 人群。

---

## 生态观察

今天 trending 的三条主线非常清晰：

1. **agentic 视频生产堆栈成型**：OpenMontage（pipeline）+ palmier-pro（编辑器）+ voicebox（语音）三件套同日上榜，开源社区第一次有了完整的"AI-first 视频制作栈"，对 Adobe / Apple 工具链构成实质性的产品压力。

2. **Claude Code 生态破圈 + MCP 成熟化**：gstack、claude-code-best-practice、claude-plugins-official、codebase-memory-mcp 同时上榜，说明 Anthropic 通过 Skills/Plugins/MCP 三件套已经搭起一个"开发者 + 高管"的双层生态。MCP 工具链从"接 API"进化到"接长期记忆"。

3. **安全赛道借头部模型公司之势爆发**：mukul975 的 817 个安全 skills 上榜，正面回应 OpenAI 与 Anthropic 当天在安全领域的攻防。下一个 90 天看谁能拿下 CISA 采购 = 决定企业市场份额。

副线观察：字节 deer-flow 的"长视野 agent harness"再次进入热榜，国产长 horizon agent 框架在 Sun / Nous Hermes 之外又站稳一席；ZhuLinsen 的多市场股票分析（46K⭐）说明散户 LLM 工具仍是巨型流量入口。
