# 加密行业每日报告 · 2026-07-24

## 今日焦点

> **DeFi "黑客日" 单日损失 3555 万美元 · SEC 批准后 4 小时又叫停 Bitwise 指数 ETF · BTC 在 $66K 附近盘整 · USDC 半年份额升至 70% · 现货 BTC ETF 七连吸金 $981M**
>
> - **AFX Trade 桥被拆走 2400 万美元**，Verus 桥两月内二次被盗，B² Network 升级密钥泄露：**三起事故 24 小时内叠加**。
> - **SEC 上午加速批准 Bitwise 10 Crypto Index ETF、下午发 stay order 撤回**，72 个加密 ETF 申请仍在排队。
> - **BTC $65,658，ETH $1,899**，Grayscale 警告熊市可能延续到 Q4，Fear & Greed 指数偏 Neutral。
> - **USDC 上半年调整后交易量占 70%**，Standard Chartered 成首家 G-SIB 提供直接 USDC 铸赎；Revolut 8 月 31 日 EEA 下架 USDT。
> - **Metaplanet Q2 增持 2,823 BTC**，总持仓 43,000 枚，晋升全球第 3 大企业金库；MicroStrategy 短暂停止购入。

---

## 热门新闻速览

| # | 标题 | 分类 | 要点 |
|---|------|------|------|
| 1 | **DeFi "Hackers' Day" 单日损失 $35.55M** | 安全 | AFX $24M、Verus $7.54M、B² $3.86M 三连爆 |
| 2 | **SEC 加速批准 Bitwise 10 Crypto Index ETF 后又撤回** | 监管 | 上午通过，下午 stay，72 个 ETF 等待 |
| 3 | **BTC 现货 ETF 七日累计流入 $981M** | 机构 | 7/23 净流入 $69M，BTC 徘徊 $66K |
| 4 | **USDC 上半年占稳定币调整交易量 70%** | 生态 | H1 总量 $8.82T，6 月单月创 $1.79T 记录 |
| 5 | **Standard Chartered 上线 USDC 机构级铸赎** | 机构 | 首家 G-SIB 与 Circle 深度集成 |
| 6 | **Revolut 8/31 起 EEA 下架 USDT** | 监管 | Tether 拒申请 MiCA 授权，欧洲战线全面退守 |
| 7 | **AMD MI455X 亮相：加密算力用户观望** | 行业 | 32 家 AI 云同步公告，加密矿商未列客户 |
| 8 | **Metaplanet 单季买入 2,823 BTC 至 43,000 枚** | 机构 | 均价 $78,872，Twenty One Capital 后成全球第 3 |
| 9 | **Base "Beryl" 硬分叉上线，加入原生代币标准** | 技术 | 提款终局时间缩短，短暂 sequencer 停机 |
| 10 | **Ethereum Glamsterdam 升级测试网活跃** | 技术 | 并行执行 + Block-Level Access Lists |
| 11 | **Solana Alpenglow 进入测试阶段** | 技术 | 目标秒级 finality，验证者简化 |
| 12 | **BNY Mellon 扩展 USDC 托管、铸赎服务** | 机构 | 世界最大托管行 $59T AUM 全面进场 |

---

## 重点点评

### 🔑 1. DeFi "黑客日" 三连爆 —— 桥和多签依然是最薄的一环

