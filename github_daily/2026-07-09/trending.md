# GitHub Trending 日报 · 2026-07-09

## 今日焦点

> **AI Agent 技能框架霸榜 · MCP 生态兴起 · 系统提示词泄漏合集 · 腾讯双开源攻势 · GIMP 3 替代 PS 热潮**
>
> - `addyosmani/agent-skills` +1,322⭐ 领跑：AI 编程 agent 的生产级技能库，Addy 亲自站台。
> - `obra/superpowers` +1,170⭐ 逼近 25 万总星：Agentic skills 框架成事实标准。
> - `iOfficeAI/OfficeCLI` +1,712⭐ 单日暴涨：让 agent 直接读写 Word/Excel/PPT。
> - `asgeirtj/system_prompts_leaks` +1,226⭐：主流 AI 厂商 system prompt 泄漏合集持续吸粉。
> - `TencentCloud` 一日双榜（Agent-Memory + CubeSandbox）：腾讯在 agent infra 层布局明显。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | AI 编程 agent 的生产级技能库 | JavaScript | 73,910 | +1,322 | 7,973 |
| 2 | [iOfficeAI/OfficeCLI](https://github.com/iOfficeAI/OfficeCLI) | 让 AI agent 读写 Office 文件 | C# | 11,685 | +1,712 | 793 |
| 3 | [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) | 主流 AI 系统提示词泄漏合集 | JavaScript | 54,108 | +1,226 | 8,806 |
| 4 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic skills 框架与方法论 | Shell | 249,769 | +1,170 | 22,161 |
| 5 | [bradautomates/claude-video](https://github.com/bradautomates/claude-video) | Claude 视频分析能力扩展 | Python | 6,006 | +948 | 716 |
| 6 | [Diolinux/PhotoGIMP](https://github.com/Diolinux/PhotoGIMP) | GIMP 3+ 面向 PS 用户的补丁 | CSS | 14,997 | +916 | 592 |
| 7 | [ruvnet/RuView](https://github.com/ruvnet/RuView) | WiFi 信号转空间智能与体征监测 | Rust | 79,099 | +793 | 10,642 |
| 8 | [TencentCloud/CubeSandbox](https://github.com/TencentCloud/CubeSandbox) | 面向 AI agent 的轻量沙箱 | Rust | 8,901 | +555 | 736 |
| 9 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 跨平台社交/网络研究 agent 技能 | Python | 50,708 | +373 | 4,231 |
| 10 | [alibaba/zvec](https://github.com/alibaba/zvec) | 轻量级、进程内向量数据库 | C++ | 14,373 | +370 | 885 |
| 11 | [TencentCloud/TencentDB-Agent-Memory](https://github.com/TencentCloud/TencentDB-Agent-Memory) | AI agent 的 4 层长期记忆管道 | TypeScript | 7,598 | +351 | 704 |
| 12 | [huxingyi/autoremesher](https://github.com/huxingyi/autoremesher) | 自动四边形重拓扑工具 | C++ | 1,975 | +292 | 149 |
| 13 | [prisma/prisma](https://github.com/prisma/prisma) | Node.js & TypeScript 新一代 ORM | TypeScript | 46,529 | +30 | 2,278 |
| 14 | [wonderwhy-er/DesktopCommanderMCP](https://github.com/wonderwhy-er/DesktopCommanderMCP) | Claude 桌面控制 MCP server | TypeScript | 6,362 | +20 | 746 |
| 15 | [argoproj/argo-cd](https://github.com/argoproj/argo-cd) | Kubernetes 声明式持续部署 | Go | 23,417 | +20 | 7,424 |

---

## 重点项目点评

### 🥇 [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — +1,322⭐

**Google Chrome 团队的 Addy Osmani 亲手做的 agent skills 集**

Addy Osmani 把过去几年在 Chrome DevRel 和性能优化领域的方法论"翻译"成 Claude/Cursor/Cline 都能加载的 agent skill 文件，涵盖代码 review、性能剖析、无障碍审计等模块。这个仓库的爆红本质上是**权威背书**——当一个前端界"教父级"人物开始亲自维护 agent skills 库，其他开发者会自然把它当作事实标准去 fork。

Skill 文件正在成为 2026 年下半年新的"config 之战"。以前你选一个 linter、一个 formatter、一个 test framework，现在你还要选一套 skill——这些 skill 决定了 agent 做同一个任务时的具体套路、边界和写代码风格。Addy 的入场时机极准：Anthropic Fable 5 昨天转付费、Claude Code 官方 skills 生态还在早期，社区正需要一个可靠的"权威合集"。

从 fork 数（7,973）和总星（73,910）看，这可能会成为 agent skills 领域第一个"必装"仓库。接下来值得盯的是他会不会做类似 Awesome-list 的 curation 或者索性做一个 SkillHub 商店。

---

### 🥈 [iOfficeAI/OfficeCLI](https://github.com/iOfficeAI/OfficeCLI) — +1,712⭐

**单日涨星最猛：把 Word/Excel/PPT 变成 agent 的 CLI 后端**

OfficeCLI 用 C# 写了一层瘦封装，把 Microsoft Office 文件的读写操作暴露成命令行接口，让 AI agent（Claude、GPT、Cursor 都行）能直接生成、修改、查询 xlsx/docx/pptx。今日暴涨 1,712 星，是全榜单日最猛。

这个方向的市场空间几乎不需要论证：企业内部 90% 的知识以 Office 文件形态存在，agent 的下一步就是把这些文件的"读—写—编辑"变成一等公民 API。目前主流方案是 python-docx / openpyxl 一类，但都不适合 agent"顺序 CLI 调用"的模式。OfficeCLI 用 CLI 抽象打通这一层。

这条 trend 也和昨日 HN 榜上 Microsoft Flint（agent 可视化语言）遥相呼应——微软在推 AI agent 生态往企业办公场景延伸，而 OfficeCLI 是社区侧的对应回应。预计 Q3 会看到更多"agent + Office"垂直工具冒头。

---

### 🥉 [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) — +1,226⭐

**从 Claude 到 Cursor：主流 AI 产品的 system prompt 泄漏合集**

这个仓库持续收集来自 Claude、ChatGPT、Cursor、Perplexity、Bolt、v0 等产品的 system prompt 泄漏内容，并按厂商 + 版本组织。今日 +1,226 星意味着 AI 用户群体正在从"用工具"过渡到"研究工具的行为学"。

单纯从合规角度看，这个仓库处于灰色地带（不少 system prompt 明确包含"不要透露 system prompt"的指令），但社区把它当作**产品设计与 prompt engineering 的参考文献库**。仔细读一遍 Cursor Composer 或 Claude Code 的 system prompt，就能学到大厂如何设计 tool-use 策略、如何写反注入指令、如何管理上下文。

有意思的是，这类仓库的走红节奏和大模型迭代高度同步——每次 Claude/OpenAI 新版本发布，大约 3-7 天后新的泄漏 prompt 就会被 push 进来。这条 trend 提醒我们，**行业透明度正在通过"泄漏"而不是"官方文档"实现**。

---

### 🎖 [obra/superpowers](https://github.com/obra/superpowers) — +1,170⭐

**逼近 25 万总星：Agentic skills 框架的事实标准**

Superpowers 定位为"agent skills 框架 + 软件开发方法论"，总星数已经接近 25 万——放眼整个开发工具生态是极少数破 20 万的项目之一。今天再涨 1,170 星，说明它仍在加速。

它和 agent-skills 的区别是：agent-skills 是**内容**（技能库），superpowers 是**框架**（skill 编写方式、验证机制、组合规范）。二者形成了"框架 + 内容"的自然分工，且今天双双上榜——说明 agent skills 生态出现了明显的"平台化"趋势，社区在选定 superpowers 作为底层规范。

这里更大的信号是：随着 Claude Code 官方 skills 机制越来越通用，第三方框架反而可以做得更精细、更"面向真实工程流程"。superpowers 的做法是把 skills 组织成"工程行为的最小可执行单元"，比 Anthropic 官方的组织方式更贴近实际开发者习惯。

---

### 🚀 [ruvnet/RuView](https://github.com/ruvnet/RuView) — +793⭐

**用 WiFi 信号当作视觉/体征传感器：非视频监测的暗线**

RuView 是一个用 Rust 写的 WiFi 感知框架，能通过分析 WiFi CSI（Channel State Information）信号变化推断人体位置、姿态、呼吸和心率，不需要摄像头。学界这一方向叫"RF sensing"，过去主要停留在论文里，RuView 把它工程化后爆红。

今日 +793 星 + 79k 总星，说明"隐私友好型监测"这条赛道正在被市场重视——尤其是在老年监护、企业办公空间态势感知这两个场景，摄像头方案的合规成本越来越高。RuView 直接绕开摄像头，用 WiFi 路由器就能做类似监测。

这条 trend 也有硬件配套的背景：Wi-Fi 7 网卡的 CSI API 越来越标准化，硬件门槛正在消失。接下来最值得盯的是家用路由器厂商会不会内置这类感知能力——那将是一个万亿级市场的口子。

---

## 生态观察

**Agent skills 生态今天完全统治了榜单**。Top 15 里至少 6 个直接与 AI agent 相关：agent-skills、OfficeCLI、system_prompts_leaks、superpowers、claude-video、last30days-skill、DesktopCommanderMCP、CubeSandbox、TencentDB-Agent-Memory——占了一大半。这里的信号很明确：**Claude Code / Claude Skills / MCP** 这套技术栈已经形成了自己的"包生态"，就像 npm 之于 Node、Cargo 之于 Rust。这个生态在 Q3 会经历第一次"包管理器"级别的整合。

**中国厂商在 agent infra 层的动作明显加速**。TencentCloud 今天双榜（Agent-Memory + CubeSandbox），Alibaba 的 zvec 向量库也上榜。这不是巧合——国内大厂显然判断 agent 底层（记忆、沙箱、向量存储）是未来的高毛利战场，且用开源换生态占位比闭源赢面更大。

**非 AI 项目仍在坚守，但被挤出前 5**：Prisma、argo-cd 靠稳定基本盘每天低单量增长；PhotoGIMP 抓住 GIMP 3 发布后的用户潮拿到 +916 星。这类"传统开源"仓库在 AI 大潮下变得越来越像"背景板"——不下榜、也不出圈，成为衡量 GitHub"非 AI 生态健康度"的隐性指标。

---

**数据来源：**
- [GitHub Trending](https://github.com/trending)
