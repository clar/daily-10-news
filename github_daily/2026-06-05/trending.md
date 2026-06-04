# GitHub Trending 日报 · 2026-06-05

## 今日焦点

> **Context 压缩 · Agent 平台战 · 国产 OCR 长青 · Spec-Driven 编程 · 物理 AI 数据集**
>
> - `chopratejas/headroom` 一夜 +3,139⭐，"LLM 输入压缩中间件"成本焦虑的直接答卷
> - `NousResearch/hermes-agent` +1,951⭐，开源 agent 生长路线再加注，对 Claude Code / Codex 的开放替代
> - `affaan-m/ECC` +1,736⭐，Agent harness 优化 + skills/memory/security 三件套，社区版"agent OS"竞速
> - `github/spec-kit` +311⭐，规格驱动开发工具包持续高位，AI 写代码倒逼"先写 spec"
> - `NVIDIA/cosmos` +244⭐，物理世界模型与数据集开放，机器人 / 自动驾驶生态进入"开源底座"阶段

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [chopratejas/headroom](https://github.com/chopratejas/headroom) | LLM 输入前的工具输出/日志/RAG 压缩中间件 | Python | 12,339 | +3,139⭐ | 804 |
| 2 | [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) | 开源 agent，强调"和用户一起成长" | Python | 180,892 | +1,951⭐ | 31,027 |
| 3 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Agent harness 性能优化套件（skills/memory/security） | JavaScript | 207,153 | +1,736⭐ | 31,801 |
| 4 | [jwasham/coding-interview-university](https://github.com/jwasham/coding-interview-university) | 长青刷题手册 | Markdown | 349,680 | +740⭐ | 83,224 |
| 5 | [Open-LLM-VTuber/Open-LLM-VTuber](https://github.com/Open-LLM-VTuber/Open-LLM-VTuber) | LLM 驱动的 Live2D 语音陪伴 | Python | 9,548 | +583⭐ | 1,145 |
| 6 | [lfnovo/open-notebook](https://github.com/lfnovo/open-notebook) | Notebook LM 的开源实现 | TypeScript | 24,940 | +482⭐ | 2,909 |
| 7 | [openclaw/openclaw-windows-node](https://github.com/openclaw/openclaw-windows-node) | Windows 上的 Claude 助手（系统托盘 + PowerToys） | C# | 1,307 | +358⭐ | 167 |
| 8 | [github/spec-kit](https://github.com/github/spec-kit) | Spec-Driven Development 工具包 | Python | 108,538 | +311⭐ | 9,593 |
| 9 | [reconurge/flowsint](https://github.com/reconurge/flowsint) | 图谱化情报调查可视化平台 | TypeScript | 5,278 | +308⭐ | 637 |
| 10 | [aquasecurity/trivy](https://github.com/aquasecurity/trivy) | 容器与代码安全扫描 | Go | 35,654 | +255⭐ | 431 |
| 11 | [NVIDIA/cosmos](https://github.com/NVIDIA/cosmos) | 物理 AI 的开放世界模型与数据集 | Jupyter Notebook | 8,961 | +244⭐ | 578 |
| 12 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 跨平台趋势研究 agent | Python | 27,538 | +173⭐ | 2,344 |
| 13 | [github/copilot-sdk](https://github.com/github/copilot-sdk) | Copilot Agent 多平台 SDK | Java | 8,945 | +107⭐ | 1,209 |
| 14 | [PaddlePaddle/PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR) | 100+ 语种 OCR 工具集 | Python | 79,820 | +105⭐ | 10,597 |

---

## 重点项目点评

### 🥇 [chopratejas/headroom](https://github.com/chopratejas/headroom) — 今日榜首，+3,139⭐

**Token 经济学已经从模型层卷到中间件层**

`headroom` 把自己定位为"在 LLM 输入前压缩工具输出、日志、文件、RAG 切片"的中间件——目标客户是任何把 Claude Code / Codex / Cursor 接入复杂工具链的开发者。一句话总结它的卖点：**与其升级到 Opus 价位，不如先把 32k tokens 的 git log / lint 输出压成 4k**。

一夜 3,139⭐ 的增量背后有非常明确的现实信号：(1) Anthropic 把 Fast Mode 价格压到 1/3 之后，开发者开始用更多并发，**输入 token 已经成为成本主项**；(2) 主流 IDE agent（Claude Code、Codex、Cursor agent 模式）都开始大量调用 shell + 多文件读写，原始输出动辄上万 token；(3) RAG 系统过去一年的"chunk 大小如何选"的争论，被一个**通用压缩管线**直接绕过。

如果未来一周 `headroom` 能扩展到 Codex / Cursor 插件层，今年大概率会出现"LLM 中间件"的独立 funding 类别——形态可能类似 nginx 对 Web 2.0 的意义。

---

### 🥈 [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) — +1,951⭐

**Nous Research 把开源 agent 从模型 push 到 runtime**

Nous Research 一向以**开源、社区微调、贴近研究者文化**著称，今天上线的 `hermes-agent` 把过去一年其 Hermes 系列模型扩展为**完整的 agent runtime**：内置记忆系统、技能库与会话级演化（"and grows with you" 的核心点）。

它的关键差异化是**模型层与 runtime 层都开源**——这一点 LangChain / CrewAI 等 agent 框架做不到，因为它们没有自家模型；而 OpenAI / Anthropic / Google 的 agent runtime（Codex、Claude Code、Gemini Spark）又不开源。**Nous 在做的是"自由派 Claude Code"**。

今天的 +1,951⭐ 其实是连锁反应：Anthropic 上周发布"递归自我改进"研究 + Opus 4.8 同期高调封闭路线之后，开源派需要一个对应叙事，Nous 就是那个钉子。

---

### 🥉 [affaan-m/ECC](https://github.com/affaan-m/ECC) — +1,736⭐

**Agent harness 优化套件：第三方"性能调度器"开始独立成赛道**

`ECC` 自我定位是"Agent harness performance optimization system with skills, memory, and security"——把 agent 运行时的三件事（**技能定义、记忆管理、安全控制**）打包成可插拔模块。这与 `hermes-agent` 思路相近但定位不同：ECC 不绑定模型，只优化 harness。

它 trending 的逻辑在于：随着 Claude Code、Codex、Cursor 都引入"skills"概念，**第三方 agent harness 开始尝试做"统一插件标准"**——你写一份 skill，能同时跑在多个 agent 上。这是 VSCode 早期 LSP 标准化的复刻路径。

值得警惕的是 207k 总星、31.8k Fork 这种异常高数据——很可能是仓库 fork 或迁移自更早项目（数据需要进一步核验），但本身概念命中点是真实的。

---

### 4️⃣ [github/spec-kit](https://github.com/github/spec-kit) — +311⭐

**"先写 spec 再让 AI 写代码"作为方法论持续上量**

`spec-kit` 是 GitHub 官方的 **Spec-Driven Development** 工具包：开发者先用结构化 spec 描述需求，工具再调用 Copilot Agent 生成、验证、回填测试。这个仓库 10w+ 总星，今天仍然在 trending，说明这套方法论已经从"实验性"进入"主流团队尝试落地"阶段。

它解决的是当前 AI 编码的核心顽疾：**LLM 一次生成 1k 行代码很容易，但用户没法判断它写得对不对**。Spec-driven 强行把"对不对"提前到 spec 阶段，再让 LLM 在严格约束下生成。结合今日 #17 那条 "Opus 4.8 形式化验证 oneshot" 的 Show HN，**"AI 写代码 + 形式化验证"组合开始有人买单**。

---

### 5️⃣ [NVIDIA/cosmos](https://github.com/NVIDIA/cosmos) — +244⭐

**物理 AI 的开源底座，机器人/自动驾驶进入"基础模型 + 数据集"阶段**

NVIDIA Cosmos 是面向"物理 AI"（机器人、自动驾驶、具身智能）开放的**世界模型基线与配套数据集**。这次 trending 的直接诱因是 NVIDIA Rubin 平台量产 + 与 Meta 等签下多代多卡协议（参见今日 AI 日报）：**硬件供给一旦确认，开发者会回头来选"开源底座"**。

Cosmos 的意义在于把"世界模型 + 物理仿真 + 数据集"压成一个仓库，让中小团队不需要重新做模拟器和合成数据基础设施。配合 vLLM 生态、华为 KVarN（参见今日 HN #6）等推理优化项目，**2026 下半年具身智能开源工具链有可能进入第二轮爆发**。

---

## 生态观察

**主题一：成本问题被中间件层接住。** `headroom` 一夜冲顶不是偶然——`tiktoken-utilities`、`gptee`、`promptlayer` 等同类项目都在升星。下一步会出现"标准化压缩协议"或"LLM 网关"的小型创业潮。

**主题二：开源 Agent 正在三条线并进。** (1) 完整 stack（hermes-agent）；(2) harness 优化器（ECC）；(3) IDE 插件（openclaw-windows-node）。三条线的共同对手是 Claude Code / Codex / Cursor 的封闭路径。

**主题三：Spec-Driven 与形式验证融合。** `spec-kit` 长期高位 + 今日 HN 上的"形式化验证 + LLM oneshot"组合，预示着 2026 下半年开发者工具的主旋律是**"AI 输出 + 强约束验证"**，不是单纯加大模型。

**主题四：国产模型与工具链稳定占位。** PaddleOCR 长青、KVarN（华为）、Qwen 系列在 trending 前 50 频繁出现——中国生态在"工具链 + 推理优化"层的影响力比一年前明显更稳。
