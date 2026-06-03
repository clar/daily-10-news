# GitHub Trending 日报 · 2026-06-04

## 今日焦点

> **Token 压缩工具登顶 · Agent harness / 记忆层全面爆发 · Markdown 与 PDF 转换继续被 RAG 拉动 · 本地 LLM 与 VTuber 上岸 · 量化交易 agent 跑出**
>
> - `chopratejas/headroom` 一日 **+3,528⭐**，Token 压缩拿到今日榜首——证明"AI 工具的下一站是省 token"
> - `affaan-m/ECC` **+2,147⭐**，全栈式 agent harness 给 Claude Code / Codex / Cursor 调优，Agent 工程化思路出圈
> - `NousResearch/hermes-agent` + `nesquena/hermes-webui` 同日双榜，**Hermes 系生态成形**
> - `microsoft/markitdown` 累计破 14 万星，**RAG 准备阶段标配**
> - `HKUDS/Vibe-Trading` 把"Vibe coding"思路搬进量化交易，一个新流派的雏形

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [chopratejas/headroom](https://github.com/chopratejas/headroom) | 压缩送进 LLM 的工具输出/日志/RAG 块 | Python | 9,498 | +3,528 | 627 |
| 2 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Agent harness 性能优化系统 | JavaScript | 205,624 | +2,147 | 31,570 |
| 3 | [microsoft/markitdown](https://github.com/microsoft/markitdown) | 文件 / Office 文档转 Markdown | Python | 142,784 | +2,006 | 9,756 |
| 4 | [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) | "随你成长"的开源 Agent 框架 | Python | 179,007 | +1,736 | 30,667 |
| 5 | [D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling) | 自适应 Web 抓取框架 | Python | 60,166 | +1,078 | 5,801 |
| 6 | [nesquena/hermes-webui](https://github.com/nesquena/hermes-webui) | Hermes Agent 的 Web/手机端 UI | Python | 13,074 | +734 | 1,590 |
| 7 | [Open-LLM-VTuber/Open-LLM-VTuber](https://github.com/Open-LLM-VTuber/Open-LLM-VTuber) | 本地多平台 Live2D + 语音 VTuber | Python | 8,909 | +702 | 1,103 |
| 8 | [supermemoryai/supermemory](https://github.com/supermemoryai/supermemory) | "AI 时代"的记忆 API 引擎 | TypeScript | 25,128 | +601 | 2,206 |
| 9 | [opendataloader-project/opendataloader-pdf](https://github.com/opendataloader-project/opendataloader-pdf) | 面向 AI 的开源 PDF 解析器 | Java | 23,219 | +573 | 2,177 |
| 10 | [jwasham/coding-interview-university](https://github.com/jwasham/coding-interview-university) | 软件工程师面试备考清单 | — | 348,965 | +459 | 83,153 |
| 11 | [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) | 个人化交易 Agent | Python | 9,855 | +221 | 1,998 |
| 12 | [lyogavin/airllm](https://github.com/lyogavin/airllm) | 单张 4GB GPU 跑 70B 推理 | Jupyter Notebook | 18,849 | +208 | 2,068 |
| 13 | [aquasecurity/trivy](https://github.com/aquasecurity/trivy) | 容器/K8s/云一站式安全扫描 | Go | 35,375 | +26 | 413 |
| 14 | [odoo/odoo](https://github.com/odoo/odoo) | 开源 ERP / 业务套件 | Python | 51,903 | +29 | 32,642 |

---

## 重点项目点评

### 🥇 [chopratejas/headroom](https://github.com/chopratejas/headroom) — 今日榜首，+3,528⭐

**Token 节流登顶：把 LLM 入口流量当作"网络流量"治理**

Headroom 把"工具输出 / 日志 / 文件 / RAG 切片"在 **送进 LLM 之前** 进行结构化压缩，号称 **60-95% token 削减、答案质量不变**。这是 Anthropic / OpenAI 价格阶梯固化后，开发者出现的典型反应：与其依赖模型方降价，不如自己在"输入端"做流量治理。

它今天能干掉所有 AI 应用项目登顶，**和昨天 HN 上 "Uber 给开发者 $1,500/月 AI 工具封顶" 是同一条暗线**——大家都在重新算 token 账。值得关注几个判断：（1）Agent 框架未来会标配"输入压缩中间件"；（2）Anthropic / Codex 之类的 long-running Agent 在多步工具调用中会成为最大受益者；（3）"AI 流量治理"作为新的 SaaS 类别隐约出现，未来可能跟 Tailscale / Cloudflare 一样产品化。

---

### 🥈 [affaan-m/ECC](https://github.com/affaan-m/ECC) — +2,147⭐

**Agent harness 工程化：技能、本能、记忆、安全、研究优先**

ECC（"Engineered Coding Companion"风格的开源 agent 调优框架）把 Claude Code、Codex、Opencode、Cursor 等编码 agent 视为可统一调度的"harness"，提供五大模块：**技能（skills）、本能（instincts）、记忆（memory）、安全（security）、研究优先（research-first）**。它把过去散落在 Markdown 规则、prompt fragment 和 settings.json 里的"agent 心智"打包成可复用、可配置的单元。

这个项目今天能爆 +2k 星，是因为它击中了几个共同诉求：（1）多 agent 协作时，**默认行为漂移**是开发者最痛的问题；（2）Claude Code / Codex / Cursor 之间 prompt 复用率极低，急需"harness-level"标准；（3）安全 / 研究优先 / 记忆三件套被越来越多团队列为 Agent 上线前必填项。

可以预期，2026 H2 会出现一波 "agent harness 框架"赛道，ECC 类项目和 Anthropic 官方的 Skills/MCP 体系将形成竞争+融合关系。

---

### 🥉 [microsoft/markitdown](https://github.com/microsoft/markitdown) — +2,006⭐

**RAG 数据准备的"事实标准"**

Markitdown 把 Word / Excel / PDF / PPTX / HTML / Image / Audio 等格式统一转成 Markdown——它的胜出不是因为算法多复杂，而是因为 **Markdown 已经成为 RAG / Agent 输入的统一中间态**。今天 +2k 星，叠加它累计 14 万星，说明该项目正在从"工具"演化为"AI 基础设施依赖"。

值得一起看的是榜单中 **opendataloader-pdf**（+573）——专门做 PDF→AI-ready 数据，强调可访问性与表格语义。两者搭配反映出一个事实：**2026 年 RAG 的真正瓶颈仍是"把脏数据洗干净"**，而不是向量召回或 prompt 工程。能在这个环节做扎实的项目，社区会持续奖励。

---

### 🤖 No.4 · [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) — +1,736⭐

**Hermes 系开源生态进入"工具年"**

NousResearch 的 hermes-agent 把"和你一起成长"的概念落到了工程层：长记忆 + 自我编辑技能 + 工具自创建 + 开放权重模型组合。**关键看点**是它在累计 17.9 万星的体量上还能日增 +1,736，且与 **nesquena/hermes-webui** 同日并榜——围绕 Hermes 形成了"核心 agent + 前端 UI + 社区 fork"的完整生态。

这呼应了今天另一个明显的趋势：**开源 Agent 不再追求"对标 GPT"，而追求"易于私有化部署、可自演化"**。Nous 走的是和 Anthropic Skills 截然不同的路径——前者从模型生态切入、后者从模型规范切入。

---

### 📈 No.5 · [HKUDS/Vibe-Trading](https://github.com/HKUDS/Vibe-Trading) — +221⭐

**"Vibe coding" 思路开始进入量化领域**

香港大学数据科学组的 Vibe-Trading 把"自然语言 + Agent 自动交易"做成了一个个人化框架。+221 的日增看起来不大，但**这是少见的来自高校实验室、却能进入主榜的 Agent 项目**。

它把过去 12 个月里 "Vibe Coding"（让 AI 凭语义和直觉直接产出代码）的思想搬到金融场景——意味着 Agent + 个人投资工具的赛道正在变得拥挤。今天的 Polymarket、Robinhood、Stocktwits 都已经接入 AI 助手，开源侧也开始有人卷个性化交易 agent。**风险与监管讨论会很快跟上**。

---

## 生态观察

- **本日双主题**：① "Token 经济学"（Headroom / Scrapling / opendataloader-pdf / markitdown）把"省钱、省 token"这件事变成了开源主旋律；② "Agent harness / 记忆 / Skills"（ECC、hermes-agent、hermes-webui、supermemory、airllm）正在成为新的基础设施层。
- **Hermes 系崛起**：核心 agent + WebUI 同日并榜，是开源社区少见的"双轨同步起飞"——下半年可能会出现 Hermes-style fork 潮，正面 PK Claude Code / Codex 的开源替代版图。
- **RAG 数据预处理仍是金矿**：Markitdown 14 万星 + opendataloader-pdf 高速增长，说明 2026 年"AI ready data"工具链空间还有。
- **冷门赛道升温**：本地 Live2D VTuber（Open-LLM-VTuber）+ 量化 Agent（Vibe-Trading）+ 4GB 显存推理（AirLLM）显示 **"个人级 AI 生活化部署"** 正在悄悄成势。
- **安全侧静音**：Trivy 等老牌项目仍在榜，但今日无新爆款；安全工具今日整体声音弱于 AI 应用层。
