# GitHub Trending 日报 · 2026-05-09

## 今日焦点

> **Anthropic 金融垂类 · 编码 Agent 与 Skills 体系 · DeepSeek V4 生态 · 推理加速 · 反检测浏览器**
>
> - `anthropics/financial-services` Anthropic 罕见亲自下场垂直行业，单日暴涨 +3,662⭐
> - `Hmbown/DeepSeek-TUI` DeepSeek V4 配套终端 Agent，+3,827⭐ 拿下今日单日新增冠军
> - `addyosmani/agent-skills` 大佬下场总结"AI 编码 Agent 工程化技能"，+1,794⭐
> - `z-lab/dflash` 块扩散 + 投机解码的工程化实现，推理加速赛道继续升温
> - `CloakHQ/CloakBrowser` C++ 源码级补丁的 stealth Chromium，Agent 自动化对抗反爬到了新阶段

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [anthropics/financial-services](https://github.com/anthropics/financial-services) | Claude 金融服务参考 Agents、Skills 与数据连接器 | Python | 14,681 | +3,662⭐ | 1,821 |
| 2 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 面向 AI 编码 Agent 的 20 个生产级工程技能集 | Shell | 35,051 | +1,794⭐ | 4,001 |
| 3 | [Hmbown/DeepSeek-TUI](https://github.com/Hmbown/DeepSeek-TUI) | DeepSeek V4 模型的终端编码 Agent | Rust | 21,623 | +3,827⭐ | 1,674 |
| 4 | [z-lab/dflash](https://github.com/z-lab/dflash) | 用块扩散做投机解码加速 LLM 推理 | Python | 3,799 | +388⭐ | 264 |
| 5 | [decolua/9router](https://github.com/decolua/9router) | 免费多供应商 AI 编码连接服务 | JavaScript | 5,465 | +1,028⭐ | 1,062 |
| 6 | [CloakHQ/CloakBrowser](https://github.com/CloakHQ/CloakBrowser) | 源码级补丁的 stealth Chromium，过几乎所有 bot 检测 | Python | 2,828 | +482⭐ | 229 |
| 7 | [awslabs/aidlc-workflows](https://github.com/awslabs/aidlc-workflows) | AWS 出品的 AI 编码 Agent 工作流规则 | Python | 1,716 | +92⭐ | 303 |
| 8 | [HKUDS/AI-Trader](https://github.com/HKUDS/AI-Trader) | 100% 自动化的 Agent 原生交易平台 | Python | 14,535 | +189⭐ | 2,430 |
| 9 | [LearningCircuit/local-deep-research](https://github.com/LearningCircuit/local-deep-research) | 本地化 Deep Research，SimpleQA 上 ~95% | Python | 6,680 | +572⭐ | 585 |
| 10 | [lobehub/lobehub](https://github.com/lobehub/lobehub) | 多 Agent 协作工作与生活空间 | TypeScript | 76,425 | +74⭐ | 15,111 |
| 11 | [datawhalechina/hello-agents](https://github.com/datawhalechina/hello-agents) | Datawhale 中文 Agent 教程，从入门到框架 | Python | 44,499 | +645⭐ | 5,415 |
| 12 | [flutter/skills](https://github.com/flutter/skills) | Flutter 官方对外发布的 Skills 集合 | Dart | 1,615 | +168⭐ | 91 |

---

## 重点项目点评

### 🥇 [anthropics/financial-services](https://github.com/anthropics/financial-services) — 单日新增 +3,662⭐

**Anthropic 第一次亲自下场做垂直行业，把"Skills"具象化到了金融行业**

这个仓库一夜间窜上榜首，并不是因为它"开源了一个金融 LLM"，而是因为它开了一个先例：Anthropic 自己出手发布了一套行业级的 Agent + Skill + Connector 参考实现。仓库里包含 11 个面向投行、股票研究、私募股权、财富管理、基金管理的 Agent，每个都配套了 pitch deck 制作、财报分析、GL 对账、KYC 等专业 Skill；同时打通了 Daloopa、Morningstar、S&P Global、FactSet 等 11 家金融数据源的 MCP 连接器，可以同时以 Claude Cowork 插件和 Managed Agents API 两种形态部署。

这个组合是过去半年 Anthropic 战略路线的一次完整落地——Skills 不再只是社区自由发挥的轻量级 Markdown 文件，而是直接被 Anthropic 编排成行业解决方案。对照 OpenAI 在金融领域更倾向于"模型 + 工具 + ChatGPT 内置"的路线，Anthropic 走的是"中性平台 + 行业生态"的路。仓库还显式写了"不做投资建议、不执行交易、必须人审"，这套谨慎措辞本身就是给受监管行业一个交付模板，潜在效仿者会很多。

---

### 🥈 [Hmbown/DeepSeek-TUI](https://github.com/Hmbown/DeepSeek-TUI) — 单日新增 +3,827⭐（今日新增冠军）

**DeepSeek V4 模型的"开源版 Claude Code"**

DeepSeek V4 上线后，整个生态都在补配套工具，DeepSeek-TUI 是这股浪潮中跑得最快的一个。它用 Rust 写了一个键盘驱动的终端 Agent，原生支持 V4 的流式 reasoning block 渲染、本地工作区的"approval-gated"编辑、文件操作、Shell 执行、git 管理、网页搜索，以及通过 MCP 接外部工具——基本就是把 Claude Code 的体验复刻到 DeepSeek 上。

亮点是它的 auto 模式：不仅自动选模型，还自动选 thinking 等级，相当于把"什么场景该花多少推理预算"这个工程问题做进了 Agent 框架本身。这指向一个值得关注的趋势——随着推理模型分级越来越细（thinking budget、speed mode、tool mode 等），Agent 端需要主动做"模型路由 + 推理预算管理"，过去一年这件事还多由人类工程师手写 prompt 决定。Rust 的选型也耐人寻味：终端 Agent 这个生态正在从 Python/Node 集体往 Rust 迁移，启动速度和长时间会话稳定性是核心驱动。

---

### 🥉 [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — 单日新增 +1,794⭐

**Google Chrome 团队大佬下场总结"AI 编码 Agent 的工程纪律"**

Addy Osmani 在前端工程界的影响力不用多说，这次他把方向对准了 AI Agent 工程实践，把高级工程师在真实项目里使用的工作流、质量门和最佳实践编码成 20 个结构化 Skill：从需求定义、TDD、安全加固、code review 标准到 CI/CD 自动化，覆盖整个开发生命周期。

它跟 anthropics/financial-services 形成了有趣的对照——后者是"行业 × Skill"，这里则是"研发流程 × Skill"。两个都说明一件事：Skills 这个抽象概念正在变成行业里"复用工程经验"的标准载体，类似当年 ESLint 规则集、Docker 镜像生态崛起的时刻。如果你今年在做 Agent 平台或内部 Cowork，这个仓库基本是绕不过去的参考。

---

### 4️⃣ [z-lab/dflash](https://github.com/z-lab/dflash) — 单日新增 +388⭐

**用"块扩散"做投机解码：推理加速赛道的新解法**

DFlash 把扩散模型这个原本属于图像生成的范式，用作投机解码（speculative decoding）里的草稿模型——一次并行生成多个 token 草稿，再交给目标 LLM 验证。相比传统用小语言模型做 draft 的做法，扩散 draft 在并行度上有天然优势。

仓库已经覆盖了 vLLM、SGLang、Transformers、MLX 四大后端，预训练 draft 模型同时支持 Qwen、Gemma、LLaMA 等，DeepSeek-V4 与 GLM-5.1 也在路线图上。星数虽然只有 3.8K，但项目方向卡得很准——2026 年模型权重已经不是稀缺品，**推理 token 经济学**才是真正的战场，谁能稳定把 throughput/latency 打下来，谁就能拿到底层基础设施话语权。

---

### 5️⃣ [CloakHQ/CloakBrowser](https://github.com/CloakHQ/CloakBrowser) — 单日新增 +482⭐

**Agent 自动化和反爬之间的军备竞赛升级到 C++ 编译期**

CloakBrowser 不走 JS 注入或者运行时配置 hack 的老路，而是直接给 Chromium 打了 49 个 C++ 源码级补丁，把 stealth 行为编进二进制里。结果是 reCAPTCHA v3 拿到 0.9 分（普通 Playwright 只有 0.1），并且号称能绕过 Cloudflare Turnstile、FingerprintJS、BrowserScan 等 30+ 检测服务。API 完全兼容 Playwright/Puppeteer，可以"换 import 即上线"。

这个仓库爆火背后的真实驱动力，是当下的 Agent 浪潮——所有 Browser-Use、Skyvern、Computer-Use 类工具都需要稳定可靠地浏览公开互联网，但反爬厂商也升级了 fingerprint 识别。CloakBrowser 这种"编译期改造"的路线，预示着下一阶段 Agent 浏览器会进一步分化为两层：一层是 Anthropic / OpenAI 自己的官方 computer use（守规矩），另一层则是社区驱动、对抗性更强的开源浏览器。这条赛道在 2026 年只会越来越热。

---

## 生态观察

今日热榜几乎被三条主线占满：

1. **Skills 生态体系化**：Anthropic 亲自做行业 Skill 包、Addy Osmani 做工程实践 Skill 包、Flutter 做框架 Skill 包，"Skill"已经从一个 Anthropic 专属概念变成了跨厂商共同接受的工程抽象。
2. **DeepSeek V4 配套生态爆发**：DeepSeek-TUI 拿下今日单日新增冠军，再加上 dflash 路线图里专门提到 V4 适配，开源世界正在围绕 V4 重新组装一遍编码 Agent 工具链。
3. **Agent 时代基础设施进一步分化**：上层是行业垂类（金融、交易），中层是研发工具链与本地研究助手（local-deep-research），底层是推理加速（dflash）和反检测浏览器（CloakBrowser）——一条完整的 Agent 工业链已经在 GitHub 上跑通了原型。

相对冷却的是"通用大模型仓库"和"前端 UI 框架"，今天没有任何这两类项目进入前 12——这本身就是 2026 年开源叙事重心彻底向 Agent 化倾斜的信号。
