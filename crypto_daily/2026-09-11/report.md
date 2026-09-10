# 加密日报 · 2026-09-11

## 今日焦点

> **CLARITY 关键投票倒计时 · BTC 跌破 $78K · Trezor 采纳 ERC-7730 · Term Labs "$951 抢下 $8.5M" 治理攻击 · Fusaka 升级临近**
>
> - **BTC 开盘 $78,291，日内跌至 $77,941**，创本周新低，等待 CPI/PPI 数据。
> - **9 月 15 日参议院 CLARITY Act 讨论程序投票**，Polymarket 通过率跌至 16%。
> - **Trezor 全线支持 ERC-7730**，终结硬件钱包"盲签"顽疾。
> - **Term Labs 治理攻击**：攻击者花 $951 拿下投票权，卷走 $8.5M。
> - **本周 BTC ETF 净流入 $986.9M**，山寨币 ETF 流入锐减 73-96%。

---

## 热门新闻速览

| # | 标题 | 分类 | 要点 |
|---|------|------|------|
| 1 | **BTC 跌破 $78K、ETH 失守 $2,470** | 行情 | 等待 CPI/PPI，日内继续下探 |
| 2 | **参议院 9/15 就 CLARITY Act 举行 cloture 投票** | 监管 | 需 60 票；Polymarket 概率 16% |
| 3 | **BTC 现货 ETF 单周净流入 $986.9M** | 机构 | 环比 +6.7%，山寨 ETF 骤降 73-96% |
| 4 | **Trezor 采纳 ERC-7730 结束"盲签"** | 技术 | 硬件钱包首次原生解析 EIP-712 payload |
| 5 | **Term Labs 治理攻击：$951 拿下 $8.5M** | 安全 | 攻击者接管治理，抽干 6 个金库 |
| 6 | **SEC "Regulation Crypto Assets"进入公众评议** | 监管 | 8 月 18 日发布，明确投资合同框架 |
| 7 | **DeepSeek 传出赴上海 STAR 板 IPO**（$74.5B 估值） | 行业 | 中国 AI 影响加密+算力叙事 |
| 8 | **Fusaka 主网升级窗口临近** | 技术 | 引入 PeerDAS 和 EIP-7742 |
| 9 | **Base 中位交易费 $0.02，L2 费用继续下探** | 生态 | Base < OP < Arbitrum < zkSync < Scroll |
| 10 | **稳定币 GENIUS 法后市场结构未定** | 监管 | 稳定币收益/伦理条款仍是最大变数 |
| 11 | **DeFi 累计年内被盗超 10 亿美元** | 安全 | 治理、Oracle、跨链桥仍是主战场 |
| 12 | **Circle USDC 因 Drift 事件面临"是否冻结"追问** | 行业 | 稳定币可编程性再被讨论 |

---

## 重点点评

### 🔑 1. CLARITY Act 9/15 关键投票 — "两年立法窗口"最后 72 小时

参议院将在 9 月 15 日下午 2:15（ET）就 CLARITY Act（Digital Asset Market Structure Clarity Act）举行 cloture on motion to proceed 投票，需要 60 票才能进入正式辩论。众议院早在 2025 年 7 月已以 294-134 通过 H.R. 3633，但参议院被三个议题卡住：涉及 Trump 家族 14 亿美元加密收入的伦理条款、Section 604 的 DeFi 开发者责任、以及威胁 Coinbase USDC 13.5 亿美元奖励收入的稳定币收益条款。

Polymarket 上"2026 年内通过"概率已从 2 月的 82% 崩至 9 月 6 日的 16%，Galaxy Research 更给出 10%。**如果 9/15 未通过 cloture，整个"CLARITY + 稳定币 GENIUS 法配套"框架有可能被推到 2027 年**，届时监管真空将持续给交易所、DeFi 协议、稳定币发行方带来经营不确定性。

