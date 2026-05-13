# GitHub Trending 日报 · 2026-05-14

## 今日焦点

> **Agent Skills 生态爆发 · 个人 AI 基础设施 · Agent 记忆层 · 反检测浏览器 · 端侧多语 TTS**
>
> - `mattpocock/skills` 一举吸纳 +3,372⭐，把"Claude Skills 直接打包成开源仓库"这套玩法推到新高度
> - `CloakHQ/CloakBrowser` +1,829⭐，反 bot 检测+Playwright 指纹补丁继续成为 Agent 时代的刚需基础设施
> - `tinyhumansai/openhuman` 与 `danielmiessler/Personal_AI_Infrastructure` 同时上榜，"私有化、个人化、可编排"的 AI 副本概念正式出圈
> - `obra/superpowers` +1,506⭐，Agentic Skills Framework 进入 18 万星俱乐部，方法论之争已从 prompt 卷到工程范式
> - `rohitg00/agentmemory` +1,335⭐，coding agent 的 long-term memory 终于有了 benchmark 驱动的新事实标准

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [mattpocock/skills](https://github.com/mattpocock/skills) | Skills for Real Engineers，直接复刻 .claude 目录 | Shell | 78,731 | +3,372⭐ | 6,779 |
| 2 | [CloakHQ/CloakBrowser](https://github.com/CloakHQ/CloakBrowser) | 反检测 Chromium，Playwright 集成 + 指纹补丁 | Python | 9,357 | +1,829⭐ | 693 |
| 3 | [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) | 私有化的个人 AI 超智能 | Rust | 5,110 | +1,595⭐ | 427 |
| 4 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic skills 框架与软件研发方法论 | Shell | 189,369 | +1,506⭐ | 16,852 |
| 5 | [rohitg00/agentmemory](https://github.com/rohitg00/agentmemory) | 基于真实 benchmark 的 coding agent 持久化记忆 #1 | TypeScript | 7,409 | +1,335⭐ | 643 |
| 6 | [supertone-inc/supertonic](https://github.com/supertone-inc/supertonic) | 端侧多语种 TTS，ONNX 原生加速 | Swift | 4,205 | +1,048⭐ | 433 |
| 7 | [yikart/AiToEarn](https://github.com/yikart/AiToEarn) | "用 AI 来 Earn"，AI 套利/赚钱合集 | TypeScript | 12,838 | +987⭐ | 2,214 |
| 8 | [millionco/react-doctor](https://github.com/millionco/react-doctor) | 抓 agent 写的劣质 React 代码 | TypeScript | 9,218 | +620⭐ | 287 |
| 9 | [apernet/hysteria](https://github.com/apernet/hysteria) | 高速抗审查代理 | Go | 20,579 | +489⭐ | 2,128 |
| 10 | [danielmiessler/Personal_AI_Infrastructure](https://github.com/danielmiessler/Personal_AI_Infrastructure) | 放大个人能力的 Agentic AI 基础设施 | TypeScript | 13,286 | +439⭐ | 1,861 |
| 11 | [imthenachoman/How-To-Secure-A-Linux-Server](https://github.com/imthenachoman/How-To-Secure-A-Linux-Server) | 持续演进的 Linux 服务器加固指南 | Markdown | 27,020 | +233⭐ | 1,773 |
| 12 | [Greedeks/GTweak](https://github.com/Greedeks/GTweak) | Windows 一键调优便携工具 | C# | 874 | +127⭐ | 75 |
| 13 | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) | 科研/工程/金融领域的 Agent Skills 工具包 | Python | 21,043 | +83⭐ | 2,320 |
| 14 | [ArthurBrussee/brush](https://github.com/ArthurBrussee/brush) | 面向所有人的 3D 重建工具 | Rust | 4,332 | +78⭐ | 231 |
| 15 | [influxdata/telegraf](https://github.com/influxdata/telegraf) | 指标/日志/数据采集与处理 agent | Go | 16,966 | +6⭐ | 5,776 |

---

## 重点项目点评

### 🥇 [mattpocock/skills](https://github.com/mattpocock/skills) — 今日榜首，+3,372⭐

**"我的 .claude 目录就是教科书"——Skills 已经从教程变成可分发资产**

Matt Pocock 是 TypeScript 社区的常驻 KOL，他选择把自己的 `.claude/skills` 目录原样开源，直接踩中了今年 GitHub 最热的新格式：Skill 不是 prompt、也不是 agent，而是一份可被 Claude Code 自动加载的"工序"。这个仓库今天单日新增 **+3,372⭐**，总星数飙到 7.8 万，等于一夜之间把一个工程师的私域工具放进了所有人的 PATH。

它真正打动开发者的不是单个 skill 本身，而是把"行业最佳实践"打包成可执行单元、可被 Agent 直接调用的范式。这意味着从 2026 年开始，简历不再只列项目，而要列你能为团队补充哪些 Skill 包。和 `obra/superpowers`、`K-Dense-AI/scientific-agent-skills` 排在一起看，今天的热榜其实就是一次 Skills 集体出道。

---

### 🥈 [CloakHQ/CloakBrowser](https://github.com/CloakHQ/CloakBrowser) — +1,829⭐

**Agent 越多，反检测浏览器就越值钱**

CloakBrowser 把"反 bot 检测的 Chromium"、Playwright 集成、指纹补丁打成了一个 Python 友好的开源底座。今天 **+1,829⭐** 不是偶然——它瞄准的正是 2026 年大爆发的 browser-use 类 agent：当模型可以自主点网页时，目标站点的 Cloudflare、Akamai、Datadome 拦截就是直接成本。

值得关注的是社区情绪：一年前同类项目大多以"灰产工具"形象出现，今天 CloakBrowser 已经能正面挂在 trending 第二位，说明开发者圈对"自动化浏览 = 第一公民工作流"达成了默认共识。下一个问题是大型站点会如何回击，但短期来看，反检测层将和 LLM、vector DB 一样成为 agent 栈的标配组件。

---

### 🥉 [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) — +1,595⭐

**Rust 写的"个人超智能"，把端侧 AI 推向了新尺度**

openhuman 的定位写得很直接：Private、Simple、Extremely Powerful，本质是把 LLM、记忆、工具、UI 全栈打包成一个可本地运行的"私有 AI 副本"。Rust 实现意味着它对内存/算力的拿捏远超同类 Electron + Python 组合，今天 **+1,595⭐** 的曲线和 `danielmiessler/Personal_AI_Infrastructure` 高度同步。

这不是普通的"chat 客户端 +1"，而是反映了一种生态焦虑：大模型云端化越深、个人数据让渡就越多，因此社区开始用工程语言（Rust）和私有部署回应这种焦虑。可以把今天的热榜上半区理解为"私有化 AI 副本 + Agent Skills"双主线，openhuman 是前者的旗手。

---

### 4️⃣ [obra/superpowers](https://github.com/obra/superpowers) — +1,506⭐

**18.9 万星的 Agentic 框架：方法论之争已经赢了**

`obra/superpowers` 今天再涨 **+1,506⭐**，总数顶到 **189,369⭐**——这个体量已经把它推到 GitHub 历史前 50 的位置。和 `mattpocock/skills`、`K-Dense-AI/scientific-agent-skills` 一起看，今天热榜其实是一场 "agentic skills" 的集体阅兵。

superpowers 的特别之处在于：它不是工具集，而是一套**方法论**——如何用 skill 化的方式重写整个软件研发流程。它今年的增长曲线证明，社区已经从"哪个 LLM 更强"切换到"哪种工程组织更高效"这个新战场。明年招聘里看到 "experience with agentic skills frameworks" 这一行已经不必惊讶。

---

### 5️⃣ [rohitg00/agentmemory](https://github.com/rohitg00/agentmemory) — +1,335⭐

**Coding Agent 的长记忆终于卷出了一个事实标准**

agentmemory 主打"coding agent 的持久化记忆"，并强调自己在真实 benchmark 上拿到 #1，今天 **+1,335⭐** 直接把这个细分品类的关注度推到顶。过去半年，memory 层从 RAG → 工具记忆 → episodic 记忆几代演进，社区终于开始用统一 benchmark 比较——而不是各自 demo。

它的火爆背后还有一条暗线：随着 agent 处理的代码库越来越大，"上下文工程"成为头号痛点。一个真正可用的 memory 层意味着 agent 可以跨 session 维持判断、跨仓库做迁移。如果它的 benchmark 复现得住，那么主流 IDE agent（Cursor、Cline、Claude Code）半年内都需要给出答复。

---

## 生态观察

今天的榜单可以用一句话概括：**Agent 的下一战，不在模型，而在工具链**。前五位都是工程层资产——Skills 仓库、反检测浏览器、个人 AI 副本、Agentic 框架、Agent 长记忆——它们共同回答的是"当模型已经够强，下一层基础设施是什么"。

热度还集中体现了两个趋势：一是**私有化 AI 副本**正从概念走向工程范式，openhuman 的 Rust 实现和 Personal_AI_Infrastructure 的体系化打包都是同一阶段产物；二是**Agent Skills 已经成为社区货币**，从 mattpocock 的工程师皮、scientific-agent-skills 的科研皮，到 obra 的方法论皮，呈现出多生态多形态的爆炸式分化。

相对冷清的是基础设施类老项目（telegraf、hysteria 增量平淡），说明 2026 年的注意力天然倾斜到 AI 工具栈。短期值得追踪的，是 **CloakBrowser** 类反检测层会不会引来主流站点的硬反制，以及 **agentmemory** 这种带 benchmark 的细分组件，能否成为 agent 标配。
