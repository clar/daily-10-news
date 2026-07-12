# 加密日报 · 2026-07-13

## 今日焦点

> **BTC 站上 $63k · ETH ETF 逆势吸金 · CLARITY 法案发酵 · Aptos 系统级漏洞险酿 700 亿 · Solana Alpenglow 定档 H2**
>
> - **BTC 周内涨 2.8% 至 $63,050 附近** ETF 资金结束 10 日净流出，单日回补 $221.7M 创两月新高
> - **ETH ETF 单日净流入 $70.5M** BTC 现货 ETF 反倒净流出 $84.9M，机构在做"BTC → ETH 战术切换"
> - **SEC 7 月三项加密新规拟稿** 涵盖代币发行、经纪商资本要求、市场结构，CLARITY 法案落地进入倒计时
> - **Hexens 揭 Aptos 共识层漏洞** 3000 美元服务器可控制 1/3 验证者，涉及 700 亿资产，已紧急修补
> - **Fannie Mae 允许加密作按揭抵押** 首次把 BTC/ETH 纳入常规住房贷款抵押品清单

---

## 热门新闻速览

| # | 标题 | 分类 | 要点 |
|---|------|------|------|
| 1 | **BTC ETF 单日净流入 $221.7M，结束 10 日流出** | 机构 | 两月最大回补，市场情绪转正 |
| 2 | **ETH ETF 单日净流入 $70.5M，Fidelity FETH 独占 $69.2M** | 机构 | 机构做 BTC → ETH 战术轮动 |
| 3 | **SEC 将三项加密规则纳入 7 月 NPRM 议程** | 监管 | 代币发行、经纪商资本、市场结构 |
| 4 | **Fannie Mae 接受 BTC/ETH 作按揭抵押** | 采用 | 房地美首次背书加密抵押品 |
| 5 | **Hexens 披露 Aptos 共识漏洞，涉 700 亿资产** | 安全 | 3000 美元服务器可攻击 1/3 验证者 |
| 6 | **Hinkal Protocol 隐私池遭 $820K USDC 攻击** | 安全 | prooflessDeposit 函数被滥用 |
| 7 | **Solana Alpenglow 升级敲定 H2 上线** | 技术 | 终局性从 12.8s 压至 100-150ms |
| 8 | **Ethereum Glamsterdam 升级路线图公布** | 技术 | 并行执行 + 更高 gas limit |
| 9 | **Bitget Wallet 用户破亿，支付日活超过交易** | 采用 | 加密钱包首次向日常支付倾斜 |
| 10 | **Clearstream 上线 Solana 机构托管** | 机构 | Deutsche Börse 系合规通道打开 |
| 11 | **Grayscale HYPE ETF 提交 S-1 修正六稿** | 机构 | Hyperliquid 质押 ETF 审核推进 |
| 12 | **Kling AI 20 亿融资中出现加密支付通道条款** | 生态 | 稳定币与 AI 结算首次公开写入合同 |

---

## 重点点评

### 🔑 1. ETH ETF 逆势吸金 vs BTC ETF 净流出 — 机构轮动信号第一次清晰

