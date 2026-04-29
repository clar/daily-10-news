# AI 行业日报 · 2026-04-30

## 今日焦点

> **五角大楼 Gemini 上岗 · Claude Mythos vs Opus 4.7 双轨化 · DeepSeek V4 价格战延烧 · Cursor 500 亿美金估值 · 微软-OpenAI 协议重谈落地**
>
> - **五角大楼正式接入 Google Gemini**：用于机密网络的 AI 能力，OpenAI 之后第二家；Anthropic 因坚持安全限制仍在打官司
> - **Claude Opus 4.7 GA**：定位"最强通用可用模型"，Mythos Preview 走前沿/Opus 走稳定的双轨开始清晰
> - **DeepSeek V4 Pro/Flash 上线**：1.6 万亿参数，深度绑定华为芯片，价格再砍一刀
> - **Cursor 估值飙到 500 亿美金**：拟融 20 亿美元，AI 编程工具赛道估值天花板再被掀
> - **微软-OpenAI 协议重谈正式生效**：4 月 27 日两家共同官宣"下一阶段合作"，结构性松绑

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | 五角大楼与 Google 签约，Gemini 进入机密网络 | NBC News / Manila Times | ⭐⭐⭐⭐⭐ |
| 2 | Anthropic Claude Opus 4.7 正式 GA，软件工程能力大幅提升 | Anthropic / CNBC | ⭐⭐⭐⭐⭐ |
| 3 | DeepSeek V4 Pro / V4 Flash 发布，1.6T 参数 + 华为芯片绑定 | Bloomberg / Fortune | ⭐⭐⭐⭐⭐ |
| 4 | Cursor 在谈 20 亿美金 D 轮，估值 500 亿美金 | CNBC | ⭐⭐⭐⭐⭐ |
| 5 | 微软-OpenAI 重谈协议官宣"下一阶段合作"，结构性松绑 | Microsoft Blog | ⭐⭐⭐⭐⭐ |
| 6 | Google 宣布最高 400 亿美金投资 Anthropic，350 亿估值起步 | TechCrunch / CNBC | ⭐⭐⭐⭐⭐ |
| 7 | OpenAI 完成 1220 亿美金巨额融资，史上最大单笔 | OpenAI 官方 | ⭐⭐⭐⭐⭐ |
| 8 | OpenAI 推出 Workspace Agents，正式取代企业版 Custom GPTs | TechCrunch | ⭐⭐⭐⭐ |
| 9 | OpenAI GPT-5.5 发布：SWE-bench 88.7% / 1200 万 token 上下文 | TechCrunch | ⭐⭐⭐⭐ |
| 10 | DeepMind 前研究员创业 Ineffable Intelligence，11 亿美金种子轮 | CNBC | ⭐⭐⭐⭐ |
| 11 | Cognition AI 在谈新一轮，估值翻倍至 250 亿美金 | Bloomberg | ⭐⭐⭐⭐ |
| 12 | Q1 2026 全球 VC 融资 2970 亿美金，AI 占 81% | Crunchbase | ⭐⭐⭐⭐ |
| 13 | 欧盟 AI Act 高风险条款 8 月 2 日落地，企业进入合规倒计时 | EU Commission | ⭐⭐⭐⭐ |
| 14 | Anthropic 内部实验：69 人 1 周用 Claude Agent 成交 186 单 | Anthropic | ⭐⭐⭐ |
| 15 | Avoca 一周内连融 1.25 亿美金，估值破 10 亿 | TechCrunch | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · 五角大楼正式接入 Google Gemini，Anthropic 因安全条款继续掉队

