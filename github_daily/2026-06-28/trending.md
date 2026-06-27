# GitHub Trending 日报 · 2026-06-28

## 今日焦点

> **Claude Code 周边继续席卷 · 隐私通讯杀回榜首 · AI 视觉规范标准化萌芽 · Agent Memory 赛道升温 · 多模态生成"PPT/网站"自动化**
>
> - `simplex-chat/simplex-chat` 隐私通讯杀回 No.1，+1,470⭐，零标识符消息网络重回视野。
> - `google-labs-code/design.md` 视觉规范标准化登场，+1,542⭐，AI 设计交付协议起跑。
> - `xbtlin/ai-berkshire` 用 Claude Code 做巴菲特式价值投资框架，+686⭐，金融 agent 思路出圈。
> - `topoteretes/cognee` Agent 记忆平台 +808⭐，agentic memory 已是事实赛道。
> - `garrytan/gstack` Claude Code 套件大热 +674⭐，"开箱即用 dev 环境"成为新流派。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [simplex-chat/simplex-chat](https://github.com/simplex-chat/simplex-chat) | 全球首个无用户标识符的消息网络 | Haskell | 13,779 | +1,470 | 792 |
| 2 | [google-labs-code/design.md](https://github.com/google-labs-code/design.md) | 视觉设计规范喂给 coding agent 的格式 | TypeScript | 22,293 | +1,542 | 1,781 |
| 3 | [topoteretes/cognee](https://github.com/topoteretes/cognee) | 面向 agent 的开源 AI 记忆平台 | Python | 23,964 | +808 | 2,252 |
| 4 | [JCodesMore/ai-website-cloner-template](https://github.com/JCodesMore/ai-website-cloner-template) | 一条命令克隆任意网站的 AI agent 模板 | TypeScript | 22,080 | +750 | 3,166 |
| 5 | [xbtlin/ai-berkshire](https://github.com/xbtlin/ai-berkshire) | 基于 Claude Code 的价值投资研究框架 | Python | 4,051 | +686 | 573 |
| 6 | [garrytan/gstack](https://github.com/garrytan/gstack) | 一套 23 个工具的 Claude Code 配置 | TypeScript | 117,207 | +674 | 17,414 |
| 7 | [hugohe3/ppt-master](https://github.com/hugohe3/ppt-master) | 文档自动生成可编辑 PPT 的 AI | Python | 33,023 | +589 | 2,812 |
| 8 | [IceWhaleTech/CasaOS](https://github.com/IceWhaleTech/CasaOS) | 简单易用的个人云 OS | Go | 35,760 | +502 | 2,043 |
| 9 | [ripienahr/free-for-dev](https://github.com/ripienahr/free-for-dev) | 开发者免费 SaaS/PaaS/IaaS 列表 | HTML | 124,147 | +459 | 13,081 |
| 10 | [NanmiCoder/MediaCrawler](https://github.com/NanmiCoder/MediaCrawler) | 多平台社交媒体爬虫 | Python | 53,757 | +394 | 11,009 |
| 11 | [commaai/openpilot](https://github.com/commaai/openpilot) | 开源辅助驾驶 OS | Python | 62,055 | +322 | 11,063 |
| 12 | [Anil-matcha/Open-Generative-AI](https://github.com/Anil-matcha/Open-Generative-AI) | 开源 AI 视频生成平台替代品 | JavaScript | 21,355 | +254 | 3,638 |
| 13 | [luongnv89/claude-howto](https://github.com/luongnv89/claude-howto) | 可视化 Claude Code 使用指南 | Python | 38,594 | +138 | 4,646 |
| 14 | [microsoft/PowerToys](https://github.com/microsoft/PowerToys) | Windows 生产力增强工具集 | C | 135,686 | +67 | 8,168 |
| 15 | [dbt-labs/dbt-core](https://github.com/dbt-labs/dbt-core) | 数据转换平台 | Rust | 13,201 | +45 | 2,438 |

---

## 重点项目点评

### 🥇 [google-labs-code/design.md](https://github.com/google-labs-code/design.md) — +1,542⭐

**Google Labs 给 coding agent 立"设计语义"标准**

`design.md` 是 Google Labs 推出的"将视觉品牌/设计规范打包成 agent 可消费格式"的开放规范。它把字体、间距、颜色 token、组件状态、栅格系统等都序列化成 Markdown + JSON 协议，让 Claude Code、Cursor、Codex 这类 coding agent 在生成 UI 时遵守人类设计师立下的视觉系统——而不是每次"随便选个 Tailwind 主题色"。

这个仓库今日暴涨 1,542 星，本质是回答了"AI 写前端但永远跑偏"这个一年来积压的痛点。它和近期的 **MCP for design tools**、**Figma Code Connect** 形成同一条产业链上的不同节点。当 agent 写代码已经接近成熟，"agent 设计协议"成为接下来一年最容易被标准化的层。

它的更深意义：Google 用一个 4KB 规范文件试图占住 agent 设计语义的位置，类似于 OpenAI 在 OpenAPI 占住 tool 描述的位置——这是低成本、高战略价值的开放协议博弈。

---

### 🥈 [simplex-chat/simplex-chat](https://github.com/simplex-chat/simplex-chat) — +1,470⭐

**隐私通讯杀回榜首：零用户标识符不再是小众概念**

SimpleX 自称是"全球首个不依赖任何用户标识符的消息网络"——不需要手机号、邮箱、用户名，仅靠一次性配对建立加密通道。今日新增 1,470 星，背后是社区对"主流即时通讯被监控化"的持续焦虑：WhatsApp / iMessage 后端日志、Signal 元数据上传、Telegram 服务器集中化都让一部分用户转向 SimpleX 这种"完全无主体身份"的方案。

技术上，SimpleX 用 Haskell 实现，强调形式化的密码学协议、单包路由、防关联通讯设计。值得注意的是它的客户端跨平台已经较为成熟（iOS/Android/桌面），用户量虽小但开发者社区高度活跃。今天的星量暴涨与近期一篇被 HN 推上首页的隐私社区分析文章有关。

---

### 🥉 [topoteretes/cognee](https://github.com/topoteretes/cognee) — +808⭐

**Agent Memory 已经从"概念"走到"事实赛道"**

`cognee` 把"AI 记忆"做成可独立部署的服务：支持知识图谱 + 向量索引 + RDB 查询的混合检索，给 LangChain、AutoGen、Claude SDK 等 agent 框架提供"长期记忆"层。它今日 +808 星，本身就是 Agentic 应用层最直观的需求信号。

过去一年大家都在喊 "agent + memory"，但真正能拿来即插即用、跑通的开源项目寥寥。cognee 的设计哲学接近"为 Agent 而生的 Postgres"——而不是仅仅做一个 RAG 包装。配合 Claude Mythos / GPT-5.6 长上下文窗口，agent memory 不再是"上下文不足的补丁"，而是结构化记忆与短上下文协同的策略层。

---

### 🏅 [xbtlin/ai-berkshire](https://github.com/xbtlin/ai-berkshire) — +686⭐

**Claude Code 跨界做"巴菲特式投研框架"**

`ai-berkshire` 用 Claude Code 编排出一整套"价值投资研究流水线"——从 10-K 抓取、护城河分析、ROIC 测算、估值模型，到行业对比。这种"模型 + 工具链 + prompt 模板"的组合让 Claude Code 第一次明确以"领域 agent"形态出圈到金融垂类。

它代表了 Claude Code 的一个新流派：**领域工程化 prompt 工程包**——不再是单 prompt，而是一整套 .claude/skills/ 配置 + 工具 + 报告模板。可以预见，未来几周会出现 ai-medical-research、ai-legal-due-diligence、ai-mna 等同类项目。

---

### 🎖️ [garrytan/gstack](https://github.com/garrytan/gstack) — +674⭐

**"开箱即用的 Claude Code 环境"成为新的开发者品味**

YC 总裁 Garry Tan 维护的 `gstack` 把 23 个最爱的工具（包含 Claude Code、ripgrep、fzf、starship、Bun 等）打包成一键脚本——核心思路是"用我的工程师品味替代你的工程师品味"。它今日 +674 星，是这一年"dev 环境策展化"潮流的代表：从 dotfiles 到 starter pack，再到现在的 LLM 优化 dev stack。

这种 stack 反映了一种新的工作流共识——AI 工具不是某一个产品，而是一组"在 shell 里彼此打配合"的小工具。`gstack` 实际上把 Claude Code 当成了 shell 一等公民，配合 fzf/ripgrep/jq 的传统 Unix 哲学，呈现出与"Cursor 全 IDE 化"完全相反的另一条路径。

---

## 生态观察

今天的 trending 高度集中在三条主线：

- **Claude Code 二级生态成熟化**：`gstack`、`ai-berkshire`、`claude-howto` 同框出现，说明 Claude Code 已经从"工具"演化为"平台"——开发者开始围绕它构筑垂类工作流、starter pack 与教学资源。
- **agent 基础设施进入"零件化"时代**：`design.md`（视觉设计协议）、`cognee`（记忆）、`ai-website-cloner-template`（克隆 agent）三条线分别瞄准 agent 工作流的不同层。开源世界正在为 agent 框架补齐"以前的浏览器扩展生态"。
- **隐私 / 自托管反潮流持续**：SimpleX 与 CasaOS 同时上榜，说明 2026 年开发者对集中化 SaaS 的不信任不仅没消退，反而随着 AI 模型供应商集中度加剧而更强烈。

冷却的是：纯生成式 AI 视频/图像项目今天明显被压（`Open-Generative-AI` 只勉强进榜尾部），这与 5 月份生成式视频热潮形成对比——开发者关注点正在从"生成"回到"工程化部署"。
