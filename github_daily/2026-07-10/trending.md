# GitHub Trending 日报 · 2026-07-10

## 今日焦点

> **AI Agent 生态大爆发 · Anthropic 系仓库刷屏 · 系统提示词泄露成新流量密码 · Claude 视频/桌面工具链齐跳增**
>
> - `addyosmani/agent-skills` +2,554⭐，谷歌前 Chrome 高管出品的"AI 编码代理生产级技能库"直冲榜首。
> - `VoltAgent/awesome-design-md` +1,391⭐，把品牌 DESIGN.md 变成 UI 生成上下文，AI 与设计系统的第一次握手。
> - `iOfficeAI/OfficeCLI` +1,929⭐，专为 AI Agent 操作 Word/Excel/PPT 而生的命令行套件。
> - `asgeirtj/system_prompts_leaks` +1,125⭐，主流 AI 厂商系统提示词大集合，一周内星标暴涨。
> - `bradautomates/claude-video` +718⭐，让 Claude 通过帧提取+转录理解视频，Anthropic 生态外延持续扩张。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | AI 编码代理生产级技能集 | JavaScript | 76,260 | +2,554 | 8,189 |
| 2 | [iOfficeAI/OfficeCLI](https://github.com/iOfficeAI/OfficeCLI) | AI Agent 操作 Office 三件套 | C# | 13,865 | +1,929 | 939 |
| 3 | [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) | 品牌 DESIGN.md 用于 UI 生成 | Multi | 100,229 | +1,391 | 11,602 |
| 4 | [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) | 各家 AI 系统提示词泄露合集 | JavaScript | 55,463 | +1,125 | 9,160 |
| 5 | [bradautomates/claude-video](https://github.com/bradautomates/claude-video) | Claude 视频理解封装 | Python | 6,888 | +718 | 782 |
| 6 | [vxcontrol/pentagi](https://github.com/vxcontrol/pentagi) | 全自主渗透测试 Agent 系统 | Go | 19,642 | +535 | 2,639 |
| 7 | [SmartlyDressedGames/U3-SDK](https://github.com/SmartlyDressedGames/U3-SDK) | Unturned 僵尸生存开源代码 | C# | 2,194 | +524 | 279 |
| 8 | [huxingyi/autoremesher](https://github.com/huxingyi/autoremesher) | 3D 网格自动四边化重建 | C++ | 2,445 | +403 | 179 |
| 9 | [prisma/prisma](https://github.com/prisma/prisma) | 下一代 Node.js/TS ORM | TypeScript | 47,039 | +376 | 2,453 |
| 10 | [imthenachoman/How-To-Secure-A-Linux-Server](https://github.com/imthenachoman/How-To-Secure-A-Linux-Server) | Linux 服务器安全指南 | Markdown | 29,250 | +243 | 1,942 |
| 11 | [kyutai-labs/pocket-tts](https://github.com/kyutai-labs/pocket-tts) | 面向 CPU 的轻量 TTS | Python | 7,115 | +235 | 710 |
| 12 | [unclecode/crawl4ai](https://github.com/unclecode/crawl4ai) | LLM 友好开源爬虫 | Python | 72,030 | +215 | 7,387 |
| 13 | [anthropics/claude-cookbooks](https://github.com/anthropics/claude-cookbooks) | Claude 官方最佳实践 | Jupyter | 47,323 | +194 | 5,565 |
| 14 | [wonderwhy-er/DesktopCommanderMCP](https://github.com/wonderwhy-er/DesktopCommanderMCP) | Claude 桌面终端/文件 MCP | TypeScript | 6,707 | +185 | 879 |

---

## 重点项目点评

### 🥇 [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — +2,554⭐

**Google Chrome 前工程主管 Addy Osmani 出手，把"AI 编码代理技能库"做成 npm 般的标准品**

Osmani 长年在前端性能领域立信，本次直接押注"AI Agent 需要工程级技能包"这一命题。仓库把常见的软件工程任务（TDD、code review、迁移、debugging）拆成可组合的 skill 模块，供 Claude Code / Cursor / Cline 直接调用；每个技能包含"何时启用、需要哪些工具、成功判定"，把过去散落在提示词工程社区里的经验固化。

单日 +2,554⭐ 的爆发背后是社区共识开始形成：**做通用 Agent 已经不是"提示词+模型"够用的场景**，需要一个 npm/pip 式的技能包生态。Osmani 用他在 Chrome DevTools 时代做扩展和最佳实践的方法论把这件事标准化——这可能是 2026 下半年最重要的 Agent 基础设施命题。

---

### 🥈 [iOfficeAI/OfficeCLI](https://github.com/iOfficeAI/OfficeCLI) — +1,929⭐

**为 AI Agent 而生的 Office 三件套**

跳过 Office 365 API 的繁琐授权、跳过 UI 自动化的脆弱，直接给 AI Agent 提供一个 CLI，可以本地操纵 Word/Excel/PowerPoint 文件——这就是 OfficeCLI 的产品切入点。C# 实现原生对接 Windows COM，同时保持 CLI 抽象，对企业内网部署的 Agent 尤其友好。

上线不久即冲上 1.3 万星，说明**企业 Agent 场景的第一波真实需求正在集中释放**——不是"生成 PPT 大纲"，而是"帮我把这份 100 页财报里的 15 张表复制到季度 review 模板里"。当 GPT-5.6 Sol 和 Sonnet 5 的代理能力升级到能"看懂多步任务"，缺的就是这种直接对物的工具适配层。

---

### 🥉 [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) — +1,391⭐

**把品牌 DESIGN.md 变成 AI 生成 UI 的官方 context**

仓库整理了主流品牌（Airbnb、Stripe、Vercel、Linear 等）的设计系统文档，用统一的 DESIGN.md 格式表达"这个品牌的颜色、字体、组件规范"。逻辑很清楚：Cursor / v0 / Lovable 这些 AI UI 生成工具需要一个可 attach 的品牌上下文文件，才能一致地产出"看起来是同一家公司"的界面。

这条赛道过去被 tokens.json、Figma variables 占据，DESIGN.md 是 AI 时代的原生解法——**文本、可 diff、可 fork**。10 万⭐+ 的历史存量说明它已经变成一个隐性事实标准，Vercel 的官方博客 6 月已经把 DESIGN.md 列入"AI 项目推荐配置"。

---

### 🎖️ [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) — +1,125⭐

**"抄谁的作业"成为 2026 年的编程新技能**

仓库汇总了 Claude、ChatGPT、Gemini、Perplexity、Cursor、v0、Copilot 等主流产品的（据称）泄露系统提示词。每次头部厂商更新产品，作者跟着抓包，社区拿来对着自己的 Agent 提示词做 diff。

这类仓库过去偶尔冲一次热榜就沉，本次持续走高背后是**"提示词工程"的方法论转变**：不再靠 A/B 生成，而是逆向头部产品——GPT-5.6 Sol 的 ultra 模式如何拆子代理？Cursor 是怎么处理 tool_use 循环的？答案都在这里，而不在博客里。这是"逆向工程 AI 产品"作为独立学科出现的信号。

---

### 🏅 [bradautomates/claude-video](https://github.com/bradautomates/claude-video) — +718⭐

**在 Anthropic 尚未官方支持视频输入之前，社区先跑起来**

Claude 目前的 API 只原生支持文本+图像；视频要"看"，社区先自己解决：帧提取（用 ffmpeg 切关键帧）+ Whisper/Deepgram 转录 + 时间轴 tag，最后拼成 Claude 能吃的多模态输入。仓库热度爆棚源于 Sonnet 5 的代理能力升级后，社区开始把 Claude 塞进"分析监控视频、拆解教程、剪辑摘要"等场景。

一个有意思的信号：**当官方多模态还没跟上时，社区会用最脏的胶带把能力糊出来**——这类项目也是 Anthropic 观察真实需求的信号源，Claude Video 的走热几乎可以预告下一次 API 更新方向。

---

## 生态观察

**今天首页几乎是 Anthropic 生态的一次校阅**：agent-skills（Skill 标准）、claude-video（视频输入垫片）、claude-cookbooks（官方教程）、DesktopCommanderMCP（MCP 桌面控制）、system_prompts_leaks（含 Claude）——从工程范式、模态扩展、系统集成、逆向学习四个方向同时热起来。这说明 Sonnet 5 和 Fable 5 回归后，**Claude 生态的开源开发者密度已明显超过其他厂商**。

第二个信号是"**AI Agent 从演示走向工具箱**"：agent-skills / OfficeCLI / awesome-design-md 都是**给 Agent 补零件**的仓库，而不是"又一个新 Agent 框架"。这种趋势和一年前"Auto-GPT / BabyAGI / CrewAI 竞速"完全相反——2026 下半年的赢家不是又一个编排器，而是能被现有编排器直接 `import` 的 skill 包。

第三个隐性信号是**语言分布回归多样**：C#（OfficeCLI、Unturned）、Go（pentagi）、C++（autoremesher）都上榜。过去几个月 GitHub trending 几乎被 Python / TypeScript 占据，本次多语言并存说明"AI 支线基础设施"正在往传统企业软件领域渗透——那些非 Python 的老栈也在被 AI 重新点燃。
