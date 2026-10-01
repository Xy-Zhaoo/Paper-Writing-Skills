# Paper Writing Skills

一套可独立安装的论文写作 Skill，用于撰写和修改英文论文的 Abstract 与 Introduction。

Three standalone skills for drafting and revising English paper Abstracts and Introductions.

每个目录都包含自己的 `SKILL.md`、`agents/openai.yaml` 和 `references/phrase-bank.md`，运行时不依赖其他 Skill，也不依赖论文 PDF。

Each package contains its own `SKILL.md`, `agents/openai.yaml`, and `references/phrase-bank.md`. No other skill or source-paper PDF is required at runtime.

## 选择 Skill / Choose a Skill

- **author1**：证据优先的系统论文论证。适合量化、注意力和推理加速，强调计算瓶颈、失败机制、组件收益，以及 kernel 与端到端结果的区分。

  **Evidence-first systems arguments.** Best for quantization, attention, and inference acceleration, with explicit bottlenecks, failure mechanisms, component-level gains, and separate kernel/end-to-end evidence.

- **author2**：从机制到部署的论证。适合说明一个有吸引力的方向为何在困难场景下失效，并将隐藏因素连接到设计决策和部署约束。

  **Mechanism-to-deployment arguments.** Best when an attractive practical direction fails in a hard regime because of an overlooked factor, and the method must state a clear deployment contract.

- **author3**：从真实场景到机制的恢复任务论证。适合视觉、图像恢复和新型退化问题，强调采集条件、物理机制、数据构建和组件映射。

  **Scene-to-mechanism restoration arguments.** Best for vision and restoration papers centered on real capture conditions, physical degradation, data construction, and component-to-challenge mapping.

三种 Skill 共享证据约束，但保留不同的论证路径。请选择与论文核心推理方式最匹配的目录。

The skills share evidence discipline while preserving different argument paths. Choose the package that matches the paper's central reasoning pattern.

## 安装与使用 / Install and Use

将一个作者目录复制到本地 skills 目录，并保持内部结构不变。例如：

Copy one author directory into your local skills directory and preserve its internal structure:

```text
<skills-directory>/author1/
  SKILL.md
  agents/openai.yaml
  references/phrase-bank.md
```

使用已安装 Skill 的配置名称，并提供研究笔记、草稿和有证据支持的实验事实。缺失证据应保持明确，不应由 Skill 猜测补全。

Use the installed skill by its configured name and provide research notes, a draft, and supported experimental facts. Missing evidence should remain explicit rather than being guessed.

## Phrase Bank / 句式库

每个 `references/phrase-bank.md` 按 rhetorical function 整理可填槽英文句式：Problem、Gap、Failure、Mechanism、Observation、Method Transition、Component Mapping、Practicalization、Evidence、Cost/Guarantee、Scope 和 Contribution。

Each `references/phrase-bank.md` organizes fill-slot English sentence structures by rhetorical function: Problem, Gap, Failure, Mechanism, Observation, Method Transition, Component Mapping, Practicalization, Evidence, Cost/Guarantee, Scope, and Contribution.

请用论文事实替换 slot，并根据上下文改写；句式库不是普通同义词表，也不是应原样粘贴的论文文本。

Replace the slots with paper-specific evidence and adapt the syntax to context. The phrase bank is neither a synonym list nor text to paste unchanged.

## 公开内容 / Public Contents

公开版本仅包含三个写作 Skill，不包含文章 PDF：

The public version contains only the three writing skills and no article PDFs:

- `papers/author1/`
- `papers/author2/`
- `papers/author3/`
