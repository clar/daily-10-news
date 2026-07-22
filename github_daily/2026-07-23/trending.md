# GitHub Trending 日报 · 2026-07-23

## 今日焦点

> **OSINT + AI 情报仪表盘登顶 · Claude Skill 生态爆发 · 免费 AI 网关抢眼 · WiFi 感知 Rust 项目 · 老代码考古回潮**
>
> - `koala73/worldmonitor` 单日 +4,131⭐，AI 情报仪表盘登顶，Palantir 平民化叙事再度升温
> - `ayghri/i-have-adhd` 单日 +1,682⭐，Claude Skill 首个"命令式简洁输出"技能爆红
> - `diegosouzapw/OmniRoute` 单日 +1,648⭐，本地 AI 网关聚合 278 家 provider + 90 家免费额度
> - `oblien/openship` 单日 +1,304⭐，自托管部署平台承接"逃离 Vercel"情绪
> - `ruvnet/RuView` 单日 +875⭐，Rust 写的 WiFi 空间感知库进入主流视野

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [koala73/worldmonitor](https://github.com/koala73/worldmonitor) | 实时全球情报仪表盘 + AI 新闻聚合 | TypeScript | 68,797 | +4,131 | 10,518 |
| 2 | [ruvnet/RuView](https://github.com/ruvnet/RuView) | 用 WiFi 信号做空间感知 / 生命体征 | Rust | 83,704 | +875 | 11,229 |
| 3 | [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) | Claude Skill：让 AI 输出更简洁直接 | Python | 8,195 | +1,682 | 375 |
| 4 | [schollz/croc](https://github.com/schollz/croc) | 端到端加密的文件传输命令行 | Go | 37,530 | +737 | 1,482 |
| 5 | [likec4/likec4](https://github.com/likec4/likec4) | 软件架构可视化 + 实时协作 | TypeScript | 4,251 | +172 | 302 |
| 6 | [chrislgarry/Apollo-11](https://github.com/chrislgarry/Apollo-11) | Apollo 11 制导计算机源代码 | Assembly | 70,570 | +766 | 7,880 |
| 7 | [jamiepine/voicebox](https://github.com/jamiepine/voicebox) | 开源 AI 语音克隆 & 听写工作台 | TypeScript | 45,714 | +565 | 5,582 |
| 8 | [diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute) | AI 网关：278 家 provider + 自动 fallback | TypeScript | 25,148 | +1,648 | 3,343 |
| 9 | [shiyu-coder/Kronos](https://github.com/shiyu-coder/Kronos) | 金融市场"语言"基础模型 | Python | 32,576 | +134 | 5,597 |
| 10 | [ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) | Claude Skill 精选合集 | Python | 68,734 | +155 | 7,803 |
| 11 | [oblien/openship](https://github.com/oblien/openship) | 自托管部署平台（Vercel 替代） | TypeScript | 7,240 | +1,304 | 534 |
| 12 | [agegr/pi-web](https://github.com/agegr/pi-web) | pi coding agent 的 Web UI | TypeScript | 2,055 | +314 | 309 |
| 13 | [rohitg00/ai-engineering-from-scratch](https://github.com/rohitg00/ai-engineering-from-scratch) | 从零学 AI 工程实战 | Python | 42,208 | +688 | 7,028 |
| 14 | [tirth8205/code-review-graph](https://github.com/tirth8205/code-review-graph) | 本地代码智能图，压缩 AI 上下文 | Python | 25,275 | +872 | 2,388 |
| 15 | [dreamhunter2333/cloudflare_temp_email](https://github.com/dreamhunter2333/cloudflare_temp_email) | Cloudflare 免费临时邮箱 | TypeScript | 10,787 | +60 | 7,287 |

---

## 重点项目点评

### 🥇 [koala73/worldmonitor](https://github.com/koala73/worldmonitor) — 今日榜首，+4,131⭐

**"人人可用的 Palantir"叙事再度点燃 GitHub**

worldmonitor 是一个把 500+ 新闻源 + 卫星/军情/金融/气象/航空/基础设施数据聚合到 3D 地球 + WebGL 平面地图上的实时情报仪表盘。技术栈相当"2026 风格"：TypeScript 前端 + Tauri 2 桌面壳 + Rust sidecar + Protocol Buffers（281 protos / 35 services）+ Ollama / Groq / OpenRouter 可插拔 LLM。它同时暴露 MCP server / REST / CLI / Python·Ruby·Go SDK，可以像一台"open-source Palantir"一样接给 agent 使用。

单日 +4,131⭐ 的爆发力，来源于三条正在合流的叙事：**OSINT 平民化、AI agent 需要"结构化世界模型"作为长期记忆、Country Instability Index 这类"可量化地缘政治指标"越来越被交易员和政策研究者需要**。项目提供 6 套子站（world / tech / finance / commodity / happy / energy），把同一套后端切成不同产品面向不同人群——这套"多面孔单一底座"设计已经开始成为 2026 年内容型开源项目的默认打法。

**最值得留意的一点：它是"local-first + BYOK"的**——完全可以用 Ollama 本地跑，不需要任何 API key，这正是 GitHub 用户在过去半年里越来越明确的偏好，也是它能一天吸 4k+ 星的最大结构性红利。

---

### 🥈 [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) — +1,682⭐

**Claude Skill 生态首个"输出风格"神技能**

`i-have-adhd` 是一个 Claude Code Skill，功能极小：**强制 AI 用最直接的、动词开头的、可编号的、去除寒暄的格式回答问题**。安装后用 `/i-have-adhd` 调用。就是这么"小"的一个东西，一天冲到 +1,682⭐，超越大量重型项目。

这是 2026 年 Claude Skill 生态一次里程碑式验证：**Skill 的价值不必是"新能力"，可以是"输出风格 / 交互约束"**。它揭示了一个正在成熟的品类——AI 使用者对"太啰嗦、埋结论、格式糟糕"的反感已经积累到一定阈值，愿意为一个 15 行的 skill 付出真金白银的关注度。可以预见，接下来会有：
- `no-emoji`（禁 emoji）
- `citations-first`（先出引用后出结论）
- `no-hedging`（去除"我认为可能"）
- `japanese-tea-ceremony`（超级礼仪派）

等一整套"输出风格 Skill 家族"出现，Composio 的 [awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) 一天涨 155⭐ 也是同一趋势的佐证。

---

### 🥉 [diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute) — +1,648⭐

**AI 网关战场进入"免费额度聚合器"新阶段**

OmniRoute 是一个跑在本地的 AI 网关：把你机器上的任意 coding tool（Claude Code / Cursor / Cline / Zed）指向 `localhost:xxxx`，就能路由到 **278 家 provider、90+ 家免费额度**。核心卖点有三：
1. **自动 fallback**：某家限流就换下一家；
2. **Token 压缩**：RTK + Caveman 双引擎，压缩 15-95%，直接省 API 费；
3. **配额共享**：一份订阅按公平策略切给团队；
4. 兼容 OpenAI / MCP / A2A 三种协议。

它一天吸 +1,648⭐，因为在 2026 年**"AI 网关 / router"品类的竞争，已经从 OpenRouter、Portkey 这类中心化托管，下沉到"本地跑 + 聚合免费额度"的新范式**。1.53B 免费 token / 月 的宣传口径直接击中"贫穷开发者"和"独立黑客"两大群体。对企业而言，OmniRoute 也提供了一条"合规友好 + 成本可控"的过渡路径。

**次生现象：** 这个赛道会继续洗牌，OpenRouter 的护城河从"我知道所有 provider"退到"我提供稳定 SLA 和结算"，未来 12 个月开源本地网关会继续吃份额。

---

### 🚢 [oblien/openship](https://github.com/oblien/openship) — +1,304⭐

**"逃离 Vercel"情绪找到一个可落地的自托管答案**

openship 是自托管的部署平台，替代 Vercel/Netlify/Render 那一层。一天涨 +1,300⭐，背后是 2026 年上半年愈演愈烈的"托管 PaaS 涨价 + Bandwidth 政策收紧"引发的迁移潮——尤其在 Vercel 对 AI Gateway 增加定价、Netlify 对函数冷启动限时之后，独立开发者与中小型团队开始集体搜索**"能自己跑一台 Docker 主机就能替代整个 PaaS 服务"** 的方案。

openship 抓住的正是这个窗口。它的技术栈以 TypeScript 为主，跑在 Docker/Compose 上；对 GitHub webhook / preview branch / edge caching 有原生支持。虽然功能比 Vercel 少一大截，但**"我能读源码 + 我能审计成本 + 我能一键 self-host"** 已经足够撑起首轮增长。

预计接下来 3 个月 openship 会分化出两个方向：一部分用户会推动它接 Cloudflare Tunnel + K3s 做集群化；另一部分会推动它变成"专给 AI agent 部署"的目标平台。

---

### 📡 [ruvnet/RuView](https://github.com/ruvnet/RuView) — +875⭐

**用 WiFi 信号做空间感知，进入 mainstream 视野**

RuView 用 Rust 实现基于 WiFi CSI（Channel State Information）的空间感知：可以做**在室人数检测、呼吸/心跳等生命体征估计、跌倒检测**——无需任何摄像头，只用商品级 WiFi 路由器的信号扰动。

这是学术圈已经研究十几年的领域（早期 MIT / CMU 都有原型），但一直卡在"驱动开源程度低 + 硬件门槛高 + 部署复杂"。RuView 通过 Rust 生态（性能好、跨平台好），加上一套开箱即用的示例，让 Home Assistant、看护、办公室占用监测等应用第一次可以在业余时间搭起来。总星数已经 83k+，说明这个领域在 GitHub 上的关注度早已积累到质变临界。

**次生思考：** WiFi 感知的隐私争议将随着易用性提升而爆发——路由器可以隐性感知住户呼吸速率，会成为 2027 年可预见的政策议题。

---

## 生态观察

今天 trending 表面上五花八门，实际上聚焦三条主线：

1. **"AI 时代的私有基础设施"** —— worldmonitor（情报）、OmniRoute（网关）、openship（部署）、code-review-graph（上下文）、cloudflare_temp_email（隐私邮箱）、RuView（感知）——所有 +500⭐ 以上的项目几乎都在做同一件事：**把过去 SaaS 提供的能力搬回本地/自托管**。这是 2026 年 GitHub 上最强的结构性叙事。

2. **Claude Skill 品类进入"品味竞争"阶段** —— i-have-adhd 上榜说明用户已经愿意为"输出风格"付关注度；awesome-claude-skills 常驻热榜说明生态目录仍在快速吸粉。下一阶段的竞争焦点将从"我能做什么"转向"我以什么风格做"。

3. **老派项目回热与新派项目共存** —— Apollo-11、schollz/croc、chrislgarry/Apollo-11 这类"考古 / 稳定实用"项目仍能挤进前 10，说明 GitHub 主页依然为"技术传承 + 工匠气质"保留了推荐权重；这与追新 AI 项目并不冲突，反而形成一种"新旧共振"的社区口味。

值得注意的次弹幕：`agegr/pi-web` (pi coding agent Web UI) 一天涨 +314⭐，说明"给某个新 agent 写 UI"仍是一种低门槛高回报的 GitHub 姿势；`tirth8205/code-review-graph` 涨 +872⭐，指向"减少 AI 上下文 token"是 2026 下半年最热的中间层机会。

**一句话总结：** 2026-07-23 的 GitHub trending，是 "self-hosted 复兴 + Claude Skill 品味战 + AI 网关本地化" 三股力量同时发力的产物；如果只挑一个信号带走，就是 **"AI 让开发者变强了，而变强的开发者正在系统性地把 SaaS 拆回来自己跑"**。
