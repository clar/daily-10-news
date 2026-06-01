# GitHub Trending 每日榜 · 2026-06-02

## 今日焦点

> **AI 短视频流水线 · Agent 插件生态 · 开源 TTS 卷出新高 · "AI 设计反范式" · LLM 从零教学**
>
> - `harry0703/MoneyPrinterTurbo` 单日 +3,325⭐ 登顶涨速榜，AI 一键产出竖屏视频走入工业化。
> - `microsoft/markitdown` 单日 +3,086⭐ 仍在涨，是 LLM 文档预处理事实标准。
> - `OpenBMB/VoxCPM` 推出 2B 参数 + 30 语言 + 48kHz 的 tokenizer-free TTS，开源 TTS 卷进生产级。
> - `EveryInc/compound-engineering-plugin` 把 Claude Code / Cursor / Codex 都能用的"37 skill + 51 agent"打成插件。
> - `pbakaus/impeccable` 用 23 命令 + 27 反范式规则治"AI 设计模板病"，AI 工程外延到设计纪律。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [microsoft/markitdown](https://github.com/microsoft/markitdown) | Office/PDF/图片转 Markdown 给 LLM 用 | Python | 138,188 | +3,086⭐ | 9,415 |
| 2 | [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) | 一键生成高清 AI 短视频 | Python | 76,760 | +3,325⭐ | 10,890 |
| 3 | [TauricResearch/TradingAgents](https://github.com/TauricResearch/TradingAgents) | 多代理 LLM 金融交易框架 | Python | 81,720 | +284⭐ | 15,886 |
| 4 | [D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling) | 自适应反检测爬虫框架 | Python | 57,947 | +1,475⭐ | 5,625 |
| 5 | [codecrafters-io/build-your-own-x](https://github.com/codecrafters-io/build-your-own-x) | "从零造 X"经典教程合集 | Markdown | 510,345 | +1,194⭐ | 48,388 |
| 6 | [supermemoryai/supermemory](https://github.com/supermemoryai/supermemory) | 给 AI 应用的高速记忆引擎 | TypeScript | 23,923 | +660⭐ | 2,141 |
| 7 | [pbakaus/impeccable](https://github.com/pbakaus/impeccable) | AI 工具的设计反范式规则集 | JavaScript | 32,636 | +612⭐ | 1,779 |
| 8 | [nesquena/hermes-webui](https://github.com/nesquena/hermes-webui) | 自托管持续 Agent 的 Web UI | Python | 11,180 | +984⭐ | 1,447 |
| 9 | [godotengine/godot](https://github.com/godotengine/godot) | 跨平台 2D/3D 游戏引擎 | C++ | 111,613 | +121⭐ | 25,509 |
| 10 | [OpenBMB/VoxCPM](https://github.com/OpenBMB/VoxCPM) | 2B 参数 30 语言开源 TTS | Python | 24,178 | +880⭐ | 2,784 |
| 11 | [EveryInc/compound-engineering-plugin](https://github.com/EveryInc/compound-engineering-plugin) | Claude Code/Cursor 的复利工程插件 | TypeScript | 19,078 | +428⭐ | 1,428 |
| 12 | [can1357/oh-my-pi](https://github.com/can1357/oh-my-pi) | 终端 AI 编程代理（带 LSP） | TypeScript | 9,432 | +333⭐ | 759 |
| 13 | [revfactory/harness](https://github.com/revfactory/harness) | 设计领域专属代理团队的元框架 | HTML | 5,111 | +527⭐ | 687 |
| 14 | [FareedKhan-dev/train-llm-from-scratch](https://github.com/FareedKhan-dev/train-llm-from-scratch) | 从零训练 LLM 的可复制方法 | Notebook | 3,673 | +860⭐ | 514 |
| 15 | [dmtrKovalenko/fff](https://github.com/dmtrKovalenko/fff) | Rust 写的高性能文件搜索 | Rust | 7,143 | +121⭐ | 298 |

---

## 重点项目点评

### 🥇 [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) — 今日榜首，+3,325⭐

**AI 短视频流水线进入"按主题印钱"阶段**

MoneyPrinterTurbo 的口号实在直白：输入一个主题或关键词，AI 自动生成脚本、配音、字幕、背景音乐与素材，输出 9:16 竖屏 1080×1920 或 16:9 1920×1080 的高清视频。它支持 OpenAI / DeepSeek / Claude / Gemini / Ollama 多 LLM 后端，覆盖中英文双语 TTS，并提供 Docker、Colab、Windows 一键包多套部署方式。最新 v1.2.9（2026 年 5 月）把批量生成和 API 接口都做扎实。

它登顶涨速榜其实是 2026 年短视频运营生态的某种"工具民主化拐点"——以前需要团队三天的视频，被压成"提示词 → 渲染队列 → 上传"的几行 YAML，运营、小代理、个人 IP 都能搬入家用机房。负面解读则是：再过半年，社交平台的低质短视频供给会进一步过载，平台审核与"AI 生成标识"政策的压力会进一步上升。

---

### 🥈 [OpenBMB/VoxCPM](https://github.com/OpenBMB/VoxCPM) — +880⭐

**开源 TTS 进入"声音设计"时代：tokenizer-free + 30 语言 + 48kHz**

OpenBMB 的 VoxCPM2 是今天最值得收藏的 ML 项目。骨干基于 MiniCPM-4 的 2B 参数模型，训练数据超过 200 万小时多语种语音，输出 48kHz 工作室级音频。架构上采用 **tokenizer-free 端到端 diffusion autoregressive**——直接生成连续语音表示，跳过离散 token 这一步，自然度和韵律因此明显跃迁。

更关键的是它把"声音设计"做成了原生能力：仅凭文字描述就能创建新声线、可控的风格化克隆、以及给到参考音频与转写的"终极克隆"。基准上 Seed-TTS-eval 英文 WER 1.84%、普通话 CER 0.97%，CV3-eval 多语种成绩与 Fish Audio S2 相当甚至更优。配合自家 30 语言（含 9 种中文方言）支持，这是首个真正可以认真用在跨语种播客 / 教育 / 客服里的全开源模型。

---

### 🥉 [microsoft/markitdown](https://github.com/microsoft/markitdown) — +3,086⭐

**LLM 文档预处理的"管道事实标准"，连续 6 个月在榜**

138K 星的老牌仓库还在以日均 3K+ 的速度涨，说明 LLM 应用层的"输入侧"工程化需求一直在加深。MarkItDown 把 PDF / Word / PowerPoint / Excel / 图片 OCR / 音频转写 / YouTube / HTML / CSV / EPub / ZIP 全部统一转成 Markdown，"GPT-4o natively speaks Markdown"已成为这套架构的市场化共识。

它的护城河有两层：一是兼容微软 Azure 的文档理解与内容理解 API，企业落地路径短；二是 2700+ 个依赖项目让它在事实层面成为"喂 LLM 的预处理标准"。当今天 hermes / oh-my-pi / compound-engineering 这些 Agent 项目同台涨星时，markitdown 充当的就是它们的共同前置——这是工程上"在淘金热里卖铲子"的活样本。

---

### 🎖️ [EveryInc/compound-engineering-plugin](https://github.com/EveryInc/compound-engineering-plugin) — +428⭐

**"AI 工程"开始有方法论：37 个 skill + 51 个 agent**

EveryInc 把过去半年大家在 Claude Code / Cursor / Codex 上散乱积累的最佳实践，沉淀为一套统一的 plugin：`/ce-strategy` `/ce-brainstorm` `/ce-plan` 做规划，`/ce-work` `/ce-debug` 做执行，`/ce-code-review` `/ce-doc-review` 做多代理审查，`/ce-compound` 把团队学习沉淀回知识库，`/ce-product-pulse` 做产品级数据回顾。

核心理念叫 **"compound engineering"**：每一单元的工程工作都应该让后续工作更容易，而不是更难——为此 EveryInc 把 80% 时间分给规划与审查、20% 分给执行。这正是 Anthropic Dynamic Workflows 上线后行业急需的"应用层最佳实践模板"，也意味着 Cursor / Claude Code / Codex 这些 IDE 与 CLI 工具之间的"插件标准化"已经事实成型。

---

### 🎯 [pbakaus/impeccable](https://github.com/pbakaus/impeccable) — +612⭐

**给 AI 设计纪律的"反范式手册"**

Paul Bakaus（前 Google）基于 Anthropic 原生 frontend-design skill 改造而成的 impeccable，是今天最有"行业讽刺意味"的项目：它正面承认了 AI 生成 UI 普遍有"模板病"——一样的字体、紫色渐变、嵌套卡片、过气动效——并用 7 个领域参考（字体、色彩、空间、动效、交互、响应式、UX 文案）、23 条设计指令、27 条**确定性反范式规则**直接禁掉这些"AI 痕迹"。

工具同时兼容 Cursor / Claude Code / Gemini CLI 多家 harness，自带一个无需 API key 的 CLI 用来扫描设计问题。一句话：当代码生成已经卷到"加 plugin 提升 leverage"时，设计生成的卷法是"加 plugin 不让我看起来像 AI 写的"。

---

## 生态观察

- **AI 短视频 + AI 文档预处理同台涨星**：MoneyPrinterTurbo 与 markitdown 一日合计 +6,400 星，AI 应用层的"输入侧 + 输出侧"两条工程化主线都进入了产能爆发期。
- **Agent harness 插件化已成共识**：compound-engineering / hermes-webui / oh-my-pi / revfactory/harness 四个项目同框上榜，标志着 2026 年下半年的开发者工具，将围绕 Claude Code / Cursor / Codex 这几家 harness **构建标准插件生态**，而不是再发明新的 IDE。
- **TTS 一夜抢回话语权**：VoxCPM2 让国内开源 TTS 在多语种 + 工作室级音质上首次正面打过 Fish Audio、ElevenLabs 的开源版本，预计接下来两周会有大量 wrapper / hosting 跟进。
- **设计也开始"被规则化"**：impeccable 上榜显示开发者群体不再满足于"AI 写代码"，开始要求"AI 写出不像 AI 的代码与设计"，这是 AI 工程审美正在分化的早期信号。
- **学习曲线被填平**：build-your-own-x 与 train-llm-from-scratch 同框，意味着 2026 年的初学者门槛已经被压到"看仓库 + 跑 notebook 就能复刻一个 LLM 训练流水线"的程度。

一句话总结：**AI 工程从"造模型"全面转向"造工具链、造插件、造纪律"，今天的 trending 几乎是这条主线的一次清单式展示。**
