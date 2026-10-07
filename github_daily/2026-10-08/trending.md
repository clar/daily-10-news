# GitHub Trending 日报 · 2026-10-08

## 今日焦点

> **Agent Skills 大爆发·逆向工程 AI 化·游戏主机破壁·自建工具复兴**
>
> - `morluto/rea` **+4,666⭐**：AI 驱动的全栈逆向工程套件，从行为到原生二进制一键剥
> - `boykopovar/AnyPS5` **+2,725⭐**：把 PS5 可执行文件自动移植到 Linux/Windows 的工具，HN 评论区在争法律边界
> - `mattpocock/skills` **+1,406⭐**：Agent "技能库"概念全面流行，前 15 名有 6 个都是技能相关
> - `DuarteSantos8/openGym` **+1,494⭐**：self-hosted 健身跟踪，self-hosted 复兴继续
> - `tester-army/e2e` **+1,391⭐**：Playwright/Cypress 之后的新一代 E2E 测试框架

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [morluto/rea](https://github.com/morluto/rea) | AI Agent 驱动的全链路逆向工具箱 | TypeScript | 14.6K | +4,666⭐ | 1,539 |
| 2 | [boykopovar/AnyPS5](https://github.com/boykopovar/AnyPS5) | PS5 可执行文件自动移植到 Linux/Windows | C++ | 10.3K | +2,725⭐ | 780 |
| 3 | [DuarteSantos8/openGym](https://github.com/DuarteSantos8/openGym) | self-hosted 健身与体重跟踪 | JavaScript | 6.8K | +1,494⭐ | 899 |
| 4 | [mattpocock/skills](https://github.com/mattpocock/skills) | Matt Pocock 整理的 Agent 工程技能库 | Shell | 279.5K | +1,406⭐ | 23.4K |
| 5 | [tester-army/e2e](https://github.com/tester-army/e2e) | 新一代 Web+Mobile 端到端测试框架 | TypeScript | 7.4K | +1,391⭐ | 332 |
| 6 | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | 42 种编辑风格图表技能（HTML/SVG） | HTML | 44.9K | +828⭐ | 2,883 |
| 7 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | Addy Osmani 的生产级 Agent 技能集 | JavaScript | 102.8K | +693⭐ | 10,765 |
| 8 | [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) | ADHD 友好的 coding agent 输出规范 | Python | 55.1K | +620⭐ | 3,158 |
| 9 | [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) | Cloudflare 开源的多阶段安全审计 Agent 技能 | JavaScript | 26.0K | +617⭐ | 1,564 |
| 10 | [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | Claude Agent 会话压缩与长时记忆注入 | TypeScript | 97.7K | +578⭐ | 8,600 |
| 11 | [trycua/cua](https://github.com/trycua/cua) | 开源 Computer Use 平台 + 跨 OS 评测 | Rust | 28.7K | +229⭐ | 2,038 |
| 12 | [manaflow-ai/cmux](https://github.com/manaflow-ai/cmux) | Ghostty 内核的 macOS AI 终端 | Swift | 27.8K | +96⭐ | 2,460 |
| 13 | [EpicGames/raddebugger](https://github.com/EpicGames/raddebugger) | Epic 开源的多进程图形化调试器 | C | 7.8K | +82⭐ | 381 |

---

## 重点项目点评

### 🥇 [morluto/rea](https://github.com/morluto/rea) — 今日榜首，+4,666⭐

**AI 代理第一次把"全链路逆向工程"做成一键产品**

rea 是一款由 AI Agent 驱动的逆向工程套件，涵盖**应用行为抓取 → 协议还原 → 原生二进制反编译**全链路。过去这些能力分散在 Frida、Ghidra、IDA、Burp、mitmproxy 等工具里，各自为政；rea 的做法是把 Agent 当 orchestrator，让 LLM 根据目标自动选择、串联这些工具并输出结构化报告。

它爆火不只是因为"AI + 逆向"的高话题性，更因为踩中两个趋势：（1）Claude Haiku 5.5 和 Gemini 3.8 Flash 让"小模型跑逆向流水线"的成本首次低于人工审计；（2）Cloudflare 刚开源 security-audit-skill（见下文），行业默认 AI 做安全审计正在正当化。但也要注意合规雷区——评论区已经有人在讨论此类工具是否违反 DMCA §1201 的反规避条款，特别是在被用于游戏/固件场景时（配合今天的 AnyPS5）。

---

### 🥈 [boykopovar/AnyPS5](https://github.com/boykopovar/AnyPS5) — +2,725⭐

**PS5 移植到 PC 的灰色地带新前线**

AnyPS5 声称可以自动把 PS5 平台的可执行文件迁移到 Linux 和 Windows，运行机制结合了反编译 + 用户态系统调用翻译。它的技术基线类似 Yuzu/Ryujinx（Nintendo Switch 模拟器）或 RPCS3（PS3），但目标是**现世代**主机，这在法律层面显著更危险。

Yuzu 2024 年被 Nintendo 诉讼后关门留下的教训很清楚，但 2026 年 AI 加速逆向使"门槛下降速度 > 诉讼响应速度"。短期内 AnyPS5 可能面临 Sony 的 DMCA 下架申请；中长期它折射的事实是：**AI Agent + 自动化移植正在让主机厂商的平台封闭策略不再可持续**。另外要留意 fork 数（780）相对星数的比例，这是典型"保存备份"行为，社区认为仓库随时可能被下架。

---

### 🥉 [mattpocock/skills](https://github.com/mattpocock/skills) — +1,406⭐（总 279.5K）

**"Agent 技能库"概念正式成型，TypeScript 教父入局**

Matt Pocock（TypeScript 教学圈顶流）把自己长年用 Claude Code / Cursor / Cline 积累的 Agent 技能整理成仓库，瞬间冲上 1.4K 星/日。重点不在仓库内容本身，而在**它和同时在榜的 addyosmani/agent-skills（102K 星）、cathrynlavery/diagram-design（44K 星）、ayghri/i-have-adhd（55K 星）、cloudflare/security-audit-skill（26K 星）构成了一个清晰趋势**：

> 2026 下半年，Agent 的护城河正在从"模型质量"转向"技能库资产"。

这意味着未来一年企业 AI 布局会多出一个新预算栏——"自建技能库 / 采购技能库"，和模型订阅并列。Claude Code 的 Skill 机制、Cursor 的 Rules、Cline 的 Workflow 都在卷同一个方向。谁率先把安全审计、E2E 测试、合规审计做成行业默认 Skill 格式，谁就能定义下一个标准（JSON Schema 层级的）。

---

### 🏅 [DuarteSantos8/openGym](https://github.com/DuarteSantos8/openGym) — +1,494⭐

**self-hosted 复兴浪潮里的新爆款**

openGym 是一款开源的自建健身追踪应用，覆盖训练日志、肌肉群分布、历史数据导入等功能。它能冲进 Top 3 的直接原因是——Strong、Hevy、Fitbod 等商业健身 app 2026 年集体涨订阅价，社区再次出现"自己托管"的报复性潮流。配合 Immich（照片）、Nextcloud、Audiobookshelf 等老牌 self-hosted 项目的持续火热，个人数字生活"去订阅化"趋势稳固。

值得注意的是，openGym 完全未提及 AI 功能——在今天的 trending 榜上这反而成了差异化卖点。它和 cmux、raddebugger 一起证明：**社区开发者在 AI 疲劳初现时，正在重新给"纯工具属性"项目留出位置**。

---

### 🔧 [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) — +617⭐

**Cloudflare 把安全审计做成"可携带 Agent 技能"**

Cloudflare 开源了一款面向 coding agent 的多阶段安全审计技能，设计上明确输出"机器可读的 verified findings"。这是 Big Tech 第一次把安全审计流程以"Skill 格式"开源，意义相当于 2015 年 Netflix 开源 Chaos Monkey——它定义了后续 security-as-a-skill 的接口标准。

搭配今天 morluto/rea 的 AI 逆向工具爆火，可以预见未来 12 个月**"AI Agent 做渗透测试 vs AI Agent 做审计"**会形成攻防双边军备竞赛。Cloudflare 把审计 skill 开源本质上是在"收编"社区——免费给防守方工具，确保 Cloudflare 云平台成为最终的受益方（捕获合规数据流）。

---

## 生态观察

今天最明显的信号是 **Agent Skills 彻底破圈**：Top 15 中有 6 个（mattpocock/skills、addyosmani/agent-skills、cathrynlavery/diagram-design、ayghri/i-have-adhd、cloudflare/security-audit-skill、thedotmack/claude-mem）都在围绕"如何让 AI Agent 更靠谱"。这个方向从 9 月末开始爆发，今天到达分水岭——TypeScript 教父 Matt Pocock、Chrome DevRel Addy Osmani、Cloudflare 公司账号同时入场，相当于盖章宣布"Skill 文件夹是开发者 2027 年必须认识的格式"。

次主线是**"AI 加速逆向工程"**。rea 和 AnyPS5 的组合证明，LLM 已经把二进制逆向、协议还原、系统调用翻译这些传统上需要专家级人力的工作民主化。接下来 2–3 个季度，游戏主机、消费电子固件、SaaS 协议私有化三条战线都会被这股浪潮冲击，法律摩擦可能会在 Q1 2027 集中爆发。

降温的方向：pure framework（React / Vue / Rust Web 框架）类项目今天完全没进榜。Agent 相关的"组合层"项目吃掉了全部社区注意力，底层技术栈项目被结构性边缘化——这不等于基础设施不重要，而是**社区阶段性对"马上能用"的东西更饥饿**。
