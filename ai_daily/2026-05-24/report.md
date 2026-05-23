# AI 日报 · 2026-05-24

## 今日焦点

> **AI 攻克 80 年数学猜想 · 监管放手与安全恐慌并存 · 供应链攻击席卷 AI 生态 · 巨头通过收购抢夺 Agent 入口 · 资本与算力的双重狂飙**
>
> - **OpenAI 内部推理模型独立证否埃尔德什 1946 年单位距离猜想**，125 页证明跨越组合几何与代数数论，菲尔兹奖得主 Tim Gowers 称"AI 数学的里程碑"
> - **特朗普应马斯克、扎克伯格、Sacks 之请废除 AI 安全行政令**，原计划的 90 天发布前审查框架胎死腹中
> - **Nx Console VS Code 扩展被投毒 18 分钟**，3,800 个内部仓库、Claude 配置、AWS Key 等大规模外泄；同期 TeamPCP 攻击 170+ npm 包，OpenAI、Mistral 均成受害者
> - **Anthropic 以超 3 亿美元收购 Stainless**，将 OpenAI/Google/Cloudflare 共用的 SDK 工具收为己有
> - **NVIDIA FY2026 Q1 营收 816 亿美元、利润 583 亿**，下季指引 910 亿继续超华尔街预期，宣布 800 亿美元回购

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | OpenAI 推理模型独立证否埃尔德什 1946 年单位距离猜想，125 页代数数论证明 | BuildFastWithAI | ⭐⭐⭐⭐⭐ |
| 2 | 特朗普废除 AI 安全行政令，马斯克/扎克伯格/Sacks 联合施压 | White House / Press | ⭐⭐⭐⭐⭐ |
| 3 | Anthropic 联创 Jack Clark 在牛津预测：12 个月内 AI 将拿出诺贝尔级成果，并承认"非零"灭绝风险 | Oxford / Anthropic | ⭐⭐⭐⭐ |
| 4 | Nx Console 扩展被投毒，3,800 个仓库外泄，含 Claude/AWS/GitHub 凭据 | Security disclosure | ⭐⭐⭐⭐ |
| 5 | TeamPCP 供应链攻击波及 170+ npm 包，受害者含 OpenAI、Mistral、欧委会 | CVE-2026-45321 | ⭐⭐⭐⭐ |
| 6 | Anthropic 收购 SDK 工具商 Stainless，估值超 3 亿美元，OpenAI/Google 失去共用基础设施 | TechCrunch | ⭐⭐⭐⭐ |
| 7 | NVIDIA FY26Q1 营收 816 亿美元 / 净利 583 亿，下季指引 910 亿，启动 800 亿美元回购 | Al Jazeera / NVIDIA | ⭐⭐⭐⭐⭐ |
| 8 | Meta 在 8,000 人裁员前用 Model Capability Initiative 跟踪员工 Gmail/VS Code/聊天记录 | Internal audio leak | ⭐⭐⭐⭐ |
| 9 | xAI 5 月连推 Grok 4.3、Grok Build 0.1、Grok Skills、Grok Connectors | xAI | ⭐⭐⭐ |
| 10 | Gemini Spark 个人 AI Agent 上线 MCP，接入 Canva、Instacart、OpenTable | Google I/O | ⭐⭐⭐⭐ |
| 11 | Intuit 裁员 3,000 人（8%），全力押注 AI Agent，预计节省 5 亿美元 | Intuit | ⭐⭐⭐ |
| 12 | OpenAI 完成 1,220 亿美元融资，投后估值 8,520 亿美元，软银/a16z 领投 | OpenAI | ⭐⭐⭐⭐⭐ |
| 13 | OpenAI 因供应链入侵，6 月 12 日撤销 macOS App 签名证书，用户需重装 | OpenAI | ⭐⭐⭐ |
| 14 | Anthropic 正式将"智能爆炸"风险写入研究议程，给出 2028 年时间表 | Anthropic | ⭐⭐⭐⭐ |
| 15 | Gemini 与 Adobe、Canva、CapCut 深度整合，支持"魔法图层"可编辑生成 | Google | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · OpenAI 模型独立证否 80 年悬案，AI 数学迎来分水岭

