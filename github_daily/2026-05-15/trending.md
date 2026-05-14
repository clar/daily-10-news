# GitHub Trending 日报 · 2026-05-15

## 今日焦点

> **Agent Skills 框架井喷 · 个人 AI 操作系统抬头 · 端侧多模态加速 · 金融大模型 · 反检测浏览器**
>
> - `obra/superpowers` 单日 +1,801⭐ 累计 19 万星，agentic skills 框架与开发方法学的事实标准化
> - `mattpocock/skills` +2,971⭐ "工程师专属技能集"二度冲榜，与 superpowers 形成 skills 生态双雄
> - `tinyhumansai/openhuman` +3,476⭐ 今日涨幅冠军，"个人超级智能"概念引爆 Rust 社区
> - `rohitg00/agentmemory` +1,978⭐ AI 编码 agent 持久化记忆，针对 Claude/Cursor 真实基准优化
> - `supertone-inc/supertonic` +1,163⭐ ONNX 端侧 TTS，多语言、低延迟，Swift 实现冲入前 10

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [ruvnet/RuView](https://github.com/ruvnet/RuView) | 把商用 WiFi 信号转化为空间感知 / 生命体征监测 | Rust | 55,669 | +1,757 | 7,379 |
| 2 | [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) | 个人 AI 超级智能，私有、简洁、强大 | Rust | 7,626 | +3,476 | 610 |
| 3 | [rohitg00/agentmemory](https://github.com/rohitg00/agentmemory) | AI 编码 agent 的持久化记忆方案 | TypeScript | 8,884 | +1,978 | 734 |
| 4 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic skills 框架与软件开发方法学 | Shell | 191,058 | +1,801 | 16,989 |
| 5 | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) | 科研 / 工程 / 金融 / 写作的开箱即用 Agent Skills | Python | 21,715 | +637 | 2,373 |
| 6 | [shiyu-coder/Kronos](https://github.com/shiyu-coder/Kronos) | 金融市场"语言"基础模型 | Python | 24,754 | +359 | 4,333 |
| 7 | [roboflow/supervision](https://github.com/roboflow/supervision) | 复用型计算机视觉工具集 | Python | 38,840 | +59 | 3,478 |
| 8 | [influxdata/telegraf](https://github.com/influxdata/telegraf) | 全能指标 / 日志采集 Agent | Go | 17,193 | +211 | 5,790 |
| 9 | [supertone-inc/supertonic](https://github.com/supertone-inc/supertonic) | ONNX 端侧多语种闪电 TTS | Swift | 5,244 | +1,163 | 508 |
| 10 | [Genymobile/scrcpy](https://github.com/Genymobile/scrcpy) | 跨平台 Android 设备控制工具 | C | 141,263 | +778 | 13,047 |
| 11 | [NVIDIA-AI-Blueprints/video-search-and-summarization](https://github.com/NVIDIA-AI-Blueprints/video-search-and-summarization) | GPU 加速视觉 agent / 视频分析参考架构 | Python | 791 | +28 | 241 |
| 12 | [CloakHQ/CloakBrowser](https://github.com/CloakHQ/CloakBrowser) | 通过所有机器人检测的隐身 Chromium | Python | 10,715 | +1,369 | 803 |
| 13 | [mattpocock/skills](https://github.com/mattpocock/skills) | 工程师专用 Skills 集合 | Shell | 81,953 | +2,971 | 7,067 |
| 14 | [github/spec-kit](https://github.com/github/spec-kit) | Spec-Driven Development 工具箱 | Python | 99,351 | +1,240 | 8,649 |
| 15 | [garrytan/gstack](https://github.com/garrytan/gstack) | 多角色工程师的 23 件套配置 | TypeScript | 96,618 | +960 | 14,366 |

---

## 重点项目点评

### 🥇 [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) — 今日涨幅冠军，+3,476⭐

**"个人 AI 超级智能"叙事再次点燃 Rust 圈**

openhuman 主打"私有、简洁、强大"三词，定位是给个体用户用的 personal AI superintelligence——本质上是把模型推理、知识库、长期记忆、工具调用打包成一个可以本地跑、对自己数据有完全控制权的 OS 级产品。它和过去半年很火的"个人 AI 操作系统"赛道高度重合，但用 Rust 写底座这一点让它在开发者社区拿到了额外好感：一是性能可期，二是分发简单（单二进制），三是与 Tauri/Wasm 等前端 / 插件生态衔接顺滑。

值得注意的是仓库才不到 8k 星但单日就拿了 3.4k，说明它今天大概率上了 Hacker News / X 的话题首页。如果你在做 agent + memory + tool use 的端侧方案，建议把它的进程模型和插件机制扫一遍，至少能省一周架构调研。

---

### 🥈 [mattpocock/skills](https://github.com/mattpocock/skills) — +2,971⭐

**Skills 已成事实标准，社区开始按"角色"打包**

Matt Pocock 把自己日常工作沉淀下来的脚本、prompt、工程实践全部封装成 Claude Code / Cursor 可以直接装载的 skills，配套有快速安装脚本。和官方 superpowers 框架不同，mattpocock/skills 是"经过实战的内容包"，二者关系类似于 npm 与某个工程师的 dotfiles。

它的快速冲榜印证了一个趋势：**skills 正在替代过去那种"几百行 system prompt + 一堆 MCP server"的私房菜做法**，转向"按角色、按场景打包、按需挂载"的模块化范式。如果团队还在用 monolithic prompt，应该尽快把流程迁过来。

---

### 🥉 [obra/superpowers](https://github.com/obra/superpowers) — +1,801⭐，累计 19 万星

**Agentic 开发的"方法学"层正在收敛**

superpowers 同时是一个框架和一套方法学——它定义了 skill 的结构、执行顺序、上下文裁剪策略，并把"软件开发"本身视作可被 agent 编排的工作流。能在 19 万星基础上单日再涨近 1,800，说明它从工具走向了"约定"：当人们提到"做一个 agentic 工程链"，越来越多团队默认是基于 superpowers 风格来组织 skill 目录。

它的下一站很可能是被 Claude Code、Cursor、Cline 等终端正式收编为推荐范式。配合 mattpocock/skills 这类内容生态，2026 年 H1 的 agentic IDE 大概率会以"框架 + skill 包市场"的双层结构稳定下来。

---

### [rohitg00/agentmemory](https://github.com/rohitg00/agentmemory) — +1,978⭐

**编码 agent 真正的护城河在"长期记忆"**

agentmemory 主打一件事：给 Claude Code / Cursor / Codex 一类的编码 agent 提供跨会话、跨仓库的持久化记忆，并且号称基准是基于"真实工程场景"（而非合成评测）做出来的。它解决的是当下 agent 最痛的两点——一是切换分支 / 切换仓库后上下文丢失，二是对项目特定约定（命名、目录、CI、私有库）无法稳定记住。

随着各家 agent 工具自己都在做 memory（Cursor 的项目记忆、Claude 的 memory tool），第三方 memory 中间件还有没有空间？短期答案是有：它跑在工具之上、和工具同步，是少数能跨厂商工作的"agent CRM"。

---

### [supertone-inc/supertonic](https://github.com/supertone-inc/supertonic) — +1,163⭐

**端侧多模态：TTS 终于跑进毫秒级**

Supertonic 是把已有的多语种 TTS 模型用 ONNX 跑在端侧（macOS / iOS / Windows / Linux），主打"原生 Swift + 闪电延迟"。在前几天 Apple 把 Foundation Models 框架对开发者放开之后，端侧 TTS / ASR / 翻译这条线明显在加速。

对于做 voice agent、可访问性、车机 / 嵌入式语音产品的团队来说，端侧多语种 TTS 一直缺一个"质量够用、license 友好、能直接 ONNX 化"的方案，Supertonic 刚好把这块缺口补上。预计下半年会看到更多团队把云端 TTS 调用替换成本地 ONNX。

---

## 生态观察

今天的榜单几乎被 **agentic skills 与个人 AI 基础设施**两个主题占满：`superpowers` + `mattpocock/skills` + `K-Dense-AI/scientific-agent-skills` 三个 skills 仓同框上榜，意味着 skill 作为一种打包格式已经从 Claude Code 的私有生态走出，开始具备跨 IDE / 跨厂商的通用性；`openhuman` + `agentmemory` + `CloakBrowser` 则代表"个人化、私有化、绕开平台限制"的另一面——用户开始希望 AI 工具不仅强，还要"是我的"。

**降温信号**：传统 ML 库（`supervision`、`telegraf`）今日涨幅都进入两位数甚至个位数，说明纯工具型项目的注意力正在被 agent 类项目挤占。

**新方向**：金融基础模型 `Kronos` 与视频 agent `NVIDIA-AI-Blueprints/video-search-and-summarization` 进入榜单，反映"垂直领域基础模型 + 多模态 agent"这两条暗线在持续累积关注度，是接下来值得跟踪的 niche。
