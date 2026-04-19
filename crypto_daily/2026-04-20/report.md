# 加密日报 · 2026-04-20

## 今日焦点

> **Kelp DAO 被盗 2.93 亿美元创年度最大 DeFi 黑客事件 · BTC 三探 $75K 支撑 · ETF 仍在吸金但市场情绪进入"恐惧" · SEC/CFTC 框架进入落地期 · Solana 稳定币流转单月近万亿美金**
>
> - **Kelp DAO 被榨干 $293M**：跨链桥漏洞 + 无背书 rsETH 铸造，接过 Drift 成为 2026 年最大 DeFi 黑客
> - **BTC 徘徊 $75K 附近**：五天内第三次测试该支撑位，市值 $2.62T，Fear & Greed 跌至 27
> - **IBIT 4 月 17 日单日 +$284M**：即使市场走弱，BlackRock IBIT 仍继续吸金，ETF 已累计净流入 $53B
> - **SEC 公布加密资产分类解读**：Atkins 主席"清晰画线"，代币正式分为数字商品 / 收藏品 / 工具 / 稳定币 / 数字证券
> - **Solana 月度稳定币转账接近 $1T**：稳定币余额突破 $11B，成为全球第三大稳定币链

---

## 热门新闻速览

| # | 标题 | 分类 | 要点 |
|---|------|------|------|
| 1 | **Kelp DAO 跨链桥被利用，损失约 $293M** | 安全 | 无背书 rsETH 铸造后抵押 Aave，40 余分钟完成提款 |
| 2 | **BTC 三探 $75K 支撑，市值回到 $2.62T** | 行情 | Fear & Greed 27，ETH/BTC 5 天下跌 2.5% |
| 3 | **IBIT 4 月 17 日单日净流入 $284M** | 机构 | Morgan Stanley MSBT 首周 $14.9M，累计 ETF 净流入破 $53B |
| 4 | **SEC + CFTC 发布联合加密资产分类解读** | 监管 | 依照 3 月 11 日 MOU 协同划线 |
| 5 | **Solana 单月稳定币转账接近 $1 万亿美元** | 生态 | SOL 报价 $84.80，Q1 链上经济活动破 $1T |
| 6 | **12 家 DeFi 协议 20 天内被黑 $605M** | 安全 | 76% 损失源自基础设施级攻击（私钥 / 前端 / 社工） |
| 7 | **BlackRock 质押 ETH ETF 首日吸金 $155M** | 机构 | 3 月 SEC/CFTC 明确质押不构成证券发行 |
| 8 | **ETH 质押量突破 3700 万枚（>30% 流通）** | 技术 | 年化 APR 约 3–4%，机构化程度继续上升 |
| 9 | **Ethereum Glamsterdam 升级目标 2026 年中** | 技术 | blob target 从 3 提至 6，max 9；PeerDAS 上线 |
| 10 | **Morgan Stanley 自营 Bitcoin ETF 上线** | 机构 | 首周 +$14.9M，投行自发产品开始进入 ETF 战场 |
| 11 | **Drift 事件被 Elliptic / TRM 归因朝鲜 DPRK 黑客组织** | 安全 | 手法与 Lazarus 过去行动高度一致 |
| 12 | **Bitwise 预测 2026 年 100+ 新加密 ETF 上线** | 监管 | 通用上市标准落地后 ETF 发行节奏将翻倍 |

---

## 重点点评

### 🔑 1. Kelp DAO $293M 被黑 —— 从 Drift 到 Kelp，DeFi 基础设施的"三周流血季"

