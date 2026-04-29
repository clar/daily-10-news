# GitHub Trending 日报 · 2026-04-30

## 今日焦点

> **Agent 终端 · Skills 生态爆发 · Codex 工作流 · Coding Harness · 语音 AI**
>
> - `warpdotdev/warp` 一夜涨星 +11,955⭐，Rust 写的"Agent 化终端"开源后直接屠榜
> - `mattpocock/skills` 单日 +7,356⭐，TypeScript 大牛把 .claude 目录搬到了 GitHub
> - `ComposioHQ/awesome-codex-skills` +1,180⭐，Codex Skills 生态正式形成 awesome list
> - `1jehuang/jcode` +386⭐，"Coding Agent Harness"赛道又一个 Rust 实现入场
> - `microsoft/VibeVoice` +1,688⭐，开源前沿语音 AI 站稳 4.5 万星

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [warpdotdev/warp](https://github.com/warpdotdev/warp) | Agentic 开发环境，从终端起步 | Rust | 42,871 | +11,955⭐ | 2,532 |
| 2 | [mattpocock/skills](https://github.com/mattpocock/skills) | "真工程师的 Skills"，直接来自作者 .claude 目录 | Shell | 43,496 | +7,356⭐ | 3,426 |
| 3 | [microsoft/VibeVoice](https://github.com/microsoft/VibeVoice) | 开源前沿语音 AI | Python | 45,588 | +1,688⭐ | 5,038 |
| 4 | [obra/superpowers](https://github.com/obra/superpowers) | Agent 化 skills 框架 + 软件开发方法论 | Shell | 172,964 | +1,683⭐ | 15,257 |
| 5 | [ComposioHQ/awesome-codex-skills](https://github.com/ComposioHQ/awesome-codex-skills) | 实用 Codex skills 精选清单 | Python | 4,707 | +1,180⭐ | 295 |
| 6 | [HunxByts/GhostTrack](https://github.com/HunxByts/GhostTrack) | 位置/手机号追踪工具 | Python | 11,481 | +1,036⭐ | 1,576 |
| 7 | [abhigyanpatwari/GitNexus](https://github.com/abhigyanpatwari/GitNexus) | 客户端知识图谱 + Graph RAG Agent | TypeScript | 33,263 | +777⭐ | 3,771 |
| 8 | [EbookFoundation/free-programming-books](https://github.com/EbookFoundation/free-programming-books) | 免费编程书籍合集 | Python | 387,106 | +609⭐ | 66,179 |
| 9 | [CJackHwang/ds2api](https://github.com/CJackHwang/ds2api) | 客户端协议转通用 API 中间件 | Go | 2,666 | +461⭐ | 717 |
| 10 | [lukilabs/craft-agents-oss](https://github.com/lukilabs/craft-agents-oss) | Agent 工艺开源库 | TypeScript | 5,295 | +432⭐ | 721 |
| 11 | [1jehuang/jcode](https://github.com/1jehuang/jcode) | Coding Agent Harness | Rust | 1,282 | +386⭐ | 124 |
| 12 | [ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis) | LLM 驱动的 A/H/美股实时分析 | Python | 32,655 | +358⭐ | 32,895 |
| 13 | [gorhill/uBlock](https://github.com/gorhill/uBlock) | 高性能广告屏蔽器 | JavaScript | 63,988 | +315⭐ | 4,071 |
| 14 | [iv-org/invidious](https://github.com/iv-org/invidious) | YouTube 替代前端 | Crystal | 19,376 | +243⭐ | 2,133 |
| 15 | [soxoj/maigret](https://github.com/soxoj/maigret) | 跨 3000+ 站点用户名情报收集 | Python | 20,142 | +31⭐ | 1,416 |

---

## 重点项目点评

### 🥇 [warpdotdev/warp](https://github.com/warpdotdev/warp) — 今日榜首，+11,955⭐

**终端的"Agent 革命"完成最后一块拼图：商用产品转身开源**

Warp 一直是"AI 时代终端"的代表作之一，但此前是闭源商用产品。今天直接把 Rust 主体仓库放出来（双协议 AGPL-3.0 / MIT），单日狂揽近 12,000 星，是今天 trending 榜上最极端的一次涨幅。仓库自我定位为 "agentic development environment, born out of the terminal"——明确把自己塞进 Claude Code、Codex CLI、Gemini CLI 之外的另一个赛道：不是命令行里的 agent，而是直接把 agent 嵌入终端这个壳层。

它已经支持 agent 自主完成 issue 分诊、写 spec、改代码、review PR 这条完整链路。开源后最直接的影响是：开发者可以本地审计这层"agent 跑批"如何调度模型、如何托管 session 状态，这对今年密集出现的"agent harness"赛道（jcode、Crush 等）形成强压制——巨头级别的工程量级一旦开源，社区微型实现的差异化空间会被快速压缩。

---

### 🥈 [mattpocock/skills](https://github.com/mattpocock/skills) — +7,356⭐

**"Skills 工业化"开始：知名 TS 教师把 .claude 目录变成产品**

Matt Pocock 是 TypeScript 教学圈最有号召力的人物之一，把自己日常用的 Claude Skills 目录直接整理成开源仓库。一夜涨 7K+ 星，本身就说明 Skills 已经从 "Anthropic 的产品特性" 演变成 "开发者社群的一种内容形态"。

更值得注意的是它的分类：Engineering（TDD、架构改进）、Productivity（grilling sessions、沟通模式）、Misc。这套结构和 Composio 的 awesome-codex-skills 几乎一模一样——说明社区正在自发收敛 Skills 的目录学，未来很可能像 awesome-* 列表那样形成事实标准。对所有还在自己捣鼓 .claude 配置的工程师来说，这种"成熟从业者公开自己的全套 skill"的范式比任何官方文档都更有学习价值。

---

### 🥉 [ComposioHQ/awesome-codex-skills](https://github.com/ComposioHQ/awesome-codex-skills) — +1,180⭐

**Codex Skills 生态完成"awesome 化"——这是范式成熟的标志**

任何技术从工具变成生态，标志之一就是出现 awesome list。今天 Composio 这份 awesome-codex-skills 单日涨 1.1K，覆盖开发工具、协作生产力、写作沟通、数据分析四大类，意味着 Codex CLI 作为 Skills 载体已经被社区认可为"OpenAI 阵营对应 Claude Skills 的标准答案"。

这件事的隐含逻辑值得玩味：Anthropic 的 Skills 通过 Claude Code/Web 推得猛，而 OpenAI 这边的 Codex CLI 在过去几个月默默把 Skills 文件结构对齐到了几乎一样的 SKILL.md 形态。两家在"模型 + Skills"协议层的事实统一，意味着开发者写一份 skill 基本可以双端复用——这条路一旦走通，类似 npm 之于前端的"skill registry"赛道几乎确定会出现，今天 Composio 已经摆好了占位符。

---

### 🏅 [1jehuang/jcode](https://github.com/1jehuang/jcode) — +386⭐

**Coding Agent Harness 赛道的下一波：Rust + 性能极致化**

jcode 自我定位是 "Coding Agent Harness"，与 Crush、opencode、Aider 等同框架性产品同赛道，但卖点是 Rust 实现下的极低内存与极快启动，并强调多会话、多 agent swarm、agent 修改自身源码这些"激进特性"。在 warp 今天开源压制下，这种小而极致的 harness 仍能涨 300+ 星，说明社区对"轻量、可控、本地优先"那批 agent 工具仍有强需求。

它和今天另一个上榜的 lukilabs/craft-agents-oss（TypeScript）形成有趣对照——一个走 Rust 极致性能，一个走 TS 易扩展，反映出 harness 这个新赛道还在分化早期：到底是终端原生派（Warp/jcode）赢，还是 Web/TS 工程化派（craft-agents）赢，仍未见分晓。

---

### 🎖️ [microsoft/VibeVoice](https://github.com/microsoft/VibeVoice) — +1,688⭐

**微软的开源语音 AI 又涨一波，4.5 万星稳了**

VibeVoice 总星数 4.5 万、今天再涨近 1.7K，是当下最热的开源语音模型之一，定位"前沿语音 AI"，覆盖 TTS / 对话语音生成等场景。微软在底层模型层（Phi 系列）已经形成自己的开源叙事，这次加上语音模态，开源故事更完整。

值得注意的是它和 Anthropic、OpenAI 的语音策略对比：后两家更倾向把语音能力深度绑定在闭源 API（Realtime / Voice 模式）里，微软选择直接放权重，给社区做二次开发的空间——对希望低成本搭语音 agent 的开发者来说，VibeVoice 这种级别的开源选项几乎是首选。

---

## 生态观察

今天的 trending 极度集中在一个主题：**"Agent 时代的工具层"全面开源**。从最上游的终端壳（Warp）、到中间的 Coding Agent Harness（jcode、craft-agents-oss）、再到内容层的 Skills 工业化（mattpocock/skills、awesome-codex-skills、obra/superpowers），这三层在同一天集中爆发，绝非偶然——这是 Skills + Agent 协议趋于稳定后，社区开始大规模"填工具链"的典型信号。

热度回落的赛道也很明显：纯模型库、纯前端框架、传统 DevOps 工具今天几乎没有新面孔上榜，连老牌 free-programming-books、uBlock 这种"长青榜"今天的涨幅也被 agent 类项目压成背景板。语音 AI（VibeVoice）和金融 LLM（daily_stock_analysis）则是垂直赛道里维持热度的代表——但它们今天的话语权远不如 agent 工具链那波。

如果只看一条信号：今天 warp 的 +11,955⭐ + mattpocock/skills 的 +7,356⭐，加起来近 2 万星都流向"agent 配套基础设施"——开发者社区对这一层的渴求度，已经到了过去三年没有出现过的强度。
