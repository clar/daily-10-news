# GitHub Trending 每日热榜 · 2026-07-16

## 今日焦点

> **Claude Code Skill 生态爆发 · 反 AI slop 设计浪潮 · 交易 Agent 抢镜 · 开源 CapCut 冲刺 · 安全护栏工具走红**
>
> - `mattpocock/skills` +2,160⭐，Matt Pocock 直接把 `.claude` 目录甩出来当训练指南
> - `OpenCut-app/OpenCut` +1,505⭐，开源 CapCut 替代品破 71k
> - `Shubhamsaboo/awesome-llm-apps` +1,278⭐，100+ Agent/RAG 应用集合稳居 topN
> - `Nutlope/hallmark` +1,119⭐，"反 AI slop 设计"技能包一天冲上 8.3k 星
> - `HKUDS/Vibe-Trading` +924⭐，港科大团队推出"氛围交易" Personal Trading Agent

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [mattpocock/skills](https://github.com/mattpocock/skills) | Skills for Real Engineers，直接来自作者 .claude 目录 | Shell | 172,187 | +2,160 | 14,786 |
| 2 | [OpenCut-app/OpenCut](https://github.com/OpenCut-app/OpenCut) | 开源 CapCut 替代品 | TypeScript | 71,490 | +1,505 | 7,332 |
| 3 | [Shubhamsaboo/awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) | 100+ Agent 与 RAG 应用集合 | Python | 121,849 | +1,278 | 17,989 |
| 4 | [Nutlope/hallmark](https://github.com/Nutlope/hallmark) | 反 AI slop 的 Claude Code / Cursor / Codex 设计 skill | CSS | 8,313 | +1,119 | 434 |
| 5 | [hasaneyldrm/exercises-dataset](https://github.com/hasaneyldrm/exercises-dataset) | 1,324 项健身动作数据集，带动画与多语言 | HTML | 14,314 | +951 | 1,717 |
| 6 | [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) | 氛围式个人交易 Agent | Python | 23,636 | +924 | 4,030 |
| 7 | [HenryNdubuaku/maths-cs-ai-compendium](https://github.com/HenryNdubuaku/maths-cs-ai-compendium) | 面向 AI/ML 研究工程师的学习地图 | TypeScript | 5,856 | +729 | 739 |
| 8 | [Dicklesworthstone/destructive_command_guard](https://github.com/Dicklesworthstone/destructive_command_guard) | 阻断 Agent 执行危险 git/shell 命令的 Rust 护栏 | Rust | 4,744 | +497 | 178 |
| 9 | [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | 面向 Claude Code 的营销技能包 | JavaScript | 39,705 | +390 | 6,314 |
| 10 | [openinterpreter/openinterpreter](https://github.com/openinterpreter/openinterpreter) | 面向低成本模型的代码 Agent | Rust | 65,427 | +345 | 5,651 |
| 11 | [moeru-ai/airi](https://github.com/moeru-ai/airi) | 自托管 AI 陪伴，含实时语音与游戏能力 | TypeScript | 42,471 | +144 | 4,249 |
| 12 | [HKUDS/DeepTutor](https://github.com/HKUDS/DeepTutor) | DeepTutor：长期个性化辅导 | Python | 26,223 | +128 | 3,560 |
| 13 | [YimMenu/YimMenuV2](https://github.com/YimMenu/YimMenuV2) | GTA5 Enhanced 实验菜单 | C++ | 1,408 | +21 | 354 |

---

## 重点项目点评

### 🥇 [mattpocock/skills](https://github.com/mattpocock/skills) — 今日榜首，+2,160⭐

**Matt Pocock 把 .claude/skills 直接开源，宣示"skill 已经是新的 README"。**

Matt Pocock（TypeScript 社区教育者）把自己日常使用的 Claude Code skill 全部同步出来，覆盖 TypeScript 严格模式重构、单元测试脚手架、Storybook 修复、type-narrowing 教学等 30 多项技能。这不仅是"分享 dotfile"，更是把"AI 工程师如何使用 AI"的最佳实践写成可运行的产物。

trend 侧的意义在于：Claude Code 4.7+ 支持项目级 skill 后，仓库 star 数已经开始类似 README 的辐射效应——好用的 skill 集合会像 awesome-list 一样被 fork、被派生。Matt 这套的价值在于 opinionated：他直接把"我如何写 TypeScript"变成 skill 定义，比通用型 skill 更能改变协作体验。

反面观察：评论区已经出现"skill 泛滥怎么办"的担忧。Anthropic 尚未提供 skill 依赖管理，一旦一个仓库跑 30+ skill，Claude 的可用 context 就要挤压。

---

### 🥈 [Nutlope/hallmark](https://github.com/Nutlope/hallmark) — +1,119⭐

**"反 AI slop"变成一个独立赛道。**

Hassan（Nutlope）是"用 AI 快速做产品"的代表人物，这次却发布了一个反向工具：hallmark 是一个 skill 包，专门告诉 Claude Code / Cursor / Codex "什么样的 UI 是 AI slop（一眼可辨的机器味）"，并提供反例设计参考。核心内容包含 Tailwind 反 slop 主题、"避免 generic gradient hero"的规范、以及一份 "AI 常犯的 20 种设计错误"清单。

这条 trend 折射的是社区共识的转向——AI 生成 UI 一年前是效率红利，现在变成了辨识度陷阱。用户开始能一眼识别 v0/Bolt/Lovable 生成的默认样式；Hassan 用 skill 的形式把"设计品味"注入 Agent 工作流，比在系统提示里堆规则更精准。

后续可以关注："反 slop"是否会向后端代码扩展——反 slop TypeScript、反 slop SQL 都有市场空间。

---

### 🥉 [OpenCut-app/OpenCut](https://github.com/OpenCut-app/OpenCut) — +1,505⭐

**开源 CapCut：Adobe 焦虑与短视频 UGC 洪流的产物。**

OpenCut 是 TypeScript + FFmpeg WASM + WebGPU 实现的桌面级视频剪辑器，对标字节跳动 CapCut。今天新增 1.5k 星，累计 71k，是本季度增长最快的桌面工具之一。核心卖点是"离线优先 + AI 特效可插拔"，用户可以接入本地大模型完成字幕生成、镜头对齐、B-roll 推荐。

社区选它的理由有二：（1）CapCut 上个月对海外免费用户限速引发反弹；（2）Adobe Premiere 与 Final Cut 的价格墙让个人创作者流失。OpenCut 把"AI 剪辑"标准化成插件市场，既可以接 Whisper 做字幕，也可以接 Runway Gen-5 API 做补帧。

风险：视频剪辑器天然是 GPU 与体验密集型工具，OpenCut 若不能在 60fps 时间线上稳定运行，会像早年 Kdenlive 一样被人爱戴但被少人使用。未来 3 个月是它的关键窗口。

---

### 4️⃣ [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) — +924⭐

**港科大的"氛围交易"Agent：模型 + 交易 + 情绪信号闭环。**

港科大数据智能实验室（HKUDS）继上月 DeepTutor 之后再度上榜。Vibe-Trading 定义了一个"个人量化 Agent"框架：拉取新闻、社群情绪、K 线、宏观事件，用 LLM 生成策略假设，再交由回测引擎裁决，最后调用券商 API 下单。仓库同时开源了 5 组基准策略（比特币趋势、美股财报事件、A 股北向、加密永续套利、外汇短周期）。

trend 意义在于——散户量化的"科研化"。以前是"我买了 Trading View 会员写 Pine Script"，现在是"我 fork 一个学术级 Agent 框架"。这也让 IB、盈透、Alpaca 这类 API 券商更加重要。

隐含风险：README 明确写了不承担合规责任，但实际操作里，港美股监管对 AI 决策记录的追溯将成为新雷区。

---

### 5️⃣ [Dicklesworthstone/destructive_command_guard](https://github.com/Dicklesworthstone/destructive_command_guard) — +497⭐

**AI Agent 时代的"防挖坟"护栏。**

Dicklesworthstone 上个月因 llm-context-router 项目走红，这次的 dcg（Destructive Command Guard）是一个 Rust 单文件小工具，钩住 Claude Code / Codex / Aider 等 Agent 的 shell 执行入口，拦截 `rm -rf`、`git push --force`、`chown -R /` 之类操作，并根据规则文件做二次确认或直接阻断。

这类工具的出现说明 AI Agent 已经进入"真的会写破坏性命令"的阶段。过去一年多次爆出的 Cursor 误删仓库、Aider 意外 hard-reset 的事故，让 destructive guard 从可选项变成必备。dcg 的差异化在于 Rust 单二进制 + 300 行规则 DSL，比 Docker 沙盒更轻量，比 shell alias 更稳。

如果 Claude Code 官方内建同类护栏，这类第三方工具会被边缘化——但在过渡期，dcg 已经找到了一批"高价值 Agent 用户"。

---

## 生态观察

**Claude Skill 已经从"实验特性"变成"社区语言"。** 今日 top15 里有 4 个 skill 相关仓库（`mattpocock/skills`、`Nutlope/hallmark`、`coreyhaines31/marketingskills` 还有 `destructive_command_guard` 也带 Claude Code 集成）。这条赛道的产品化速度可能超出 Anthropic 官方预期，接下来关注 skill 的分发市场与依赖机制。

**"反 AI slop"是新的品味信号。** Hallmark 的爆红说明：只要"AI 味"变成负面标签，围绕"审美防御"的工具就有市场。这个模式可以迁移到文档写作、前端命名、产品文案。

**Agent × 领域"融合期开启。"** Vibe-Trading（交易）、DeepTutor（教育）、marketingskills（营销）出现在同一天前 10，说明"垂直 Agent"从概念走向可用。共同特点：领域数据 + skill 定义 + 反馈闭环，缺一不可。

**Rust 在护栏 / 系统层继续吃份额。** destructive_command_guard 与 openinterpreter 都用 Rust。当 AI 侧 Python 依然占大头时，"围绕 AI 的边界工具"正在被 Rust 蚕食。

**中国团队学术出品加速：** HKUDS 一天两项目上榜（Vibe-Trading + DeepTutor），是继 THUML、SJTU-IIPL 之后的又一支高频输出团队，值得中长线关注。
