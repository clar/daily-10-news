# GitHub Trending 日报 · 2026-09-13

## 今日焦点

> **卫星情报可视化爆红 · AI 销售 CRM 蹿升 · System Prompt 泄露站长期霸榜 · Agent + Git worktree · 加密预测市场自动化交易**
>
> - `bilawalsidhu/gods-eye-view` 单日 +2,265⭐，浏览器里的"上帝视角"卫星仿真器登顶。
> - `melgarafael/DeskcommCRM` +505⭐，开源 AI 销售平台，主打 WhatsApp + 自建 CRM。
> - `asgeirtj/system_prompts_leaks` 长期霸榜（65k⭐），今日 +357⭐，前沿模型 System Prompt 泄露合集。
> - `alsk1992/CloddsBot` +377⭐，覆盖 1000+ 加密与预测市场的自动交易 Agent。
> - `max-sixty/worktrunk` +137⭐，为并行 AI Agent 优化的 Git worktree 管理 CLI，Rust 生态。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [bilawalsidhu/gods-eye-view](https://github.com/bilawalsidhu/gods-eye-view) | 浏览器版真实数据卫星仿真器 | JavaScript | 29,727 | +2,265 | 5,996 |
| 2 | [melgarafael/DeskcommCRM](https://github.com/melgarafael/DeskcommCRM) | 开源 AI 销售平台 / WhatsApp 集成 | TypeScript | 1,775 | +505 | 548 |
| 3 | [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) | Claude/ChatGPT/Gemini 系统提示词泄露合集 | JavaScript | 65,362 | +357 | 10,733 |
| 4 | [nab138/iloader](https://github.com/nab138/iloader) | 用户友好的 iOS 侧载工具 | TypeScript | 3,066 | +209 | 209 |
| 5 | [Flowseal/zapret-discord-youtube](https://github.com/Flowseal/zapret-discord-youtube) | 网络访问工具（Discord/YT） | Batchfile | 33,201 | +52 | 2,540 |
| 6 | [jihe520/MathModelAgent](https://github.com/jihe520/MathModelAgent) | 数学建模自动化 Agent，生成研究论文 | Python | 5,113 | +264 | 401 |
| 7 | [Sonarr/Sonarr](https://github.com/Sonarr/Sonarr) | 智能 PVR 追剧下载器 | C# | 15,908 | +228 | 1,952 |
| 8 | [alsk1992/CloddsBot](https://github.com/alsk1992/CloddsBot) | 覆盖 1000+ 加密与预测市场的自动交易 Agent | TypeScript | 2,475 | +377 | 310 |
| 9 | [yuliskov/SmartTube](https://github.com/yuliskov/SmartTube) | Android TV 高级 YouTube 客户端 | Java | 33,199 | +160 | 2,013 |
| 10 | [Shubhamsaboo/awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) | 100+ AI Agent 与 RAG 应用合集 | Python | 137,594 | +237 | 20,233 |
| 11 | [p1neappleXpress/OpenFlux](https://github.com/p1neappleXpress/OpenFlux) | 可插拔传输层的 TCP 隧道网络栈研究工具 | Go | 1,389 | +355 | 103 |
| 12 | [armory3d/armorpaint](https://github.com/armory3d/armorpaint) | PBR 材质绘制软件 | C | 4,900 | +237 | 547 |
| 13 | [SnailSploit/Claude-Red](https://github.com/SnailSploit/Claude-Red) | AI 辅助渗透测试进攻性技能库 | Python | 3,567 | +99 | 549 |
| 14 | [multimodal-art-projection/YuE](https://github.com/multimodal-art-projection/YuE) | 具备符号规划与 Agentic 编辑的音乐生成平台 | Python | 7,257 | +193 | 818 |
| 15 | [max-sixty/worktrunk](https://github.com/max-sixty/worktrunk) | 面向并行 AI Agent 的 Git worktree 管理 CLI | Rust | 7,207 | +137 | 255 |

---

## 重点项目点评

### 🥇 [bilawalsidhu/gods-eye-view](https://github.com/bilawalsidhu/gods-eye-view) — 今日榜首，+2,265⭐

**"浏览器里的间谍卫星"：把公开地理数据可视化到极致**

一款完全跑在浏览器端的"卫星仿真器"，作者拿真实公开数据（NOAA、ESA、Sentinel、AIS 船只轨迹、ADS-B 航班）拼出一层交互式全景视角，UI 直接模拟情报机构常见的战术界面。它并不发明新数据源，胜在把散乱的公共 API 汇成一个直观、随手可用的工程作品——单日暴涨 2,265 星，反映的是"公开数据 + 展示层"依然是 GitHub 最容易破圈的组合。

它的走红也踩到了两条时事线：一是加沙、乌克兰战事让公众对卫星情报的兴趣长期居高；二是本周 Anthropic 与 Nvidia 的 IPO 循环金融讨论让"open-source 情报（OSINT）"话题重新被讨论。作者顺势把 README 写成了"我如何把 Sentinel API 拉进 WebGL"的教程，二次传播效率极高。

对于早期开发者而言，这是一份可复用的"数据+可视化"模板：地理层、时序层、匿名船只/航班层的解耦方式，可直接借鉴到任何数据可视化项目中。

---

### 🥈 [melgarafael/DeskcommCRM](https://github.com/melgarafael/DeskcommCRM) — +505⭐

**AI CRM 的"自建替代"叙事又赢了一次**

DeskcommCRM 主打三个卖点：本地部署、原生 AI Agent、原生 WhatsApp 集成。它瞄准的是 Twilio + HubSpot + OpenAI 组合的中小企业客户——这类企业苦于 SaaS 订阅堆叠已久，一个把销售 pipeline、消息通道、AI 打通的自建方案有天然吸引力。

它的另一个关键节点是"WhatsApp 一等公民"。全球中小企业 CRM 场景 60% 以上的沟通已发生在 WhatsApp，但 Meta 的 WhatsApp Business API 定价高且难用，任何能把这条通道原生自建的项目都会在拉美、东南亚、中东获得快速的自发传播——这也是它两周内从冷启动跳到 1,775 星的原因。

从代码结构看，DeskcommCRM 在 Agent 侧做了 "Handoff-to-Human" 显式接口，这是它比其他"AI 销售 SaaS"的关键工程差异——把托管性 Agent 与人工客服的接管节点写成一等公民，避免了传统 LLM 客服"死循环"的问题。

---

### 🥉 [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) — +357⭐（累计 65k）

**"System Prompt 圣经"的长期霸榜说明什么？**

这个仓库已经稳居 GitHub trending 数月，累计 65,362 星、10,733 fork。核心内容是从主流 AI 平台（Claude、ChatGPT、Gemini、Copilot 等）逆向或诱导得到的 System Prompt 全文，按厂商、版本、语种归类。每次一个新前沿模型发布，就会出现一次爆发式增长——例如上周 GPT-6 Astra 发布后仓库出现 GPT-6-astra.md 提交，本周 Anthropic Fable 5.1 更新后又新增了对应文件。

这个仓库长期高涨反映的是 AI 应用开发的两个真相：一是自建 Agent 的开发者事实上把它当"事实工业标准"参考——每个厂商都在悄悄抄同行的提示词模式；二是"System Prompt 泄露"的伦理边界在 GitHub 社区已经默认让位于工程价值。Anthropic 与 OpenAI 曾多次警告过此类仓库，但至今没有 DMCA takedown 落地——因为技术上很难主张 System Prompt 是"作品"级别的独创性。

对 Prompt 工程师而言，这是研究前沿实验室"对话行为规范"最直接的窗口；对模型厂商而言，这是不得不接受的公开审计——某种程度上加速了 Prompt 的规范化。

---

### 🚀 [alsk1992/CloddsBot](https://github.com/alsk1992/CloddsBot) — +377⭐

**Polymarket 时代的 Agent 交易范式**

CloddsBot 声称覆盖 1000+ 个加密和预测市场（Polymarket、Kalshi、Manifold、Drift、Hyperliquid 等），把 LLM 作为决策核心，配合链上事件驱动的下注系统。它踩中的是 2026 年最热的两条曲线：一是 Polymarket 在美国大选后的用户量高位；二是 AI Agent + 链上支付/托管的组合终于走到 "钱包+签名+多市场"可用形态。

技术上它做了两件工程价值最高的事：一是 uniform market interface，把 CEX/DEX/预测市场统一成同一 Trade API；二是 shared context memory，让 Agent 能跨市场保留立场（例如把选举概率、加密价格、股票价格的信号交叉引用）。这套架构预示着"Agent 交易平台"层可能从纯量化 quant 生态进入 Retail Agent 生态。

需要提醒：这类项目的历史违约率极高，README 中列出的"多市场夏普比"缺少滚动窗口数据，读者不要把 GitHub 星数当作策略有效性证据。

---

### 🚀 [max-sixty/worktrunk](https://github.com/max-sixty/worktrunk) — +137⭐

**为"多 Agent 并行编码"设计的工具首次进入 trending**

worktrunk 用 Rust 写就，本质是 `git worktree` 的开发者体验封装，专门针对"同一仓库里同时跑多个 AI Agent 分支"的场景做了三件事：批量创建/回收 worktree、按 Agent ID 隔离 branch、自动同步远程与自动 rebase。它把"多个 Claude/Codex 会话在同一代码库里并行开工"这类新兴工作流的痛点，用一个几百行 CLI 解决了。

worktrunk 的走红反映了 2026 年下半年一个隐蔽但重要的趋势：单 Agent 已经不是主流，主流是"5-10 个 Agent 分头做工"。Codex、Claude Code、Cursor Agent Mode 都在做类似的分裂-并合模式，但工具链层长期没有统一约定——`worktrunk` 是第一个把命名、状态、清理都规范化的开源尝试。

从生态位来看，它未来大概率不会是被 Anthropic/OpenAI 自己收敛掉的层——因为多 Agent 并行需要工具中立、能同时对接 Codex/Claude/Cursor，而这恰恰是社区项目更适合承担的位置。

---

## 生态观察

**AI Agent 应用层正在从"个人助手"分裂出两条并行路径。** 一条是"细分工作流"（DeskcommCRM 面向销售、MathModelAgent 面向学术、CloddsBot 面向预测市场），把 Agent 深度绑定单一垂直行业；另一条是"多 Agent 基础设施"（worktrunk 面向 git 并行、awesome-llm-apps 面向组合复用）。这两条路径同时上榜，说明社区已经不再迷信"通用 Agent"，转而分层做 vertical 和 infra。

**OSINT 与地理数据可视化在 2026 年下半年重新变成流量入口。** gods-eye-view 的爆红不是孤例，本月已经有多个 satellite / AIS / ADS-B 类项目登过 trending。背后是三件事叠加：地缘政治持续紧张、公开数据 API 更成熟、WebGPU/WebGL 门槛显著降低。

**"逆向 + 泄露 + 合集"类项目依然是最稳定的长期流量池。** system_prompts_leaks 与 Claude-Red 都属于此类；它们的合规风险始终存在，但 GitHub 平台的 takedown 门槛远高于社区收藏价值，短期内会继续存在。

**一句话总结：** 今日榜单没有出现 SOTA 级新模型或新框架，热度均分给了"垂直 Agent 应用 + 数据可视化 + 逆向合集"三个稳定池——这在前沿实验室大动作频出的一周里，恰恰是 GitHub 社区选择"避开巨头正面竞争、做剩下的一切"的清晰写照。
