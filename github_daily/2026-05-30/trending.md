# GitHub Trending 日报 · 2026-05-30

## 今日焦点

> **AI Skill 生态爆发 · Claude Code 插件化 · 文档解析回归 Rust · AI 短视频产线工具化 · 全平台 Agent harness 成为底层基础设施**
>
> - `harry0703/MoneyPrinterTurbo` 一键 AI 短视频生成器 +3,563⭐，今日新增第一。
> - `Leonxlnx/taste-skill` 反"AI 味"风格 Skill +2,066⭐，提示词工程进入"反生成感"阶段。
> - `microsoft/markitdown` 文档转 Markdown 工具 +1,876⭐，老项目继续吸流量。
> - `EveryInc/compound-engineering-plugin` 多 IDE Agent 协作插件 +354⭐，Claude Code/Cursor/Codex 同框已成默认。
> - `run-llama/liteparse` Rust 写的开源 PDF 解析 +680⭐，LlamaIndex 主推的新一代解析底座。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) | LLM 一键生成短视频 | Python | 69,521 | +3,563 | 10,021 |
| 2 | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | 反"AI 风味"的提示 Skill | Shell | 28,050 | +2,066 | 2,079 |
| 3 | [microsoft/markitdown](https://github.com/microsoft/markitdown) | 文件/Office 转 Markdown | Python | 129,827 | +1,876 | 8,909 |
| 4 | [byoungd/English-level-up-tips](https://github.com/byoungd/English-level-up-tips) | 进阶英语学习指南 | Various | 49,615 | +1,564 | 5,196 |
| 5 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Agent harness 性能优化平台 | JavaScript | 198,535 | +1,413 | 30,505 |
| 6 | [DigitalPlatDev/FreeDomain](https://github.com/DigitalPlatDev/FreeDomain) | 免费域名注册服务 | HTML | 171,711 | +1,317 | 3,340 |
| 7 | [run-llama/liteparse](https://github.com/run-llama/liteparse) | 快速开源文档解析（Rust） | Rust | 7,223 | +680 | 441 |
| 8 | [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop) | 去除 AI 化味道的写作技能 | Various | 6,950 | +618 | 490 |
| 9 | [twentyhq/twenty](https://github.com/twentyhq/twenty) | 开源 AI 原生 CRM（Salesforce 替代） | TypeScript | 48,378 | +575 | 6,859 |
| 10 | [anthropics/claude-code](https://github.com/anthropics/claude-code) | 终端原生的 agentic 编码工具 | Python | 127,839 | +460 | 20,907 |
| 11 | [EveryInc/compound-engineering-plugin](https://github.com/EveryInc/compound-engineering-plugin) | 多 IDE Agent 协作官方插件 | TypeScript | 18,111 | +354 | 1,376 |
| 12 | [galilai-group/stable-worldmodel](https://github.com/galilai-group/stable-worldmodel) | 可复现的 world model 研究平台 | Python | 1,225 | +346 | 148 |
| 13 | [Crosstalk-Solutions/project-nomad](https://github.com/Crosstalk-Solutions/project-nomad) | 离线生存式 AI 计算机 | TypeScript | 26,927 | +294 | 2,653 |
| 14 | [cursor/plugins](https://github.com/cursor/plugins) | Cursor 官方插件规范 + 实现 | TypeScript | 1,279 | +129 | 108 |
| 15 | [Biohub/esm](https://github.com/Biohub/esm) | 生物序列建模研究 | Jupyter | 2,557 | +64 | 313 |

---

## 重点项目点评

### 🥇 [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) — 今日榜首，+3,563⭐

**AI 短视频"印钞机"再起势，自动化内容产线进入工程化阶段**

MoneyPrinterTurbo 不是新项目（2024 年首发），但今天突然单日吸 3.5K 星，背后明显有内容创作者社群的二次推广。它的卖点是"一句话 → 文案 → TTS → BGM → 字幕 → 拼接 → 输出"全链路自动化，本地化封装得很彻底（中文 TTS / 中文 prompt / B 站 / 抖音模板）。

这次它再次冲榜的原因不是功能升级，而是大量 YouTube/抖音内容创作者在新一轮"AI 内容工厂"教学视频里把它当默认推荐。结合 The Verge 同日 Shift 那篇"扫地换数据"的报道一起看，**2026 年的 AI 内容生态正在加速分层**：底层是模型，中层是工具链（MoneyPrinterTurbo 这类一键产线），顶层是"刷量+变现"——这条产业链跑通后，"内容是否由人产出"已经不再是市场首要关注点。

---

### 🥈 [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) — +2,066⭐

**"反 AI 味"成为提示词工程的下一个战场**

taste-skill 是一个面向 Claude / GPT / Gemini 的 Skill 包，核心功能是"让你的 AI 输出不像 AI 生成的"——通过约束 prompt 模板（避免 em-dash、避免空洞副词、避免列表罗列、避免 "delve" / "navigate" / "in the realm of"）和示范风格样本对模型施加风格压力。

这类工具其实从 2024 年就有，但今年第一次冲上 GitHub trending，原因是"反 AI 味"在内容工作流上的实际收入差距越来越大——SEO、博客、newsletter、商务邮件都开始被算法/读者标记"AI 化"内容并惩罚。今天另一个上榜项目 `hardikpandya/stop-slop` 与它形成完美对照——两个项目背靠的是同一种焦虑：**LLM 已经会写、但写得太像彼此**。下一步看的是这类 Skill 能否被吸收进 Claude / OpenAI 官方的风格控制 API。

---

### 🥉 [run-llama/liteparse](https://github.com/run-llama/liteparse) — +680⭐

**LlamaIndex 用 Rust 重写文档解析底座**

liteparse 是 LlamaIndex 团队的最新作品，定位是"快、准、开源"的 PDF / Office / 网页解析器，目标客户是所有用 RAG / 文档问答 / Agent 的人。技术选型很有意思——Rust 写核心、Python 提供绑定——这是 2024-2026 年 AI infra 的稳定趋势：Pydantic v2、tokenizers、tiktoken-rs、surrealdb、qdrant 全部走这条路。

把它和今日榜上的 microsoft/markitdown（+1,876）放一起看，整个"文档→结构化文本"赛道还在加速。markitdown 是工程级 polish 的产物，liteparse 是 LlamaIndex 这种 RAG 框架公司的战略护城河。**Agent 工具链的下一段红利在哪里？答：从模型转向数据预处理。** 这是过去三个月所有 Y Combinator AI 项目共同的结论。

---

### 🛠️ [EveryInc/compound-engineering-plugin](https://github.com/EveryInc/compound-engineering-plugin) — +354⭐

**Claude Code / Codex / Cursor 同框，"多 IDE 协作 Agent"进入插件化阶段**

Every 团队（Dan Shipper 的 Every / Substack 系媒体公司）做的官方 compound engineering 插件，把"多 agent 在不同 IDE 里协同工作"的工作流抽象成可装载的 plugin。支持 Claude Code、Codex、Cursor，本质是在标准化"agent → agent"的协议层。

这件事的信号意义大于代码本身：**插件化是 IDE Agent 生态走向成熟的标志**。Cursor 今天也上榜了它的官方插件 spec（[cursor/plugins](https://github.com/cursor/plugins)）。一旦 plugin spec 形成共识，Agent 与 IDE 的耦合会显著松动，开发者可以"换 IDE 不换 agent，换模型不换 workflow"，这是 Claude Code、Cursor、Codex 三足鼎立期最重要的中间层基础设施竞争。

---

### 🌍 [galilai-group/stable-worldmodel](https://github.com/galilai-group/stable-worldmodel) — +346⭐

**世界模型从论文走向"可复现研究框架"**

stable-worldmodel 把 World Model 研究做成了类似 stable-baselines3 那样的开箱即用平台——统一的环境接口、训练循环、评估指标，目标是让世界模型这种之前主要在 DeepMind/Sakana/AI Habitat 等机构内部能跑的研究范式，普通研究组也能上手。

它的趋势意义在于：**WorldModel 在 2026 年第一次出现"基础设施化"信号**。过去两年大家关心的是 Genie 2、SIMA、V-JEPA 这些大公司的 demo；今年开始研究侧需要一个"小框架统一所有方法"的工具——和 2018 年 Stable Baselines、2020 年 HuggingFace Transformers 出现时的市场需求结构高度相似。如果世界模型真的成为 robot foundation model 的核心范式（参考今天 AI 日报里 Rhoda AI 的 FutureVision），这类基础设施会在 2027 年成为兵家必争。

---

## 生态观察

**Skill / 插件化成为今日主线**：taste-skill、stop-slop、compound-engineering-plugin、cursor/plugins、claude-code、liteparse 全部围绕"工具/插件/Skill 抽象"展开——2026 年 GitHub trending 已经从"模型仓库"完全转向"模型周边生态"。

**"反 AI 味"是新的提示词工程**：两个直接相关的 Skill 项目同日上榜（taste-skill + stop-slop），加上 stable-worldmodel 的"风格统一"——AI 输出的同质化已经被开发者社区当成一个工程问题来解决。

**Rust 在 AI infra 的占位继续扩大**：liteparse 是今天唯一的 Rust trending 项目，但站位关键（RAG 数据预处理基础设施）。Python 仍是 AI 工程师入口语言，但底层"快 + 正确"层全面 Rust 化的趋势在持续。

**Agent harness 进入工业级竞争**：affaan-m/ECC 这种"agent harness 性能优化平台"出现在榜单上，说明"agent 系统的可观测/可调优"已经从 dev tool 变成产品类目。这条线值得后续追踪。

---

*报告日期：2026-05-30（北京时间） | 数据来源：github.com/trending*
