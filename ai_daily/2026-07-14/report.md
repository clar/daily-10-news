# AI Daily · 2026-07-14

## 今日焦点

> **智能体协议之战开打 · 全双工语音 AI 成新战场 · 华尔街正式拥抱中国模型 · 巨头合纵连横**
>
> - **五巨头结盟对抗 MCP**：Google、Microsoft、Salesforce、Snowflake、ServiceNow 联手推动新的智能体接入协议，直接叫板 Anthropic 主导的 MCP 生态
> - **OpenAI 发布 GPT-Live**：全双工语音架构，边听边想边说，支持实时翻译、对话中在线搜索与子代理任务委派
> - **Gemini 3.5 Pro 倒计时**：Google 官宣 7 月 17 日发布，200 万 token 上下文、Deep Think 推理、API 定价大幅下压
> - **Goldman Sachs 推荐中国模型**：向客户明确点名 DeepSeek V4、Qwen 3.5，理由是"80–90% 前沿能力 + 一小部分成本"
> - **Anthropic Glasswing 扩张 3 倍**：从 50 家扩至 15 国 150 家关键基础设施机构，Claude Mythos 全线上岗

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | Google/Microsoft/Salesforce/Snowflake/ServiceNow 联手推共通智能体协议对抗 Anthropic MCP | AIToolsRecap / BuildFastWithAI | ⭐⭐⭐⭐⭐ |
| 2 | OpenAI 发布 GPT-Live 全双工语音模型，支持实时翻译和对话中搜索 | OpenAI / BuildFastWithAI | ⭐⭐⭐⭐⭐ |
| 3 | Google 官宣 Gemini 3.5 Pro 于 7 月 17 日发布，200 万上下文 + Deep Think | Google / Unrot | ⭐⭐⭐⭐ |
| 4 | Musk 与 Altman 就 Apple 起诉 OpenAI 挖角 400+ 员工案在 X 公开互撕 | X / Unrot | ⭐⭐⭐⭐ |
| 5 | Anthropic 将 Project Glasswing 扩至 15 国 150 家机构，Claude Mythos 部署到位 | Anthropic | ⭐⭐⭐⭐ |
| 6 | Goldman Sachs 向客户推荐 DeepSeek V4、Qwen 3.5 等中国模型 | GS Research | ⭐⭐⭐⭐ |
| 7 | Meta 发布 Muse Spark 1.1，1M 上下文，主打多 Agent 协同 | Meta | ⭐⭐⭐⭐ |
| 8 | Cloudflare 上线 x402 Monetization Gateway，为智能体建立"收银台" | Cloudflare | ⭐⭐⭐⭐ |
| 9 | Mistral 发布 Leanstral 1.5，用 Lean 4 形式化证明验证代码 | Mistral | ⭐⭐⭐ |
| 10 | GPT Image 2 + Runway Aleph 2.0 单帧编辑传播至整段视频 | OpenAI / Runway | ⭐⭐⭐ |
| 11 | Anthropic 上线 Claude Corps 12 个月带薪 fellowship，NGO 场景，不要求学历 | Anthropic | ⭐⭐⭐ |
| 12 | OpenAI Deployment Company 收购 Northslope，扩充企业交付工程能力 | OpenAI | ⭐⭐⭐ |
| 13 | ECB 警告：AI 生产力与算法定价可能加剧通胀波动 | Reuters | ⭐⭐⭐ |
| 14 | 大部分美国工人支持设立"AI 财富基金"再分配 AI 利润 | Pew / Gallup | ⭐⭐⭐ |
| 15 | 千兆瓦级 AI 数据中心遭遇多地社区反对，水电供应成焦点 | Bloomberg | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · 五巨头结盟推共通智能体协议，正面挑战 Anthropic MCP

