# GitHub Trending 每日观察 · 2026-04-25

## 今日焦点

> **Claude 生态爆发 · 自主 ML 代理 · 免费代理工具 · 代码检索 MCP · 安全供应链**
>
> - `Alishahryar1/free-claude-code` 一夜 +2,640⭐，把 Claude Code 流量代理到 NVIDIA NIM / OpenRouter / 本地模型的"平替网关"
> - `huggingface/ml-intern` +2,981⭐，HF 官方开源的自主 ML 工程 agent，能读论文、写代码、跑训练
> - `zilliztech/claude-context` +706⭐，Zilliz 把语义代码检索做成 Claude Code 的 MCP，号称降 40% token
> - `Anil-matcha/Open-Generative-AI` +847⭐，主打"200+ 模型聚合、无审查"的开源图像/视频生成目录
> - `google/osv-scanner` +147⭐，Go 漏洞扫描器继续稳居前排，反映企业端对供应链安全的持续投入

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [Alishahryar1/free-claude-code](https://github.com/Alishahryar1/free-claude-code) | 通过 NIM / OpenRouter / 本地模型代理免费使用 Claude Code | Python | 8,414 | +2,640⭐ | 1,270 |
| 2 | [huggingface/ml-intern](https://github.com/huggingface/ml-intern) | 开源自主 ML 工程师，读论文、训模型、交付方案 | Python | 5,127 | +2,981⭐ | 425 |
| 3 | [Z4nzu/hackingtool](https://github.com/Z4nzu/hackingtool) | 一站式渗透测试工具集合 | Python | 62,156 | +1,377⭐ | 6,964 |
| 4 | [Anil-matcha/Open-Generative-AI](https://github.com/Anil-matcha/Open-Generative-AI) | 200+ 模型的开源图像/视频生成目录 | JavaScript | 7,581 | +847⭐ | 1,409 |
| 5 | [codecrafters-io/build-your-own-x](https://github.com/codecrafters-io/build-your-own-x) | 通过重写知名技术掌握编程 | Markdown | 494,550 | +817⭐ | 46,839 |
| 6 | [zilliztech/claude-context](https://github.com/zilliztech/claude-context) | Claude Code 的代码语义检索 MCP | TypeScript | 8,937 | +706⭐ | 689 |
| 7 | [open-metadata/OpenMetadata](https://github.com/open-metadata/OpenMetadata) | 数据发现、可观测与治理的统一元数据平台 | TypeScript | 13,299 | +530⭐ | 2,032 |
| 8 | [dani-garcia/vaultwarden](https://github.com/dani-garcia/vaultwarden) | Rust 编写的 Bitwarden 兼容服务器 | Rust | 59,137 | +252⭐ | 2,725 |
| 9 | [google/osv-scanner](https://github.com/google/osv-scanner) | 基于 OSV 数据的 Go 漏洞扫描器 | Go | 9,420 | +147⭐ | 615 |
| 10 | [PostHog/posthog](https://github.com/PostHog/posthog) | 分析、实验、特性开关一体化平台 | Python | 33,033 | +90⭐ | 2,579 |
| 11 | [deepseek-ai/DeepEP](https://github.com/deepseek-ai/DeepEP) | 面向 MoE 的高效专家并行通信库 | Cuda | 9,307 | +29⭐ | 1,181 |
| 12 | [microsoft/typescript-go](https://github.com/microsoft/typescript-go) | TypeScript 编译器的 Go 原生移植 | Go | 24,995 | +22⭐ | 907 |

---

## 重点项目点评

### 🥇 [huggingface/ml-intern](https://github.com/huggingface/ml-intern) — 今日榜首，+2,981⭐

**Hugging Face 官方下场做 "AI ML 工程师"，而不是又一个代码补全**

`ml-intern` 是 HF 把自家 Hub、论文、数据集、Jobs 计算资源全部串起来，做成一个可以自主读论文、跑训练、交付模型的 agent。它不是又一个 "让 Claude 帮你写几行 PyTorch"——而是一个有**完整 agentic loop**（最多 300 轮迭代）、**170k token 自动压缩**、**doom-loop 检测**、**敏感操作审批门**的工程化 agent。

技术栈选择值得注意：底层通过 `litellm` 调 Claude（而不是自家 HF Inference），同时把 MCP server 做成一等公民、支持第三方工具扩展。这意味着 HF 把自己定位成**执行环境和数据提供方**，而不是模型提供方——用户想用什么模型随便，但训练机、数据、论文检索锁定在 HF。

这种 "基础设施 + 官方 agent" 的打法，是继 OpenAI Codex CLI、Anthropic Claude Code 之后，第三种主流路径，也是垂直做 ML 的第一家。近期如果 Kaggle / Databricks 跟进类似 agent，就是信号。

---

### 🥈 [Alishahryar1/free-claude-code](https://github.com/Alishahryar1/free-claude-code) — +2,640⭐

**"免费 Claude Code" 的真正含义：把 Claude 换成别的模型**

榜首争议项目。项目本身是一个**协议翻译代理**：截住 Claude Code 发往 Anthropic 的请求，改写成 OpenAI 兼容格式，再分流到 NVIDIA NIM 免费额度、OpenRouter、DeepSeek 直连或本地 LM Studio / llama.cpp。所以所谓 "free" 其实是 "你仍然用 Claude Code 的 CLI 壳和工具链，但换了后端大脑"。

它之所以能一天涨近 3k star，折射出两个市场情绪：（1）Claude Code 的 **产品体验**（agentic loop、tool use、终端整合）已经强到让人愿意绕过 Anthropic 订阅；（2）开源社区对 NVIDIA NIM、OpenRouter 这类 "免费 / 超低价 LLM 入口" 的关注度远超此前预期。

值得警惕的合规问题：这明显踩在 Anthropic ToS 的灰色边界。如果 Anthropic 选择收紧 Claude Code 对非官方端点的调用（比如加签名或版本绑定），这类项目会迅速失效。但在此之前，它会继续吸引想 "花本地模型的钱、用 Claude Code 的工具" 的群体。

---

### 🥉 [zilliztech/claude-context](https://github.com/zilliztech/claude-context) — +706⭐

**向量数据库厂商抢滩 Claude Code 的 "检索层"**

Zilliz（Milvus 背后的公司）把自家向量检索能力封装成 MCP server 塞给 Claude Code。卖点非常具体：**在同等检索质量下降低 ~40% token 消耗**。做法也务实——BM25 + dense embedding 混合检索、基于 Merkle 树的增量索引、AST 代码切分、多语言 / 多嵌入模型适配。

这类 MCP 的出现标志着 **Claude Code 生态的第二层开始成形**。第一层是 Anthropic 自己的 agent loop 和官方工具；第二层是向量检索（Zilliz）、代码理解、调试、可观测等垂直能力通过 MCP 接入。Zilliz 此刻抢跑的逻辑也很清晰：一旦某种 MCP 成为默认配置，替换成本极高。

类似这条赛道值得观察的还有 Pinecone、Qdrant、Weaviate 是否会跟进发布自己的 Claude Code MCP——今天之后可能是一场 "代码检索 MCP 竞赛"。

---

### 🏅 [Anil-matcha/Open-Generative-AI](https://github.com/Anil-matcha/Open-Generative-AI) — +847⭐

**"无审查 + 200+ 模型" 的图像/视频生成聚合目录**

项目本质是一个**策展式目录**，把 200 多个开源图像 / 视频 / 音频生成模型集合在一个 README，按 "Flux / Stable Diffusion / Wan / HunyuanVideo / 音乐" 等分类陈列。它之所以热，靠的是一句"**Uncensored alternative**"的定位——面对越来越严格的商业模型内容策略（Imagen 4、Veo 3、Sora 3），一部分用户开始迁徙到开源栈。

这类"模型目录"类项目在 GitHub 有长期流量，类似的前辈是 `awesome-chatgpt-prompts`、`awesome-llm`。但其时机选择耐人寻味：Sora 3 刚发布、Veo 3 加码内容过滤，这种 "反审查聚合" 正好踩到**创作者社群的不满情绪**。

---

### 🔧 [google/osv-scanner](https://github.com/google/osv-scanner) — +147⭐

**老将继续上榜，反映企业端的真实 Top Concern**

Google 的 OSV (Open Source Vulnerabilities) 扫描器，连续在榜已经说明问题：供应链安全 / SBOM 合规已经成为企业日常工作流的一部分。`osv-scanner` 的亮点是**数据权威（OSV.dev）、引擎轻量（Go 单二进制）、集成 CI 简单**。

相比较 Snyk 等商业方案，它的定位是 "无需账号、无需 SaaS"，因此在内部 pipeline 工具链里越来越常见。今天这 147 颗星意义不在峰值，而在它的**基线持续性**——这是真正的"刚需项目"。

---

## 生态观察

今天是非常典型的 **"Claude 生态日"**：榜单 top 10 里有 3 个直接围绕 Claude Code（免费代理、语义检索 MCP、自主 agent 调 Claude）。这三个项目分别对应三种商业应对方式：**替换模型（free-claude-code）、增强能力（claude-context）、把它当引擎（ml-intern）**，生态位非常清晰。

另一个 undercurrent 是 **"反审查"的消费侧情绪**。`Open-Generative-AI` 的爆发、以及 hackingtool 这种老牌红队工具仍然保持每日千星级的增速，说明在主流 AI 产品合规越收越紧的背景下，"开源兜底"的心智正在形成。

Rust / Go 基础设施项目（vaultwarden、osv-scanner、typescript-go）继续缓慢涨星，没有爆点但底盘稳——这类项目的 star 增速往往和 HN / Reddit 周报更相关，而非当日热点。
