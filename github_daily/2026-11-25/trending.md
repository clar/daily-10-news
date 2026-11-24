# GitHub Trending 日报 · 2026-11-25

来源：[GitHub Trending 官方日榜](https://github.com/trending)（不限语言），上海时间 11 月 25 日抓取。官方未标明页面刷新时间；“今日新增”取页面原值，不等于上海时间零点以来的净增，不决定榜序。

## 今日焦点

> **工具接口 · 工程验证 · 上架检查 · 图解设计**
>
> - `HKUDS/CLI-Anything` 第 3，+1,075⭐，较上期日增多 292，是前 15 名中升幅最大的项目。
> - `obra/superpowers` 第 2，+1,006⭐，较上期多 168。
> - `mjmirza/app-store-compliance` 第 12，+936⭐，较上期多 181。
> - `cathrynlavery/diagram-design` 第 9，+794⭐，较上期多 170。

---

## 今日热榜总览

本期前 15 名均为续榜，成员与名次和 11 月 24 日快照逐项相同。末列比较的是两个快照各自显示的“今日新增”，不是总星数差。

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks | 今日新增较上期 |
|------|------|------|------|--------|-----------|-------|----------------|
| 1 | 安全工具（略） | 略 | Python | 21,162 | +1,833⭐ | 2,211 | -204 |
| 2 | [obra/superpowers](https://github.com/obra/superpowers) | 编程代理的工程流程与技能组合 | Shell | 325,813 | +1,006⭐ | 28,892 | +168 |
| 3 | [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | 将现有应用包装成代理可调用的命令 | Python | 64,587 | +1,075⭐ | 5,888 | +292 |
| 4 | [jingyaogong/minimind](https://github.com/jingyaogong/minimind) | 小型语言模型训练教学 | Python | 70,086 | +727⭐ | 9,126 | -101 |
| 5 | [cursor/plugins](https://github.com/cursor/plugins) | Cursor 官方插件与插件规范 | TypeScript | 19,128 | +359⭐ | 2,067 | -36 |
| 6 | [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) | 网页检索、抓取与信息提取接口 | TypeScript | 208,734 | +990⭐ | 10,906 | +70 |
| 7 | [nginx/nginx](https://github.com/nginx/nginx) | 开源 Web 服务器与反向代理 | C | 33,175 | +158⭐ | 8,392 | -16 |
| 8 | [openvinotoolkit/openvino](https://github.com/openvinotoolkit/openvino) | 模型推理优化和部署工具 | C++ | 12,423 | +187⭐ | 3,690 | +4 |
| 9 | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | 生成可独立浏览的 HTML 和 SVG 图解 | HTML | 71,832 | +794⭐ | 4,793 | +170 |
| 10 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 汇集近期公开讨论并生成研究摘要 | Python | 74,057 | +695⭐ | 6,530 | -95 |
| 11 | [google-labs-code/stitch-skills](https://github.com/google-labs-code/stitch-skills) | 与 Stitch MCP 配合的跨客户端设计技能 | TypeScript | 12,582 | +401⭐ | 1,524 | -24 |
| 12 | [mjmirza/app-store-compliance](https://github.com/mjmirza/app-store-compliance) | 移动应用商店提交前检查和发布指南 | Shell | 5,698 | +936⭐ | 369 | +181 |
| 13 | [Tracer-Cloud/opensre](https://github.com/Tracer-Cloud/opensre) | 面向持续集成与交付可靠性的开源代理 | Python | 15,121 | +408⭐ | 2,006 | -30 |
| 14 | [toeverything/AFFiNE](https://github.com/toeverything/AFFiNE) | 整合文档、白板和知识管理的工作空间 | TypeScript | 77,866 | +589⭐ | 5,695 | -4 |
| 15 | [XiaoYouChR/Ghost-Downloader-3](https://github.com/XiaoYouChR/Ghost-Downloader-3) | 开源桌面文件下载工具 | Python | 17,182 | +1,102⭐ | 1,041 | +24 |

---

## 重点项目点评

### [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) · 第 3，+1,075⭐

**让代理重复调用软件时，不必每次重新找按钮。** 这个项目把已有应用功能包装为命令。团队由此可以记录调用参数、保存结果，并在应用升级后检查同一任务是否仍能完成。

本期日增升幅在前 15 名中最大，但榜单并不能说明是谁在使用它。实用的评估标准是看失败能否恢复、返回是否可验证，以及读操作和写操作是否明确分开。

### [obra/superpowers](https://github.com/obra/superpowers) · 第 2，+1,006⭐

**代理能写出代码，不代表它知道何时可以交付。** Superpowers 将需求澄清、计划、测试、审查组织为可复用技能，帮助团队事先定义可接受的交付证据。

对有多名开发者或多个代理的项目，我会先固定最常漏的验证步骤，再测返工时间是否下降。不必让每次小修都付出和大型功能相同的流程成本。

### [mjmirza/app-store-compliance](https://github.com/mjmirza/app-store-compliance) · 第 12，+936⭐

**把上架驳回从发布当天提前到提交之前。** 项目将常见审核问题和隐私等提交字段整理为可执行的检查。它把代理工作从生成代码推到更容易遗漏的发布末端。

最合适的用法是将通用清单当预检查，再用平台最新要求和应用实际行为逐项核实。清单能减少漏项，不能替代平台审核。

### [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) · 第 9，+794⭐

**让系统图能随代码一起审阅。** 这个项目提供供代理使用的图解设计技能，输出可以独立打开的 HTML 与 SVG。对架构或流程评审，独立文件比只能留在聊天记录里的图片更方便追踪变更。

真正要审核的是连线和依赖是否符合实现，而非美观程度。一次小范围试用就能看出：新版本发布后，图能否跟着代码一起更新。

---

## 生态观察

虽然榜序不变，新增关注有起伏：CLI-Anything、上架检查和图解设计的日增分别多了 292、181 和 170；last30days-skill 与 MiniMind 分别少了 95 和 101。这提示本期值得看的是同一批项目里工程交付环节的相对变化，不是新项目替代旧项目。单次快照不能证明增星缘由或实际采用率。