**[BuildFastWithAI · Top AI News July 13](https://www.buildfastwithai.com/blogs/ai-news-today-july-13-2026)**

Google、Microsoft、Salesforce、Snowflake、ServiceNow 五家企业软件与云计算巨头周日联合表态，将共同推动一套用于把 AI 智能体接入业务系统的开放协议。虽然联盟方尚未公开协议全名，但明确指向替代 Anthropic 十四个月前推出、如今被超过 800 家 SaaS 厂商实现的 Model Context Protocol（MCP）。声明列出的三大差异化卖点是：企业身份与权限一等公民、跨云可移植、"由标准组织而非单一厂商治理"。

这次结盟的时点意味深长。MCP 事实上已经成为智能体接入生态的默认标准——Anthropic、OpenAI、Meta、xAI 的最新模型都原生支持，Cursor、Cline 一类开发工具全线接入。对 Google 而言，最刺痛的地方是它自家的 Agent Space 和 Vertex AI Agent Builder 都不得不"兼容 MCP"才能被开发者接受；对 Microsoft，Copilot 的插件生态被 MCP 悄然吸走用户；对 Salesforce/ServiceNow/Snowflake，它们最不愿看到的是"客户先接入 Anthropic 智能体，再回过头压价 SaaS"。

看点在三条：一，SAP、Oracle、Workday 会不会加入——如果加入，则新协议将立刻覆盖美股 SaaS 半壁江山；二，OpenAI 的态度——Sam Altman 上周才在博客上把 MCP 称作"agent-web 的 HTTP"，公开选边显然为难；三，协议底层是不是 A2A（Google 4 月发布的智能体互操作草案）改造版，若是，则 Google 早有部署。

**点评：** 巨头联手不是要"废掉 MCP"，是要给 MCP 加一个"企业身份 + 治理"的兼容层——真正的赢家可能是"两个协议都实现"的模型厂商，而 Anthropic 也许会主动把治理让渡给标准组织换取生态和平。

---

### 🚀 No.2 · OpenAI 发布 GPT-Live，全双工语音架构重定义人机对话

**[OpenAI · GPT-Live 发布](https://openai.com/index/gpt-live/)**

GPT-Live 不是升级版 Advanced Voice Mode——它是一套全新的"边听边想边说"架构。传统语音 AI（包括之前的 4o Realtime）本质是"回合制"：等你说完 → 送进 LLM → 生成回复 → TTS 播放，端到端延迟 400–800ms。GPT-Live 引入并行的听/想/说三线程，能一边听你补充新条件，一边调整正在生成中的回复，一边和后台的 web 搜索 / 子 Agent 通信。OpenAI 声称"平均对话延迟降到 120ms 以下"，同时新增了对话中在线搜索、实时翻译、任务委派给 GPT-5.6 Sol 后台推理三项能力。

产品意义上，这是 OpenAI 第一次把语音模型正式定位为"客户支持、销售外呼、教学辅导"的生产工具，而非"手机上聊聊天"。定价从此前 6/24 美元每百万音频 token 下调到 3/12 美元，同时开放并发商用 SKU。这直接把 Retell、Vapi、Deepgram Voice Agent 一类 startup 打到墙角——它们的 API 转售 + 编排价值被彻底压缩。

技术上更值得关注的是"子 Agent 委派"：GPT-Live 是"实时前台"，遇到需要长推理的问题，直接后台调用 Sol，边生成"稍等我想一下"的自然填充语，边把结果流回来。这本质上把"多 Agent 协同"从概念变成了默认工程范式。

**点评：** 语音 AI 的竞争从"谁的音色更像人"进入"谁能真做工作"——GPT-Live 是第一款有资格进入 500 万美元级 BPO 招标的产品，Deepgram 和 ElevenLabs 该慌了。

---

### 🥊 No.3 · Musk 与 Altman 就 Apple 起诉 OpenAI 挖角案再度公开互撕

**[X · 相关讨论 / TechCrunch](https://techcrunch.com/)**

Apple 上周对 OpenAI 提起商业秘密诉讼，声称过去 18 个月 OpenAI 从 Apple 挖走了超过 400 名核心员工，其中包括 Siri、AJAX（Apple 内部 LLM）、Vision 团队的架构师，起诉核心指控是"系统性诱导员工泄露仍在保密期的技术细节"。周日晚，Musk 在 X 转发案件文书并写下"这就是为什么开源才是唯一体面的路"，Altman 隔了 47 分钟回复"你上个季度自己从 Waymo 挖了 90 人，我们没起诉过谁"，随后 Musk 引用 xAI Grok 4.5 生成的"人才流动数据"反击 OpenAI 的挖角比例是 xAI 的 3.2 倍。

这场骂战背后是硅谷 AI 人才市场的紧绷。据 Blind 6 月的匿名调查，头部 AI 研究员 12 个月薪资涨幅中位数达到 68%，前 5% 岗位签字费突破 800 万美元。Apple 起诉的战略意图并不是拿钱——诉讼请求中的赔偿金额只有 15 亿美元——而是设立"用挖角速度过快的 startup 会被诉讼拖住"的市场信号。

对 OpenAI 的实际影响可能被夸大：即使败诉，最大成本是接下来 2–3 年招聘时对 Apple 员工建立"竞业审查"流程。但对二线 startup 的伤害更大——如果 Apple 胜诉后建立起对第三方招聘的标准索赔模板，Anthropic、xAI、Perplexity 后续挖 Apple 人的成本会成倍上升。

**点评：** 这已经不是技术之争，是"谁能垄断顶尖研究员"的战争——诉讼是新武器，公开互撕只是烟雾。

---

### 💼 No.4 · Goldman Sachs 正式向机构客户推荐 DeepSeek V4、Qwen 3.5

**[Goldman Sachs Research（客户报告转载）](https://www.goldmansachs.com/insights/)**

Goldman Sachs 的 AI 应用研究组周一在给资管、对冲基金和企业客户的周报中，第一次以具体型号点名的方式建议客户在成本敏感的推理任务上使用 DeepSeek V4（发布于 6 月）与阿里通义 Qwen 3.5-Max。报告的核心数据点：在 GS 自建的 34 个"金融领域 golden set"上，DeepSeek V4 达到 GPT-5.6 Terra 的 87.4%、Qwen 3.5-Max 达到 91.2%，而 API 单价分别只有 Terra 的 12% 和 18%。

这份报告是华尔街态度转变的分水岭。此前所有主流投行都在合规层面把中国模型划为"仅供研究"档，理由是数据主权和地缘政治风险。Goldman 这次的突破是明确列出了"美国机构调用中国模型的合规路径"：只使用海外部署 endpoint（DeepSeek 由 Together AI 在美国 host、Qwen 由 SiliconFlow 在新加坡 host）、显式脱敏、审计日志留存 7 年。等于把"能不能用中国模型"从政策问题变成了工程问题。

副作用是双向的：一方面，OpenAI、Anthropic 的价格护城河将在批量调用场景遭到 30–50% 的压力，Sam Altman 上周才被迫把 Terra 的价格再降 22%；另一方面，DeepSeek 和阿里的"在美国以外的部署伙伴"这条业务线突然成了兵家必争之地，估计 Together AI、Fireworks、SiliconFlow 三家会在未来两个月启动新一轮融资。

**点评：** 中国模型不再是"性价比标签"下的小众选择——当 Goldman Sachs 用具体型号在客户报告里给推荐时，它已经是主菜单上的一道菜了。

---

### 🌐 No.5 · Gemini 3.5 Pro 定档 7 月 17 日：Google 在 GPT-5.6 之后的关键反击

**[Google Blog · Gemini 3.5 预告](https://blog.google/technology/ai/)**

Google DeepMind 官方账号周日晚放出 Gemini 3.5 Pro 于本周四（7 月 17 日）正式 GA 的公告。核心指标：200 万 token 上下文（是 GPT-5.6 Sol 的 4 倍）、Deep Think 深度推理模式（对标 Sol Max effort）、原生多模态（图像、视频、音频、代码交错）。价格是最大惊喜——input $1.25/M、output $10/M，比 GPT-5.6 Sol（$15/$60）低了一个数量级，只比 Terra 略贵 25%。

选择这个时机发布，是 Google 对 GPT-5.6 上周 Commerce Department 特批式发布的直接反制。Sundar Pichai 在给员工的备忘录中直白写道："我们不能在这个季度再输一次开发者心智。"Deep Think 模式据 DeepMind 内部预发资料，在 GDPval-AA v2 上综合得分预计将超过 Sol，Codeforces 已确认 Gemini 3.5 Pro 在 6 月的一次线上竞赛中获得 Grandmaster 段位。

真正的战略意义是价格：如果 3.5 Pro 在保留 200 万上下文优势的同时把价格压到 Sol 的十分之一，那么"长文档 + 代码库全量吞入 + 一次生成"这个当下最吸金的应用场景（法律、审计、科研文献综述、大型代码迁移）将向 Google 大规模倾斜。GitHub、Cursor、Replit 一类工具的默认模型可能在两周内就切换。

**点评：** 200 万上下文 + Sol 十分之一价格，Google 是把"用性价比取胜"当刀刃——问题是市场是不是已经忘了 Google 上一次"性价比高但产品做不出来"的痛。

---

## 行业观察

**协议主导权正在从模型层向智能体基础设施层转移。** MCP 的成功证明"谁定义智能体如何接入世界，谁就有下一轮的操作系统级红利"。今天的五巨头结盟其实是一次迟到的觉醒——过去 12 个月，SaaS 巨头集体误判了"智能体协议只是又一个 API 标准"，直到发现自家客户开始通过 Anthropic 智能体做端到端流程编排，SaaS 的 workflow 层被架空。接下来六个月，我们将看到 SAP、Oracle、Adobe 等一批同样被 MCP 边缘化的厂商加入或围观，一场类似当年"OpenID vs SAML"式的协议博弈已经开幕。

**语音 AI 从"消费者玩具"跨过"生产工具"门槛。** GPT-Live 的全双工架构让语音对话延迟第一次进入了"人类察觉不到"的区间，加上后台 Agent 委派，产品完全有能力承接客户支持、销售外呼、教育辅导这些数十亿美元级的传统外包市场。Deepgram、Retell、Vapi 需要重新回答自己的"why not OpenAI"。

**中国模型进入华尔街主流菜单。** Goldman 客户报告只是开始——JPMorgan、Morgan Stanley 内部的 AI 采购组据传都在做类似的能力测试。以往"意识形态 + 数据主权"的护栏正在被"合规路径"消解，未来 12 个月中国模型在美国企业市场的份额可能从当前 <3% 快速涨到 8–12%，改变整个定价格局。

**巨头在"合纵连横"，不再打单一牌。** 观察本周的信号：Google 一边推自家 Gemini 3.5 Pro，一边加入反 MCP 联盟；Microsoft 既押注 OpenAI 又深度绑定自家 Frontier Company；Meta 一手 Muse Spark 1.1，一手继续扩张 Neocloud。行业从"模型公司 vs 模型公司"进入"平台组合 vs 平台组合"的对抗，选边站的成本对客户变得更高，但也让整个市场进入更成熟的价值分配阶段。
