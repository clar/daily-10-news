# GitHub Trending 日报 · 2026-06-14

## 今日焦点

> **AI Agent Skills 生态 · Claude Code 工具链 · Apple Silicon 容器化 · KV Cache 加速 · 老牌仓库长青**
>
> - `addyosmani/agent-skills` 单日 +1,507⭐——"agent skills 工程化"成显学，Addy 的 production-grade 范本被开发者奉为参考。
> - `obra/superpowers` +931⭐，22.6 万总星——agentic skills framework 持续扩散，开发方法论已经从博客文走向工程仓库。
> - `apple/container` +1,471⭐——Apple Silicon 原生容器化方案正式成为 Mac 开发者的 Docker 替代选项。
> - `NVIDIA/SkillSpector` +809⭐——NVIDIA 亲自下场做 AI agent skills 的安全扫描，生态出现安全工具层。
> - `LMCache/LMCache` +246⭐——KV Cache 优化层进入 vLLM 之外的工程主流视野，本地推理性价比战在持续。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [iptv-org/iptv](https://github.com/iptv-org/iptv) | 全球公开 IPTV 频道聚合 | TypeScript | 119,002 | +650 | 6,363 |
| 2 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 生产级 AI agent 工程能力集 | Shell | 58,270 | +1,507 | 6,291 |
| 3 | [chatwoot/chatwoot](https://github.com/chatwoot/chatwoot) | 开源 omni-channel 客服平台 | Ruby | 30,822 | +86 | 7,553 |
| 4 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic skills 框架与开发方法论 | Shell | 226,883 | +931 | 20,173 |
| 5 | [apple/container](https://github.com/apple/container) | Apple Silicon 原生 Linux 容器 | Swift | 36,239 | +1,471 | 1,033 |
| 6 | [music-assistant/server](https://github.com/music-assistant/server) | 开源音乐流媒体聚合器 | Python | 1,989 | +277 | 429 |
| 7 | [kenn-io/agentsview](https://github.com/kenn-io/agentsview) | Local-first 编程 agent 会话分析 | Go | 2,337 | +187 | 215 |
| 8 | [LMCache/LMCache](https://github.com/LMCache/LMCache) | LLM 推理 KV Cache 加速层 | Python | 8,868 | +246 | 1,303 |
| 9 | [microsoft/PowerToys](https://github.com/microsoft/PowerToys) | Windows 生产力工具集 | C | 134,648 | +374 | 8,078 |
| 10 | [andrewyng/aisuite](https://github.com/andrewyng/aisuite) | 多模型统一 SDK | Python | 14,083 | +132 | 1,487 |
| 11 | [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) | AI agent skills 安全扫描 | Python | 4,377 | +809 | 331 |
| 12 | [bannedbook/fanqiang](https://github.com/bannedbook/fanqiang) | 科学上网工具集 | Kotlin | 47,468 | +86 | 8,079 |
| 13 | [swc-project/swc](https://github.com/swc-project/swc) | Rust 实现的前端编译平台 | Rust | 33,624 | +12 | 1,398 |
| 14 | [x1xhlol/system-prompts-and-models-of-ai-tools](https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools) | 主流 AI 工具系统提示词集 | — | 140,288 | +107 | 34,655 |

---

## 重点项目点评

### 🥇 [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — 今日榜首，+1,507⭐

**Addy Osmani 把"agent skills 工程化"做成了开发者的入门教材**

Addy Osmani（Chrome 团队、《Learning JavaScript Design Patterns》作者）把过去半年在 Claude Code / Cursor / Codex 上沉淀的 agent skills 整理成生产级仓库——内含 60+ 经过实战验证的 skill 定义，覆盖代码审查、安全扫描、PR 总结、API 文档生成、回归测试等场景，并附带每个 skill 的 prompt schema、触发条件和失败兜底策略。

这个仓库今天蹿升的速度（24h 内 +1,507⭐，逼近 6 万总星）说明 agent skills 已经从"博客上玄学传播"过渡到了"工程化复用"。这恰好与今日 HN 上的本地 AI 工作站讨论形成共振——开发者不仅在压缩成本，也在沉淀复用模式，而 Addy 的仓库给出了一份"production checklist"。

值得注意的是文件结构和命名直接对齐了 Claude Code 的 `.claude/skills/` 目录约定，意味着这套规范已经在事实上成为社区标准。

---

### 🥈 [apple/container](https://github.com/apple/container) — +1,471⭐

**Apple Silicon 原生容器，正式终结 Docker Desktop 的统治期**

Apple 自家开源仓库 `container` 提供基于 Apple Silicon 优化的轻量虚拟机方案，专门用于在 Mac 上跑 Linux 容器，单日 +1,471⭐说明 Mac 开发者群体在等这个工具等很久了。它不是 Docker 的薄壳替代，而是利用 macOS 的 Virtualization.framework 直接调度 ARM 原生镜像，启动速度、内存占用、CPU 调度都明显优于 Docker Desktop。

更关键的是它把 OCI 镜像、containerd 兼容、网络命名空间这些底层组件做完了，并提供 CLI `container run` 直接对齐 Docker UX——意味着团队迁移成本几乎为零。对正在为 Docker Desktop 订阅费用纠结的中小团队，这个仓库实际上提供了一条"零迁移成本 + 性能更好"的路径。

Apple 把它放出来也是有姿态意义的——继 Swift on Server、Xcode Cloud 之后，Apple 在开发者基础设施层的开源步伐明显加快，目标是 Mac 不再"只是设计师笔记本"，而要承担云原生开发的本地端工作流。

---

### 🥉 [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) — +809⭐

**NVIDIA 给 AI agent skills 装上安全扫描层**

SkillSpector 是 NVIDIA 内部安全团队释出的工具，专门扫描 AI agent skills（YAML / Markdown / shell 脚本组合）中的漏洞、prompt injection 路径与恶意模式。考虑到 NVIDIA 自身在 NeMo / NIM agent 产品线投入巨大，把"skills security"这层做成开源工具显然是想推动行业建立扫描标准——这跟当年 Bandit / Semgrep 出现的时机有相似味道。

它能识别的几类问题：(a) skill 中调用外部 webhook 时未做域名白名单；(b) 系统命令拼接里存在用户输入注入；(c) Skill 间能力越权（高权限 skill 被低信任度 skill 调用）；(d) 已被社区 flag 过的恶意 skill 指纹。

它的出现说明 agent skills 生态已经走过了"野蛮生长"，下一阶段是合规与供应链安全。配合上面 Addy 的仓库——一个负责标准化、一个负责审计——agent skills 的工程范式雏形基本完成。

---

### 🏅 [obra/superpowers](https://github.com/obra/superpowers) — +931⭐

**22.6 万总星的方法论仓库继续扩散**

obra (Jesse Vincent，Anthropic Claude Code 核心开发者) 的 superpowers 仓库总星已突破 22 万，今天再 +931⭐。这个仓库本质上是"如何用 Claude Code / agent 写软件"的工程手册——包含 skill 规范、agent prompt patterns、failure mode catalog、tooling 接入指南。

它的扩散意义在于：把 Anthropic 内部的工程实践公开化，让 Claude Code 用户可以站在官方人员的肩膀上调优自己的 agent 工作流。今天的 +931⭐ 主要来自 Addy 仓库被引用 + HN 与 Twitter 端的二级传播——大家在比较"两份 agent skills 圣经"。

可以预见，未来 6 个月内 agent skills 仓库会经历一次"明星收敛"过程，社区会围绕 1-2 份事实标准重组——目前看 obra 与 addyosmani 两位是首选。

---

### 🏅 [LMCache/LMCache](https://github.com/LMCache/LMCache) — +246⭐

**KV Cache 层进入 vLLM 之外的工程主流**

LMCache 是 UChicago 团队孵化的 KV Cache 加速层，可以与 vLLM、SGLang、TensorRT-LLM 等推理引擎插拔配合，宣称在长上下文 + 多轮对话场景下吞吐能提升 3-7×。今日新增 246⭐，叠加昨日热度，已经突破 8.8K 总星。

它的意义在于：本地 LLM 部署正在分化——上层模型由 GLM 5.2 / Qwen 3.6 / DeepSeek-V4 等开源大模型承担，中层有 vLLM / SGLang 等推理引擎，下层则需要 KV Cache、量化、PagedAttention 这类基础设施。LMCache 出现填补了"多轮对话缓存复用"的工程空白——对本地 AI 编程工作站这种 prompt 反复填充 context 的场景尤其有用。

这与昨日 HN 上"AI coding at home"和 RTX 5080+3090 跑 Qwen 3.6 的话题再次构成生态闭环——开源大模型、推理引擎、缓存层、agent skills 已经在围绕 Claude Code 的对立面拼成一套完整栈。

---

## 生态观察

今日 trending 三大主轴清晰：**Agent skills 工程化**（Addy、obra、SkillSpector、agentsview 同时上榜）、**本地 / Mac 开发栈复兴**（apple/container、LMCache、aisuite）、以及**老牌仓库长青**（iptv-org、PowerToys、swc、chatwoot 长期上榜）。

"Agent skills" 已经从去年概念阶段进入工业化阶段——开源标准、安全工具、会话观测三层都开始出现。从 Addy 仓库今天 +1,507⭐ 的速度看，开发者正在从被动消费 Claude Code 文档转向主动建立自己的 skill 库；NVIDIA 把安全审计工具开源，则给整套生态加上了进入企业管线的合规凭证。

值得留意的是今天 trending 里**几乎没有新的 LLM 推理大模型本体仓库**——上周 Qwen 3.6、Kimi K2.7-Code、GLM 5.2 的释出热度已经被消化。市场注意力正在向"如何用好这些模型"的工具链层迁移，这是 2026 下半年 GitHub 生态最值得关注的拐点。
