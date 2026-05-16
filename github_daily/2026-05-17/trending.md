# GitHub Trending 日报 · 2026-05-17

## 今日焦点

> **Agent Skills 框架战开打 · Claude Code 配套生态爆发 · Rust 在新 AI 工具占主导 · 本地 / 私有 AI 抬头 · WiFi 感知作为非视觉传感新方向**
>
> - `obra/superpowers` 一日 +1,281⭐，"agentic skills framework" 强势走红
> - `tinyhumansai/openhuman` 一日 +1,601⭐ 登顶日榜，主打"私有个人超级智能"
> - `K-Dense-AI/scientific-agent-skills` 一日 +669⭐，把"科研 Agent Skill"标准化
> - `colbymchenry/codegraph` Claude Code 配套：预索引代码知识图谱，省 token、零远程
> - `supertone-inc/supertonic` 端侧 ONNX TTS，多语种，主打 "Lightning-Fast"

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) | 私有个人超级智能 | Rust | 10,554 | +1,601 | 901 |
| 2 | [obra/superpowers](https://github.com/obra/superpowers) | Agentic skills 框架与开发方法论 | Shell | 193,858 | +1,281 | 17,246 |
| 3 | [ruvnet/RuView](https://github.com/ruvnet/RuView) | WiFi 空间感知 + 生命体征监测 | Rust | 58,230 | +990 | 7,606 |
| 4 | [supertone-inc/supertonic](https://github.com/supertone-inc/supertonic) | 端侧多语种 ONNX TTS | Swift | 6,736 | +745 | 690 |
| 5 | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) | 科研/工程/金融 Agent Skill 集 | Python | 23,049 | +669 | 2,481 |
| 6 | [oven-sh/bun](https://github.com/oven-sh/bun) | 极快的 JS 运行时 / 打包工具 | Rust | 91,105 | +414 | 4,540 |
| 7 | [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) | Claude Code 的本地代码知识图谱 | TypeScript | 2,404 | +397 | 203 |
| 8 | [Anil-matcha/Open-Generative-AI](https://github.com/Anil-matcha/Open-Generative-AI) | 200+ 模型自托管图像/视频生成 | JavaScript | 14,329 | +393 | 2,506 |

---

## 重点项目点评

### 🥇 [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) — 今日榜首，+1,601⭐

**"个人超级智能"——这是 2026 年 Rust 系最强叙事**

openhuman 把所有 LLM 推理、工具调用、向量数据库、Agent 编排压进一个 Rust 二进制，主打"私有 / 简单 / 极强"。它的真正卖点不在性能 benchmark，而在**叙事**：在 Anthropic 估值冲 9500 亿、OpenAI 接管用户银行账户的同一周，一个 GitHub 仓库公开说"你的大脑外延应该 100% 跑在你自己机器上"——这种立场正在变成一种新的开发者价值观。

技术上它走的是 llama.cpp + qdrant-rs + 自研 agent runtime 的组合，所有依赖都打包成单文件。它的真正威胁不是与 Claude Desktop 比能力，而是为"AI 主权"提供了一个可装配的参照实现——下个月会有 50 个 fork。

---

### 🥈 [obra/superpowers](https://github.com/obra/superpowers) — +1,281⭐

**"Skills" 作为新的工程范式：Claude Code 把 prompt 变成可分发的工件**

obra/superpowers 已经累积 19 万星，但今天又拿了 +1,281——原因是 Anthropic 在 5 月对 Claude Code "Skills" 机制做了重大升级，superpowers 直接成了"事实标准模板库"。它把开发流程（如何 review PR、如何写 changelog、如何做 root cause 分析）封装为可加载 skill，本质是**把 prompt engineering 从私房菜变成 npm 包**。

K-Dense-AI/scientific-agent-skills（榜单第 5）走的是同一逻辑，但定位科研垂直场景——两个一起上榜说明 "agent skills" 正在脱离 toy demo，进入"包管理器战争"阶段。下一步必然出现 skill registry 和企业市场。

---

### 🥉 [ruvnet/RuView](https://github.com/ruvnet/RuView) — +990⭐

**WiFi 信号成为继摄像头之后的非视觉感知通道**

RuView 利用 WiFi CSI（信道状态信息）做空间感知、姿态识别、呼吸/心跳监测，全程无摄像头、无穿戴设备。技术不算新（CMU 等学校 2010s 就有论文），但 ruvnet 把它做到能在 Raspberry Pi + 普通 ESP32 网卡上跑——**第一次让 "WiFi 当雷达"成了平民项目**。

为什么今天爆？因为它直接对接 AI 安防、智能家居、老人监护这条市场——既能避开摄像头的隐私伦理压力，又能给 LLM 提供新一类感知 token。Rust 实现让性能足够嵌入式，这是项目能走出学术圈的关键。

---

### 🏅 [supertone-inc/supertonic](https://github.com/supertone-inc/supertonic) — +745⭐

**端侧 TTS 的"质量天花板"被韩国团队又拉高一截**

Supertone（被 HYBE 收购的 AI 语音公司）开源了一个 ONNX 端侧 TTS 模型，主打多语种 + 极低延迟，单台 iPhone 上能跑实时合成。开源的不是完整商业模型，但权重 + Swift demo 完整可跑——这是 K-pop 工业级语音技术第一次开放出来。

时间点非常微妙：xAI 本月刚发标准化 Speech API，ElevenLabs 估值传言再涨——supertonic 用开源端侧把"语音 API"这个产业问句反过来了：**如果端侧免费且本地，云端语音订阅还卖给谁？**

---

### 🎖️ [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) — +397⭐

**Claude Code 配套工具开始成系列：本地代码图谱省 token**

codegraph 是 Claude Code 生态的明星项目之一：本地预索引整个代码库的符号、调用、依赖关系，让 Claude Code 通过结构化查询代替"扫一遍全仓库"——官方 demo 显示 token 用量降 60-80%。

这条赛道（Serena、codegraph、ast-grep + MCP 各种插件）刚成型一个月，已经在 trending 上反复出现。说明 Claude Code 用户群体已经大到能撑起自己的"工具市场"——和 VSCode 插件生态的早期一样，**最先做出来的 5-10 个工具会拿走最大份额**。

---

## 生态观察

- **"Agent Skills" 包管理器战争开启：** superpowers + scientific-agent-skills 两个 skills 仓库同时上榜，反映 Claude Code Skills 机制（以及 OpenAI 跟进的 "Custom GPT actions v2"）正在催生一个新的工件层——可分发、可组合、可付费。半年内会出现 "npm for skills"。
- **Rust 在 AI 工具层全面崛起：** 8 个仓库里 4 个 Rust（openhuman、RuView、bun 用 Zig 但生态接 Rust、+ supporting libs）。AI runtime 这一层已经事实上倒向 Rust——Python 守住训练，Rust 接管推理 / agent / 工具。
- **本地优先（local-first）反潮流：** openhuman、codegraph、supertonic 都强调"100% 本地"。在 OpenAI/Anthropic 把用户数据集中化的同一周，GitHub 用户用 ⭐ 表达了相反方向的偏好——这是一条贯穿 2026 的暗线。
- **科学 Agent 进入大众视野：** K-Dense-AI 的科研 Agent Skill 集是中国/华人团队的项目（K-Dense 来自加州/上海），25k 星，证明"AI for Science"叙事从 paper 走入 working code。
- **今日榜单变窄：** 仅 8 个 trending 条目（GitHub trending 偶发现象），但每个的今日增星量比一般日子大——说明流量在头部集中，长尾被冷落。这是 AI 工具发现的"超新星化"。
