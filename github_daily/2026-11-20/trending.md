# GitHub Trending 日报 · 2026-11-20

数据取自 [GitHub Trending 官方日榜](https://github.com/trending)（不限语言），榜首及每日新增与 [11 月 20 日存档](https://www.mackeabit.co.kr/trending/date/2026-11-20/) 抽样交叉核验。官方页面未标明精确抓取时间；“今日新增”沿用 GitHub 口径，不代表上海时间零点以来的净增，榜序也不按新增星数排列。

## 今日焦点

> **代理工作流 · 软件接口 · 网页数据 · 移动应用发布**
>
> - `obra/superpowers` 排第 2，+2,029⭐，是本期前 15 名中新增最多的项目。
> - `HKUDS/CLI-Anything` 排第 3，+899⭐，关注如何让代理直接调用已有软件。
> - `firecrawl/firecrawl` 排第 6，+795⭐，把网页检索与结构化提取放到同一个接口。
> - `mjmirza/app-store-compliance` 排第 12，+542⭐，把应用商店提交前的检查提前到开发流程。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [elementalsouls/Claude-BugHunter](https://github.com/elementalsouls/Claude-BugHunter) | 面向安全评估的 Claude Code 技能合集 | Python | 12,267 | +1,353⭐ | 1,577 |
| 2 | [obra/superpowers](https://github.com/obra/superpowers) | 面向编程代理的技能组合与软件开发流程 | Shell | 321,951 | +2,029⭐ | 28,618 |
| 3 | [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | 为已有应用提供代理可调用的命令行接口 | Python | 60,425 | +899⭐ | 5,484 |
| 4 | [jingyaogong/minimind](https://github.com/jingyaogong/minimind) | 从零训练小型语言模型的教学项目 | Python | 66,778 | +301⭐ | 8,778 |
| 5 | [cursor/plugins](https://github.com/cursor/plugins) | Cursor 插件规范与官方插件 | TypeScript | 17,502 | +383⭐ | 1,928 |
| 6 | [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) | 为代理和应用提供网页搜索、抓取与信息提取 | TypeScript | 203,991 | +795⭐ | 10,689 |
| 7 | [nginx/nginx](https://github.com/nginx/nginx) | NGINX Web 服务器及反向代理的官方开源仓库 | C | 32,288 | +66⭐ | 8,411 |
| 8 | [openvinotoolkit/openvino](https://github.com/openvinotoolkit/openvino) | 用于优化和部署模型推理的工具包 | C++ | 11,524 | +246⭐ | 3,619 |
| 9 | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | 帮助编程代理生成独立 HTML、SVG 图解的设计技能 | HTML | 68,535 | +332⭐ | 4,608 |
| 10 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 汇集多个公开平台的近期讨论，产出带来源的研究摘要 | Python | 70,698 | +952⭐ | 6,298 |
| 11 | [google-labs-code/stitch-skills](https://github.com/google-labs-code/stitch-skills) | 与 Stitch MCP 配合使用的跨客户端技能库 | TypeScript | 10,660 | +303⭐ | 1,383 |
| 12 | [mjmirza/app-store-compliance](https://github.com/mjmirza/app-store-compliance) | 面向 App Store 和 Google Play 的提交前检查与发布指南 | Shell | 1,719 | +542⭐ | 122 |
| 13 | [Tracer-Cloud/opensre](https://github.com/Tracer-Cloud/opensre) | 面向持续集成与交付可靠性的开源代理 | Python | 13,043 | +25⭐ | 1,899 |
| 14 | [toeverything/AFFiNE](https://github.com/toeverything/AFFiNE) | 将文档、白板与知识管理整合在一起的工作空间 | TypeScript | 75,043 | +170⭐ | 5,555 |
| 15 | [XiaoYouChR/Ghost-Downloader-3](https://github.com/XiaoYouChR/Ghost-Downloader-3) | 开源桌面文件下载工具 | Python | 12,552 | +449⭐ | 785 |

---

## 重点项目点评

### [obra/superpowers](https://github.com/obra/superpowers) · 第 2，+2,029⭐

**把工程步骤交给代理执行，而不是每回都重新提醒。** 这个项目把需求澄清、规划、测试和代码审查组织成一组可以复用的技能。它针对的不是模型能不能写代码，而是同一个团队能否让代理在不同任务里按一致的标准交付。

它是本期前 15 名中新增最多的仓库。我的判断是，工作流类项目的价值要看返工是否变少，而不是代理是否生成了更长的计划。小改动和跨模块功能不必套用同样重的流程。

### [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) · 第 3，+899⭐

**让已有软件变成代理能稳定调用的工具。** 项目围绕命令行包装展开：应用执行实际任务，代理负责组织参数和读取输出。相比让代理看屏幕猜按钮位置，明确的命令更容易做回归测试，也更容易记录失败发生在哪里。

这解释了为什么它和工作流技能同时受关注：有了流程，还需要可靠的动作接口。接入价值取决于接口是否足够稳定、失败原因是否能被反馈给代理，以及应用更新后需要谁维护这一层。

### [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) · 第 6，+795⭐

**把网页从“给人看的界面”整理成“给代理用的材料”。** 它将查找网页、抓取正文和提取结构化数据集中到一个接口。做资料收集时，这能减少团队反复维护 HTML 解析逻辑的负担。

同榜的 last30days-skill 更接近面向用户的研究工作流，而 Firecrawl 偏向为此类工作流提供原料。选型时应分开看两件事：正文能否稳定提取，以及最终摘要能否溯源；前者并不能保证后者。

### [mjmirza/app-store-compliance](https://github.com/mjmirza/app-store-compliance) · 第 12，+542⭐

**把上架驳回从发布当天移到提交之前。** 这个项目把常见驳回情形和隐私声明等检查集中起来，并做成适合编程代理使用的技能。对小团队而言，它解决的是会反复出现、却很难靠记忆做到不漏项的工作。

它说明技能不只适合写代码，也适合整理明确、重复的发布检查。但第三方清单不等于审核结论：规则会随时间、地区和应用类别变化，正式提交仍以平台最新要求为准。

---

## 生态观察

昨天的榜单突出插件分发和技能评测；今天关注点更多落在具体工作上：怎样按团队流程写代码、怎样调用已有软件，以及怎样取得代理能用的数据。应用上架检查是一个有意思的例子，使用者需要的未必是更聪明的模型，而是把容易遗漏的检查放进开发流程。一日榜单只反映当下的注意力，不能当成采用率或软件质量排名。
