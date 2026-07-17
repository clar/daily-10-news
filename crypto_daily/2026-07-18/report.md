# Crypto 每日资讯 · 2026-07-18

## 今日焦点

> **中东局势压低 BTC/ETH · Visa 亲自下场发稳定币平台 · Ostium 被 oracle 攻击 2200 万 · Circle × Fireblocks 打包机构 USDC · FATF 点名"抗冻结稳定币"**
>
> - **BTC 跌破 $63,000、ETH 跌到 $1,832**：美伊冲突第 6 天，风险资产集体避险。
> - **Visa Stablecoin Platform 上线**：把银行/金融科技/加密公司的稳定币铸造 & 结算全托到 Visa 环境里。
> - **Ostium 永续 DEX 被"未来时间预言机"攻击**：损失 $18-22M，暂停交易。
> - **BlackRock IBIT 单日 $209.4M 流入**：结束 8 周连续净流出，$8.2B 卖压止住。
> - **FATF 报告：犯罪集团开始自铸抗冻结稳定币**，监管口径将全面收紧。

---

## 热门新闻速览

| # | 标题 | 分类 | 要点 |
|---|------|------|------|
| 1 | **BTC 跌破 $63,000、ETH 跌到 $1,832** | 行情 | 美伊冲突 6 天避险 |
| 2 | **Visa Stablecoin Platform 正式发布** | 生态 | 银行 & 金融科技一键铸稳定币 |
| 3 | **Ostium 永续 DEX 遭 $18-22M oracle 攻击** | 安全 | 未来时间预言机数据欺骗 |
| 4 | **BlackRock IBIT 单日流入 $209.4M** | 机构 | 结束 8 周连续净流出 |
| 5 | **Circle × Fireblocks 打包 USDC + Gateway** | 机构 | 面向机构的策略化 USDC 通路 |
| 6 | **FATF 报告：犯罪集团自铸抗冻结稳定币** | 监管 | 稳定币立法或全面提级 |
| 7 | **DefiTuna Lending 被盗 $580K** | 安全 | Solana 借贷池窟窿 |
| 8 | **Citadel Securities 4 亿投 Crypto.com 估值 $20B** | 机构 | 华尔街做市巨头下场 |
| 9 | **韩国推第二版加密资产监管框架** | 监管 | 亚洲 MiCA 加速对标 |
| 10 | **ETH ETF 单日流入 $58.34M（全来自 BlackRock ETHA）** | 机构 | ETH 现货 ETF 稳态 |
| 11 | **Sony 稳定币 SLST 面向日本电商上线** | 采用 | Web2 巨头进圈 |
| 12 | **L2 TVL 破 $52B，Base+Arbitrum 占 80%** | 技术 | L2 集中度提升 |

---

## 重点点评

### 🔑 1. Visa Stablecoin Platform 上线 — 稳定币的"发卡组织"正式登场

Visa 昨日官宣 **Visa Stablecoin Platform (VSP)**，把银行、金融科技和加密公司的稳定币铸造 / 转账 / 管理整合到 Visa 托管环境中。首批合作方包括 BBVA、Standard Chartered 等银行，用户不必自建预言机 / 结算路径，也不必与 Circle / Tether 单独集成。VSP 底层用 Visa Direct 网络做即时结算，前端提供 SDK + API，官方文案强调"面向 60 亿张 Visa 卡的分发能力"。

这一步的战略含义比它的技术方案本身重要得多。**Visa 不是要发一个稳定币，而是要成为稳定币世界的"发卡组织"**——就像它在信用卡时代做的一样，做规则、做清算、做品牌，不做发行。这直接对准了 Circle 的市场：过去 USDC 的机构 onboarding 一直是"银行走 Circle、Circle 走链"，现在 Visa 说"直接走我"。Circle 昨天与 Fireblocks 的合作可以视为对该压力的第一反应。

对市场的直接影响：**中小稳定币的发行门槛可能被 Visa 拉低两个数量级，但机构侧的清算话语权更集中**。这与 FATF 今天点名"犯罪自铸稳定币"形成一对镜像——去中心化侧越松散，中心化侧越强大。接下来 6 个月值得关注 Mastercard 是否跟进类似产品、以及美国 GENIUS Act 立法进程中 Visa/Master 是否被写入清算白名单。

