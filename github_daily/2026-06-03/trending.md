# GitHub Trending 日报 · 2026-06-03

## 今日焦点

> **Agent 基建生态全面爆发 · LLM 文档前处理刚需 · 中文 TTS 杀回前沿 · OSINT 工具复兴**
>
> - `microsoft/markitdown` 单日 **+3,616⭐**，141K 星，几乎垄断"文件转 Markdown 喂 LLM"赛道。
> - `nesquena/hermes-webui` 单日 **+1,725⭐**，自托管持久化 agent 平台 Web 端火出圈。
> - `affaan-m/ECC` 单日 **+1,597⭐**，号称生产级 agent harness 性能优化系统（63 agents / 249 skills）。
> - `chopratejas/headroom` 单日 **+1,266⭐**，号称为 LLM 上下文压缩 60-95%，agent 经济进入"省 token"卷阶段。
> - `OpenBMB/VoxCPM` 单日 **+779⭐**，2B 参数 tokenizer-free 多语言 TTS，30 语言 + 9 种汉语方言。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [microsoft/markitdown](https://github.com/microsoft/markitdown) | 文件/Office 文档转 Markdown，专为 LLM 优化 | Python | 141,014 | +3,616 | 9,606 |
| 2 | [nesquena/hermes-webui](https://github.com/nesquena/hermes-webui) | Hermes 自治 Agent 平台的 Web UI | Python | 12,500 | +1,725 | 1,536 |
| 3 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Agent harness 性能/技能/记忆/安全套件 | JavaScript | 203,810 | +1,597 | 31,267 |
| 4 | [chopratejas/headroom](https://github.com/chopratejas/headroom) | LLM 上下文压缩：日志/工具输出/RAG 块 | Python | 6,213 | +1,266 | 433 |
| 5 | [D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling) | 自适应网页爬取框架 | Python | 59,100 | +1,196 | 5,708 |
| 6 | [OpenBMB/VoxCPM](https://github.com/OpenBMB/VoxCPM) | 端到端扩散自回归 TTS，30 语言 + 方言 | Python | 25,068 | +779 | 2,878 |
| 7 | [supermemoryai/supermemory](https://github.com/supermemoryai/supermemory) | AI 应用的统一记忆引擎/API | TypeScript | 24,590 | +677 | 2,176 |
| 8 | [stefan-jansen/machine-learning-for-trading](https://github.com/stefan-jansen/machine-learning-for-trading) | 算法交易 ML 教材配套代码 | Jupyter | 18,426 | +570 | 5,222 |
| 9 | [reconurge/flowsint](https://github.com/reconurge/flowsint) | 可视化图谱网络安全调查平台 | TypeScript | 4,472 | +190 | 580 |
| 10 | [Open-LLM-VTuber/Open-LLM-VTuber](https://github.com/Open-LLM-VTuber/Open-LLM-VTuber) | 免手操作 LLM 语音交互 + Live2D | Python | 8,306 | +65 | 1,071 |
| 11 | [jamwithai/production-agentic-rag-course](https://github.com/jamwithai/production-agentic-rag-course) | 生产级 Agentic RAG 教学课程 | Python | 6,359 | +31 | 1,488 |

---

## 重点项目点评

### 🥇 [microsoft/markitdown](https://github.com/microsoft/markitdown) — 今日榜首，+3,616⭐

**Markdown 作为 LLM 的标准摄入格式，正在被一个微软工具垄断**

markitdown 把 PDF、PowerPoint、Word、Excel、HTML、CSV、JSON、XML、ZIP、YouTube URL、EPub、图像（带 EXIF 和 OCR）、音频文件统一转换成 Markdown。141K 星 + 2.7K 个 dependent 项目 + 5/26 刚发布的 v0.1.6 让它今日继续爆涨。它能爆的真实原因不在功能多，而在卡到了 **agent 时代的工程瓶颈** —— 每个 RAG / agent 项目都要做"任意文件 → 适合 LLM 喂养的纯文本"这一步，而 markitdown 把这件事做到了"装一个 Python 包就完事"。

它和今日 #4 headroom（上下文压缩）、#7 supermemory（记忆引擎）、#11 agentic RAG course 形成了清晰的"agent 前处理栈"——markitdown 负责 ingest，headroom 负责 compress，supermemory 负责持久化记忆。这就是 2026 年下半年 agent 应用的"四件套"标准答案。

**项目侧风险**：竞品在追，包括 unstructured.io、docling、llama-parse 等。markitdown 的护城河是微软背书 + 简洁 API + 文件格式覆盖宽，但 OCR 与表格保真度仍是短板。

---

### 🥈 [nesquena/hermes-webui](https://github.com/nesquena/hermes-webui) — +1,725⭐

**自托管、可持久化、能跨 session 学习的 agent，正在变成开发者的"个人 OS"**

Hermes WebUI 是 Hermes Agent 的 Web 前端，三栏布局（session/聊天/文件），最关键的是它对应的 Hermes Agent 本身是 **持续运行在你服务器上的自治系统**——cross-session 记忆、自托管 cron、多 provider（OpenAI/Anthropic/Google），并且会自动写下"自我改进的 skill"。这套设计在今天上榜不是巧合：它是对"Claude Code/Cursor/Devin 都跑别人的云"这件事的反作用力。

为什么社区在投票？因为 2026 年中段，开发者意识到"agent 的状态不在云上就在自己机器上"才是可控的——本地 Hermes + 本地 Ollama / 本地 MAI-Code、再加 hermes-webui 这种轻量界面，刚好补齐了"我不想把全部历史交给 SaaS"的开发者群。MIT 协议 + Python + Vanilla JS 无 build 流程，进一步降低了部署门槛。

**和今日 #3 ECC 互补**：ECC 是"内嵌进 Claude Code/Cursor 等 harness"的优化套件，Hermes 是"独立自洽的 agent + UI"。两者今天同时上榜，说明 self-hosted agent 这条线已经从极客玩具走向通用工具。

---

### 🥉 [chopratejas/headroom](https://github.com/chopratejas/headroom) — +1,266⭐

**"省 token = 省钱"成为 agent 时代的新隐性 KPI**

headroom 是一个上下文压缩层：JSON 用 SmartCrusher、代码用基于 AST 的 CodeCompressor、文本用 Kompress-base ML 模型；号称在 GSM8K / TruthfulQA / SQuAD 上保持精度的同时压掉 73-92% token。它能跑成 Python/TypeScript 库、HTTP 代理、MCP server 或直接 wrap agent，部署灵活到几乎覆盖所有 agent 工程姿势。

它和今天 HN 头条 GitHub Copilot 6/1 转 AI Credits 计费、Microsoft Build MAI-Code-1-Flash "token 用量低 60%" 形成完美呼应——**token 单价虽然在跌，但 agent workflow 调用量在指数级涨，结果是开发团队的 LLM 账单仍在飙升**。这种环境下，"无侵入式压缩"瞬间从可选项变成必装项。

特别注意它的 **Reversible Compression (CCR)** 设计——原始数据本地存，LLM 要全 context 时可以反查。这把"压缩"与"召回"解耦，是把传统 RAG 思路嫁接到 agent token 流的有趣尝试。

---

### 🏅 [OpenBMB/VoxCPM](https://github.com/OpenBMB/VoxCPM) — +779⭐

**中文实验室再次定义开源 TTS 前沿**

OpenBMB（清华系 MiniCPM 团队）发的 VoxCPM2：2B 参数、tokenizer-free 端到端扩散自回归架构、200 万小时多语言数据训练、48kHz 录音棚级输出、RTX 4090 上 RTF ≈ 0.3。覆盖 30 语种 + 9 种汉语方言，自然语言描述就能生成新嗓音、短样本即可克隆——Apache-2.0 商用友好。

这件事的产业意义：（1）TTS 从 2024 年的"几十 MB 小模型"走到 2026 年的"几十亿参数 + 扩散架构"，质量门槛已被中文实验室拉到 ElevenLabs 同档；（2）"tokenizer-free + 直接连续表征"是这一波声学模型的范式更新——传统 codec-based TTS 在自然度上会被显著拉开；（3）方言能力是中国厂商独占的护城河，9 种汉语方言一次性放出，让英文厂商短期难以追上。

值得追踪：MiniCPM-V、VoxCPM、AgentCPM 是 OpenBMB 在 2026 年构建的 multi-modal agent 三件套，已经隐隐和 Meta Llama 形成"开源前沿"双极。

---

### 🎖️ [D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling) — +1,196⭐

**LLM-era 爬虫复兴：从"反反爬"到"喂 LLM 数据闭环"**

Scrapling 是自适应网页爬取框架，能从单次请求扩展到全规模抓取。它今日的爆发不在新颖性，而在 **LLM 训练 + agent 实时检索两条线一起拉爆数据需求**——前沿模型团队需要新鲜语料、agent 工具 builder 需要稳定的"网页 → 结构化数据"管道。

它和 markitdown 形成互补：Scrapling 解决"从公网拿到原始内容"，markitdown 解决"把内容标准化喂给 LLM"。如果你今天要从零搭一个新闻聚合 agent，今天 trending 榜上 Scrapling + markitdown + headroom + supermemory + Hermes Agent 几乎就是完整答案。

---

## 生态观察

今日 trending 几乎是一份"agent 工程师工具清单"：

- **Agent 基建集中爆发**：榜上 11 个里有 7 个直接服务 agent 工作流（markitdown ingest、headroom compress、supermemory memory、Hermes agent runtime、ECC harness optimization、Scrapling crawler、agentic RAG course）。2026 年 H2 的 GitHub trending 正在被 agent stack 各层模块**逐层洗榜**。
- **省 token 战争开启**：headroom 这种以"压缩 token 输入"为唯一卖点的工具突然冲到 +1,266⭐，意味着行业已经从"模型变好"焦虑转向"账单变低"焦虑。下一波 trending 中类似工具会越来越多。
- **中文实验室在多模态前沿持续输出**：OpenBMB VoxCPM2 把开源 TTS 拉到了 48kHz + 多语言 + 方言覆盖，加上 Qwen / DeepSeek / Kimi 三线并行的 LLM，中文 AI 开源贡献度在 2026 年已经稳居全球第一梯队。
- **OSINT 工具回潮**：flowsint 这种"可视化网络安全调查图"在 LLM agent 帮助下越来越易上手——意味着调查记者、企业安全团队开始把 agent 当 OSINT 助手用，下一年这条线值得追踪。
- **教学项目悄然进榜**：production-agentic-rag-course + machine-learning-for-trading 两个教材类仓库同日上榜，说明"agent 学习曲线"已经形成市场——人们意识到光靠跟着官方文档已经不够。

值得关注的几个**下周可能继续上扬**的项目：headroom（agent 经济新刚需）、Hermes Agent + WebUI（self-hosted agent 浪潮）、VoxCPM（开源 TTS 新基线）。