来源：[Motley Fool](https://www.fool.com/investing/2026/08/22/senators-plan-a-clarity-act-vote-on-sept-15/) · [Bitget Academy](https://www.bitget.com/academy/clarity-act-vote-september-2026-senate-cloture-what-to-know)

---

### 🔑 2. BTC 跌破 $78K、ETH 跌破 $2,470 — 数据周前的仓位再平衡

BTC 周四开盘 $78,291.64、盘中回落至 $77,941.56；ETH 开盘 $2,467、跌至 $2,464.92。两者创本周新低，节奏与今晚（美东）PPI 和明晚 CPI 数据高度相关——下周二起 FOMC 开始为期两天的利率会议，这套数据将决定 9 月是否有 50 bp 的降息可能。

值得留意的是**现货 ETF 端资金仍在净流入**：BTC 现货 ETF 上周净流入 $986.9M，环比 +6.7%；但山寨币 ETF（SOL、DOGE、ADA 等）净流入下降 73-96%。这种"BTC 与山寨 ETF 分化"意味着机构选择在 Q4 前继续压注 BTC，而对山寨的 ETF 化叙事已经明显冷却。

来源：[Yahoo Finance](https://finance.yahoo.com/personal-finance/investing/article/bitcoin-and-ethereum-prices-today-thursday-september-10-2026-crypto-prices-slide-back-with-inflation-data-on-tap-113018195.html) · [Altcoin Buzz](https://www.altcoinbuzz.io/bitcoin-etf-inflows-altcoin-etf-demand-september-2026)

---

### 🔑 3. Trezor 支持 ERC-7730 — 硬件钱包"盲签时代"终结

9 月 8 日，Trezor 官方宣布全系硬件钱包升级支持 ERC-7730 —— 一份由 Ledger 团队主导、Ethereum 社区共同制定的"结构化签名标准"。这套标准允许钱包直接展示 EIP-712 payload 中的字段含义（例如"授权 Uniswap Router 代花费 xxx USDC"），而不是仅显示一串十六进制哈希，让用户不必再"盲签"任何交易。

这次升级的重要性远不止硬件钱包体验。**近两年 DeFi 大额被盗案里，超过 40% 来自"盲签 permit / approve"**，包括今年 3 月 Resolv、7 月 Allbridge、8 月 Term Labs。ERC-7730 从格式层解决了这个问题，如果 Ledger、GridPlus、Keystone、SafePal 全线跟进，"钓鱼式 approve"这类攻击面将大幅收窄。

来源：[Ethereum ecosystem in 2026 - Symbiosis blog](https://symbiosis.finance/blog/ethereum-ecosystem-in-2026-what-changed-in-defi)

---

### 🔑 4. Term Labs 治理攻击 — $951 撬动 $8.5M，DAO 安全模型再敲警钟

8 月 23 日 Term Labs 被曝治理接管攻击，攻击者仅花 $951 就买到足以控制 4 个 USDC 策略金库 + 91% ETH Meta Vault 治理权重的代币，通过一份"看起来平常的提案"关闭金库交易延时，然后一次性提走 2,841.74 WETH + 1,679,639 USDC（约 $8.5M）。到 9 月初 Term Labs 才逐步收回大部分 fixed-rate 头寸。

**根源在于 Term 的治理设计**：投票权不与金库存款直接绑定，用户需要主动将 vault shares 包装成治理代币，而绝大多数用户没做这一步，导致市场上流通的治理代币极少、买断成本极低。这不是一个孤立事件——今年以来 Compound、Curve、Balancer 都出现过类似治理攻击面警告，DeFi 治理必须重新审视"低流通治理代币 = 高攻击面"这一结构性问题。

来源：[Crypto.news](https://crypto.news/term-labs-dao-governance-heist-951-dollars-8-5-million-exploit/) · [CoinPaper](https://coinpaper.com/34627/term-finance-exploit-how-85-million-was-drained-from-defi-vaults)

---

### 🔑 5. Fusaka 升级窗口临近 — L2 费用"再打骨折"的关键催化剂

以太坊 Fusaka 主网升级（EIP-7594 PeerDAS + EIP-7742 blob 独立计数）计划在 Q4 主网上线，是继 Dencun (Cancun-Deneb) 后规模最大的一次数据可用性提升。PeerDAS 让 L2 数据发布带宽再上一个量级，EIP-7742 允许 blob 数量与 gas 目标解耦，被 L2 团队视为"下一次 100 倍降本"的前提。

参照 Dencun 后 Base 中位费用从 $0.09 降到 $0.02、Arbitrum 从 $0.15 降到 $0.04 的历史，Fusaka 后 L2 的极限费用有望进入"低于稳定币转账手续费"区间。**这将彻底改变支付、消费者应用、稳定币零售**的经济模型——尤其是与 GENIUS 法后的持牌稳定币结合，加密支付有望在 2027 年真正打入 Visa / Mastercard 的费率区间。

来源：[Bitcoin Foundation - Major Ethereum Updates 2026](https://bitcoinfoundation.org/news/ethereum/major-ethereum-updates-2026-overview-protocol-upgrades-and-strategic-roadmap/)

---

## 市场脉搏

- **BTC**: $77,941（-0.5% 24h），关键支撑 $76,500 / $74,000；上方压力 $80,500。
- **ETH**: $2,464（-0.8% 24h），$2,400 是本周关键防守位；上方压力 $2,560。
- **BTC 现货 ETF**: 本周净流入 $986.9M，累计年内净流入维持在历史前列。
- **山寨 ETF**：本周流入 -73% 至 -96%（SOL、DOGE、ADA 主流 5 家聚合）。
- **稳定币总市值**：稳定于 $225B 区间，USDC 占比继续微幅上升。
- **Polymarket 事件概率**：CLARITY Act 2026 内通过 = 16%；Fed 9 月降息 25 bp = 62%。
- **市场情绪**：Fear & Greed Index 落在 42（Neutral 偏 Fear），永续资费率 8h 约 0.005%。

短线关注**今晚 PPI（美东 8:30）+ 明晚 CPI**两个决定 Fed 语调的关键节点，以及**9/15 CLARITY Act 投票**——三个催化剂集中在同一周，本周 BTC/ETH 波动率可能显著放大。
