# GitHub Trending · 2026-11-14

## 今日焦点

> **Agent 工具链持续称王 · 大厂加码代码安全 · 浏览器与 Web 平台知识底座 · 金融场景 LLM 应用 · 隐私自托管仍是硬刚需**
>
> - `alibaba/open-code-review` 阿里开源混合式代码审查工具，一天 +206⭐ 冲上第一，LLM + 规则双引擎直接对标 Copilot Review
> - `GoogleChrome/modern-web-guidance-src` Google、MDN、Chrome、Edge、Firefox 联合把"现代 Web 实践"包成 coding agent 可直接引用的模块，+1,875⭐
> - `openai/codex-security` OpenAI 新发安全漏洞 CLI + SDK，+754⭐，让 Codex 成为开发流水线里的"自动漏洞修复代理"
> - `we-promise/sure` 隐私自托管个人财务 app，+944⭐，开源替代 Mint / Monarch 一类商业产品的热度再度回暖
> - `tailscale/tailcat` Tailscale 版 netcat，+324⭐，重新定义开发者"内网穿透 + 一次性 TCP 工具"

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [alibaba/open-code-review](https://github.com/alibaba/open-code-review) | LLM + 规则引擎混合代码审查，内置 NPE / 并发 / XSS / SQLi 检查 | Go | 50,552 | +206 | 3,757 |
| 2 | [GoogleChrome/modern-web-guidance-src](https://github.com/GoogleChrome/modern-web-guidance-src) | 浏览器厂商联合输出的 coding agent 现代 Web 指引 | TypeScript | 4,753 | +1,875 | 265 |
| 3 | [openai/codex-security](https://github.com/openai/codex-security) | 用 Codex 查找、验证并修复安全漏洞的 CLI + SDK | TypeScript | 13,093 | +754 | 1,021 |
| 4 | [ZhuLinsen/daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis) | LLM 多市场股票分析，含仪表盘 + 推送 + 定时任务 | Python | 71,549 | +272 | 57,271 |
| 5 | [we-promise/sure](https://github.com/we-promise/sure) | 隐私自托管个人财务 app | Ruby | 14,692 | +944 | 1,112 |
| 6 | [backnotprop/plannotator](https://github.com/backnotprop/plannotator) | Agent 协作工作台：计划、批注、审查、反馈 | TypeScript | 10,420 | +100 | 783 |
| 7 | [louislam/uptime-kuma](https://github.com/louislam/uptime-kuma) | 自托管监控与 uptime 面板 | JavaScript | 93,825 | +61 | 8,721 |
| 8 | [block/buzz](https://github.com/block/buzz) | Rust 写的"蜂巢思维"通讯平台 | Rust | 37,284 | +95 | 4,941 |
| 9 | [tradermonty/claude-trading-skills](https://github.com/tradermonty/claude-trading-skills) | Claude Code 交易员技能：选股、绘图、策略 | Python | 4,130 | +60 | 859 |
| 10 | [tailscale/tailcat](https://github.com/tailscale/tailcat) | Tailscale 版 netcat，走数据面不走控制面 | Go | 9,423 | +324 | 429 |
| 11 | [Likely7/Veyra-NRVideo](https://github.com/Likely7/Veyra-NRVideo) | Windows 视频超分 + 插帧增强播放器 | C++ | 1,590 | +245 | 71 |
| 12 | [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) | Chrome DevTools 的 MCP Server，面向代码代理 | TypeScript | 55,428 | +145 | 4,602 |

---

## 重点项目点评

### 🥇 [alibaba/open-code-review](https://github.com/alibaba/open-code-review) — 今日榜首，+206⭐

**阿里把"规则引擎 + LLM"的代码审查工具链一次性开源，直接对标 Copilot Code Review**

这个项目把过去十年静态分析（NPE、线程安全、XSS、SQLi）和 2024 年以来 LLM 代码审查两个阵营拼接起来：先用规则流水线过第一道，再把剩下语义型问题交给 Agent 做行级点评。相比传统 SAST 工具，它的差异在于"评审意见与 git patch 行号绑定"；相比纯 LLM 方案，它又能保证低误报率。

它一上榜就冲到第一，并不只是阿里影响力——总星数 50K+、Fork 3.7K 说明这是已经在内部被大规模使用、如今才正式对外。本周 Google 发布 Modern Web Guidance、OpenAI 发布 Codex Security CLI，三家同一天把"面向代码代理的审查/规范"开源，标志着 **"Agent-native 代码治理"正成为 2027 年企业 DevOps 工具栈的默认模块**。

---

### 🥈 [GoogleChrome/modern-web-guidance-src](https://github.com/GoogleChrome/modern-web-guidance-src) — +1,875⭐

**Chrome / Edge / Firefox / MDN 联手，第一次把"现代 Web 实践"做成代理可消费的模块**

这是 11 月 10 日四大浏览器 + MDN 联合宣布的新项目的源仓：所谓 "one-line install"，就是开发者只需在 coding agent（如 Claude Code、Cursor、Copilot）中引入一行配置，它就能自动获取最新的 Web 平台兼容性、API 推荐用法以及反模式清单。

这件事的意义在于：以前"Web 最佳实践"散布在 MDN、Can I Use、Google Web.dev 之间；现在它被结构化为一个 Agent 可引用的知识文件。对于 2026 这一波 "Agent-first" 开发，Modern Web Guidance 近乎于浏览器厂商向代理生态投的第一张"统一规范"选票。今日 +1,875⭐ 几乎全部来自 Agent 工具链圈的转发。

---

### 🥉 [openai/codex-security](https://github.com/openai/codex-security) — +754⭐

**OpenAI 把 Codex 包装成"安全漏洞自动修复流水线"：发现 → 验证 → 修复三位一体**

OpenAI 很少直接出 CLI 工具，这次的 Codex Security 却是面向企业开发流程的完整产品：它封装了 SAST + Fuzzer + LLM 修复，通过 TypeScript SDK 嵌入 CI/CD。关键是它不是只给"报告"，而是直接提 PR，并用 Codex 回归测试其修复没有引入新 bug。

与阿里 open-code-review 定位互补：前者偏企业内部 code review 环节，后者偏 CI/CD 漏洞自动化。叠加 Microsoft "Lazarus" 后门研究（AI 日报同日）揭示仅 10 个神经元即可植入恶意，**"AI 做防御 + AI 制造威胁"的双向军备竞赛本周正式进入可观测阶段。**

---

### 🏅 [we-promise/sure](https://github.com/we-promise/sure) — +944⭐

**隐私自托管个人财务 app 的热度回潮，是对 Mint 关停后的"社区记忆"再激活**

Sure 用 Ruby + Rails 实现 Plaid 聚合 + 多账户资产追踪 + 规则引擎，功能对标 Monarch 和 Copilot Money。本次 +944⭐ 的驱动是作者本周重写了同步引擎，支持美股券商 + 加密钱包 + 多币种折算，把 Intuit 停掉 Mint 之后的"遗民"再次聚拢。

叠加 `ZhuLinsen/daily_stock_analysis`（LLM 多市场分析）+ `tradermonty/claude-trading-skills`（Claude 交易技能），**"个人金融 + AI" 已经成为 2026 开源趋势里最稳定的一条长尾**。它与去年相比的最大变化是：开发者不再只做"记账"，而是把自动化 + 代理 + 多市场数据组合进个人投资工作流。

---

### 🎖️ [tailscale/tailcat](https://github.com/tailscale/tailcat) — +324⭐

**Tailscale 做了一个只走数据面的 netcat，小而漂亮地回答了"控制面依赖"的老问题**

Tailscale 把 WireGuard 封装得非常成功，但长期被诟病"离线场景依赖 coordination server"。Tailcat 的思路是：数据面可独立运作，只做点对点 TCP/UDP，不触控制面。换句话说，它把 Tailscale 组网"降级到纯 crypto 通道"，让它在 CI 环境、短生命容器、离线调试里有了类 netcat 的工具形态。

对比今日 HN 热榜第 2 的 Coway 反向工程、第 11 的 Android 剪贴板绕过，**开发者正在以越来越细的粒度拆解"大厂基础设施"**：既要 Tailscale 的便利，又要 netcat 的独立；既要 Home Assistant 的自动化，又拒绝厂商云锁定。Tailscale 的聪明在于，它自己下场把这一把刀递给社区。

---

## 生态观察

今天的 GitHub Trending 呈现出 2026 年典型的**"Agent 工具链 + 平台方下场 + 隐私自托管"三线共进**：

- **大厂一致转向 Agent-native 工具链**：Alibaba Code Review、Google Modern Web Guidance、OpenAI Codex Security、Chrome DevTools MCP 四个仓同日进榜。平台厂商已经不再满足于"发大模型"，而是在为未来 coding agent 建立它们各自的"生态入口"。
- **Fintech + LLM 持续霸榜长尾**：Sure、daily_stock_analysis、claude-trading-skills 三者说明金融场景是开源 LLM 工具真正落地的高价值赛道。
- **隐私 / 自托管 / 本地化仍是刚需**：Uptime Kuma、Buzz、Sure 都在证实"反 SaaS"的长期趋势。
- **语言分布有意思**：今日 TypeScript 四项（都是 agent 工具）、Go 两项、Python 两项、Rust 一项。**TypeScript 已成为 2026 年 Agent 工具链的事实标准语言**，这对 Deno、Bun、Node 生态都意味着下一轮红利。

一个值得关注的"反向信号"：**纯 LLM 框架（LangChain / LlamaIndex 类）本周完全未进入 Trending**。开发者注意力正在从"框架"转向"业务工具"，这是 2026 年 Q4 开源 AI 生态最重要的拐点之一。
