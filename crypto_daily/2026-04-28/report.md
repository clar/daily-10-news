# 加密日报 · 2026-04-28

## 今日焦点

> **BTC 试探 $80K · ETF 连续四周净流入 · LayerZero 跨链漏洞扩散 · "Reg Crypto" 临门一脚 · 4 月成 2025 年 2 月以来最惨被黑月**
>
> - **BTC 周一开盘 $78,670 后回落 $77,856**，盘中曾摸 $79,000，市场卡在 $80K 整数关口前蓄势
> - **现货 BTC ETF 上周净流入 $824M**，连续第四周为正，BlackRock IBIT 占 $733M，AUM 突破 $1,020 亿
> - **KelpDAO $2.93 亿被盗事件 + 4 月 1 日 Drift $2.85 亿被盗共占月度损失 95%**，均指向朝鲜 Lazarus
> - **Tether USDT0（$40.65 亿）成 LayerZero 漏洞最大暴露资产**，全行业 $45 亿 TVL 同样攻击向量未修复
> - **SEC 主席 Atkins：白宫即将批准"Reg Crypto"提案**，针对初创豁免与发币融资规则一次性立规

---

## 热门新闻速览

| # | 标题 | 分类 | 要点 |
|---|------|------|------|
| 1 | **BTC 短暂触 $79,000 后回落，等待美联储议息** | 行情 | 现价 $77,856，离 $80K 仅 2.7% |
| 2 | **现货 BTC ETF 连四周净流入，IBIT 单周吸金 $733M** | 机构 | 全市场 4/20-4/24 +$824M，AUM $1,020 亿 |
| 3 | **现货 ETH ETF 第三周连流入 +$155M** | 机构 | Solana/XRP 小额 ETF 同步吸金 |
| 4 | **Morgan Stanley MSBT 上市后首周净流入 $71M** | 机构 | 大行系 BTC 现货 ETF 阵营再添一员 |
| 5 | **KelpDAO 跨链桥被盗 $293M，疑 Lazarus 所为** | 安全 | 经 LayerZero 伪造跨链消息释放 116,500 rsETH |
| 6 | **Aave 联合 DeFi 伙伴启动救市，稳定币贷方撤资 $5B** | 安全 | 4 月单月已损失 $606M，年度最差 |
| 7 | **Volo Protocol 被攻击损失 $3.5M / GiddyDefi 损失 $1.3M** | 安全 | KelpDAO 后续余震不断 |
| 8 | **Circle 呼吁 DeFi 全面启用"熔断器"机制** | 行业 | 回应 Drift Protocol $270M 被盗 |
| 9 | **SEC 主席 Atkins：Reg Crypto 待白宫签字即发布** | 监管 | 涉初创豁免、ICO/ITO 融资规则 |
| 10 | **以太坊 Glamsterdam 升级路线图：并行执行+gas 上调至 100M** | 技术 | H1 内主网，配合 ePBS |
| 11 | **Aave V4 在以太坊主网上线** | 生态 | 市场分段+定制风险曲线，重夺借贷主导 |
| 12 | **Solana TVL 因 Drift 事件回落至 $6.3B** | 行情 | 仅为以太坊 11% |

---

## 重点点评

### 🔑 1. KelpDAO $2.93 亿被盗 — LayerZero 跨链信任模型迎来"系统性时刻"

