# GitHub Trending 日报 · 2026-05-23

## 今日焦点

> **Claude Code 插件生态官方化 · 代码知识图谱集体爆发 · AI 编码代理工具链密集更新 · MCP 工具链下沉 · yt-dlp 回潮**
>
> - `anthropics/claude-plugins-official` 单日 +2,556⭐ —— Anthropic 亲自下场做插件商店式仓库，Claude Code 生态走向标准化
> - `colbymchenry/codegraph` 单日 +3,688⭐（涨幅榜首）—— 把 Claude Code 和其他 AI 编码工具接上本地代码知识图谱
> - `Lum1104/Understand-Anything` +1,391⭐ —— "把代码变成可探索查询的知识图谱"，与 codegraph 同主题双爆
> - `ChromeDevTools/chrome-devtools-mcp` +499⭐ —— Chrome DevTools 官方 MCP server，浏览器作为 agent 第一公民
> - `yt-dlp/yt-dlp` +536⭐ —— 因弃用 Bun 的公告被 HN 头条带火

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) | Anthropic 官方 Claude Code 高质量插件目录 | Python | 24,783 | +2,556 | 2,760 |
| 2 | [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) | 为 Claude Code 等 AI 编码工具提供本地代码知识图谱 | TypeScript | 16,397 | +3,688 | 905 |
| 3 | [ruvnet/RuView](https://github.com/ruvnet/RuView) | 基于 WiFi 信号的空间感知和无视频生命体征监测 | Rust | 63,963 | +992 | 8,452 |
| 4 | [rohitg00/ai-engineering-from-scratch](https://github.com/rohitg00/ai-engineering-from-scratch) | 从零开始学习构建并发布 AI 产品的教程 | Python | 11,816 | +988 | 2,255 |
| 5 | [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) | Chrome DevTools 官方 MCP 服务器 | TypeScript | 40,941 | +499 | 2,600 |
| 6 | [dotnet/skills](https://github.com/dotnet/skills) | 给 AI 编码代理用的 .NET/C# 技能库 | C# | 2,505 | +391 | 197 |
| 7 | [Lum1104/Understand-Anything](https://github.com/Lum1104/Understand-Anything) | 把代码转成可交互查询的知识图谱 | TypeScript | 18,417 | +1,391 | 1,671 |
| 8 | [odoo/odoo](https://github.com/odoo/odoo) | 开源企业应用全家桶 | Python | 51,105 | +48 | 32,514 |
| 9 | [byJoey/cfnew](https://github.com/byJoey/cfnew) | 社区驱动的 Cloudflare 工具集 | Multiple | 13,289 | +85 | 6,478 |
| 10 | [trimstray/the-book-of-secret-knowledge](https://github.com/trimstray/the-book-of-secret-knowledge) | 经典 CLI/Web 工具与运维秘籍合集 | Documentation | 223,163 | +964 | 13,379 |
| 11 | [Fincept-Corporation/FinceptTerminal](https://github.com/Fincept-Corporation/FinceptTerminal) | 金融终端，行情分析和研究工具 | Python | 22,597 | +337 | 3,121 |
| 12 | [can1357/oh-my-pi](https://github.com/can1357/oh-my-pi) | 终端里的 AI 编码代理，支持高级编辑 | TypeScript | 6,311 | +455 | 512 |
| 13 | [yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp) | 命令行音视频下载器 | Python | 164,287 | +536 | 13,820 |
| 14 | [karpathy/nn-zero-to-hero](https://github.com/karpathy/nn-zero-to-hero) | 神经网络基础课系列 | Jupyter Notebook | 22,305 | +270 | 3,242 |

---

## 重点项目点评

### 🥇 [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) — 今日涨幅榜首，+3,688⭐

**Claude Code 的"项目记忆"层在被开发者集体补齐**

codegraph 想解决一件具体的事：让 Claude Code、Cursor 等编码代理在调用前先看一张当前仓库的依赖/调用图，再决定要读哪些文件。所有处理都本地完成，不上云、不联网。这正好踩在所有"重 IO + 大仓库"用户的痛点上——Claude Code 默认靠 grep 探索代码，仓库一大就容易兜圈子。

它的爆火只是冰山一角：今天同主题的 `Lum1104/Understand-Anything` 也涨了 1,391⭐，主打"把代码变成可查询的知识图谱"。两个项目核心思路一致：**用确定性的图数据结构给 LLM 当"prior"，把 token 花在推理而不是搜索上**。这是 2026 年代理工具链的一条主线——从"给 LLM 更多 token"演化到"让 LLM 看到更少但更准的 token"。

未来 1–2 个月预测：Anthropic 官方很可能会在 Claude Code 里集成类似能力（甚至直接采购或合并这一类项目），就像它今天直接下场做 plugins-official 仓库一样。

---

### 🥈 [anthropics/claude-plugins-official](https://github.com/anthropics/claude-plugins-official) — +2,556⭐

**Claude Code 从"工具"走向"操作系统"的关键一步**

这是 Anthropic 官方维护的"高质量插件目录"，意味着 Claude Code 终于有了一个相当于 VS Code Marketplace 的官方策展层。背后逻辑很清楚——过去半年 Claude Code 上的 skill / hook / MCP 生态野蛮生长，第三方插件良莠不齐，用户在选型阶段的认知成本极高。Anthropic 用一个"官方背书"的清单收口。

商业上更重要的是它给"专业插件作者"开了空间：进入官方目录就意味着可信度，开发者愿意为之投入精力。结合昨日 Project Glasswing 的 50 家伙伴生态，Anthropic 正在快速搭建一个"前沿模型 + 编码代理 + 安全代理 + 官方插件"四件套，剑指企业市场。

对比 OpenAI Codex 的相对封闭路线，这是 Anthropic 当前最重要的差异化。

---

### 🥉 [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) — +499⭐

**MCP 标准的"操作系统级"代表性接入**

Chrome DevTools 官方下场做 MCP server——这是过去 3 个月里 MCP 标准化进程中最有分量的一次接入。意味着 Claude、ChatGPT、Cursor 等任何支持 MCP 的代理，都能直接调用浏览器的 DOM 检查、network 抓包、performance 录制等能力，不再需要每家自己写 puppeteer 包装。

把今天的 chrome-devtools-mcp、`dotnet/skills` 一起看，整张图就清晰了：**主流大厂在把自家产品 SDK 改造成"代理可调用"的形态**。MCP 在 2026 上半年从 Anthropic 内部标准已经基本变成事实标准，类似 LSP 在 IDE 圈的角色。下一个看点：苹果会不会把 Xcode 工具链做成 MCP server。

---

### 🛰️ [ruvnet/RuView](https://github.com/ruvnet/RuView) — +992⭐（累计 63,963⭐）

**WiFi 信号开始变成 "环境感知"层**

不属于 AI 编码代理主线，但今天非常值得专门点名。RuView 用商用 WiFi 信号做空间感知和无接触生命体征监测——本质是把 CSI（Channel State Information）当成雷达数据用。这条技术线在学术圈走了十年，今天第一次有 Rust 实现拿到 6 万星量级。

它的潜在场景值得一并指出：智能家居（无摄像头的存在感检测）、老人监护（无视频的心率/呼吸频率）、安防（穿墙检测）。三者都对"摄像头隐私"敏感人群非常友好——这是技术伦理上少有的"用更少数据做更多事"的正向案例。

---

### 📥 [yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp) — +536⭐（累计 164,287⭐）

**HN 头条带来的回流，但意义不止于"被讨论"**

yt-dlp 因今天 HN 上的"弃用 Bun"公告 重新获得关注。在 16 万星的体量上单日多 500 颗星算不了什么，但有意思的是后续效应：很多开源项目维护者把 yt-dlp 这条公告当模板转发，作为"我们对 AI 生成代码的官方立场"。这是 2026 年开源项目首次开始公开化"AI 代码可接受范围"政策。

预计未来一个月会有更多大型项目在 CONTRIBUTING.md 中加入类似条款。开源治理正在被迫面对"AI 提交比例"这个新议题。

---

## 生态观察

**1. AI 编码代理工具链已经从"主代理"扩展到"主代理 + 子工具集群"**——从 codegraph、Understand-Anything 这种代码图谱，到 chrome-devtools-mcp、dotnet/skills 这种领域 skills，再到 oh-my-pi 这种终端代理，今天榜上一半项目都是"给 Claude / Codex / Cursor 用的零件"。Anthropic 推 plugins-official 就是要把这堆零件官方收口。

**2. 知识图谱回归**——前几年被 LLM 浪潮压抑的 KG 思路重新成为热点，主因是 LLM 在大仓库上的"上下文盲点"开始被严肃对待。codegraph + Understand-Anything 双爆不是巧合，这条线接下来 6 个月会持续。

**3. 教程类项目稳定有市场**——`rohitg00/ai-engineering-from-scratch` 和 `karpathy/nn-zero-to-hero` 同时在榜，说明"系统学 AI"的需求依然旺盛，2026 年新入场者数量仍在增长，并未饱和。

**4. 非 AI 的硬技术项目偶尔会大爆**——RuView 是今天的"反例"，提醒我们 GitHub trending 不完全被 LLM 叙事垄断，纯工程/物理层创新依然有强吸引力。
