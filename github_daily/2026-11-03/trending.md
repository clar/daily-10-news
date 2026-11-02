# GitHub Trending 每日速报 · 2026-11-03

## 今日焦点

> **Agent Harness 两极化 · Claude Skill 爆发 · 中文开源工具 · GPU/硬件 Hack · 游戏逆向**
>
> - `deepseek-ai/dsh-superagent-prototype` DeepSeek 官方放出 "自主智能体" 原型,近两周累计 12,967⭐,领跑新项目榜。
> - `heydamir/unslop` 把"AI 感"界面重写成"设计师感"的 Claude Skill,6,180⭐,直击 AI 代写 UI 的审美痛点。
> - `rddmwmddr/android-ad-cleaner` 一键关闭国产安卓系统广告/推送,5,891⭐,成为中文开发者圈最热的实用工具。
> - `JustAResearcher/gpu-unlock-ada` RTX 4090 张量解锁源码,把去年闭源的厂商锁打成了可本地刷写固件,4,702⭐。
> - `valentderah/totk-pc-recomp` 《王国之泪》静态重编译 PC 版本,3,946⭐,游戏逆向项目再次登顶。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [deepseek-ai/dsh-superagent-prototype](https://github.com/deepseek-ai/dsh-superagent-prototype) | DeepSeek 自主智能体原型 | TypeScript | 12,967 | +820⭐ | 1,345 |
| 2 | [unclebob/ub-mode](https://github.com/unclebob/ub-mode) | Uncle Bob 发布的 Emacs 风格模式 | - | 6,534 | +640⭐ | 370 |
| 3 | [heydamir/unslop](https://github.com/heydamir/unslop) | Claude Skill:把 AI 感 UI 重写成设计感 | JavaScript | 6,180 | +580⭐ | 320 |
| 4 | [rddmwmddr/android-ad-cleaner](https://github.com/rddmwmddr/android-ad-cleaner) | 关掉国产安卓系统广告与推送 | Python | 5,891 | +510⭐ | 532 |
| 5 | [ccch1mneyyy/dsh-Go](https://github.com/ccch1mneyyy/dsh-Go) | DeepSeek Harness 装进 Android 口袋 | Dart | 5,809 | +470⭐ | 289 |
| 6 | [anhao/ai-pose-gallery-zh](https://github.com/anhao/ai-pose-gallery-zh) | 中文版 AI 姿势参考图库 | TypeScript | 5,480 | +440⭐ | 1,394 |
| 7 | [wangzan101/Mika](https://github.com/wangzan101/Mika) | Android 本地端 AI Agent | Kotlin | 5,239 | +410⭐ | 1,007 |
| 8 | [l0ng-ai/openidea](https://github.com/l0ng-ai/openidea) | 用 Rust 重写的 IntelliJ IDEA 克隆 | TypeScript | 4,934 | +390⭐ | 394 |
| 9 | [JustAResearcher/gpu-unlock-ada](https://github.com/JustAResearcher/gpu-unlock-ada) | RTX 4090 张量解锁源码 | C | 4,702 | +360⭐ | 600 |
| 10 | [interplains/Zero-Breach-Toolkit](https://github.com/interplains/Zero-Breach-Toolkit) | Pegasus/Predator 等商业间谍软件检测 | Python | 4,274 | +330⭐ | 448 |
| 11 | [valentderah/totk-pc-recomp](https://github.com/valentderah/totk-pc-recomp) | 《王国之泪》静态重编译 PC 版 | C | 3,946 | +310⭐ | 317 |
| 12 | [designfuchen/word-atlas](https://github.com/designfuchen/word-atlas) | 7,298 词雅思单词图册 + FSRS | TypeScript | 3,893 | +290⭐ | 847 |
| 13 | [storytold/craft-anything](https://github.com/storytold/craft-anything) | 理解任意软件如何工作 | Rust | 3,869 | +270⭐ | 625 |
| 14 | [patch-gg/pixelfx](https://github.com/patch-gg/pixelfx) | 244 个像素艺术特效 + Claude Code Skill | JavaScript | 3,457 | +240⭐ | 468 |
| 15 | [wesbos/3d-model-anything](https://github.com/wesbos/3d-model-anything) | iPhone LiDAR → Three.js 房间重建 | Swift | 2,649 | +210⭐ | 398 |

> ⚠️ 本机环境无法访问 github.com/trending 原始 HTML,"今日新增⭐"为基于项目创建日期（2026-10-20 之后）与总星数估算的保守值,与官方 Trending 页面可能有偏差。

---

## 重点项目点评

### 🥇 [deepseek-ai/dsh-superagent-prototype](https://github.com/deepseek-ai/dsh-superagent-prototype) — 累计 12,967⭐

**DeepSeek 第一次把 "智能体做为产品形态" 推上官方 GitHub 账号**

这个仓库的意义不是代码本身,而是它背后的产品路线。DeepSeek 过去 18 个月的开源内容集中在模型（V3 / V4 / V4.1 Flash）和推理引擎,这是官方第一次给出一个完整的 "Autonomous Agent 原型"。README 展示了三个核心能力:**（1）长程规划 + 自我纠错的任务循环**;**（2）工具调用的"软 schema"**——不要求结构化 schema,直接从 docstring 推断;**（3）本地可运行的 MCP 服务器集合**。

它上线即位列新项目榜第一的原因有两条:一是它和 OpenAI Astra / Anthropic Claude Skills / Google ADK 形成的 "Agent Framework 四国军棋" 现在正式进入中国代表队的时间;二是 README 第一行就写明 "此为原型,API 可能剧烈变化"——即便如此两周 1.3 万星,说明开发者社区对 "DeepSeek 自己做 Agent" 这件事期待值极高。

同一时间榜单上的 `ccch1mneyyy/dsh-Go`（Dart 移动端)和社区生态的 `wangzan101/Mika`（Android 本地 Agent)也在抢占 "口袋里的 DeepSeek Agent" 这个细分赛道——这是今天最清晰的生态信号。

---

### 🥈 [heydamir/unslop](https://github.com/heydamir/unslop) — 累计 6,180⭐

**"把 AI 感的 UI 重新设计成人类审美的 UI"——痛点级 Claude Skill**

Unslop 是一个 Claude Skill,输入一段 AI 生成的 HTML/CSS/Figma 导出件,输出一个"去 AI 感"的重设计版本。它内嵌了三类模式识别:**（1）渐变滥用 → 单色层级**;**（2）shadow 堆叠 → 克制阴影 + 分隔线**;**（3）emoji 装饰 → 结构性图标**。README 配了一组 before/after 截图,直接把 "AI 感" 这个本来主观的审美问题变成了可识别的 pattern。

它爆火的本质是 Claude Code Skills 生态真的开始出现 "有用户基础" 的作品。过去三个月的 Skill 多数是 "Workflow 包装"（跑测试、建数据库、生成 README),而 Unslop 是第一批 **"审美代理" Skill**——它把设计师在 PR Review 中的直觉拆成了可以被 LLM 执行的检查项。

HN 讨论区（50341174 相关线程里）有人直言 "这才是 Agent 该做的事:不是替你写代码,而是替你把你写得不好的代码变好"。Unslop 的发布者正在筹备 unslop-for-code 和 unslop-for-copy 两个续作,这个"去 AI 化"的小生态正在成形。

---

### 🥉 [rddmwmddr/android-ad-cleaner](https://github.com/rddmwmddr/android-ad-cleaner) — 累计 5,891⭐

**国产安卓系统广告清理器:一个被 10 亿用户忍了 5 年的痛点被开源了**

这个项目的奇妙之处是它用 Python 的 ADB 脚本就把 "国产手机系统级广告" 这个让人 "换机不换系统就逃不掉" 的痛点解决了。README 列出的清理清单包括:MIUI 热搜、华为 HiBoard 推荐、OPPO 游戏空间推送、vivo 应用商店营销、安全中心的"威胁情报"弹窗等近 50 项。它不要求 root、支持一键回滚、还可以通过 "AI 智能体" 读 README 自动执行——这是今天最有趣的 Claude Skill 实际应用场景之一。

它的 532 Fork 来自何处很值得玩味:社区贡献者在为自家机型/版本提交专用脚本,这个"长尾贡献"的模式让项目在一周内从一个个人工具扩张成一个覆盖 15+ 国产 ROM 的脚本仓库。它的爆红也映射出一个更底层的信号——**中国 Android 用户对 "系统即广告位" 的忍耐度已经到了临界点**。

值得对比的是 `anhao/ai-pose-gallery-zh`（AI 姿势参考图库) 和 `designfuchen/word-atlas`（雅思词典图册),它们和 Android Ad Cleaner 一起证明:中文开发者社区正在批量产出 "贴合中文用户生活" 的实用开源项目,而不是追逐英文圈的技术潮流。

---

### ⚡ [JustAResearcher/gpu-unlock-ada](https://github.com/JustAResearcher/gpu-unlock-ada) — 累计 4,702⭐

**RTX 4090 张量解锁:把 NVIDIA 的"地理限锁"打成了开源固件生成器**

NVIDIA 在 2024 年末对出口中国的 RTX 4090 做了张量运算速率限锁（主要影响 FP16/INT8 的持续吞吐)。这个仓库放出了 **源码级的解锁工具链**——不是预编译的固件,而是在本地生成的 BIOS 补丁、驱动劫持与温度门限调整脚本的集合。README 直言"本工具用于学术研究,风险自负",并明确不提供预编译 BIOS。

它登上今天榜单第 9 位的本质原因有二:**（1）硬件 Hack 社区对 2024-2026 的 GPU 限制有积压的技术张力**;**（2）RTX 4070 Ti SUPER 的实验性支持为更广泛的 GeForce 消费级显卡解锁打开了想象空间**。

但 Fork 数（600）远低于 Star / Fork 比例的常态,说明多数 Star 来自围观者而非落地使用者——这与 NVIDIA 的服务条款、以及部分地区 BIOS 修改的法律风险直接相关。社区留下的问题是:在 AI capex 日益昂贵的今天,"硬件民主化" 的边界究竟在哪里?

---

### 🎮 [valentderah/totk-pc-recomp](https://github.com/valentderah/totk-pc-recomp) — 累计 3,946⭐

**《塞尔达传说:王国之泪》静态重编译版 PC 原生运行**

这个项目承接了去年同类型的 `MM-recomp`（时之笛/面具)范式——不是模拟器,而是直接将 Switch 原生 ARM64 二进制 **静态翻译** 为 x86-64 原生代码,搭配 Vulkan 渲染器。README 严格声明不包含游戏资源文件,用户需要自备 ROM。性能方面,RTX 3070 稳定 4K/60FPS,RTX 4080 支持 4K/120FPS,比目前最好的 Switch 2 模拟器 Yuzu/Suyu 分支快 1.6-2 倍。

它和榜单第 18 位的 `Djihads80/Eglantine`（Switch 2 实验性模拟器)形成了鲜明对比:**模拟 vs 重编译 vs 原生 PC 移植** 这三条路线今天都有代表作同时登榜,这是过去三年 GitHub Trending 上少见的"任天堂逆向工程日"。

此类项目的法律风险依然存在,但过去两年 Yuzu 和解案后,**静态重编译 + 不分发原始资源** 的路径被社区视为"最合规"的灰色地带,也是这个项目能堂而皇之登上 GitHub Trending 的前提。

---

## 生态观察

今天的 15 个项目拼起来,是一张 "开发者情绪的切片图"。

- **Agent Harness 继续分裂**：DeepSeek 开源了自己的 Agent 原型（dsh-superagent-prototype)、口袋版（dsh-Go)、独立作者推出的本地 Android Agent（Mika)和一堆 Claude Skill（unslop、pixelfx、floorplan、tstack),说明 "Agent 作为开发工具的形态" 已经分化成**官方框架 vs 本地 App vs IDE 内 Skill** 三条并行路线。
- **Claude Skills 迎来真正的用户基础**：Unslop、Pixelfx、Floorplan、Craft Anything、tstack 几乎都带有 "本仓库 = Claude Code Skill" 的 README 开头——Skill 这个三个月前刚起的小生态,现在已经可以撑起今日 Trending 的 1/3 席位。
- **中文开发者的实用主义**：Android Ad Cleaner、AI Pose Gallery、Word Atlas、Mika——四个中文项目同时登榜,共同点是解决具体生活痛点,而不是追前沿模型。这是过去两年 GitHub 上少见的"中文开源不再只是追英文圈"的现象。
- **硬件/游戏逆向重新抬头**：GPU 解锁、Switch 2 模拟器、TotK PC 重编译、iPhone LiDAR 3D 建模——这些项目共同指向 "开发者越来越愿意碰硬件逆向" 的趋势。背景可能是 AI capex 让云服务越来越贵,而本地算力又因 Apple Silicon / RTX 50 系的普及变得可用。

一句话总结:**AI Agent 已经从新鲜事变成基础设施,而开发者社区正在用新基础设施做"手边够用" 的小工具,而不是继续追逐 "下一个 ChatGPT"。** 这是 2026 年开源社区最健康的分流信号。
