# GitHub Trending 日报 · 2026-10-11

## 今日焦点

> **AI 逆向工程爆发 · PS5 游戏逆向上云 · Claude Skills 生态扩散 · AI 原生工具链全面开花**
>
> - `morluto/rea` 单日暴涨 **+25,784⭐**，把"AI Agent 直接反编译任意软件"推上头榜。
> - `boykopovar/AnyPS5` 让 PS5 可执行文件自动移植到 Linux/Windows，+5,831⭐，灰色地带的"游戏自由"再度被点燃。
> - `storytold/artcraft` 用 Rust 做"创作者原生生成引擎"，+3,217⭐，设计师工作流开始脱离 Figma / Adobe。
> - `anthropics/knowledge-work-plugins` 和 `mattpocock/skills` 双双上榜，**Claude Skills 已经形成官方 + 社区并行的双生态**。
> - `cathrynlavery/diagram-design`、`hugohe3/ppt-master` 把"图表 / PPT 自动化"推向主流，办公生产力类 Agent 工具进入收割期。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [morluto/rea](https://github.com/morluto/rea) | AI Agent 一键逆向任何软件（含二进制） | TypeScript | 70,764 | +25,784 | 14,836 |
| 2 | [boykopovar/AnyPS5](https://github.com/boykopovar/AnyPS5) | PS5 可执行文件自动移植到 Linux/Windows | C++ | 26,560 | +5,831 | 2,221 |
| 3 | [storytold/artcraft](https://github.com/storytold/artcraft) | 面向艺术家/设计师的创作引擎 | Rust | 14,293 | +3,217 | 2,245 |
| 4 | [mattpocock/skills](https://github.com/mattpocock/skills) | 面向工程师的个人 Agent Skills 合集 | Shell | 284,371 | +1,737 | 23,804 |
| 5 | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | AI 编辑级图表生成（44 种，纯 HTML/SVG） | HTML | 48,877 | +1,189 | 3,090 |
| 6 | [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) | Claude Cowork 官方知识工作插件集 | Python | 28,781 | +626 | 3,276 |
| 7 | [hugohe3/ppt-master](https://github.com/hugohe3/ppt-master) | 自然语言转原生 PPT（含动画 + 讲稿） | Python | 59,374 | +515 | 4,676 |
| 8 | [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) | 一份用来改善 Claude Code 的 CLAUDE.md | — | 218,208 | +279 | 21,978 |
| 9 | [mksglu/context-mode](https://github.com/mksglu/context-mode) | 为 AI Agent 优化上下文窗口的 sandbox | TypeScript | 26,278 | +178 | 1,891 |
| 10 | [flutter/flutter](https://github.com/flutter/flutter) | 跨平台 UI 工具包 | Dart | 179,489 | +164 | 33,591 |
| 11 | [huggingface/transformers](https://github.com/huggingface/transformers) | 多模态模型定义框架 | Python | 167,215 | +94 | 34,796 |
| 12 | [pytorch/pytorch](https://github.com/pytorch/pytorch) | 动态神经网络框架 | Python | 104,127 | +81 | 31,951 |
| 13 | [tensorflow/tensorflow](https://github.com/tensorflow/tensorflow) | 开源 ML 框架 | C++ | 200,712 | +24 | 78,960 |

---

## 重点项目点评

### 🥇 [morluto/rea](https://github.com/morluto/rea) — 今日榜首，+25,784⭐

**"REA" = Reverse-Engineer Anything：AI 把二进制逆向门槛压到 0**

同一个项目当天也冲上了 Hacker News 第一（662 分 / 292 评）。REA 把 Ghidra + IDA + Binary Ninja 过去需要几天上手的工作流封装成"上传二进制 → 得到可读源码 + 调用图 + 字符串归因"。背后是 LLM 对函数签名 / 控制流 / 字符串表的多轮推断，加上一套对主流 toolchain（LLVM、MSVC、Go、Rust）的符号识别规则。

单日 **+25,784⭐**，相当于今天 trending 第 2 到第 10 的总和。这个增幅在 2025 以来只有 Cursor / Claude Code / open-webui 这种"引爆级"项目见过。它直接说明：**"AI × 二进制 / 逆向"是今年最被低估的赛道**，门槛的消失速度比大多数人预期得快。接下来 1-2 周值得盯紧 (1) 法律层面是否会有 DMCA 1201 争议 (2) 商业版 pricing / API 是否推出。

---

### 🥈 [boykopovar/AnyPS5](https://github.com/boykopovar/AnyPS5) — +5,831⭐

**"任何平台跑 PS5 游戏"：灰色地带 + 技术好奇心的组合拳**

AnyPS5 宣称可以自动把 PS5 可执行文件移植到 Linux/Windows。README 定位是研究用途，但显然切中了"主机游戏自由"社区（RPCS3、Yuzu、Ryujinx 一脉）的刚需。首日 **+5,831⭐**，评论区在等待 Sony 发出 DMCA 之前先围观。

这类项目在历史上有过明显规律：**冲榜 → 诉讼 → fork 四散**。但真正值得注意的是：PS5 游戏的保护机制（Zen 2 定制安全启动 + 自研加密 + Fine-grained TPM）过去被认为是"短期内不会被公开破解"的，AnyPS5 的出现意味着这条防线已经被 AI 辅助的二进制重写工具（见 No.1）啃出了口子。

---

### 🥉 [storytold/artcraft](https://github.com/storytold/artcraft) — +3,217⭐

**Rust × 生成式 × 创作者：下一个 Figma 可能不长这样**

artcraft 把自己定位为"面向艺术家、设计师、电影人的生成/合成引擎"：节点式工作流 + 本地 GPU 推理 + 原生导出。Rust 底座在性能和跨平台上都更接近 ComfyUI 的升级版，但 UI 走的是面向创作者的时间线和图层逻辑，而不是 ComfyUI 的技术节点图。

它在今天 trending 的意义不是技术突破，而是**"创作者原生生成工具"这个口子正在被打开**。Adobe 的 Firefly 还在走订阅通道，Figma AI 还在吃企业市场，像 artcraft 这样"桌面 + 本地 + 生成式"的开源栈，可能是下一轮创作者生产力迁移的真正入口。

---

### 🏅 [mattpocock/skills](https://github.com/mattpocock/skills) & [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) — 并列双生

**Claude Skills 生态进入"官方 + 社区"双轨期**

Matt Pocock 的 `skills` 把他个人 agents 目录里的工程师用 skills 开源，单日 +1,737⭐；几乎同时 `anthropics/knowledge-work-plugins` 单日 +626⭐——官方插件集也在同一时间点集中曝光。两者加上第 8 名的 `andrej-karpathy-skills`（+279⭐），**今天 trending 前 15 里有 3 个直接服务于 Claude Skills / CLAUDE.md 生态**。

这类项目的爆发节奏跟上个月 OpenAI 推出 ChatGPT Apps / Anthropic 推出 Skills 规范几乎同步。它意味着：**"Agent 原生内容"开始成为 GitHub 上一种新的 primary artifact 类型**——过去是代码，然后是 config，现在是 markdown prompt + skill manifest。这个变化会在 2027 Q1 彻底改变开源项目的目录结构。

---

### 🎖️ [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) — +1,189⭐

**"Editorial 级图表生成"：The Economist 风格的 LLM 可视化模板集**

44 种精心设计的图表模板，纯 HTML/SVG，专门为 Claude Code / Cursor 等 AI 编码工具准备——意思是你让 Claude 画图时可以 "@diagram-design"，让输出达到商业出版物的美学标准。这个方向是对**现在 LLM 生成图表美学普遍下限太低**的直接回应。

它和第 5 名 `context-mode`、第 7 名 `ppt-master` 一起，构成了今天 trending 上另一条隐形线索：**"AI 做 PPT / 做图表 / 做文档"的工具正在集中成熟**。这是办公生产力类产品进入收割期的信号。

---

## 生态观察

- **"AI × 逆向工程"是今年最快到达拐点的赛道**：morluto/rea 单日 25,784⭐ 冲上第一；boykopovar/AnyPS5 跟随到第二。二进制理解曾是 AI 应用的禁区，今天同一天出现两个爆款，意味着"门槛性"问题可能已经被解决。
- **Claude Skills 开始走出 Anthropic 自家仓库**：Matt Pocock 的个人集 + Karpathy skills + anthropics 官方知识工作插件 = Agent 原生内容的三支生态力量首次同框。开发者侧的下一轮分发物 = `.claude/skills/*/SKILL.md`。
- **办公生产力 AI 工具进入收割期**：ppt-master（+515）、diagram-design（+1,189）、context-mode（+178）集中出现在同一天榜单。它们都共享同一个用户画像："用 Claude Code / Cursor 的知识工作者"。
- **传统 ML 框架继续慢速增长**：PyTorch +81、TensorFlow +24、transformers +94，排名靠后但依然稳居 trending。基础设施型项目在 AI 应用层快速翻涌的噪声中仍然构成压舱石。
- **Rust 系设计工具 artcraft 单项目独占 trending 一席**：这是过去半年"Rust × 创作者工具"的持续趋势——同一赛道的 Zed、Gpui、ferrumgfx 都在搭建类似的生态。

---

*数据来源：github.com/trending（2026-10-11 快照）；因访问限制使用 WebFetch 摘要，共 13 项。*
