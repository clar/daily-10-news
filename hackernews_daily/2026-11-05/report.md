# Hacker News 日报 · 2026-11-05

## 今日焦点

> **AI 翻出 40 年老代码债 · Nvidia 加密固件锁死 Linux · 朝鲜社工 63 亿 Binance 大劫 · 白宫网络出现家用代理出口 · AMD Q4 收入史上首次反超 Intel · 可验证推理工业化**
>
> - **AI is forcing us to pay off 40 years of technical debt** —— 983分 593评,HN 今日最大讨论:PHP 老洞被 AI 翻出,安全债到期。
> - **Nvidia RTX Spark encrypted firmware slows inference speed to 35% on Linux** —— 569分 263评,Linux 被固件加密表卡在 780 MHz。
> - **North Korean fake job interview led to $6.3B Binance heist** —— 538分 318评,一场假面试撬开 63 亿美元。
> - **Residential proxies detected on White House network** —— 373分 107评,Executive Office 的 ASN 下有 236 次家用代理出口。
> - **AMD expects to outsell Intel in Q4 for the first time in history** —— 419分 134评,170 亿美元指引压过 Intel。

---

## 今日热榜总览

| 排名 | 标题 | 描述 | 分数 | 评论数 |
|------|------|------|------|--------|
| 1 | [AI is forcing us to pay off 40 years of technical debt](https://news.ycombinator.com/item?id=50364336) | AI 翻出 PHP 老洞,安全债到期 | 983 | 593 |
| 2 | [Nvidia RTX Spark encrypted firmware slows inference speed to 35% on Linux](https://news.ycombinator.com/item?id=50362905) | 加密功率表让 Linux 卡死 | 569 | 263 |
| 3 | [North Korean fake job interview led to $6.3B Binance heist](https://news.ycombinator.com/item?id=50365755) | 假面试换来 63 亿美元 | 538 | 318 |
| 4 | [AMD expects to outsell Intel in Q4 for the first time in history](https://news.ycombinator.com/item?id=50367125) | 170 亿指引压过 Intel | 419 | 134 |
| 5 | [Residential proxies detected on White House network](https://news.ycombinator.com/item?id=50371246) | Executive Office ASN 挂代理 | 373 | 107 |
| 6 | [Verification Is Not Knowledge: Science needs more than answers](https://news.ycombinator.com/item?id=50363019) | AI 时代的科学方法反思 | 215 | 128 |
| 7 | [A new Go API for JSON](https://news.ycombinator.com/item?id=50369106) | Go 官方发布 jsonv2 | 177 | 75 |
| 8 | [Ripple-65B Preview: U.S. Open-Weight SOTA on Agentic Coding](https://news.ycombinator.com/item?id=50369925) | 美国开源编程 SOTA | 167 | 58 |
| 9 | [Tencent Hy4](https://news.ycombinator.com/item?id=50365780) | 腾讯新模型 Hy4 发布 | 159 | 47 |
| 10 | [Progress on provable inference for large language models](https://news.ycombinator.com/item?id=50368626) | Anthropic FlashProve 研究 | 153 | 75 |
| 11 | [OpenAI to acquire Pierre Computer Company](https://news.ycombinator.com/item?id=50366863) | OpenAI 又收一家硬件公司 | 141 | 49 |
| 12 | [Insects don't swarm at LED lights](https://news.ycombinator.com/item?id=50370610) | 常识被实验推翻 | 112 | 63 |
| 13 | [Show HN: Co-op working in DOS Wing Commander](https://news.ycombinator.com/item?id=50369895) | 十年逆向改出联机 | 71 | 4 |
| 14 | [Qualcomm Cloud AI 100 Ultra – 150W/128GB/548GB/s](https://news.ycombinator.com/item?id=50370654) | 高通推新推理卡 | 66 | 33 |
| 15 | [Conductor Is Joining Meta](https://news.ycombinator.com/item?id=50369503) | Build 工具团队被 Meta 收编 | 64 | 115 |
| 16 | [Launch HN: Kino AI (YC S23) – AI media manager and video editor](https://news.ycombinator.com/item?id=50368804) | YC AI 视频工具发布 | 57 | 24 |
| 17 | [Ask HN: Cryptography book for 10 year olds?](https://news.ycombinator.com/item?id=50347425) | 给孩子的密码学启蒙 | 21 | 28 |
| 18 | [Ask HN: experience with "who wants to be hired" thread](https://news.ycombinator.com/item?id=50372294) | 月度招聘贴到底管用吗 | 22 | 6 |
| 19 | [Hacking the Xbox 360 Hypervisor Part 3](https://news.ycombinator.com/item?id=50372164) | 老主机继续被拆解 | 13 | 2 |
| 20 | [Show HN: The DNA of DOOM – code across 44 ports](https://news.ycombinator.com/item?id=50339183) | DOOM 跨平台"基因"可视化 | 7 | 8 |

---

## 重点讨论点评

### 🥇 [AI is forcing us to pay off 40 years of technical debt](https://news.ycombinator.com/item?id=50364336) —— 983分 · 593评

**AI 这次不是攻击方,是放大镜 —— 把埋了四十年的 C/PHP 内存错当成一枚枚可用漏洞翻了出来。**

IEEE Spectrum 的这篇长文围绕 PHP2Shell 案例展开:一个 2024 年报告的 PHP 内存 bug 当年被评估为"只是会崩一下的小毛病",2026 年研究员借助 AI 工具重新审视,发现足以发起远程代码执行。文章的核心论点是:AI 让漏洞发现的边际成本坍塌,但"找到"远比"修好"便宜;几十年积累的 C 和早期脚本语言代码,在新的攻击面放大镜下集体过期。文中引用 Matthew Green 的警告 ——"真正的行动,大概要等一次更糟糕的事件"—— 把今天的 HN 情绪钉得死死的。

HN 评论区分两派:一派是基础设施老兵,支持文章建议的"更多资金 + 形式化验证"方向,另一派(占多数)认为问题根源不是技术,是组织 —— 没有人为 20 年前的开源 C 库付工资,AI 只是把这块空洞照亮了。一个高赞评论问得更残酷:"如果 AI 代审(AI code review)成了标准,保险公司会不会强制要求?不然这些 CVE 爆出来后你赔不起。"

> *热门评论摘要:* 技术债的真问题不是代码质量,而是治理模型 —— 开源基础设施长期被当免费资源,AI 把无人维护的那一部分变成了可预测的安全风险,接下来会被监管或保险业"定价"。

---

### 🥈 [Nvidia RTX Spark encrypted firmware slows inference speed to 35% on Linux](https://news.ycombinator.com/item?id=50362905) —— 569分 · 263评

**一张只能在 Windows 驱动里解密的"功率设置表",把 Linux 的 GPU 时钟锁在了 780 MHz。**

作者在同一台搭载 RTX Spark 的笔记本上做了 Windows、WSL、DGX Spark、原生 Linux 四组对照:Windows 本地跑 GPT-OSS-120B 约 65 tokens/s,原生 Linux 只有 13.9 tokens/s —— 约 21% 的性能(文章标题的"35%"源自另一组对照,具体数字评论区还在争)。实验排除了内核、驱动版本和散热,最终锁定问题:Nvidia Platform Controllers and Framework 把电源配置以加密形式交给 Windows 驱动,只有 Windows 才能把 CPU/GPU 的功率预算解出来 —— Linux 上这张表是黑盒,GPU 时钟因此被卡在约 780 MHz,Windows 下可以跑到 2.2 GHz。

HN 的愤怒点不在"性能差一半",而是"厂商用加密主动阻断开源操作系统的发挥"。这个话题和今年早些时候 Nvidia 对开源驱动的历史积怨叠在一起:老用户抬出 2012 年 Torvalds 那次著名的"NVIDIA, Fxxx you!",新用户问 Framework、System76 这些主打 Linux 的 OEM 还要不要继续押 Nvidia。评论区也有理性派:加密表并不是针对 Linux,而是 Nvidia 对自家功率配置流程的信任边界,但 Linux 驱动没拿到对等的授权实现,结果一样。

> *热门评论摘要:* 厂商可以说这不是"锁"是"没适配",但当加密表只对一个 OS 开门时,实践效果就是封闭 —— 开源社区目前除了"从 Windows 驱动里抽密钥"没别的办法,而这显然不是稳定方案。

---

### 🥉 [North Korean fake job interview led to $6.3B Binance heist](https://news.ycombinator.com/item?id=50365755) —— 538分 · 318评

**社工攻击的回报率再创新高 —— 一份假的招聘流程换来了 63 亿美元。**

The Register 整理了朝鲜 Lazarus 系(或旁支)在今年针对 Binance 工作人员的攻击链条:精心包装的 LinkedIn 招聘联系 → 多轮技术面试 → 以"请在隔离环境运行我们的编码测试"为由投递伪装成测试环境的 npm 包 → 开发机获得立足点 → 横向移动至签名流程 → 绕过多签 → 窃走 63 亿美元资产。这是迄今最大的一次加密货币盗窃,也是"假 Zoom 面试 + 恶意 npm 包"这个老配方的收益新高度。

HN 评论区把火力对准了 Binance 自己的流程设计:为什么工程师的开发机能和签名密钥环境走到同一张网?为什么"候选人提交的代码"竟然可以在内部环境被执行?另一拨人在聊供应链侧 —— npm 对朝鲜/恶意账户的清理一直是弱项。再有一派在算冷账:63 亿美元,相当于朝鲜 2025 年 GDP 估算的~15%,制裁没堵住的,黑客给补上了。

> *热门评论摘要:* 工程师把"假面试"当笑话,但招聘流程天然要求你与陌生人分享屏幕、跑对方给的代码 —— 这是企业现在最脆弱的一块攻击面,从 Coinbase、LastPass 到现在的 Binance,剧本一模一样。

---

### 🏛️ [Residential proxies detected on White House network](https://news.ycombinator.com/item?id=50371246) —— 373分 · 107评

**AS2650(Executive Office of the President 的自治系统)被 Layer3 Intel 的 Residential Proxy Observatory 捕获为"家用代理出口"。**

数据:2026 年 10 月 5 日至 11 月 3 日的 30 天里,该 ASN 内 6 个 IP 共 236 次出口流量,涉及 28 家家用代理商;出口时间大约一半集中在东部时间下午 5 点到午夜 —— 更像是某台个人设备被植入了代理 SDK,而不是公开访客 Wi-Fi。Layer3 也强调:他们只看到"出口",看不到"设备上是谁"。Spur 和 Synthient 做了独立交叉验证。

HN 的反应比"白宫被攻击"要冷静得多。一类解读是:有人在 EOP 办公网内的个人设备上装了带捆绑代理 SDK 的 App —— 常见的"免费 VPN / 盗版插件 / 翻墙工具"背后都挂这类 SDK,流量会被重卖给代理商。另一类更深层的担心:这类 SDK 不只是把设备变成代理出口,还是一条可横向移动的内网入口 —— Kimwolf 僵尸网络就是靠这条链路攻陷了 200 万台设备。

更有意思的是 —— 几位评论员指出,Layer3 的数据集还把 McMurdo 站(南极,Cloudflare WARP)、Saint Helena(32,000 次观测)、Pitcairn、Svalbard 等几乎所有"远端孤岛"一并暴露出来了;家用代理市场现在实际上已经把地球上大多数网络角落都纳入了"商业出口资源池"。

> *热门评论摘要:* 这件事不代表白宫被黑,而是代表"员工个人设备在工作网上"的边界崩了 —— 任何有 BYOD 的机构,只要内网不隔离,都可能是下一张代理地图上的热点。

---

### 🔐 [Progress on provable inference for large language models](https://news.ycombinator.com/item?id=50368626) —— 153分 · 75评

**Anthropic 把"可验证推理"做到了 400B MoE 模型 + 单张 H100 + 110 tokens/s —— 比正常推理慢 70-95 倍,但第一次"可以上线讨论"。**

论文核心很干净:模型方发布一次"权重承诺"(fingerprint),每次响应附带一个 zkSNARK 证明"这个输出来自那个权重"。用户/监管/下游应用用普通 CPU 就能验证。Anthropic 的 FlashProve 系统在 Llama 4 Maverick(400B MoE,4-bit)上做出来 110 tok/s、19MB 证明/1024 token,目前限制也写得很清楚:整数化模型 + greedy decoding + 不覆盖采样 + 只验到 1024 token 上下文 + 不隐藏架构 + 不防旁路。

HN 社区读到这篇普遍比较兴奋,但快速分裂成三派:

1. **密码学派**:认可这是把 zkML 从玩具搬到真实推理规模的里程碑 —— 之前 zkML 的参数量都在 B 以下;
2. **工程派**:70-95x 开销在 B2B 场景可以接受(审计 / 合规 / 主权 AI),但不可能"每次 chat 都挂证明";
3. **怀疑派**:提示"greedy decoding + 整数化"意味着被证的模型和你实际用的模型不是同一个 —— 这是"证明一个代用人",商业模型的 full-precision + sampled 输出仍然处于黑盒。

与今日热榜 No.1 的技术债讨论形成呼应:行业现在同时在修"过去留下的"(老代码老漏洞)和"未来要建的"(可验证的 AI 调用链),真正麻烦的是中间这一段 —— 当前大模型推理的信任假设几乎全是口头承诺。

> *热门评论摘要:* 这不是给你我每天 chat 用的,它是给监管、给企业审计、给"主权 AI"打基础;重要性 ≈ HTTPS 之于 Web —— 现在慢,但方向对。

---

## 社区脉搏

今天 HN 的情绪线是**"账本到期"**:

- **代码债到期**:AI 把老代码翻了个底朝天(No.1)、Nvidia 的加密固件被开发者翻出来算总账(No.2)、朝鲜黑客把"假面试+npm 包"玩成 63 亿美元现金流(No.3) —— 三条高赞主帖共同的叙事都是:过去我们"能跑就行"的妥协,现在被 AI 和成熟的攻击生态一次性敲收。
- **信任机制重建**:Anthropic 的 FlashProve(No.10)、Cosmos Institute 的《Verification Is Not Knowledge》(No.6) 以及 Pierre Computer 被 OpenAI 收购(No.11) 的讨论交织成另一个暗线 —— "AI 时代怎么对输出建立可审计的信任"开始从哲学讨论下沉到工程方案。
- **硬件版图在松动**:AMD Q4 预期收入 170 亿美元压过 Intel(No.4)、高通推出 128GB 的 Cloud AI 100 Ultra 推理卡(No.14)、腾讯 Hy4 低调上线(No.9)、Ripple-65B 作为"美国开源 agentic coding SOTA"(No.8)—— 加速器和开源权重的"第三/第四梯队"在悄悄合围,头部格局今年底会比年初更分散。
- **Meta 又下一子**:Conductor 团队加入 Meta(No.15) 115 条评论绝大多数是"创业者独立性"的旧式辩论,但对照今日 AI 日报里的 Cat Wu 离职 Anthropic,头部团队的人员流动节奏明显比 2025 年加快。

一句话收尾:**今天 HN 不在庆祝新东西,而在清账 —— 旧代码、旧驱动、旧招聘流程、旧内网边界,都在 AI 把放大镜架好的瞬间一起显形。**
