# GitHub Trending 日报 · 2026-09-19

## 今日焦点

> **Agent Skill 生态爆发 · Claude 生态占据半壁江山 · 阿里/腾讯双双入场 · 浏览器 Agent 落地 · Rust 存储稳步收割**
>
> - `cloudflare/security-audit-skill` 一日暴涨 +3,019⭐ 冲上榜首，"多阶段安全审计 + 独立验证 + 机器可读结果"成为 Agent Skill 事实模板。
> - `alibaba/open-code-review` +2,724⭐ 挤到第 3，阿里首个正式冲榜的 Agent 项目。
> - `Tencent/BrowserSkill` +1,319⭐ 让 AI Agent 无缝接管你的已登录浏览器——2026 年新赛道的头炮。
> - `anthropics/claude-code` +442⭐ 依然稳如泰山，`agent-skills`、`knowledge-work-plugins` 集体上榜，说明 Claude 生态正在自我聚拢。
> - `rustfs/rustfs` +298⭐ 单日稳增，Rust 系统软件在存储/边缘领域继续吃 Go 和 C++ 的市场份额。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) | 多阶段安全审计 Agent Skill | JavaScript | 13,508 | +3,019⭐ | 723 |
| 2 | [anthropics/claude-code](https://github.com/anthropics/claude-code) | 终端里的 Agentic 编码助手 | TypeScript | 146,261 | +442⭐ | 23,776 |
| 3 | [alibaba/open-code-review](https://github.com/alibaba/open-code-review) | 混合架构代码 Review 工具 | Go | 36,605 | +2,724⭐ | 2,607 |
| 4 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | Agent harness 性能优化系统 | JavaScript | 262,005 | +965⭐ | 39,204 |
| 5 | [Tencent/BrowserSkill](https://github.com/Tencent/BrowserSkill) | 让 Agent 接管已登录浏览器 | TypeScript | 5,244 | +1,319⭐ | 364 |
| 6 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 生产级 AI 编码 Agent 技能库 | JavaScript | 96,372 | +677⭐ | 10,186 |
| 7 | [TencentCloud/Octop](https://github.com/TencentCloud/Octop) | 多用户多 Agent 自托管助手 | Python | 3,933 | +571⭐ | 405 |
| 8 | [Fission-AI/OpenSpec](https://github.com/Fission-AI/OpenSpec) | AI 编码助手的规范驱动框架 | TypeScript | 69,315 | +298⭐ | 4,748 |
| 9 | [ankitects/anki](https://github.com/ankitects/anki) | 间隔重复记忆卡片老牌开源 | Rust | 31,193 | +177⭐ | 3,237 |
| 10 | [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) | Claude Cowork 知识工作插件 | Python | 24,860 | +300⭐ | 2,969 |
| 11 | [supermemoryai/supermemory](https://github.com/supermemoryai/supermemory) | 本地极速 Memory API 引擎 | TypeScript | 30,242 | +140⭐ | 2,640 |
| 12 | [tradesdontlie/tradingview-mcp](https://github.com/tradesdontlie/tradingview-mcp) | Claude Code 接 TradingView | JavaScript | 6,450 | +64⭐ | 2,717 |
| 13 | [rustfs/rustfs](https://github.com/rustfs/rustfs) | Rust 版 S3 兼容对象存储 | Rust | 33,135 | +298⭐ | 1,483 |
| 14 | [supabase/supabase](https://github.com/supabase/supabase) | Postgres 开发平台老牌选手 | TypeScript | 110,126 | +128⭐ | 14,289 |
| 15 | [coder/coder](https://github.com/coder/coder) | 面向开发者与 Agent 的沙箱 | Go | 15,262 | +478⭐ | 1,503 |

---

## 重点项目点评

### 🥇 [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) — 今日榜首，+3,019⭐

**Agent Skill 生态第一个"标杆级"作品出自 Cloudflare**

Cloudflare 昨晚开源了这个 "coding-agent skill"，专门用于多阶段的自动化安全审计。项目一晚上收获 3019 颗星，几乎是当日 top 15 里其余项目的 star 总和。它的核心创新在于把安全审计拆成了 **fetch → categorize → verify → report** 四阶段流水线，其中最关键的 verify 阶段由独立的子 agent 完成，产出机器可读的 JSON findings。这是 skill 模式（一次 workflow、可复用、可验证）第一次在**大厂主导**下形成的完整开源模板。

背后的信号极强：**Cloudflare 官宣加入 Claude Skills 生态**。项目 README 明确说明它兼容 Claude Code、Cursor 以及任何遵循 Skills spec 的 agent runtime。过去 6 个月里，addyosmani/agent-skills 和 anthropics 自己的 skill 集合一直是社区默认参考，但都还偏"个人项目"气质；Cloudflare 这次的入场意味着 skill = 新 SDK 的说法从社区共识变成了商业共识。

对 side-project 作者的启发：如果你有一个"多步骤 + 需要验证 + 结果要可复审"的场景，把它写成 skill 会比写成 CLI/library 更快获得关注。今天的榜首是最好的社会证明。

---

### 🥈 [alibaba/open-code-review](https://github.com/alibaba/open-code-review) — +2,724⭐

**阿里首次以官方账号强势冲榜——目标很明确：把 code review 变成必装 Agent**

阿里巴巴开源账号今天上线了 open-code-review，一天冲上第 3。这是阿里巴巴少数几次以 `alibaba/` 组织名冲上 GitHub Trending 首页，上一次是 Qwen 系列。项目定位"混合架构 code review"：**确定性 pipeline**（静态分析、lint、依赖漏洞扫描）负责快、稳、可复现的部分，**LLM Agent**负责语义、架构、代码坏味道的判断。多语言支持覆盖了 Java、Go、Python、TypeScript、C++、Rust。

真正让它冲榜的原因不是技术，而是**时机**：GitHub 原生 Copilot Review、Anthropic 官方 code-review skill、Amazon CodeGuru 三家都在过去两周有大动作。阿里挑这个时点开源，摆明了要给行业一个"不绑 Copilot、不绑 Anthropic、不绑 AWS"的第三选项。对国内私有化部署场景（政企、金融、军工），open-code-review 因为 Go 实现 + 支持内网 LLM，落地阻力显著低于任何一家美国方案。

配合 Qwen3-Max 等自研模型，这条产品线的野心其实是"阿里云上一站式 AI DevOps"，值得持续观察。

---

### 🥉 [Tencent/BrowserSkill](https://github.com/Tencent/BrowserSkill) — +1,319⭐

**"Agent 接管你已经登录好的浏览器"——2026 年新赛道正式开火**

Tencent/BrowserSkill 走的路线和 Anthropic Computer Use、OpenAI Operator 完全不同——它不启动新浏览器、不重新登录，而是通过一个浏览器扩展 + CLI 桥，把 AI Agent 直接注入你**当前正在使用的**浏览器。所有网站身份都由你本人保留，Agent 只有"操作权"没有"凭据"。这是过去半年"浏览器 Agent"这个赛道最尖锐的一个体验切入点。

技术实现上，它借助 Chrome 的 Native Messaging + WebSocket 通道打通 CLI 与浏览器扩展。安全模型是**能力受限**（只允许特定 tab、特定 domain）而不是**凭据授权**。这规避了 OAuth 授权/Cookie 泄露的最大风险，也让企业 IT 更容易接受。

腾讯这次冲榜说明国内大厂在"Agent 落地场景"上已经完成技术选型：**不与 OpenAI/Anthropic 在通用 Agent 层拼命，而是在垂直动作层直接落地**。BrowserSkill、Alibaba 的 open-code-review 都在同一逻辑下——**用垂直 Agent 抢应用层入口**。

---

### 4️⃣ [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — +677⭐

**Google DevRel 大佬亲自维护的生产级 Skill 集合，一周内翻倍**

Addy Osmani 一贯的品味代表着 Google 前端 DevRel 的品味。这个仓库是过去 60 天里 star 增长最快的 Agent 相关项目之一，今日新增 677⭐。集合中包含 code refactor、TDD workflow、a11y audit、performance triage 等 30+ 个 Skill，每个都提供了 SKILL.md、评估用例和真实生产反馈数据。

结合今天 #1 的 Cloudflare security-audit-skill、#10 的 Anthropic knowledge-work-plugins，可以说 **"Skill" 正在成为 2026 年 Agent 世界的 npm package**。生态飞轮已经形成：Anthropic 定义标准 → 大厂做参考实现 → 个人开发者聚拢标准。

---

### 5️⃣ [rustfs/rustfs](https://github.com/rustfs/rustfs) — +298⭐

**Rust 版 MinIO 替代品——低调稳增，暗流涌动**

rustfs 是一个 Rust 实现的 S3 兼容对象存储，主打"MinIO 迁移体验"。今日新增 298⭐，看似不多但已经是连续第三周稳定进入 Trending。项目重点是**内存效率 + AI 训练数据场景**：面向 PB 级数据集、支持零拷贝对象存取、异步 IO 深度优化。

在 MinIO 母公司近期改变许可（AGPLv3 + 商业授权双轨）后，社区对开源 S3 替代品的胃口空前旺盛。SeaweedFS、Garage、rustfs 三家在过去一年都在收割 MinIO 用户。选择 Rust 而不是 Go，是因为 AI 数据管道场景对内存和 GC 停顿非常敏感。这个项目虽然不刷屏，但**是最能预测 2027 年基础设施走向的信号**之一。

---

## 生态观察

**主题一：Skill = 2026 年的 npm package。** 今日榜单里，`cloudflare/security-audit-skill`、`addyosmani/agent-skills`、`anthropics/knowledge-work-plugins`、`Tencent/BrowserSkill` 四条同时上榜，且 3 条进入 top 6。这不是巧合，而是标准形成的最后阶段——Anthropic Skills spec 已经被 Cloudflare、腾讯、阿里、Google DevRel 分别以不同方式确认接受。**未来 6 个月，一个新工具如果不能被写成 Skill，将无法进入主流 Agent 工作流。**

**主题二：Claude 生态占据半壁江山。** claude-code、knowledge-work-plugins、tradingview-mcp（Claude Code 接 TradingView）、coder/coder（面向 Agent 的沙箱）、以及大量 Skill 项目都直接引用 Claude Code 或 Claude Agent SDK。相比之下，OpenAI/Codex/ChatGPT Enterprise 相关项目今日几乎全部落榜。**GitHub Trending 已经成为 Claude 生态的主场。**

**主题三：中国大厂开始集中冲榜。** alibaba/open-code-review、Tencent/BrowserSkill、TencentCloud/Octop 同一天进入 top 10，是 2026 年 Q3 以来最密集的一次。策略共性很清楚：**不去与美国大厂正面较量通用模型，而是抢应用层入口和垂直 Agent**。

**主题四：Rust 系统软件继续稳步收割。** rustfs、anki（Rust 重写完成）、以及大量小型 Rust 工具的存在，说明 Rust 已经从"新兴替代"进入"默认选择"的阶段——尤其在存储、内存敏感、AI 数据管道领域。

**主题五：Postgres 平台化继续。** supabase 单日 +128⭐ 稳增，长期依然是 "Postgres 平台化"路线的绝对赢家。今天没有强势竞品挑战它。

---

_数据截至 2026-09-19（Asia/Shanghai）_
