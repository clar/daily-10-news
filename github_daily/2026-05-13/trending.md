# GitHub Trending — 2026-05-13

## 今日焦点

> **AI 智能体记忆 · Claude 工具链 · 反检测自动化 · 本地隐私化 AI · LLM 从零造轮**
>
> - `mattpocock/skills` Matt Pocock 把私人 `.claude/` 全套放出，一日新增 +3,886⭐，是今日榜首
> - `CloakBrowser` 不靠 JS 注入而是 C++ 源码级指纹补丁的 Playwright 替代品，反爬大战进入"魔改 Chromium"阶段
> - `agentmemory` 自称在 LongMemEval-S 上达到 95.2% 检索准确率、节省 92% token，AI agent 记忆层成为新战场
> - `openhuman` Rust 写的本地 AI 助手，118 个集成 + Obsidian 兼容 Memory Tree，主打离线私有
> - `react-doctor` 不是写给人看的 linter，而是教 AI 不要写烂 React 的 0-100 分诊断工具

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [mattpocock/skills](https://github.com/mattpocock/skills) | Skills for Real Engineers，作者私人 `.claude` 目录 | Shell | 75,692 | +3,886⭐ | 6,522 |
| 2 | [CloakHQ/CloakBrowser](https://github.com/CloakHQ/CloakBrowser) | 反检测 Chromium，Playwright 直接替换，30/30 bot 测试通过 | Python | 7,621 | +1,589⭐ | 554 |
| 3 | [yikart/AiToEarn](https://github.com/yikart/AiToEarn) | Let's use AI to Earn！AI 自动化变现 | TypeScript | 11,754 | +1,264⭐ | 2,077 |
| 4 | [rohitg00/agentmemory](https://github.com/rohitg00/agentmemory) | 面向 AI 编码 agent 的持久化记忆，跨 12+ 工具共享 | TypeScript | 5,703 | +1,067⭐ | 539 |
| 5 | [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) | 本地超个人 AI，118 集成 + Memory Tree，Rust 实现 | Rust | 2,504 | +1,042⭐ | 246 |
| 6 | [millionco/react-doctor](https://github.com/millionco/react-doctor) | 检测 AI 写出来的烂 React，输出 0-100 健康分 | TypeScript | 8,681 | +804⭐ | 277 |
| 7 | [rasbt/LLMs-from-scratch](https://github.com/rasbt/LLMs-from-scratch) | PyTorch 从零实现一个类 ChatGPT LLM | Jupyter Notebook | 93,658 | +776⭐ | 14,409 |
| 8 | [datawhalechina/hello-agents](https://github.com/datawhalechina/hello-agents) | 《从零开始构建智能体》中文教程 | Python | 48,157 | +600⭐ | 5,798 |
| 9 | [HKUDS/AI-Trader](https://github.com/HKUDS/AI-Trader) | 100% 全自动 Agent-Native 交易系统 | Python | 16,500 | +267⭐ | 2,607 |
| 10 | [apernet/hysteria](https://github.com/apernet/hysteria) | 强力快速抗审查代理 | Go | 20,148 | +112⭐ | 2,090 |
| 11 | [anonfaded/FadCam](https://github.com/anonfaded/FadCam) | 开源无广告 Android 后台录像/直播/远程控制 | Java | 2,164 | +111⭐ | 166 |

---

## 重点项目点评

### 🥇 [mattpocock/skills](https://github.com/mattpocock/skills) — 今日榜首，+3,886⭐

**Claude Code 生态进入"个人作坊式工具链"传播期**

Matt Pocock 是 TypeScript 教学圈的头部，今天他把自己的 `.claude/` 目录原样开源，分成"工程类技能"（TDD、架构改造、Issue 分类）和"生产力类技能"（结构化访谈、交接文档）两组。**单日 3,886⭐ 几乎是榜单第二名的 2.5 倍**——这说明 Claude Code skills 已经从"官方文档上的玩具"，演化成开发者愿意 fork 个人化工作流的真实生产工具。

更值得注意的是这条路线的反共识立场：仓库 README 明确反对"把开发完全自动化"，把 skill 定位为"小颗粒、可组合、可改写"的实践片段，对应的是工程基本功而不是大一统 agent。结合 #6 的 `react-doctor` 和 #4 的 `agentmemory`，Claude Code 周边正在形成一个共识——**未来 AI 编程的护城河不在模型，而在"教 agent 守规矩的工具层"**。

---

### 🥈 [CloakHQ/CloakBrowser](https://github.com/CloakHQ/CloakBrowser) — +1,589⭐

**反检测大战进入 C++ 源码级**

CloakBrowser 是一个 drop-in 替换 Playwright/Puppeteer 的 Chromium，关键差异是它**不在 JavaScript 层注入 patch**——市面上大部分 stealth 方案（puppeteer-extra-stealth、undetected-chromedriver 等）都是 JS 注入，已经被 Cloudflare、DataDome 等识别得七七八八。CloakBrowser 直接在 Chromium C++ 源码层改指纹，号称 30/30 通过现行 bot 检测测试套件。

它一天破 1,500⭐ 的真实驱动力其实是 **AI agent 浪潮的副作用**：越来越多 LLM agent 需要稳定访问受保护页面（爬数据、刷价格、跑订单），而前一代 stealth 工具普遍开始失效。可以预期，这个仓库会被反向研究——Cloudflare 一类的反爬厂会写新规则匹配它的指纹，然后 CloakBrowser 又被迫升级，进入下一轮军备循环。

---

### 🥉 [rohitg00/agentmemory](https://github.com/rohitg00/agentmemory) — +1,067⭐

**AI agent 的"记忆即基础设施"时刻**

agentmemory 自称在 LongMemEval-S 上做到 95.2% rank-5 检索准确率、相比 LLM-summarize 方案省 92% token、年成本从 $500 降到 $10。技术栈很克制：本地 SQLite，单进程内存服务器，不依赖任何外部数据库。

真正的杀手锏在于**横向兼容**——一份记忆同时被 Claude Code（hooks/plugins）、Cursor、Cline、Windsurf 通过 MCP 共享。这是一个非常聪明的定位：**它不和任何 IDE 竞争，而是赌"agent 越多越分散，统一记忆层越值钱"**。配合榜单上 #5 OpenHuman 的 Memory Tree、#1 skills 的工作流封装，AI agent 这一代的"操作系统层"开始浮现——存档、技能、记忆、权限。

---

### [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) — +1,042⭐

**本地 AI 助手的"118 集成 + Rust + Obsidian"组合拳**

openhuman 这个项目几乎在用"反 ChatGPT 默认设定"的所有维度建身份：Rust 写、本地 SQLite 加密、Obsidian-compatible wiki、118 个 SaaS 自动同步。Memory Tree 是它的核心叙事，把 Gmail/Notion/GitHub/Slack 的数据压缩成树形 wiki，让 agent 不靠云端长上下文也能"了解你"。

这个赛道上一波 Rewind/Personal AI 都是闭源 + 上传云的路线，OpenHuman 把所有差异化都压在"开源 + 本地 + Rust"上，吃到的是**对隐私敏感开发者群体**的红利。能不能从 demo 走向日用，关键看 Rust 桌面端在不同操作系统上的体验稳定性，以及那 118 个集成的维护成本——这两点都是国内同类项目难以复制的护城河。

---

### [millionco/react-doctor](https://github.com/millionco/react-doctor) — +804⭐

**专为 AI 写的 linter，不是给人看的**

`npx react-doctor@latest .` 跑完输出 0-100 的健康分，覆盖 state 管理、性能、架构、安全、可访问性。乍看是 ESLint 升级版，仔细看 README 才发现它的目标用户是 **Claude Code 和 Cursor 这类 agent**——通过把诊断器装进 agent 工具链，让 AI 在生成 React 代码时就自己检查、自己修。

这个产品形态有意思的地方在于：它本质上承认 **"AI 写的 React 普遍很差"** 是当下事实，而不是去做更好的 prompt 或更聪明的模型，而是做"代码后端的体检站"。这种"AI 输出 → 工具回环 → AI 自修正"的反馈循环，可能比单纯堆模型规模更有性价比——配合 #1 skills、#3 agentmemory，整套是 2026 年 Claude Code 生态的典型形态。

---

## 生态观察

今天榜单的主旋律是**"AI agent 的工具层正在产业化"**：

- **Claude Code 工具链爆发**：mattpocock/skills、agentmemory、react-doctor 三个项目都直接以 Claude Code 为一等公民，单日合计加星接近 6,000，是任何单一 LLM 工具仓库都没法比的传播速度
- **本地 + 隐私 + Rust 三件套**：openhuman 代表的"私人超级助手"路线，配合 hysteria 的反审查代理，本地化、自托管、抗审查仍是 2026 年开发者群体的强烈偏好
- **反检测进入 C++ 层**：CloakBrowser 一天涨 1,589⭐ 说明 AI agent 爬数据的实战需求已经把 stealth 浏览器顶上了主流热榜
- **教育类 LLM 实战仓库仍然长青**：rasbt/LLMs-from-scratch 和 datawhalechina/hello-agents 各自加 600-800⭐，"从零造一个 LLM/Agent"始终是中文 + 英文社区的高需求方向
- **AI 变现仓库出现**：AiToEarn 单日 +1,264⭐ 显示开发者已经在认真思考"AI 不是用来玩的，是用来挣钱的"——但这类项目的代码质量参差，警惕风口

整体看，2026 年 5 月这一波 GitHub 热度正在从"模型/框架本身"下沉到"模型周边工具链"——记忆、技能、代码检查、反检测、变现，每一层都开始出现明确的细分赢家。
