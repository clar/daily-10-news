# AI 日报 · 2026-11-28

> 截至北京时间 11 月 28 日 05:00（11 月 27 日 21:00 UTC）。报道、交易交割、研究演示和产品上线分别标注。

## 今日焦点

> **AI 硬件供应链 · 政务智能体 · 自研芯片上的视频生成 · 多媒体压缩组件**
>
> - **媒体报道 OpenAI 对苹果提出反诉。** 涉及商业秘密和供应商关系；这是当事方指控，尚未经法院认定。
> - **阿联酋 FedAI 公布首批 17 个合作伙伴。** 名单是采购与实施的起点，不代表一半政府流程已迁移。
> - **Hugging Face 披露 Trainium3 的视频生成实验。** 在文中配置上，模型加载后，生成一段 10 秒有声视频用时约 22–23 秒。
> - **Kandinsky Lab 发布 KVAE-3.0。** 图像、视频和音频编码组件公开权重与推理代码，便于单独比较压缩和重建效果。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---------|---------|---------|---------|
| 1 | **据报道，OpenAI 在苹果商业秘密案中提出反诉**：11 月 27 日 19:06 UTC 前后见报，争议涉及消费硬件计划及供应商关系；双方各自的指控尚未经法院认定。 | [The Information](https://www.theinformation.com/briefings/openai-countersues-apple-trade-secrets-battle) | ⭐⭐⭐⭐ |
| 2 | **阿联酋联邦政务智能体平台 FedAI 公布首批 17 家合作伙伴**：包括微软、IBM、甲骨文和 Google Cloud；两年推动约一半政府业务相关流程采用智能体仍是目标。 | [哈姆丹官方发文](https://x.com/HamdanMohammed/status/2126209571672977580)、[当地报道与原文摘录](https://www.arnnewscentre.ae/en/news/uae/h-h-sheikh-hamdan-witnesses-17-partners-joining-uae-agentic-ai-ecosystem/) | ⭐⭐⭐⭐ |
| 3 | **Hugging Face 测试 Trainium3 上的 LTX-2.5**：在指定实验配置、模型已加载的情况下，生成 10 秒有声视频约需 22–23 秒；不是同口径跨芯片排名。 | [实验作者博客](https://huggingface.co/blog/video-trainium3) | ⭐⭐⭐ |
| 4 | **Kandinsky Lab 公开 KVAE-3.0**：发布适用于图像、视频和立体声音频的编码组件；其中图像版本由此前约 2.18 亿参数减至约 0.86 亿，相同测试协议下的重建分数接近。 | [研究团队发布稿](https://huggingface.co/blog/kandinskylab/kvae-3) | ⭐⭐⭐ |
| 5 | **印度 Aditya Infotech 完成收购 KGraph AI Solutions 30% 股权**：按完全摊薄口径，现金对价约 4.54 亿卢比；这是此前交易进展的交割更新。 | [印度国家证券交易所披露](https://nsearchives.nseindia.com/corporate/CPPLUS_27112026182333_seintimation.pdf) | ⭐⭐⭐ |
| 6 | **印度 Netweb 推出 Skylus Workspaces**：工作空间统一提供企业应用、容器环境及 GPU 资源入口；产品公告未给出实际部署规模。 | [印度国家证券交易所披露](https://nsearchives.nseindia.com/corporate/NETWEB1234_27112026075412_Intimation_Press_Release_Product_Launch.pdf) | ⭐⭐⭐ |
| 7 | **科技日报披露格秩科技 Envision AI 成立**：团队计划以空间物理基础模型为主线，探索可编辑 3D、模拟和可控视频；报道未提供成立日、模型交付时间或独立评测。 | [北京国际科技创新中心转载科技日报](https://www.ncsti.gov.cn/kjdt/kjrd/rgzn_kjrd/202611/t20261127_266193.html) | ⭐⭐⭐ |
| 8 | **Parallel Science 发布科研基础设施预印本**：提出分别记录 AI 生成研究与人类撰写研究，并允许相互引用；平台标识不等于研究经过人类同行评审。 | [项目预印本平台](https://papers.parallelscience.org/list/cs.AI/new) | ⭐⭐⭐ |
| 9 | **FINAL-Bench 团队公开模型看板当日快照**：团队称 27 日跟踪 885 个模型，同时公开数据与计算规则；汇总名次取决于覆盖范围与权重。 | [团队说明](https://huggingface.co/blog/FINAL-Bench/ai-model-market-daily-reading-ai-models-like-a-sto)、[快照数据](https://huggingface.co/datasets/VIDraft/ai-model-market-daily) | ⭐⭐⭐ |
| 10 | **独立开发者发布 Machine-load**：作者在 27 日公开展示这款 macOS 工具，按编程会话查看 CPU、项目和 Docker 负载；并非 Claude Code 官方功能。 | [项目仓库](https://github.com/Stak-Technologies/machine-load)、[作者发布帖](https://news.ycombinator.com/item?id=50670688) | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · AI 公司做硬件，首先得把供应链建起来

**[The Information 报道](https://www.theinformation.com/briefings/openai-countersues-apple-trade-secrets-battle)**

媒体报道 OpenAI 已在加州的既有争议中提出反诉，指控苹果不当获取其消费硬件计划等信息，并对共同供应商施压。苹果此前也曾就商业秘密向 OpenAI 提出指控。诉状陈述不是法院认定，当前不应将任何一方的主张写成已证实事实。

这场争议体现了 AI 公司跨入硬件行业的另一道门槛：产品量产依赖工程人才、组件供应与代工协作。模型能力可以带来用户需求，却不能代替供应链执行。

值得看的是后续公开法庭文件能证明什么，以及硬件项目有没有可独立核实的产能和交付进度。

**点评：** 先看法院文件和实际交付，别用诉状替厂商证明产品已经走到哪一步。

---

### 🏛 No.2 · FedAI 的首批合作名单公布，政务授权仍要按流程划分

**[哈姆丹官方发文](https://x.com/HamdanMohammed/status/2126209571672977580)** · **[当地报道与原文摘录](https://www.arnnewscentre.ae/en/news/uae/h-h-sheikh-hamdan-witnesses-17-partners-joining-uae-agentic-ai-ecosystem/)**

阿联酋公布 FedAI 的首批 17 个合作伙伴。统一入口可以减少机构各自整合供应商的工作，但从合作名单到公共服务上线，还要经过采购、对接、权限设计和运营验证。

回答办事问题和代居民提交申请是两类风险。后者需要明确授权范围、错误更正和审计，而不能只看回复是否流畅。两年的转型目标也需要按事项口径衡量，以免把已有聊天入口算作整条流程完成改造。

最有说服力的后续指标是分事项的成功办理率、错办率、人工转接和申诉处理时间。

**点评：** 政务自动化最重要的问题，是系统出错后居民能否及时纠正。

---

### 🎞 No.3 · Trainium3 的视频实验给出了一条复测起点

**[Hugging Face 实验记录](https://huggingface.co/blog/video-trainium3)**

作者记录了使用 Trainium3 运行 LTX-2.5 的案例。文中给出的 22–23 秒是模型加载后的生成时间，且对应指定机器配置，不包括所有生产开销。

对需要处理突发批量请求的团队，冷启动、排队和失败重试也会影响单条视频的实际成本。比较不同芯片时，还要固定视频规格、质量要求和运行设置，避免同样是“十秒视频”，实际做的工作完全不同。

**点评：** 这个结果证明了一种配置可以运行。是否值得迁移，要用自己的视频任务测总成本。

---

### 🧩 No.4 · 视频和图像质量也取决于前面的编码组件

**[Kandinsky Lab 发布稿](https://huggingface.co/blog/kandinskylab/kvae-3)**

KVAE-3.0 发布了面向图像、视频和立体声音频的组件。团队报告显示，图像组件的参数量明显下降，而在同套 COCO 重建测试中的分数与前代接近。这些结果针对组件及指定测试，不应直接外推为所有生成模型提速。

编码器将素材压缩成生成器能处理的表示。部署方应检查压缩后仍能保留哪些细节，特别是字幕小字、连续运动、左右声道关系等，再评估接入现有模型所需的适配工作。

**点评：** 多媒体生成成本不只由主模型决定；单独测编码组件，有时比直接换整套模型更有价值。

## 行业观察

本期最值得跟踪的是从演示走向部署的证据：算力要看端到端成本，平台要看办理结果，开源组件要看在自身数据上的可复测表现。热榜、合作名单和一次成功运行都可以帮人缩小选择，但不能代替验收。
