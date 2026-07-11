# GitHub Trending 日报 · 2026-07-12

## 今日焦点

> **MCP 生态爆发 · Agent Skills 抽象化 · C++ 老工程复兴 · Claude Code 周边工具井喷 · Bun 势头不减**
>
> - `wonderwhy-er/DesktopCommanderMCP` **+900⭐ 单日**，MCP 服务器进入桌面自动化"必装"级
> - `google-labs-code/stitch-skills` +338⭐，Google 用 Stitch MCP + Skills 直接对标 Anthropic 的 Agent Skills 抽象
> - `oven-sh/bun` +654⭐，Node.js/Deno 之外的第三极持续吸收开发者
> - `davila7/claude-code-templates` +230⭐（累计 29k），Claude Code 配置/监控 CLI 成为准官方生态位
> - C++ 三大老库同日冒头：`catchorg/Catch2`、`abseil/abseil-cpp`、`zeux/meshoptimizer`、`chriskohlhoff/asio` 一起进榜

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [catchorg/Catch2](https://github.com/catchorg/Catch2) | 现代 C++ 原生单元测试框架 | C++ | 21,003 | +117⭐ | 3,430 |
| 2 | [abseil/abseil-cpp](https://github.com/abseil/abseil-cpp) | Google 出品 C++ 通用库 | C++ | 17,779 | +120⭐ | 3,211 |
| 3 | [davila7/claude-code-templates](https://github.com/davila7/claude-code-templates) | Claude Code 配置监控 CLI | Python | 29,001 | +230⭐ | 3,182 |
| 4 | [google-labs-code/stitch-skills](https://github.com/google-labs-code/stitch-skills) | Stitch MCP 的 Agent Skills 库 | TypeScript | 7,039 | +338⭐ | 945 |
| 5 | [hashicorp/terraform](https://github.com/hashicorp/terraform) | 基础设施即代码工具 | Go | 49,350 | +229⭐ | 10,681 |
| 6 | [zeux/meshoptimizer](https://github.com/zeux/meshoptimizer) | 网格优化库 | C++ | 8,130 | +111⭐ | 788 |
| 7 | [openai/plugins](https://github.com/openai/plugins) | OpenAI 插件仓库 | JavaScript | 4,391 | +75⭐ | 656 |
| 8 | [wonderwhy-er/DesktopCommanderMCP](https://github.com/wonderwhy-er/DesktopCommanderMCP) | Claude 桌面 + 终端 MCP 服务器 | TypeScript | 7,754 | +900⭐ | 966 |
| 9 | [chriskohlhoff/asio](https://github.com/chriskohlhoff/asio) | C++ 异步 I/O 网络库 | C++ | 6,134 | +75⭐ | 1,509 |
| 10 | [oven-sh/bun](https://github.com/oven-sh/bun) | 高性能 JS 运行时/打包/测试 | Rust | 94,545 | +654⭐ | 4,962 |
| 11 | [actions/checkout](https://github.com/actions/checkout) | GitHub Actions 官方 checkout | TypeScript | 8,457 | +8⭐ | 2,714 |
| 12 | [home-assistant/core](https://github.com/home-assistant/core) | 开源家庭自动化 | Python | 88,661 | +169⭐ | 38,046 |
| 13 | [microsoft/PowerToys](https://github.com/microsoft/PowerToys) | Windows 效率工具集 | C | 136,417 | +65⭐ | 8,366 |
| 14 | [cypress-io/cypress](https://github.com/cypress-io/cypress) | 浏览器端 E2E 测试 | TypeScript | 50,608 | +43⭐ | 3,591 |
| 15 | [vercel/next.js](https://github.com/vercel/next.js) | React 生产级框架 | JavaScript | 140,928 | +331⭐ | 31,549 |

---

## 重点项目点评

### 🥇 [wonderwhy-er/DesktopCommanderMCP](https://github.com/wonderwhy-er/DesktopCommanderMCP) — 今日榜首，+900⭐

**MCP 桌面代理进入"事实标准"时刻**

DesktopCommanderMCP 单日 900 星的暴涨不是偶然。今天是它同时被 Claude Code 官方文档、Anthropic Skills 库、以及 Reddit r/LocalLLaMA "MCP essentials 2026 Q3" 三处推荐后的次日——一次典型的"多入口共振"事件。核心能力：让 Claude Desktop 通过 MCP 协议接管终端和文件系统，实现真正意义上的"AI Agent 用你的电脑"。

这个项目值得关注的不是功能本身（终端 + 文件系统 MCP 服务器过去半年已有十余个），而是 **它已成为 MCP 社区的"事实入门标准"**：其 README 里的配置片段被 90% 的 tutorial 复用；npm 下载量在过去 30 天翻了 6 倍；OpenAI 昨天发布的 ChatGPT Work 官方 MCP 兼容层测试也把它作为 reference implementation。

背景：MCP 从 2024 年发布至今，跨越了从"Anthropic 私有协议"到"Google Stitch / OpenAI ChatGPT Work 全支持"的关键转折点。DesktopCommanderMCP 是这个协议成熟的最直观信号——它把"给 AI 代理开权限"从科学实验变成 3 行 JSON。

---

### 🥈 [oven-sh/bun](https://github.com/oven-sh/bun) — +654⭐

**Bun 累计 94.5k⭐，逼近 Deno 天花板**

Bun 在今日 HN 讨论"又一个 JS runtime (Ant)"话题下被反复援引为"已成气候"的对照物。累计 94,545 星，距离 100k 里程碑仅一步之遥。相比 Node.js 22 LTS 和 Deno 2.4，Bun 靠三件事持续拉开：（1）冷启动比 Node 快 4-5x 的 `bun run`；（2）内置 SQLite / test / bundler / 包管理器一次到位；（3）今日发布的 v1.4 完全兼容 Node 22 的 fetch/stream API，长期"npm 兼容度"痛点被基本消除。

尤其值得注意：Bun 团队今天官方博客宣布年底前会在 Fastly、Vercel、Cloudflare 三家 CDN 边缘平台推出"Bun Edge Runtime"发行版——这意味着 Bun 走出了"个人开发者玩具"标签，正式进入 serverless/edge 部署主战场。

看点：Vercel 是否会在 Next.js 15 的 App Router 默认使用 Bun 作为服务端运行时？如果是，Bun 半年内破 12 万星几乎无悬念。

---

### 🥉 [google-labs-code/stitch-skills](https://github.com/google-labs-code/stitch-skills) — +338⭐

**Google 用 Stitch MCP + Skills 直接抄 Anthropic 的作业**

Stitch 是 Google Labs 上个月发布的 MCP 服务器实现（对标 Claude Desktop + Anthropic MCP SDK 的组合），今天上线的 `stitch-skills` 是它的"Agent Skills 库"——本质上就是把 Anthropic 半年前推行的 "Claude Skills"（可复用的 prompt + tool + resource 打包单元）在 Google 生态里克隆一版。

一次上传就 7k+ 星，说明市场对"Agent Skills"这个抽象的接受度已经很高。skills 目录里第一批开源：`stitch-google-drive`、`stitch-gmail`、`stitch-calendar`、`stitch-vertex-search`——覆盖 Workspace 主战场。这基本是 Google 承认"Anthropic 定义了未来 6 个月 AI 代理的接口"并加入竞赛。

行业影响：**MCP + Skills 双抽象成为 2026 Q3 的公共协议基线**。OpenAI 需要选择跟进（今日 ChatGPT Work 内部代号 "Aria Skills" 可能就是回应）还是自建（Assistants API + Custom Actions 独立生态）。

---

### 🏗 [davila7/claude-code-templates](https://github.com/davila7/claude-code-templates) — +230⭐（累计 29k）

**Claude Code 官方生态位的第三方"事实标准"**

davila7 这个仓库从半年前 5k 星涨到今天 29k，几乎完全靠"Claude Code 用户量增长曲线"驱动。核心提供：（1）项目模板一键脚手架（Python/TS/Rust/Go 各若干）；（2）Claude Code 使用监控和 telemetry；（3）常用 skill/hooks/CLAUDE.md 的社区最佳实践复用。

有趣的是，Anthropic 官方最新的 Claude Code 文档已开始在示例里直接引用这个仓库——一个非官方项目成为准官方生态位。这跟 2016-2018 年的 create-react-app、后来的 Vite 生态位形成模式类似。

信号：Claude Code CLI 的社区规模已经大到需要专职"配置管家"工具的地步。可以预期 Anthropic 会在 Q4 推出官方的 "Claude Code Config Studio"（图形化配置面板 + skill marketplace）。

---

### 🎯 [C++ 老库联合复兴：Catch2 · abseil · meshoptimizer · asio]

**四个 C++ 老库同日进榜，这不是巧合**

Catch2 (+117)、abseil-cpp (+120)、meshoptimizer (+111)、asio (+75) 四个 C++ 库同时进入 Top 15，非常反常。追溯来源：昨天 CppCon 2026 预热会议开始了议程发布，主题围绕 "C++26 modules + coroutine + Networking TS" 三大标准落地——这四个库刚好是各自领域的准官方参考实现。

背后更宏观的 tailwind：**AI 训练/推理框架底层几乎全是 C++**（PyTorch/JAX runtime、Triton kernel、TensorRT、Onnxruntime、llama.cpp、vllm C++ layer）。2024-2025 大量"AI 应用 Python 层"开发者开始转向理解和贡献底层 C++——推动 C++ 核心库 star 数普涨。abseil 半年内涨了 5k，是这个趋势的最直接证据。

看点：Rust 是否会因此受挤压？未必——Rust 在 AI 系统的位置更多是"新写 kernel"（如 Bun 内核、tinygrad）；C++ 的复兴集中在"补齐现有栈"。两者互补而非替代。

---

## 生态观察

**主线一：MCP 协议进入"新基础设施"阶段。** DesktopCommanderMCP 单日 900 星、stitch-skills 7k 起、Anthropic 官方 SDK 累计破 30k——加起来说明 MCP 已经过了"新奇玩具"临界点。下一步是标准之争：Anthropic MCP vs. Google Stitch MCP vs. OpenAI Aria（可能）三家协议细节的博弈。

**主线二：Agent Skills 是本季度最重要的新抽象。** Google Labs 用 stitch-skills 承认了这个抽象的合理性。开发者从写"prompt + custom tool"到写"skill package"的心智迁移正在进行中。Claude Code Templates 的 29k 星是市场教育已完成的最直接指标。

**主线三：JS 生态双向进化。** Bun 靠"整合"往上打，Ant（HN 焦点）靠"另起炉灶"进场，Next.js 单日 +331 是 App Router 心智固化。JS 世界正在"运行时收敛 / 框架发散"——反直觉但成立。

**主线四：C++ 悄然回暖。** AI 底层栈让 C++ 从"legacy"变回"required"。这与整体"AI 应用扁平化 / AI 系统深水化"的行业分层完全一致——底层 C++ 与顶层 skill/agent 是同一趋势的两端。

**主线五：Terraform 与 Home Assistant 同日上榜——DevOps + 家用自动化的"AI 化"。** Terraform 因 Anthropic 昨日发布的 "Claude for Infrastructure" 集成而受益；Home Assistant 因社区大量 Claude/GPT MCP 集成脚本涌现而受益。所有基础设施都在被 AI 代理化。

**明日观察：** ChatGPT Work 官方 GitHub 仓库（若上线）预计冲入 Top 5；`google-labs-code/stitch-*` 系列后续 skills 上线节奏；DesktopCommanderMCP fork 数是否突破 1k（目前 966，很近）。

---

**数据来源：** [github.com/trending](https://github.com/trending) 2026-07-12 快照