[CoinDesk: 'DeFi is dead' — community scrambles after $292M KelpDAO hack](https://www.coindesk.com/news-analysis/2026/04/19/defi-is-dead-crypto-community-scrambles-after-usd292-million-hack-exposes-cross-chain-risks) · [Crowdfund Insider: Billions Exposed](https://www.crowdfundinsider.com/2026/04/275229-defi-hack-analysis-billions-in-crypto-assets-left-exposed-after-kelp-dao-exploit/)

事件经过：4 月 19 日，攻击者通过伪造 LayerZero 跨链消息让 KelpDAO 的桥相信"另一条链确认了一笔合法指令"，从而向攻击者地址释放 116,500 rsETH，按当时价折合约 $2.93 亿。这是 2026 年至今最大单笔 DeFi 被盗，配合 4 月 1 日 Drift Protocol 的 $2.85 亿事件（事后归因 Lazarus），4 月单月损失合计 $6.06 亿，仅 18 天就把这个月推到 2025 年 2 月（Bybit $14 亿）以来最惨。

为什么这次不一样：研究人员指出**几乎一半基于 LayerZero 的活跃应用仍然存在同一攻击向量**，潜在暴露资产 $45 亿，其中 Tether 的全链稳定币 USDT0（$40.65 亿在外流通）独占 87%。稳定币贷方在事件次日从 Aave 抽走了 $50 亿，恐慌效应已经蔓延到借贷与做市端。Aave 牵头的"DeFi 救援基金"试图把损失内部消化，但市场更关心的是：跨链消息层这种"信任由几个 oracle/relayer 联合给出"的设计，是否还能继续做生产级桥的核心。

接下来三件事必须看：(a) LayerZero 是否给出强制升级路径以及由谁承担升级成本；(b) Tether 会不会主动把 USDT0 余额回到原生 USDT 以降低系统风险；(c) Circle 已经公开呼吁的"DeFi 熔断器"是否被主流协议采纳——如果是，这一年 DeFi 的设计语言可能从"无许可即时结算"转向"有条件可暂停"。

---

### 🔑 2. ETF 四周连阳 + MSBT 入场 — 机构买盘正在成为 BTC 的隐形"日内做市商"

[CoinDesk: BTC ETFs pulled $2B in 8 days](https://www.coindesk.com/markets/2026/04/24/bitcoin-etfs-just-pulled-usd2-billion-in-8-days-while-short-term-holders-quietly-started-selling) · [Crypto Times: $824M weekly inflow](https://www.cryptotimes.io/2026/04/27/spot-bitcoin-etfs-post-fourth-straight-week-of-gains-with-824m-inflows/)

数据切片：4/20-4/24 现货 BTC ETF 周净流入 $824M（连续四周正流入），单 IBIT $733M；8 个交易日维度净流入 $20 亿；累计 AUM 突破 $1,020 亿。Morgan Stanley 4 月 8 日新上的 MSBT 首个完整交易周吸金 $7,100 万——大行渠道正在把"传统经纪账户里的 BTC 配置"做成默认动作。同期短期持有者（STH）开始悄悄出货，这种"机构买、散户卖"的剪刀差通常是结构性牛市中后期的特征。

为什么对今日行情重要：BTC 在 $77K-$80K 横盘已经超过两周，本周还有美联储议息（市场预期不变利率但有可能转鸽）和伊朗-美国和谈消息双重宏观触发器。如果 ETF 流入继续吸收 STH 的派发，价格上行就只是时间问题；反之，若机构资金也开始观望，$77K 心理位将面临再次测试。

值得记下的结构性变化：现货 ETH ETF 也连续第三周净流入（+$155M），Solana/XRP 小额 ETF 开始有确定性正流入。**BTC 不再独享机构通道**——多资产 ETF 化让加密 beta 资金可以在不离开美元基金账户的前提下完成轮动。

---

### 🔑 3. SEC "Reg Crypto" 临门 — 美国第一次有"统一加密发行规则"

[CoinDesk daybook 多篇引述 Atkins 表态]

SEC 新主席 Paul Atkins 表示，"Reg Crypto"提案待白宫签字即对外发布，重点解决**初创豁免与代币发行/融资规则**——这是历史上 SEC 第一次拟把 ICO/ITO 与传统证券发行套利空间正面收紧，并配套给合规初创一条"小额简化"路径。配合 3 月底已经获批的现货 BTC ETF 期权交易，美国正在把"加密 = 主流证券"这条法律叙事一次性闭环。

对市场的实际影响分两层：短期，**境内合规发币的窗口被打开**，但门槛与披露可能更接近 Reg A+ / Reg D，传统 VC 主导的代币融资将受益，meme coin 与匿名团队的发行难度上升；长期，监管套利从"美国 vs 其他"变成"哪个豁免类别最划算"，加密律师事务所的业务结构会被改写。

需要观察的伏笔：CFTC 与 SEC 的边界（ETH 与新型 staking 代币归谁管）、链上身份/KYC 是否会被纳入规则、以及 Atkins 在国会听证会上承诺的"小额豁免每年金额上限"。这一条新闻今天还没落地，但市场已经在前置定价——即将上市的几只合规 token 项目的二级折价正在收敛。

---

### 🔑 4. ETH Glamsterdam 升级 + Aave V4 上线 — 以太坊主网"赢回 DeFi"的最后一步

[Bitcoin Foundation: Major Ethereum Updates 2026](https://bitcoinfoundation.org/news/ethereum/major-ethereum-updates-2026-overview-protocol-upgrades-and-strategic-roadmap/) · [Symbiosis: Ethereum Ecosystem 2026](https://symbiosis.finance/blog/ethereum-ecosystem-in-2026-what-changed-in-defi)

技术维度：Glamsterdam 升级目标在 2026 上半年主网，三件事——**并行交易执行**、**enshrined PBS（出块者-构建者分离写进协议）**、**gas 上限提升到 100M+**。配合 2025 年 Pectra 已经把 L2 单笔成本压到 $0.10-0.50，主网交易能力的天花板被一次性顶高。

应用维度：4 月 Aave V4 主网上线，引入"市场分段+定制风险曲线"，让借贷市场从一个超级池变成多池治理。这一变更在 KelpDAO 事件后看尤其关键——"风险隔离"在不到一周时间被实战验证为正确方向，机构 DeFi 资金会优先流向支持隔离风险的协议。

宏观信号：Solana TVL 在 Drift 事件后回落到 $6.3B，约为以太坊的 11%。Solana 在交易速度和零售活跃度上仍领先，但**机构 DeFi 资金（借贷、稳定币、RWA）正在加速回到以太坊主网+L2**。这与 2024-2025 的"高频应用上 Solana、价值储存上 ETH"叙事吻合，但今年走得更快。

---

### 🔑 5. 4 月被黑月：$606M / 18 天，Wall Street 信心被动摇

[crypto.news: April 2026 Worst Month](https://crypto.news/april-2026-worst-month-for-crypto-hacks/) · [TheStreet: Crypto hacks raise concerns](https://www.thestreet.com/crypto/markets/crypto-hacks-raise-fresh-concerns-for-wall-street-adoption)

数据上看：4 月前 18 天累计被盗 $6.06 亿，仅次于 2025 年 2 月 Bybit 被盗 $14 亿，是这一年最差。Drift（$2.85 亿）和 KelpDAO（$2.93 亿）两笔大单合计占 95%，且都指向朝鲜 Lazarus。Volo Protocol $350 万、GiddyDefi $130 万属于"小额持续渗透"——攻击者已经在用同样的 LayerZero 漏洞做"批发-零售"分层收割。

对华尔街叙事的影响：BTC ETF 流入屡创新高，但 DeFi 这一翼正在让传统资金看到"链上托管+智能合约组合"的真实风险。预计未来 30 天里，机构会显著加大对**保险型协议（Nexus Mutual、Sherlock 等）**和**链上托管 + 多签**方案的配置，而新进 DeFi 资金会更挑协议——任何依赖跨链消息的产品要重新被风控部门看过。

宏观结论：2026 年加密市场正在出现"资金两极化"——**ETF 通道吸金创新高**，**DeFi 通道在被快速去信任化**。这不是矛盾，而是机构在做风险定价：BTC 当数字黄金可买，但 DeFi 应用必须等到代码更安全、桥更可靠、保险更厚再说。

---

## 市场脉搏

- **BTC**：$77,856（-1.0% 24h），前高 $79,000，关键阻力 $80,000，支撑 $76,500
- **ETH**：$2,320.84（-2.1% 24h），$2,300 是短期心理位；Glamsterdam 升级临近形成预期溢价
- **SOL**：受 Drift 事件拖累，TVL $6.3B，相对以太坊比值降至 11%
- **ETF 流向**：BTC 现货 ETF 月内 +$24.3 亿；ETH 现货 ETF 三周连阳；BlackRock IBIT 单日 $167.5M 进入全美 ETF 流入前 1%
- **DeFi**：4 月被盗 $6.06 亿（Drift + KelpDAO 占 95%）；Aave 借贷池一度被抽走 $50 亿稳定币
- **宏观催化**：本周美联储议息 + 伊朗-美国和谈消息 + 美国"Reg Crypto"提案落地三大变量交汇