**[The Block · Crypto ETFs 2026 tailwinds](https://www.theblock.co/post/383361/crypto-etfs-2026-regulatory-tailwinds-issuers-brace-crowded-year)**

7 月 8 日的数据尤其值得关注：BTC 现货 ETF 单日净流出 $84.9M，同时 ETH 现货 ETF 净流入 $70.5M，其中 Fidelity FETH 单只占 $69.2M。这不是简单的"资金再平衡"，而是自今年 3 月 ETH ETF 允许质押收益以来第一次出现的机构轮动：ETH ETF 因 3.5-4% 的原生收益率对配置盘吸引力显著超过 BTC ETF。

宏观上，7 月 CLARITY 法案预期升温 + FOMC 议息临近 + 美股 mag7 盈利周期尾声，多种资产同时进入"重估阶段"。ETH 的定价里现在混入了"收益 + 支付 + L2 生态"三重叙事，BTC 短期缺少新催化剂。CoinShares 数据显示 7 月至今 ETH 产品累计流入已超 BTC 产品的 40%，这个比例在过去 12 个月只有两次出现过。

下一步观察：如果 8 月 Solana staking ETF 通过并出现类似 ETH 的资金结构，"配置级机构在收益型加密 ETF 里分层部署"的模式就会成为默认玩法。

---

### 🔑 2. Aptos 700 亿美元系统性漏洞被 3000 美元服务器揭穿 — L1 安全预警

**[CoinDesk · Ethical hackers found $70B flaw](https://www.coindesk.com/tech/2026/07/04/how-ethical-hackers-with-just-a-usd3-000-server-found-a-flaw-that-could-ve-put-usd70-billion-in-crypto-at-risk)**

以色列白帽团队 Hexens 披露：Aptos 主网存在一个共识层 bug，攻击者用一台 3000 美元的普通服务器就能模拟 1/3 验证者做出 90%+ 成功率的攻击，理论上可波及主网上所有稳定币、跨链桥和 DeFi TVL，累计价值约 700 亿美元。漏洞于 2 月 25 日通过紧急通道报告，几天内完成补丁，未产生实际损失。

问题是舆论层面的连锁——过去两年 L1 的"验证者数量安全叙事"被反复引用，但 Aptos 事件表明经济安全和拜占庭安全不是同一件事：即使 stake 分布合规，代码层的 corner case 也可能让 1/3 验证者足以推翻 finality。这与传统 PoS 假设"1/3 攻击需要现金收购或社交攻击"的模型有质的区别。

行业级影响：多家资管在 7 月前正在完成 Aptos 的托管接入评估，事件后至少三家暂停。同时，Move 语言（Aptos/Sui 共用）阵营会承受更严苛的审计压力，Sui 的类似逻辑也在紧急自查。这对 Solana、EVM 系是短期利好，中期则是"L1 审计标准全面升级"的信号弹。

---

### 🔑 3. Fannie Mae 接受 BTC/ETH 作按揭抵押 — 传统金融第一次实操落地

**[Yahoo Finance · Bitcoin ethereum July 10](https://finance.yahoo.com/personal-finance/investing/article/bitcoin-and-ethereum-prices-today-friday-july-10-2026-up-nearly-3-since-last-friday-130101171.html)**

美国最大房贷再融资通道 Fannie Mae 本周官宣：常规住房贷款抵押池现在正式接受 BTC 与 ETH 作为部分抵押，估值按 30 日 VWAP 打 65% 折扣，托管必须走 SEC 注册的合格托管人（当前名单包含 Coinbase Custody、Fidelity Digital Assets、BitGo Trust）。这是首次由联邦系挂钩机构在合规抵押品清单中纳入原生加密资产。

意义在两个层面：其一，加密从"投资资产"跨越到"信用抵押"，这是宏观资产负债表意义上的一次身份升级；其二，Fannie Mae 的接受意味着 GSE 内部风控（尤其是 BSA/AML 与破产隔离）已经通过初步审查，为其他 GSE（Freddie Mac、Ginnie Mae）跟进铺路。

风险面：VWAP + 65% 折扣意味着抵押物波动放大后可能触发追加保证金链条，历史上房贷市场对波动敏感度极高。若 BTC 出现 30%+ 单月回撤，可能引发首次"加密抵押追加"事件，会成为监管一年内的核心议题。

---

### 🔑 4. SEC 7 月三项加密新规同期启动 — CLARITY 法案配套落地进入实操

**[Cryptonomist · SEC crypto exchange July 2026](https://en.cryptonomist.ch/2026/07/08/sec-crypto-exchange-regulation/)**

SEC 2026 年度统一监管议程新增三项加密规则，全部指向 7 月 NPRM（Notice of Proposed Rulemaking），涵盖：（1）代币发行披露标准；（2）经纪商-交易商资本充足与客户资产隔离；（3）加密市场结构修订，特别是 ATS 是否需要注册为交易所。虽然只是"提议"，但 SEC 主席 Atkins 已明确表示三项规则将同期进入 60 日公开征求意见期，与国会正在推动的 CLARITY 法案形成夹击。

对交易所生态影响最直接的是第 (2) 项：如果最终版本要求"客户资产 100% 独立且实时可核验"，Coinbase、Kraken 尚有一定合规缓冲，但离岸系（Binance.US、OKX 美国分部）压力陡增；对 DeFi 侧，如果 (3) 把去中心化前端也纳入 ATS 定义，Uniswap Labs 面临的将不是清算，而是主动注册。

预测市场信号：Polymarket 上"CLARITY 法案 2026 年底前签字"合约本周从 41% 涨到 58%，"SEC 一年内起诉某主流 DEX"合约从 32% 降至 24%——市场判定的方向是"新规通过、老诉讼下架"。

---

### 🔑 5. Bitget Wallet 破亿用户，日活支付超过日活交易 — 加密进入支付基础设施阶段

**[Yahoo Finance · July 10 wallet news](https://finance.yahoo.com/personal-finance/investing/article/bitcoin-and-ethereum-prices-today-friday-july-10-2026-up-nearly-3-since-last-friday-130101171.html)**

Bitget Wallet 本周官宣全球用户破 1 亿，标志性数据是"日均支付活跃用户首次超过日均交易活跃用户"。这在整个加密钱包历史上第一次。背后是稳定币（尤其 USDT/USDC 在拉美与东南亚的商户接入）+ Solana Pay/Base Pay 的组合让支付场景第一次跑通了 UX。

结构性意义：过去五年"crypto = trading"是全行业主流假设，即便 Coinbase、Binance 也把交易列为核心收入。Bitget 数据说明"as-a-medium"的场景终于形成 mass market——如果继续三个月，行业会开始重估钱包类产品的估值倍数（从交易佣金型 → 支付流量型）。

对 Visa/Mastercard 也是暗涌。Mastercard 6 月宣布 Solana Pay 深度集成，Visa 同期在与 PayPal PYUSD 谈直连结算。传统卡组织在做的事情，不是拦截加密支付，而是"把加密支付变成自己交易量的一部分"。

---

### 🔑 6. Solana Alpenglow 定档 H2 与 Ethereum Glamsterdam 同步 — 主网性能军备赛

**[Bitcoin Foundation · Solana updates 2026](https://bitcoinfoundation.org/news/altcoins/top-solana-updates-in-2026-network-upgrades-ecosystem-growth-and-institutional-adoption-trends/)**

Solana 治理确认 Alpenglow 升级将在 2026 下半年上线，最激进指标是把终局性（finality）从当前平均 12.8 秒压到 100-150 毫秒——这基本相当于传统金融清算级别的响应时间。同期 Ethereum Glamsterdam（H1 2026 完成）已实现并行执行，Hegota（H2 2026）将上 Verkle Trees，路径是抗审查 + 状态压缩。

两条路径的对比越来越清晰：Solana 走"单链最大化性能"，Alpenglow 后 L1 就是最终形态；Ethereum 走"L1 稳态 + L2 高吞吐"，Glamsterdam 让 L1 到 10k TPS，L2 目标百万 TPS。Base、Avalanche、Sui 都在跟进类似升级窗口。

对开发者与机构：**性能不再是差异化，而是入场券**。真正拉开差距的是应用生态（Solana 强于交易+支付，Ethereum 强于稳定币+RWA+机构基础设施）和监管友好度（美国资金正在向 SEC 明确表态过的资产集中）。2026 H2 会是"性能对齐后叙事重新分化"的关键窗口。

---

## 市场脉搏

**主要资产快照（UTC 2026-07-12 上午）**

- BTC：约 **$63,050**，周涨 **+2.8%**，24h +0.7%；关键阻力 $65,000（前高），支撑 $60,500
- ETH：约 **$3,420**，周涨 **+2.7%**，24h +1.1%；受 ETH ETF 资金推动，关键阻力 $3,600
- SOL：约 **$148**，周涨 **+5.4%**；Alpenglow 定档 + Grayscale HYPE ETF 推进带来 alt 集体走强
- Total Market Cap：**$2.42T**，恢复到 6 月中旬水平

**技术与情绪**

- Fear & Greed Index：**58（Greed）**，从上周 42（Neutral）反弹
- BTC 现货 ETF 累计持仓 **$121B**（Farside），单周净流入 $180M
- ETH 现货 ETF 累计持仓 **$18.4B**（SoSoValue），单周净流入 $310M
- 永续资金费率：BTC 0.008%，ETH 0.011%，未出现杠杆过热
- Polymarket 关键合约：CLARITY 法案 2026 签字 **58%**（+17pp），Fed 7 月降息 **34%**（+9pp）

**未来一周关注点**

- 美国 6 月 CPI 数据（周三）
- Fed 主席讲话（周四）
- ETH ETF 净流入是否继续 $50M+/日节奏
- 更多 GSE 是否跟进 Fannie Mae 的加密抵押品清单
- SEC 三项加密规则文本正式发布时间

---

*数据来源：CoinDesk、The Block、Yahoo Finance、Cryptonomist、Bitcoin Foundation、Farside、SoSoValue、Polymarket。价格与流量数据抓取时间 UTC 2026-07-12。*
