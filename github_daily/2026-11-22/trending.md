# GitHub Trending 日报 · 2026-11-22

数据来自 [GitHub Trending 官方日榜](https://github.com/trending)，为上海时间 11 月 22 日查询到的不限语言快照。官方页面未标明精确更新时间。“今日新增”是 GitHub 页面口径，不等于上海时间零点以来的净增，也不决定榜序。

## 今日焦点

> **网页数据 · 工程验证 · 命令行接口 · 图解设计**
>
> - `firecrawl/firecrawl` 第 6，+999⭐，把网页搜索、正文抓取和数据提取放在同一接口。
> - `obra/superpowers` 第 2，+884⭐，让编码代理按约定做设计、测试和审查。
> - `HKUDS/CLI-Anything` 第 3，+767⭐，让代理通过命令行调用已有应用。
> - `cathrynlavery/diagram-design` 第 9，+582⭐，用独立 HTML 与 SVG 输出便于分享和审阅的图解。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | elementalsouls/Claude-BugHunter | 面向安全评估的 Claude Code 技能合集 | Python | 15,782 | +1,794⭐ | 1,814 |
| 2 | [obra/superpowers](https://github.com/obra/superpowers) | 面向编程代理的技能组合与工程流程 | Shell | 323,616 | +884⭐ | 28,707 |
| 3 | [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | 把现有软件包装成代理可调用的命令行工具 | Python | 61,979 | +767⭐ | 5,612 |
| 4 | [jingyaogong/minimind](https://github.com/jingyaogong/minimind) | 从零训练小型语言模型的教学项目 | Python | 68,091 | +488⭐ | 8,902 |
| 5 | [cursor/plugins](https://github.com/cursor/plugins) | Cursor 官方插件与插件规范 | TypeScript | 18,064 | +261⭐ | 1,973 |
| 6 | [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) | 统一网页搜索、抓取和结构化提取的接口 | TypeScript | 206,048 | +999⭐ | 10,772 |
| 7 | [nginx/nginx](https://github.com/nginx/nginx) | NGINX Web 服务器和反向代理的开源仓库 | C | 32,707 | +195⭐ | 8,373 |
| 8 | [openvinotoolkit/openvino](https://github.com/openvinotoolkit/openvino) | 用于模型推理优化和部署的工具包 | C++ | 11,904 | +202⭐ | 3,648 |
| 9 | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | 帮助代理生成独立 HTML 与 SVG 图解的设计技能 | HTML | 69,746 | +582⭐ | 4,685 |
| 10 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 聚合多平台近期讨论并整理为带来源的摘要 | Python | 71,899 | +566⭐ | 6,371 |
| 11 | [google-labs-code/stitch-skills](https://github.com/google-labs-code/stitch-skills) | 与 Stitch MCP 配合使用的跨客户端技能库 | TypeScript | 11,360 | +324⭐ | 1,431 |
| 12 | [mjmirza/app-store-compliance](https://github.com/mjmirza/app-store-compliance) | 移动应用商店提交前检查和发布指南 | Shell | 3,296 | +724⭐ | 204 |
| 13 | [Tracer-Cloud/opensre](https://github.com/Tracer-Cloud/opensre) | 面向持续集成与交付可靠性的开源代理 | Python | 13,926 | +450⭐ | 1,942 |
| 14 | [toeverything/AFFiNE](https://github.com/toeverything/AFFiNE) | 整合文档、白板和知识库的工作空间 | TypeScript | 76,202 | +577⭐ | 5,592 |
| 15 | [XiaoYouChR/Ghost-Downloader-3](https://github.com/XiaoYouChR/Ghost-Downloader-3) | 开源桌面文件下载工具 | Python | 14,363 | +774⭐ | 875 |

---

## 重点项目点评

### [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) · 第 6，+999⭐

**把抓取和核查分成两步。** Firecrawl 面向网页数据接入，提供检索、抓取和结构化提取。它与同榜的 last30days-skill 对照鲜明：前者负责拿材料，后者更侧重把近期讨论整理成回答。二者同时在榜，说明研究工作流上下游都有独立工具的需求。

如果用于真正的事实核查，提取成功并不等于内容可信。保留原始页面链接、记录抓取时间，并把源站正文与自动生成的摘要区分开，比追求格式统一更重要。

### [obra/superpowers](https://github.com/obra/superpowers) · 第 2，+884⭐

**把「怎样算做完」变成可复用的工程约定。** Superpowers 将设计、实施计划、测试和审查拆成可复用的技能，减少每个任务重复交代流程的成本。对多人协作，它尤其适合明确何时要先澄清、验证什么、哪些结论必须附证据。

不过，流程越完整并不一定越省时间。可先挑一种常见改动跟踪返工和遗漏，再决定哪些步骤默认保留；单行改动和跨模块调整不必走同一套流程。

### [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) · 第 3，+767⭐

**接入现有软件，不一定要让代理学会读屏。** 项目提供为已有应用构建命令行接口的办法。输入输出明确，更容易做自动测试，也更容易还原同一操作为什么成功或失败。

实际应用的分水岭是接口能否在软件升级后继续工作、能否区分只读和会改动数据的操作。快速包装适合验证需求，高频流程则更需要稳定的接口和可预测的错误返回。

### [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) · 第 9，+582⭐

**图解也可以成为可检查的工程交付。** 项目以独立 HTML 和 SVG 生成图解，结果可以在浏览器打开，也更容易随代码一起审阅。它关注的是流程图、系统图能否清楚表达关系，不只是画得好看。

例如，在方案评审里，把图与实现放在一起，图中的依赖写错时就能通过代码变更一并修正。需要注意的是，排版清晰不等于关系准确；节点和方向仍应对照实际设计核查。

---

## 生态观察

本期前 15 名的榜序与上一期相同，但增星仍在变化。应用上架检查工具总星数从 2,592 增至 3,296；网页数据、代理工作流与应用接口项目也继续占据前列。相比判断哪一种代理「赢了」，这个快照更适合用来找值得单独改进的环节：拿数据、执行动作、验证改动，以及解释结果。单日星数只反映关注，不代表采用率或软件质量。