**[BuildFastWithAI · AI News Today May 23](https://www.buildfastwithai.com/blogs/ai-news-today-may-23-2026)**

OpenAI 周五披露，一款内部通用推理模型自主完成了对埃尔德什 1946 年单位距离猜想的证否——这是数论与组合几何中悬而未决近 80 年的核心问题之一。模型给出 125 页完整证明，构造出一族平面点配置，使单位距离对的数量显著高于历来被视为最优的方格排列，直接推翻了埃尔德什提出的上界估计。

最具冲击力的不是结果本身，而是路径。模型没有沿用既有的方格优化思路，而是借助 1964 年 Golod–Shafarevich 准则中无限类域塔的代数数论结构，强行把一道"看似纯几何"的问题嫁接到深层数论上——这是组合几何学者几十年来从未尝试的跨域跳跃。菲尔兹奖得主 Tim Gowers 公开将其称为"AI 数学的里程碑"。

更值得关注的是节奏：上月 DeepMind 还在主张"AI 数学家"五年内才能独立攻克 Erdős 级别问题，OpenAI 此次直接把时间表压缩为零。Anthropic Jack Clark 在牛津所言"12 个月内 AI 将拿出诺贝尔级突破"，正在从预测变成趋势线的延长。

**点评：** 这是 AGI 实证派最有力的一份"业绩单"——当模型能在数学家最骄傲的领地原创性地解决百年悬案，关于 LLM "只是统计模式"的反对意见正在快速失声。下半年将密切关注哪一项物理/化学猜想率先被"按下回车键"。

---

### 🛡️ No.2 · 特朗普废 AI 安全令、Anthropic 写"智能爆炸"——美国监管"右脚刹车 左脚油门"

**[BuildFastWithAI](https://www.buildfastwithai.com/blogs/ai-news-today-may-23-2026)**

白宫 5 月 23 日宣布废除上届政府遗留的 AI 安全行政令，该命令原本要求所有前沿模型发布前进行 90 天审查并向 NIST 提交红队报告。废除的直接推手是马斯克、扎克伯格、David Sacks 三人联合致信特朗普，理由是"延缓 AI 发展会令美国失去对华优势"。

讽刺的是，同一天 Anthropic 发布的最新研究议程首次正式收录"intelligence explosion"（智能爆炸）这一历来仅在理论圈出现的术语，并给出明确概率：2028 年底前有 60%+ 概率出现递归自我改进。联创 Jack Clark 在牛津更进一步——承认 AI 灭绝人类风险"非零"，与白宫的乐观节奏构成鲜明对比。

这种"政府松绑 + 实验室加码警告"的撕裂正在成为 2026 年特征：欧盟 5 月 7 日通过 AI Act 简化修正案、各成员国按计划在 8 月 2 日前设立沙盒；中国继续"放发展、紧管控"双轨；美国则把决定权从合规岗位转向实验室自身。

**点评：** 当政策真空成为常态，"前沿实验室自我监管"将成为下一轮舆论焦点——Anthropic 主动写智能爆炸进议程是占据道德高地的明智防御性动作，OpenAI/xAI 是否跟进将决定监管节奏从 H2 起的方向。

---

### 💰 No.3 · NVIDIA 单季净利 583 亿、回购 800 亿——AI 资本周期还没拐头

**[Al Jazeera · Nvidia 创纪录利润](https://www.aljazeera.com/economy/2026/5/21/nvidia-posts-record-profit-and-revenue-amid-ai-chip-boom)**

NVIDIA FY2026 Q1（2–4 月）报出 816 亿美元营收（同比 +85%、环比 +20%）和 583 亿美元净利润（同比 +200%+），EPS 1.87 美元，全面超出华尔街预期。数据中心业务单季 752 亿美元（同比 +92%），下季指引 910 亿美元，再度叫板"AI 资本开支见顶论"。

最值得品味的是配股动作：800 亿美元回购 + 每股股息加 1 美分，承诺将 2026 年自由现金流约一半返还股东。这是黄仁勋在 1) Blackwell 已彻底锁定一年期产能、2) Rubin 即将进入预订窗口的双重确定性下，对市场释放"现金流足够支撑双线投入"的强信号。

更宏观的对照：OpenAI 同期完成 1,220 亿美元融资（投后 8,520 亿美元）、Anthropic 拿下 Google 400 亿美元承诺、Meta 资本开支指引区间上调至 1,150–1,350 亿——三大客户的资本支出曲线全部上行，NVIDIA 单 GPU 折旧周期仍在被市场"按 18 个月"重新定价。

**点评：** 想看 AI 周期顶点的人，请把日历翻到 Rubin Ultra 货架的那一刻；在此之前任何关于"过度投资"的叙事都要先穿过 NVIDIA 这道 910 亿美元的下季指引。

---

### 🔪 No.4 · Anthropic 抢下 Stainless：Agent 时代 SDK 即基础设施

**[TechCrunch · Anthropic 收购 Stainless](https://techcrunch.com/2026/05/18/anthropic-has-acquired-the-dev-tools-startup-used-by-openai-google-and-cloudflare/)**

Anthropic 5 月 18 日宣布以超 3 亿美元收购 SDK 工具商 Stainless，标的之前是 Sequoia 与 a16z 押注、为 OpenAI、Google、Cloudflare、Replicate、Runway 等同时输出 SDK 的核心中间件供应商。交易完成后，Stainless 的工具未来仅服务 Anthropic 自家产品。

读懂这次收购需要切换到 Agent 视角：当模型不再只是 Chatbot，而要主动调用 Canva、Instacart、OpenTable、Vercel、S&P Global 等数百个外部服务时，SDK 的生成质量、版本兼容、错误回放就直接决定了 Agent 的可靠性。Stainless 等于 Agent 时代的"水电网"，Anthropic 砸 3 亿截胡的本质，是把对手赶回手写 SDK 的"高摩擦"赛道。

放在更长的叙事里，这是继 Anthropic 拿下 Google 400 亿美元算力承诺、推出 MCP 协议成为事实标准之后的又一次"基础设施圈地"。OpenAI 当下不缺资金，但要在 Stainless 缺位后维持相同 SDK 体验，须自建团队或在二级市场寻找替代——这都是时间和摩擦。

**点评：** 模型层正在快速商品化，下一轮护城河属于 Agent 调用链的"管道工"——Anthropic 用 3 亿美元换的不是技术，是对手 12 个月的研发延迟。

---

### 🚨 No.5 · 一周内两起 AI 生态供应链攻击，"投毒插件"成为新常态

**[BuildFastWithAI](https://www.buildfastwithai.com/blogs/ai-news-today-may-23-2026)**

5 月 23 日披露的两起事件让"AI 编程供应链"风险一夜成显学：(1) VS Code 的 Nx Console 扩展被植入恶意载荷，仅 18 分钟即被发现并下架，但已外泄 3,800 个内部仓库，含 Claude 配置文件、AWS Key、GitHub Token 与企业凭据；(2) 一个被命名 TeamPCP 的组织通过 170+ 个 npm 包发起协同攻击（CVE-2026-45321，CVSS 9.6），受害名单包括 OpenAI、Mistral AI 与欧盟委员会。

两起事件共同特征是"模型即攻击面"：攻击者并不直接打模型本身，而是污染开发者日常调用 LLM API 时的中间件，再借助 AI Coding Agent 自动化扩散。OpenAI 因此宣布 6 月 12 日吊销 macOS App 全部签名证书，要求所有用户重新安装客户端——这是 OpenAI 历史上规模最大的一次客户端层面紧急响应。

**点评：** 当 80% 的开发者把 Cursor/Claude Code 作为默认入口，"投毒一个 VS Code 扩展 = 黑掉 3,800 个仓库" 的攻击 ROI 高得无可抗拒；2026 H2 注定迎来 AI Coding 工具层的"凭据隔离"标准之争。

---

## 行业观察

今天最强的隐线是**"研究突破、监管退潮、安全事故"三件事同日发生**——这并非巧合，而是 AI 飞轮加速到一定阈值的必然副产品：模型能力越是接近"原创科研"门槛，资本与政治压力越倾向于"放手让美国先跑"，而供应链 / Agent 调用链等周边基础设施在赛跑中暴露的裂缝就越多。

竞争格局上，Anthropic 通过 Stainless 收购 + MCP 协议 + 智能爆炸研究议程，正在完成"基础设施 + 安全话语权"双轴卡位；OpenAI 凭 1,220 亿美元弹药与 Erdős 级证明继续维持"能力第一"叙事；Google 用 Gemini Spark + 第三方 MCP 全面发力 Agent 落地；xAI 5 月一气推 4 款产品但仍未跨出"高速跟随者"区间。

下一周值得追踪：(1) 是否再有 AI 自主完成的科研突破登《Nature》；(2) 白宫废令后，加州、欧盟会否补位填空；(3) Cursor、Replit 等 AI 编程入口在供应链事件后会否出台凭据隔离协议；(4) NVIDIA Rubin 量产时间表是否被 Q1 财报推前。

---

*数据截至 2026-05-24 17:00 UTC+8；本报告仅供研究参考，不构成投资建议。*
