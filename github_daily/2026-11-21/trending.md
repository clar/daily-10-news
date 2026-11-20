# GitHub Trending 日报 · 2026-11-21

数据来自 [GitHub Trending 官方日榜](https://github.com/trending)，为上海时间 11 月 21 日清晨查询到的不限语言快照。GitHub 未标明榜单更新时间；“今日新增”沿用页面口径，不等于上海时间零点以来的净增，榜序也不按新增星数排列。

## 今日焦点

> **网页数据 · 代理工程流程 · 模型训练 · 应用上架**
>
> - `firecrawl/firecrawl` 第 6，+1,226⭐，单一接口覆盖网页发现、抓取和结构化提取。
> - `obra/superpowers` 第 2，+888⭐，把编码代理的设计、测试和审查步骤变成可复用流程。
> - `jingyaogong/minimind` 第 4，+841⭐，用小模型展示从训练到部署的基本流程。
> - `mjmirza/app-store-compliance` 第 12，+874⭐，将商店审核常见问题变成提交前检查。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [elementalsouls/Claude-BugHunter](https://github.com/elementalsouls/Claude-BugHunter) | 面向安全评估的 Claude Code 技能合集 | Python | 13,877 | +1,660⭐ | 1,665 |
| 2 | [obra/superpowers](https://github.com/obra/superpowers) | 面向编程代理的技能组合与开发流程 | Shell | 322,715 | +888⭐ | 28,667 |
| 3 | [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | 为已有软件提供代理可调用的命令行接口 | Python | 61,236 | +774⭐ | 5,547 |
| 4 | [jingyaogong/minimind](https://github.com/jingyaogong/minimind) | 从零训练小型语言模型的教学项目 | Python | 67,609 | +841⭐ | 8,863 |
| 5 | [cursor/plugins](https://github.com/cursor/plugins) | Cursor 插件规范与官方插件 | TypeScript | 17,785 | +292⭐ | 1,955 |
| 6 | [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) | 通过统一接口搜索、抓取网页并提取数据 | TypeScript | 205,062 | +1,226⭐ | 10,748 |
| 7 | [nginx/nginx](https://github.com/nginx/nginx) | NGINX Web 服务器及反向代理的官方开源仓库 | C | 32,522 | +246⭐ | 8,432 |
| 8 | [openvinotoolkit/openvino](https://github.com/openvinotoolkit/openvino) | 面向模型推理优化与部署的工具包 | C++ | 11,737 | +219⭐ | 3,634 |
| 9 | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | 帮助编程代理生成 HTML 和 SVG 图解的设计技能 | HTML | 69,189 | +634⭐ | 4,656 |
| 10 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 汇集公开平台的近期讨论并生成研究摘要 | Python | 71,341 | +685⭐ | 6,347 |
| 11 | [google-labs-code/stitch-skills](https://github.com/google-labs-code/stitch-skills) | 与 Stitch MCP 配合使用的跨客户端技能库 | TypeScript | 10,957 | +315⭐ | 1,401 |
| 12 | [mjmirza/app-store-compliance](https://github.com/mjmirza/app-store-compliance) | 面向移动应用商店的提交前检查与发布指南 | Shell | 2,592 | +874⭐ | 168 |
| 13 | [Tracer-Cloud/opensre](https://github.com/Tracer-Cloud/opensre) | 面向持续集成与交付可靠性的开源代理 | Python | 13,521 | +465⭐ | 1,922 |
| 14 | [toeverything/AFFiNE](https://github.com/toeverything/AFFiNE) | 整合文档、白板与知识管理的工作空间 | TypeScript | 75,670 | +686⭐ | 5,584 |
| 15 | [XiaoYouChR/Ghost-Downloader-3](https://github.com/XiaoYouChR/Ghost-Downloader-3) | 开源桌面文件下载工具 | Python | 13,561 | +1,082⭐ | 833 |

---

## 重点项目点评

### [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) · 第 6，+1,226⭐

**代理做研究前，先得拿到能用的材料。** Firecrawl 负责网页搜索、抓取与正文提取；同榜的 last30days-skill 更靠近任务终点，负责把检索结果组织成回答。两者同时入榜，值得留意的是网页数据接入正被独立做成基础设施。

如果用在事实核查，稳定提取正文只是起点。还要保留源链接、发布时间和抓取时间，能辨认付费墙或提取缺失，避免把格式整齐的结果误当作完整证据。

### [obra/superpowers](https://github.com/obra/superpowers) · 第 2，+888⭐

**把容易跳过的工程步骤写进代理工作流。** 这个仓库把设计、规划、测试和审查整理成可复用技能。它的吸引力不是让代理写出更多代码，而是让团队更容易约定哪些步骤不能省。

这类工具最好用返工率、遗漏率和交付时长来评估。多模块修改往往值得先约定边界和验证方法；单行改动如果也被迫走完整流程，收益反而容易被等待时间抵消。

### [jingyaogong/minimind](https://github.com/jingyaogong/minimind) · 第 4，+841⭐

**用跑得动的小模型理解训练，而不是追求大模型能力。** MiniMind 将从头训练变成个人可以尝试的工程练习。它适合把数据、训练过程和输出质量联系起来，而不是只从调用模型接口理解语言模型。

它和同榜的 OpenVINO 分别落在训练学习和推理部署两端。两者一起说明：除了给代理写技能，如何获得、运行以及理解模型本身，仍是开发者关注的一条线。

### [mjmirza/app-store-compliance](https://github.com/mjmirza/app-store-compliance) · 第 12，+874⭐

**让检查发生在发布之前，而不是等驳回再补。** 这个项目把常见审核问题、隐私信息和提交检查整理成可复用清单。对移动应用小团队来说，价值主要在于少漏项、缩短来回返工，而非替产品做审核判断。

适合把它当预检查，不适合当成上架保证。规则随平台、地区和应用类别而变，尤其是隐私填写，仍需以官方要求和应用实际行为为准。

---

## 生态观察

这次所见的前 15 名榜序与上一期相同，但新增星数并不相同。Firecrawl 从 +795⭐ 变为 +1,226⭐，MiniMind 从 +301⭐ 变为 +841⭐，应用上架检查工具从 +542⭐ 变为 +874⭐。这一快照中，关注并不只集中在编码代理框架，也流向网页数据、模型训练和发布检查等具体环节。星数是关注度信号，不是生产可用性或市场采用率的证明。
