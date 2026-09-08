# GitHub Trending 日报 · 2026-09-09

## 今日焦点

> **Skills 生态爆发 · Agent-first 工具链 · 视频/文档 → HTML 化 · 隐蔽爬虫回潮 · Claude Code 周边繁荣**
>
> - `heygen-com/hyperframes` 单日 +2,628⭐，"写 HTML 生成视频"这种 agent-first API 抽象终于跑通
> - `cathrynlavery/diagram-design` +1,020⭐，38 种编辑图形直接作为 Claude Code / Codex / Pi 的 skill 分发
> - `microsoft/markitdown` +2,045⭐，Office / PDF → Markdown 长红，成为所有 RAG 项目的默认前处理器
> - `openai/skills` +490⭐、`obra/superpowers` +446⭐、`ayghri/i-have-adhd` +422⭐——skills 概念在多个生态并行开花
> - `jo-inc/camofox-browser` +872⭐，绕过 Cloudflare 的隐蔽浏览器再次登上榜单，agent 抓取战争升级

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [heygen-com/hyperframes](https://github.com/heygen-com/hyperframes) | 写 HTML 直接渲染视频，专为 agent 设计 | TypeScript | 47,699 | +2,628 | 4,391 |
| 2 | [microsoft/markitdown](https://github.com/microsoft/markitdown) | 把 Office/PDF/媒体统一转 Markdown | Python | 181,625 | +2,045 | 13,343 |
| 3 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | agent harness 性能优化系统，主打 skills+memory | JavaScript | 254,240 | +1,426 | 38,103 |
| 4 | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | 38 种编辑图形，供 Claude Code/Codex/Pi 使用 | HTML | 34,670 | +1,020 | 2,198 |
| 5 | [jo-inc/camofox-browser](https://github.com/jo-inc/camofox-browser) | 绕 Cloudflare 的隐蔽 headless 浏览器 | JavaScript | 10,444 | +872 | 1,050 |
| 6 | [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | 面向 Claude Code 的营销能力包 | JavaScript | 48,768 | +666 | 7,494 |
| 7 | [mksglu/context-mode](https://github.com/mksglu/context-mode) | AI coding agent 的 context 窗优化 | TypeScript | 21,362 | +652 | 1,543 |
| 8 | [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) | 基于 Karpathy 心得的 CLAUDE.md 集 | Markdown | 211,412 | +533 | 21,469 |
| 9 | [MoonTechLab/LunaTV](https://github.com/MoonTechLab/LunaTV) | 开源多媒体聚合项目 | TypeScript | 10,144 | +505 | 9,044 |
| 10 | [The-Swarm-Corporation/AutoHedge](https://github.com/The-Swarm-Corporation/AutoHedge) | 分钟级搭建自动化对冲基金的 swarm 框架 | Python | 5,679 | +494 | 836 |
| 11 | [openai/skills](https://github.com/openai/skills) | Codex 的官方 skills catalog | Python | 26,481 | +490 | 1,776 |
| 12 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic skills 框架 + 软件开发方法论 | Shell | 283,327 | +446 | 25,365 |
| 13 | [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) | 阻止 coding agent 埋结论的 skill | Python | 30,175 | +422 | 1,843 |
| 14 | [browser-use/browser-use](https://github.com/browser-use/browser-use) | 让 AI agent 操作浏览器完成任务 | Python | 113,441 | +320 | 12,486 |
| 15 | [viarotel-org/escrcpy](https://github.com/viarotel-org/escrcpy) | scrcpy 图形化，Android 屏幕镜像 | JavaScript | 11,356 | +173 | 795 |

---

## 重点项目点评

### 🥇 [heygen-com/hyperframes](https://github.com/heygen-com/hyperframes) — 今日榜首，+2,628⭐

**"写 HTML 生成视频"——agent-first 视频生成第一次有了合适的 API 抽象**

Heygen 出手把 HTML 语义当作视频描述语言：agent 只需要用它熟悉的 DOM / CSS 概念产出一段"帧"，hyperframes 负责把它 diff、插值、合成为完整视频。这个抽象层的价值在于——**AI agent 天然会写 HTML，不天然会写 After Effects/Premiere 时间线**。今天单日 +2,628⭐ 说明社区在等这样一个"agent-friendly video toolkit"等了很久。

技术上它把浏览器渲染管线（可以做到帧一致、字体一致、动画一致）借来当视频引擎，规避了传统 video SDK 里 "渲染细节全交给低层库" 的黑盒问题。对内容创作 SaaS 而言，这是个能替代 Runway/Descript API 层的开源候选；对 LLM 应用而言，它把"给我做个 30 秒宣传片"这件事从"生成视频"降维为"生成 HTML"，成本和可预测性都被显著改善。

---

### 🥈 [microsoft/markitdown](https://github.com/microsoft/markitdown) — +2,045⭐

**微软亲自把"Office → Markdown"做成默认前处理器，RAG 生态受益**

markitdown 用 Python 把 Office、PDF、图像 OCR、音频转写等一股脑归一成干净的 Markdown。总星数 181k 已是超一线，今天还能冲 +2k，说明它正逐步取代 Unstructured、LangChain 原生解析器等成为**新项目的默认前处理器**。三个关键推力：微软官方背书、依赖极轻、CLI 与 Python API 并存。

对 RAG / agent 项目意义在于：数据管道能少写 40% 的胶水代码。目前榜上的 skills 类项目（ECC、context-mode、i-have-adhd）几乎都会把 markitdown 隐式或显式列为推荐依赖——**skills 生态在快速形成一套事实上的"标准栈"**。

---

### 🥉 [affaan-m/ECC](https://github.com/affaan-m/ECC) — +1,426⭐

**agent harness 性能优化系统：把 skills + memory 当成一等公民**

ECC 的定位是给现有 agent harness（Claude Code、Codex、Cursor 等）加一个"性能层"：核心概念是把 skills 加载策略、长期 memory、上下文压缩当成可插拔组件优化。基于 JS 生态、总星 254k，是目前 agent tooling 里体量最大的开源框架之一。

它今天的爆发（+1,426⭐）与榜单上其他 skills 项目形成合力：**"skills"不再只是 Anthropic 内部术语，而是 agent 生态的通用抽象**。ECC 提供了实现层，OpenAI/skills 提供了目录层，各家的 skill 包（marketingskills、i-have-adhd、diagram-design）提供了内容层，一个完整的分发 → 加载 → 执行三段式栈正在自组织。

---

### 🎯 [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) — +1,020⭐

**38 种编辑级图形直接封装成跨厂 skill：设计能力也能"包装出售"**

这个仓库只做一件事——把 38 种编辑级别的图表（不是"折线图/柱状图"，而是像 The Economist 那种编辑图形）封装成可以直接被 Claude Code / Codex / Pi 调用的 skill。今天 +1,020⭐ 说明**"用 skill 分发设计能力"这件事的市场正式被验证**。

它与 heygen/hyperframes 形成了有趣的呼应：一个把视频降维为 HTML，一个把复杂图表降维为可复用 skill，共同的模式是——**用一层薄薄的语义抽象，让 LLM 直接输出高质量视觉产物**。设计师职业焦虑加剧，但设计能力的可分发性达到史上新高。

---

### 🕵️ [jo-inc/camofox-browser](https://github.com/jo-inc/camofox-browser) — +872⭐

**Cloudflare 攻防再次白热化：agent 时代的爬虫必然武装到牙齿**

camofox 是一款专为绕过 Cloudflare bot protection 设计的隐蔽 headless 浏览器：TLS fingerprint、Canvas 指纹、WebGL 指纹全部随机化。它今天 +872⭐ 冲上榜单，与 `browser-use/browser-use` (+320⭐) 组成"agent 抓取工具组合拳"。

从生态视角看，这标志着一件事：**agent 大规模跑起来以后，"合法访问互联网"变得越来越贵，反爬体系被迫升级到 fingerprinting 层，攻击方随即武装到 TLS 层**。这场军备竞赛在过去五年一直存在，但 AI agent 让它从"少数爬虫工程师的游戏"扩大为"每个应用开发者都要面对的现实"。Cloudflare、Akamai 未来一年会推出更激进的机器人识别策略——这不是预测，是 GitHub trending 直接给出的信号。

---

## 生态观察

- **Skills 已经是 GitHub trending 的绝对主角**：15 个热榜里有 8 个直接跟 skills / Claude Code / agent harness 相关（i-have-adhd、diagram-design、openai/skills、marketingskills、karpathy-skills、superpowers、ECC、context-mode）。这在半年前完全不成立。
- **视频 / 文档的 agent-first 表达**：hyperframes 用 HTML 表达视频、markitdown 用 Markdown 归一文档——AI 时代的通用逻辑是**"选一个 LLM 最会写的媒介来当中间格式"**。
- **抓取战争升级**：camofox + browser-use 上榜说明 agent 消费互联网的规模已经到了让整个反爬产业链再度动员的门槛。
- **金融自动化"梗"仓库回潮**：AutoHedge (+494⭐) 上榜，"自动化对冲基金"是长期性 meme，但确实反映有一批开发者在玩链上 + LLM + agent 组合的边缘实验。
- **老牌工具类**：LunaTV、escrcpy、markitdown 稳定发挥，说明**在纯 AI 热度之外，Utility 类项目一直有稳定的需求底盘**。

一句话总结：**AI agent 生态今天的 GitHub 主叙事已经从"模型"迁移到"skills + agent 工具链"，与此同时反爬、视频、设计等具体领域被 skills 抽象层顺势重构。**
