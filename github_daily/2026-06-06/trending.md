# GitHub Trending 每日报告 · 2026-06-06

## 今日焦点

> **Agent 框架持续屠榜 · Token 压缩成新刚需 · NotebookLM 开源平替 · NVIDIA 押注物理 AI · OCR 数据预处理回归视野**
>
> - `chopratejas/headroom` 单日 +2,503⭐ 暴涨，60-95% token 压缩成 Agent 工程刚需
> - `NousResearch/hermes-agent` 18.3 万星霸榜，"会成长的 Agent" 概念吃尽眼球
> - `lfnovo/open-notebook` +1,142⭐，NotebookLM 的开源克隆持续累积关注
> - `NVIDIA/cosmos` +494⭐，物理 AI 世界模型基础设施开始抢开发者
> - `PaddleOCR` +755⭐，AI 系统的"喂料管道"重新成为热门基建

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [chopratejas/headroom](https://github.com/chopratejas/headroom) | 60-95% token 压缩中间件，写在 LLM 调用前 | Python | 14,451 | +2,503⭐ | 918 |
| 2 | [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) | "会成长的 Agent"，开源持续学习框架 | Python | 183,033 | +1,821⭐ | 31,387 |
| 3 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Agent 框架性能优化系统，含 skills & memory | JavaScript | 208,306 | +1,368⭐ | 31,959 |
| 4 | [lfnovo/open-notebook](https://github.com/lfnovo/open-notebook) | 开源 NotebookLM，强化灵活性与功能 | TypeScript | 25,950 | +1,142⭐ | 2,988 |
| 5 | [PaddlePaddle/PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR) | 轻量 OCR，PDF/图像转结构化数据喂 AI | Python | 80,508 | +755⭐ | 10,631 |
| 6 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 多平台研究 + 接地气总结的 AI Skill | Python | 28,177 | +738⭐ | 2,390 |
| 7 | [NVIDIA/cosmos](https://github.com/NVIDIA/cosmos) | 世界模型开放平台，物理 AI 基础设施 | Jupyter | 9,387 | +494⭐ | 600 |
| 8 | [CopilotKit/CopilotKit](https://github.com/CopilotKit/CopilotKit) | Agent 与生成式 UI 的前端栈 | TypeScript | 32,635 | +350⭐ | 4,189 |
| 9 | [openclaw/openclaw-windows-node](https://github.com/openclaw/openclaw-windows-node) | OpenClaw Windows 系统托盘 + PowerToys 集成 | C# | 1,590 | +329⭐ | 180 |
| 10 | [666ghj/MiroFish](https://github.com/666ghj/MiroFish) | 通用群体智能引擎，号称"什么都能预测" | Python | 64,664 | +324⭐ | 10,083 |
| 11 | [MemPalace/mempalace](https://github.com/MemPalace/mempalace) | 开源 AI 记忆系统，benchmark 最强免费方案 | Python | 53,848 | +228⭐ | 7,079 |
| 12 | [aquasecurity/trivy](https://github.com/aquasecurity/trivy) | 容器/代码/云环境的漏洞扫描器 | Go | 35,840 | +208⭐ | 443 |
| 13 | [Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach) | Agent 跨 Twitter/Reddit/YouTube/GitHub 检索 | Python | 21,515 | +127⭐ | 1,861 |
| 14 | [withastro/flue](https://github.com/withastro/flue) | "沙盒式" Agent 框架 | TypeScript | 4,495 | +126⭐ | 241 |
| 15 | [openai/plugins](https://github.com/openai/plugins) | OpenAI Plugins 框架 | JavaScript | 1,510 | +82⭐ | 238 |

---

## 重点项目点评

### 🥇 [chopratejas/headroom](https://github.com/chopratejas/headroom) — 今日榜首，+2,503⭐

**Agent 工程师终于承认：token 不是算力问题，是工程问题**

Headroom 把自己定位成"LLM 调用之前的压缩中间件"——把 tool output、log、context history 在送进模型前**砍掉 60-95% token**，业务侧无感知。这种"看似平庸"的工具能单日吸 2500 颗星，说明一个朴素现实：**Agent 跑起来 90% 成本不是推理本身，是 context 反复重塑的开销**。Anthropic 这周还在公布 Claude Opus 4.8 已经支持 100 万 token 上下文，但开发者用脚投票——"我宁可花一周做压缩，也不愿付一周的 token 账单"。

Headroom 的火爆完美契合本周 HN 焦点：当 ChatGPT Dreaming V3 把记忆做成可演化、Anthropic 的 Glasswing 给企业供 100 万 token、Microsoft Scout 长期驻留——所有这些都在**把 context 膨胀压力转嫁给开发者**。Headroom 就是开发者反击的方式：在 prompt 与模型之间加一层"语义压缩 + 日志剪枝"。

这种工具属于典型的"基础设施红利"——一旦确立默认地位，整个 Agent 生态都会绕它建立。Cline、Cursor、Claude Code 等下游迟早要么集成它要么 fork 它。

---

### 🥈 [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) — +1,821⭐

**Nous 把"会成长的 Agent"做成元 narrative，开源派的旗手回归**

Hermes 系列一直是开源 LLM 圈最有 narrative 张力的项目，本次发布的 hermes-agent 主打**"陪你成长"**——一套面向个人开发者的持续学习 Agent 框架，能在每次交互后做 fine-tune-lite 的偏好积累。18.3 万星基础上单日 +1,821 ⭐，说明社区在寻找 Anthropic / OpenAI 的"持久化"叙事之外的开源对照物。

这条路线之所以现在火起来，是因为 ChatGPT Dreaming V3、Claude Mythos、Microsoft Scout 三家都在做"AI 在工作流中常驻"——但全是闭源、全是订阅、全是数据上交。Hermes Agent 给出反命题：**"持久 Agent 应该跑在你自己机器、用你自己模型、记忆归你自己"**。这种叙事对开发者群体的吸引力，远大于任何企业版功能。

注意它的 31,387 fork 数——这是 hermes-agent 真正的护城河，开源持续学习一旦能形成 commit 生态，会比单纯的模型权重更难追上。

---

### 🥉 [lfnovo/open-notebook](https://github.com/lfnovo/open-notebook) — +1,142⭐

**NotebookLM 平替持续累积关注：Google 的"知识工作"心智正在被开源切走**

Google NotebookLM 用一年时间把"上传几份资料 → 问答 + 生成播客摘要"做成了一个标志性 AI 产品类别。open-notebook 是其完整开源平替，强调**多模型可切换、本地存储、可控数据出境**。+1,142⭐ 看似不爆炸，但持续 7 天保持在 Trending 前 5 是更强信号——说明这不是 hype，是"NotebookLM 商业版被锁在 Workspace 里"的反噬。

值得关注的是它和 Microsoft Scout、ChatGPT Sites（直接输出托管交互站）、Claude Mythos 同一周登上 HN——**"AI 知识容器"已成为 2026 年的核心产品形态**。NotebookLM 给了用户 demo，Scout 给了企业入口，open-notebook 给了"我要自己掌控"的那批人选择权。

对个人和小团队的意义：这是 2026 年首选的"个人知识管理 + AI" 起手仓库。

---

### 🚀 [NVIDIA/cosmos](https://github.com/NVIDIA/cosmos) — +494⭐

**NVIDIA 抢"物理 AI" 开发者心智：CUDA 之后的下一道护城河**

Cosmos 是 NVIDIA 押注的"世界模型平台"——给机器人、自动驾驶、工业仿真等**Physical AI**应用提供基础设施。+494⭐ 在巨头项目里不算极端，但意义在于**NVIDIA 终于把 World Model 从 demo / 论文层下放到可使用的 SDK 层**。配合本周 NVIDIA Computex 发布的 RTX Spark Arm 超级芯片，"边缘端 + 物理 AI"的硬件 + 软件双 stack 正在闭环。

DeepSeek 4 月发布的 V4 也提到"agentic abilities"，但仍然停留在数字世界；NVIDIA 选择跳出 LLM 文字 / 代码竞赛，直接卡位"AI 控制物理世界"赛道——**这是它从 GPU 厂转向 AI 计算平台公司的关键举措**。开源 Cosmos 等于在邀请整个机器人 / 自动驾驶生态把世界模型托管在 NVIDIA 标准之上。

短期内 Cosmos 不会火得像 Hermes，但 18 个月后回头看，今天 +494 星可能是 NVIDIA 物理 AI 帝国的起点。

---

### 🛡️ [PaddlePaddle/PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR) — +755⭐

**老牌 OCR 项目重新被发现：AI 工作流的"喂料管道"被严重低估**

PaddleOCR 总星 8 万的成熟项目突然单日 +755⭐ 上榜，原因不是它有新版本，而是 **AI 大爆发之后开发者发现"输入数据"才是真正的瓶颈**——你的 Agent 再强，喂进去的还是 PDF / 截图 / 工单图片，不能结构化就没法用。Headroom 解决"出门前压缩"，PaddleOCR 解决"进门前提取"，两个项目同日上榜不是巧合。

这条线索的更大背景是 OCR 已经从"独立模块"变成"RAG / Agent 的第一公里"。MIT 本周发的 ChartNet 数据集（100 万合成图表）专门训练图表理解，也是同一个动作——**所有人都在补"非结构化数据 → 模型可用 token"的转换层**。中国系开源在这块（百度、阿里、MinerU 等）几乎垄断了 Trending 榜单。

对工程团队的意义：当你下游用 Claude Code、Codex 加速代码生成时，上游真正的护城河往往就在 OCR / parsing / chunking 这种"看着无聊"的地方。

---

## 生态观察

**主线一：Agent 框架已经从"如何写一个 Agent" 进化到 "如何让 Agent 跑得便宜、记得住、用得久"**。今日 Trending 一半项目（Hermes、ECC、CopilotKit、flue、Agent-Reach、headroom、MemPalace、last30days-skill）都在解决同一件事——**Agent 全栈的非模型部分**：context 压缩、记忆持久化、跨平台检索、UI 渲染、生命周期管理。模型本身已经不再是 GitHub Trending 的兴奋点。

**主线二：开源"持久化 AI" 派与闭源巨头正面对决**。本周 OpenAI 推 Dreaming V3、Microsoft Scout、Anthropic Glasswing、Claude Opus 4.8 全部主打"驻留 + 长记忆"，开源端则用 hermes-agent、mempalace、open-notebook 给出**"数据归你自己"**的反命题。这场战争未来 12 个月会决定个人开发者是订阅 ChatGPT/Claude 还是自托管 Agent。

**主线三：物理 AI 与边缘端开始出现独立赛道**。NVIDIA Cosmos + RTX Spark Arm 芯片 + Adobe 重写 Photoshop 原生支持 ARM——**整个生态正在从"云端 GPU 推理"转向"端侧多核 + 物理交互"**，这是 2026 下半年最值得长期跟踪的方向。

**主线四：基础设施类项目（OCR、漏扫、压缩）正在乘 AI 之风重启增长**。PaddleOCR、headroom、Trivy 同日上榜——AI 越热，底层"数据预处理 + 调用经济性 + 安全审计"越值钱。**Build the picks and shovels** 在 2026 仍然有效。
