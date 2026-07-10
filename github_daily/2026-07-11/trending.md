# GitHub Trending 日报 · 2026-07-11

## 今日焦点

> **Claude Skills 生态爆炸 · MCP 服务器成流量入口 · Bun 稳步蚕食 Node · 中国厂商发力 Agent 记忆 · C++ 老库集体回暖**
>
> - `mattpocock/skills` +1,663⭐——TypeScript 圈明星 Matt Pocock 把自己的 `.claude` 目录开源，直接冲进榜首。
> - `addyosmani/agent-skills` +1,114⭐——Google Chrome 团队 Addy Osmani 的"生产级 AI 编码 Agent 技能"合集。
> - `obra/superpowers` +969⭐——总星数 25 万+，把"Agentic Skills 框架"推到主流工作流层面。
> - `wonderwhy-er/DesktopCommanderMCP` +349⭐——给 Claude 加终端控制/文件系统能力的 MCP 服务器持续吸流。
> - `TencentCloud/TencentDB-Agent-Memory` +134⭐——腾讯云开源本地长期记忆系统，中国云厂商首次在 Agent 记忆赛道立旗。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [mattpocock/skills](https://github.com/mattpocock/skills) | 我的 `.claude` 目录，工程师专用 | Shell | 164,542 | +1,663 | 14,157 |
| 2 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | 生产级 AI 编码 Agent 技能集 | JavaScript | 76,776 | +1,114 | 8,245 |
| 3 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic Skills 框架 + 方法论 | Shell | 251,748 | +969 | 22,462 |
| 4 | [wonderwhy-er/DesktopCommanderMCP](https://github.com/wonderwhy-er/DesktopCommanderMCP) | 给 Claude 加终端/FS 能力的 MCP | TypeScript | 7,238 | +349 | 921 |
| 5 | [oven-sh/bun](https://github.com/oven-sh/bun) | 极速 JS 运行时/打包/测试一体化 | Rust | 94,178 | +307 | 4,938 |
| 6 | [tailscale/tailscale](https://github.com/tailscale/tailscale) | 最简单最安全的 WireGuard + 2FA | Go | 33,618 | +183 | 2,909 |
| 7 | [microsoft/TypeScript](https://github.com/microsoft/TypeScript) | TS 官方仓库 | TypeScript | 109,760 | +166 | 13,631 |
| 8 | [TencentCloud/TencentDB-Agent-Memory](https://github.com/TencentCloud/TencentDB-Agent-Memory) | AI Agent 4 级本地长期记忆 | TypeScript | 8,205 | +134 | 754 |
| 9 | [abseil/abseil-cpp](https://github.com/abseil/abseil-cpp) | Google Abseil C++ 基础库 | C++ | 17,506 | +106 | 3,193 |
| 10 | [davila7/claude-code-templates](https://github.com/davila7/claude-code-templates) | Claude Code 配置与监控 CLI | Python | 28,749 | +104 | 3,160 |
| 11 | [google-labs-code/stitch-skills](https://github.com/google-labs-code/stitch-skills) | Google Stitch MCP 配套技能库 | TypeScript | 6,712 | +101 | 927 |
| 12 | [chriskohlhoff/asio](https://github.com/chriskohlhoff/asio) | C++ 异步网络库 | C++ | 6,064 | +87 | 1,499 |
| 13 | [zeux/meshoptimizer](https://github.com/zeux/meshoptimizer) | 网格优化库，加速渲染 | C++ | 8,014 | +86 | 782 |
| 14 | [catchorg/Catch2](https://github.com/catchorg/Catch2) | 现代 C++ 单测/TDD/BDD 框架 | C++ | 20,605 | +69 | 3,406 |
| 15 | [jbeder/yaml-cpp](https://github.com/jbeder/yaml-cpp) | YAML C++ 解析器 | C++ | 6,072 | +65 | 2,255 |

---

## 重点项目点评

### 🥇 [mattpocock/skills](https://github.com/mattpocock/skills) — 今日榜首，+1,663⭐

**TypeScript 顶流把自己的 `.claude` 目录搬到 GitHub，一天冲上热榜第一**

Matt Pocock（Total TypeScript 创始人、TS 教材第一 KOL）今天开源了他的整个 `.claude/skills` 目录，标题就是"Skills for Real Engineers. Straight from my .claude directory"。仓库里是他在实际工程中长期沉淀的 Skill 定义：TypeScript 类型体操调试、Zod schema 生成、npm 包版本冲突排查、React 组件迁移等等。总星数已经 16.4 万，说明这个仓库其实累积很久，但今天的 +1,663 峰值来自昨天他在推特发的一条推文"stop copy-pasting the same prompt into Claude, put it in a Skill"。

这个仓库的技术含量本身并不高（大部分 Skill 是几百行 Markdown），但意义在于确认了一件事：**Claude Skills 已经变成"个人品牌资产"**。就像 dotfiles 时代 vim/emacs 老手会把配置放 GitHub 作为身份符号，2026 年的 AI 时代，Skills 成了新型 dotfiles——你的 `.claude/skills` 目录代表你的工程品味。

值得留意的次生效应：Matt 明确写在 README 里的"我不接受 PR，这是我的目录不是社区标准"——这种"作者制"路线跟 dotfiles 生态早期一模一样。

---

### 🥈 [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) — +1,114⭐

**Google Chrome 团队负责人 Addy Osmani 的"生产级"Skill 合集**

Addy Osmani（Chrome 团队 Web Platform 主管、《Learning JavaScript Design Patterns》作者）的 `agent-skills` 仓库主打"production-grade"——跟 mattpocock/skills 的"个人品味"路线不同，Addy 的合集更偏企业协作：CI 集成、code review 模板、生产事故 postmortem 生成、依赖升级评估。7.7 万总星、+1,114 日增，说明市场对"有权威署名的 Skill 集合"的信任建立了。

值得注意的一点是仓库结构：Addy 把每个 Skill 都放在 `skills/{category}/{skill}/SKILL.md` 里，明确了目录层级，并且写了一个 `skills-manifest.json` 用于让 Claude Code / Cursor 自动识别可用 Skills。这跟本月 obra/superpowers 提出的 Skill Manifest 规范互相呼应——**社区正在自发收敛出 Skill 的目录约定**。

---

### 🥉 [obra/superpowers](https://github.com/obra/superpowers) — +969⭐

**"Agentic Skills 框架" 累计 25 万星，成为事实上的方法论标准**

obra（Jesse Vincent，早期 Perl 6/rakudo/Prophet 作者、后来做过多个 Rails 工程项目）的 `superpowers` 已经累积 25.1 万星、22.4k fork。它比单纯的 Skills 集合更进一步——是**一个方法论 + 框架**：定义了 Skill 的分层（个人层、项目层、组织层）、生命周期（起草/评审/退役）、测试机制（每个 Skill 都要有 golden test）。

这个仓库今天冲上第三是因为 Jesse 昨天发了 v3.0，主要引入"Skill Composition"——即让多个 Skill 通过声明式配置组合成更复杂的工作流。这跟 UNIX pipe 哲学一脉相承，也和 mattpocock/skills 的"作者制"形成有趣对照：obra 走的是标准化路线，Matt 走的是个性化路线，两者互补。

---

### 🎯 No.4 · [wonderwhy-er/DesktopCommanderMCP](https://github.com/wonderwhy-er/DesktopCommanderMCP) — +349⭐

**MCP 服务器成为 Claude 生态的下一个流量入口**

MCP（Model Context Protocol）今年被 Anthropic 正式确立为跨模型标准后，MCP 服务器仓库正在批量涌现。DesktopCommanderMCP 是给 Claude Desktop 加"本地终端 + 文件系统 + 文件差异编辑"能力的服务器，7.2k 星、+349 日增，反映用户对"Claude Desktop 版功能补齐"的强需求——因为官方 Claude Desktop 本身刻意保守，很多 IDE-like 功能都靠社区 MCP 补。

它的意义在于确认了 MCP 生态的"网关效应"：一旦某个 MCP 成为默认安装，就能截获所有 Claude 与本地环境的交互，某种意义上是新时代的浏览器扩展。

---

### 🇨🇳 No.5 · [TencentCloud/TencentDB-Agent-Memory](https://github.com/TencentCloud/TencentDB-Agent-Memory) — +134⭐

**中国云厂商首次在 Agent 记忆赛道开源立旗**

腾讯云开源了 TencentDB-Agent-Memory，主打"完全本地长期记忆"，架构是 4 层渐进流水线（原始事件 → 会话摘要 → 主题聚合 → 长期知识）。8.2k 星、+134 日增，属于中等热度，但战略意义比数字重要——**这是中国云厂商首次在 Agent 记忆基础设施赛道亮相**（此前主要是 mem0、Zep 主导）。

技术上有几个亮点：4 级流水线设计是对 LLM 上下文窗口有限性的直接应对；完全本地（可选依赖 TencentDB）意味着企业内部数据不出域，符合中国合规环境；MIT License 也让海外开发者可以直接引入。跟 mem0（美系）、Letta（美系）、Zep（美系）形成对照，Agent 记忆基础设施成为 2026 下半年中美开源竞争的下一个前线。

---

## 生态观察

- **Claude Skills = 新型 dotfiles**：mattpocock、addyosmani、obra 三个仓库合计今日新增 3,746 星，说明 Skills 生态从工具属性升级为"个人/团队品牌资产"。Skills 目录约定（`skills/{category}/{name}/SKILL.md` + manifest）在自发收敛中，Anthropic 官方目前没出规范但社区已经动手了。
- **MCP 生态处于"扩展商店化"前夜**：DesktopCommanderMCP、TencentDB-Agent-Memory、google-labs-code/stitch-skills 三条不同路径的 MCP 服务器同时进榜，说明 MCP 正在成为多云/多模型的"跨端接口"。下一步等着看 Anthropic 或第三方推出 MCP Store。
- **C++ 老库集体回暖**：abseil-cpp、asio、Catch2、meshoptimizer、yaml-cpp 五个 C++ 传统库同时上榜是罕见现象，可能与近期 Bun / Zed / Ghostty 等 native 项目的走红有关——AI 助手让 C++ 门槛降低，新一代开发者回流。
- **Bun 继续稳步蚕食 Node**：+307 星把总数推向 9.4 万，速度稳定。跟 Node.js 生态最近的分裂（Deno 2.0 尝试反攻、npm 政策变动）形成对比，Bun 的"包管理 + 运行时 + 打包 + 测试一体化"故事继续说服市场。
- **中国厂商 open source 差异化**：腾讯云选 Agent 记忆而非模型层，是聪明的差异化——避开与 OpenAI/Anthropic 正面模型竞争，切基础设施细分。同类国内玩家（阿里 Qwen-Memory、字节扣子长记忆）可能会跟进。

---

*榜单快照时间：2026-07-11 CST，数据来自 [github.com/trending](https://github.com/trending)。*
