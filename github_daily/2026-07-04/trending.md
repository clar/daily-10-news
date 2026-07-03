# GitHub Trending 每日热榜 · 2026-07-04

## 今日焦点

> **AI 渗透测试 · Claude Code 生态 · Chrome DevTools MCP · 知识图谱代码助手 · 设计系统开源**
>
> - `usestrix/strix` +2,804⭐ 开源 AI 渗透测试工具，一天暴涨占据榜首
> - `JuliusBrussee/caveman` +2,851⭐ Claude Code 精简通信 Skill，号称降 token 65%
> - `openai/codex-plugin-cc` +629⭐ OpenAI 官方发布 Claude Code 调用 Codex 的插件，敌营互通信号
> - `facebook/astryx` +943⭐ Meta 开源可定制、Agent 就绪的设计系统
> - `safishamsi/graphify` +937⭐ 把代码目录转成可查询知识图谱的 AI 助手

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [usestrix/strix](https://github.com/usestrix/strix) | 开源 AI 渗透测试工具 | Python | 34,514 | +2,804 | 3,540 |
| 2 | [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) | Claude Code 通信精简 Skill，省 65% token | JavaScript | 82,868 | +2,851 | 4,623 |
| 3 | [openai/codex-plugin-cc](https://github.com/openai/codex-plugin-cc) | 在 Claude Code 里调用 Codex 的官方插件 | JavaScript | 23,169 | +629 | 1,402 |
| 4 | [facebook/astryx](https://github.com/facebook/astryx) | 可定制、Agent 就绪的设计系统 | TypeScript | 4,548 | +943 | 266 |
| 5 | [safishamsi/graphify](https://github.com/safishamsi/graphify) | 代码目录 → 知识图谱 → AI 助手 | Python | 77,059 | +937 | 7,632 |
| 6 | [harvard-edge/cs249r_book](https://github.com/harvard-edge/cs249r_book) | 哈佛《ML Systems》公开教材 | Python | 26,132 | +792 | 3,120 |
| 7 | [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) | 给 Coding Agent 用的 Chrome DevTools MCP | TypeScript | 45,464 | +404 | 2,953 |
| 8 | [pytorch/pytorch](https://github.com/pytorch/pytorch) | 深度学习框架 | Python | 101,414 | +290 | 28,248 |
| 9 | [anthropics/claude-code](https://github.com/anthropics/claude-code) | Claude Code 官方代码 Agent | Python | 135,809 | +245 | 21,855 |
| 10 | [rommapp/romm](https://github.com/rommapp/romm) | 自托管 ROM 管理器 | Python | 9,782 | +236 | 471 |
| 11 | [supabase/supabase](https://github.com/supabase/supabase) | Postgres 一体化开发平台 | TypeScript | 105,435 | +145 | 12,968 |
| 12 | [actions/checkout](https://github.com/actions/checkout) | GitHub Actions 官方 checkout | TypeScript | 8,257 | +129 | 2,533 |
| 13 | [elastic/elasticsearch](https://github.com/elastic/elasticsearch) | 分布式搜索引擎 | Java | 77,326 | +77 | 25,923 |
| 14 | [apache/maven](https://github.com/apache/maven) | Java 构建工具 | Java | 5,219 | +53 | 2,901 |
| 15 | [ansible/ansible](https://github.com/ansible/ansible) | IT 自动化平台 | Python | 69,183 | +50 | 24,107 |

---

## 重点项目点评

### 🥇 [usestrix/strix](https://github.com/usestrix/strix) — 今日榜首，+2,804⭐

**AI 渗透测试成为下一个爆款品类**

Strix 是首个"完全开源 + 面向应用漏洞挖掘"的 AI 渗透测试工具，一天涨近 3000 星。核心叙事：把 GPT-5.6 Sol 那一类"网络安全长任务模型"能力普及到中小公司自查。这两天 OpenAI 刚刚发布 GPT-5.6 Sol 网络安全 SOTA、并向政府限量分发，社区侧就立刻长出对应的开源工具链。

Strix 定位不是替代红队，而是"每次上线前先跑一遍 AI 扫"。评论区最热话题是"敢不敢让 AI 直接在生产系统跑 exploit 验证"——目前策略是沙箱重放。可预见的下一步：更多 SaaS 会把 Strix 拼进 CI，把安全"左移"从静态扫描进化到智能体式验证。

---

### 🥈 [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) — +2,851⭐

**Claude Code Skill 生态开始出现"通讯优化层"**

Caveman 是一个 Claude Code Skill：让 Agent 使用极简、去修饰、"穴居人式"的表达，实测节省 65% token。Sonnet 5 上周免费开放，1M 上下文 + 智能体默认，用户对"Agent 交互 token 成本失控"的痛感开始集中爆发——今天 caveman 就是这个痛点的答案。

有趣的是这条路径本质上和 HN 首页那条"代码转图像省 60% Fable 成本"是同源思路——都在挑战主流大模型 API 的定价结构，只是一个是压缩输入格式，另一个是压缩输出风格。当 Claude Code Skill 生态里出现"通讯优化 Skill"，说明 Skill 市场已从"给 Agent 加能力"进化到"给 Agent 省钱"。

---

### 🥉 [openai/codex-plugin-cc](https://github.com/openai/codex-plugin-cc) — +629⭐

**OpenAI 主动出插件让 Claude Code 用户调用 Codex——竞对生态互通信号**

这条挂在 openai 官方账号下的插件，允许 Claude Code 里直接把某类子任务"外派"给 OpenAI Codex 完成、再拿结果回来。表面看是 OpenAI 承认 Claude Code 已经是 Agent 交互事实标准之一，本质上是防御性动作——如果不做这个插件，OpenAI 会彻底失去 Anthropic 用户群里的推理和代码 workflow 入口。

配合本周 GPT-5.6 家族限量预览 + Anthropic 自报营收反超 OpenAI 的产业事件，OpenAI 通过插件形式"寄生"到 Claude Code 是必然选择。可以预见 Google 也会很快跟进类似 Gemini plugin，"Agent 宿主 vs. 模型供应"的分离会逐渐加剧。

---

### 🎯 No.4 · [facebook/astryx](https://github.com/facebook/astryx) — +943⭐

**Meta 开源"Agent 就绪"设计系统，第一次把 UI 组件与 Agent 交互建成一等公民**

Astryx 号称"可定制、Agent 就绪"，第一次把"Agent 可读元数据"作为组件基础属性——Agent 直接理解按钮语义、表单意图、错误状态，而不是靠 DOM 猜测。这与传统 UI 库（Material、Shadcn）设计哲学完全不同。

Meta 选择在 Llama 后续（Muse Spark）主导消费级产品的窗口期开源 Astryx，意在成为"Agent 时代的 UI 底座"。如果 Astryx 普及，Anthropic 和 OpenAI 的 Computer Use / Browser Use 都能直接吃这块红利，属于罕见的"平台方给全体上游送弹药"。

---

### 📊 No.5 · [safishamsi/graphify](https://github.com/safishamsi/graphify) — +937⭐

**代码知识图谱：RAG 之后的下一站？**

Graphify 把代码目录转成可查询的知识图谱，然后让 AI 助手基于图谱做"跨文件推理"。核心问题是 RAG 只能返回相似片段，而代码理解需要"调用链 + 类型继承 + 数据流"这类结构化上下文。Graphify 用 tree-sitter + AST 差分构图 + 增量更新解决这个。

这类项目过去一年出现过很多次（例如 CodeGraph、Sourcegraph Cody 的 Symbol Search 分支），但没有真正跑出。Graphify 起量的时点很微妙——Sonnet 5 上线 1M 上下文，理论上"直接把整仓塞进去"变可行；社区反而更需要一种"精确定位而不是暴力灌"的方案。这暗示业界对纯长上下文路线开始产生疑虑。

---

## 生态观察

**Claude Code 生态占据今日半壁。** Caveman、Codex 插件、Astryx 和 Graphify 全部围绕 Coding Agent；Claude Code 官方仓库本身也保持每日两百多星的稳态增长。可以判断 Coding Agent 已经从"某个大厂产品"演化成"跨厂商共存的开发者事实标准平台"，2026 下半年围绕它的 Skill / 插件 / MCP 供给会继续加速。

**安全 + AI 首次登顶 GitHub Trending。** Strix 一天 +2800 星，与 GPT-5.6 Sol 的 SOTA 位置直接呼应。当年 Metasploit / Nmap 那批工具的 AI 化正在真正发生。

**"省 token"跃升为新品类。** Caveman 说自己节省 65%、xk 那边有代码转图像省 60%——同一天两个"降成本 Hack"上榜。API 定价结构和实际推理成本之间的差异已经足够大，社区开始集体寻找套利工具。这是模型层已经"够用了"、成本层还未成熟的信号。

**制造 / IT 老兵仍在缓慢续命。** Ansible、Elasticsearch、Maven 依然在榜单里保持低位增长——AI 时代的存量运维和搜索底座并没有被替代，反而被越来越多 Agent 反向依赖。这是 GitHub Trending 榜"老树新芽"的常态。
