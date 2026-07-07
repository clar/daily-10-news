# GitHub Trending 日报 · 2026-07-08

## 今日焦点

> **AI 求职工具霸榜 · 会议 AI 卷向本地 · Claude Skills 生态延伸 · System Prompt 泄露热议 · Rust 系统工具再起**
>
> - `MadsLorentzen/ai-job-search` 单日 +2,402⭐ 登顶，AI 时代求职工具进入实用化
> - `Zackriya-Solutions/meetily` +1,781⭐，Rust 写的本地会议助手，冲击 Otter/Fireflies
> - `asgeirtj/system_prompts_leaks` +1,704⭐，主流 AI 产品的 system prompt 泄露合集
> - `addyosmani/agent-skills` +1,311⭐，Claude Skills 玩法被前 Google 工程师系统化
> - `bradautomates/claude-video` +953⭐，Claude 视频代理，围绕 Claude 的第三方应用生态在成型

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ |
|------|------|------|------|--------|-----------|
| 1 | [MadsLorentzen/ai-job-search](https://github.com/MadsLorentzen/ai-job-search) | AI 求职助理，自动填表+匹配 | TypeScript | 10,592 | +2,402 |
| 2 | [Zackriya-Solutions/meetily](https://github.com/Zackriya-Solutions/meetily) | Rust 本地会议 AI 助手 | Rust | 20,635 | +1,781 |
| 3 | [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) | 主流产品 system prompt 泄露集 | JavaScript | 52,906 | +1,704 |
| 4 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | Claude Skills 玩法整理与示范 | JavaScript | 72,064 | +1,311 |
| 5 | [ruvnet/RuView](https://github.com/ruvnet/RuView) | Rust 编写的通用文件查看器 | Rust | 78,461 | +1,122 |
| 6 | [bradautomates/claude-video](https://github.com/bradautomates/claude-video) | Claude 视频代理框架 | Python | 5,105 | +953 |
| 7 | [iOfficeAI/OfficeCLI](https://github.com/iOfficeAI/OfficeCLI) | Office 全家桶命令行代理 | C# | 9,842 | +802 |
| 8 | [TencentCloud/CubeSandbox](https://github.com/TencentCloud/CubeSandbox) | 腾讯云出品的 Agent 沙箱 | Rust | 8,426 | +665 |
| 9 | [kyutai-labs/pocket-tts](https://github.com/kyutai-labs/pocket-tts) | Kyutai 端侧 TTS 引擎 | Python | 6,118 | +510 |
| 10 | [steipete/CodexBar](https://github.com/steipete/CodexBar) | macOS 菜单栏 Codex 客户端 | Swift | 17,010 | +377 |
| 11 | [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) | Claude Code 生态资源合集 | Python | 49,070 | +227 |
| 12 | [AhmadIbrahiim/Website-downloader](https://github.com/AhmadIbrahiim/Website-downloader) | 一键克隆网站的浏览器脚本 | HTML | 3,939 | +173 |
| 13 | [dotnet/skills](https://github.com/dotnet/skills) | .NET 官方推出的 Skills 集 | C# | 4,284 | +82 |

---

## 重点项目点评

### 🥇 [MadsLorentzen/ai-job-search](https://github.com/MadsLorentzen/ai-job-search) — 今日榜首，+2,402⭐

**AI 求职工具从"填表脚本"进化为"完整代理"**

这个 TypeScript 项目一天涨 2,402 星，直接冲进 GitHub 全站前列。它把 LinkedIn/Indeed/公司官网的求职流程做成一个 agent：自动抓 JD、和用户简历匹配、生成定制化 cover letter、自动填表、跟踪状态。区别于早期"简历生成器"类工具，它把整条求职流水线纳入代理框架。

爆红的时机不是偶然。7 月上旬正值美国大厂新一轮"AI 相关裁员"周期，OpenAI GPT-5.6 与 Anthropic Fable 5 的上市又直接冲击白领求职岗——尤其是软件、市场、法律助理这些原本"AI 补位"的岗位。求职者需要一个能匹配 AI 时代节奏的工具，而 ai-job-search 恰好把这个空缺填上。

它也预示了一个更大的趋势：**未来 12 个月，"AI 找 AI 工作"会成为一个独立赛道**，比 2015-2020 年的"Applicant Tracking System"更卷。Recruiter 端已经在用 AI 筛简历，求职者端也必须用 AI 反筛——博弈论上的均衡点会推动这个赛道大爆发。

---

### 🥈 [Zackriya-Solutions/meetily](https://github.com/Zackriya-Solutions/meetily) — +1,781⭐

**用 Rust 写的本地会议助手，直击 Otter/Fireflies 隐私痛点**

meetily 是一个纯本地会议 AI 助手：Rust 写的实时转录 + 本地 LLM 生成摘要 + 会议行动项抽取。用户不需要把音频送到云端。项目在过去 24 小时内涨 1,781 星，反映出对"云端会议 AI"的信任危机。

Otter、Fireflies、Grain 这些商业会议 AI 都有一个共同问题：会议内容进入云端后无法验证是否被用于训练。企业法务部门和高管群体对这类产品的抵触持续加剧——尤其是在欧盟 AI Act 8 月 2 日全面适用的档口。meetily 用 Rust 本地方案打这个市场的时机点非常准。

技术选型也值得注意：Rust 让它在 M 系列 Mac 和 Windows on ARM 上都能获得原生级性能，本地 whisper.cpp + llama.cpp 组合已经足够处理 4 小时会议。开源本地路线正在从 Ollama、LM Studio 这些 "chat" 场景扩展到**垂直生产力工具**。这是 2026 年下半年最值得跟踪的架构模式之一。

---

### 🥉 [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) — +1,704⭐

**System prompt 泄露合集：AI 产品的"源代码"再次被公开审视**

这个仓库汇集了 ChatGPT、Claude、Gemini、Perplexity、Cursor、Windsurf、v0 等主流 AI 产品的 system prompt 泄露版本。+1,704 星表明这是当下开发者社区最感兴趣的元问题之一。

爆红原因有二：第一，随着 AI 编程工具、Agent 平台在企业采纳率飙升，"到底给模型注入了什么指令"变成了合规、安全、产品对标的关键；第二，白宫昨日的 AI 治理框架和欧盟 AI Act 8 月 2 日全面实施都在强化 "AI 系统透明度"要求，system prompt 从"商业秘密"往"必须可审计"过渡。

对开发者而言，这些泄露文件也是一份免费的产品设计教材：Cursor 如何做代码补全的指令层、Perplexity 如何压制 hallucination、Claude 如何拒绝敏感请求——每一份都是一次 prompt engineering 的高浓度速成课。**这也解释了为什么这类"泄露仓库"在 GitHub 星标市场里持续有热度**。

---

### 4️⃣ [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — +1,311⭐

**前 Google 工程师系统整理 Claude Skills 玩法**

Addy Osmani（前 Google Chrome 工程师、《Learning JavaScript Design Patterns》作者）出手整理的 Claude Agent Skills 教程集。72,064 总星、+1,311 今日新增，标志着 Claude Skills 生态正在被"传统前端权威"背书，进入主流开发者视野。

Skills 是 Anthropic 6 月推出、7 月起在 Claude Code / Web / API 全线打通的能力封装机制——本质上是可复用的 agent 行为模板。Addy 的仓库把 Skills 从"Anthropic 的功能"抽象成"通用 AI Agent 模式"，把 Cursor、Windsurf、v0 用户也纳入受众。

**关键信号：Anthropic 的 Skills 正在成为 Agent 时代的"npm package"**。当足够多的社区教程、示例、awesome-list 出现，一个技术标准就完成了自我强化的第一步。今天 dotnet/skills 也进入热榜，微软 .NET 团队跟进说明这不是单一生态圈的自嗨。

---

### 5️⃣ [bradautomates/claude-video](https://github.com/bradautomates/claude-video) — +953⭐

**Claude 视频代理：多模态 agent 生态迎来第一个爆款第三方**

claude-video 是一个用 Claude 做视频理解、剪辑、生成脚本的框架。+953 星表明 Anthropic 上周更新 Claude 视频原生输入能力后，第三方生态在 72 小时内已经开始迭代出应用形态。

从产品角度看，claude-video 提供了一个 pipeline：视频输入 → Claude 多模态理解 → 生成分镜/剪辑指令 → 调用 ffmpeg 输出。这套架构和早期 GPT-4V 时代的"截图理解"不同——Claude 的原生视频输入让整个流程不需要拆帧再理解，端到端延迟大幅降低。

结合 Anthropic 今天开始对 Fable 5 转向按量计费，可以预判：**Claude Skills + 视频原生 + 按量计费**将构成一个新的开发者商业模式基础——很多小工作室会把过去在 CapCut、Descript 里手动完成的流程"Claude Agent 化"，按用量向客户收费。

---

## 生态观察

**Agent Skills 生态在成型。** addyosmani/agent-skills (+1,311)、hesreallyhim/awesome-claude-code (+227)、dotnet/skills (+82)、bradautomates/claude-video (+953) 四个仓同榜，说明 Claude Skills 从 Anthropic 的产品功能变成一个跨生态的开发范式。npm 化的信号已经很清晰。

**Rust 系统工具卷第二波。** meetily (+1,781, Rust)、RuView (+1,122, Rust)、CubeSandbox (+665, Rust) 三个 Rust 项目在热榜前 10 里占三席。第一波 Rust 热潮是命令行工具（ripgrep、fd、eza），这一波则是**AI 场景下的本地系统工具**——转录、代理沙箱、通用文件预览器。Rust 依然是"本地高性能 AI 应用"的默认选择。

**AI 求职工具是 2026H2 新赛道。** ai-job-search 一天涨 2,402 星，是本季度首次有"求职工具"冲上 GitHub 全站榜首。AI 时代的白领岗位挤压是催化剂，未来 6 个月这个赛道会出现 3-5 个具备商业化能力的项目。

**System Prompt 透明化压力上升。** asgeirtj/system_prompts_leaks 一天涨 1,704 星，与白宫 AI 治理框架、欧盟 AI Act 全面适用的时点高度耦合。**"AI 产品的系统提示"正在从商业秘密变成半公开的行业基础设施**。

---

*报告生成时间：2026-07-08（Asia/Shanghai）*
