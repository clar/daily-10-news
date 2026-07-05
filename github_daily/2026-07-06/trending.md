# GitHub Trending · 2026-07-06

## 今日焦点

> **Agent 生态爆发 · Claude Code Skills 集群 · 隐私 AI 会议 · 渗透测试自动化 · 中国 GUI Agent**
>
> - `Zackriya-Solutions/meetily` 以 **+1,409⭐** 登顶——Rust 写的本地会议助手，隐私 AI 打法开始拿到大量票数。
> - `openai/codex-plugin-cc` **+1,519⭐** 冲上第二——OpenAI 官方把 Codex 塞进 Claude Code 生态，Agent 互认打通新阶段。
> - `JuliusBrussee/caveman` **+1,043⭐** 已经累计 84.8k⭐，"Claude Code token 节流 skill" 变成新品类。
> - `usestrix/strix` **+1,121⭐**——开源渗透测试自动化，安全 Agent 首次跻身当周前十。
> - `alibaba/page-agent` **+801⭐**——阿里推 in-page GUI Agent，中国 Agent 派开始瞄准浏览器交互层。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [Zackriya-Solutions/meetily](https://github.com/Zackriya-Solutions/meetily) | 隐私优先的本地 AI 会议助手 | Rust | 16,811 | +1,409 | 1,791 |
| 2 | [openai/codex-plugin-cc](https://github.com/openai/codex-plugin-cc) | Codex 接入 Claude Code 代码评审 | JavaScript | 25,404 | +1,519 | 1,535 |
| 3 | [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) | Claude/ChatGPT/Gemini system prompt 泄漏合集 | JavaScript | 49,867 | +981 | 8,165 |
| 4 | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | 抑制 AI 生成"套话"的 Skill 框架 | JavaScript | 57,389 | +850 | 3,927 |
| 5 | [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills) | 337 个 Claude Code Skill 汇总 | Python | 20,510 | +394 | 2,794 |
| 6 | [rommapp/romm](https://github.com/rommapp/romm) | 自托管 ROM 管理器 | Python | 10,504 | +411 | 503 |
| 7 | [ogulcancelik/herdr](https://github.com/ogulcancelik/herdr) | 终端 Agent 多路复用器 | Rust | 12,013 | +650 | 700 |
| 8 | [alibaba/page-agent](https://github.com/alibaba/page-agent) | 页内 GUI Agent，自然语言控制网页 | TypeScript | 23,812 | +801 | 2,056 |
| 9 | [harvard-edge/cs249r_book](https://github.com/harvard-edge/cs249r_book) | 哈佛 ML 系统教材 | Python | 26,813 | +333 | 3,188 |
| 10 | [usestrix/strix](https://github.com/usestrix/strix) | 开源渗透测试自动化 | Python | 37,030 | +1,121 | 3,761 |
| 11 | [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) | Claude Code 资源集散地 | Python | 48,325 | +188 | 4,232 |
| 12 | [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | 面向营销的 AI Skill 集合 | JavaScript | 36,389 | +209 | 5,894 |
| 13 | [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) | 减少 Claude Code token 消耗的 Skill | JavaScript | 84,805 | +1,043 | 4,719 |
| 14 | [CoplayDev/unity-mcp](https://github.com/CoplayDev/unity-mcp) | Unity 编辑器 MCP 桥接 | C# | 11,902 | +415 | 1,276 |
| 15 | [facebook/astryx](https://github.com/facebook/astryx) | Meta 面向 Agent 设计的开源 Design System | TypeScript | 5,851 | +540 | 372 |

---

## 重点项目点评

### 🥇 [openai/codex-plugin-cc](https://github.com/openai/codex-plugin-cc) — +1,519⭐

**OpenAI 官方接入 Claude Code：Agent 生态互认里程碑**

这是过去 24 小时最戏剧化的事件——OpenAI 出人意料地发布了一个 Claude Code 官方插件，允许把 Codex（当前 GPT-5.6 三档模型）挂载进 Claude Code 的 skill/tool 系统里。这意味着开发者可以在同一个 CLI/IDE 环境里同时调用 Claude、Codex 两套底层模型，各取所长。

对生态影响非常直接：过去半年 Anthropic 的 Claude Code + Skill 生态膨胀速度极快（本次前 15 里有至少 6 个仓库都是 Claude Code 相关），OpenAI 选择"如果打不赢就先接入"的策略——让 Codex 的用户不用离开 Claude Code UI 就能用，等价于承认 Claude Code 已成为一部分开发者的默认工作环境。

Star 增速 +1,519 意味着仓库上线首日就冲到前二。技术圈普遍解读：这是 OpenAI 商业策略上向"开放互操作"的第一次让步，将来 xAI、Google DeepMind 可能会跟进同类插件。

---

### 🥈 [Zackriya-Solutions/meetily](https://github.com/Zackriya-Solutions/meetily) — +1,409⭐

**Rust + 本地推理的"隐私会议助手"，反 SaaS AI 情绪的直接受益者**

Meetily 用 Rust 写了一个完整的本地会议助手：本地转写 + 本地 LLM 生成摘要，全程不上云。对比 Otter.ai、Fireflies 等 SaaS 竞品，它的最大卖点不是精度，而是"你的对话内容永远不离开你的机器"。

这个仓库的爆发和整个 HN/开源社区当下的"用户主权"情绪高度呼应（HN 今日前 5 也是同一主线）。也在配合一个更宏观的趋势：本地推理硬件（Apple Silicon、AMD Strix Halo、Nvidia DGX Spark）在过去 6 个月出货量激增，"能在笔记本上跑 30B 模型"从少数极客走向普通开发者。

---

### 🥉 [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) — +1,043⭐

**"Claude Code Token 节流"成为新一代 skill 头部品类**

caveman 已经累计 84.8k⭐，是当前 Claude Code 生态里最大的 skill 型仓库。它的核心逻辑简单粗暴：把 Claude Code 的输出限制为极简、命令式风格，从而减少 token 消耗。据 README 里的实测数据，长会话可以省下 40–60% 的输出 token。

这个仓库暴露出 Claude Code 生态的核心痛点：token 成本已经成为大规模落地的最大摩擦。用户不缺工具，缺的是让工具"少花钱"的元工具。caveman 之后，"prompt 精简 skill"很可能像"lint 工具"一样标配化。

同类别的 `Leonxlnx/taste-skill`、`alirezarezvani/claude-skills`、`hesreallyhim/awesome-claude-code`、`coreyhaines31/marketingskills` 齐齐上榜，可以断定：Claude Skill 已经从"锦上添花"进化成了"必装底座"。

---

### 🔒 [usestrix/strix](https://github.com/usestrix/strix) — +1,121⭐

**Agent 系统首次进入"进攻性安全"主流视野**

Strix 是一个开源的渗透测试自动化框架，把 Agent 系统直接应用于漏洞发现、扫描、利用链构造。它的兴起标志着 Agent 的应用场景开始严肃跨入"进攻端"——过去几年安全 Agent 多用于防守（SOC 自动化），这次是首次有工具在渗透测试自动化上冲到 GitHub Trending 前十。

对企业来说这是双刃：安全团队获得新一代自动化红队工具；同时攻击面也在扩大，因为犯罪团伙同样可以用它做侦查。评论区已经在讨论"开源发布 vs 负责任披露"的伦理问题，社区目前的态度倾向于"透明化胜过被动"。

---

### 🇨🇳 [alibaba/page-agent](https://github.com/alibaba/page-agent) — +801⭐

**阿里推出 in-page GUI Agent，中国厂商杀入浏览器交互层**

page-agent 走的是"注入式 GUI Agent"路线：不做浏览器插件，而是直接以脚本形式加载进任何网页，让用户用自然语言指挥当前页面（填表、抓数据、多步操作）。相较 Anthropic 的 Computer Use、OpenAI 的 Operator，page-agent 的优势是"零特权、零安装"，网页开发者可以直接把它嵌入自家产品。

这也是中国 Agent 派系继阿里 Qwen-Agent、字节 Coze、月之暗面 Kimi Web 之后的又一次浏览器层落地，符合"中国 Agent 更贴近 SaaS 应用集成、美国 Agent 更贴近开发者 CLI"的分化格局。今天正好 GLM-5.2 也在 AI 日报里刷屏——中国 AI 层次的动作节奏明显加快。

---

## 生态观察

**主题一：Claude Code Skill 已从"扩展"变成"标配"。** 前 15 里有 6 个是 Claude Skill 相关（caveman、taste-skill、claude-skills、awesome-claude-code、marketingskills，加上 openai/codex-plugin-cc 也是接入 Claude Code）。这意味着"skill 生态"事实上取代了传统 IDE 插件，成为 AI 时代的开发者软件市场。

**主题二：Agent 应用往"垂直深井"下潜。** 会议（meetily）、渗透测试（strix）、Unity 游戏开发（unity-mcp）、营销（marketingskills）都在同一天出现——Agent 已经不再"通用"，而是被拆到各个垂直场景里再包装。

**主题三：本地推理生态在悄悄成型。** Rust 写的隐私 Agent (meetily, herdr) 密集出现，反映本地推理硬件普及后的开发者需求转变——"能在自己机器跑 + 隐私强" 是新一代 killer feature。

**主题四：System Prompt 泄漏仓库热度不减。** `system_prompts_leaks` 累计 49k⭐、今日 +981，反映的是"AI 公司越来越不愿意开源，但用户越来越想知道内部机制"的持续张力。这个矛盾短期内不会消退。
