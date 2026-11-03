# GitHub Trending 每日报告 · 2026-11-04

## 今日焦点

> **Claude / Agent 生态继续霸榜 · 本地 MoE 推理栈崛起 · 爬虫与金融 FM 回流 · 去审查权重编辑 · 并行 Agent 工程化**
>
> - `thedotmack/claude-mem` 跨会话持久记忆仓库，+1,138⭐，Claude 代理基建继续扩军。
> - `vercel-labs/agent-desktop` Rust 实现的 Computer-use CLI，+3,792⭐，今日最大赢家。
> - `JustVugg/colibri` C 语言 MoE 分层推理引擎，把 GPU/RAM/NVMe 当成三级显存。
> - `D4Vinci/Scrapling` 老牌爬虫框架 +1,658⭐，LLM 数据管道让爬虫需求回暖。
> - `p-e-w/heretic` 免训练修改模型以降低审查/谄媚倾向，掀起权重操控新一轮讨论。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | AI 代理跨会话持久记忆，附 AI 压缩 | TypeScript | 111,820 | +1,138 | 9,732 |
| 2 | [vercel-labs/agent-desktop](https://github.com/vercel-labs/agent-desktop) | Rust 版 Computer-use CLI | Rust | 12,567 | +3,792 | 867 |
| 3 | [max-sixty/worktrunk](https://github.com/max-sixty/worktrunk) | git worktree + 并行 agent 工作流 CLI | Rust | 10,449 | +437 | 375 |
| 4 | [JustVugg/colibri](https://github.com/JustVugg/colibri) | 跨 GPU/RAM/NVMe 的分层 MoE 推理引擎 | C | 47,214 | +803 | 5,460 |
| 5 | [mattpocock/skills](https://github.com/mattpocock/skills) | 作者 `.agents` 目录里的工程技能合集 | Shell | 311,371 | +1,164 | 26,169 |
| 6 | [p-e-w/heretic](https://github.com/p-e-w/heretic) | 免训练修改模型降低审查与谄媚 | Python | 38,735 | +699 | 4,377 |
| 7 | [spotify/portal-ai-plugins](https://github.com/spotify/portal-ai-plugins) | Spotify Portal 的 AI 插件 | TypeScript | 3,021 | +94 | 235 |
| 8 | [floci-io/floci](https://github.com/floci-io/floci) | 轻量本地 AWS 模拟器 | Java | 28,692 | +679 | 3,197 |
| 9 | [Usagi-org/ai-goofish-monitor](https://github.com/Usagi-org/ai-goofish-monitor) | Playwright + AI 咸鱼监控 | Python | 16,330 | +204 | 2,840 |
| 10 | [anomalyco/hex](https://github.com/anomalyco/hex) | 跨平台本地语音听写 | Rust | 4,536 | +410 | 255 |
| 11 | [D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling) | 从单请求到大规模爬虫的框架 | Python | 94,686 | +1,658 | 9,929 |
| 12 | [shiyu-coder/Kronos](https://github.com/shiyu-coder/Kronos) | 面向金融市场数据的基础模型 | Python | 46,484 | +503 | 7,659 |
| 13 | [Donchitos/Claude-Code-Game-Studios](https://github.com/Donchitos/Claude-Code-Game-Studios) | Claude Code 变 49 agent / 72 skill 的游戏工作室 | Shell | 34,604 | +1,181 | 4,588 |

---

## 重点项目点评

### 🥇 [vercel-labs/agent-desktop](https://github.com/vercel-labs/agent-desktop) — 今日最大新增，+3,792⭐

**Vercel 亲自下场，Computer-Use 开始"CLI 化"**

这是今天涨得最猛的仓库。Vercel 把一个 Rust 写的"桌面代理"的本地 CLI 开源出来——它直接把屏幕、键盘、鼠标、文件系统封装成一组工具调用，对接 Claude 的 computer-use API 和 OpenAI Responses 的工具链。在 Anthropic 本周把 Claude Code 的游戏克隆权限收紧、Goldman Sachs 收紧 Claude Code 使用权限的背景下，Vercel 的策略是反方向的：把代理式 computer use 做成开发者本地可以完全自托管的 CLI。

更值得注意的是它用 Rust 而非 TypeScript。两点信号：（1）Vercel 内部的 agent runtime 正在脱离 Node.js 向 systems 语言下沉；（2）这类产品需要的截屏/输入注入/沙箱隔离在 Rust 里能做得又快又安全——这是 Zed、Flipper 等项目选 Rust 的同一逻辑。

今天的 +3,792 几乎等于把整个前 20 其他项目的日增总和的三分之一，它可能成为未来几周 "self-hosted computer use" 的 reference impl。

---

### 🥈 [D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling) — +1,658⭐

**LLM 把爬虫需求又拉回了 2015 年的热度**

Scrapling 是一个相对老牌的 Python 爬虫框架，突然被 +1,658 顶到前列的驱动力并不是新 release，而是整个 LLM 生态对"结构化网页数据"的饥渴程度：Deep Research、RAG、模型评测、垂直 Agent 都需要稳定可控的网页抓取管道。本周纽约时报起诉 Brave、Reddit 继续对抗 AI 抓取、Cloudflare 推新一轮 bot 挑战，叠加 OpenAI / Anthropic 对训练数据的审计压力，每个要做 vertical agent 的团队都在重新搭自己的爬虫栈。

Scrapling 这类"中级复杂度 + 开源 + 可自部署"的框架最受益——它既不像 Playwright 那么重，也不像 requests 那么没防御性，正好贴合 LLM 产品化阶段的工程需要。

---

### 🥉 [JustVugg/colibri](https://github.com/JustVugg/colibri) — +803⭐

**本地推理栈的下一个突破点：让 NVMe 变成"冷显存"**

colibri 是用 C 实现的 MoE 分层推理引擎，核心想法是把专家权重按活跃度放到 GPU / RAM / NVMe 的三级存储上，并在 token 级别预取。这之所以重要，是因为 2026 年我们已经看到一波万亿级 MoE 开源：DeepSeek-V4、Qwen 3.x、Kimi K2、Meituan LongCat-2.5（今天刚发的 1.6T 稀疏模型）。在 24 GB 显存、128 GB RAM、2 TB NVMe 的开发者机器上，谁能把 1.6T MoE 的推理成本控制下来，谁就赢。

colibri 的方向与 llama.cpp 的 offloading、DeepSpeed-Inference 的 Zero-Inference 构成竞争——但它把速度瓶颈压到 NVMe 读的 IOPS 这一层，而不是 PCIe 带宽。这是一个值得密切跟踪的 systems-level 项目。

---

### 🧠 [p-e-w/heretic](https://github.com/p-e-w/heretic) — +699⭐

**"修改权重把模型调回不审查"：一道新的伦理与法律边界**

Heretic 以 Python 实现一套 **training-free** 修改方式，针对 LLM 的 refusal direction 与 sycophancy direction 做权重编辑（概念上类似 2024 年 ablation of refusal direction 的方法学）。这在 HN、Twitter / X、Reddit 本地模型圈同时发酵——一方面被当成"把模型解封"的捷径，另一方面也意味着开源权重一旦发布，任何对齐工作都不再是最后一道门。

这件事放在今天的宏观叙事里格外微妙：Anthropic 刚在 S-1 里警告正逼近"AI 自加速研发"阈值并计划升级 RSP；MIT 的 Astra 本周被误传为"AI 自改权重"后被 Honnibal 拉回地面。Heretic 展示的恰好是"研究所警告的那个风险的日常版本"——不是 AGI，而是任何有 GPU 的人都能让一个开源模型变得更危险。

---

### 💾 [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) — +1,138⭐（榜首）

**Claude 代理记忆基建继续横向扩张**

claude-mem 把 Claude 会话的上下文做跨会话压缩、分片、持久化，使 Claude Code / Claude Agent SDK 可以像"长期雇员"一样记住之前的决策、代码库约定、用户偏好。它和前几周先后登榜的 claude-agent-sdk-memory、claude-flow、worktrunk（今天也在榜上）一起，构成一套围绕 Anthropic 官方 SDK 的"外设生态"。

这个方向在 2026 下半年火的根本原因是：Anthropic 自己给 Claude Agent SDK 留了钩子，但没自己做完整的记忆层——于是社区把"记忆 / 并行 worktree / 任务队列 / 技能库"这几块缺口统统补上。Github 上 claude-* / claude-code-* 前缀仓库目前日增数量仍在持续增长，说明"Claude 生态 ≈ 2026 年的 npm 时刻"这件事并不是口号。

---

## 生态观察

今天 13 条热榜里有 **5 条**直接服务 Claude / Computer-Use / 代理工作流（claude-mem、agent-desktop、worktrunk、skills、Claude-Code-Game-Studios），加上 colibri（本地跑 MoE）、heretic（权重编辑）、hex（本地语音）、ai-goofish-monitor（Playwright + LLM 实用 agent），整整 **9 条**可归入"开源 AI 基础设施"。剩下的 Scrapling 和 Kronos 虽然没写 LLM，但本质上也在为 LLM 时代的输入与金融应用做基础构件。

两个趋势越来越明显：

1. **代理工具链"Rust 化"**。agent-desktop、worktrunk、hex 均为 Rust；Zed、Flipper、Nushell 已是常态；Node.js 继续被挤到"UI + glue layer"。
2. **"开源模型 ≠ 可控模型"**。colibri 让本地跑大 MoE 更容易，heretic 让开源权重被进一步"解封"。两者组合意味着下一波"本地未审查大模型"会越来越普及——与同一天 Anthropic 更新 RSP 的监管收紧形成了明显的对冲。

Spotify 今天上榜（portal-ai-plugins）也是个有趣的信号：主流大公司开始为自己的平台铺 AI 插件入口，这类趋势还会继续放大。
