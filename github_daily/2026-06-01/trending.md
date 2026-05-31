# GitHub Trending 日报 · 2026-06-01

## 今日焦点

> **AI Agent 工程化继续狂飙 · 文档转换刚需工具霸榜 · 中文开源 TTS 出圈 · "造轮子学技术"再次封神 · 从零训练 LLM 的教学项目走红**
>
> - `microsoft/markitdown` +2,759⭐ 文件转 Markdown 工具登顶第二，仓库总星突破 13.4 万。
> - `harry0703/MoneyPrinterTurbo` +1,937⭐ AI 一键短视频生成稳居榜首。
> - `codecrafters-io/build-your-own-x` +1,112⭐ 总星超 50 万，仍在每日新增。
> - `OpenBMB/VoxCPM` +639⭐ 国产开源 TTS 多语种 + 真实音色克隆爆红。
> - `EveryInc/compound-engineering-plugin` +243⭐ 多 AI IDE 通用插件，承接 Claude Code / Cursor 工作流融合趋势。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) | AI 一键生成短视频 | Python | 74,029 | +1,937 | 10,567 |
| 2 | [microsoft/markitdown](https://github.com/microsoft/markitdown) | 文件/Office 转 Markdown | Python | 134,815 | +2,759 | 9,221 |
| 3 | [D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling) | 自适应 Web 爬虫框架 | Python | 56,547 | +639 | 5,482 |
| 4 | [nesquena/hermes-webui](https://github.com/nesquena/hermes-webui) | Hermes Agent 的 WebUI | Python | 9,906 | +320 | 1,366 |
| 5 | [EveryInc/compound-engineering-plugin](https://github.com/EveryInc/compound-engineering-plugin) | Claude Code/Codex/Cursor 共享插件 | TypeScript | 18,685 | +243 | 1,408 |
| 6 | [github/docs](https://github.com/github/docs) | GitHub 官方文档仓库 | TypeScript | 19,712 | +20 | 67,285 |
| 7 | [OpenBMB/VoxCPM](https://github.com/OpenBMB/VoxCPM) | 多语种零样本 TTS 与声音克隆 | Python | 23,440 | +639 | 2,711 |
| 8 | [revfactory/harness](https://github.com/revfactory/harness) | 设计领域专用 agent 团队的元 skill | HTML | 4,568 | +318 | 645 |
| 9 | [FareedKhan-dev/train-llm-from-scratch](https://github.com/FareedKhan-dev/train-llm-from-scratch) | 从零训练 LLM 教学 | Jupyter | 2,912 | +627 | 440 |
| 10 | [supermemoryai/supermemory](https://github.com/supermemoryai/supermemory) | AI 时代的记忆引擎/API | TypeScript | 23,293 | +236 | 2,100 |
| 11 | [Crosstalk-Solutions/project-nomad](https://github.com/Crosstalk-Solutions/project-nomad) | 离线生存型 AI 终端 | TypeScript | 27,695 | +372 | 2,710 |
| 12 | [anthropics/claude-code](https://github.com/anthropics/claude-code) | Anthropic 官方终端代理 | Python | 128,868 | +490 | 20,993 |
| 13 | [nicobailon/pi-subagents](https://github.com/nicobailon/pi-subagents) | Pi 异步 sub-agent 委派扩展 | TypeScript | 1,825 | +59 | 254 |
| 14 | [emmabostian/developer-portfolios](https://github.com/emmabostian/developer-portfolios) | 开发者作品集合集 | Python | 23,330 | +67 | 4,606 |
| 15 | [codecrafters-io/build-your-own-x](https://github.com/codecrafters-io/build-your-own-x) | 从零造常见技术 | Markdown | 509,339 | +1,112 | 48,309 |

---

## 重点项目点评

### 🥇 [microsoft/markitdown](https://github.com/microsoft/markitdown) — 今日榜首，+2,759⭐

**LLM 时代"文档喂模型"工具的事实标准**

markitdown 是微软维护的开源工具，把 PDF、Word、Excel、PowerPoint、HTML、音频、图像（含 OCR）一键转成 Markdown，专门为"投喂给 LLM"这个场景设计。今天 +2,759⭐、总数突破 13.4 万，这种持续高斜率的原因不在功能本身——开源界类似工具不少——而在它**和 Office 文档生态、AI 工作流的契合度**：企业的私有数据 80% 仍躺在 PPT/Word/Excel 里，把它们高质量转成 Markdown 等于打开 RAG 大门。

更值得注意的是 markitdown 的发布节奏：版本 0.x 时只支持寥寥几种格式，过去半年陆续加入了 Excel 公式保留、PowerPoint 母版识别、PDF 表格抽取等"难活"，几乎填齐了企业文档的最后一公里。当微软自己的 Copilot 都开始把 markitdown 当作默认上下文化工具时，它的标准化进程基本已成。

替代项目（unstructured、docling 等）质量都不差，但 markitdown 在"零依赖、纯 Python、单一 CLI"上的极简姿态，符合 AI 工程师"少装东西、多写 prompt"的偏好。这是 GitHub 上典型的"工具 + 时机"双赢。

---

### 🥈 [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) — +1,937⭐

**AI 短视频流水线的"标杆开源版"**

MoneyPrinterTurbo 把"输入一个主题 → LLM 生成脚本 → TTS 配音 → 自动剪辑素材 → 输出竖屏短视频"打包成一键流水线。今天 +1,937⭐，仓库已超 7.4 万。它没有任何模型上的创新，胜在**把所有商业短视频工厂的工作流抽象成 YAML 配置**，单 GPU 跑得动、文档支持中英双语，国内外创作者都能直接复用。

这类项目过去两年起起伏伏，但 MoneyPrinterTurbo 的差异化在于"对中文用户体验的死磕"：从中文 TTS、抖音/B 站尺寸预设、到字幕 Tail 时间轴的对齐，每个细节都对准中文创作者。它的爆红本质是：**"AI + 真实变现路径"** 在国内开源圈的吸引力远高于"AI + 学术演示"。

副作用是 issue 区充斥着"为什么生成的视频上不了首页"——这是创作者把工具当成"印钞机"的天然期待，开发者最近不得不在 README 顶部加了一行"本工具不保证商业成功"的免责声明。

---

### 🥉 [OpenBMB/VoxCPM](https://github.com/OpenBMB/VoxCPM) — +639⭐

**中文开源 TTS 进入"真实音色克隆 + 多语种"新阶段**

VoxCPM2 由清华系 OpenBMB 出品，主打 *tokenizer-free* 架构、多语种零样本 TTS、创意声音设计（"模仿一个有点感冒的女主播"这类描述即可）、真实音色克隆。今天 +639⭐，热度集中在 demo 视频被 X/小红书转发后的二次扩散。

技术上的卖点是 tokenizer-free——避开传统语音 token 的离散误差，直接在连续表征上建模，这是 2025 年下半年 TTS 学术圈的共识方向（Seed-TTS、F5-TTS 都在这条线上）。商业上的关键是**许可证清晰、可本地部署**，给独立创作者和教育公司提供了"不依赖 ElevenLabs"的选项。

VoxCPM 的走红佐证了一个趋势：开源 TTS 在 2026 年正在以肉眼可见的速度逼近闭源天花板，"做播客 / 视频 / 有声书的工具链彻底本地化"已经触手可及。

---

### 4️⃣ [FareedKhan-dev/train-llm-from-scratch](https://github.com/FareedKhan-dev/train-llm-from-scratch) — +627⭐

**"教你训一个能用的 LLM"，Jupyter 教育项目的复兴**

这是一个 Jupyter Notebook 形式的教学仓库，从数据下载、tokenizer、Transformer 实现到训练循环、生成代码全程手写。基础参考 nanoGPT / GPT-NeoX，但定位是"门外汉到能跑出生成结果"。今天 +627⭐，是教学类项目里少见的高斜率。

它的意义在于：**当所有人都在用 Hugging Face 和 OpenAI API 时，第一性原理仍然有市场**。许多 2024-2025 入行 AI 的工程师从未真正跑过一次完整的预训练循环，对 attention/optimization 只有 API 级理解；这类教程把"从零跑通"压缩到一台 24GB 卡，几乎是 AI 工程师再教育的最佳门票。

它的对照组是 #15 的 build-your-own-x（+1,112⭐、总星 50 万+）——两个项目都在告诉社区一个事实：**重复造轮子是程序员最稳定的学习路径**，再多 AI 工具也无法替代手敲一遍。

---

### 5️⃣ [EveryInc/compound-engineering-plugin](https://github.com/EveryInc/compound-engineering-plugin) — +243⭐

**Claude Code/Codex/Cursor 共享插件：Agent IDE 生态融合开始了**

EveryInc 出的 compound-engineering-plugin 是少见的"一份插件、多 Agent IDE 共用"的尝试，明确支持 Claude Code、Codex（OpenAI）、Cursor 和"more"。它把 Compound Engineering 理念（多 Agent 协同完成软件工程任务）打包成 skill 集合，给每家 IDE 提供一致的工具调用接口。

今天 +243⭐ 看起来不高，但战略意义被低估——这是 GitHub 上第一个公开喊出"Agent IDE 应该有跨厂商插件标准"的成熟项目，跟 Anthropic 主推的 MCP（Model Context Protocol）形成事实上的应用层试点。Codex 上周开始支持 MCP，Cursor 早就是 MCP 重度用户，Claude Code 本身就是 MCP 的发起方。当三家 Agent 形态产品都接入同一份 plugin spec 时，Agent IDE 生态正式从"各立山头"走向"接口统一"。

下一步关键看 JetBrains、Replit Agent、Windsurf 等会不会加入这套规范。

---

## 生态观察

今天的 Trending 拼起来是 2026 年 AI 工程化的一张缩影：

**第一，"AI 数据流水线"工具持续霸榜**。markitdown（文档转 MD）、Scrapling（爬虫）、MoneyPrinterTurbo（视频生成）、VoxCPM（语音生成）、supermemory（记忆引擎）——AI 时代真正大规模盈利的工具，不是模型本身，而是把数据"喂入/喂出"模型的管道。今天前 10 里 6 个都属于这一类。

**第二，Agent 生态的接口标准化在加速**。compound-engineering-plugin、pi-subagents、revfactory/harness（设计 agent 团队的元 skill）共同指向同一个未来：未来 Agent 不再是"哪家 IDE 的专属"，而是按 skill / capability 跨平台流通。MCP 是底层协议、这些项目是应用层标准。

**第三，"中文开源 AI"的国际能见度仍在上升**。MoneyPrinterTurbo、VoxCPM、claude-code（中文文档质量爆表）三个项目今日都进了前 12，说明 GitHub Trending 早已是中英文双向流动的市场——"开源出海"不再需要刻意为之，做得够好的项目自然会被全球开发者发现。

**第四，"造轮子学习"的反复回潮**。build-your-own-x 总星 50 万+、仍每天 +1,112，train-llm-from-scratch 单日 +627——在 AI 工具越来越多的语境下，社区反而更愿意为"亲手实现"的教学投票。这是对"AI 替代基础理解"焦虑的集体回应。
