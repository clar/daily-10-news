# GitHub Trending 日报 · 2026-07-05

## 今日焦点

> **Skills 生态爆发 · AI 渗透测试杀出黑马 · Claude Code 反向调用 Codex · 浏览器 Agent 全线加码 · 终端 Agent 复用运维栈**
>
> - `mattpocock/skills` 单日 +1,013⭐，把 skills 生态推到 156k 星总量，与 `agentskills/agentskills`、`dotnet/skills` 一起形成"skills 三剑客"
> - `JuliusBrussee/caveman` +1,089⭐，把 skill 玩到"token 减半"，成为 Claude Code 用户最热的降本工具
> - `usestrix/strix` +1,910⭐，AI 渗透测试用一个 Agent 拉完全流程，登顶单日增星榜
> - `openai/codex-plugin-cc` +716⭐，OpenAI 官方以插件姿态"寄生"Claude Code，模型商互调闭环
> - `alibaba/page-agent` 与 `ChromeDevTools/chrome-devtools-mcp` 双箭齐发，浏览器自动化再度成为热榜主线

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [usestrix/strix](https://github.com/usestrix/strix) | 开源 AI 渗透测试 Agent | Python | 35,965 | +1,910 | — |
| 2 | [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) | 用简化语法减少 Claude Code token | JavaScript | 83,896 | +1,089 | — |
| 3 | [mattpocock/skills](https://github.com/mattpocock/skills) | 面向工程师的 skills 集合 | Shell | 156,508 | +1,013 | — |
| 4 | [Zackriya-Solutions/meetily](https://github.com/Zackriya-Solutions/meetily) | 隐私优先本地会议助手 | Rust | 15,173 | +865 | — |
| 5 | [alibaba/page-agent](https://github.com/alibaba/page-agent) | 用自然语言驱动浏览器 GUI Agent | TypeScript | 23,065 | +726 | — |
| 6 | [openai/codex-plugin-cc](https://github.com/openai/codex-plugin-cc) | 在 Claude Code 里调用 Codex 处理任务 | JavaScript | 24,301 | +716 | — |
| 7 | [ogulcancelik/herdr](https://github.com/ogulcancelik/herdr) | 常驻终端的 Agent 多路复用器 | Rust | 11,393 | +706 | — |
| 8 | [harvard-edge/cs249r_book](https://github.com/harvard-edge/cs249r_book) | 《Machine Learning Systems》教材 | Python | 26,538 | +446 | — |
| 9 | [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) | 主流 AI 平台系统 Prompt 泄漏合集 | JavaScript | 48,861 | +432 | — |
| 10 | [rommapp/romm](https://github.com/rommapp/romm) | 自托管 ROM 管理与游玩平台 | Python | 10,176 | +400 | — |
| 11 | [agentskills/agentskills](https://github.com/agentskills/agentskills) | Agent Skills 规范与文档 | Python | 22,304 | +351 | — |
| 12 | [chthollyphile/folia-major](https://github.com/chthollyphile/folia-major) | 支持动态歌词的本地音乐播放器 | TypeScript | 979 | +319 | — |
| 13 | [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) | 面向 coding agent 的 Chrome DevTools MCP | TypeScript | 45,749 | +303 | — |
| 14 | [immich-app/immich](https://github.com/immich-app/immich) | 高性能自托管照片管理 | TypeScript | 105,595 | +198 | — |
| 15 | [dotnet/skills](https://github.com/dotnet/skills) | .NET/C# 官方 Agent Skills | C# | 3,793 | +57 | — |

---

## 重点项目点评

### 🥇 [usestrix/strix](https://github.com/usestrix/strix) — 今日榜首，+1,910⭐

**开源 AI 渗透测试第一次上主流，OSS 版 XBOW 的雏形**

Strix 主打"一个 Agent 跑完渗透测试全流程"，把侦察、模糊测试、poc 编写、报告输出用统一 LLM 调度串起来。近三日随着 OpenAI GPT-5.6 Sol 强调"网络安全前沿模型"的产品叙事，Strix 直接成为"手里有开源版工具了吗？"这个问题的答案，登顶单日增星。

Strix 更聪明的一点是**免费定位**——用 Claude Sonnet 5 / GPT-5.6 Terra 一类中等成本模型足以跑完 SaaS 上的常规漏洞流；相比 XBOW/HackerOne 那种付费 SaaS，安全团队可以自建 CI 集成而不用把内网代码交给外部。生态位极准，涨星几乎不需要额外营销。

---

### 🥈 [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) — +1,089⭐

**"石器时代英语"式降本 skill，把 Claude Code 变便宜的邪门歪道**

Caveman 是一个 Claude Code Skill，核心思路是把 prompt 转成极简语法（省掉冠词、连词、语气助词等）以显著削减 token 用量。作者宣称 token 减半而模型理解力几乎无损。这条思路两周前在推特上刷屏，现在开源版本终于跟上，一天涨 1k 星。

它的爆火说明两件事：**（1）Claude Code 用户对 token 成本极其敏感**，即便 Sonnet 5 定价已下调；**（2）Skills 已经成为一线用户改造 IDE 的最小抽象**——一个 markdown + prompt 组合就能形成社区级的工程效应。

---

### 🥉 [mattpocock/skills](https://github.com/mattpocock/skills) — +1,013⭐

**Skills 生态第一大 KOL，把工程师默会知识变成可分发的 markdown**

Matt Pocock（TypeScript 教育者）把自己写代码时反复用到的规则集打包成一份 skills 目录，一举把总星数拉到 156k+——他的 skills 从"TypeScript 类型推导陷阱"到"Node.js 内存 profiling"应有尽有，非常实用。

配合今日榜上的 `agentskills/agentskills`（规范文档）和 `dotnet/skills`（官方语言集合），**Skills 生态已经出现"社区 → 规范 → 官方"三层结构**。这几乎和 2015 年左右 npm 生态早期一样，谁能把 skill 装配的分发协议做成事实标准，谁就掌握了 AI 编程时代的包管理器叙事。

---

### 🎯 [openai/codex-plugin-cc](https://github.com/openai/codex-plugin-cc) — +716⭐

**OpenAI 官方以插件姿态寄生 Claude Code，模型商相互调用出现新形态**

OpenAI 官方推出的 Claude Code 插件，让 Claude Code 用户可以直接调用 Codex（GPT-5.6）来 review 或代跑子任务。此前跨模型互调多靠民间 wrapper，这次是**OpenAI 首次官方承认 Claude Code 是分发通路**并主动接入，姿态耐人寻味。

技术上，插件用 MCP 协议桥接 Codex 服务端，本地不落 API Key；商业上，它意味着 OpenAI 承认 Anthropic 在 IDE 场景已占先手，主动"寄生"以维持在场景中的存在感。对开发者而言，这条路径给出了"在 IDE 里同时用两家最强模型"的低门槛方案。

---

### 🌐 [alibaba/page-agent](https://github.com/alibaba/page-agent) — +726⭐

**浏览器 Agent 从"外部驱动"转向"页面内驻留"**

阿里出品的 page-agent 是一个**注入到网页内部**的 JavaScript GUI Agent。以往浏览器 Agent 大多在外层用 CDP/Playwright 控制，page-agent 直接在页面运行时插入 hooks，能自然响应 SPA 路由变化、隐藏元素、跨 iframe 等复杂情况。

配合 `ChromeDevTools/chrome-devtools-mcp`（+303），浏览器自动化今天两头齐发：一头是浏览器官方给 agent 铺 DevTools 通道，一头是页面内注入的 GUI agent。这两条路线未来必然会撞车——"浏览器提供 API vs. 页面自带 Agent"的博弈即将开启。

---

## 生态观察

**今日主线是 Skills 生态 + Agent 三大栈**：

1. **Skills 生态**（`caveman`、`mattpocock/skills`、`agentskills/agentskills`、`dotnet/skills`）——从"社区玩法"进入"官方接管"的转折窗口。Anthropic 上周把 Skills 变成 Claude Code 一等公民后，第三方开始批量把默会规则转成 skill 分发
2. **Agent 三大栈**——`strix`（安全）、`page-agent` / `chrome-devtools-mcp`（浏览器）、`herdr`（终端）分别代表垂直、水平、系统三条 agent 路径；官方与生态的界线正在被打破
3. **降本仍是硬需求**——即便 Sonnet 5 已经把价格打下来，`caveman` 依然一天涨 1k 星；说明 Claude Code 用户群体对"任何能省 token 的 tricks"仍处于强烈需求
4. **模型厂互调开始官方化**——`openai/codex-plugin-cc` 打破"OpenAI 只出 ChatGPT/Codex CLI"的产品洁癖，接下来极可能出现"Gemini 在 Claude Code / Codex CLI 双向可用"的连环插件

一句总结：**Skills + Agent + 降本插件**——今日 GitHub 热榜的三条支柱，全部指向"如何让 Claude Code / Codex CLI 更快更省更强"。Coding Agent 的次级市场，正在形成。
