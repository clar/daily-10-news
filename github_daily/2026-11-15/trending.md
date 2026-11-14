# GitHub Trending 每日报告 · 2026-11-15

## 今日焦点

> **Coding Agent 工具链爆发 · Claude Skills 生态落地 · Chrome / Google 系统性入场 · 代码审查 AI 化 · 自托管财务工具抬头**
>
> - `GoogleChrome/modern-web-guidance-src` 单日 **+1,225⭐**：Google 正式给 Coding Agent 下发"现代 Web 规范"参照系。
> - `tradermonty/claude-trading-skills` **+556⭐**：面向股票投资者的 Claude Code Skills 包，Skills 生态开始出现"垂直职业包"。
> - `alibaba/open-code-review` **+897⭐**：阿里开源混合式代码审查系统，流水线 + LLM Agent 双模。
> - `ChromeDevTools/chrome-devtools-mcp` **+673⭐**：Chrome DevTools 全面 MCP 化，浏览器调试成为 Agent 的"手眼"接口。
> - `backnotprop/plannotator` **+412⭐**：Agent 工作的"规划 + 标注 + 评审"工作台，Human-in-the-loop 工具产品化。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [backnotprop/plannotator](https://github.com/backnotprop/plannotator) | Agent 工作规划、标注、评审并反馈的协作面板 | TypeScript | 11,073 | +412 | — |
| 2 | [GoogleChrome/modern-web-guidance-src](https://github.com/GoogleChrome/modern-web-guidance-src) | 让 Coding Agent 跟上现代 Web 最佳实践 | TypeScript | 5,947 | +1,225 | — |
| 3 | [tradermonty/claude-trading-skills](https://github.com/tradermonty/claude-trading-skills) | 面向股票投资者的 Claude Code Skills 合集 | Python | 4,760 | +556 | — |
| 4 | [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) | Chrome DevTools 的 MCP 实现 | TypeScript | 56,255 | +673 | — |
| 5 | [alibaba/open-code-review](https://github.com/alibaba/open-code-review) | 混合流水线 + LLM Agent 的代码审查工具 | Go | 51,384 | +897 | — |
| 6 | [QwenLM/qwen-code](https://github.com/QwenLM/qwen-code) | 终端里运行的开源 AI Coding Agent | TypeScript | 30,303 | +116 | — |
| 7 | [dream-num/univer](https://github.com/dream-num/univer) | 构建 AI 办公套件（编辑/计算/协作）的 SDK | TypeScript | 24,445 | +495 | — |
| 8 | [ag-ui-protocol/ag-ui](https://github.com/ag-ui-protocol/ag-ui) | Agent–前端交互协议 | TypeScript | 17,332 | +9 | — |
| 9 | [ashhart/TensorFold](https://github.com/ashhart/TensorFold) | 面向 Metal / CUDA / Vulkan 的 LLM 推理引擎 | Zig | 2,148 | +53 | — |
| 10 | [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) | "穴居人式"简短回复代理代理，号称省 65% token | Go | 120,030 | +227 | — |
| 11 | [louislam/uptime-kuma](https://github.com/louislam/uptime-kuma) | 自托管监控工具 | JavaScript | 94,213 | +432 | — |
| 12 | [we-promise/sure](https://github.com/we-promise/sure) | 开源个人财务应用 | Ruby | 15,264 | +659 | — |
| 13 | [Tencent/LoopForge](https://github.com/Tencent/LoopForge) | 自托管工作流，编排 CodeBuddy / Codex / Claude Code | Go | 866 | +101 | — |
| 14 | [Likely7/Veyra-NRVideo](https://github.com/Likely7/Veyra-NRVideo) | Windows 端 AI 超分 + 插帧视频播放器 | C++ | 2,188 | +423 | — |
| 15 | [martin-olivier/airgorah](https://github.com/martin-olivier/airgorah) | WiFi 安全审计工具 | Rust | 5,815 | +269 | — |

---

## 重点项目点评

### 🥇 [GoogleChrome/modern-web-guidance-src](https://github.com/GoogleChrome/modern-web-guidance-src) — 今日新增 +1,225⭐

**Google 入场"Agent 教材"赛道：谁定义"现代 Web"，谁就掌握下一代前端默认值**

这个仓库本质上是 Google Chrome 团队为 Coding Agent（Claude Code、Cursor、Qwen Code 等）编写的"现代 Web 实践知识库"，涵盖 Core Web Vitals、INP 指标、Baseline 2026 可用 API、CSS @scope / anchor positioning 这些 2026 年"应当默认启用"的新特性。它不是普通文档站，而是被设计为 Agent 直接检索的结构化上下文。

今天 1,225⭐ 单日增长意味着开发者已经意识到：**Agent 生成的代码实际默认值，正在被几家科技公司"规范化"地写进上下文包**。Google 做 Web 规范、Anthropic 做 Code Skills、各家都在抢 Agent 的"默认知识图谱"。谁的 guidance 被 Agent 消费得多，谁就事实上成为下一代前端生态的隐性 BDFL。

这类项目值得前端社区高度关注——它不只是"又一个文档站"，而是 **Coding Agent 时代的"事实标准编写权"争夺战**。

---

### 🥈 [alibaba/open-code-review](https://github.com/alibaba/open-code-review) — 今日新增 +897⭐

**代码审查 AI 化的"企业落地样板"**

阿里开源的混合代码审查系统：用确定性流水线处理 lint / 安全 / 规范这些可枚举规则，用 LLM Agent 处理语义级 review（设计建议、潜在 bug、可读性建议），最后以行级评论的形式回写到 PR。支持多语言规则集，与 GitLab / Gerrit / GitHub 都可以集成。

今天的 +897⭐ 说明"AI Code Review"从 2023 年的概念验证阶段彻底走到了生产级工具链阶段。亮点在于它的**双模架构**：让确定性规则和 LLM 判断各司其职，而不是让 LLM 吃掉所有流程。这种"规则 + Agent"的拆分正逐渐成为 2026 年企业落地 AI 工程工具的标准模式。

对国内团队的意义尤其大：它既有阿里规范的本地化支持，又能接入 Qwen / 千问系列模型，为国内 toB 的"AI DevOps"提供了一个高质量开源基座。

---

### 🥉 [tradermonty/claude-trading-skills](https://github.com/tradermonty/claude-trading-skills) — 今日新增 +556⭐

**Claude Skills 生态的"垂直职业包"现象**

一个专为股票投资者设计的 Claude Code Skills 合集：覆盖市场分析、技术形态、Screener、策略开发等全套工作流。使用方法是把这个 repo 放进 `~/.claude/skills/`，Claude 就能直接调用"今天美股财报日历"、"RSI 过热 screening"、"回测策略"等结构化技能。

这标志着 Anthropic 的 Skills 生态进入"垂直职业包"阶段——继 `anthropic-skills/*` 官方包之后，社区开始输出面向特定职业角色的 Skills 合集。可以预见接下来会出现：律师、医生、教师、内容创作者、运营等各类"职业 Skills 包"。

**Skills 的生态位实际上介于 ChatGPT GPTs 和插件市场之间**：它可组合、可继承、可覆盖，且与 Claude Code 的 agent loop 深度绑定。tradermonty 这个包能上榜，说明 **Skills 已经进入"社区内容创作者变现"的早期阶段**。

---

### 🏅 [backnotprop/plannotator](https://github.com/backnotprop/plannotator) — 今日新增 +412⭐

**Human-in-the-loop 的"Agent 工作台"产品化**

plannotator 是一个专门为"审阅 Agent 工作"而设计的网页工作台：Agent 的计划、中间产物、diff 都可以被可视化地标注，人工反馈再按结构化格式回流给 Agent。这种"Agent 外挂一个人类编辑器"的模式，在 Cursor / Claude Code 内置 approval UI 之外，首次有了独立产品形态。

它的意义不在于技术多新，而在于**形态选择**：承认 Agent 不能全自动，并把"人工监督"做成一个常驻工作台，而不是弹窗式审批。随着 Agent 执行时长从秒级进入分钟 / 小时级，这类"后台任务 + 人工检视面板"的产品会变多。

---

### 🏅 [ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) — 今日新增 +673⭐

**浏览器调试工具正式成为 Agent 的"手眼"**

Chrome DevTools 官方 MCP server：Agent 可以通过标准协议调用 DOM / 网络面板 / Performance 录制 / 控制台命令等能力。意味着 Claude、Cursor、Codex、Qwen Code 等都能在"写完前端代码"之后，**自己打开浏览器，自己跑 Performance 分析，自己调试**。

这是 2026 下半年 Coding Agent 工具链一个重要的分水岭：Agent 不再被限制在"写代码 + 跑 CLI"，而是获得了**完整的浏览器自省能力**。配合今天上榜的 modern-web-guidance，Google 的意图越来越清晰：把 Chrome 变成 Agent 时代的"事实上的开发环境"。

---

## 生态观察

**今天的 Trending 可以浓缩成四个关键词：Agent 工作台、Skills 生态、浏览器接入、企业级 Code Review。**

- **Agent 工具链进入"工作台时代"**：plannotator、LoopForge、chrome-devtools-mcp、open-code-review 都是围绕 Agent 的"周边工具"，而非 Agent 本身。这个分层清晰的产品矩阵出现，说明 Coding Agent 市场在从"模型 war"转入"应用 war"。
- **Claude Skills 生态进入垂直化**：tradermonty 的 trading skills 包和 Tencent LoopForge 都在证明 Skills + MCP 双协议组合正在成为"Agent 可组合化"的默认底座。
- **Google / Alibaba / Tencent 三家开始"开源教材化"**：Chrome 下发 Web 规范、阿里下发 Code Review 流程、腾讯下发 Agent 编排模板——大厂通过开源项目向 Agent 投递"默认知识"的现象明显增多。
- **非 Agent 类长青项目仍坚挺**：uptime-kuma、sure、univer、airgorah——每天 Trending 榜单都留有 30% 左右位置给"工匠级自托管工具"，这也是 GitHub 生态健康的一个风向标。

一句话总结：**2026 年 11 月的 GitHub Trending，正在讲一个"Agent 外围工具链爆发"的完整故事**。
