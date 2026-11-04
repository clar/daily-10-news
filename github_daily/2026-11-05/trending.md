# GitHub Trending 日报 · 2026-11-05

## 今日焦点

> **代理桌面成热门 · NVIDIA 下场做知识图谱 · 2.78T 参数模型 CPU 跑 · 代理记忆/会话复用 · 工程"技能库"分发**
>
> - `vercel-labs/agent-desktop` 今日 +2,463⭐,Rust 写的"计算机使用"CLI,把 computer-use agent 搬出实验室
> - `NVIDIA/auto-ontology` 今日 +2,053⭐,英伟达亲自下场推"图谱 + LLM"的语义推理层
> - `D4Vinci/Scrapling` 今日 +2,006⭐,爬虫框架重新回榜,agent 数据供给需求压顶
> - `JiaFeiMiao-K-Cat/DiscImageStudio` 今日 +1,792⭐,一个几乎无介绍的 C# 磁盘镜像工具神秘冲榜
> - `FareedKhan-dev/kimi-k3-in-c` +351⭐,把 2.78 万亿参数的 Kimi K3 用 C99 塞进 8.24GB RAM 跑在一颗 CPU 上

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [NVIDIA/auto-ontology](https://github.com/NVIDIA/auto-ontology) | 面向 LLM/agent 的图谱式语义推理层 | Python | 4,801 | +2,053 | 384 |
| 2 | [max-sixty/worktrunk](https://github.com/max-sixty/worktrunk) | 为并行 AI agent 设计的 Git worktree CLI | Rust | 10,991 | +524 | 410 |
| 3 | [mattpocock/skills](https://github.com/mattpocock/skills) | 作者个人 .agents 目录中的工程技能集 | Shell | 313,220 | +1,376 | 26,279 |
| 4 | [floci-io/floci](https://github.com/floci-io/floci) | 轻量级 AWS 本地模拟器 | Java | 29,551 | +1,082 | 3,271 |
| 5 | [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | 捕获 agent 会话、压缩后回注,实现记忆 | TypeScript | 112,778 | +1,165 | 9,798 |
| 6 | [vercel-labs/agent-desktop](https://github.com/vercel-labs/agent-desktop) | AI agent 的 computer-use CLI | Rust | 14,921 | +2,463 | 1,030 |
| 7 | [github/spec-kit](https://github.com/github/spec-kit) | 面向 Spec-Driven Development 的脚手架 | Python | 147,253 | +810 | 13,213 |
| 8 | [The-PR-Agent/pr-agent](https://github.com/The-PR-Agent/pr-agent) | 开源 AI PR 评审(非 Qodo 免费版) | Python | 14,711 | +279 | 2,092 |
| 9 | [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) | 关键词 → HD 短视频全流程自动化 | Python | 138,897 | +615 | 22,165 |
| 10 | [garrytan/gstack](https://github.com/garrytan/gstack) | 23 个 Claude Code 角色工具(CEO/设计/QA) | TypeScript | 139,291 | +285 | 20,629 |
| 11 | [FareedKhan-dev/kimi-k3-in-c](https://github.com/FareedKhan-dev/kimi-k3-in-c) | 单 CPU 跑 2.78T 参数 Kimi K3(8.24GB RAM) | C | 10,250 | +351 | 1,625 |
| 12 | [JiaFeiMiao-K-Cat/DiscImageStudio](https://github.com/JiaFeiMiao-K-Cat/DiscImageStudio) | 磁盘镜像工具(页面未附描述) | C# | 6,529 | +1,792 | 232 |
| 13 | [MichaelCade/90DaysOfDevOps](https://github.com/MichaelCade/90DaysOfDevOps) | 90 天 DevOps 学习路线图 | Shell | 30,375 | +264 | 6,790 |
| 14 | [D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling) | 从单次请求到全面抓取的 Web 爬取框架 | Python | 96,435 | +2,006 | 10,096 |
| 15 | [Thysrael/Horizon](https://github.com/Thysrael/Horizon) | 中英双语 AI 新闻日报 radar | Python | 12,452 | +121 | 1,817 |

---

## 重点项目点评

### 🥇 [vercel-labs/agent-desktop](https://github.com/vercel-labs/agent-desktop) —— 今日榜首,+2,463⭐

**Vercel 把"computer use"从实验室搬到了 Rust 二进制。**

这是本周 AI 工程圈最快被转发的项目:一个 Rust 写的 CLI,把 AI 代理对桌面 GUI 的操控能力(截屏 → 推理 → 点击/输入)包装成稳定的命令行工具,支持接入 OpenAI、Anthropic 以及本地 vLLM 后端。意义不在"又一个 computer-use demo",而在**部署形态**:
- Rust 单二进制,交叉编译,服务器/CI/无头环境都能跑
- 把 Anthropic 的 computer-use、OpenAI 的 Operator-style 调用统一成一个可脚本化接口
- Vercel 的品牌背书让企业试用门槛显著下降

今天 AI 日报里 OpenAI 用 GPT-6 Astra 一周自主设计出 Codex 配套硬件、Apple 在 10-K 风险因素里把"agent 越权交易"列为独立风险 —— 和 agent-desktop 的爆发相互呼应:**"桌面代理商业化"这条赛道的工具链正在 2026 Q4 集中成熟**,风险和生产力同时在爬坡。

---

### 🥈 [NVIDIA/auto-ontology](https://github.com/NVIDIA/auto-ontology) —— +2,053⭐

**英伟达亲自下场做"图谱 + LLM"的语义推理层。**

NVIDIA 很少主动做上层应用框架,这次例外。auto-ontology 的目标是让企业对接自家数据时能自动构造"实体 - 关系 - 约束"的本体层,给 LLM 和 agent 提供可解释的推理锚点 —— 本质上是把"RAG"升级成"推理图谱"。背后是 NVIDIA 自己的战略诉求:当下 LLM 推理栈的差异化越来越窄,英伟达需要给企业客户提供"除了 GPU 以外,我还能帮你落地业务"的叙事。

值得注意的三点:
- 项目用 Python 而非 C++/CUDA,目标受众是数据团队,不是系统工程师
- 文档明确对标 Neo4j + LangChain 的组合,官方提供适配
- README 强调与 Blueprint / Enterprise RAG 的集成 —— 这是 NVIDIA 把"全栈 AI 工厂"做实的一块拼图

对社区的影响:知识图谱 / Ontology 这个被 Google、IBM 冷落多年的方向,在 LLM 时代反而被硬件厂商重新激活。企业要的不是更聪明的 chat,而是"答案可追溯"。

---

### 🧠 [FareedKhan-dev/kimi-k3-in-c](https://github.com/FareedKhan-dev/kimi-k3-in-c) —— +351⭐

**2.78 万亿参数的 Kimi K3,一个 CPU、8.24 GB RAM、纯 C99 跑起来。**

这不是量化,也不是蒸馏 —— 作者用 memory-mapped + 分块量化 + 精心设计的前向调度,把 Kimi K3 这种规模的模型做成"可以在 CPU 上以可用延迟运行",代码是便携 C99。它当然慢(README 给出的是 single-digit tokens/s),但象征意义巨大:

- 2.78T 参数被塞进 8.24GB —— 等于把"必须进 H100"的门槛,降到"在家开发板都能装"的水平
- 纯 C99 代表零依赖,可以编进嵌入式、路由器、甚至 WebAssembly
- 与 llama.cpp 在 2023 年的意义相似 —— 它不是最快的,但是让"开源大模型 + 普通硬件"的故事成立的那颗种子

这类项目在今天的 Hacker News 高赞帖"AI 翻出 40 年技术债"的语境下更有意味:底层优化这条路还远没有走完,**AI 不是只能靠砸 GPU** —— C99 写得好一样能挤出数量级。

---

### 🧬 [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) —— +1,165⭐

**Agent 上下文在"长会话 → 跨会话"过渡,记忆基础设施开始商品化。**

claude-mem 做的事很直白:监听 agent 的会话流,把工具调用、决策、文件读写编码成压缩表示,下一次会话再把"相关片段"回注到 context。它专为 Claude Code 生态优化,但接口是通用的。相关竞品一下冒出来好几个:Mem0 2.0、Letta、Zep 的 agent-memory 版本等,不过 claude-mem 走的是"本地优先 + TypeScript + 零配置"路线,更接近个人开发者。

为什么这周爆:
- Anthropic 10 月末更新 Claude Code 的 session resume 后,大家意识到"下次继续"这件事被低估了很多年
- 今日 AI 日报里 Anthropic Claude Code 负责人 Cat Wu 离职,引发社区对"Claude Code 独立工具链"是否继续的讨论,claude-mem 这类第三方工具跟涨
- 人们开始习惯"agent 每天干活",而不是"agent 一次 demo",memory 不再是研究议题

同榜的 `max-sixty/worktrunk`(Rust,+524⭐,面向 parallel AI agents 的 Git worktree 管理)配合着读 —— **"一个开发者 + 多个 agent + 多条 worktree + 共享记忆"** 的工作流正式成为今年底的开发者主流姿势。

---

### 🏢 [mattpocock/skills](https://github.com/mattpocock/skills) —— +1,376⭐

**从 ".dotfiles 共享" 进入 ".agents 共享" 的时代:Skill 是新的 preset。**

Matt Pocock(TypeScript 教育者)把自己日常用的 agent "skills"(可被 Claude Code / Cursor / 类 agent 读取的指令集)开源出来,配上 README 讲每个 skill 如何工作。短短数天 31 万+ 星,和 2024 年 dotfiles / awesome-* 系列仓库的爆发曲线一模一样,但语义更重:

- Skill 不只是"喜欢什么字体",它直接影响代码产出的质量和样式
- 开源 Skill 本质上是"把你的工程判断力分发出去",未来可能被嵌入 IDE 市场、plugin marketplace
- 与同榜 `garrytan/gstack`(23 个 Claude Code 角色工具)、`github/spec-kit`(Spec-Driven Development 脚手架)形成同族:**人类个体的方法论,被打包为 agent 可消费的资产**

这是 2026 Q4 最有潜力的"开发者文化"趋势之一 —— "我的工作方式"从视频教程 → 开源 skill 分发,商业价值和技术价值同时在重估。

---

## 生态观察

今天 GitHub trending 的主线,可以浓缩成一句话:**"Agent 落地要工具,工具要配套,配套要开源。"**

- **工具链爆发**:agent-desktop(computer use)、worktrunk(并行 worktree)、claude-mem(跨会话记忆)、pr-agent(自动化代码评审)四条线同时上榜,全部围绕"让 agent 稳定每天干活"展开。
- **厂商下场**:NVIDIA 做知识图谱(auto-ontology)、GitHub 做 spec-kit、Vercel 做 agent-desktop,一线平台开始把 agent 原语做成官方资产 —— 之前这块基本由草根仓库占据,现在"产品化"开始。
- **低资源推理反弹**:kimi-k3-in-c 这种"2.78T 塞进 8GB"的工程奇迹获得关注,反映社区在"GPU 军备竞赛"外主动寻找出口 —— 和今日 HN 热榜 No.2 的 Nvidia 加密固件锁死 Linux 事件,互为因果。
- **"技能"成为新原子**:mattpocock/skills、garrytan/gstack、github/spec-kit 都在用不同形态做同一件事 —— 把人的工程判断打包给 agent 用。"Skill"在 2026 下半年很可能成为继 "Plugin"、"Prompt Template" 之后第三个被广泛接受的 LLM 基元。
- **异常项**:DiscImageStudio(C#,磁盘镜像)本周 +1,792⭐ 但官方没提供描述 —— 要么是某个社群集中引流,要么是某个漏洞 / 破解场景引发的人气爆发,值得明天继续观察。

一句话收尾:**"开发者的日常不是写代码,而是在配一台能替我写代码的机器。"** 今天榜单上的每个项目,都是在为那台机器加一个零件。
