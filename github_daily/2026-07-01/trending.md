# GitHub Trending 日报 · 2026-07-01

## 今日焦点

> **AI Agent 全栈爆发 · Google 入场 agents-cli · 安全/红队工具回潮 · 隐私通讯 SimpleX 大涨 · 视频编辑也 agentic**
>
> - `msitarzewski/agency-agents` 一日 +1,793⭐：完整"AI 公司"模板成为今日榜首之一。
> - `google/agents-cli` +433⭐：Google 把 Agent SDK 套件下沉到 CLI 层，正面对线 Claude Code。
> - `usestrix/strix` +395⭐：开源 AI 渗透测试工具继续累计，已破 28k 总星。
> - `simplex-chat/simplex-chat` +1,229⭐：在 AI / 隐写 / 监管话题密集的当下，"无用户标识符通信"被重新热捧。
> - `browser-use/video-use` +722⭐：browser-use 团队把 agent 范式从浏览器扩展到视频剪辑。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | 全套"AI agency"专家 agent 模板 | Shell | 120,762 | +1,793 | 19,736 |
| 2 | [hasaneyldrm/exercises-dataset](https://github.com/hasaneyldrm/exercises-dataset) | 433 个健身动作多媒体数据集 | HTML | 6,460 | +1,413 | 777 |
| 3 | [simplex-chat/simplex-chat](https://github.com/simplex-chat/simplex-chat) | 无用户标识符的隐私通讯网络 | Haskell | 17,313 | +1,229 | 1,006 |
| 4 | [xbtlin/ai-berkshire](https://github.com/xbtlin/ai-berkshire) | 四大投资大师方法论 multi-agent 框架 | Python | 7,457 | +966 | 953 |
| 5 | [ripienahr/free-for-dev](https://github.com/ripienahr/free-for-dev) | 开发者免费 SaaS/PaaS/IaaS 清单 | HTML | 127,287 | +740 | 13,305 |
| 6 | [browser-use/video-use](https://github.com/browser-use/video-use) | 用 coding agent 编辑视频 | Python | 12,541 | +722 | 1,602 |
| 7 | [altic-dev/FluidVoice](https://github.com/altic-dev/FluidVoice) | macOS 上的本地 STT + AI 听写 | Swift | 4,884 | +586 | 300 |
| 8 | [ogulcancelik/herdr](https://github.com/ogulcancelik/herdr) | 终端里的 agent 多路复用器 | Rust | 8,963 | +485 | 537 |
| 9 | [diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute) | 支持 231+ 提供商的 AI gateway | TypeScript | 8,428 | +459 | 1,391 |
| 10 | [google/agents-cli](https://github.com/google/agents-cli) | Google 出品的 Agent CLI 套件 | Python | 4,138 | +433 | 451 |
| 11 | [usestrix/strix](https://github.com/usestrix/strix) | 开源 AI 渗透测试 / 漏洞修复 | Python | 28,068 | +395 | 3,121 |
| 12 | [CoreBunch/Instatic](https://github.com/CoreBunch/Instatic) | 1 分钟上手的自托管可视化 CMS | TypeScript | 1,488 | +351 | 137 |
| 13 | [roboflow/supervision](https://github.com/roboflow/supervision) | 通用计算机视觉工具集 | Python | 45,880 | +336 | 4,071 |
| 14 | [microsoft/AI-For-Beginners](https://github.com/microsoft/AI-For-Beginners) | 12 周 24 节 AI 入门课 | Jupyter | 49,303 | +180 | 10,156 |
| 15 | [Mebus/cupp](https://github.com/Mebus/cupp) | 常用用户密码画像工具 (CUPP) | Python | 6,085 | +61 | 2,046 |

---

## 重点项目点评

### 🥇 [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) — 今日榜首，+1,793⭐

**"开箱即用的 AI 公司"——一组职业化 agent 模板的爆款。**

repo 提供了一整套带"人格设定 + 职责边界 + 工具调用"的专家 agent 模板，相当于一份"AI agency 启动包"。一日新增 1,793 星，总星数已经飙到 12 万——这种增长曲线只有在 GitHub 把它放进 trending 首位 + 多个 newsletter 同时转发的情况下才会出现。

它代表的是 2026 年 AI 仓库的一个新阶段：**从"模型/SDK"到"组织/角色"**。开发者不再满足于"集成一个 LLM"，而是开始把"一家公司怎么分工"这件事直接打包成可复用 prompt 工程产物。Shell 作为主语言也说明这套东西的工程门槛被刻意压到最低——能写 bash 的人就能 fork 一份"自己的 AI 公司"。

---

### 🥈 [google/agents-cli](https://github.com/google/agents-cli) — +433⭐

**Google 正面对线 Claude Code 和 Cursor 的 CLI 入场券。**

description 写得很直白："让任何 coding assistant 变成创建/部署 AI agent 的专家"。这是 Google 第一次把 Agent 生态做成 **CLI + skills** 的形态——也就是说，它不绑死 Gemini，而是允许用户接到任何模型上。这是个聪明的姿态：在 Claude Code 因为"隐写标记"争议被 HN 怒喷的同一天，Google 用"开放 CLI"的形式提供另一种选择。

它的真正信号是：**Agent 主战场正在从"IDE 插件"下沉到"CLI / 工作流"**。过去 18 个月，IDE-first 的 Cursor / Windsurf 占了大头；现在 Claude Code、google/agents-cli、herdr 这一组终端原生 agent 都在抢"做你脚本的那个东西"的位置。

---

### 🥉 [simplex-chat/simplex-chat](https://github.com/simplex-chat/simplex-chat) — +1,229⭐

**在监管、隐写、平台水印密集的今天，"无身份通讯"被集体上票。**

SimpleX 是少数主流的、连 user-id 都不存在的通讯协议——它通过单向消息队列地址实现端到端无标识连接。今天它能拿到 1,229 星，并不是因为发了什么新版，而是社区情绪在某种程度上和 HN 的"Claude Code 隐写"事件叠加：当大公司被发现给请求打水印、Colorado AI Act 今日生效、EU 透明义务即将启动——开发者会本能地寻找"我能不能彻底匿名通信"的工具。

值得注意的是，它依然用 Haskell 写——这在 2026 年仍然非常少见，本身也说明它的目标用户是密码学 / 协议层 hacker 而非大众 IM 用户。

---

### 4️⃣ [browser-use/video-use](https://github.com/browser-use/video-use) — +722⭐

**Agent 范式从浏览器外溢到视频剪辑工作流。**

browser-use 团队的影响力上半年已经在 GitHub 立稳。今天 video-use 上榜证明 **"用 coding agent 操作复杂多模态工作流"** 这个范式已经从浏览器自动化扩展到视频。它的核心 pitch 是：你不再用 Premiere/CapCut 的 UI，而是用自然语言告诉 agent"剪掉 3-5 秒、把这段拼到那段后面、加字幕"。

这条线和今天 HN 上的 Claude Science（科研 agent）形成呼应——**2026 年下半年，垂直领域 agent 会成为创业新一轮赛道**：科研、视频、设计、法律。

---

### 5️⃣ [usestrix/strix](https://github.com/usestrix/strix) — +395⭐ · 累计 28k

**红队 / 安全 agent 正式进入工业级。**

Strix 是一个"AI 渗透测试"工具，可以自动发现 app 漏洞并给出 PoC + 修复建议。它今天虽然新增不及前 3，但累计已经站稳 28k 星，是 2026 年安全方向最大的 AI 开源项目之一。

它能持续增长的原因是 **AppSec 团队普遍缺人**：很多公司的安全人员对 1：50 的开发：安全比例已经无能为力，他们更愿意接受"用一个不完美但 24×7 跑的 agent"替代"等三个月招一个 senior"。Strix 这类工具未来一定会和 GitHub Actions / GitLab CI 深度集成。

---

## 生态观察

今天的 trending 板面有 4 条核心规律：

1. **Agent 主题压倒一切**：top 15 里至少 7 个是 agent 相关（agency-agents / video-use / herdr / OmniRoute / agents-cli / strix / ai-berkshire），全栈覆盖企业、视频、终端、网关、CLI、安全、投研。
2. **"非身份"的反向流量**：SimpleX 大涨说明，AI 透明 / 监管 / 隐写争议正在转化为对"匿名工具"的实际拥抱，而不只是讨论。
3. **数据集仓库回潮**：exercises-dataset 一日 +1,413 上到 #2，说明高质量结构化数据集本身就是"AI 喂料原材料"，再次成为创业起点。
4. **大厂仓库重新争夺 mindshare**：google/agents-cli、microsoft/AI-For-Beginners、roboflow/supervision 在同一天进入前 15，证明大厂在"教育 + 工具 + 框架"三个层面都没有放弃 GitHub 这块开源主战场。

值得继续观察：`google/agents-cli` 会不会在两周内进入 10k 俱乐部、`agency-agents` 在突破 12 万星后是否进入 "fork 大潮" 阶段（fork/star 比率是 16% 已经偏高）。
