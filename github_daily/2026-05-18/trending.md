# GitHub Trending 日报 · 2026-05-18

## 今日焦点

> **个人 AI 超级智能 · Agent Skills 注册表大爆发 · CLI 优先 · 安全 Agent 落地 · 自托管反 SaaS 浪潮**
>
> - `tinyhumansai/openhuman` 单日 +1,694⭐ 登顶，Rust 写的私有"个人 AI 超脑"。
> - `tech-leads-club/agent-skills` 单日 +923⭐，押注 Skill 注册表生态成为下一代包管理器。
> - `K-Dense-AI/scientific-agent-skills` +764⭐，学科级 Skill 集合直接奔企业 RAG 替代品。
> - `Anil-matcha/Open-Generative-AI` +704⭐，主打"零内容过滤 + MIT + 200 模型"——闭源 AI 视频平台的暗黑面镜像。
> - `KeygraphHQ/shannon` +213⭐，自动渗透 Agent 把白盒 + 真实 exploit 链做成产品。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) | 私有、简洁、强大的个人 AI 超级智能 | Rust | 12,831 | +1,694 | 1,100 |
| 2 | [tech-leads-club/agent-skills](https://github.com/tech-leads-club/agent-skills) | 验证过的安全 Skill 注册表 | TypeScript | 3,438 | +923 | 314 |
| 3 | [oven-sh/bun](https://github.com/oven-sh/bun) | 极速 JS 运行时 / 打包 / 测试一体 | Rust | 91,672 | +908 | 4,574 |
| 4 | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) | 科研、工程、金融等学科级 Skill 集 | Python | 23,748 | +764 | 2,531 |
| 5 | [Anil-matcha/Open-Generative-AI](https://github.com/Anil-matcha/Open-Generative-AI) | 200+ 模型免审查生成式 AI 工作室 | JavaScript | 14,986 | +704 | 2,577 |
| 6 | [calcom/cal.diy](https://github.com/calcom/cal.diy) | 通用日程基础设施 | TypeScript | 43,186 | +425 | 13,383 |
| 7 | [BigBodyCobain/Shadowbroker](https://github.com/BigBodyCobain/Shadowbroker) | 公司飞机/卫星/地震情报 + AI 关联 | Python | 6,984 | +405 | 1,098 |
| 8 | [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | 让任何软件具备 Agent 原生能力 | Python | 35,486 | +306 | 3,472 |
| 9 | [dograh-hq/dograh](https://github.com/dograh-hq/dograh) | 开源语音 Agent 平台 | Python | 1,567 | +236 | 350 |
| 10 | [NirDiamant/agents-towards-production](https://github.com/NirDiamant/agents-towards-production) | GenAI Agent 生产级教程 | Jupyter | 19,858 | +225 | 2,641 |
| 11 | [knadh/listmonk](https://github.com/knadh/listmonk) | 高性能自托管邮件列表系统 | Go | 20,515 | +222 | 2,139 |
| 12 | [KeygraphHQ/shannon](https://github.com/KeygraphHQ/shannon) | 白盒自动渗透 AI Agent | TypeScript | 42,636 | +213 | 4,867 |
| 13 | [TryGhost/Ghost](https://github.com/TryGhost/Ghost) | 独立出版与订阅平台 | JavaScript | 53,221 | +209 | 11,604 |
| 14 | [medusajs/medusa](https://github.com/medusajs/medusa) | 灵活的电商平台 | TypeScript | 33,401 | +200 | 4,458 |
| 15 | [Light-Heart-Labs/DreamServer](https://github.com/Light-Heart-Labs/DreamServer) | 全栈本地 AI（LLM、语音、RAG、绘图）| Python | 1,085 | +89 | 200 |

---

## 重点项目点评

### 🥇 [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) — 今日榜首，+1,694⭐

**"个人 AI 超级智能"的 Ollama 时刻？**

OpenHuman 用 Rust 写了一个号称"个人级超级智能"的本地框架，主打三个关键词：私有、简洁、强大。从社区反馈看，它真正吸引人的不是模型本身（其实是一个胶水层），而是"一行命令把多模型 + 长期记忆 + Tool Use 串起来"的工程整合度，外加 Rust 二进制带来的部署体验。

为什么 1,694 颗星集中在今天？因为今天 HN 同时在讨论"Apple Silicon 比 OpenRouter 还贵"和"AI 订阅是定时炸弹"——本地 AI 阵营情绪正盛。OpenHuman 这种"一个 binary 跑完所有事"的范式正好踩在这个情绪上。

更深层看，这是 Ollama / LM Studio 路线的下一步：从"在本地起一个模型"升级到"在本地起一个有记忆、有工具、有 Agent 的 AI 操作系统"。短期内会涌出几十个同类项目，能活到 2027 年的取决于谁先把 Skill 生态接通。

---

### 🥈 [tech-leads-club/agent-skills](https://github.com/tech-leads-club/agent-skills) — +923⭐

**Skill 注册表正在变成 Agent 时代的 npm**

这个仓库是一个"经过验证、安全签名"的 Skill 注册中心，目标是给 Claude Code、Cursor、Copilot、Antigravity 等编码 Agent 提供可信任的 Skill 来源。卖点不是"我也有 Skill 仓库"，而是"我做了签名校验、依赖审计和兼容性测试"。

Anthropic 在去年底正式把 Skill 作为顶层概念之后，Skill 生态进入了"100 个仓库都说自己是中心"的混乱期。任何能解决"我装的 Skill 会不会偷我代码"这个问题的项目，都有变成事实标准的机会——这就是为什么它能在一天内吸 923 颗星。

值得关注：与第 4 名的 `scientific-agent-skills` 是合作还是竞争——一个是横向（注册表 / 工具链），一个是纵向（学科内容），如果两者能互相引用，就构成了 Agent 包管理的早期雏形。

---

### 🥉 [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) — +764⭐

**学科级 Skill 把"小聪明 Agent"推向"专业助手"**

这个集合涵盖科研、工程、金融、写作等纵深领域，每个 Skill 不是几行 prompt，而是"工具调用 + 知识载入 + 评估 rubric"的成品。它今天爆涨的关键，是当 Anthropic Skills 机制成熟后，开发者意识到"通用 Agent"已经卷不动，纵向专业化才是差异点。

如果你要让 Claude Code 做"债券现金流分析"或"差速气相色谱实验设计"，从零写 Skill 太慢，从这个仓库里挑一个跑通再迭代，是最现实的路径。这意味着仓库本身会迅速从"代码集合"演化成"知识载体" + 评测 benchmark。

下一步看点：是否会出现学科 Skill 的"打包发行"机制（比如医药 Skill 包 / 量化 Skill 包），从而让企业能像装 Linux 发行版一样装"Agent 发行版"。

---

### 🏅 [Anil-matcha/Open-Generative-AI](https://github.com/Anil-matcha/Open-Generative-AI) — +704⭐

**200 模型 + 零审查：闭源生成平台的暗黑镜像**

这是一个 MIT 许可的自托管图像/视频生成"工作室"，集成了 Flux、Midjourney、Kling、Sora、Veo 等 200+ 模型。卖点写得非常直白：「No content filters」「Self-hosted」「Open-source alternative」——直接对标 Runway、Pika、Sora 的限制。

它的爆涨是一个值得警觉的信号：随着监管收紧（参考今天欧盟 AI Act 12 月 2 日水印强制），创作者社区会用脚投票，把"无审查 + 可控部署"作为反抗信号。同时这也是一个法律灰区项目，能否长期存在取决于上游模型权重合规性以及部署者的本地法律。

对企业用户的启示：这种模式不会替代主流商业平台，但会作为"内部沙盒"被许多公司私下部署用于素材原型设计。

---

### 5️⃣ [KeygraphHQ/shannon](https://github.com/KeygraphHQ/shannon) — +213⭐

**白盒自动渗透 Agent：把 Mythos vs Daybreak 的故事开源化**

Shannon Lite 把"读源码 → 识别攻击面 → 自动构造 exploit → 验证可利用"这一条线做成开源 Agent。与今天 AI 圈的 Anthropic Project Glasswing / OpenAI Daybreak 主线呼应，但走的是社区路线。

它的关键差异在"白盒"二字——给它你的源码，它输出真实 PoC 而不是 SAST 报告。这意味着安全工程师能直接拿它做 CI 集成，把"准生产代码"在合并前过一遍。讨论里最尖锐的问题是：这个能力是否会被攻击方更快利用？答案显而易见——所以高质量的红队/蓝队同步部署会成为下一阶段的标配。

---

## 生态观察

今天 trending 几乎被两个浪潮主导：**Agent Skills 生态**（2、4、8、10）和 **本地 AI 自托管**（1、5、15）。前者反映的是 Anthropic Skill 标准开始把"Agent 商店"做成可投资的赛道；后者反映的是 AI 订阅经济压力下，开发者主动寻找替代方案。

值得注意的反方向是 Bun（第 3 名）+908⭐，传统 JS 基础设施仍在加速；以及 Ghost、Medusa、Listmonk 三个老牌自托管 SaaS 替代品同时上榜——这是"反订阅"叙事在非 AI 领域的延伸。

明日预测：随着 Anthropic Code Mythos 和 OpenAI Daybreak 的进一步细节披露，安全 Agent 这一垂直方向（Shannon、Shadowbroker）会继续吸星；同时 OpenHuman 之类"个人 AI OS"项目可能迎来 fork 潮，社区会很快开始辩论"哪种本地 Agent 框架成为下一个 Ollama"。