2026 年 4 月 19 日 Kelp DAO 因跨链桥漏洞被盗约 2.93 亿美金，一举刷新了仅 18 天前 Drift Protocol $285M 保持的"年度最大 DeFi 黑客"纪录。攻击者通过 bridge 漏洞铸造了无真实背书的 rsETH，再将这些"凭空造出来的"代币作为抵押品存入 Aave，完成了一轮纯合成头寸套现。([CoinDoo](https://coindoo.com/the-biggest-defi-hack-of-2026-293-million-gone-in-46-minutes/) · [Blockchain.News 汇总](https://blockchain.news/news/12-defi-protocols-hacked-drift-exploit-april-2026))

从 4 月 1 日 Drift 到 4 月 19 日 Kelp，20 天内已经有 12 家 DeFi 协议合计损失 $605M 以上，其中约 76% 来自"基础设施级攻击"——私钥被盗、前端被劫持、Solana "durable nonces" 被滥用让 Security Council 预签名等手法成为主流。这与 2022-2024 年那波"智能合约重入漏洞"完全不同：攻击面上移到了团队运维层，代码审计救不了这些项目。

这个趋势最危险的地方在于：Kelp 的问题出在跨链桥，而跨链桥正是 LST/LRT 和再质押协议的核心。一旦市场意识到任何 rsETH / eETH / PufETH 的 1:1 挂钩都可能被桥端攻击打破，整类资产都会面临折价和连环流动性问题。

**值得关注的下一步：** Aave 如何处理这批问题抵押品（清算或冻结？）、其他 LRT 协议是否会被挤兑、以及 DPRK 关联组织是否会在下周继续输出下一个目标。

---

### 🔑 2. BTC 三探 $75K —— 恐惧指数 27，却没浇熄机构资金面

比特币本周三次测试 $75,000 支撑位，市值缩水到 $2.62 万亿美元、Fear & Greed Index 跌到 27 的"恐惧"区间，ETH 在同一时间表现更弱，无法承接任何避险资金。([Blockchain Magazine](https://blockchainmagazine.net/crypto-market-today-2026-04-19/))

但一个反常信号是：即使在这一轮回调中，IBIT 4 月 17 日仍然净流入 2.84 亿美元，累计 ETF 净流入站稳 $53B。Morgan Stanley 自营的 MSBT 甚至在这样的市况下选择首发并拿到 $14.9M 首周流入——机构端并没有随零售情绪走。([The Block](https://www.theblock.co/post/396499/bitcoin-etfs-largest-day-inflow-six-weeks) · [CoinDesk](https://www.coindesk.com/markets/2026/04/07/bitcoin-etf-inflows-hit-highest-level-since-february))

这种"情绪恐惧 + ETF 持续吸金"的背离，和 2024 年 9 月那次非常像：彼时恐惧指数跌到 30 以下、BTC 在 $55K 震荡，但 ETF 净流入一直维持。本轮如果 $75K 最终守住，接下来的反弹斜率可能很陡，因为空头+情绪都已先行耗尽。

**值得关注的下一步：** 若 $75K 失守，量价共振概率极高，$70K 附近是下一条关键防线；反之，任一单日 +$500M 级 ETF 流入就足以撬动短期反转。

---

### 🔑 3. SEC/CFTC 联合分类 —— 美国加密市场第一次有了"法律坐标系"

3 月 11 日 SEC 与 CFTC 签订 MOU 之后，两家监管机构本月联合发布了一份综合性法律解释，把加密资产清晰地划分为：数字商品（commodity）、数字收藏品（NFT 主流部分）、数字工具（utility-like）、稳定币、数字证券五类。主席 Paul Atkins 说"这就是监管机构该做的——用清晰的话划清晰的线"。([SEC 官方](https://www.sec.gov/newsroom/press-releases/2026-30-sec-clarifies-application-federal-securities-laws-crypto-assets) · [The Block 分析](https://www.theblock.co/post/383241/crypto-regulation-2026-sec-ambitious-agenda-empowered-cftc))

这份解读第一次正式把 ETH 归入"数字商品"并明确质押不构成证券发行，直接给 BlackRock 的质押版 ETH ETF 铺了路，该产品首日即吸金 $155M。现货 + 质押 ETF 的合流意味着 ETH 的机构配置叙事正式升级为"带息资产"。

更深远的是 ETF "通用上市标准"带来的发行效率变化：Bitwise 预测 2026 全年将有超过 100 支新加密 ETF 上线。对市场是结构性利好，但对发行方是红海——预计 80% 新产品资产规模将低于 $50M。

**值得关注的下一步：** CLARITY Act 签署进度、Solana / XRP / LTC 等下一批现货 ETF 是否被接受、以及以"质押 + 分类"做前提的复合策略 ETP 产品。

---

### 🔑 4. Solana 月度稳定币转账逼近 $1 万亿 —— L1 叙事重新回到 SOL 手里

Solana 月度稳定币流转接近 $1T、稳定币总余额突破 $11B 并成为全球第三大稳定币网络；Q1 链上经济活动整体突破 $1T。([Symbiosis 行业报告](https://symbiosis.finance/blog/ethereum-ecosystem-in-2026-what-changed-in-defi))

这些数字放在 SOL 今天 $84.80、下跌 3% 的价格表现旁边非常有意思：基本面数据持续走强，但资金在本轮回调里选择先 de-risk altcoin。历史上 Solana 的价格和链上稳定币转账相关性很高，当前折价意味着一旦 BTC 企稳，SOL 的修复力度可能高于 ETH。

值得担忧的是，Drift 事件让"Solana 上的 DeFi 安全"这个议题再度被放大。尽管稳定币转账本身不依赖具体协议合约，但如果未来 12 周 Solana 上再发生一次 $100M 级事故，生态主叙事就会被再次打回 2023 年的"快但脆弱"定位。

**值得关注的下一步：** Jito、Jupiter、Raydium 等核心协议的安全治理公告，以及 Firedancer 主网化进度能否在 Q2 如期落地。

---

### 🔑 5. LRT 板块的系统性风险 —— Kelp 事件可能只是开始

Kelp DAO 被黑的方式——在跨链桥漏洞下直接铸造 rsETH 抵押 Aave——揭示了 Liquid Restaking Token (LRT) 赛道的核心风险：这类资产的"价值"完全依赖多层链间保证（L1 质押 → LST → 桥接 → LRT），任何一层失败都会击穿挂钩。

当前 LRT 赛道 TVL 仍超过 $20B，其中 EtherFi、Renzo、Kelp、Puffer 占据主要份额。Kelp 出事后，Aave、Morpho、Silo 等把 rsETH 列为抵押品的借贷协议必须立刻重新评估这类资产的 LTV 参数，否则会出现"抵押品本身归零但债务仍在"的坏账。

更结构化的问题是：机构端通过 ETF 获得 ETH 敞口之后，大量"想要额外收益"的需求原本会下沉到 LRT 板块。Kelp 事件很可能把这条路径至少堵上 3-6 个月，机构的"收益增强"需求被迫回流到 BlackRock 质押 ETF 这类更保守的产品。

**值得关注的下一步：** Aave 治理提案动向、ETH LRT TVL 变化曲线、以及 EigenLayer 官方是否会介入提出统一的 LRT 风险参数框架。

---

## 市场脉搏

**主流资产行情（2026-04-19 收盘附近）：**
- **BTC：** ~$75,200（24h -1.8%）· 关键支撑 $75K / $70K，阻力 $80K
- **ETH：** ~$2,310（24h -2.5%）· 关键支撑 $2,280–$2,300，阻力 $2,500
- **SOL：** ~$84.80（24h -3.1%）· 关键支撑 $80–$82，阻力 $95
- **总市值：** $2.62T（近 5 日缩水约 4.6%）

**情绪与结构指标：**
- **Fear & Greed Index：** 27（Fear）· 跌破本月均值 38
- **BTC 永续 funding rate：** 多数交易所回落至 0.003%/8h 附近，中性偏空
- **ETH/BTC ratio：** 3 个月新高后回落，短期仍由 BTC 主导节奏
- **ETF 累计净流入：** $53B（IBIT 占近 60%，FBTC 居次）

**下一周关注：**
1. Kelp DAO 事件处置与 LRT 板块 TVL 变化
2. BTC $75K 支撑是否守住，周度收盘位置至关重要
3. BlackRock 质押 ETH ETF 本周流入节奏
4. CLARITY Act / 下一批现货 ETF 的审批进度
5. 是否出现第 13 起 DeFi 协议被黑事件

**风险提示：** 本报告所有价格、流入、TVL 数据来自公开资讯，仅供研究用途，不构成投资建议。
