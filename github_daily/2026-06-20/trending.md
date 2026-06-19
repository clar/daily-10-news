# GitHub Trending 日报 · 2026-06-20

## 今日焦点

> **Agentic 工具继续洗榜 · 时序基础模型 · Token 压缩 · 视频 AI · 中国开源 (GLM-5) 杀回赛道**
>
> - `chopratejas/headroom` 一日 +3,938⭐，把 RAG / 日志 / 工具输出压缩 60-95% 再喂给 LLM，2026 年的"省 Token"赛道之王。
> - `google-research/timesfm` 一日 +1,516⭐，时间序列基础模型重回热度榜，预示企业预测领域的 LLM 化拐点。
> - `obra/superpowers` 一日 +1,113⭐，已 23 万⭐的 agentic skills 框架仍在被 Claude Code / Codex 用户疯狂 star。
> - `DeusData/codebase-memory-mcp` 一日 +1,055⭐，C 语言实现的高性能代码索引 MCP，专为"代码代理记忆"打造。
> - `zai-org/GLM-5` 一日 +478⭐，智谱新一代模型仓库，主打"vibe coding → agentic engineering"叙事。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [chopratejas/headroom](https://github.com/chopratejas/headroom) | 压缩工具/日志/RAG 输入，省 60-95% Token | Python | 38,486 | +3,938 | 2,622 |
| 2 | [google-research/timesfm](https://github.com/google-research/timesfm) | Google 时间序列基础模型 | Python | 24,052 | +1,516 | 2,269 |
| 3 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic skills 框架 & 软件开发方法论 | Shell | 233,298 | +1,113 | 20,721 |
| 4 | [DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) | 高性能代码索引 MCP，持久化知识图谱 | C | 8,150 | +1,055 | 623 |
| 5 | [palmier-io/palmier-pro](https://github.com/palmier-io/palmier-pro) | macOS 上的 AI 原生视频剪辑器 | Swift | 1,816 | +749 | 183 |
| 6 | [zai-org/GLM-5](https://github.com/zai-org/GLM-5) | 智谱 GLM-5，主打 agentic engineering | — | 4,543 | +478 | 460 |
| 7 | [n0-computer/iroh](https://github.com/n0-computer/iroh) | Rust 写的模块化 P2P 网络栈 | Rust | 10,240 | +307 | 466 |
| 8 | [withastro/flue](https://github.com/withastro/flue) | 沙箱式代理框架 | TypeScript | 5,814 | +305 | 323 |
| 9 | [koala73/worldmonitor](https://github.com/koala73/worldmonitor) | AI 驱动的全球新闻 / 地缘监控仪表盘 | TypeScript | 57,194 | +300 | 9,135 |
| 10 | [Kong/insomnia](https://github.com/Kong/insomnia) | 开源跨平台 API 客户端 | TypeScript | 38,955 | +291 | 2,300 |
| 11 | [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) | 开源 agentic 视频生产系统 | Python | 6,234 | +236 | 1,078 |
| 12 | [penpot/penpot](https://github.com/penpot/penpot) | 开源设计 / 代码协作工具 | Clojure | 50,563 | +213 | 3,268 |
| 13 | [BuilderIO/agent-native](https://github.com/BuilderIO/agent-native) | Agent 原生应用框架 | TypeScript | 1,009 | +210 | 116 |
| 14 | [Lightricks/LTX-2](https://github.com/Lightricks/LTX-2) | LTX-2 音视频生成模型推理 / LoRA 训练 | Python | 7,657 | +196 | 1,220 |
| 15 | [aishwaryanr/awesome-generative-ai-guide](https://github.com/aishwaryanr/awesome-generative-ai-guide) | 生成式 AI 学习 / 面试资源大全 | HTML | 27,592 | +155 | 5,738 |

---

## 重点项目点评

### 🥇 [chopratejas/headroom](https://github.com/chopratejas/headroom) — 今日榜首，+3,938⭐

**省 Token 是 2026 年 AI 工程的隐形战场**

`headroom` 是一个专门用来"压缩进入 LLM 上下文的内容"的工具：把工具输出 (日志、文件 dump、shell 输出、RAG chunk) 在送进模型之前压缩 60-95%。它针对的痛点几乎所有 Claude Code / Codex / Continue 用户都熟：context 一不小心就被 build log、grep 结果、API 响应撑爆。Headroom 用一组语言学 + 结构化 heuristics + 自适应模型对长尾输出做"信息密度提取"，并保留可恢复性。

一天 +3,938⭐的爆发证明两件事：(1) 即便有 200k-1M context 的前沿模型，**实际生产里的 token 成本 + 信号噪音问题没有被解决**，大家依然需要中间层降本；(2) Anthropic 上周宣布的 Claude Cowork 限额翻倍只是缓兵之计，真正高频用户会去找下沉一层的工具方案。

这个仓库今天能登顶，反映了 2026 年 AI 应用层的核心矛盾——更长的 context 反而催生了"更激进的压缩"。

---

### 🥈 [google-research/timesfm](https://github.com/google-research/timesfm) — +1,516⭐

**时间序列基础模型迎来"GPT 时刻"**

Google Research 的 TimesFM 是一个针对时间序列预测的 foundation model，2024 年首发，但今天能再涨 1.5k+ ⭐ 显然不是巧合。最近一周企业级 AI 圈大量讨论"为什么我们还在用 ARIMA"——业界发现 TimesFM v2 / v2.5 在零样本预测里已经能击败传统的 Prophet 和 LightGBM。

更深层的信号是：金融、电网、零售、广告四个领域今年都在认真考虑"用基础模型替换内部时序栈"，TimesFM 几乎是唯一一个有 Google 训练资源 + 开源协议 + 真实部署案例的选择。当 Anthropic 在韩国签三星 SDS、当 OpenAI 收 Astral 时，Google 这条"开源科研牌"反而在企业市场默默积累 star。

---

### 🥉 [obra/superpowers](https://github.com/obra/superpowers) — +1,113⭐

**已经 23 万⭐的 agentic skills 框架仍未达到顶**

`superpowers` 是 Jesse Vincent 维护的"agentic skills"集合，定位是给 Claude Code / Codex 这类 CLI agent 提供"可复用、可组合、可分发"的高阶能力。23 万 ⭐ 已经把它推到 GitHub 上"开发者工具开源项目"前 20 名级别，但今天还在涨 1k+，意味着这个项目的"飞轮"还没停。

为什么继续涨？两点：(1) Anthropic 上周给所有 Claude Cowork 用户翻倍限额，**直接催生了"工具开发"的边际收益**；(2) `superpowers` 是少数同时支持 Claude / Codex / Cursor / Continue 的跨厂商 skill 标准，是事实上的"agent 应用商店"。

---

### 💾 [DeusData/codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp) — +1,055⭐

**代码记忆变成 agent 标配**

这是一个 C 语言实现的高性能 MCP 服务器：把代码库索引成持久化知识图谱，让 LLM agent 能跨会话记住"这个 monorepo 的架构"、"这个函数的调用链"、"这个 PR 改了什么"。一天涨 1k+ ⭐ 反映了 MCP 生态正在从"标准定义阶段"进入"刚需工具阶段"。

值得注意的是它用 C 而不是 Python/TS——这个语言选择本身就是信号：当 MCP server 要服务大型 monorepo (TB 级)，性能和内存占用开始成为差异化指标。如果你听说今天 Claude Code 的 Sonnet 4.6 在企业里"明显比上个月聪明"，背后多半是这种持久化记忆 MCP 的功劳。

---

### 🇨🇳 [zai-org/GLM-5](https://github.com/zai-org/GLM-5) — +478⭐

**智谱的 GLM-5：从 vibe coding 到 agentic engineering**

智谱 (Z.ai) 今天开 GLM-5 的官方仓库，slogan 直接打出"From Vibe Coding to Agentic Engineering"——明显对标 Claude Code / Codex 的"agent 工程师"叙事。仓库本身的 478⭐ 不算爆，但要放在背景里看：今天 MiniMax 也在借 Fable 5 出口管制做"开源权重不会被召回"的营销，**中国开源 AI 模型正在抓住地缘窗口集中输出**。

GLM-5 主打三件事：极长 context、agentic loop 原生支持、本地推理友好。如果接下来几周 Fable 5 仍然没法完全解禁，亚太市场会有相当一部分开发者主动尝试 GLM-5 + 自托管 MCP 的组合。

---

## 生态观察

今天的 GitHub Trending 几乎是 **「Agent 工业化」** 的横截面：5 个 agent / skill / MCP 相关仓库 (headroom、superpowers、codebase-memory-mcp、agent-native、flue) 同时挤进前 10，这是过去 6 个月里 agent 主题密度最高的一天。

第二条线：**视频 AI 在 GitHub 上找到了入口**——`palmier-pro` (macOS AI 视频剪辑) + `OpenMontage` (开源 agentic 视频流水线) + `LTX-2` (开源音视频生成) 三个项目同日上榜，表明 2026 年下半年视频 agent 的工具化拐点已经到来。

第三条线：**国产开源加速**。`GLM-5` 仓库的出现配合最近 MiniMax M3、Qwen3.5、DeepSeek V4 的密集更新，明显是中国厂商在用"开源权重不可召回"的叙事抢全球开发者心智。结合 Anthropic Fable 5 出口管制事件，这股势头很可能在 6-9 月持续放大。

最后一条值得记的反向信号：今天**没有任何一个新 Web 前端框架登顶**。Svelte、Solid、Qwik 这些 2024-2025 年的常客全部缺席，整个榜单都在围绕"AI 工程基础设施"，这是 GitHub 生态过去三年最明显的一次"AI native 全面碾压"。
