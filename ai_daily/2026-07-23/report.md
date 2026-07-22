# AI 日报 · 2026-07-23

## 今日焦点

> **闭源加速分化 · 中国开源三巨头逼门 · 巨头借并购抢机器人赛道 · 监管临界 · 芯片超级周期继续**
>
> - **Google 一次连发三款 Gemini 3.6/3.5 Flash，Pro 旗舰再度跳票** — Flash 定价 $1.5 / $7.5，知识截止推进到 2026 年 3 月；同时官宣 Gemini 4 已进入预训练。
> - **Anthropic 收购 Physical Intelligence 传闻发酵** — π0.5 模型广泛使用的机器人独角兽估值一度 $110 亿，OpenAI 是其股东，两大巨头 IPO 前抢人抢技术白热化。
> - **Kimi K3（2.8T 参数）7 月 27 日全权重开源，DeepSeek V4 稳定版 7 月 24 日** — 中国开源阵营将连续两周向 Flash 级闭源模型发起价格 + 能力双重进攻。
> - **Q2 AI 游说支出全线创新高，Anthropic +26%、OpenAI +18%** — 白宫据报即将发布前沿模型自愿标准，EU AI Act 8 月 2 日高风险条款截止日进入倒计时。
> - **AMD Q1 数据中心 $58 亿 (+57% YoY)、Q2 指引 $112 亿** — OpenAI + Meta 6GW 大单落地，Nvidia 数据中心 $752 亿 (+92% YoY) 依旧压制，AI 芯片超级周期未见拐点。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Google 发布 Gemini 3.6 Flash / 3.5 Flash-Lite / 3.5 Flash Cyber，Pro 继续跳票 | BuildFastWithAI | ⭐⭐⭐⭐⭐ |
| 2 | Anthropic 洽购 Physical Intelligence 传闻发酵，OpenAI 作为股东被卷入 | TechCrunch / The Information | ⭐⭐⭐⭐⭐ |
| 3 | Moonshot Kimi K3（2.8T 参数）承诺 7 月 27 日全权重开源，改良 MIT 协议 | VentureBeat | ⭐⭐⭐⭐⭐ |
| 4 | DeepSeek V4 稳定版定档 7 月 24 日，直接对标 Kimi K3 与 Flash 系列 | AIbase | ⭐⭐⭐⭐ |
| 5 | Q2 AI 游说支出：Meta $5.99M、Anthropic $1.97M(+26%)、OpenAI $1.2M(+18%) | Public Filings | ⭐⭐⭐⭐ |
| 6 | 白宫据 FT 报道即将出台前沿模型自愿发布标准 | Financial Times | ⭐⭐⭐⭐ |
| 7 | AMD Q1 数据中心 $58 亿、股价盘后 +14%，Q2 指引 $112 亿 | Tech Insider | ⭐⭐⭐⭐ |
| 8 | Florida 州检察长起诉 OpenAI，首个州级 AG 直接起诉案 | For The People | ⭐⭐⭐⭐ |
| 9 | Andrej Karpathy 加入 Anthropic，回归 R&D | ThursdAI | ⭐⭐⭐⭐ |
| 10 | Anthropic Claude Cowork 支持屏幕录制→技能，绕过传统 prompt | Anthropic | ⭐⭐⭐ |
| 11 | Meta 声称自家审核 AI 错误率比人工低 13%、多识别 10% 违规 | Meta | ⭐⭐⭐ |
| 12 | Substack 集成 Pangram AI 检测（100 词以上文本） | Substack | ⭐⭐⭐ |
| 13 | Block 开源 Buzz：基于 Nostr 的 Agent 协作工作台 | Block | ⭐⭐⭐ |
| 14 | Gemini 3.5 Flash Cyber 加入 Anthropic Mythos 阵营，向政府/受信合作方限售 | Google | ⭐⭐⭐ |
| 15 | ICML 2026 "Selective Activation Sparsity" 使小模型追平 3x 大模型 | ICML | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Google 三连发 Flash，Pro 再跳票 —— "旗舰失焦，中端救场"