**[CoinDesk](https://www.coindesk.com/tech/2026/07/23/bitcoin-ethereum-linked-protocols-lose-usd35-million-in-multiple-attacks-hours-apart)** · **[CryptoTimes AFX](https://www.cryptotimes.io/2026/07/23/cryptos-hackers-day-afx-trade-hit-for-24m-losses-reach-35-55m/)** · **[Verus](https://www.cryptotimes.io/2026/07/23/verus-ethereum-bridge-exploited-again-for-7-54m-in-repeat-attack/)**

Lookonchain 将 7 月 23 日直接命名为 "**Hackers' Day**"：单日 3 起独立事故，累计损失 3555 万美元——**Arbitrum 上 AFX Trade 的第三方桥私钥被盗 $24M、Verus 以太坊桥两个月内二度被同一 import path 攻破 $7.54M、B² Network 因升级权限外泄丢失 $3.86M**。

三起事件几乎都不是"密码学失败"，而是**运维/权限管理失败**——桥密钥、升级密钥、多签阈值。这与本轮牛市中"合约本身越写越安全，但支撑合约的 off-chain 基础设施越拉越松"的老结论一致。Verus 两次被相同攻击载体命中，尤其令人震惊：**这提示第一次事件后的"补丁 + 审计"流程正在被时间压力压垮**。

对交易员而言，三起事件都发生在 Arbitrum 与 Ethereum 桥面上，桥资产的隔夜风险应显著提高。对 DeFi 开发者，**Multichain-style 桥基础设施可能进入下一轮整合/信任收缩期**——本次事件之后，一线机构可能加速转向 CCTP、Wormhole Native Token Transfers 等"由发行方直接背书"的模型。

---

### 🔑 2. SEC 一日之内批准又撤回 Bitwise 10 Crypto Index ETF —— 内部张力浮出水面

**[Bitcoin Foundation](https://bitcoinfoundation.org/news/regulation/us-crypto-approach/)** · **[The Block](https://www.theblock.co/post/383241/crypto-regulation-2026-sec-ambitious-agenda-empowered-cftc)**

SEC 7 月 22 日**加速批准 Bitwise 的 10 币指数 ETF**（含 BTC、ETH、SOL、XRP、DOGE 等），但**几小时后即发 stay order 撤回**——这是本届 SEC 最戏剧化的一次翻脸，公开暴露了委员会内部就"下一代多币指数 ETF"的严重分歧。72 个加密 ETF 申请正在排队，其中包括 Grayscale 的 XRP/SOL/LTC 单币产品、Franklin 的 Solana ETF 等。

Stay order 通常意味着某位委员对批准依据提出程序性异议——**可能来自新任 SEC 委员对"20 天加速批准"程序的原则性反对**，也可能是财政部/白宫层面对"XRP 分类"的最后一刻介入。无论理由是什么，市场对"多币现货 ETF 洪流即将开闸"的定价将被显著推迟。

短期看，这次翻船会让 BTC ETF 继续独享"institutional 流入唯一合规入口"的地位，**巩固 BlackRock IBIT 的资金磁力**；中期看，则暴露了 CLARITY Act 立法窗口未开之前 SEC/CFTC 分工不清的老问题。**关注下周是否有委员公开发表 dissent，那才是真信号。**

---

### 🔑 3. USDC 半年占 70% 交易量 —— 银行阶级选边站，Tether 被推向"离岸"角色

**[CoinDesk](https://www.coindesk.com/business/2026/07/06/circle-s-usdc-is-leaving-tether-behind-in-the-stablecoin-volume-race)** · **[Bankless](https://www.bankless.com/read/news/usdc-extends-lead-over-usdt-to-70-of-volume-in-2026)**

2026 上半年调整后稳定币交易量达 **$8.82T**，其中 **USDC 占 ~70%，USDT 占 ~25%**——完全颠倒了两年前 USDT 8 成、USDC 2 成的格局。6 月单月冲上 $1.79T 历史峰值（同比 +125%）。**关键推手是主流银行的"选边站"**：BNY Mellon 上周开放 USDC 托管+铸赎，本周 Standard Chartered 成为首家提供 USDC 直接铸赎的 G-SIB。

Tether 的战略选择也在同步固化：**拒绝申请 MiCA 授权**，Revolut 已宣布 8/31 在 EEA 全面下架 USDT。这意味着 Tether 正式接受"离岸美元流动性 + 新兴市场支付层"的角色，把机构 DeFi 交易层让给 USDC。

从二级市场角度看，Circle 上市后的估值溢价可能在下半年被这些数据兑现，**IPO 后的 lock-up 到期与业务基本面同步利好可能形成罕见共振**。反过来，稳定币规范化也可能让部分 Yield / 桥接协议失去关键的"USDT 流动性带"，值得追踪。

---

### 🔑 4. BTC 徘徊 $66K + 现货 ETF 七日 $981M 净流入 —— "买盘充足、但没人 FOMO"

**[FXStreet](https://www.fxstreet.com/cryptocurrencies/news/bitcoin-etfs-approach-1b-in-seven-session-inflow-run-202607231000)** · **[Yahoo Finance](https://finance.yahoo.com/personal-finance/investing/article/bitcoin-and-ethereum-prices-today-thursday-july-23-prices-mixed-as-analysts-debate-crypto-bottom-152654561.html)**

BTC 现货 ETF 已经连续 7 个交易日净流入，7 月 14 日以来累计 **$981M**，7 月 23 日单日 $69M——**流入是稳的，但相比 4 月 9 天 $21 亿的爆发式流入，节奏明显更"机构 DCA"化**。BTC 现货价格在 $65K-$66K 反复拉锯，Ethereum $1,899 依旧疲软。

这种"温和吸筹 + 价格不涨"的结构通常出现在**两类叙事同时存在**的时期：多头看好"Q4 降息 + Bitwise 多币 ETF 开闸"，空头则接受 Grayscale 四年周期框架下"熊市持续到 9-10 月"的判断。目前定价接近两派观点的加权中值。

值得关注的是 **funding rate 中性偏低、Fear & Greed Index 稳定在 45-55 中性区**——这在过去 3 年多次成为**中期底部信号**。若下周 SEC 就 Bitwise 事件发布 5-3 或 4-4 分歧的正式意见，可能引发一轮波动突破。

---

### 🔑 5. Metaplanet 43,000 BTC 晋升全球第 3 —— "MicroStrategy 模型"日本化

**[Bitcoin Magazine](https://bitcoinmagazine.com/news/metaplanet-adds-2823-bitcoin-reaches-43000)** · **[CoinDesk](https://www.coindesk.com/markets/2026/07/02/metaplanet-buys-another-usd170-million-of-bitcoin-expanding-treasury-to-43-000-btc)**

Metaplanet Q2 增持 **2,823 BTC**（均价 $78,872，成本 $225M），累计 **43,000 BTC**，成为全球第 3 大企业金库，仅次于 Strategy（847,363 BTC）和 Twenty One Capital。**关键差异是融资结构**：Metaplanet 主要通过信贷额度 + 普通债券 + 期权收入完成购入，避免了 Strategy 早期严重的股票稀释。

Metaplanet 的期权收入业务 Q2 实现 $10.95M 营业收入，**首次证明"BTC treasury + income generation"这套模型可以在非美国司法辖区跑通**。这为韩国、香港、新加坡的上市公司提供了非常清晰的 playbook——2026 下半年可能出现更多亚太 BTC 金库公司。

同期 **MicroStrategy 短暂暂停购入**，与 Metaplanet 的激进形成有趣对比。这可能意味着：**Strategy 已达 4% 总供应上限，进入了以 ATM 换 BTC 而非新增净持仓的稳态；Metaplanet 仍在成长期，通过财务结构创新获得更高杠杆**。中期这条曲线值得追踪。

---

## 市场脉搏

**主要资产价格 (2026-07-23 US 收盘)**：
- **BTC** $65,658 · 24h -0.6% · 总市值 $1.33T
- **ETH** $1,899 · 24h -1.8% · 总市值 $233B
- **BTC 现货 ETF 7 日累计净流入** +$981M（7/23 单日 +$69M）

**核心技术位**：
- BTC：**$64K 关键短期支撑**（4 月 - 6 月多次触及）；上方压力 $68.5K + $72K
- ETH：**$1,850 是本轮周期低点区间**，若失守直指 $1,650；上方压力 $2,050

**情绪 & 结构指标**：
- **Fear & Greed Index：45-55 中性偏保守**
- **BTC 永续 funding rate：低位**，做多情绪未过热
- **稳定币总市值：>$210B**（USDC 主导）

**跨界联动**：**AMD MI455X + Nvidia Spectrum-6 的算力升级**对加密矿业中期利好（能耗单位价格进一步下探），但短期没有直接矿业新客户；**白宫指控 Moonshot 蒸馏 Anthropic Fable** 引发的"美中 AI 脱钩加速"叙事可能间接支撑 BTC 作为跨境结算资产的估值上限。

**下周关键事件**：(1) 美联储 FOMC 会议纪要发布；(2) SEC 就 Bitwise 撤回是否给出说明；(3) 8 月 2 日 EU AI Act 大限日的市场反应；(4) 一批 Q2 加密公司财报（Coinbase 7/31，Robinhood 加密板块）。
