# GitHub Trending 日报 · 2026-05-12

## 今日焦点

> **AI Agent 桌面化 · 反爬虫军备升级 · 免费 AI Router · 内容变现自动化 · 自学习智能体**
>
> - `bytedance/UI-TARS-desktop` 字节多模态 GUI 智能体跃居榜首，+956⭐
> - `CloakHQ/CloakBrowser` C++ 源码级反检测浏览器，单日 +1,325⭐
> - `NousResearch/hermes-agent` 自学习 Agent 单日狂增 +2,229⭐
> - `decolua/9router` 免费 AI 编码路由聚合 40+ 提供商，+942⭐
> - `yikart/AiToEarn` AI 全自动内容变现平台，+595⭐

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [bytedance/UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop) | 开源多模态 AI Agent 栈 | TypeScript | 32,920 | +956 | 3,261 |
| 2 | [CloakHQ/CloakBrowser](https://github.com/CloakHQ/CloakBrowser) | 通过机器人检测的隐身浏览器 | Python | 5,956 | +1,325 | 448 |
| 3 | [yikart/AiToEarn](https://github.com/yikart/AiToEarn) | "用 AI 来赚钱" 全栈内容变现 | TypeScript | 10,637 | +595 | 1,991 |
| 4 | [playcanvas/supersplat](https://github.com/playcanvas/supersplat) | 3D 高斯点云编辑器 | TypeScript | 7,270 | +533 | 796 |
| 5 | [datawhalechina/easy-vibe](https://github.com/datawhalechina/easy-vibe) | 面向初学者的现代编程课程 | JavaScript | 9,823 | +808 | 940 |
| 6 | [decolua/9router](https://github.com/decolua/9router) | 自动 fallback 的免费 AI 编码路由 | JavaScript | 8,194 | +942 | 1,315 |
| 7 | [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) | 个人 AI 超级智能 | Rust | 1,326 | +501 | 174 |
| 8 | [millionco/react-doctor](https://github.com/millionco/react-doctor) | 检测低效 React 模式 | TypeScript | 7,946 | +340 | 252 |
| 9 | [Lordog/dive-into-llms](https://github.com/Lordog/dive-into-llms) | LLM 编程教程系列 | Jupyter Notebook | 37,260 | +451 | 4,568 |
| 10 | [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) | Stable Diffusion Web UI | Python | 162,880 | +29 | 30,333 |
| 11 | [rasbt/LLMs-from-scratch](https://github.com/rasbt/LLMs-from-scratch) | 从零实现 ChatGPT 级 LLM 指南 | Jupyter Notebook | 92,884 | +408 | 14,328 |
| 12 | [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) | 与你共同成长的 Agent | Python | 144,532 | +2,229 | 22,593 |
| 13 | [rohitg00/agentmemory](https://github.com/rohitg00/agentmemory) | AI 编码 Agent 的持久化记忆 | TypeScript | 4,619 | +604 | 436 |

---

## 重点项目点评

### 🥇 [bytedance/UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop) — 今日榜首，+956⭐

**字节把多模态 Agent 做成了"一台可被语言操控的电脑"**

UI-TARS-desktop 由两个模块组成：通用型 **Agent TARS**（带 CLI 与 Web UI，整合 MCP 工具协议，可控制终端、电脑与浏览器）与 **UI-TARS Desktop** 原生桌面应用（基于视觉-语言模型识别截图，并把自然语言指令翻译成精准的鼠标键盘动作）。它对标的不是 LangChain 级的 SDK，而是 Claude Desktop + Computer Use 整合形态——通过 MCP + GUI Vision 形成"系统级 Copilot"。

今日跃居榜首并非偶然：在过去两周中，AnthropIC Computer Use 与 OpenAI Operator 商业化加速，社区急需一个**开源、可本地化部署、且可深度定制**的等价物。字节这一栈把"截图→意图→操作"的回路彻底开源，对开发者、企业内部自动化场景都极具吸引力。Fork 数已飙到 3,261，说明二开/私有部署需求强烈。

它也是国产团队第一次在桌面 Agent 这条赛道上拿出能直接与硅谷叫板的开源方案——某种意义上，今日榜首是 2026 年中文 AI 工具链国际化进程的一个里程碑。

---

### 🥈 [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) — +2,229⭐

**真正会"学习"的 Agent，把"经验"变成可复用技能**

Hermes Agent 来自著名的开源团队 Nous Research，最大卖点是内置 **learning loop**——它能在使用中自动把交互沉淀成技能，并在后续调用时持续打磨这些技能。它支持任意 LLM 提供商（本地或云端均可），通过 MCP 接入工具，可在 Telegram/Discord/Slack 上随时使用，部署门槛低至一台 $5 VPS。

绝对增量 2,229 是今天的"巅峰"。原因可以归结为三点：一，Nous 团队在长期记忆/技能合成方向积累深厚，社区信任度高；二，"自演化 Agent"这一概念在过去半年已被 Anthropic Constitutional Skills、Microsoft Copilot Studio 等反复验证，开源版本市场缺口巨大；三，22,593 的 Fork 数表明这并非新项目，而是一次重大版本/重命名后的"二次爆发"。

如果说 ByteDance 的 UI-TARS 解决"如何让 Agent 操作物理界面"，Hermes 解决的则是"如何让 Agent 越用越聪明"——两条赛道叠加，今日榜单本质上勾勒出 2026 年 Agent 工程的两大支柱。

---

### 🥉 [CloakHQ/CloakBrowser](https://github.com/CloakHQ/CloakBrowser) — +1,325⭐

**Web 自动化进入"源码级反检测"时代**

CloakBrowser 走的是激进路线：**不是通过 JS 注入或运行时 patch 来绕过检测，而是直接修改 Chromium 源码**——49 个 canvas/WebGL/audio 指纹补丁、配合"humanize"行为模拟，可一举击穿 reCAPTCHA v3、Cloudflare Turnstile 与 FingerprintJS。对 Playwright/Puppeteer 而言是 drop-in 替代，`pip install cloakbrowser` 即可使用。

它单日 +1,325 的爆发反映了一个深层趋势：随着 AI Agent 大量需要浏览网页、调用真实服务，**反爬虫与反 Agent 检测正快速升级**，过去的 stealth-puppeteer 一类已经不够用。CloakBrowser 把"对抗工具"做到了内核层，标志着 Web 自动化武器库进入下一代。

需要警惕的是，这把"双刃剑"会同步推高诈骗团伙的能力上限——平台侧的 fingerprint 防御也将被迫升级，可能在未来 6-12 个月引发新一轮"反反爬"军备竞赛。

---

### 🏅 [decolua/9router](https://github.com/decolua/9router) — +942⭐

**白嫖 Claude Code 的最优路径已开源**

9router 是一个 AI 编码路由器，把 Claude Code、Cursor、Cline 等客户端的请求**自动路由**到 40+ 提供商、100+ 模型之间，规则是"订阅 → 便宜 → 免费" 的智能 fallback，附带 20-40% 的 token 压缩。换言之，它能在你免费/廉价额度耗尽时无缝切换，几乎不会触发 rate limit。

今日 +942 的增长背后是一个长期未被满足的需求：**Claude Code、Cursor 等付费工具体验好但额度紧张，DeepSeek、Qwen、Gemini 等模型有免费 API 但接入碎片化**。9router 用一个 proxy 把这些资源拼起来，相当于给开发者发了张"AI 共享出行卡"。

随着官方平台对滥用的封堵越来越严，这类聚合路由的可持续性仍是未知数；但短期内它会成为非北美/非企业开发者绕过 token 焦虑的事实标准。

---

### 🏅 [yikart/AiToEarn](https://github.com/yikart/AiToEarn) — +595⭐

**AI Agent 终于学会了帮你赚钱**

AiToEarn 是一个全栈内容变现平台：AI 自动生成内容 → 一键发布到 TikTok/YouTube/Instagram/抖音/小红书等 12+ 平台 → 自动评论互动 → 通过 CPS/CPE/CPM 等模式给创作者结算。提供 Web 和 Docker 私有部署两种形态。

这是今日榜单中**最具"商业可执行性"的项目**：相比技术尝鲜，它直接面向"想用 AI 替自己运营自媒体矩阵"的小商家与个人 IP。1,991 的 Fork 数（接近 stars 的 1/5）说明大量人在 fork 后做私有化部署或二次开发，与"研究型项目"明显不同。

侧面也透露一个信号：2026 年 AI 工具的下一站不是模型本身，而是**让 AI 成为可持续产出现金流的劳动力**。"Agent + 内容平台 + 联盟营销"组合，可能是未来一年最拥挤的赛道。

---

## 生态观察

今日榜单可用六个字概括："**Agent 走出聊天框**"。Top 13 中，9 个项目与 AI Agent/LLM 直接相关，且共同特征是**操作真实世界**——操控桌面（UI-TARS）、对抗反爬（CloakBrowser）、自动发内容赚钱（AiToEarn）、聚合算力路由（9router）、长期记忆（agentmemory）、自我演化（hermes-agent）。

中文团队表现亮眼：bytedance、datawhalechina、Lordog、yikart 占据 4 席，且全部位列前 10。Stable Diffusion 这种"老牌神级仓库"今天只增 29 ⭐，提醒我们 2026 年的开源叙事已经从"生成模型"完全转向"自主 Agent"。

短期值得关注的次级趋势：**3D 高斯点云**（supersplat）作为 Vision Pro 2/Quest 3 内容生产工具开始进入工程化阶段；**React 性能审计**（react-doctor）说明前端社区正在反思 React 19 时代的运行时开销。
