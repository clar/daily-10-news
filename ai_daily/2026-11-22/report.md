# AI 日报｜2026-11-22

*北京时间 11 月 22 日 05:00。周末版：先列过去 24 小时有可核实进展的消息，再补列未在上一期收录的 11 月 20 日背景。标为前情的条目不计为今日新讯。*

## 今日焦点

> **AI 辅助数学核验 · 研发能力评估 · 开放权重分化 · 企业智能体**
>
> - **经典黎曼猜想证明获 Lean 与 Mathlib 社区形式核验。** Levent Alpöge 称与 Claude 合作找到证明；社区声明确认经典版本，不能据此推及所有广义版本。
> - **METR 发布研发能力评估。** 在该机构合并任务集的时间跨度指标上，估计约每 3.6 个月翻倍；这个数字不代表真实研发产出或通用智能翻倍。
> - **开放权重覆盖不同部署场景。** 腾讯公布旗舰 Hy4 权重及自有许可，Thinking Machines Lab 发布可在部分本地设备运行的 Inkling 2 Mini。
> - **企业 AI 两端同时推进。** Oracle 称已筹齐履行 OpenAI 基础设施合同所需资金；财跃星辰发布面向金融岗位的智能体工作台 FinWork。

---

## 热点速览

| # | 新闻标题 | 来源 | 重要度 |
|---------|---------|------|--------|
| 1 | Lean 与 Mathlib 社区确认 Alpöge 的形式化工程证明了经典黎曼猜想；确认范围不包括所有广义版本 | [Lean 与 Mathlib 联合声明](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/) · [独立核验](https://math.mit.edu/~drew/grh/) | ⭐⭐⭐⭐⭐ |
| 2 | Transformers v5.24.0 新增 Inkling 2 Mini、Apertus 1.5 等模型支持，并统一缓存参数名 | [Hugging Face 发布说明](https://github.com/huggingface/transformers/releases/tag/v5.24.0) | ⭐⭐⭐⭐ |
| 3 | 财跃星辰披露 FinWork V1.0 发布细节，定位金融岗位办公智能体，内置 220 余项技能 | [科创板日报现场报道](https://api3.cls.cn/share/article/2540745?app=stib&os=android&selected=&source=&sv=815) | ⭐⭐⭐ |
| 4 | 美国财长称对较旧英伟达芯片无需再加限制；这是表态，不是商务部新规 | [美联社采访报道](https://apnews.com/article/88142455395552afe74caec3399a648b) | ⭐⭐⭐⭐ |
| 5 | METR 合并两套任务后估计模型可完成任务的时间跨度约每 3.6 个月翻倍（11 月 20 日前情） | [METR](https://metr.org/blog/2026-11-20-q4-2026-capability-update/) | ⭐⭐⭐⭐ |
| 6 | Oracle 称履行 OpenAI 合同所需融资已就位，仍按计划推进设备交付（11 月 20 日前情） | [Oracle 声明](https://www.oracle.com/news/announcement/oracle-statement-2026-11-20/) | ⭐⭐⭐⭐ |
| 7 | 腾讯公开旗舰多模态 Hy4、FP8 指令版及基础版权重，适用 Tencent Hy License（11 月 20 日前情） | [腾讯模型卡](https://huggingface.co/tencent/Hy4) | ⭐⭐⭐⭐ |
| 8 | Thinking Machines 发布开放权重 Inkling 2 Mini：264 亿总参数、接受图文输入（11 月 20 日前情） | [Thinking Machines Lab](https://thinkingmachines.ai/news/inkling-2-mini/) | ⭐⭐⭐⭐ |
| 9 | ChatGPT Space 开始面向年满 18 岁的 Plus 用户推出，外部共享需要登录与访问权限（11 月 20 日前情） | [OpenAI 产品更新](https://help.openai.com/en/articles/6825453-chatgpt-release-notes) | ⭐⭐⭐ |
| 10 | Baseten 发布基于 Gemma 4 的两款决策模型，支持图文输入和 128K 上下文（11 月 20 日前情） | [Baseten](https://www.baseten.co/blog/meet-bison-1-and-groundhog-1/) | ⭐⭐⭐ |
| 11 | Zscaler 公布与前沿模型供应商的合作，为企业提供 AI 安全防御能力（11 月 20 日前情） | [Zscaler 投资者关系](https://ir.zscaler.com/node/16796/pdf) | ⭐⭐⭐ |

---

## 深度点评

### 🏆 No.1 · 经典黎曼猜想：形式核验通过，证明范围仍要分清

**[Levent Alpöge 原稿](https://alpo.ge/remark.pdf) · [Andrew Sutherland 核验记录](https://math.mit.edu/~drew/grh/) · [Lean 与 Mathlib 联合声明](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/)**

Alpöge 在 11 月 20 日公布说明，称与 Claude 合作找到黎曼猜想的证明，且论证可扩展到狄利克雷 L 函数的广义版本。他公开了形式化材料。黎曼猜想的核心表述是黎曼 ζ 函数非平凡零点的实部均为二分之一，与素数分布密切相关。

MIT 数学家 Andrew Sutherland 的独立核验记录显示，约 **17.5 万个** Lean 模块成功编译；对五个主要定理的公理审计仅报告 Lean 的标准公理。其技术记录还将形式化命题与标准表述作了核对。Lean 与 Mathlib 社区的联合声明进一步确认，独立工具比对了所证命题与 Mathlib 对经典黎曼猜想的定义，并对导出的证明做了交叉检查。该声明核验的是经典版本，不能据此把所有广义版本写成已确认，也不能把合作成果说成 Claude 独立解题。

接下来的另一项工作是把关键数学思路解释给人读。经典版本的形式化结论已经有可重复检查的公开证据，不必把形式化核验和后续论文解读混为一谈。

**点评：** 这条新闻最重要的不是「Claude 说证明了」，而是其他人已有材料可以核验。

---

### 🧪 No.2 · METR 的 3.6 个月翻倍，量的是任务跨度而不是生产力

**[METR 评估报告](https://metr.org/blog/2026-11-20-q4-2026-capability-update/)**

METR 将两套任务合并后估计，所测模型的时间跨度指标约每 **3.6 个月**翻倍。该指标用人类完成任务所需的时间描述难度，再估计模型达到特定成功概率时能处理多长的任务；它不是模型实际运行时间，也不是模型版本更新的周期。

新任务集相对更难。同一个模型在合并任务集上的 50% 成功时间跨度比只用旧集更低，说明选什么任务会改变绝对读数。报告也明确指出，研究人员仍不确定哪些能力是加快真实 AI 研发的必要条件，模型评分与专家判断在一些开放任务上还可能不同。

比外推一条指数曲线更有用的是，把结果和现实任务的复核成本放在一起：模型能不能找到有价值的问题、验证结果能不能推广、研究员要花多少时间返工。能做更长的任务是信号，但不是这些问题的替代答案。

**点评：** 任务跨度翻倍，不能直接推出团队研发产出翻倍。

---

### 🚀 No.3 · Hy4 与 Inkling 2 Mini：开放权重相同，部署选择不同

**[腾讯 Hy4 模型卡](https://huggingface.co/tencent/Hy4) · [Inkling 2 Mini 发布说明](https://thinkingmachines.ai/news/inkling-2-mini/) · [Inkling 2 Mini 模型卡](https://huggingface.co/thinkingmachines/Inkling-2-Mini)**

腾讯公开 Hy4 旗舰的指令版、FP8 版和预训练基础版，采用 **Tencent Hy License**。Thinking Machines Lab 的 Inkling 2 Mini 则提供 **264 亿参数**的开放权重模型，在生成每个 token 时重复计算中间层；模型卡注明 **Apache 2.0** 许可。

两款模型都公开权重，但不能由此推断它们有相同的使用条款或硬件门槛。旗舰权重面向较重的部署环境；Inkling 2 Mini 将部分能力放进更小的模型中，定位包括本地运行。发布方给出了一些编码成绩，但也指出 Mini 在多轮对话、复杂约束和部分重推理测试上并不领先。

团队选型时应先核对许可，再测实际设备、任务长度、输出速度和验收通过率。笔记本能启动模型，不代表可以用同样的速度处理很长的上下文。

**点评：** 权重能下载只是第一关；许可合适、设备跑得动、结果能验收才是部署。

---

### 💼 No.4 · Oracle 称融资到位，算力交付仍需分阶段验证

**[Oracle 11 月 20 日声明](https://www.oracle.com/news/announcement/oracle-statement-2026-11-20/)**

Oracle 表示已筹得履行 OpenAI 合同所需资金，包括该公司此前介绍的供应商融资，并称后续与供应商接触不构成履约前提。Oracle 同时表示，Abilene 园区接近完工，下一座大型园区 Shackelford 已获所需许可，部分 Vera Rubin 机柜计划在未来几周交接。

融资到位和合同交付是不同阶段。即使资金已落实，机柜到货、并网和验收仍决定客户收到算力的时间。上述里程碑是 Oracle 的公开陈述，并不是对合同全额履行或未来现金流的独立确认。

值得继续跟踪机柜交接之后的服务上线、客户验收以及现金流披露。把公司给出的计划与后续公告逐项对照，比把「融资到位」视为「收入确定」更稳妥。

**点评：** 有钱履约是一项进展；按时交付可计费算力，才是下一项。

## 行业观察

今天容易混淆的四件事是：**证明通过技术核验与完成数学审查、基准趋势与生产力、公开权重与实际部署、融资落定与算力交付**。它们各自都值得关注，但要判断影响，应该追踪下一步能不能被不同的人用同一套材料独立验证。
