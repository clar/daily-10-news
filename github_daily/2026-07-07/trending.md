# GitHub Trending 日报 · 2026-07-07

## 今日焦点

> **Claude Skills 生态井喷 · Agent 工程化工具集 · 系统提示词泄漏再度登顶 · 会议助手本地化 Rust 复兴 · Web 抓取仍是 Agent 刚需**
>
> - `asgeirtj/system_prompts_leaks` +1,386⭐ 各家 AI 系统提示词大合集再登榜首，Fable 5 与 Opus 4.8 新条目引爆
> - `addyosmani/agent-skills` +1,114⭐ 生产级 AI 编码 Agent 技能库，Google 前 Chrome DevRel 亲自维护
> - `Zackriya-Solutions/meetily` +2,493⭐ 隐私优先本地 Rust AI 会议助手，日增第一
> - `Leonxlnx/taste-skill` +1,453⭐ "给 AI 灌注品味"的技能包，反对 LLM 生成"平庸稿"
> - `alirezarezvani/claude-skills` +611⭐ 345+ Claude 技能大杂烩，反映 Skill 生态从工具走向平台

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) | AI 系统提示词泄漏汇总（含 Fable 5、Opus 4.8） | JavaScript | 51,417 | +1,386 | 8,382 |
| 2 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 生产级 AI 编码 Agent 技能仓库 | Shell | 70,734 | +1,114 | 7,666 |
| 3 | [Zackriya-Solutions/meetily](https://github.com/Zackriya-Solutions/meetily) | 隐私优先本地 Rust AI 会议助手 | Rust | 19,263 | +2,493 | 1,955 |
| 4 | [ruvnet/RuView](https://github.com/ruvnet/RuView) | WiFi 空间智能与生命体征监测 | Rust | 77,465 | +471 | 10,404 |
| 5 | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | 让 AI 有品味，摆脱"通用平庸稿" | JavaScript | 58,848 | +1,453 | 4,008 |
| 6 | [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills) | 345+ Claude 技能与 Agent 插件合集 | Python | 21,119 | +611 | 2,839 |
| 7 | [openai/codex-plugin-cc](https://github.com/openai/codex-plugin-cc) | OpenAI Codex 官方 Code Review 集成 | JavaScript | 26,247 | +910 | 1,572 |
| 8 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 全网跨平台话题研究 Skill | Python | 49,698 | +511 | 4,141 |
| 9 | [ogulcancelik/herdr](https://github.com/ogulcancelik/herdr) | 终端里的 Agent 多路复用器 | Rust | 12,823 | +783 | 746 |
| 10 | [bradautomates/claude-video](https://github.com/bradautomates/claude-video) | 让 Claude 能"看"视频 | Python | 4,165 | +539 | 596 |
| 11 | [karakeep-app/karakeep](https://github.com/karakeep-app/karakeep) | 自托管 AI 打标签书签工具 | TypeScript | 26,856 | +178 | 1,318 |
| 12 | [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) | Web 抓取搜索交互 API | TypeScript | 146,165 | +834 | 8,406 |
| 13 | [steipete/CodexBar](https://github.com/steipete/CodexBar) | Codex 和 Claude Code 使用统计 | Swift | 16,709 | +598 | 1,375 |
| 14 | [alibaba/zvec](https://github.com/alibaba/zvec) | 阿里进程内轻量级向量数据库 | C++ | 13,472 | +355 | 821 |
| 15 | [sindresorhus/awesome](https://github.com/sindresorhus/awesome) | Awesome 列表之王 | Markdown | 482,243 | +393 | 35,733 |

---

## 重点项目点评

### 🥇 [Zackriya-Solutions/meetily](https://github.com/Zackriya-Solutions/meetily) — +2,493⭐

**日增最猛：会议助手赛道的"本地化 + Rust"双 buff**

在 Otter/Fireflies 等 SaaS 会议助手已成红海的赛道，Meetily 用 **完全本地处理 + Rust 引擎 + 隐私优先** 做出了差异化，一天涨 2,493 星登顶日榜。它把 Whisper + LLM 归纳链路全塞进 Rust，音频不出机器，直接击中企业与律所对 SaaS 会议摘要的顾虑。

Rust 重回榜首前列并非偶然——今日 Top 15 里 Rust 项目占 3 席 (meetily、RuView、herdr)。**"性能敏感 + 隐私敏感 + Agent 场景"三合一场景，是 Rust 在 AI 时代找到的第二增长曲线**——不是替代 Python，而是包裹 Python，做本地端的执行层。

Meetily 的走红也预示了 2026 下半年 AI 硬件 (Mac Studio、Ryzen AI Halo) 落地场景的第一个 killer app：**离线可跑的会议 & 通话 assistant**。硬件正在追上模型能耗曲线，是这类项目突然可行的根本原因。

---

### 🥈 [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) — +1,386⭐

**AI 时代的"透明化施压"仓库：Fable 5、Opus 4.8 新提示词条目引爆**

这个仓库长期存在，但今天再次上榜跟 Fable 5 出口管制解除同步。它汇总了 Anthropic、OpenAI、Google 等主流 AI 产品的系统提示词——不是靠 API 猜出来的，而是通过用户 prompt injection、错误回显、bug bounty 等方式流出来的**真实内部指令**。

社区对这类仓库爱恨交织：**开发者视角**上，它是研究"防护栏、拒答策略、身份注入、工具使用规则"的一手资料，也是 Prompt Engineering 逆向学习最好的教材；**厂商视角**上，它相当于把商业机密开源，Anthropic 曾要求下架但被社区抵制。

新增 Fable 5 与 Opus 4.8 提示词让讨论重回热点，也从侧面回应了昨天 UN 日内瓦对话上的一个议题：**"厂商是否有义务公开安全 policy"**。仓库星标本身就是社区在用行动投票。

---

### 🥉 [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — +1,114⭐

**7 万星库继续加速：Google 明星工程师亲自维护的 Agent 技能圣经**

Addy Osmani（Google 前 Chrome 团队 DevRel Lead，畅销书作者）把他积累多年的 web performance & engineering 知识重构成 Claude Code 兼容的 Skills 库。它不是玩具，而是**围绕生产级 Agent 编码的完整能力模块**——性能审计、a11y 检查、bundle 分析、SEO 优化，一一封装成可复用 skill。

这个库把 Skills 生态推到了新阶段：**从"个人玩具技能包"过渡到"工业级最佳实践的标准分发方式"**。整个 Top 15 里有 4 个跟 Skills 直接相关 (agent-skills、taste-skill、claude-skills、last30days-skill)，说明 Claude Code 的 Skill 系统正在成为整个 AI 编码 Agent 生态的事实标准。

对比 Cursor、Windsurf 等 IDE 的"内置规则"，Skills 的开放格式让 Osmani 这样的社区领袖能主导规范，而不用等 Anthropic 官方每次发版本。这是产品设计上的一次以退为进。

---

### 🎨 [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) — +1,453⭐

**"给 AI 一些品味"：反 LLM 平庸稿的技能包爆红**

taste-skill 的自我定位是"stops the AI from generating boring, generic slop"。它做的事情很简单但击中痛点——通过一整套 prompt 模式、示例集与反面样本，让 Claude 在创意与文案任务上摆脱"官方 GPT 味"。它的走红本身就是社区对 LLM 生成物同质化的集体不满宣言。

从 5.8 万星和昨天大涨 +1,453 看，taste 这个抽象概念正在被工程化。开发者不再满足于"看起来能写"，而追求"写得像有人"。当 CNBC 观察到用户"从 tokenmaxxing 转向 efficiency"时，另一半故事就是**"从数量转向品味"**。

这也预示了 2026 下半年 Skill 生态的分化方向：**技术型 Skill (Osmani)** vs **审美型 Skill (Leonxlnx)** 会形成两条平行的高速轨道，各自吸引不同的开发者与内容创作者。

---

### 🔍 [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) — +834⭐

**14.6 万星库还在加速：Agent 抓 Web 这件事仍然没有被解决**

Firecrawl 是 Web 抓取 API 里的绝对头部。它今日仍能新增 834 星，说明 **Agent 的"看 web、读 web、抓 web"能力依然是一个远未定型的市场**。理论上 Claude 有 WebFetch、GPT 有 web search，但真正做生产级 Agent 时，工程师仍需要一层可控可预测的抓取层。

Firecrawl 的成功也解释了为什么 Anthropic 昨天上线 "Claude 科学工作台" 直接接入 60+ 数据库——**通用 web search 精度不够、结构化程度不够、可再现性不够**。垂直数据源 + 高质量抓取正在成为 Agent 应用差异化的关键要素。

---

## 生态观察

**Skills 生态从工具进化为经济。** 今日 Top 15 里 6 个直接与 Claude Skills 相关（agent-skills、taste-skill、claude-skills、last30days-skill、bradautomates/claude-video、CodexBar）。Skill 生态在 3 个月内从"配置文件集合"演化到"社区领袖亲自策展、跨平台复用"的开源分发标准。这是 2026 年最值得关注的生态位。

**Rust 找到 AI 时代第二身位。** Meetily、RuView、herdr 三个 Rust 项目集体进入 Top 15，方向惊人一致：**本地化 + 隐私 + Agent 运行时**。Rust 不做模型，做 LLM 的执行外壳与 IO 边界。这与 Python "写模型 + 训练 + 推理"分工明确，是 2026 下半年硬件本地化浪潮的直接受益。

**中国开源账户开始有存在感。** Alibaba/zvec 进入 Top 15，反映阿里在整合 AI 组织架构（昨日 Token 事业群成立）后，开始把内部基础设施对外开源。中国厂商的 GitHub 战略正从"翻译文档"进化到"开源核心组件"。

**"Agent 中间层"进入大爆发。** herdr (多路复用)、CodexBar (可视化统计)、codex-plugin-cc (工具桥接) 都指向同一个新兴子赛道：**Agent 的运维观测、多 Agent 编排、用量成本管理**。这是继模型层、Skill 层之后的第三个 Agent 生态卡位战。

---

*报告时间：2026-07-07（Asia/Shanghai）*
