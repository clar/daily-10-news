# GitHub Trending 日报 · 2026-10-07

## 今日焦点

> **Agent 工具链继续霸榜 · 逆向工程 Agent 爆红 · Claude 生态外溢 · E2E 测试新秀 · DeepSeek 底层库再出手**
>
> - `morluto/rea` 一天 +2,963⭐，Agent 做"逆向工程任何东西"是今天最热的新概念；
> - `tester-army/e2e` 一天 +1,720⭐，E2E 测试框架首次出现一个 Agent-first 架构的挑战者；
> - `mattpocock/skills` 累计 27.8 万⭐、`thedotmack/claude-mem` 9.7 万⭐，Claude Code / Agent "技能库 + 记忆层"类项目成为开发者 workflow 标配；
> - `deepseek-ai/DeepGEMM` +363⭐，DeepSeek 继续向上游走，手写 GPU BLAS 内核库；
> - `cathrynlavery/diagram-design` 定位"编辑级示意图设计语言"，让 Agent 画出看得过去的图。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [morluto/rea](https://github.com/morluto/rea) | 用 Agent 逆向工程任何东西，从 App 行为到原生二进制 | TypeScript | 9,026 | +2,963 | 986 |
| 2 | [tester-army/e2e](https://github.com/tester-army/e2e) | 新一代 Web / 移动端 E2E 测试框架 | TypeScript | 6,215 | +1,720 | 274 |
| 3 | [DuarteSantos8/openGym](https://github.com/DuarteSantos8/openGym) | 自建健身房 / 自重训练追踪，排计划记日志 | JavaScript | 5,611 | +1,419 | 772 |
| 4 | [mattpocock/skills](https://github.com/mattpocock/skills) | 真·工程师 skills，直接从 `.agents` 目录拉 | Shell | 278,068 | +972 | 23,285 |
| 5 | [boykopovar/AnyPS5](https://github.com/boykopovar/AnyPS5) | PS5 可执行文件自动移植到 Linux / Windows | C++ | 6,377 | +943 | 464 |
| 6 | [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) | 一整套"AI 代运营"专家 agent | Shell | 157,782 | +621 | 25,440 |
| 7 | [earthtojake/text-to-cad](https://github.com/earthtojake/text-to-cad) | 给你的 Agent 装上 CAD 超能力 | Python | 17,939 | +620 | 1,797 |
| 8 | [pbakaus/impeccable](https://github.com/pbakaus/impeccable) | 让 AI 工具更会"设计"的设计语言 | JavaScript | 77,652 | +609 | 4,623 |
| 9 | [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | 跨平台 AI Agent 持久化上下文系统 | TypeScript | 97,128 | +536 | 8,555 |
| 10 | [deepseek-ai/DeepGEMM](https://github.com/deepseek-ai/DeepGEMM) | 干净高效的 GPU BLAS 内核库 | CUDA | 8,675 | +363 | 1,370 |
| 11 | [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) | 让 Agent 别把答案埋在底下的 skill | Python | 54,362 | +318 | 3,123 |
| 12 | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | Claude Code / Codex / Copilot / Pi 的编辑级示意图 | HTML | 43,986 | +227 | 2,840 |

---

## 重点项目点评

### 🥇 [morluto/rea](https://github.com/morluto/rea) — 今日榜首，+2,963⭐

**Agent 做逆向工程：从 App 行为一路戳到原生二进制**

Rea 是一个 Agent-first 的逆向工程框架：它接受"行为级问题"（例如"这个 app 在后台把什么数据发到哪里"），然后编排多个 Agent 分别去挂代理、注入 hook、反汇编原生 so/dylib、追 symbol、交叉引用，最后给出一份结构化报告。TypeScript 实现，核心是编排层，底层仍调用 Ghidra / Frida / mitmproxy 等既有工具。

它一天爆冲 +2,963⭐，一方面是因为它第一次把"逆向工程"这个传统上门槛极高、工具链极碎的领域包成了可对话工作流；另一方面也是因为它赶上了 2026 年 Q3 以来"Agent 做基础设施型工作"的新一轮热潮——继 OpenTPU 把 AI 推到硬件设计，Rea 把 AI 推到反汇编，社区正在用一个个"过去 10 年没人敢让 AI 碰"的领域给前沿模型做压力测试。

值得警惕的是：逆向工程本身是一把双刃剑，仓库里是否内置了 ToS / 法律边界检查、以及如何防止被用于盗版和恶意分析，将决定它能不能稳住社区信任。

---

### 🥈 [tester-army/e2e](https://github.com/tester-army/e2e) — +1,720⭐

**Agent-first E2E 测试：对 Playwright / Cypress 的首次有效挑战**

E2E 测试这个赛道，Playwright 和 Cypress 过去三年几乎是双寡头格局，没有人成功做出有真实采用的新项目。tester-army/e2e 的赌注在于：**测试脚本不再用 locator 和断言写出来，而是用自然语言描述场景，让 Agent 实时去找元素、规划交互、自愈 selector**。这对"UI 微调导致测试全挂"的痛点来说是降维打击。

今天 +1,720⭐ 的爆发主要来自前端工程社区——Tweet 和 Reddit 上几个 QA 大 V 推荐把它放进 CI 里跑 happy-path。但代码库目前只有 274 forks，和 Playwright 社区体量差 2-3 个数量级，真正要观察的是未来 2-4 周 CI 集成稳定性和假阳性率。

**信号**：E2E 测试是 2026 年 Agent 落地 ROI 最清晰的领域之一——它直接把人类 QA 的 flaky-test 维护成本转移到 Agent。如果这个 workflow 稳住，Playwright 必须跟进 Agent 模式。

---

### 🥉 [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) — +536⭐，累计 97,128⭐

**Claude 生态里的"记忆层"事实标准正在形成**

claude-mem 做的是跨会话、跨平台的 Agent 持久化上下文系统——简单说就是 Agent 的"长期记忆"。累计 9.7 万星，意味着这已经不是"周末尝鲜"项目，而是 Claude Code / Codex / 自写 Agent 工作流里几乎默认装的一块中间件。

这类项目今天同时霸榜的，还有 `mattpocock/skills`（27.8 万⭐，Skills 技能库）、`msitarzewski/agency-agents`（15.7 万⭐，专家 Agent 集合）、`ayghri/i-have-adhd`（5.4 万⭐，让 Agent 直截了当回答）、`cathrynlavery/diagram-design`（4.3 万⭐，为 Agent 优化的示意图语言）。合在一起看，一个完整的"Agent 中间件栈"正在社区自发涌现：**技能库（skills）+ 记忆层（claude-mem）+ 代理专家（agency-agents）+ 输出规范（i-have-adhd）+ 可视化（diagram-design）**。

这意味着：开发者不再把 Agent 当"API"，而是当"操作系统"——操作系统需要文件系统、调度器、驱动。社区在用开源方式替厂商把"操作系统"补齐。

---

### 🧮 [deepseek-ai/DeepGEMM](https://github.com/deepseek-ai/DeepGEMM) — +363⭐

**DeepSeek 的"从模型往硬件走"路线又进一步**

DeepGEMM 是 DeepSeek 开源的 GPU BLAS 内核库，针对低比特量化和 MoE 推理场景做了特定优化。相较于通用的 cuBLAS 或 cutlass，DeepGEMM 更像是"针对 DeepSeek V3/V4 架构反向定制"的内核。

过去一年 DeepSeek 已经先后开源了 DeepSeek-V3、DeepSeek-R1、FlashMLA、DeepEP、DeepGEMM，形成一条**"模型 → 推理引擎 → 底层算子"**完整开源栈。这是中国前沿模型团队第一次有能力自己端到端拥有软件栈——而不是像过去那样在 PyTorch + cuBLAS 之上做改造。

对社区的意义：这些算子库虽然初衷是服务 DeepSeek 自家模型，但由于细节公开，很快会被 Mistral、通义等其他开源模型借用，形成"开源派共享底层优化"的生态。

---

### 🎨 [pbakaus/impeccable](https://github.com/pbakaus/impeccable) — +609⭐，累计 77,652⭐

**让 AI 工具"懂设计"的设计语言：Agent UX 第一次有了行业规范雏形**

Impeccable 的定位很细——它是一个"喂给 AI harness 的设计语言规范"：规定了 Agent 产出 UI 时的组件间距、色阶、字号层级、交互反馈节奏。社区把它比作"Agent 时代的 Material Design"。

它上榜的原因不是功能复杂，而是**第一次把"Agent 产出 UI 质量不一致"这个痛点变成了一个可引用的规范文件**。Vercel v0、Cursor Composer、Replit Agent 3 等几家下游工具都在实验把 impeccable 作为输出约束。配合今天榜上 `cathrynlavery/diagram-design`（Agent 示意图规范），"Agent 产出的视觉资产"赛道正在标准化。

---

## 生态观察

今天的 trending 可以用一句话总结：**"Agent 操作系统"的中间件栈正在社区里成型**。

- **五大中间件齐聚一榜**：技能库（`mattpocock/skills` 27.8 万⭐）、记忆层（`claude-mem` 9.7 万⭐）、代理专家（`agency-agents` 15.7 万⭐）、输出规范（`i-have-adhd` 5.4 万⭐）、设计语言（`impeccable` 7.7 万⭐、`diagram-design` 4.3 万⭐）。这个组合第一次让人看见"开发者把 Agent 当 OS 来堆基础设施"的轮廓。
- **Agent 开始啃难的领域**：Rea（逆向工程）、text-to-cad（CAD 建模）、tester-army/e2e（E2E 测试）——都是过去"不敢让 AI 碰"的领域。2026 Q4 的爆点，可能是 Agent 从代码写作走向代码外的工程工作。
- **开源底层继续被 DeepSeek 顶**：DeepGEMM 是今年 DeepSeek 开源栈的第五个模块，这家中国实验室正把开源派的底层基础设施补起来——这对 Mistral、通义等开源模型是一张免费礼券。
- **工具型应用也有空间**：`openGym`（自建健身房 app）+1,419⭐，`AnyPS5`（PS5 到 Linux 的 porter）+943⭐，提醒我们 trending 不止是 Agent——有真实需求和具体受众的开发者工具一样能上榜。
- **冷门但重要**：没有 Rust 新项目上榜（和过去 6 个月的 Rust 密度相比是个短暂空窗），也没有 LLM 本体模型仓库出现——今天的焦点完全在上层工具链。