---

### 🔑 2. Ostium 被"未来时间预言机"攻击 — DeFi 老 bug 换新皮肤

Ostium 是 Arbitrum 上的永续合约 DEX，昨晚被利用一个 "**PriceUpKeep forwarder**" 授权漏洞：攻击者用一个已注册的合法 forwarder，向合约提交**带未来时间戳的价格报告**，协议默认信任其为 authorized，从而以"错时价格"开仓 / 平仓，把流动性池中的资金以虚假利润提走。损失区间在 $18-22M，Ostium 已暂停所有交易并披露审计报告更新。

这个漏洞的老套之处在于"信任已注册身份就绕过时间约束"——过去两年在 Chainlink 生态类似案例已出现三次，但每一次都被简单归因"protocol 自身错"，很少有人系统地做**"authorized reporter × 时间戳一致性"**的静态检查。Ostium 事件说明**"预言机安全"这个话题从来没有真正被 DeFi 通用地解决**，只是对特定协议做了一次补丁。

对操作端的启示：**用户在参与永续 / 借贷 DEX 时，应该主动查看协议是否公开 forwarder 白名单，以及是否有 "报告时间戳 - 当前时间" 的 delta 校验**。2026 的 DeFi 已经进入"能不能穿越信任而不是能不能上 leverage"的下半场。

---

### 🔑 3. BlackRock IBIT 单日 $209.4M — 8 周流出止住了吗？

BTC ETF 从 2 月起出现罕见的 8 周连续净流出（累计 $8.2B），全年 ETF 从"2024 年 +50 万 BTC 净流入"翻转到"2026 年至今 -12 万 BTC 净流出"。这一势头在 7 月初出现拐点：连续 3 个交易日净流入合计 $510M，其中 BlackRock IBIT 7 月 6 日单日 $209.4M 领跑。这是市场从"机构 rebalance"回到"机构增配"的可能信号。

但要谨慎解读："止住"不等于"反转"。ETH 现货 ETF 昨日单日 $58.34M 净流入全部来自 BlackRock ETHA，说明**目前进场的边际资金依然高度集中在 BlackRock 一家**，而 Fidelity FBTC、Bitwise BITB 等本周依然是净流出。**这是 BlackRock 单点回补，还是全面机构回归**，看下周三大 ETF 的三日均值是否同步转正才能判断。

宏观侧，昨日美 CPI 温和 + 中东避险两个对立力量并存，机构侧显然更看重 CPI 与降息前景。若下周 FOMC 前 IBIT 单日流入维持 $150M+ 水位，那本轮从 $58k → $63k 的回踩基本可以定性为 "第 8 周流出末端 + 机构低吸"。

---

### 🔑 4. FATF 报告点名"抗冻结稳定币" — 稳定币立法要提速

金融行动特别工作组（FATF）在昨日发布的 2026 年虚拟资产洗钱报告中首次点名——**"部分犯罪网络已经开始自行发行稳定币，专门设计成不可冻结、不可扣押"**。这一表述有明显针对性，业内人士普遍猜测指的是几款近半年内在东南亚 / 中东灰产链条使用的低知名度 stablecoin。

这条报告的政策含义远大于案件本身：**它给美国 GENIUS Act、欧洲 MiCA 稳定币子条例、香港 SFC 稳定币牌照的"三合一"审议方向提供了 FATF 层级的合规压力**，稳定币发行方将被要求实现"链上可冻结、可追溯"作为发行前置条件。这对 Tether 是显性利空（USDT 冻结机制多次被批评滞后），对 Circle、PYUSD 等已经嵌入 traditional compliance 栈的稳定币是相对利好。

值得关注的是 **Visa Stablecoin Platform 的时机**——恰好在 FATF 报告发布同一周。可以合理猜测这个平台的合规框架已经与 FATF / OFAC 有前置沟通，其"链上可冻结、可 KYC 溯源"能力将成为下一阶段稳定币竞争的第一优先事项。

