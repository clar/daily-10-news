# 加密货币日报 · 2026-10-24

## 今日焦点

> **BTC ETF 单日入超 5 亿美元 · ETH ETF 相反净流出 · SEC 加密托管提案进入 60 天评议窗口 · DeFi 全年被盗突破 23.4 亿 · GENIUS Act 稳定币监管州级规则落地**
>
> - **BTC Spot ETF 10 月录得近月最大单日流入 $526.7M**（Farside），BlackRock IBIT 独揽 ~$665M，但月度仍为净流出约 $88M。
> - **ETH Spot ETF 同日反向净流出 $103.3M**，ETHA 为主要赎回方。
> - **SEC 批准加密资产自托管/州信托托管提案**，60 天公开评议，RIA 托管结构大改。
> - **DefiLlama 2026 累计被盗金额达 $2.344B / 304 起**，其中最大的 Bitget 9 月被盗 $387M。
> - **美国财政部按 GENIUS Act 发布州级稳定币监管最终临时规则**，各州须在 2028 年 1 月前完成合规认证。

---

## 热门新闻速览

| # | 标题 | 分类 | 要点 |
|---|------|------|------|
| 1 | **BTC Spot ETF 10 月 19 日单日流入 $526.7M** | 机构 | IBIT 独揽 $665M；月累计仍 -$88M |
| 2 | **ETH Spot ETF 同日净流出 $103.3M** | 机构 | ETHA 为主要赎回方 |
| 3 | **SEC 启动加密托管规则征求意见** | 监管 | 允许自托管与州信托托管 |
| 4 | **Treasury 公布 GENIUS Act 州稳定币规则** | 监管 | 2028 年 1 月前完成认证 |
| 5 | **Ledger 10 月 9 日供应链攻击损失 $93M** | 安全 | 前端+基础设施被劫持 |
| 6 | **Qubic 密钥生成缺陷损失 $1.3M** | 安全 | 10 月 17 日披露 |
| 7 | **Gamdom 密钥泄露损失 $4.21M** | 安全 | 基础设施凭据泄漏 |
| 8 | **稳定币总市值回落至约 $308B** | 行情 | 较 5 月峰值 $322B 下滑 |
| 9 | **CLARITY Act 市场结构法案仍滞留参议院** | 监管 | 稳定币奖励条款分歧 |
| 10 | **伊利诺伊州 0.2% 加密税延期至 2027 年 7 月** | 监管 | 待法院批准 |
| 11 | **NYDFS 与怀俄明州签署监管协作备忘录** | 监管 | 跨州数据共享 |
| 12 | **BTC 维持 $112K 附近震荡，ETH 稳于 $4,500** | 行情 | 波动率压低、funding 转负 |

---

## 重点点评

### 🔑 1. BTC/ETH ETF 分化——"机构主力偏 BTC、避 ETH"的信号变得更鲜明

