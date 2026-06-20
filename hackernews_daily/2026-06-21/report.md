# Hacker News 日报 · 2026-06-21

## 今日焦点

> **AI 剽窃争议 · CSS 极限玩具 · Linux 6 年技术债清偿 · 媒体标准开源 · Agent 友好的云基础设施**
>
> - **CSSQuake** 用 CSS 3D Transform 重写 Quake，427 分 89 评，"M1 Pro 跑得不如 90 年代 Pentium"成为热评。
> - **Obscure Sorrows 被 AI Agency 整本抄袭** 283 分 121 评，原作者面对 SEO 反超无力维权，DMCA 失败 → 平台问责争论再起。
> - **SMPTE 标准全免费开放** 188 分，AI/Provenance/IP-based workflows 时代下，闭源标准已成行业累赘。
> - **Linux 7.2 终结 strncpy** 50 分 17 评，360 个补丁、6 年长跑，内核安全 API 重构里程碑。
> - **Cloudflare 为 AI Agent 推出临时账号** 137 分 86 评，agentic infra 的"无注册即部署"范式开始落地。

---

## 今日热榜总览

| 排名 | 标题 | 描述 | 分数 | 评论数 |
|------|------|------|------|--------|
| 1 | [CSSQuake](https://news.ycombinator.com/item?id=48608223) | CSS 3D 复刻 Quake | 427 | 89 |
| 2 | [The Wholesale Plagiarism of Obscure Sorrows](https://news.ycombinator.com/item?id=48611411) | AI Agency 整本抄袭原创书 | 283 | 121 |
| 3 | [SMPTE Standards 全部免费](https://news.ycombinator.com/item?id=48610827) | 媒体行业标准库免费 | 188 | 57 |
| 4 | [F-15 Strike Eagle II DOS 逆向项目](https://news.ycombinator.com/item?id=48609766) | 找老飞行员测试逆向版 | 172 | 47 |
| 5 | [Cloudflare Temporary Accounts for AI Agents](https://news.ycombinator.com/item?id=48608394) | 给 Agent 用的临时账号 | 137 | 86 |
| 6 | [UHF X11: visionOS / Vision Pro 上的 X11](https://news.ycombinator.com/item?id=48610853) | Vision Pro 跑 X11 | 133 | 18 |
| 7 | [Show HN: StartupWiki](https://news.ycombinator.com/item?id=48610224) | Crunchbase 的免费替代 | 125 | 35 |
| 8 | [Bun 给 JavaScriptCore 提交共享内存线程 PR](https://news.ycombinator.com/item?id=48610841) | Bun 推 JSC 加多线程 | 94 | 147 |
| 9 | [South Korea 武器出口生意](https://news.ycombinator.com/item?id=48608515) | 韩国军工崛起报道 | 83 | 30 |
| 10 | [Show HN: Make PDFs look scanned](https://news.ycombinator.com/item?id=48611513) | PDF 伪装成扫描件 | 62 | 30 |
| 11 | [PostgresBench by ClickHouse](https://news.ycombinator.com/item?id=48611942) | Postgres 服务可复现基准 | 55 | 9 |
| 12 | [巴西全国手机收到伪造预警短信](https://news.ycombinator.com/item?id=48612502) | 黑客攻破 CBS 警报系统 | 54 | 28 |
| 13 | [Linux 7.2 砍掉 strncpy](https://news.ycombinator.com/item?id=48612943) | 360 补丁 6 年清算技术债 | 50 | 17 |
| 14 | [Why pointe shoes 几百年没变](https://news.ycombinator.com/item?id=48605310) | 芭蕾鞋为何抗拒创新 | 41 | 41 |
| 15 | [Show HN: Windows XP 风格作品集](https://news.ycombinator.com/item?id=48612095) | 含 Game Boy 与 iPod | 38 | 17 |
| 16 | [Tesco 起诉 VMware 违约](https://news.ycombinator.com/item?id=48613008) | Broadcom 收购后续诉讼 | 34 | 4 |
| 17 | [Inference cost at scale with napkin math](https://news.ycombinator.com/item?id=48560227) | 推理成本心算 | 30 | 4 |
| 18 | [Alice is impatient (Brooker)](https://news.ycombinator.com/item?id=48612740) | 关于等待的工程思考 | 21 | 1 |
| 19 | [A Love Story (Pudding.cool)](https://news.ycombinator.com/item?id=48612714) | 数据新闻互动作品 | 12 | 2 |
| 20 | [Coding a Brick Tower (video)](https://news.ycombinator.com/item?id=48602683) | 砖塔生成的编程视频 | 8 | 0 |

---

## 重点讨论点评

### 🥇 [The Wholesale Plagiarism of Obscure Sorrows](https://waxy.org/2026/06/the-wholesale-plagiarism-of-obscure-sorrows/) — 283 分 · 121 评

**当"AI 重新打包"成为流量黑市的标准操作**

Andy Baio 撰文披露：一家叫 Qontour 的网页设计公司用 "**the**dictionaryofobscuresorrows.com" 整本搬运了 John Koenig 的同名作品——全部 311 个生造词与释义照搬，插图换成 AI 生成，再用 GPT-4 加了一个"造词器"功能，然后把网站当作品集自吹自擂，**还塞了 Amazon affiliate 抽佣**。最讽刺的是：盗版站现在 Google 搜索排名比原版还高，ChatGPT/Gemini 都把它当 Koenig 本人作品引用。Simon & Schuster 提了两次 DMCA 都被驳回。Koenig 本人无奈："Yeah man, I had nothing to do with it."

HN 评论区的核心情绪是**无力感**——不是关于"AI 是否会创造价值"，而是关于"平台问责机制是否还在运转"。多位用户分享了相似的被盗用经历，结论一致：Google/Apple 没法院命令不动，DMCA 在 AI 重排后基本失效，统计损害赔偿要求版权预先注册。

> *热门评论摘要：* "Google 和 Apple 在 DMCA 上毫无作用，除非你有法院命令。" "整本逐字复刻，为什么版权法不能让原作者获得侵权页的所有权？" "Amazon affiliate 计划准入门槛太低，给了 AI slop 一个套利通道。"

这条讨论是 HN 当天最浓缩的"2026 内容生态危机"切片：**AI 让盗版成本骤降到接近零，而维权成本几乎没变**。

---

### 🥈 [CSSQuake](https://cssquake.com/) — 427 分 · 89 评 · [HN 讨论](https://news.ycombinator.com/item?id=48608223)

**"能跑"与"该跑"的距离从未如此具体**

CSSQuake 用纯 CSS 3D Transform 渲染整个 Quake 场景，TypeScript 写游戏逻辑——一个典型的"看看 CSS 还能被滥用到什么程度"的炫技作品。HN 上线即冲到 #1，427 分。

但顶级评论几乎全是性能吐槽——"我 90 年代的 Pentium-133 跑 Quake 比我现在的 M1 Pro 跑这个流畅"。Safari/WebKit 卡顿严重，Chrome/Firefox 才能勉强玩，电梯按钮要用枪打而不能碰一下、碰撞检测也飘。

这条讨论的真正看点不是"CSS 能不能渲染 Quake"，而是 HN 集体心照不宣的一个判断：**浏览器作为通用计算平台已经到了"能力盈余但效率赤字"的阶段**。CSS 变换比纯软渲染慢几个数量级，但因为通用，反而成了"显摆精神"的最佳载体。

---

### 🥉 [Cloudflare Temporary Accounts for AI Agents](https://blog.cloudflare.com/temporary-accounts/) — 137 分 · 86 评 · [HN 讨论](https://news.ycombinator.com/item?id=48608394)

**"Agent-friendly infra"作为新基础设施品类的开端**

Cloudflare 推出 `wrangler deploy --temporary`：AI agent 不需要注册、不需要 OAuth、不需要 MFA，就能拿到一个临时账号部署 Worker，60 分钟内可以多次迭代，事后可以让人类点链接"领养"成正式账号。

Cloudflare 在博客里有一句很出圈的话："the moment an agent needs to deploy something, it slams face-first into a wall built for humans." HN 上的讨论分两派：

- **乐观派**：这是 agentic infra 的关键缺失环节，认证流程是当前 agent 自主迭代的真正瓶颈。
- **担忧派**：60 分钟无认证部署 = 完美的滥用窗口，Cloudflare Worker 已经是钓鱼/恶意脚本重灾区，这等于发面包给狼。

这条讨论值得反复读：**未来 12-18 个月，"为 agent 重新设计的 SaaS 入口"会成为 SaaS 厂商的差异化战场**。Cloudflare 这次是第一家公开把"为人类设计"和"为 agent 设计"分成两条产品线的。

---

### 🏅 [SMPTE Makes Its Standards Freely Accessible](https://www.smpte.org/blog/smpte-makes-its-standards-freely-accessible-openingstandards-library-to-the-global-media-technology-community) — 188 分 · 57 评 · [HN 讨论](https://news.ycombinator.com/item?id=48610827)

**当内容真实性危机倒逼标准组织开源**

SMPTE（动画电影与电视工程师协会）宣布：包括 Standards、Recommended Practices、Engineering Guidelines、RDD 在内的**全部已发布与未来标准**都免费开放。这在数十年闭源付费下载的传统下是巨大转向。

SMPTE 总裁 Rich Welsh 的话很点睛：*"行业正在面对从 IP-based workflows 到 AI 真实性与内容溯源的转型。"* 翻译：**当 deepfake 和 AI 生成内容随处可见时，标准库不能再是付费墙后面的"行业秘密"——Provenance、C2PA、SMPTE 2110 这类标准必须能被任何小厂、任何独立开发者直接读取并实现**，否则真实性体系会被绕过。

HN 评论里一个高赞观点：*"这不是慈善，这是行业自救——标准被付费墙挡着的时代，已经 50% 的开发者绕过 SMPTE 用 GitHub 上的'类似实现'。"* Diamond 级赞助方包括 AWS / Apple / Disney / Dolby / Sony，背后明显有 CDN/流媒体大厂的推动。

---

### 🎖️ [Linux 7.2 Eliminates the strncpy API After Six Years](https://www.phoronix.com/news/Linux-7.2-Drops-strncpy) — 50 分 · 17 评 · [HN 讨论](https://news.ycombinator.com/item?id=48612943)

**360 个补丁、6 年的"语义陷阱清算"**

Linux 内核 7.2 正式删除 `strncpy` —— 这个 C 标准库里最容易写错的 API（不保证 null-terminate、可能不填满 buffer、行为依赖于源串长度）终于在内核中绝迹。整个迁移耗时 **6 年、360 个补丁**，替换成 `strscpy` 和 `strscpy_pad`。

这条新闻评论数不多，但意味深远：**大型代码库的 API 替换不是"重写"，而是"博物馆式清扫"**。Linux 的做法（不一次性废弃、逐子系统迁移、有 deprecation 周期、自动化扫描工具同步推出）是所有想做长期演进的语言/标准库组的教科书案例。Rust 社区在 ABI 演进上、CPython 在 C API 上面临的恰好是同一类问题。

---

## 社区脉搏

今天的 HN 出现了**清晰的两条主线**：

**主线一 · "AI 时代的边界争论"**：Obscure Sorrows 抄袭事件、Cloudflare 给 Agent 开后门、SMPTE 标准免费——三者本质都在回答同一个问题："当 AI 大规模生产/部署/分发时，原有的人类制度（版权、认证、付费标准）该怎么改？" 评论区的态度比 6 个月前明显务实——**少了道德指责、多了制度漏洞分析**，社区开始接受"AI 不会停下来等制度修补"。

**主线二 · "技术债清算与平台代际更替"**：Linux 砍 strncpy、Bun 给 JavaScriptCore 提共享内存线程 PR、Vision Pro 上跑 X11——HN 老用户对"技术陈年问题"的关注热度比对新框架还高。Bun 那个 PR 居然 94 分却 147 评（评论比分高，HN 上少见），说明社区认真在算"如果 JSC 拿到多线程，Node.js 和 Deno 的相对竞争力会怎么变"。

值得一提的是，**今天有 4 条 Show HN 进了前 20**（StartupWiki、PDF 扫描化、Windows XP 作品集、CSSQuake），但只有 CSSQuake 出圈——HN 对"实用 Show HN"的耐心今天明显不如对"炫技作品"的耐心。
