# AI 日报 · 2026-11-27

> 截至北京时间 11 月 27 日 05:00（11 月 26 日 21:00 UTC）。区分新模型、已有模型新增资源、厂商测试与政策议程。

## 今日焦点

> **智能体中断恢复 · 文档识别的新数据 · 本地推理实测 · 硬件可验证性**
>
> - **Qwen Code 更新托管会话。** 等待审批或后台工作时可以挂起，运行框架崩溃后支持恢复。
> - **BharatGen 发布 Patram 1.5，英伟达补充文档模型资源。** 前者面向印度文档，后者开放既有 Nemotron Parse 的训练与推理资源。
> - **ggml-org 上线 AMD 本地推理公开测试面板。** 把读入提示词和生成文字分别计速，首批只覆盖指定设备。
> - **Vitalik 讨论芯片可验证性。** 公开逻辑设计和可以检验实际制造出的硬件，是两个层次。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---|---------|------|--------|
| 1 | **Qwen Code v0.28.6 发布**：11 月 26 日 05:51 UTC（GitHub 发布时间）；托管会话可在等待批准、答复或后台工作时挂起，并支持运行框架崩溃后从已保存状态恢复。 | [Qwen Code 发布说明](https://github.com/QwenLM/qwen-code/releases/tag/v0.28.6) | ⭐⭐⭐⭐ |
| 2 | **BharatGen 推出 Patram 1.5-7B**：开放权重的文档理解模型新增 OCR 3.0 和在证据不足时拒答的能力；首发权重可从 Hugging Face 获取。 | [BharatGen 发布稿](https://bharatgen.com/blogs/introducing-patram-1-5/)、[模型卡](https://huggingface.co/bharatgenai/Patram1.5-7B) | ⭐⭐⭐⭐ |
| 3 | **ggml-org 发布 llama.cpp × AMD 性能面板**：公开本地提示词处理和生成吞吐，起步覆盖 Radeon 8060S、Radeon AI Pro R9700S，并提供原始数据。 | [项目维护方公告](https://huggingface.co/blog/ggml-org/llamacpp-amd-bench) | ⭐⭐⭐ |
| 4 | **英伟达为 Nemotron 3.5 Parse 补充数据与工具**：包括合成训练数据、微调方案和加速推理资源；这是既有文档解析模型的配套更新。 | [英伟达发布稿](https://huggingface.co/blog/nvidia/building-on-nemotron-35-parse-open-data-fine-tunin) | ⭐⭐⭐ |
| 5 | **AWS DevOps Agent 加入 Fast agent**：与完整调查并行，先显示初步根因，供运维人员参考；不是已经确认的最终结论。 | [AWS 更新日志](https://docs.aws.amazon.com/devopsagent/latest/userguide/whats-new.html) | ⭐⭐⭐ |
| 6 | **阿联酋 EGF 签署对 XEBO.ai 的 1,050 万美元投资协议**：作为 A 轮的一部分，支持其 AI 客户体验管理业务；该数额是 EGF 承诺投资额。 | [Emirates Growth Fund](https://www.egf.gov.ae/en/news/emirates-growth-fund-invests-%2410.5-million-in-uae-built-ai-company-xebo.ai) | ⭐⭐⭐ |
| 7 | **蚂蚁 inclusionAI 公开 Ming-Image-0.2-Design 权重**：模型卡列为 6B 级视觉设计模型，面向复杂版式和文字渲染；实际文字准确率仍应使用自己的素材验证。 | [inclusionAI 模型卡](https://huggingface.co/inclusionAI/Ming-Image-0.2-Design) | ⭐⭐⭐ |
| 8 | **联合国独立国际 AI 科学小组巴巴多斯会议进入最后一天**：官方时间表列为 11 月 23 至 26 日第二次线下会议；未把会议日程写成已通过新规则。 | [联合国官方时间表](https://www.un.org/independent-international-scientific-panel-ai/en/timeline) | ⭐⭐⭐ |
| 9 | **Vitalik 发文区分芯片开放设计与实物验证**：文章讨论逻辑描述、物理版图与制造信任；是作者对硬件供应链的观察，不是行业标准或芯片发布。 | [Vitalik 原文](https://vitalik.eth.limo/general/2026/11/26/a_shallow_dive_into_open-source_chip_design.html) | ⭐⭐⭐ |
| 10 | **Blue Cloud 在孟买市长论坛披露面向城市服务的 AI 展示**：涉及政府服务和健康场景；公司介绍的是展示内容，未披露新增采购或规模化部署结果。 | [公司公告（PDF）](https://bluecloudsoftech.com/wp-content/uploads/2026/11/Final-press-release20261126.pdf) | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · Qwen Code 恢复任务后，仍需核对授权

**[Qwen Code 发布说明](https://github.com/QwenLM/qwen-code/releases/tag/v0.28.6)**

托管会话可以等人，而不必一直占着运行资源；运行框架崩溃后，也可以从保存的状态恢复。改动主要在任务执行生命周期，不是模型突然更擅长写代码。

恢复后最需要谨慎的是时间差。等待期间仓库可能变化，批准也可能只针对当时看到的内容。团队应验证恢复时能否识别状态变化，以及重试是否会重复执行已完成的动作。

**点评：** 长任务不仅要接得上，还要知道哪些旧决定已经不能直接沿用。

---

### 📄 No.2 · 文档模型的新竞争点是不确定时会停下

**[BharatGen Patram 1.5](https://bharatgen.com/blogs/introducing-patram-1-5/)** · **[英伟达 Nemotron Parse 配套更新](https://huggingface.co/blog/nvidia/building-on-nemotron-35-parse-open-data-fine-tunin)**

Patram 1.5 将印度文档识别和证据不足时拒答放在一起。英伟达则围绕已有的解析模型提供更多训练和推理资源，方便用户针对自己的材料做适配。

对表单和合同处理而言，错误字段被直接写入下游系统的成本，可能远高于把一页交给人复查。应同时衡量字段正确率、误拒率和无法回答时的处理成本，并按扫描质量、语言和表格结构拆开看。

**点评：** 比起多读出几个字，能判断哪些字段不该自动落库，有时更值得付费。

---

### 📊 No.3 · AMD 面板让本地模型选型有了可检查的基线

**[ggml-org 基准公告](https://huggingface.co/blog/ggml-org/llamacpp-amd-bench)**

公开数据能让开发者区分输入阶段的消化速度和输出阶段的生成吞吐，也便于追踪不同构建版本的性能回归。这比只公布某个峰值更实用。

但硬件范围有限，短时测量也不涵盖长对话的峰值内存、缓存压力或整机持续功耗。购买设备前，仍应核对自己的模型、上下文长度与典型并发。

**点评：** 用看板筛硬件，再用真实负载做决定；把两者混在一起，容易选到跑分更高却更慢的机器。

---

### 🔍 No.4 · 板上印着同一个型号，不代表硬件可以独立核验

**[Vitalik 原文](https://vitalik.eth.limo/general/2026/11/26/a_shallow_dive_into_open-source_chip_design.html)**

文章有用的地方在于拆开两件事：一是能不能检查设计的逻辑和物理版图，二是拿到实物后有没有可靠的手段核验它与公开设计相符。公开前者有帮助，但不会自动解决制造与交付的信任。

这对加密硬件、边缘 AI 设备和数据中心采购都有参考价值。各场景的验证成本差别很大；文章提出的是评估框架，不是断言当前某款芯片存在问题。

**点评：** 采购时与其只问“开不开源”，不如问供应商能公开到哪一层、能用什么证据把设计和交付实物连起来。

## 行业观察

从会话恢复到文档拒答，再到公开性能数据，今天的更新主要改善了模型出错或信息不全时的处理方式。这些改动很少出现在排行榜最显眼的位置，却直接决定了团队能否将 AI 放进长期运行的流程。
