# AI 日报 · 2026-05-02

## 今日焦点

> **五角大楼绕开 Anthropic · Mythos 成"国家安全时刻" · Anthropic 9000 亿估值 · OpenAI 月营收破 20 亿 · 欧盟 AI Act 8 月大限将至**
>
> - **五角大楼与 7 家 AI 公司签机密合同，独缺 Anthropic** —— Anthropic 因坚持"不让 Claude 用于全自主武器"被列入"供应链风险"
> - **Pentagon CTO：Mythos 是"国家安全时刻"** —— 即便在黑名单上，NSA 仍在偷偷用 Anthropic 的 Mythos Preview 找网络漏洞
> - **Anthropic 据传洽谈 9000 亿美元估值融资** —— 年化收入从 2025 年底的 90 亿冲到 300 亿，6 个月狂飙 3.3 倍
> - **OpenAI 月营收突破 20 亿美元** —— 折算 ARR 约 240–250 亿，Q4 2026 IPO 目标价仍直奔万亿
> - **欧盟 AI Act 高风险条款将于 8 月 2 日生效** —— "Digital Omnibus"延期方案不确定，企业不能赌

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | 五角大楼与 7 家 AI 巨头签机密网络合同，跳过 Anthropic | CNN / Defense News | ⭐⭐⭐⭐⭐ |
| 2 | Pentagon CTO：Anthropic 仍在黑名单，但 Mythos 是"国家安全时刻" | CNBC / The Register | ⭐⭐⭐⭐⭐ |
| 3 | Anthropic 据传以 9000 亿美元估值洽谈新一轮融资 | The Motley Fool | ⭐⭐⭐⭐⭐ |
| 4 | NSA 仍在使用 Anthropic Mythos Preview，绕开 DOD 禁令 | Axios / TechCrunch | ⭐⭐⭐⭐ |
| 5 | OpenAI 月营收突破 20 亿美元，ARR 触及 250 亿区间 | Sacra / WSJ | ⭐⭐⭐⭐ |
| 6 | Trump 政府起草执行令，拟将 Anthropic 拉回政府合作 | Axios | ⭐⭐⭐⭐ |
| 7 | Google 拟向 Anthropic 投资最高 400 亿美元（首笔 100 亿，估值 3500 亿） | TechCrunch | ⭐⭐⭐⭐ |
| 8 | Nvidia 承诺向 OpenAI 分批投资最高 1000 亿美元（绑定 10GW Vera Rubin 部署） | Nvidia / OpenAI | ⭐⭐⭐⭐ |
| 9 | Reflection（开权重模型创业公司）获 Pentagon 合同，与巨头同列 | DefenseScoop | ⭐⭐⭐⭐ |
| 10 | 欧盟 AI Act 8 月 2 日高风险条款生效，Digital Omnibus 延期未定 | Legal Nodes / EU Commission | ⭐⭐⭐⭐ |
| 11 | Nvidia 投资瑞典法律 AI Legora，估值 56 亿美元 | CNBC | ⭐⭐⭐ |
| 12 | OpenAI 向散户开放 122 亿美元融资轮 | TechCrunch | ⭐⭐⭐ |
| 13 | Stanford HAI 2026 AI Index 发布，前沿模型趋同 | IEEE Spectrum | ⭐⭐⭐ |
| 14 | SpaceX/xAI 合并实体进入 DOD 机密网络 | DefenseScoop | ⭐⭐⭐ |
| 15 | Mattpocock、obra 的 Claude Skills 仓库一夜爆红，Skills 工程化破圈 | GitHub Trending | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · 五角大楼与 7 家 AI 公司签机密合同，独把 Anthropic 排除在外