---

### 🔑 5. Circle × Fireblocks — 机构 USDC 通路补齐最后一环

Circle 昨天与 Fireblocks 官方合作，将 **Circle Payments Network + Gateway** 与 Fireblocks 的机构级政策控制 / 多签保管 / 合规工作流打包供机构使用。以往机构做 USDC 结算必须"Circle API + 独立自建保管"，现在 Fireblocks 一次接入即可获得两者能力。

这一步是 **Circle 应对 Visa Stablecoin Platform 的应急动作**。Visa 想吃"银行 & 金融科技侧"的稳定币入口，Circle 就必须把"高净值机构 & 加密原生金融机构"的入口牢牢锁死。Fireblocks 恰好是这条链上的行业事实标准——覆盖 2000+ 家机构客户，是过去两年 USDC 机构侧最重要的分销伙伴。

对 DeFi 侧的意义：Circle Payments Network + Fireblocks Policy Engine 组合，让机构可以直接把 USDC 送进 Aave/Compound/Maker 等协议，同时保持 KYC/AML 记录不断链。这是**"机构 DeFi"落地的重要一里程**——过去这个方向被反复讨论，但没有一站式方案。Circle 这次是把碎片拼起来。

---

### 🔑 6. Citadel Securities $400M 投 Crypto.com 估值 $20B — 华尔街做市巨头正式下场

Citadel Securities（不是 Citadel Hedge Fund，而是 Ken Griffin 旗下负责美国 25% 股票流量的做市巨头）宣布向 Crypto.com 战略投资 $400M，估值 $20B。这笔投资是 Citadel 在加密领域近 5 年最大动作，且明显不是财务投资——**Citadel 会为 Crypto.com 提供做市与流动性支持**。

这个信号有两层：**一，做市侧终于开始严肃看待加密交易所**。过去两年 Citadel 一直在 crypto 上做少量试水，这次直接锁定 Crypto.com 意味着 Citadel 内部风控与合规完成了从"experimental"到"business line"的过渡。**二，Crypto.com 拿到 Citadel 的流动性 = Coinbase 之外第一个具有严肃机构做市支持的美国零售 CEX**。

对市场结构的影响可能是：Crypto.com 在美国 spot 市场的价差可能被压到 Coinbase 水平以下（Citadel 的流动性 + Crypto.com 的成本结构），进而挤压 Binance.US、Kraken 的美国零售份额。这是 US 现货交易所战争进入下半场的关键节点。

---

## 市场脉搏

**核心资产快照：**
- **BTC**: $62,800（24h -3.2%），跌破 $63k 关键支撑，下一个关键位 $60k / $58k
- **ETH**: $1,832（24h -2.8%），$1,800 是 200-day MA，跌破则打开 $1,650 空间
- **SOL**: $137（24h -4.1%），DefiTuna 事件情绪拖累
- **总市值**: 约 $2.15T（24h -3.0%）
- **稳定币总市值**: $178B，USDT / USDC 依然占比 82%
- **DeFi TVL**: $79B（ETH+L2 占 63-68%）

**衍生品与情绪：**
- BTC 永续合约资金费率 -0.005% ~ 0.008%，接近中性偏空
- ETH 永续 OI 环比 -6%，杠杆持仓被清洗
- Fear & Greed Index: **32 (Fear)**，从月中 45 (Neutral) 快速下滑
- 隐含波动率 DVOL: BTC 55, ETH 68，比 6 月低 20-30%

**关键技术位（周线）：**
- BTC：$60k 是过去 3 个月的水平支撑；跌破则 $58k / $55k 成短期目标
- ETH：$1,800 = 200-day MA + 3 个月区间底；破位后无明显中期支撑到 $1,650
- 总山寨市值：跌破 $600B 短期需谨慎

**下周关注：**
- 7/22 白宫 AI/加密监管一揽子闭门吹风（预期 GENIUS Act 时间表更新）
- 7/24 BlackRock 2026 Q2 财报（IBIT 净流入细节）
- 中东局势升级 / 缓和的每周窗口——Strait of Hormuz 是否重开决定原油与风险资产联动方向
