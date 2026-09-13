# GitHub Trending · 2026-09-14

## 今日焦点

> **AI Agent 工具链 · 攻防安全生态 · 消费级前沿模型 · 本地 MoE 推理 · 开源多模态创作**
>
> - `bilawalsidhu/gods-eye-view` +2,898⭐ 登顶，浏览器里的"上帝之眼"卫星模拟——数据是真实的。
> - `debpalash/VoiceStudio` +2,546⭐ 开源版 ElevenLabs，语音克隆/配音本地化冲击商业订阅。
> - `JustVugg/colibri` +960⭐ 用纯 C 在个人硬件上跑前沿 MoE，零依赖是它的杀手锏。
> - `asgeirtj/system_prompts_leaks` +727⭐ 全球主流 AI 平台 system prompt 泄漏合集，一夜狂涨。
> - `vxcontrol/pentagi` +613⭐ 自主 AI 渗透测试代理，攻防生态 agent 化再进一步。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [bilawalsidhu/gods-eye-view](https://github.com/bilawalsidhu/gods-eye-view) | 浏览器里的真实数据卫星模拟器 | JavaScript | 31,770 | +2,898 | 6,378 |
| 2 | [debpalash/VoiceStudio](https://github.com/debpalash/VoiceStudio) | 开源 ElevenLabs 替代，语音克隆/配音 | Python | 26,613 | +2,546 | 3,282 |
| 3 | [JustVugg/colibri](https://github.com/JustVugg/colibri) | 纯 C 本地跑前沿 MoE，零依赖 | C | 29,693 | +960 | 3,233 |
| 4 | [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) | 主流 AI 平台系统提示词泄漏合集 | JavaScript | 65,985 | +727 | 10,797 |
| 5 | [vxcontrol/pentagi](https://github.com/vxcontrol/pentagi) | 自主 AI 渗透测试 agent 系统 | Go | 23,928 | +613 | 3,093 |
| 6 | [SnailSploit/Claude-Red](https://github.com/SnailSploit/Claude-Red) | Claude Skills 攻防安全能力库 | Python | 4,093 | +507 | 590 |
| 7 | [multimodal-art-projection/YuE](https://github.com/multimodal-art-projection/YuE) | YuE2：符号规划驱动的前沿音乐生成 | Python | 7,707 | +500 | 862 |
| 8 | [melgarafael/DeskcommCRM](https://github.com/melgarafael/DeskcommCRM) | 自托管 AI 销售 OS，原生 agent | TypeScript | 2,155 | +444 | 587 |
| 9 | [alibaba/open-code-review](https://github.com/alibaba/open-code-review) | 确定性流水线 + LLM 混合代码评审 | Go | 23,417 | +438 | 1,731 |
| 10 | [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) | 首个开源 agentic 视频制作系统 | Python | 58,382 | +383 | 7,348 |
| 11 | [alphaXiv/OpenResearch](https://github.com/alphaXiv/OpenResearch) | 并行研究 agent，任何模型可插入 | Rust | 2,016 | +304 | 144 |
| 12 | [jihe520/MathModelAgent](https://github.com/jihe520/MathModelAgent) | 自动完成数学建模任务的 agent | Python | 5,331 | +268 | 407 |
| 13 | [yuliskov/SmartTube](https://github.com/yuliskov/SmartTube) | Android TV 自定义规则播放器 | Java | 33,426 | +238 | 2,031 |
| 14 | [tech-leads-club/agent-skills](https://github.com/tech-leads-club/agent-skills) | 面向专业代码 agent 的安全技能注册中心 | TypeScript | 5,609 | +215 | 499 |
| 15 | [ever-co/ever-gauzy](https://github.com/ever-co/ever-gauzy) | 开源业务管理平台 ERP/CRM/HRM | TypeScript | 4,996 | +58 | 937 |

---

## 重点项目点评

### 🥇 [bilawalsidhu/gods-eye-view](https://github.com/bilawalsidhu/gods-eye-view) — 今日榜首，+2,898⭐

**浏览器里的"上帝之眼"，数据是真实的**

这是一个开源的 web 端卫星情报（satellite intelligence）模拟器，把 Sentinel-2、Landsat、Planet、Airbus 等公开卫星影像与商用高分数据源打包成"轨道视角"的可视化系统。用户可以在浏览器直接拖拽时间轴查看某个点的历史 imagery，或者拉一条 AOI 观察多光谱变化——本质上是把 OSINT 分析师的桌面工作流搬到了浏览器。

它今日爆冲近 3,000 颗星，原因不是纯技术——而是**"卫星情报大众化"这个话题本身**。过去两周乌俄战场、加沙人道走廊、南海船只轨迹都在 X/Twitter 上以 OSINT 帖形式高频传播，专业工具（Sentinel Hub、Skywatch）门槛太高，普通网友想复刻分析没有入口。这个仓库正好卡在这个需求的正中央——**"你也可以做卫星记者"**。

技术上值得注意的是 Cesium + WebGPU 的组合以及 tile 侧的流式请求策略，README 里明确讲了如何接入自己的 API key。可以预见接下来一周会有大量 fork 用于报道向应用。

---

### 🥈 [debpalash/VoiceStudio](https://github.com/debpalash/VoiceStudio) — +2,546⭐

**开源 ElevenLabs 冲击商业订阅"最后一里"**

VoiceStudio 是一个自托管的 TTS / 语音克隆 / 多语配音项目，目标非常直接——**替代 ElevenLabs**。它支持 zero-shot voice cloning、多语言配音、自动对齐口型、批量处理长音频，一整套 pipeline 可以在单张消费级 GPU 上跑。README 明确对标 ElevenLabs 的 pricing——月费 5-330 美元的档位，被"一个 Python 命令跑起来"的开源方案挑战。

它的爆发跟上周多个"ElevenLabs 涨价"、"API 限额收紧"的讨论直接相关。同时，本周 YouTube、TikTok 创作者社群开始批量试用开源 TTS 做多语版本——这个仓库正好在需求峰值撞上供应。

值得留意的是模型权重的开源许可：VoiceStudio 使用了 XTTS-v3 / Fish-Audio 蒸馏路径，商业用途仍需检查条款。这一点也是 HN/Reddit 讨论最激烈的地方——**"开源"到底能不能商用**，是决定它能否真正吃下 ElevenLabs 长尾用户的关键。

---

### 🥉 [JustVugg/colibri](https://github.com/JustVugg/colibri) — +960⭐

**纯 C 本地跑前沿 MoE，零依赖是杀手锏**

colibri 是一个"纯 C、零依赖"的 MoE（Mixture of Experts）推理引擎，slogan 直接：**"Run frontier MoE models on hardware you already own"**。它把 llama.cpp 的思路推得更极致——不依赖 PyTorch、不依赖 CUDA runtime、甚至不需要 BLAS 库，代码全部是可移植 C，任何有点 SIMD 的机器都能跑。

它今天爆红的直接触发点，是本周 Mixtral 系列开源新版本 + DeepSeek-V4.1 Flash 上线（都是重度 MoE 架构）。开发者社区一直在等一个不用配环境就能跑 MoE 的最小引擎，colibri 卡准了这个空档。总星数已经 29,693，说明并非新项目，而是"事件驱动的二次爆发"——这在 llama.cpp 生态很常见。

对企业侧的意义在于：MoE 模型的 CPU / low-end GPU 推理效率一直是短板，colibri 的路径为"边缘 agent"提供了一条可能——把 8×7B MoE 塞进一台 24GB RAM 的 mini PC 做本地推理。

---

### 🎯 No.4 · [asgeirtj/system_prompts_leaks](https://github.com/asgeirtj/system_prompts_leaks) — +727⭐

**"AI 平台祛魅"的持续引擎**

这个仓库聚合了从 ChatGPT、Claude、Gemini、Perplexity、Cursor、Windsurf、v0、Devin、Manus 等平台反向拿到的 system prompt 全文。它是老项目（总星 66k），今天冲榜的原因是**新版 GPT-6 Astra 和 Claude Fable 5.1 的 system prompt 被首次收录**——一个持续更新且高价值的知识库。

它的存在有多重意义。对 prompt engineer 来说，是免费的 prompt design 教材；对开源 agent 项目来说，是可参考的行为规范设计；对研究者来说，则是揭示厂商行为策略的公开档案。评论区最有意思的观察是——**近半年来所有前沿平台的 system prompt 越写越长，从 500 tokens 涨到 5,000+ tokens**，安全规则、工具使用规范、身份护栏堆得像法律条款。

这个仓库的持续走高，本身是 AI 平台"透明度需求"的市场信号：越关心 AI 安全的开发者，越倾向于把厂商的护栏拆开看清楚。

---

### 🛡️ No.5 · [vxcontrol/pentagi](https://github.com/vxcontrol/pentagi) & [SnailSploit/Claude-Red](https://github.com/SnailSploit/Claude-Red)

**Agent 攻防生态化的双子星**

同一天两个"AI + 攻防"项目同时上榜，是非常明确的生态信号。

**pentagi** 是 Go 写的自主 AI 渗透测试 agent，可以接受一个 URL 或网段，自主完成侦察、漏扫、payload 生成、报告输出的完整流程。它已经积累到 23,928 星，是 AI-red-team 类目里最成熟的开源项目之一——今天再涨 613，很可能与本周 OpenAI GPT-6 Astra 触发 critical-cyber 安全阈值的报道相关。

**Claude-Red** 则走另一条路——它不是独立 agent，而是**为 Claude Skills 生态提供的攻防能力包**：SQL injection、目录穿越、SSRF、认证绕过等测试能力封装成 Skills，Claude Code / Claude Web 用户 install 即用。这是 Skills 生态的"下沉行业"标志——从写代码工具下沉到具体安全测试岗位。

这两个项目同天涌起 1,000+ 星，标志着 **AI 攻防的开源武器化正在完成**。这也是 EU AI Act 与加州 Frontier AI Safety Act 立法者眼下最担忧的一类"双用途"能力。

---

## 生态观察

今日 trending 有非常清晰的三条主线。

**第一条是 agent 工具链的行业下沉**：从做代码（agent-skills、open-code-review）到做销售（DeskcommCRM）、到做研究（OpenResearch、MathModelAgent）、到做安全（pentagi、Claude-Red）、再到做视频（OpenMontage）——agent 的"横向平台"故事讲完了，现在开始垂直行业分头出击。这是继"通用 agent 框架"（LangChain、AutoGPT、CrewAI）之后的第二波开源浪潮。

**第二条是消费级前沿模型的本地化**：colibri 让 MoE 上你手上的机器，VoiceStudio 挑战 ElevenLabs，YuE2 挑战 Suno/Udio——**开源社区对"云端订阅"的反击已经从技术圈溢出到内容创作圈**。语音、音乐、图像三个方向都在快速平价化。

**第三条是"卫星/传感器/OSINT"这条冷门线的意外爆发**：gods-eye-view 说明公开数据+浏览器可视化仍然是低成本高传播的组合。它不需要 AI 加持也能一天涨 3k 星，说明工具的"人人可用"仍然比"最先进"更能打。

安静的领域：纯基础设施（数据库、编译器、内核）今天几乎没有代表项目上榜；前端框架也罕见地缺席。这不是长期趋势，只是 AI 洪流暂时挤占了榜单。

---

_数据来源：github.com/trending · 2026-09-14 Asia/Shanghai_