**[CNN Business](https://www.cnn.com/2026/05/01/tech/pentagon-ai-anthropic) · [Defense News](https://www.defensenews.com/news/pentagon-congress/2026/05/01/pentagon-freezes-out-anthropic-as-it-signs-deals-with-ai-rivals/) · [DefenseScoop](https://defensescoop.com/2026/05/01/dod-expands-classified-ai-work-with-8-companies-excluding-anthropic/)**

5 月 1 日，国防部宣布与 SpaceX、OpenAI、Google、Nvidia、Reflection、Microsoft、AWS 七家 AI 公司签订协议，把它们的能力部署到 DOD 的机密网络（Impact Levels 6 和 7）。**Anthropic 被明确排除**。冲突的导火索是 Anthropic 拒绝让 Claude 用于"全自主武器"和"大规模国内监控"——它要求保留可接受用途条款，而 Pentagon 想要"all lawful purposes"的不限制访问。Trump 政府随后宣布与 Anthropic 切断联系，并将其打上"供应链风险"标签——这个标签过去只用在跟敌对国家关联的公司身上。Anthropic 已就此起诉政府，加州一名联邦法官上月已经阻止了部分行政措施。

这是 AI 行业第一次出现"主流前沿模型公司被本国国防部以政治理由列入黑名单"的事件。它对行业的影响是**结构性的**：第一，它给所有 AI 实验室上了一课——你的"模型政策"不再只是公关声明，而是会直接决定能不能进入万亿级政府市场；第二，它把"对齐 vs 商业"的张力搬到了台面上——Anthropic 选择守住红线，代价是把 DOD 这块巨型预算让给了 OpenAI、Google 和 Reflection；第三，它给后入局者（Reflection 这种开权重创业公司）创造了"上桌"的窗口——平时根本挤不进巨头名单的玩家，因为接受了 Pentagon 的全条款而被点名同列。

**值得继续观察的是"复合"信号**：4 月 17 日 Trump 幕僚长 Susie Wiles 与 Dario Amodei 在白宫开过会，4 月 29 日 Axios 又爆出政府内部在起草执行令重新拉 Anthropic 回来。换句话说，Trump 政府嘴上"封杀"，私下"和谈"——这个矛盾正是 Mythos 撕开的口子（见下条）。

**点评：** 这件事的真正信号不是"Anthropic 被踢出局"，而是"美国政府第一次系统性地把'AI 公司服从度'当作采购门槛"——所有走前沿路线的实验室，未来都要在"政策红线"和"政府生意"之间做一次不可逆的选择题。

---

### 🚀 No.2 · Pentagon CTO：Mythos 是"国家安全时刻"，但 Anthropic 仍在黑名单

**[CNBC](https://www.cnbc.com/2026/05/01/pentagon-anthropic-blacklist-mythos-michael.html) · [The Register](https://www.theregister.com/2026/05/01/mythos_complicates_anthropic_us_gov_breakup/) · [Axios](https://www.axios.com/2026/04/19/nsa-anthropic-mythos-pentagon)**

在 5 月 1 日同一天的发布会上，Pentagon CTO Emil Michael 公开说了一段非常分裂的话：Anthropic 仍然是"供应链风险"，但 Anthropic 的 **Mythos** 模型——一款专门强化了网络攻防能力的模型——是一个"separate national security moment"。Mythos 的强项是自主发现并修补软件零日漏洞。Axios 早在 4 月 19 日就独家披露：**NSA 已经在使用 Mythos Preview**，绕开了 DOD 的封禁。

这条新闻把"Anthropic 被禁"的故事彻底反转：DOD 嘴上拒绝整个公司，但情报机构正在偷偷用它最强的模型干最敏感的活。Pentagon CTO 把"Mythos 是国家安全级别的能力"这话说出口，等于公开承认**美国政府离不开 Anthropic 的最前沿能力**——只是它需要一个面子上的解决方案。

这件事释放的工业信号也很重要：**网络攻防是大模型第一个被官方背书的"杀手级垂直应用"**。过去两年所有人都在猜"哪个垂直会先跑通"，现在 Pentagon CTO 等于盖章了——cyber 是第一个。Mythos 之所以被切割对待，正是因为它在零日漏洞发现/修补上的能力强到不可替代。

**点评：** 当一家被本国国防部列入黑名单的公司，同时被同一个国防部的 CTO 称为"国家安全时刻"，这本身就说明前沿模型的稀缺性已经超过了任何政治叙事——政治会让步，能力不会。

---

### 🥇 No.3 · Anthropic 据传以 9000 亿美元估值洽谈新一轮融资，年化收入冲上 300 亿

**[The Motley Fool](https://www.fool.com/investing/2026/05/01/spacex-anthropic-and-openai-could-be-fast-tracked/) · [Anthropic Blog](https://www.anthropic.com/news)**

最新报道显示，Anthropic 正在以**约 9000 亿美元估值**洽谈新一轮融资，对标 OpenAI 当前 8520 亿美元的估值水平。同时，Anthropic 公布的运营数据非常激进：年化收入（run-rate revenue）已突破 **300 亿美元**，相比 2025 年底的 90 亿暴涨超过 3 倍；年消费超 100 万美元的企业客户从 2 月份的 500+ 翻倍到 1000+。

这一组数据有几个值得拆开看的地方：第一，**ARR 在半年内翻 3 倍**意味着 Anthropic 抓住了"企业级 Claude（特别是 Claude Code 和 Sonnet/Opus 系列）"这一波采购浪潮——几乎每个企业都在给开发团队配 Claude Code 席位；第二，**百万美元级客户翻倍**说明 Anthropic 在大客户深耕上远比 OpenAI 想象中扎实；第三，估值倍数（9000 亿 / 300 亿 = 30 倍 ARR）和 OpenAI（8520 亿 / 240 亿 ≈ 35 倍）几乎贴齐，市场已经把两家放在同一档定价。

更耐人寻味的是与上面两条新闻的对照：**被 Pentagon 封杀的同一周，私募市场给出了 9000 亿美元的估值**。资本市场用真金白银投票认为，Anthropic 不靠政府订单也能赢。

**点评：** Anthropic 的故事正变成 AI 时代最特别的样本——一家拒绝把模型卖给国防部、却能在 6 个月里把 ARR 跑到 300 亿的公司，证明了"对齐立场"在企业市场反而是定价权。

---

### 💰 No.4 · OpenAI 月营收突破 20 亿美元，IPO 估值仍直奔万亿

**[Sacra](https://sacra.com/c/openai/) · [TechCrunch](https://techcrunch.com/2026/03/31/openai-not-yet-public-raises-3b-from-retail-investors-in-monster-122b-fund-raise/) · [IndexBox](https://www.indexbox.io/blog/openai-targets-q4-2026-ipo-with-1-trillion-valuation-goal/)**

Sacra 数据显示，OpenAI 月营收已突破 20 亿美元，年化收入从 2025 年底 200 亿涨到 2026 年 2 月的 250 亿；CFO Sarah Friar 公开确认 2025 财年 200 亿的数字。**企业业务占比超 40%，预计 2026 年底与消费业务持平**——这是 OpenAI 商业模型的关键转向：从一个 ChatGPT C 端公司变成一个真正的企业 SaaS。

同时，OpenAI 刚刚以 8520 亿美元估值完成 1220 亿美元融资轮，目标 Q4 2026 提交 IPO 申请、2027 年挂牌，目标估值瞄准**1 万亿美元**。但《华尔街日报》也报道公司错过了部分内部营收目标，散户已经开始紧张。

把这条和 Nvidia 投资 1000 亿美元的承诺放一起看尤其有意思：Nvidia 的 1000 亿是**"按 GW 部署分批兑现"**——也就是说，OpenAI 的资本注入和 Nvidia 的 Vera Rubin 平台部署进度强绑定。这是一种新型的"结构化融资"：资本不是一次给到，而是按算力消耗节奏放款。

**点评：** OpenAI 营收数字的真实意义是——**它正在变成历史上最贵的"硬件订阅公司"**：每一美元营收背后是几十亿美元的算力承诺，IPO 估值的天花板取决于它能不能把"模型边际成本下降"跑赢"用户使用量上升"。

---

### 🌍 No.5 · 欧盟 AI Act 8 月 2 日大限将至，Digital Omnibus 延期能不能落地仍是悬念

**[EU Commission](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) · [Legal Nodes](https://www.legalnodes.com/article/eu-ai-act-2026-updates-compliance-requirements-and-business-risks) · [TechPolicy.Press](https://www.techpolicy.press/what-the-eus-first-digital-markets-act-review-actually-changes/)**

距离 2026 年 8 月 2 日还剩 3 个月，届时欧盟 AI Act 的**高风险 AI 系统义务**将正式生效——覆盖招聘、信贷、教育、执法、医疗等场景。所有 Annex III 高风险系统都要走完合规评估、注册到欧盟数据库、配备人类监督机制。罚款最高可达**全球年营收 7%**。

唯一的不确定性是欧盟委员会在 2025 年底提出的"Digital Omnibus"方案，可能把 Annex III 高风险义务推迟到 2027 年 12 月。但律所普遍建议：**不要赌延期会通过**，按 8 月 2 日为硬截止做合规。

这条和前面几条放一起看其实是同一个故事的另一面：当美国把"AI 政治化"，欧盟在把"AI 规则化"。两套体系正在分叉——美国版是"政府点头算数"，欧盟版是"流程合规算数"。任何一家全球部署的 AI 公司未来都要同时玩这两种游戏。

**点评：** AI 公司的法务团队正在变成战略部门——8 月 2 日不是合规小问题，而是欧盟版"AI 公司护照"的发证日；没拿到的，等于失去欧洲企业市场的入场资格。

---

## 行业观察

今天的所有大新闻汇集成一个明确的主题：**AI 行业进入"主权时代"**。

**地缘维度**：美国把 AI 政治化（Anthropic 黑名单事件），欧盟把 AI 规则化（8 月 2 日 Annex III 生效）。两个体系开始分别向 AI 公司提出"政治服从度"和"流程合规度"的双重门槛。

**资本维度**：OpenAI 8520 亿、Anthropic 9000 亿、Nvidia–OpenAI 1000 亿绑定算力、Google–Anthropic 400 亿绑定算力——前沿模型公司的融资方式已经不是"卖股权换现金"，而是"卖股权换算力承诺"。资本市场在用估值告诉所有人：算力等于话语权。

**商业维度**：OpenAI 月营收 20 亿、Anthropic ARR 300 亿，企业业务全面起飞。但同时 GitHub Trending 上 `mattpocock/skills`、`obra/superpowers` 一夜爆红说明——**真正决定企业付钱的是"工程化方法论"**，而不只是模型本身。前沿模型趋同（Stanford AI Index 显示 GPT-5.4、Claude Opus 4.6、Gemini 3.1 Pro 在综合榜上互相只差 4 分），差异化战场正在转移到工具链和工作流。

**安全维度**：Mythos 这条线最值得长期跟踪。Pentagon CTO 公开承认"Mythos 是国家安全时刻"，加上 NSA 已经在偷偷用，意味着**网络攻防成为前沿模型第一个被官方认证的"国家级垂直应用"**。这会带动整个 AI 安全产业从"研究话题"上升为"国防资产"。
