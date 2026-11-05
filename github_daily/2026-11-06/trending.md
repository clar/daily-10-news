# GitHub Trending 每日热榜 · 2026-11-06

## 今日焦点

> **Skills 生态爆发 · Agent 终端化 · 图谱式 RAG 回归 · 并行 Agent 工作流 · 国产闲鱼监控出海**
>
> - `NVIDIA/auto-ontology` 以 **+2,707⭐** 登顶：NVIDIA 把图谱式语义推理框架开源，剑指 Agent 时代的 RAG 上限。
> - `mattpocock/skills` 持续霸榜 **+2,053⭐**：个人 Agent Skill 集成为开发者"事实标准"模板，总星数突破 31.5 万。
> - `vercel-labs/agent-desktop` **+2,173⭐**：Vercel 用 Rust 把"AI 操作本地电脑"变成 CLI 原语，与 agent-browser 形成双栈。
> - `D4Vinci/Scrapling` **+1,661⭐**：Python 爬虫框架在 Agent 时代第二春——"让模型自己抓网页"成为常规需求。
> - `JiaFeiMiao-K-Cat/DiscImageStudio` **+977⭐** 异军突起：C# 光盘镜像工具黑马，暗示非 AI 领域的小众实用项目仍能破圈。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [NVIDIA/auto-ontology](https://github.com/NVIDIA/auto-ontology) | 面向 LLM/Agent 的图谱式语义推理与 RAG 增强框架 | Python | 7,214 | +2,707⭐ | 567 |
| 2 | [mattpocock/skills](https://github.com/mattpocock/skills) | 个人 Agent Skill 的工程化合集 | Shell | 315,117 | +2,053⭐ | 26,388 |
| 3 | [vercel-labs/agent-desktop](https://github.com/vercel-labs/agent-desktop) | 让 AI Agent 操作本地电脑的 CLI | Rust | 16,754 | +2,173⭐ | 1,177 |
| 4 | [D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling) | 从单请求到大规模爬取的 Python 框架 | Python | 97,896 | +1,661⭐ | 10,251 |
| 5 | [JiaFeiMiao-K-Cat/DiscImageStudio](https://github.com/JiaFeiMiao-K-Cat/DiscImageStudio) | 光盘镜像处理工具 | C# | 7,234 | +977⭐ | 259 |
| 6 | [floci-io/floci](https://github.com/floci-io/floci) | 轻量本地 AWS 模拟器，LocalStack 替代 | Java | 30,360 | +784⭐ | 3,329 |
| 7 | [scenario-labs/skills](https://github.com/scenario-labs/skills) | 通过 Scenario MCP 生成图/视频/音频/3D 资产 | Python | 3,012 | +674⭐ | 265 |
| 8 | [garrytan/gstack](https://github.com/garrytan/gstack) | 模拟 CEO/设计师/QA 等角色的 23 个 Claude Code 工具 | TypeScript | 139,912 | +608⭐ | 20,692 |
| 9 | [max-sixty/worktrunk](https://github.com/max-sixty/worktrunk) | 为并行 AI Agent 工作流打造的 Git worktree 管理 CLI | Rust | 11,483 | +546⭐ | 437 |
| 10 | [Usagi-org/ai-goofish-monitor](https://github.com/Usagi-org/ai-goofish-monitor) | Playwright + AI 实时监控闲鱼商品 | Python | 17,491 | +242⭐ | 2,940 |
| 11 | [ConardLi/garden-skills](https://github.com/ConardLi/garden-skills) | 开源 Skill 集合（网页设计/知识检索/生图） | JavaScript | 14,100 | +241⭐ | 1,644 |
| 12 | [microsoft/VibeVoice](https://github.com/microsoft/VibeVoice) | 微软开源语音 AI 项目 | Python | 55,844 | +214⭐ | 6,279 |
| 13 | [google/skills](https://github.com/google/skills) | Google 产品与技术的 Agent Skills 合集 | Python | 22,333 | +199⭐ | 1,888 |
| 14 | [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) | AI Agent 浏览器自动化 CLI | Rust | 45,836 | +181⭐ | 3,146 |
| 15 | [lz4/lz4](https://github.com/lz4/lz4) | 极速压缩算法 | C | 12,354 | +16⭐ | 1,632 |

---

## 重点项目点评

### 🥇 [NVIDIA/auto-ontology](https://github.com/NVIDIA/auto-ontology) — 今日榜首，+2,707⭐

**NVIDIA 下场做"图谱 RAG"：Agent 时代的上下文战争新一回合**

NVIDIA 在 Agent 工作流这条线上一直靠 TensorRT-LLM 与 Blackwell 硬件撑场，很少直接发框架。这次 auto-ontology 首秀即登顶，说明两件事：（1）**图谱式语义推理在 2026 年底重新回到主流 RAG 技术栈**；（2）NVIDIA 想在"软件上下文层"上插一脚，不再仅做底层 GPU 提供商。框架核心能力是把非结构化数据自动构建为知识图谱，并在查询时做"图 + 向量混合检索"——这与此前 Microsoft GraphRAG、LlamaIndex 的 property graph 路线正面竞争。

今天 +2,707⭐ 的爆发式增长，几乎全部来自 Agent / RAG 社区——这说明开发者不再满足于 "向量 + 关键词混合检索"，而是开始拥抱更结构化的上下文表示。配合最新一代上下文窗口动辄 200 万 tokens，图谱 RAG 的真正价值不在"节省 tokens"，而在**让 Agent 的推理路径可解释、可审计**。

接下来要看：NVIDIA 是否会把它深度绑定到 NIM / Blueprints 生态，以及社区能否在非 NVIDIA 硬件上保持同样性能。

---

### 🥈 [mattpocock/skills](https://github.com/mattpocock/skills) — +2,053⭐

**31.5 万星 Skills 标杆库：个人工程师如何成为 Agent 时代的"事实标准"**

mattpocock/skills 已经不只是一个仓库，而是**整个 Claude Code / Skill 生态的隐形标准**。总星数突破 31.5 万，fork 2.6 万——这意味着它被成千上万个企业内部 Agent 项目直接当作基础模板使用。今天新增 +2,053⭐，和 [google/skills](https://github.com/google/skills)、[ConardLi/garden-skills](https://github.com/ConardLi/garden-skills)、[scenario-labs/skills](https://github.com/scenario-labs/skills) 一起占据 Top15 四席，构成了榜单最清晰的主题线——**Skills 已经成为 Agent 时代的"包管理单位"**。

更深一层的信号是：个人开发者在 AI 时代获得了**打破大厂"基础设施垄断"的真实窗口**。一个前端社区活跃者的个人仓库，星数超过绝大多数大厂框架；Google 的官方 skills 仓库反而排在他下面。这种"民间模板 > 官方模板"的格局，是 2023 年的 Python 时代难以想象的。

---

### 🥉 [vercel-labs/agent-desktop](https://github.com/vercel-labs/agent-desktop) — +2,173⭐

**Vercel 用 Rust 把"Agent 控电脑"做成 CLI 原语**

Vercel 这家本来做前端部署的公司今年完全转型为 **Agent 基础设施提供商**。[agent-desktop](https://github.com/vercel-labs/agent-desktop) 与此前的 [agent-browser](https://github.com/vercel-labs/agent-browser) 配对，分别覆盖"控电脑"与"控浏览器"两条 Agent 操作栈。两者都用 Rust 写——**不是因为性能，而是因为分发**——单一静态二进制，可以嵌入任何语言的 Agent 框架里调用。

今日 +2,173⭐ 的爆发，叠加 agent-browser 继续新增 +181⭐，说明开发者对 "computer use" 从去年还停留在"概念 demo"阶段，到今天开始真正在产品里使用。关键是：Vercel 的发行渠道（Next.js、v0）让这套工具链自然嵌入前端工作流，比 Anthropic 直发的 computer-use 更亲开发者。

这也间接回应了今日 HN 榜首 [sshhole SSH 漏洞事件](https://news.ycombinator.com/item?id=50378228) 所凸显的担忧——**当 Agent 开始大规模控电脑，底层系统的"默认安全性"将成为 2027 年最大的隐忧**。

---

### 🎯 [D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling) — +1,661⭐

**爬虫的 Agent 时代：从"写规则"到"派 Agent"**

一个月前 Scrapling 还没进 Top50，今天一跃 +1,661⭐。原因并不复杂：Agent 生态开始大量需要"实时抓网页"。传统做法是 Playwright + 手写规则，但在 Agent 调用场景里，这类静态规则随网站改版一夜失效，维护成本极高。Scrapling 的卖点是**让大模型本身充当选择器写手**——给 URL 和"你要什么"，框架用 LLM 实时生成 / 修正选择器。

这类"Agent-native"版本的传统工具，预计会在未来 6-12 个月横扫所有分类：爬虫、数据库客户端、监控、构建工具……今天榜单上 Usagi-org/ai-goofish-monitor 的爆红是同一个趋势的佐证——**老工具 + LLM 粘合 = 新爆款**。

---

### 🧩 [max-sixty/worktrunk](https://github.com/max-sixty/worktrunk) — +546⭐

**并行 Agent 工作流的基建：Git worktree 自动管理**

worktrunk 解决一个真实痛点：**让多个 Claude Code / Codex / Cursor Agent 同时工作，又不互相踩车**。做法是自动在同一仓库下管理多个 worktree，每个 Agent 一个独立分支与工作目录，彼此隔离。几周前这还是 power user 手动 `git worktree add` 的玩法，今天已经有专用 CLI 并进入热榜 Top10。

这个仓库是整个榜单最干净的"工程师信号"：**AI Coding 不再是"一个人 + 一个 Agent"的范式，而是"一个人 + 多个 Agent"**。相关信号还包括 [mattpocock/skills](https://github.com/mattpocock/skills) 和 [garrytan/gstack](https://github.com/garrytan/gstack) 的持续霸榜。预计 2027 年 Q1 会看到更多面向 "agent team coordination" 的基础工具出现（例如多 Agent 冲突合并、投票选择器、任务路由）。

---

## 生态观察

今天 Top15 里 **五个是 Skill 仓库，四个是 Agent 操作 CLI**——GitHub Trending 已经从"开源项目橱窗"演变成"Agent 工具链战场"。核心趋势有三：

1. **Skills 成为 Agent 时代的"包"**。个人、大厂、官方、第三方都在争夺这一层——这一层决定了未来 Agent 调用生态的分发权。预计半年内会出现正式的 "skills registry"（类似 npm / pypi），谁能先成为事实标准就能收获整整一代开发者。
2. **Agent 操作栈正在"CLI 化"**。vercel-labs/agent-desktop + agent-browser 用 Rust 把"控电脑/控浏览器"做成静态二进制 CLI。这是 AI 工具链少见的"回归 UNIX 哲学"——不做 SDK 也不做 SaaS，而是让 Agent 像人一样用 shell 调工具。
3. **RAG 的下一站是图谱**。NVIDIA auto-ontology 一天 +2,707⭐，说明在 Context 容量已经不是瓶颈的今天，**可解释性 + 结构化推理**正变成新的瓶颈。接下来一年内，预计 Claude / Gemini / Anthropic 都会推出官方图谱式 RAG 组件。

一句话：**今天的 Trending 不是在说哪个库好用，而是在告诉你"Agent 工程"这个新职业的工具箱长什么样。**

---

*报告日期：2026-11-06（UTC+8）*