**[BuildFastWithAI · Google 一次上线三款 Gemini 模型](https://www.buildfastwithai.com/blogs/ai-news-today-july-22-2026)**

7 月 21 日 Google DeepMind 一次性上架 Gemini 3.6 Flash、3.5 Flash-Lite 与专为政企定制的 3.5 Flash Cyber，同时官宣 Gemini 4 已进入预训练——但 Pro 旗舰再一次没有出现在发布清单里，据内部测试其在编码和复杂推理上仍落后 Sonnet 5 与 GPT-5.6 Sol。3.6 Flash 定价 $1.5 / $7.5（每 M input / output token），比前代减少 17% 输出 token 消耗，知识截止时间从 2025 年 1 月推进到 2026 年 3 月，直接压向 Kimi K3、DeepSeek V4 的价格区间。

Pro 缺席背后是一个更结构性的问题：Google 已把资源从"打旗舰刷榜"转向"打价格战 + 拉高知识时效"。Flash 系列以 Artificial Analysis Index 上的成本/性能比作为主线，反而让 Google 在企业侧的存在感更强。这条路径与 OpenAI 的 Luna/Terra/Sol 三层策略、Anthropic 的 Fable/Opus/Sonnet 分层策略趋同，都是承认"单一旗舰赢家通吃"已成过去。

值得关注的是 3.5 Flash Cyber 的销售策略：加入 Anthropic Mythos 阵营，只对政府和受信合作伙伴出售。行业开始在**没有监管强制**的前提下，自发对双用途 AI 能力实行访问限制——这是 2026 下半年最值得盯的一条主线。

**点评：** Google 已经放弃"每一代都要在旗舰上打赢"的执念，Flash 才是它的护城河；Pro 再跳一次票，说明 Gemini 4 才是它真正要押的赌注。

---

### 🚀 No.2 · Anthropic × Physical Intelligence：并购传闻背后的机器人抢购潮

**[TechCrunch · Anthropic-Physical Intelligence 传闻搅动 AI Twitter](https://techcrunch.com/2026/07/21/the-anthropic-physical-intelligence-rumor-roiling-ai-twitter/)**

7 月 21 日科技博客作者 Robert Scoble 在 X 上放出"Anthropic 收购 Physical Intelligence"传闻，PI CEO Karol Hausman 在 Slack 用一张 Office GIF 表示否认，但 The Information 随后确认春季确有洽购谈判，只是细节可能有出入。Physical Intelligence 已融资超 $10 亿，最近一轮估值 $110 亿，其 π0.5 模型是学术圈机器人研究的事实标准之一——OpenAI 也在其股东名单上。

真正引爆讨论的是**IPO 前的抢购逻辑**：Anthropic 2026 年已完成 4 起公开并购，OpenAI 自 2023 年至少并购 17 家。两家都在为上市前的资产负债表、人才结构与叙事补齐动作。机器人是最后一块"垂直大模型 + 硬件 + 数据飞轮"未完全归属的战略高地，任何一家龙头的独立性都足以搅动整个格局。

OpenAI 作为 PI 的股东，可能在信息权限甚至优先谈判权上占优；Anthropic 若真的谈成，等于从后台把 OpenAI 的一张牌抽走。这也是为什么两家最近对 "acqui-hire vs. investor rights" 的法务口径都变得异常敏感。

**点评：** 传闻真假次要，重要的是市场已经默认——下一代大模型公司会把 "拥有一家一流机器人实验室" 当成入门资格；PI 的最终归属，可能会改写 2027 年整个 physical AI 的资本地图。

---

### 🥉 No.3 · Kimi K3 + DeepSeek V4：中国开源模型的"合围周"

**[VentureBeat · Moonshot Kimi K3 成史上最大开源 LLM](https://venturebeat.com/technology/chinas-moonshot-ai-releases-kimi-k3-the-largest-open-source-model-ever-rivaling-top-u-s-systems)**

Moonshot 已于 7 月 16 日发布 Kimi K3（2.8 万亿参数 MoE，约为 DeepSeek V4 Pro 的 1.75 倍），并在 7 月 17 日承诺 7 月 27 日以改良 MIT 协议发布**完整权重**；DeepSeek V4 稳定版将于 7 月 24 日上线，Hugging Face 首日 MIT 全权重开放。两者都是万亿级 MoE + 约 1M 上下文 + 激进定价，未来一周将形成中国开源阵营的"合围周"。

对企业而言，这直接压制 Flash 级闭源模型的定价空间。据 MarkTechPost 与 OrcaRouter 的对比，K3 与 V4 Pro 在推理与代码基准上都进入 Sonnet 5/GPT-5.6 Terra 同档位，而每 M token 的部署成本仍显著低于闭源 API。企业的 make-vs-buy 决策正在向 "hybrid" 快速倾斜——Flash 类 API 用来打冷启动，K3/V4 承担规模化推理。

值得注意的是许可证策略的变化：Kimi K3 的"改良 MIT"引入若干限制条款，而 DeepSeek 依然保持纯 MIT。这可能是 2026 年下半年开源阵营的第一次"许可证分化"，其他厂商会在此基础上试探自己的护栏。

**点评：** Flash 级闭源模型正在被中国开源阵营从下方"截断毛利"，7 月 24-27 日这一周之后，$3 / $10 的 API 定价将成为一条明确的天花板。

---

### 🏛️ No.4 · Q2 AI 游说破纪录 + 白宫自愿标准逼近 —— 监管窗口进入倒计时

**[BuildFastWithAI · Q2 AI 游说支出统计](https://www.buildfastwithai.com/blogs/ai-news-today-july-22-2026)**

Q2 各家 AI 公司披露的游说支出全线走高：Meta $5.99M（-15%，仍为最高单季）、Anthropic $1.97M（+26%）、OpenAI $1.2M（+18%）。同时 FT 消息，白宫正在与 OpenAI、Google、Anthropic 敲定前沿模型自愿发布标准，最快下周宣布。EU 则站在 8 月 2 日 AI Act 高风险条款生效倒计时，Q1 已开出 50 张、总额 €2.5 亿的罚单；中国的 "虚拟陪伴" 框架已于 7 月 15 日生效。

三个地区同时在收窄自由度：美国用"自愿标准+州诉讼"（Florida AG 已起诉 OpenAI）、EU 用"硬立法+高额罚款"、中国用"细分场景强合规"。这构成 2026 下半年最重要的一层背景噪声——**任何模型的发布都要多考虑一层"跨司法辖区可交付性"**，而 Gemini 3.5 Flash Cyber、Anthropic Mythos 这类自愿受限模型，就是提前给监管留的"合作姿态"。

**点评：** 监管从"要不要来"过渡到"以什么形式来"，各厂商的游说预算越涨越高，其实是在为下一步的"合规成本资本化"做准备；小玩家会被这个门槛直接筛掉。

---

### 💰 No.5 · AMD Q1 数据中心 $58 亿 + OpenAI/Meta 6GW 大单 —— AI 芯片超级周期未见拐点

**[Tech Insider · AMD 财报及大单公告](https://tech-insider.org/amd-stock-ai-data-center-2026/)**

AMD Q1 数据中心收入 $58 亿（+57% YoY），Q2 指引 $112 亿，OpenAI 与 Meta 的 6GW 采购承诺是主要驱动力，股价盘后 +14%。Nvidia 同期数据中心 $752 亿（+92% YoY），继续在 S&P 500 中占 7.5% 权重，超过整个能源+公用事业板块的合计。上半年北美创业融资创纪录 $5100 亿，其中超 70% 流向 AI 公司，OpenAI + Anthropic 合计吸走 $2170 亿。

三条趋势值得追踪：
1. **"第二供应商"结构落地**：OpenAI/Meta 不再只买 Nvidia，AMD 拿到 6GW 表明超大客户开始主动分散；
2. **AI 基建层估值反超模型层**：Fireworks AI 融资 $15 亿（估值 $175 亿）、Spectro Cloud $1 亿、Assort Health $1.2 亿——推理、编排、垂直落地成为新钱主方向；
3. **国防自主 7 月已吸引 $30 亿+**，物理 AI 与国防 AI 正在成为下一波军民融合的融资标签。

**点评：** 只要超大 AI Lab 还在"抢电、抢地、抢芯片"，芯片超级周期的拐点就不会在 2026 出现——真正的天花板是电力和先进封装，不是需求。

---

## 行业观察

7 月 22-23 日这两天，AI 行业最大的信号不是某一个新模型，而是三条主线**同时进入"分化落地期"**：

- **模型层已经承认没有"通杀旗舰"**：Google Pro 跳票、Anthropic 分 Fable/Opus/Sonnet、OpenAI 分 Sol/Terra/Luna、Meta 分 Muse Spark 系列——头部公司都在把资源从"打榜刷分"迁到"定价分层 + 场景分层"，Flash 级模型才是决定 2026 下半年营收曲线的关键。
- **开源阵营即将攻入闭源腹地**：Kimi K3 与 DeepSeek V4 的"合围周"会把 $3 / $10 的 API 定价钉成天花板；这也是为什么闭源模型开始集体做"受限版本"（Mythos、Flash Cyber）——差异化的价值锚正在从"能力"迁向"访问权与合规姿态"。
- **物理 AI + 机器人成为并购主战场**：Physical Intelligence 传闻只是冰山一角，接下来 6 个月的重要新闻将频繁涉及"某某大模型公司控股/收购某某机器人独角兽"；OpenAI 的股东身份 vs. Anthropic 的谈判姿态将定义这条赛道的初期规则。

配套观察：监管窗口在收窄（EU 8/2、白宫下周、州级诉讼频出）；芯片资本开支还在加速（AMD 6GW 只是开始）；应用侧的胜负手已经从"模型质量"转向"数据护城河 + 部署工程 + 合规姿态"三件套。下半年真正需要盯的，不是哪家又刷了 AIME，而是**谁掌握了物理 AI 数据飞轮 + 中低价 API 议价权**。

---

**数据来源：**
- [BuildFastWithAI - AI News Today July 22 2026](https://www.buildfastwithai.com/blogs/ai-news-today-july-22-2026)
- [TechCrunch - The Anthropic-Physical Intelligence rumor](https://techcrunch.com/2026/07/21/the-anthropic-physical-intelligence-rumor-roiling-ai-twitter/)
- [VentureBeat - Kimi K3 open-source release](https://venturebeat.com/technology/chinas-moonshot-ai-releases-kimi-k3-the-largest-open-source-model-ever-rivaling-top-u-s-systems)
- [ThursdAI July 2026 releases](https://thursdai.news/releases/2026-07)
- [Tech Insider - AMD Data Center Q1 2026](https://tech-insider.org/amd-stock-ai-data-center-2026/)
- [Financial Times - White House voluntary standards](https://www.ft.com/) (转引)
- [Crunchbase - H1 2026 startup funding](https://news.crunchbase.com/venture/na-startup-funding-ma-shattered-records-ai-q2-2026/)
- [DataCamp - Muse Spark 1.1](https://www.datacamp.com/blog/muse-spark-1-1)
