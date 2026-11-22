# GitHub Trending 日报 · 2026-11-23

[GitHub Trending 官方日榜](https://github.com/trending)（不限语言），上海时间 11 月 23 日约 05:00 查询。官方未标示榜单更新时间；“今日新增”是 GitHub 页面口径，不代表上海时间零点以来的净增。前 15 名的成员及榜序和 11 月 22 日快照相同，以下全部标为续榜；数值已重新核对。

## 今日焦点

> **代理流程 · 网页研究 · 跨工具设计 · 推理部署**
>
> - `obra/superpowers` 第 2，+785⭐，把测试、审查和交付验证整理成代理可复用的流程。
> - `mvanhorn/last30days-skill` 第 10，+673⭐，近期讨论检索的热度较上一快照回升。
> - `google-labs-code/stitch-skills` 第 11，+516⭐，把设计协作接到多种编码代理。
> - `openvinotoolkit/openvino` 第 8，+155⭐，提供模型推理优化与部署工具。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | `elementalsouls/Claude-BugHunter` | Claude Code 安全评估技能合集 | Python | 17,451 | +1,721⭐ | 1,945 |
| 2 | [obra/superpowers](https://github.com/obra/superpowers) | 编程代理的技能组合与工程流程 | Shell | 324,040 | +785⭐ | 28,754 |
| 3 | [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | 为已有软件提供代理可调用的命令行接口 | Python | 62,662 | +687⭐ | 5,683 |
| 4 | [jingyaogong/minimind](https://github.com/jingyaogong/minimind) | 从零训练小型语言模型的教学项目 | Python | 68,572 | +473⭐ | 8,969 |
| 5 | [cursor/plugins](https://github.com/cursor/plugins) | Cursor 官方插件与插件规范 | TypeScript | 18,387 | +301⭐ | 1,999 |
| 6 | [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) | 网页搜索、抓取与结构化数据提取 | TypeScript | 206,870 | +910⭐ | 10,811 |
| 7 | [nginx/nginx](https://github.com/nginx/nginx) | 开源 Web 服务器及反向代理 | C | 32,856 | +168⭐ | 8,381 |
| 8 | [openvinotoolkit/openvino](https://github.com/openvinotoolkit/openvino) | AI 模型推理优化与部署工具包 | C++ | 12,064 | +155⭐ | 3,656 |
| 9 | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | 为代理提供可独立分享的 HTML 与 SVG 图解 | HTML | 70,212 | +513⭐ | 4,712 |
| 10 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 汇集多个平台的近期讨论并生成研究摘要 | Python | 72,599 | +673⭐ | 6,419 |
| 11 | [google-labs-code/stitch-skills](https://github.com/google-labs-code/stitch-skills) | 与 Stitch MCP 配合的跨客户端设计技能 | TypeScript | 11,845 | +516⭐ | 1,472 |
| 12 | [mjmirza/app-store-compliance](https://github.com/mjmirza/app-store-compliance) | 移动应用商店提交前检查与发布指南 | Shell | 3,869 | +617⭐ | 234 |
| 13 | [Tracer-Cloud/opensre](https://github.com/Tracer-Cloud/opensre) | 用于提升持续集成与交付可靠性的代理 | Python | 14,327 | +395⭐ | 1,960 |
| 14 | [toeverything/AFFiNE](https://github.com/toeverything/AFFiNE) | 整合文档、白板及知识库的工作空间 | TypeScript | 76,721 | +537⭐ | 5,613 |
| 15 | [XiaoYouChR/Ghost-Downloader-3](https://github.com/XiaoYouChR/Ghost-Downloader-3) | 开源桌面下载工具 | Python | 15,016 | +690⭐ | 901 |

---

## 重点项目点评

### [obra/superpowers](https://github.com/obra/superpowers) · 第 2，+785⭐，续榜

**团队需要的不是更多步骤，而是知道哪些步骤不能省。** 该项目把设计、测试与审查组织成代理可复用的技能。把验证要求写清楚，比依赖大家每次都想起来提醒代理更可靠。

对于重复任务，先统一最低验证标准，再用返工率和耗时判断是否要增加流程。小改动和跨模块重构不必共用一套重流程。

### [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) · 第 10，+673⭐，续榜

**适合发现最近在讨论什么，不适合直接判定事实。** 这个技能从多个公开渠道搜集近期讨论，再整理成摘要；它和同榜的 Firecrawl 分工不同，前者偏研究流程，后者偏数据接入。

适合先拿来生成线索，再追到原始报道、文档或发布说明。遇到同一故事被多平台转发时，应按独立来源去重，不能把讨论数量当作事实置信度。

### [google-labs-code/stitch-skills](https://github.com/google-labs-code/stitch-skills) · 第 11，+516⭐，续榜

**复用的是设计工作方法，不只是一个插件。** 项目将设计相关技能交给不同代理客户端，并通过 Stitch MCP 接入服务。值得观察的是设计任务能否在现有工具中复用，而不是团队是否要因此统一更换编辑器。

落地可先选一个小页面：检查同一需求在不同客户端的输出是否便于审阅、是否保留设计约束。兼容技能格式不等于结果一致。

### [openvinotoolkit/openvino](https://github.com/openvinotoolkit/openvino) · 第 8，+155⭐，续榜

**把模型跑起来和把模型稳定交付是两回事。** OpenVINO 面向推理优化和部署。与同榜的 MiniMind 相比，两者分别对应部署和训练；值得关注的是同一模型在真实硬件上的响应时间和资源成本，而不是榜单名次。

比较方案时应固定模型、输入和硬件，分别测延迟、吞吐及内存占用。一次基础演示不能代替应用自己的负载测试。

---

## 生态观察

本期没有新增进入前 15 名的项目，但关注度并非静止：Stitch Skills 的 GitHub 日增从 +324⭐ 变为 +516⭐，last30days-skill 从 +566⭐ 变为 +673⭐，Firecrawl 则从 +999⭐ 降至 +910⭐。这一轮更适合观察同一批项目里哪类工作受到更多关注，而不能据此宣称市场份额发生变化。
