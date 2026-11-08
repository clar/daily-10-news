# GitHub Trending 每日报告 · 2026-11-09

## 今日焦点

> **Agent 基础设施全面开源 · OSINT 工具再登顶 · 设计系统也要"agent ready" · 消费级 GPU 推理栈 · 上下文压缩成为刚需**
>
> - `sherlock-project/sherlock` 今日 +2,372⭐，老牌 OSINT 社工工具再次出圈，用户名跨站匹配成为 AI 时代刚需。
> - `milind-soni/OpenMausBot` 今日 +1,437⭐，开源版的 Grok Bot——给 AI 代理挂一台虚拟机，让它"真正会用电脑"。
> - `meta/astryx` 今日 +863⭐，Meta 开源的"面向 Agent 的设计系统"，组件默认附 JSON Schema、行为契约和 UI 指令。
> - `vercel-labs/agent-browser` 今日 +812⭐，Rust 写的 CLI 级浏览器自动化工具，直接给 Claude/GPT/Gemini 的 computer use 当引擎。
> - `ranxianglei/billion-context` 今日 +460⭐，长会话的"上下文压缩插件"，用小模型做 token 回缩，适配 8k/32k 窗口。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [sherlock-project/sherlock](https://github.com/sherlock-project/sherlock) | 按用户名跨社交网络定位账号 | Python | 103,296 | +2,372⭐ | — |
| 2 | [milind-soni/OpenMausBot](https://github.com/milind-soni/OpenMausBot) | 开源 Grok Bot 替代，含虚拟机 | TypeScript | 18,161 | +1,437⭐ | — |
| 3 | [meta/astryx](https://github.com/meta/astryx) | 可定制、面向 Agent 的开源设计系统 | TypeScript | 16,505 | +863⭐ | — |
| 4 | [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) | 面向 AI 代理的浏览器自动化 CLI | Rust | 47,534 | +812⭐ | — |
| 5 | [anthropics/skills](https://github.com/anthropics/skills) | Agent Skills 公共仓库 | Python | 189,563 | +793⭐ | — |
| 6 | [ranxianglei/billion-context](https://github.com/ranxianglei/billion-context) | 小上下文窗口下的长会话压缩插件 | TypeScript | 5,092 | +460⭐ | — |
| 7 | [dsx-ai-factory/nvke](https://github.com/dsx-ai-factory/nvke) | NVIDIA 裸金属 GPU 的 K8s 管理面 | Go | 819 | +345⭐ | — |
| 8 | [anthropics/claude-quickstarts](https://github.com/anthropics/claude-quickstarts) | Claude API 快速起步项目集 | Python | 19,379 | +28⭐ | — |
| 9 | [google-deepmind/mujoco](https://github.com/google-deepmind/mujoco) | 多关节动力学 + 接触物理仿真器 | C++ | 16,367 | +26⭐ | — |

> 备注：今日 GitHub trending 主页仅显示 9 条，OSSInsight 后端自 2026-03 起捕获率下降至约 0.3%，无法作为补充口径——保留现有名单。

---

## 重点项目点评

### 🥇 [sherlock-project/sherlock](https://github.com/sherlock-project/sherlock) — +2,372⭐

**OSINT 老将再出山，背后是 AI 代理时代的"身份扩散"焦虑**

sherlock 作为 OSINT（开源情报）领域的常青树，核心功能是输入一个用户名，自动跨 400+ 社交网络检索匹配账号。它的核心逻辑没有大变，但最近两周被大量 AI 代理项目重新集成——Claude、Perplexity、ChatGPT Agent 乃至开源 LangGraph 工作流都把 sherlock 当作"身份聚合"的入口工具。

此时登顶的意义，在于 AI 让"身份扩散"的问题前所未有地严重：同一用户名可能在 50 个平台出现，每个平台的头像、简介、发帖都可能是 AI 生成。sherlock 成了"反 AI 泛滥"的最后一张手工网，也是合规团队做尽调的首选起点。

工程亮点在增量稳健性——500+ 社交平台的探测模板由社区维护，稳定率在近三个月显著提升。对红队、新闻记者、企业风控都是零成本接入的工具。

---

### 🥈 [milind-soni/OpenMausBot](https://github.com/milind-soni/OpenMausBot) — +1,437⭐

**"给 Agent 一台真正的电脑"：开源 Grok Bot 的追赶战**

OpenMausBot 的卖点非常简单：一个可以挂载 VM/浏览器/文件系统/Shell 的 agent 容器，让任何 LLM 都能像 Grok Bot、ChatGPT Agent、Claude Computer Use 那样"真的操作一台电脑"。它用 TypeScript 实现，内置了 QEMU/Firecracker 两套 VM 后端，支持挂载任意 MCP 工具。

这个项目爆火对应的是闭源阵营的集体收紧——Grok 对 Bot 功能加了额度门槛、Anthropic 的 computer use 价格较高、OpenAI 的 Agent 仍在 waitlist。开源社区用一套"自己托管 VM + 自己接 LLM"的方案把成本打到底。

更深层的信号是：Agent 的技术护城河从模型下移到执行环境。谁掌握最轻、最安全、最可审计的沙盒，谁就控制 Agent 的下一代入口。OpenMausBot 的热度直接呼应了这条趋势。

---

### 🥉 [meta/astryx](https://github.com/meta/astryx) — +863⭐

**第一套明确以"Agent-ready"为设计目标的开源设计系统**

astryx 在组件库之外，为每个组件暴露了机器可读的"行为契约"（JSON Schema + 自然语言说明），使 LLM 代理可以精确地知道"按钮能做什么、输入框接受什么、页面状态有哪几种"。Meta 把它直接开源，意味着对 2027 年的 web 竞争格局已经有新的押注：**每个页面都是 Agent 可读的接口**，而不是过去 25 年人机交互的"视觉 + DOM"二元组合。

astryx 的技术实现并不惊艳——TypeScript + React + 少量 Design Token DSL——但示范效应巨大：MUI、Radix、Shopify Polaris、Ant Design 都需要在 2027 年给出自己的"agent-ready 版本"。

---

### 🏅 [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) — +812⭐

**浏览器自动化的新一代标准品：Rust 内核 + Agent 原生 API**

Vercel Labs 用 Rust 重写了"面向 AI 代理的浏览器自动化 CLI"——不是另一个 Playwright/Puppeteer，而是直接把 Claude computer use、Gemini Computer Control、Mistral Operator 的调用协议以 First-Class 方式实现。它消除了"screenshot → OCR → action"的中间层，直接走"DOM + Vision"双通道 + 原生 anti-fingerprint。

对开发者的意义是"写一次，在三家 LLM 上都能跑"。对生态的意义是——Vercel 把 web 自动化赛道从一个"开源基础设施"升级成"闭源 LLM 的协议接入层"，这也是为什么这个项目能和 OpenMausBot 并排登榜。

---

### 📦 [ranxianglei/billion-context](https://github.com/ranxianglei/billion-context) — +460⭐

**Context 压缩插件 —— 不是显卡买不起，而是上下文用不起**

billion-context 的定位相当精巧：在 8k/32k 小上下文模型里塞下近乎无限的会话历史。原理是"小模型做总结 + 事实提取 + 分层压缩"，再在合适时机"按需展开"。它直接对接 Ollama、llama.cpp、LM Studio、Claude Desktop MCP 等本地推理方案。

爆火的原因有两条：其一，今天榜一 HN 帖"Llama-modchip 把 284B DeepSeek 跑在 64GB 内存"让"本地推理 + 小上下文"成为真正的生产组合；其二，Anthropic/OpenAI/Google 的 token 单价仍在高位，长会话场景下 Token 成本甚至超过电费。

项目的工程创新是支持"Session Delta"——每次压缩只重新计算改变的部分；这让 10 万轮的 chat history 可以稳定在 2k-4k 的工作 token 内维持语义连贯。

---

## 生态观察

今天的 GitHub Trending 结构性地显示一件事：**2026 年末的开源热度已经全面转向"Agent 栈"**。

- 执行层：`OpenMausBot`（VM 沙盒）、`vercel-labs/agent-browser`（浏览器）、`dsx-ai-factory/nvke`（K8s GPU 调度）——Agent 需要的三类基础设施同时涌现。
- 协议层：`anthropics/skills`（Agent Skills）、`meta/astryx`（agent-ready UI）——从"API 调工具"升级为"产品原生面向 Agent"。
- 认知层：`billion-context`（上下文压缩）、`anthropics/claude-quickstarts`（Agent 应用骨架）——补齐长会话、长记忆、长决策的工程缺口。
- 情报层：`sherlock-project/sherlock` 再登顶，说明"AI 可以生成一切、但身份关联仍要人工 OSINT"的辩证关系依旧成立。

一周前的 trending 还有不少传统基础设施（数据库、ORM、框架），今天几乎全部被 Agent 工具替换。这是"Agent 工业化"从实验室走向生产系统的最明显信号。
