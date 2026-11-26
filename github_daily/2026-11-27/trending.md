# GitHub Trending 日报 · 2026-11-27

来源：[GitHub Trending 官方日榜](https://github.com/trending)（不限语言）。上海时间 11 月 27 日约 05:05 读取；官方未标明页面数据的刷新时刻。“今日新增”是官方页面口径，不等于上海时间零点以来的净增，也不决定榜序。

## 今日焦点

> **网页数据 · 图解交付 · 插件扩展 · 应用发布**
>
> - `firecrawl/firecrawl` 第 6，+1,042⭐，连续两期日增过千。
> - `cathrynlavery/diagram-design` 第 9，+951⭐，较上期少 182。
> - `cursor/plugins` 第 5，+268⭐，官方插件库总星数接近两万。
> - `mjmirza/app-store-compliance` 第 12，+561⭐，较上期少 292。

---

## 今日热榜总览

前 15 名均为续榜，名次与 11 月 26 日快照逐项相同。末列对比两次官方页面各自列出的“今日新增”，不是总星数变化。

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks | 今日新增较上期 |
|------|------|------|------|--------|-----------|-------|----------------|
| 1 | 未列名 | 安全评估项目，名称略 | Python | 24,298 | +1,600⭐ | 2,471 | -44 |
| 2 | [obra/superpowers](https://github.com/obra/superpowers) | 编程代理的工程流程与验证技能 | Shell | 327,334 | +853⭐ | 29,028 | -49 |
| 3 | [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | 为已有软件建立代理可调用的命令行接口 | Python | 66,240 | +744⭐ | 6,021 | -350 |
| 4 | [jingyaogong/minimind](https://github.com/jingyaogong/minimind) | 从零训练小型语言模型的教学项目 | Python | 71,560 | +701⭐ | 9,288 | -127 |
| 5 | [cursor/plugins](https://github.com/cursor/plugins) | Cursor 插件规范及官方插件 | TypeScript | 19,749 | +268⭐ | 2,130 | -140 |
| 6 | [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) | 网页检索、抓取与结构化提取 | TypeScript | 210,797 | +1,042⭐ | 11,041 | -89 |
| 7 | [nginx/nginx](https://github.com/nginx/nginx) | 开源 Web 服务器和反向代理 | C | 33,500 | +150⭐ | 8,416 | -24 |
| 8 | [openvinotoolkit/openvino](https://github.com/openvinotoolkit/openvino) | 模型推理优化和部署工具 | C++ | 12,788 | +176⭐ | 3,727 | -12 |
| 9 | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | 生成独立 HTML 和 SVG 图解 | HTML | 73,739 | +951⭐ | 4,918 | -182 |
| 10 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 汇集公开平台上的近期讨论 | Python | 75,640 | +755⭐ | 6,669 | -195 |
| 11 | [google-labs-code/stitch-skills](https://github.com/google-labs-code/stitch-skills) | 与 Stitch MCP 配合的跨客户端设计技能 | TypeScript | 13,231 | +308⭐ | 1,557 | -44 |
| 12 | [mjmirza/app-store-compliance](https://github.com/mjmirza/app-store-compliance) | 移动应用商店提交前检查 | Shell | 6,930 | +561⭐ | 458 | -292 |
| 13 | [Tracer-Cloud/opensre](https://github.com/Tracer-Cloud/opensre) | 面向 CI/CD 可靠性的开源代理 | Python | 15,754 | +325⭐ | 2,051 | -18 |
| 14 | [toeverything/AFFiNE](https://github.com/toeverything/AFFiNE) | 集成文档、白板和知识库的工作空间 | TypeScript | 78,879 | +521⭐ | 5,743 | -57 |
| 15 | [XiaoYouChR/Ghost-Downloader-3](https://github.com/XiaoYouChR/Ghost-Downloader-3) | 桌面文件下载工具 | Python | 18,994 | +887⭐ | 1,142 | -63 |

---

## 重点项目点评

### [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) · 第 6，+1,042⭐

**研究助手的瓶颈不只在回答，也在拿到可靠的正文。** Firecrawl 将网页查找、抓取和结构化提取放在一个接口。它与同榜的 last30days-skill 分别覆盖内容获取和研究整理；把这两步分开，有利于定位摘要错误究竟出在读取还是解释。

评估这类工具时，我会拿同一批新闻、产品文档和动态页面测试，分别记录正文提取率、漏读情况，以及结果能否追溯到原始链接。连续两期日增过千说明受关注，但不能替代这类验证。

### [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) · 第 9，+951⭐

**图解最有用的时候，是关系能被逐条核查。** 该项目帮助代理输出能独立打开和分享的 HTML、SVG 图解。相比截一张图交付，可保留源文件的设计更便于审阅和迭代。

团队可以用一张真实的流程图试水：让使用者根据图指出依赖和异常分支，再与代码或文档核对。评价标准是减少理解偏差，而不是成品看起来像不像设计稿。

### [cursor/plugins](https://github.com/cursor/plugins) · 第 5，+268⭐

**官方插件仓库的长期价值在于降低分发和维护成本。** 这个项目同时提供插件规范与参考实现。对团队而言，判断标准不是可装多少插件，而是是否能复用同一份配置、限制可访问内容，并在升级时识别变更。

它和 Stitch Skills 指向不同路线：前者侧重特定客户端的扩展生态，后者强调让设计任务在多个客户端复用。已经在用多种编辑器的团队，不必为少量共用能力先统一整套工具。

### [mjmirza/app-store-compliance](https://github.com/mjmirza/app-store-compliance) · 第 12，+561⭐

**把上架规则变成每次发版都会跑过的清单。** 这个项目汇整常见驳回情形和提交前核对项。适合发布频繁的小团队先发现显而易见的遗漏，而不必等审核退回。

第三方清单可能滞后于平台，也无法证明隐私说明符合应用的实际行为。更稳妥的是把通用项和项目特有项分开，并记录每次驳回原因，用真实反馈修正检查重点。

---

## 生态观察

本期榜序没有变化，日增却整体走弱：15 个项目全部低于上期快照，其中 CLI-Anything 少 350，发布检查少 292，近期研究少 195。网页数据工具仍然日增过千。这个对比能描述所见热度变化，不能证明开发者采用率下滑，更不能解释变化原因。
