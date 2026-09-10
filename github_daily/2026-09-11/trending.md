# GitHub Trending 日报 · 2026-09-11

## 今日焦点

> **Agent Skills 大爆发 · 3D 地理情报可视化走红 · 大模型路由/引擎两开花 · 中国大厂加入"团队 AI"赛道**
>
> - `ayghri/i-have-adhd` 一款给 coding agent 的"ADHD 输出格式化"技能包，一日暴增 +3,854⭐
> - `bilawalsidhu/gods-eye-view` 浏览器版 3D 间谍卫星模拟器，+1,588⭐
> - `cathrynlavery/diagram-design` 面向 AI 工具的 38 类编辑级 SVG 图示模板，+1,287⭐
> - `Tencent/teamai-cli` 腾讯"Team AI Native"平台正式开源，+837⭐
> - `diegosouzapw/OmniRoute` 支持 352 家 provider、1,200+ 模型的 AI 网关，+591⭐

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) | 给 coding agent 的 ADHD 友好输出技能包 | Python | 38,101 | +3,854 | 2,196 |
| 2 | [bilawalsidhu/gods-eye-view](https://github.com/bilawalsidhu/gods-eye-view) | 浏览器 3D 间谍卫星情报模拟器 | JavaScript | 24,063 | +1,588 | 5,008 |
| 3 | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | 面向 AI 工具的 38 种 SVG 图示模板 | HTML/SVG | 37,684 | +1,287 | 2,389 |
| 4 | [freestylefly/awesome-gpt-image-2](https://github.com/freestylefly/awesome-gpt-image-2) | 530+ GPT Image 提示词模板 | JavaScript | 30,804 | +957 | 2,983 |
| 5 | [liquidslr/system-design-notes](https://github.com/liquidslr/system-design-notes) | 《System Design Interview》学习笔记 | Markdown | 18,730 | +891 | 3,478 |
| 6 | [Tencent/teamai-cli](https://github.com/Tencent/teamai-cli) | 腾讯 Team AI Native 平台 CLI | TypeScript | 3,743 | +837 | 242 |
| 7 | [THU-MAIC/OpenMAIC](https://github.com/THU-MAIC/OpenMAIC) | 多 Agent 互动式课堂平台（清华出品） | TypeScript | 35,252 | +806 | 5,627 |
| 8 | [obra/superpowers](https://github.com/obra/superpowers) | agentic skills 框架与开发方法论 | Shell | 284,670 | +731 | 25,464 |
| 9 | [diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute) | 352 家 provider / 1,200+ 模型的 AI 网关 | TypeScript | 64,183 | +591 | 8,989 |
| 10 | [alsk1992/CloddsBot](https://github.com/alsk1992/CloddsBot) | 跨 1000+ 市场的自主交易 agent | TypeScript | 1,598 | +299 | 253 |
| 11 | [AlexsJones/llmfit](https://github.com/AlexsJones/llmfit) | 面向本地硬件的模型匹配器 | Rust | 35,708 | +247 | 2,262 |
| 12 | [vercel-labs/skills](https://github.com/vercel-labs/skills) | npx 直调的开源 agent skills 工具 | TypeScript | 31,102 | +175 | 2,657 |
| 13 | [JustVugg/colibri](https://github.com/JustVugg/colibri) | 纯 C 实现的前沿 MoE 推理引擎 | C | 27,427 | +130 | 3,005 |
| 14 | [nashsu/llm_wiki](https://github.com/nashsu/llm_wiki) | 桌面版文档→互链知识库工具 | TypeScript | 18,057 | +94 | 2,098 |
| 15 | [armory3d/armorpaint](https://github.com/armory3d/armorpaint) | 开源图形创作工具 | C | 4,391 | +87 | 519 |

---

## 重点项目点评

### 🥇 [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) — 今日榜首，+3,854⭐

**"Agent Skills"生态的第一款出圈神作**

这个仓库名字看起来像玩笑，但是抢下今日榜首。核心是一套写给 coding agent（Claude Code / Cursor / Devin）的 "skill package"，专门重写工具输出格式，让易走神、上下文碎片化的模型能"读进去"—— 短段落、明显视觉锚点、显式 next-step、及时中断长输出。作者把这一套抽象成 Python + JSON schema，可以被 Anthropic Skills、Cursor Rules、Copilot Instructions 等任何 skill 系统直接加载。

它爆红的直接原因是最近一周 Anthropic Fable 5.1 / Cognition SWE-2 / Vercel Labs Skills 集体上线，社区突然意识到"skill 就是新一代 prompt"。这个仓库用一个自嘲的名字，精准命中了"agent 需要被 UI/UX 设计"这一新兴共识——它不是给模型编程，而是给模型"写用户体验文档"。

搭配今天 8 号位 `obra/superpowers`（agentic skills 框架，累计 28 万星，仍在爆增）和 12 号位 `vercel-labs/skills`，可以清楚看到"Skills"正在成为 2026 下半年 GitHub 上最快形成生态位的关键词。

---

### 🥈 [bilawalsidhu/gods-eye-view](https://github.com/bilawalsidhu/gods-eye-view) — +1,588⭐

**从游戏化到"公民 OSINT"：地理情报的开源化**

一个纯浏览器端的 3D 卫星情报模拟器：真实卫星轨道、可视化"当前哪里在被谁看见"、可加载公开的 SAR / 光学影像 tile。项目基于 Cesium / three.js 构建，无需后端就能在本地跑出"当地时间某国海军基地上空的可视卫星窗口"。

它踩中了 2026 年地缘冲突话题下"公民 OSINT"的高涨热度：从乌克兰战场 Twitter 卫星比对，到最近印度、澳洲卫星情报社区，工具门槛正在被 web-first 项目彻底摧毁。作者显然定位为"教育 + 情报科普"，但 issue 区已经出现和 Bellingcat 等组织的合作请求。

这条趋势值得关注：**当军工/情报能力被下沉到"3D 浏览器 demo"，任何一次涉密卫星轨道数据泄露的公开影响都会被指数级放大**。

---

### 🥉 [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) — +1,287⭐

**"AI 也要会画图"：面向大模型的 SVG 素材库**

38 种 editorial 级 SVG 图示模板：类比比较、因果链、金字塔、四象限、流程带、地图叠加等等，全部以 HTML/SVG 呈现，可直接被大模型作为"参考样式"传入 few-shot。这是继"UI 组件库给 LLM 用"（如 shadcn/ui）之后，"设计资产给 LLM 用"的第一波爆款。

它踩到了三件事的合流：一是 Claude Artifact / GPT Canvas / Gemini Deep Research 都开始默认渲染 SVG；二是 Anthropic 官方 skills 文档明确列出了 `artifact-diagramming` 作为一等公民；三是自媒体和演讲者开始意识到"用 AI 出图"过去审美太差，用一套设计过的模板可以立刻提高专业度。

预计接下来几周会出现同类型的 poster、slide、infographic 版本。今天上榜也侧面说明：**"给 AI 用的设计资产"正在形成新的开源赛道**。

---

### 🏅 [Tencent/teamai-cli](https://github.com/Tencent/teamai-cli) — +837⭐

**中国大厂正式加入"团队协作 AI Native"战场**

腾讯把内部使用的 "Team AI Native" 平台开源出 CLI 部分。定位是"多人协作的 agent 工作台"——把 Slack/飞书里的对话、Jira/PingCode 里的任务、Doc 里的文档以 MCP 方式暴露给 agent，作为团队级 memory。此前微软 Copilot Studio、Cursor 的 team workspace、Anthropic 的 Projects 都在做类似的事，腾讯这次直接开源 CLI 是想抢占"国内自建 AI Workspace"的默认位。

值得关注的是与国内头部 IM/文档生态的深度整合能力——如果 Team AI Native 能像 Coding Agent 一样把飞书、企业微信、腾讯文档、蓝鲸智云打通，将成为"没有 OpenAI/Anthropic 的中国团队"的可行开源替代。

---

### 🥇 [diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute) — +591⭐

**LLM Gateway 之战：352 家 provider、1,200+ 模型的开源统一路由**

在 LiteLLM、Portkey、OpenRouter 已经形成"三国鼎立"的赛道上，OmniRoute 这次能挤进榜单的原因是三个：（1）覆盖了 DeepSeek V4.1-Flash、Cognition SWE-2、Gemini 3.8 Flash、Astra 等本周新模型的路由预设；（2）引入 token 压缩层（在路由层就做 cache-aware prompt 重写），据 README 声称可以在长上下文场景省 20-40% token 成本；（3）Docker 镜像开箱即用，60 分钟内可以部署到自己 VPC。

配合今天的 6 号位 `Tencent/teamai-cli` 与 11 号位 `AlexsJones/llmfit`，"**自建 AI 中台**"这条主线在今天的 GitHub 上非常抢眼：企业不想被单一大模型厂锁定，也不想把网关业务外包给 OpenRouter 一家。

---

## 生态观察

今天 GitHub Trending 的三条主线：

- **Skills 是新的 prompt**：`i-have-adhd`、`superpowers`、`vercel-labs/skills` 组合登榜，标志着"如何写 agent skill"取代"如何写 prompt engineering"成为新一代显学。
- **自建 AI 中台被中国大厂+独立开发者共同推进**：`Tencent/teamai-cli`、`OmniRoute`、`llmfit` 显示企业侧对"避免被单模型厂锁定"的诉求已经进入代码层。
- **"给 AI 用的资产库"正在起飞**：`diagram-design`、`awesome-gpt-image-2`、`llm_wiki` 都是"内容/设计/知识库直接为大模型服务"的产物，用户体验开始从"文本 + 代码"扩展到"图示 + 结构化知识"。

同时值得留意的是 `gods-eye-view` 这种"公民 OSINT / 3D 情报可视化"项目——它提示 GitHub 已经不只是软件平台，而正在成为**地缘敏感能力的分发渠道**。