[Cointelegraph / The Block / Farside Investors](https://cointelegraph.com/markets/bitcoin-etfs-ether-etfs-largest-inflow-october)

10 月 19 日的 ETF 数据刻画出一个相当清晰的分化：**BTC 现货 ETF 吸金 $526.7M（本月以来最大单日流入）；ETH 现货 ETF 同日净流出 $103.3M**。BlackRock IBIT 一家就贡献了 $665M 的净流入，而 FBTC 和 GBTC 继续赎回；ETH 这端 BlackRock ETHA 却是最大赎回方。

这是一个关键信号：**配置型资金正在从"BTC+ETH 一起买"回到"只配 BTC"**。原因有三：（1）BTC 上一轮减半后供应曲线已被机构充分建模，而 ETH 的质押收益—通胀—EIP-1559 燃烧的三重机制在当前环境下未被定价为"收益资产"；（2）SEC 对以太坊再质押生态（EigenLayer / LRT）的监管态度仍不明朗；（3）10 月全月 BTC ETF 累计仍是净流出 ~$88M，说明 19 日的大单日反弹并没扭转趋势，更可能是机构基金的季度再平衡窗口。

接下来一周看点：（a）11 月 FOMC 前的两次做市窗口能否推动 ETH ETF 月度回正；（b）BlackRock 是否通过 ETHA 产品引入 staking 收益——这会立刻改变 ETF 的现金流叙事。

---

### 🔑 2. SEC 托管提案——加密 ETF 结构面临首次重大修订

[Chapman On Chain / Akin Gump CryptoLink](https://www.akingump.com/en/insights/newsletters/cryptolink-newsletter-august-2026-updates)

10 月 1 日，SEC 公布加密资产托管规则征求意见稿，关键改动是：**正式允许注册投资顾问（RIA）与注册基金使用"自托管"与"州信托公司"方案**，公开评议期 60 天（从联邦公报登载日算起）。这打破了过去"必须用 Qualified Custodian"的硬性限制。

对资管机构的意义：如果最终规则不走回头路，Fidelity / BlackRock / Franklin 都能把一部分 ETF 资产放进自己的信托子公司或分段放入 Coinbase Custody 之外的替代方案，**定价权和费率结构都将被改写**；对小型基金则意味着可以直接去 Wyoming / South Dakota 的州信托公司申请托管资格。

潜在陷阱：自托管对 ETF 的"合规可审计性"要求会变得极高——SEC 可能通过 Rule 206(4)-7 的"书面合规计划"把审计责任全部压到 RIA 身上。接下来 60 天评议期内，Coinbase Custody / Anchorage 等现有托管商会强烈反对；预计明年初出台的最终规则会在"自托管+第三方证明"方向上折中。

---

### 🔑 3. DefiLlama 2026 累计被盗 $23.4 亿——Bitget 单起 $387M 占比超 16%

[DefiLlama Hacks Tracker](https://defillama.com/hacks)

截至 10 月 20 日，DefiLlama 累计记录 304 起被盗事件，总额 $2.344B——其中 9 月的 Bitget $387M 事件独占 16.5%，10 月 9 日的 Ledger 供应链攻击 $93M 列第二位。Ledger 事件的特殊性在于：**攻击者没有直接攻击 Ledger 硬件钱包的签名链路，而是通过前端供应链（第三方 JavaScript 库）在 WebDapp 环境里偷换交易参数**。

把 2026 全年 vs 2025 对比，有三个结构性变化：
- **CEX 被盗金额超过 DEX / 协议级事件总和**（Bitget $387M + Gamdom $4.21M 等中心化成分占大半），这是 2022 年 FTX 之后首次反转；
- **供应链攻击占比显著上升**（Ledger / 多个前端 CDN 事件），对应的是浏览器钱包与第三方脚本的"动态加载"模式漏洞；
- **DeFi 协议直连漏洞（oracle、重入）占比下降**，说明过去三年 DeFi 协议级安全有真实进步。

安全侧的下一个争议点：**是否要求 CEX 实名披露主要前端依赖的第三方包与 SBOM**。欧盟 DORA + MiCA 已经在往那个方向走。

---

### 🔑 4. Treasury 的 GENIUS Act 执行规则——州级稳定币监管的时间表落定

[Chapman On Chain Spotlight](https://www.chapman.com/assets/htmldocuments/Chapman-On-Chain-Spotlight%E2%80%93100526.pdf)

9 月 30 日，美国财政部发布 GENIUS Act 的临时最终规则：**各州如果要维持本州稳定币发行牌照，必须向财政部证明本州监管框架"实质上等同于联邦标准"**，最晚期限 2028 年 1 月。否则，稳定币发行只能走联邦路径（OCC/Fed/FDIC）。

这个规则的两层含义：
- **短期：Wyoming / New York / Texas 的"稳定币特许"牌照成为稀缺资源**。NYDFS 和 Wyoming 本周签署的 MOU 很可能是对等认证的前奏。
- **长期：会压缩算法稳定币和链上发行的监管灰色地带**。GENIUS Act 事实上把"合规稳定币 = 100% 法币或国债储备+月度审计"写死——USDT 若坚持 commercial paper 结构，将在美国受限制。

Circle、PayPal PYUSD、Ripple RLUSD 都是潜在受益者；Tether 若不转移储备结构，可能继续被挡在美国银行代付通道外。

---

### 🔑 5. CLARITY Act 仍滞留参议院——市场结构立法窗口被缩到 2027

两院通过的概率在今年夏季被 Polymarket 定在 >60%，但到了 10 月 Senate 休会结束之后，关键矛盾仍未解决：
- **稳定币 reward（类似"链上利息"）是否合法**；
- **DEX 做市者是否触发 BSA 的"货币传输人"身份**；
- **"数字商品"与"数字证券"的 bright-line**。

**最可能的时间线被向后推到 2027 年初**。这给了业界几个月的"合规窗口"去游说，但也意味着**美国本土 Perp DEX / RWA 协议在接下来 6 个月仍要在"合规叙事"下自我约束**——这是今年 Base / Arbitrum / Solana 的新一波 RWA 项目普遍选择 BVI、瑞士结构的直接原因。

---

### 🔑 6. 行情面：BTC 停在 $112K，波动率压低、Funding 转负

虽然缺少 10 月 23 日的权威报价，但主要信号已经成型：**BTC 自月初以来基本横盘于 $108K-$115K**，30 日已实现波动率跌至 2026 年新低；**ETH 则沿 $4,400-$4,700 震荡**。永续合约 funding rate 自 10 月中旬以来转为负值，表明空头被迫支付——这是**宏观对冲基金在上涨尾声累积空头的典型姿态**。

需要盯的两件事：
- **11 月 Anthropic IPO 热度 + 12 月初美联储议息决议**——两个事件会把波动率打回来；
- **Bitget 盗币后对主要山寨币的"黑钱出清"路径**，部分交易所流动性已经被动降低。

---

## 市场脉搏

**价格概览（10 月 23 日观察区间，非实时报价）：**

- **BTC**：~$112,000（30 日 ±2.5% 窄震荡）
- **ETH**：~$4,500（相对 BTC 继续走弱，ETH/BTC = 0.040）
- **SOL**：~$199–$210（经过一波 FTX 相关解锁消化后反弹）
- **总市值**：加密整体 $3.9–$4.0T；稳定币部分 $308B

**技术位：**

- BTC 关键支撑 $107K / 阻力 $118K；只要 funding 保持负值，突破上沿更可能是空头回补驱动。
- ETH/BTC 若跌破 0.038 将确认季度级下行通道。

**情绪指标：**

- Fear & Greed Index：中性偏贪婪（约 55）；
- 永续 funding：BTC -0.004% / 8h，ETH -0.008% / 8h（空头付费）；
- GBTC 贴水已消失一年多，这波流出以 FBTC 和 GBTC 并行。

**要点：** BTC 现在是"合规资产", ETH 还在"收益资产 vs 合规资产"中间夹层。SEC 托管提案落地之前，机构会继续偏 BTC；真正能改变 ETH 配置权重的，是 ETF 内嵌 staking 的审批结果。

---

*数据来源：Farside Investors、The Block、Cointelegraph、DefiLlama、Chapman On Chain、Akin Gump CryptoLink。价格为近期区间观察，不构成实时报价。*
