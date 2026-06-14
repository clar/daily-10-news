# Polymarket Daily · 2026-06-15

## 今日焦点

> **世界杯赛事 24h 成交 $95M · 美伊和平押注两侧分裂 · FOMC "零变动"概率 99.5% · RFK Jr 共和党 2028 领跑 49% · 民主党 Newsom 23.5%**
>
> - **World Cup Winner**：西班牙 16.4% 与法国 16.1% 几乎并列，市场单日 $95.3M 流入。
> - **美伊永久和平协议**：5-6 月所有截止日 YES 全是 0，市场不相信"永久"；但"短期 ceasefire 延期至 6/30" YES 99.65%。
> - **6 月 FOMC 降息 25bp 概率 0.25%、加息 0.15%、加 50bp 0.15%**——市场把"按兵不动"押到 99.5%。
> - **2028 共和党初选**：RFK Jr 49% 领跑、Vance 33%、Rubio 23%——三者 YES 总和 >100%，疑似中场极右翼押注情绪。
> - **2028 民主党初选**：Newsom 23.5% 一马当先，AOC 9.3%、Ossoff 7.8%、Harris 7.3% 紧随。

---

## 热门市场速览

| # | 市场 | 分类 | YES 概率 | 24h 交易量 | 流动性 |
|---|------|------|----------|-----------|--------|
| 1 | [World Cup Winner](https://polymarket.com/event/world-cup-winner) | 体育 | 西班牙 16.4% | $95.3M | $479.2M |
| 2 | [Netherlands vs. Japan](https://polymarket.com/event/fifwc-nld-jpn-2026-06-14) | 体育 | 平局 99.95% | $26.2M | $6.1M |
| 3 | [US x Iran permanent peace deal by...?](https://polymarket.com/event/us-x-iran-permanent-peace-deal-by) | 地缘 | 各截止日 YES≈0% | $16.7M | $1.9M |
| 4 | [US announces new Iran agreement/ceasefire extension by...?](https://polymarket.com/event/us-announces-new-iran-agreementceasefire-extension-by) | 地缘 | 6/30 前 99.65% | $6.4M | $3.9M |
| 5 | [Fed Decision in June?](https://polymarket.com/event/fed-decision-in-june-825) | 宏观 | 维持 99.5% | $5.5M | $8.6M |
| 6 | [Next Prime Minister of Ethiopia?](https://polymarket.com/event/next-prime-minister-of-ethiopia) | 政治 | 多人混战 | $4.3M | $0.07M |
| 7 | [CS2: NaVi vs Team Falcons (BO3)](https://polymarket.com/event/cs2-navi-fal2-2026-06-14) | 电竞 | Map2 NaVi 99.9% | $4.3M | $1.4M |
| 8 | [Côte d'Ivoire vs. Ecuador](https://polymarket.com/event/fifwc-civ-ecu-2026-06-14) | 体育 | 厄瓜多尔 38.5% | $3.7M | $5.5M |
| 9 | [Sweden vs. Tunisia](https://polymarket.com/event/fifwc-swe-tun-2026-06-14) | 体育 | 瑞典 51.5% | $3.6M | $6.7M |
| 10 | [Netherlands vs. Japan – Exact Score](https://polymarket.com/event/fifwc-nld-jpn-2026-06-14-exact-score) | 体育 | 各比分 <1% | $2.8M | $3.0M |

---

## 重点点评

### ⚽ 1. World Cup Winner — 西班牙、法国"V 字双雄"格局成型

24h 成交 **$95.3M**、流动性 **$479M**——本届世界杯单事件已经成为 Polymarket 历史上 liquidity 最高的体育市场之一。当前赔率：

- 西班牙 **16.4%**、法国 **16.1%**——几乎并列，代表市场对欧洲两强的高一致性预期
- 葡萄牙 11.2%、英格兰 9.7%——稳定的"半决赛常客"档
- 阿根廷 8.0%、巴西 6.8%、德国 6.0%、荷兰 5.1%——南美和欧洲中游

值得注意的是 **西班牙今天的 Cabo Verde 小组赛 YES 91.5%**，几乎是"白送钱"押注，因此目前的全胜赔率没有把"小组赛冷门"风险计入；如果西班牙在小组赛意外掉链，冠军赔率会立刻往 12% 以下打。**今日观察重点**是 14 日 Netherlands vs. Japan（最新行情显示开盘后被押到 99.95% 平局，强烈异常，详见下）。

---

### 🇳🇱🇯🇵 2. Netherlands vs. Japan = 99.95% 平局？市场结构问题，不是真实判断

这是一个明显的**数据/合约异常**：在一场已开始或即将开始的小组赛里，YES 价被推到接近 1.0 的"平局"几乎不可能反映真实预期。两个解释：

1. **比赛已结束且确为平局**，市场处于结算前最后阶段（合约还活着但价格已收敛）；
2. **合约 metadata 错位**，导致"Draw" YES 被等价于"已结算 / 待发放"——查 outcomePrices 数组对应"draw" 的最后值。

对照"Exact Score" 子市场（所有具体比分 YES 都在 0），这种结构暗示比赛大概率是 **0-0 平局** 或某种异常已结算状态。这个事件在 24h 成交了 $26.2M——是当日除冠军盘外最大体育成交，可能在赛后还有清算流动性。

**结论：不构成交易信号，是赛果反映**。这种"已知信息但合约未结算"窗口里，bid-ask 价差通常会保持 0.5%-1%，不存在真套利。

---

### 🕊️ 3. 美伊：永久和平 0%，临时停火延期 99.65% — 市场看法明确

两个相关市场拼起来看就很清楚了：

- **永久和平协议 by [任何 2026 截止日期]**：YES 全部接近 0%
- **临时 ceasefire/agreement 延期 by 6/30**：YES **99.65%**

市场的判断毫不含糊：**短期会有协议、长期不会有永久和平**。这与昨夜的市场叙事完全一致——油价跌 2%、风险偏好回暖、SpaceX IPO 强势开盘，都是 short-term peace dividend，但没有人愿意为"永久和平"出价。

这背后的合理 prior 是：美伊关系的结构性矛盾（核计划、地区代理人战争、制裁博弈）在 18 个月内不可能解决；任何"协议"都是阶段性 ceasefire + 部分制裁松绑，而非完整重建外交。**6/30 截止前如果协议正式签署**，"延期"YES 应该完成结算（小幅获利空间已基本消失）；"永久"市场仍会维持低概率，但可能从 0% 抬到 3-5%，为投机者提供长尾。

---

### 🇺🇸 4. 2028 共和党初选 — RFK Jr 49% 让人意外

这是今天最值得 raise eyebrow 的市场：

- RFK Jr. **49%**
- J.D. Vance **33.2%**
- Marco Rubio **23.1%**
- Tucker Carlson 6.6%
- 川普本人 2.1%

**两点必须指出**：

**(1) YES 概率总和远超 100%（仅前三人就 105%）**——这要么是 Polymarket 多市场之间的"叠加买入"造成的临时市场失衡（Marco Rubio vs Vance 同 YES 被多次买）；要么是市场处于"信息冲击"窗口，每个押注者只看到自己看好的人。理论上存在**全部卖 YES 的负向 arb**，但需要扣 spread 和资金成本，未必划算。

**(2) RFK Jr 在 49% 是反共识的极端押注**——传统民调里他并未进入共和党 top 3，能押到 49% 大概率是某次政治事件（健康部长任期表现、副总统提名传闻等）触发的资金涌入。值得查最近 7 天的价格走势。

---

### 🇺🇸 5. 2028 民主党初选 — Newsom 23.5% 暂时领跑，AOC 9.3% 是底层暗流

民主党盘相对"健康"：

- Gavin Newsom **23.5%**
- AOC **9.3%**
- Jon Ossoff 7.8%
- Kamala Harris 7.3%
- Josh Shapiro 5.1%

合理且分散——没有明确"早期共识候选人"。**AOC 9.3% 是最被低估的信号**：传统建制媒体对她在初选中的可能性几乎不报道，但 Polymarket 用真金白银押到第二位，说明 progressive wing 在民主党失利后的复仇情绪在累积。

下一波价格变动取决于 **(1) Newsom 是否正式宣布**（届时 YES 可能直接抬到 35%+）；**(2) 中期选举后是否出现"黑马"州长**（Shapiro / Beshear 都可能在 2026 中期后大幅上扬）。

---

## 套利与异常信号

### 配对成本异常 (YES + NO < .98)

今日未发现明显套利机会（成熟市场如 Fed Decision、Iran 延期、World Cup 各队 spread 都已收敛到 0.1-1% 区间）。

### 高价差市场 (Spread > 5%)

| 市场 | best Bid | best Ask | 价差 | 说明 |
|------|----------|----------|------|------|
| Shimelis Abdisa (Ethiopia PM) | 0.001 | 0.030 | ~2.9pt | 政治冷门市场，流动性极差 |
| Iran closes airspace by 7/31 | 0.19 | 0.22 | 3pt | 地缘事件型，价差偏宽 |
| Trump 解除霍尔木兹封锁 | 0 | 0.001 | <1pt | 极端低概率市场 |

总体而言**主流市场流动性充足**，仅在低成交、政治冷门和地缘事件题材中能看到 5pt+ 价差。

### 异常加和 (Σ YES > 1.05)

| 市场组 | 总和 | 解读 |
|--------|------|------|
| 2028 GOP Nominee（前 3 人） | ~105% | 多市场叠加 YES，存在反向 arb 但成本不低 |
| Iran ceasefire by Jun 30 | 99.65% | 接近确定但未结算 |

---

## 新上线市场

最近创建的市场以**高频"5/15 分钟币价上下"合约**为主（BNB / ETH / SOL / HYPE / DOGE / XRP / BTC up-or-down），属于自动机器人喂单，可观察价值低。建议关注稍早创建的：

1. **Spain vs. Cabo Verde 小组赛**（slug: `fifwc-esp-cvi-2026-06-15`）——西班牙 91.5%，是"高赔率单边"配对的典型样本，对应保险类策略
2. **Sweden vs. Tunisia**（slug: `fifwc-swe-tun-2026-06-14`）——瑞典 51.5%，开赛前最接近 50/50 的世界杯小组赛
3. **Fed Decision in June** 与 **Iran ceasefire extension by 6/30** 仍在持续吸金，作为宏观+地缘的对冲篮子值得关注

---

## 分类概览

- **体育**：世界杯成绝对主角，单事件 $95M 量级把 Polymarket 流量推到年内高点；个别"已结算待清算"合约（NLD vs JPN）显示出极端 YES。
- **地缘**：美伊主题，市场用价格清楚区分"短期 ceasefire" vs "永久和平"——这种分层是 Polymarket 价值最直接的体现。
- **宏观**：FOMC 维持 99.5% 已无悬念，市场转向"决议措辞 / SEP 修订"等不可下注的 narrative 维度。
- **政治**：2028 两党初选都还在 narrative pricing 阶段，民主党分散、共和党出现 RFK Jr 这种反共识热点。
- **电竞 / 其他**：日常成交分散，单笔市场 < $5M，对全市场流动性贡献有限。

> 免责声明：本报告仅供信息参考，不构成任何投资或交易建议。Polymarket 在部分司法管辖区可能受到限制。
