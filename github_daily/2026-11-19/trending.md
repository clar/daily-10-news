# GitHub Trending 日报 · 2026-11-19

数据取自 [GitHub Trending 日榜](https://github.com/trending)，榜序及每日新增以所查到的官方页面快照为准，并与 [GitStock 11 月 19 日存档](https://gitstock.org/trending/2026-11-19) 交叉核验。页面没有公开精确快照时间；“今日新增”是 GitHub 的统计口径，不等同于上海时间零点以来的净增。

## 今日焦点

> **插件分发 · 命令行接口 · 技能评测 · 科研写作**
>
> - `cursor/plugins` 以 +314⭐ 登顶，官方规范让第三方扩展有了共同的发布格式。
> - `HKUDS/CLI-Anything` 新增 +389⭐，把既有软件功能包装成代理可调用的命令。
> - `NVIDIA/SkillEvaluator` 新增 +312⭐，用有无技能的对照运行检查实际收益。
> - `google-research/paper-orchestra` 新增 +1,524⭐，是前 15 名中新增最多的仓库。

---

## 今日热榜总览

| 排名 | 仓库 | 描述 | 语言 | 总星数 | 今日新增⭐ | Forks |
|------|------|------|------|--------|-----------|-------|
| 1 | [cursor/plugins](https://github.com/cursor/plugins) | Cursor 插件规范与官方插件 | TypeScript | 17,242 | +314⭐ | 1,904 |
| 2 | [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | 为既有软件生成适合代理调用的命令行接口 | Python | 59,818 | +389⭐ | 5,432 |
| 3 | [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) | 聚合多个公开平台的近期讨论，生成带来源的研究摘要 | Python | 70,077 | +1,059⭐ | 6,247 |
| 4 | [getarcaneapp/arcane](https://github.com/getarcaneapp/arcane) | 用网页界面管理 Docker 资源 | Go | 9,842 | +547⭐ | 565 |
| 5 | [NVIDIA/SkillEvaluator](https://github.com/NVIDIA/SkillEvaluator) | 分层评估代理技能和插件的质量及效果 | Python | 3,760 | +312⭐ | 519 |
| 6 | [nvm-sh/nvm](https://github.com/nvm-sh/nvm) | 在同一环境管理和切换多个 Node.js 版本 | Shell | 96,161 | +237⭐ | 10,781 |
| 7 | [astral-sh/uv](https://github.com/astral-sh/uv) | 用 Rust 编写的 Python 包与项目管理工具 | Rust | 92,245 | +258⭐ | 3,923 |
| 8 | [google-research/paper-orchestra](https://github.com/google-research/paper-orchestra) | 用多个代理协作起草科研论文 | Python | 4,351 | +1,524⭐ | 538 |
| 9 | [google-labs-code/stitch-skills](https://github.com/google-labs-code/stitch-skills) | 面向 Stitch MCP 服务的跨代理客户端技能库 | TypeScript | 10,425 | +365⭐ | 1,368 |
| 10 | [sveltejs/svelte](https://github.com/sveltejs/svelte) | 以编译为核心的 Web 界面框架 | JavaScript | 89,638 | +692⭐ | 6,208 |
| 11 | [jquery/jquery](https://github.com/jquery/jquery) | 用于 DOM 操作和事件处理的 JavaScript 库 | JavaScript | 60,022 | +266⭐ | 20,709 |
| 12 | [appwrite/appwrite](https://github.com/appwrite/appwrite) | 提供认证、数据库、存储和函数等能力的开源后端平台 | TypeScript | 58,249 | +232⭐ | 5,883 |
| 13 | [openvinotoolkit/openvino](https://github.com/openvinotoolkit/openvino) | 优化和部署 AI 模型推理的工具包 | C++ | 11,349 | +24⭐ | 3,603 |
| 14 | [obra/superpowers](https://github.com/obra/superpowers) | 面向编程代理的技能框架与开发流程 | Shell | 321,368 | +822⭐ | 28,561 |
| 15 | [affaan-m/ECC](https://github.com/affaan-m/ECC) | 为多种编程代理提供技能、记忆和工程工作流配置 | JavaScript | 306,573 | +1,108⭐ | 45,129 |

---

## 重点项目点评

### 🥇 [cursor/plugins](https://github.com/cursor/plugins) · 今日榜首，+314⭐

**让插件从一组本地文件变成可以发布的扩展。** 这个仓库不只是官方插件合集，也给出了插件的组织规范。开发者有了可参照的结构和示例，不必每次自己约定如何打包、发现和维护扩展。

与同榜的 Stitch Skills 对照，值得看的是同一项能力能否在不同客户端低成本复用，而不是某家平台的插件数有多少。它是今日榜首，但并非新增星数榜首；两项指标不能混用。

### 🥈 [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) · +389⭐

**让代理调用已有软件，而不是重新实现它。** 这个项目为既有应用包装命令行接口。相比让代理根据屏幕截图找按钮，有明确参数和输出的命令更容易复现、记录与测试。

这条路线能否落地，要看包装层是否真实调用了应用、出错时是否能给出可靠反馈，以及升级之后接口是否仍然兼容。对有大量存量工具的团队来说，这比演示中能跑通一次更重要。

### [NVIDIA/SkillEvaluator](https://github.com/NVIDIA/SkillEvaluator) · 第 5，+312⭐

**技能写得好不好，和它能否提高成功率，是两件事。** SkillEvaluator 把格式检查、语义重叠检测与真实代理运行分开；其中最值得看的是使用和不使用技能的对照，避免把基础模型本来就会做的事算成技能收益。

如果团队已经累积了大量技能，与其再新增一批，不妨先选几个真实高频任务做对照，记录成功率、耗时和额外调用成本。测试集的代表性比单次分数更重要。

### [google-research/paper-orchestra](https://github.com/google-research/paper-orchestra) · 第 8，+1,524⭐

**把研究材料整理成论文初稿，但不替代科研判断。** PaperOrchestra 将论文起草拆成多个协作环节，适合把已有研究笔记和实验结果整理成结构、章节与图表。它在这份榜单前 15 名里新增最多，显示出对科研写作工作流的关注。

实际价值要看论文中的结论能否回溯到原始记录，引用和图表能否独立核查。对作者而言，比较稳妥的用法是把它当起草与整理工具，而不是实验结论或文献真实性的裁判。

## 生态观察

今天最清楚的一条线是：代理技能开始分化出发布规范、软件接口和评估工具。Cursor 管分发，CLI-Anything 管调用，SkillEvaluator 检验技能是否有用；PaperOrchestra 则展示这些能力如何进入具体行业。同时，nvm、uv、Svelte 和 jQuery 也都在榜上。单日星数反映注意力，不说明框架迁移已经发生，也不说明这些工具已达到生产可用水平。

