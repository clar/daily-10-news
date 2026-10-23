# GitHub Trending 日报 · 2026-10-24

## 今日焦点

> **Claude Skills 生态爆发 · NVIDIA 开源 Agent 安全运行时 · PHP 核心仍是最热主语言之一 · AI Agent 安全/红队工具链全面开花 · 中文传统命理学遇见 TypeScript**
>
> - `cloudflare/security-audit-skill` **+2,706⭐** — Cloudflare 开源多阶段安全审计 Skill，Claude Skills 生态首个"官方级"项目冲上第一。
> - `NVIDIA/OpenShell` **+1,240⭐** — Rust 写的"自主 AI Agent 安全运行时"，NVIDIA 亲自下场做 Agent sandbox。
> - `php/php-src` **+722⭐** — PHP 核心仓库罕见挤入第二，8.5 发布节点驱动。
> - `anthropics/knowledge-work-plugins` **+643⭐** — Anthropic 为 Cowork 推出的知识工作插件集合，直接官方加持。
> - `SnailSploit/Claude-Red` **+209⭐** — 攻击性安全 Skills 组合包，与 Cloudflare 的审计 Skill 一起把"Claude Red/Blue Team"做成了双生生态。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) | 面向 Coding Agent 的多阶段安全审计 Skill，输出可机器读取的发现项 | JavaScript | 42,029 | +2,706⭐ | 2,628 |
| 2 | [php/php-src](https://github.com/php/php-src) | PHP 解释器核心代码 | C | 41,545 | +722⭐ | 8,357 |
| 3 | [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) | 面向知识工作者的 Claude Cowork 开源插件集 | Python | 32,180 | +643⭐ | 3,569 |
| 4 | [NVIDIA/OpenShell](https://github.com/NVIDIA/OpenShell) | 面向自主 AI Agent 的安全、私有运行时 | Rust | 18,739 | +1,240⭐ | 1,881 |
| 5 | [Renhuai123/ziwei-doushu](https://github.com/Renhuai123/ziwei-doushu) | 开源紫微斗数排盘引擎（算法 + 四化系统 + 古籍数据） | TypeScript | 6,832 | +547⭐ | 1,403 |
| 6 | [SnailSploit/Claude-Red](https://github.com/SnailSploit/Claude-Red) | 为 Claude 整理的攻击性安全 SKILL.md 技能库 | Python | 8,425 | +209⭐ | 1,095 |
| 7 | [OpenBMB/VoxCPM](https://github.com/OpenBMB/VoxCPM) | VoxCPM2：无 tokenizer 的多语种 TTS，支持 voice design 与 cloning | Python | 40,227 | +144⭐ | 4,573 |
| 8 | [nodejs/node](https://github.com/nodejs/node) | Node.js JavaScript 运行时 | JavaScript | 122,835 | +93⭐ | 39,849 |
| 9 | [sindresorhus/awesome](https://github.com/sindresorhus/awesome) | 全领域 Awesome 列表的根仓库 | Markdown | 523,636 | +900⭐ | 37,709 |
| 10 | [supabase/supabase](https://github.com/supabase/supabase) | 开源 Postgres 开发平台，适配 Web/Mobile/AI | TypeScript | 113,775 | +440⭐ | 16,950 |
| 11 | [yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp) | 功能最丰富的命令行音视频下载器 | Python | 200,943 | +384⭐ | 17,535 |
| 12 | [f/prompts.chat](https://github.com/f/prompts.chat) | Prompt 分享/自托管平台（原 Awesome ChatGPT Prompts） | HTML | 174,237 | +242⭐ | 22,265 |
| 13 | [mitmproxy/mitmproxy](https://github.com/mitmproxy/mitmproxy) | 交互式 TLS 中间人代理 | Python | 46,254 | +202⭐ | 4,873 |
| 14 | [donnemartin/system-design-primer](https://github.com/donnemartin/system-design-primer) | 系统设计学习与面试资料集 | Python | 375,334 | +175⭐ | 58,953 |
| 15 | [coollabsio/coolify](https://github.com/coollabsio/coolify) | 自托管 Vercel/Heroku 替代方案 | PHP | 63,591 | +118⭐ | 5,720 |

---

## 重点项目点评

### 🥇 [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) — 今日榜首，+2,706⭐

**Claude Skills 从社区实验走向大厂背书**

Cloudflare 开源了一个"安全审计 Skill"，为 Coding Agent（主要是 Claude Code）提供可复用的多阶段审计工作流：先遍历仓库变更面、再按 OWASP 分类扫描、再做跨文件数据流推理、最后输出机器可读的 JSON 发现项（含严重性、复现路径、修复建议）。它不是一个新的扫描器，而是**把一次完整的审计流程拆成了一组 Agent 可编排的 Skill 子程序**，并在 README 里给了 90% 以上的审计流程做了确定性包装（即明确工具调用顺序而非让 LLM 自由发挥）。

它一上来就冲到 +2,706⭐ 的原因有两个：（1）**Cloudflare 是第一个把 Skills 这种"小而专的 agent 原语"做到生产级的头部云厂商**，这让社区看到 Skills 可能从玩具变成产品的信号；（2）与过去一周 Claude Skills Marketplace 的内测节奏吻合——先放工具，再放 Skill 库，再放大厂级 Skill，节奏明确。

生态侧的信号比项目本身更重要：**Cloudflare、Anthropic、Snaisploit 的 Skill 仓库同一天冲榜前七**，意味着 "SKILL.md" 已经事实上成为 2026 下半年 Agent 生态里的新 package 单位，很可能走向类似 npm/pip 的开放协议。

---

### 🥈 [NVIDIA/OpenShell](https://github.com/NVIDIA/OpenShell) — +1,240⭐

**NVIDIA 自己下场做 Agent 的"安全壳"**

一个用 Rust 写的 "safe, private runtime for autonomous AI agents"——定位上非常接近 E2B、Daytona、Modal 这些"Agent 云"，但 NVIDIA 的差异在于：底座被设计成能本地运行、与 CUDA/NIM 深度集成，并把 syscall 过滤、文件系统写时克隆（CoW）、网络白名单、GPU memory sandboxing 都做在同一个 runtime 内。

NVIDIA 这个动作必须和 TechCrunch 本周报道的 **Daytona 独角兽（$1B 估值）** 一起读：**整个"Agent 执行环境"赛道刚诞生、就要被芯片厂商直接卷入**。差别是 Daytona 卖的是云端 SaaS、OpenShell 卖的是**让客户在自家数据中心装一个和 NIM 栈兼容的 agent sandbox**。这对企业 CIO 是极大诱惑：不出域、不走云厂商、GPU 利用率不损耗。

二级影响：**在"决策模型 + Agent 云 + Agent 运行时"这三件事上，2026 Q4 的头部玩家已经各就各位**——OpenAI 占前端决策、Daytona/E2B 占托管运行时、NVIDIA 占本地化运行时、Cloudflare 占 Skill 协议。接下来 6-9 个月的并购会很热闹。

---

### 🥉 [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) — +643⭐

**Cowork 时代的"官方插件库"**

Anthropic 开源了一个"面向知识工作者"的插件集，直接 PR 给 Claude Cowork（他们本周公开的"面向团队协作的 Claude 工作台"）。插件覆盖了律师、分析师、研究员、Product 等岗位的日常任务（文档审阅、财报抽取、决策日志等），全部以 Python Skills 的形式实现，并给出了可商用授权。

它冲到今日第 3 并不意外——**官方维护的"行业 Skill 包"等于把 Skills 这件事从个人 side project 推进到企业 B2B SaaS 的叙事**。你可以预期：（1）这个仓库会很快演化成 Anthropic 的"Skill Store 官方 reference"；（2）**律师 / 分析师 / HR 这类细分 vertical 的 Skill 市场一定会被创业公司瓜分**；（3）Claude Cowork 本身要和 ChatGPT Work（Uber 本周部署 30k 员工）正面肉搏。

---

### 🧮 [Renhuai123/ziwei-doushu](https://github.com/Renhuai123/ziwei-doushu) — +547⭐

**非典型"黑马"：中文命理学遇到 TypeScript**

今天最有话题性的黑马。这是一个开源紫微斗数（中国传统星命学）排盘引擎：从干支转换、宫位排布、四化神秘、三方四正，到古籍原文嵌入，全部用 TypeScript 实现并提供 npm 包。README 完全中文、测试用例覆盖"古今案例"。

它的爆火并非来自技术，而是来自**"用现代工程方法去严谨地实现一个古代系统"的审美快感**——HN 上有过八字排盘库走红，GitHub Trending 这次换成了紫微斗数。它反映的其实是一个很稳固的开发者文化趋势：**非主流知识的工程化在 2025–2026 这一轮里非常好融资/涨星**（看中医方剂库、佛教藏经库、梵语字典也都有类似节奏）。

---

### ⚔️ [SnailSploit/Claude-Red](https://github.com/SnailSploit/Claude-Red) — +209⭐

**Red Team Skills 库，和 Cloudflare 的 Blue Team Skills 当日同场**

今天榜单最微妙的组合：**第 1 的 Cloudflare 做"Blue Team / 防守审计 Skill"，第 6 的 Claude-Red 做"Red Team / 攻击能力 Skill"**。后者里包含 recon、payload gen、post-exploit 等常见 kill chain 阶段的 SKILL.md，并明确标注"仅限授权渗透测试、CTF 和防御研究"。

这类项目的出现 inevitably 会推动 Anthropic 对 Skill Marketplace 的内容审核政策做出收紧（预计很快会有类似 npm security review 的审查协议）。更深的信号是：**Claude 的 Skills 生态如果采用开放发布机制，天然会复刻 npm/PyPI 时期的"攻击者/防御者军备竞赛"**，这件事提前到来并不坏——社区被迫在很早期就讨论治理机制。

---

## 生态观察

- **Skills 生态的"创世日"**：今日 Top 15 中有 3 个直接是 Skill 仓库（Cloudflare、Anthropic、Claude-Red），一个是 Agent 运行时（NVIDIA OpenShell）——占了前 7 名中的四席，这是过去 180 天 Trending 榜上**最明确的一次"主题统治"**。
- **语言分布正在倾向 Rust / Python / TypeScript 三角**：传统霸主 JavaScript 位列第一，但其位置被 Cloudflare 的 agent 工具占据，而不是传统前端项目；C++/C 代表只剩 php-src 这类核心项目和 ONNX Runtime 这类基础设施。
- **"命理学 x TypeScript" 这类文化黑马**：说明 Trending 的推荐权重把"社会化传播"比"工程稀缺性"更放大了——仓库语言的分布正在部分反映 Twitter/X 和小红书的热度，而不只是开发者生产力数据。
- **AI Agent 安全是 2026 Q4 最拥挤的新赛道**：Cloudflare、NVIDIA、SnailSploit 分别占据防御、运行时、红队三端，而 OpenAI 本周也刚发了"训练环境安全"白皮书。Skill-based 的安全协议（SKILL.md 对外暴露的权限边界、工具调用白名单）很可能成为**接下来 90 天的产品标准化焦点**。

---

*数据来源：GitHub Trending (2026-10-24, Asia/Shanghai)。星数为当日 Trending 页快照，次日可能变化。*