**[NBC News](https://www.nbcnews.com/tech/tech-news/pentagon-inks-deal-google-ai-services-rcna342661)** · **[Manila Times](https://www.manilatimes.net/2026/04/29/world/pentagon-makes-deal-to-expand-use-of-google-ai-reports/2331857)**

五角大楼与 Google 签下协议，将 Gemini 模型部署到 DoD 的机密网络上。在这之前 OpenAI 已先一步进了同样的供应商池子，意味着美国国防部这条最大单的 AI 合同从"OpenAI 独占"变成"OpenAI + Google 双供"格局。值得注意的对照是 Anthropic：因坚持要求对其模型的国防/情报场景使用施加更严格的"safeguards"条款，Anthropic 与五角大楼仍在打官司，至今没拿到合同。

为什么这件事是今天最高规格的新闻？因为它把过去一年关于"AI 安全派 vs 部署派"的张力，第一次以政府采购最直接的形式定价——选择更强 safety 立场的 Anthropic 在国防赛道上正在付出真金白银的市场份额代价，而 Google 凭借更灵活的部署条款拿走了过去 OpenAI 独占的盘子。这也解释了为什么 Anthropic 今年同时在拼命拉 Google（最高 400 亿美金）和 Amazon（追加 50 亿）的投资——商业客户的天花板必须撑得起政府客户的"留白"。

**点评：** 国防是 AI 商业化最厚的护城河之一，今天起 Google 与 OpenAI 正式分掉这条河，Anthropic 暂时被晾在岸上。安全立场的代价已经从抽象变得很具体。

---

### 🚀 No.2 · Anthropic 释出 Claude Opus 4.7：双轨产品线就此成型

**[Anthropic 官方](https://www.anthropic.com/news/claude-opus-4-7)** · **[CNBC](https://www.cnbc.com/2026/04/16/anthropic-claude-opus-4-7-model-mythos.html)**

Claude Opus 4.7 现已 GA，定位是"在通用能力上最强的可用版本"。官方承认它在广义任务上不如 Claude Mythos Preview，但在软件工程、指令跟随、真实任务完成度上做了显著优化——本周 GitHub trending 榜上各种 Claude Skills/Coding Harness 的爆发，背后正是 Opus 4.7 把 SWE 类任务能力又拔高一档之后的连锁反应。

更值得拆开看的是 Anthropic 的产品线策略：Mythos Preview 走"狂飙模型 / 全能但可能踩雷"，Opus 4.7 走"通用、安全、企业可签合约"。这种"前沿研究线 + 商用稳定线"的双轨，明显是在抄 OpenAI（GPT-5.5 / o-series）的产品架构作业，但更进了一步——商用线被明确标注"less broadly capable"，等于先帮企业客户管理预期。这对一个曾经只有"一个最强 Claude"的 Anthropic 来说，是产品成熟度的一次硬升级。

**点评：** 模型公司开始公开承认"我们最强的版本并不一定适合你买"，是一个比模型本身更关键的拐点——AI 进入"配菜单时代"。

---

### 🌶️ No.3 · DeepSeek V4 Pro / V4 Flash：1.6T 参数 + 华为芯片，价格屠刀再挥一次

**[Bloomberg](https://www.bloomberg.com/news/articles/2026-04-24/deepseek-unveils-newest-flagship-a-year-after-ai-breakthrough)** · **[Fortune](https://fortune.com/2026/04/24/deepseek-v4-ai-model-price-performance-china-open-source/)**

DeepSeek 在去年 V3 一鸣惊人之后，本月发布 V4：1.6 万亿参数，分 Pro / Flash 两个档，并强调与华为芯片的深度集成。Fortune 拿到的对比数据显示，V4 在编码 benchmark 上对标 GPT-5.4 / Claude Opus 4.6 / Gemini 3.1 Pro 不落下风，而价格继续用"碾压式低价"打——这是 DeepSeek 一贯的杀招。

V4 真正的战略意义不是模型本身，而是**算力供应链的中美彻底分叉**。DeepSeek 选择把旗舰模型与华为昇腾深度绑定，意味着中国 AI 头部公司开始正式跳出 H100/H200 这条线。在 Nvidia 4 月 24 日刚刚冲上 5 万亿美金市值的同一周，DeepSeek 用"非 Nvidia 路径"完成顶级模型迭代，这是过去三年第一次出现"不靠 Nvidia 也能跑到前沿"的有力反证。对企业客户而言，影响也是直接的：开源 + 低价 + 自主可控算力 = 中国 AI 国产替代的版本号正式从 v3 升到 v4。

**点评：** Nvidia 的市值故事和 DeepSeek 的开源故事今天同时被验证——两个互相矛盾的叙事开始并行存在，中长期看 DeepSeek 的故事更危险。

---

### 💰 No.4 · Cursor 拟融 20 亿美元，估值 500 亿美元——AI 编码已是头等赛道

**[CNBC](https://www.cnbc.com/2026/04/19/cursor-ai-2-billion-funding-round.html)**

Cursor 在谈一轮 20 亿美金的融资，估值超过 500 亿美金。一年多前它的估值还只是十位数级别。同期 Cognition AI（Devin 的母公司）传出在谈估值 250 亿美金的新一轮——AI 编码这个赛道现在的估值天花板，已经接近"应用层小型 OpenAI"。

为什么市场愿意给 AI 编码工具这么高溢价？三个原因叠加：第一，开发者付费意愿被 GitHub Copilot 验证过；第二，Coding Agent 是目前 LLM 能力提升带来 ARR 增速最猛的场景（Anthropic Claude Code 一年内 ARR 可观）；第三，Cursor 这类工具同时占据 IDE 和 agent harness 两个入口，形成了少有的"应用层壁垒"。但风险也明显——这个赛道里的玩家几乎全部依赖几家底层模型，护城河更多在 UI/工作流而不是模型本身。

**点评：** AI 编程是 LLM 应用层目前唯一被资本市场全票通过的赛道，Cursor 的 500 亿美金估值是它的天花板验证，不是顶。

---

### 🤝 No.5 · 微软-OpenAI 重谈协议正式落地：从"独家算力捆绑"走向"灵活、明确"

**[Microsoft Official Blog](https://blogs.microsoft.com/blog/2026/04/27/the-next-phase-of-the-microsoft-openai-partnership/)**

4 月 27 日微软发布官方博客《下一阶段微软-OpenAI 合作》，正式宣布两家修订协议，关键词是 "flexibility, certainty"。结合此前传出的 OpenAI 最新 1220 亿美金融资，可以推断这次重谈背后的本质是：OpenAI 拿到了独立融资和算力扩张能力，不再需要把所有筹码绑在 Azure 一家身上；而微软也需要重新定义自己在 AI 时代相对独立的位置（Copilot 自研 + 多模型路线）。

这件事的链式反应已经在发生：今天上榜的 Google–Anthropic 400 亿美金投资其实是一次镜像——巨头投 AI 实验室、但允许实验室拥抱多云。"AI 实验室一对一 lock-in 给某家云厂"的旧版本游戏在 2026 年 4 月正式翻篇，所有 AI 实验室都在做"多云 + 多投资方"的重组。最直接的结果是企业客户：之前用 Azure OpenAI 的客户未来在 Anthropic、xAI、自研模型上的可选性会显著增加。

**点评：** 微软-OpenAI 的"婚约"变成"商业合伙"，这是 AI 巨头时代最重要的一次结构性松绑。

---

## 行业观察

今天的信号面非常密集，但有一根主线非常清楚——**AI 行业正在进入"再分配 + 双轨化"阶段**。

- **再分配**：政府订单（五角大楼 → Google）、巨头资本（Google → Anthropic、Amazon → Anthropic）、模型公司算力供应（OpenAI 跳出 Azure 独占、DeepSeek 跳出 Nvidia 独占）三条线同时在重新洗牌。过去两年那种"AI = OpenAI + Microsoft + Nvidia 三联体"的简单叙事彻底瓦解。
- **双轨化**：Anthropic Mythos vs Opus 4.7、OpenAI o-series vs GPT 主线、DeepSeek Pro vs Flash——所有头部模型公司都在正式确立"研究前沿线 + 商用稳定线"两条产品线。这意味着企业采购侧第一次有"选哪条线"的抽象问题，而不再是"买不买 GPT-4"那种简单决策。

垂直观察：欧盟 AI Act 高风险条款 8 月 2 日落地的倒计时已经开始，今天距离 deadline 还有 95 天。结合 Cursor / Cognition / Avoca 一周三家 AI 应用层公司刷估值的速度，可以预期 5-7 月会出现一波"合规前的最后一冲"——估值高峰大概率出现在 8 月之前。

如果今天只能记一件事：**美国政府已经开始用合同投票"AI 安全派"和"AI 部署派"——而部署派今天又赢了一次。**

Sources:
- [NBC News · Pentagon-Google deal](https://www.nbcnews.com/tech/tech-news/pentagon-inks-deal-google-ai-services-rcna342661)
- [Anthropic · Claude Opus 4.7](https://www.anthropic.com/news/claude-opus-4-7)
- [CNBC · Anthropic Opus 4.7 vs Mythos](https://www.cnbc.com/2026/04/16/anthropic-claude-opus-4-7-model-mythos.html)
- [Bloomberg · DeepSeek V4](https://www.bloomberg.com/news/articles/2026-04-24/deepseek-unveils-newest-flagship-a-year-after-ai-breakthrough)
- [Fortune · DeepSeek V4 价格](https://fortune.com/2026/04/24/deepseek-v4-ai-model-price-performance-china-open-source/)
- [CNBC · Cursor 500 亿估值](https://www.cnbc.com/2026/04/19/cursor-ai-2-billion-funding-round.html)
- [Microsoft Blog · 下一阶段微软-OpenAI 合作](https://blogs.microsoft.com/blog/2026/04/27/the-next-phase-of-the-microsoft-openai-partnership/)
- [TechCrunch · Google 投 Anthropic 400 亿](https://techcrunch.com/2026/04/24/google-to-invest-up-to-40b-in-anthropic-in-cash-and-compute/)
- [OpenAI · 1220 亿融资](https://openai.com/index/accelerating-the-next-phase-ai/)
- [TechCrunch · GPT-5.5 发布](https://techcrunch.com/2026/04/23/openai-chatgpt-gpt-5-5-ai-model-superapp/)
- [Crunchbase · Q1 2026 VC 数据](https://news.crunchbase.com/venture/record-breaking-funding-ai-global-q1-2026/)
- [CNBC · Ineffable Intelligence 11 亿种子轮](https://www.cnbc.com/2026/04/27/deepmind-ineffable-intelligence-record-seed-funding-nvidia-google.html)
- [EU 数字战略 · AI Act](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)
