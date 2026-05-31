# GitHub Trending 日报 · 2026-05-31

## 今日焦点

> **文档→Markdown 管道再爆 · Agent harness 与 Plugin 生态扩张 · 多模态生成（视频/语音/世界模型）· Rust 解析栈崛起 · 离线生存知识箱**
>
> - `microsoft/markitdown` 单日 **+2,470⭐**：Office/PDF/PPT/音频统一转 Markdown，仍是 LLM 上下文清洗的事实标准
> - `harry0703/MoneyPrinterTurbo` 今日 **+2,768⭐**：AI 短视频自动化生成霸榜
> - `anthropics/claude-code` 仓库累计 **128k⭐**：今日继续吸金 +592，agent CLI 工具的"长尾刚性需求"
> - `OpenBMB/VoxCPM` +779⭐：tokenizer-free TTS，2B 模型覆盖 30 语言 + 9 中文方言
> - `run-llama/liteparse` +925⭐：Rust 写的本地文档解析器，无 LLM 无云依赖

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [microsoft/markitdown](https://github.com/microsoft/markitdown) | 把 Office/PDF/图片/音频统一转 Markdown 喂 LLM | Python | 132,614 | +2,470 | 9,076 |
| 2 | [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) | AI 自动生成高清短视频 | Python | 72,146 | +2,768 | 10,340 |
| 3 | [anthropics/claude-code](https://github.com/anthropics/claude-code) | 终端里的 agentic 编码助手 | Python | 128,433 | +592 | 20,954 |
| 4 | [cursor/plugins](https://github.com/cursor/plugins) | Cursor 插件规范与官方插件 | TypeScript | 1,475 | +205 | 118 |
| 5 | [revfactory/harness](https://github.com/revfactory/harness) | 设计领域专用 agent 团队的元-skill | HTML | 4,291 | +55 | 628 |
| 6 | [EveryInc/compound-engineering-plugin](https://github.com/EveryInc/compound-engineering-plugin) | 跨多个 coding 助手的 Compound Engineering 插件 | TypeScript | 18,444 | +349 | 1,393 |
| 7 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Agent harness 性能优化与安全 skills | JavaScript | 199,404 | +908 | 30,616 |
| 8 | [OpenBMB/VoxCPM](https://github.com/OpenBMB/VoxCPM) | tokenizer-free 多语 TTS + 声音克隆 | Python | 22,816 | +779 | 2,673 |
| 9 | [galilai-group/stable-worldmodel](https://github.com/galilai-group/stable-worldmodel) | 可复现世界模型研究与评测平台 | Python | 1,473 | +318 | 166 |
| 10 | [Crosstalk-Solutions/project-nomad](https://github.com/Crosstalk-Solutions/project-nomad) | 离线生存"知识 + AI"计算机 | TypeScript | 27,385 | +469 | 2,686 |
| 11 | [run-llama/liteparse](https://github.com/run-llama/liteparse) | 本地化文档解析，无 LLM 无云 | Rust | 7,941 | +925 | 467 |
| 12 | [chen08209/FlClash](https://github.com/chen08209/FlClash) | 跨平台 ClashMeta 代理客户端 | Dart | 40,399 | +187 | 2,527 |
| 13 | [FareedKhan-dev/train-llm-from-scratch](https://github.com/FareedKhan-dev/train-llm-from-scratch) | 从下载数据到生成文本的 LLM 训练全流程 | Jupyter | 2,318 | +327 | 375 |
| 14 | [ruvnet/RuView](https://github.com/ruvnet/RuView) | WiFi 信号转空间感知/生命体征 | Rust | 68,971 | +655 | 9,201 |
| 15 | [DataTalksClub/data-engineering-zoomcamp](https://github.com/DataTalksClub/data-engineering-zoomcamp) | 免费 9 周数据工程实战课程 | Jupyter | 41,797 | +274 | 8,286 |

---

## 重点项目点评

### 🥇 [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) — 今日 +2,768⭐

**"一键变现"叙事仍在 2026 年继续奏效**

MoneyPrinterTurbo 已经在 GitHub Trending 上"长青"两年多，每次大型模型升级都能再涨一波星。其逻辑非常简单：输入主题 → LLM 生成脚本 → 调 TTS → 自动剪辑 + B-roll + 字幕，一条 60 秒短视频在 5 分钟内出炉。**今天再次冲榜的原因，几乎可以肯定与 VoxCPM 同期发布的高质量多方言 TTS 直接相关**——一个负责生成、一个负责发声，两个开源仓库形成了完整工具链。

它从来不是"严肃 AI 项目"，但它精准命中"用 AI 赚 quick money"的内容侧需求。作为开发者，可以把它当作"短视频自动化的最小可工作样板"——架构粗糙，但每个环节都可替换。

---

### 🥈 [microsoft/markitdown](https://github.com/microsoft/markitdown) — 今日 +2,470⭐

**LLM 时代的 textract：把"业务知识"喂进上下文窗的标准管线**

微软把"任意文档 → 干净 Markdown"做成一个 Python 工具，今日新增 2.4k⭐，仓库总数突破 13.2 万。覆盖 PDF / Word / Excel / PPT / 图片 / 音频，可选挂 Azure Document Intelligence 提升结构化抽取质量。模块化安装（按格式装依赖）和插件架构让它实际成为"个人/企业知识库前置预处理"的事实标准。

它今天再爆，与 RAG 应用普及到中小企业有关：当一家 50 人公司决定"内部把 Confluence + 共享盘喂给 Claude"时，markitdown 几乎是默认选项。**从生态位看，它和 [run-llama/liteparse](https://github.com/run-llama/liteparse) 形成"上层 LLM-optimized vs 底层 spatial-preserving"两条互补路径**——后者也在今日 trending 榜上 +925⭐。

---

### 🥉 [OpenBMB/VoxCPM](https://github.com/OpenBMB/VoxCPM) — 今日 +779⭐

**Tokenizer-free TTS 把"逼真度"再推一档**

VoxCPM2 是清华-面壁智能 OpenBMB 推出的 2B 参数 TTS 模型，最大创新点是**抛弃离散 token 化**，直接在 AudioVAE V2 的潜空间内做端到端 diffusion + autoregressive 生成，原生 48 kHz 输出。覆盖 30 种语言 + 粤语、四川话等 9 种中文方言；提供 voice design（用文本描述造声音）和 ultimate cloning（参考音 + 转写复刻细微嗓音）。

这条线在 2026 年的开源 TTS 赛道是非常硬的存在：**Tokenizer-free 意味着 expressiveness 上限被打开**，比离散 token 派（VITS / GPT-SoVITS）能输出更细微的呼吸、笑声、情绪起伏。配合上面 MoneyPrinterTurbo 之类的下游应用，"开源中文短视频内容工厂"的最后一块短板正在被补齐。

---

### 4️⃣ [run-llama/liteparse](https://github.com/run-llama/liteparse) — 今日 +925⭐

**Rust 写的本地解析器：当"云依赖"成了 RAG 的 P0 风险**

LiteParse 出自 LlamaIndex 团队，定位与 LlamaParse（云服务）互补：**完全本地、Rust 实现、保留 bounding box 的高质量 PDF/DOCX/XLSX/PPTX/图片解析**。底层用 PDFium、Tesseract（可换 EasyOCR/PaddleOCR）、LibreOffice、ImageMagick；上层提供 Python (PyO3)、Node (napi-rs)、WebAssembly 三套绑定。

它今日爆发反映了一个真实趋势：**2026 年企业 RAG 越来越警惕"把所有 PDF 上传给 SaaS 解析"的合规风险**——金融、医疗、政府客户希望"解析 + 嵌入 + 检索"全链路本地化。LiteParse 是 LlamaIndex 的"主权方案对冲"。

---

### 5️⃣ [Crosstalk-Solutions/project-nomad](https://github.com/Crosstalk-Solutions/project-nomad) — 今日 +469⭐

**"离线生存计算机"：当 AI 不连网也要能用**

Project Nomad 是一个完全离线、自给自足的"生存知识箱"：本地塞入 Wikipedia 离线版、医学手册、地图、急救文档，加上一个本地推理的小模型（通常是 Qwen/Llama 系），所有内容打包到一台树莓派或迷你 PC。今日 +469⭐，反映出 **2026 年"AI 主权 + 灾备"叙事的下沉**——从企业的"私有部署"延展到个人的"灾难/断网场景准备"。

技术上看不复杂，但理念契合当下：本地 LLM 已可用，存储白菜价，复合到"离网仍可问 AI"是合乎逻辑的产品形态。

---

## 生态观察

今天的 trending 板块有三股清晰的流：

1. **"LLM 数据前处理"工具链密集爆发**——markitdown 与 liteparse 同日上榜，说明 RAG 进入"工程化精修"阶段，把质量瓶颈从模型本身转向了 ingestion。

2. **Agent harness / Plugin 生态拥挤**——claude-code、cursor/plugins、revfactory/harness、compound-engineering-plugin、affaan-m/ECC 同日入榜，反映"agent 时代真正的护城河是元-skill 与工作流定义"。

3. **多模态生成下沉到方言级别**——VoxCPM2 的 9 中文方言 + 30 语言、MoneyPrinterTurbo 的视频自动化，把"完整本地化内容生产管线"再压缩了一档。

冷静期：**纯前端框架、纯 Web3、纯 DevOps** 类项目今日基本无声——市场注意力被 AI tooling 持续吸走。
