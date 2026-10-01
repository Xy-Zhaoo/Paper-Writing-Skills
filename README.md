# Paper Writing Skills

一套可独立安装的论文写作 Skill，用于撰写和修改英文论文的 Abstract 与 Introduction。

Three standalone skills for drafting and revising English paper Abstracts and Introductions.

每个目录都包含自己的 `SKILL.md`、`agents/openai.yaml` 和 `references/phrase-bank.md`。

Each package contains its own `SKILL.md`, `agents/openai.yaml`, and `references/phrase-bank.md`. No other skill or source-paper PDF is required at runtime.

## 选择 Skill / Choose a Skill

- **author1**：适合写量化、注意力和推理加速类论文。它会先说明系统哪里变慢、现有方法为什么不够，再把各个设计和实验结果对应起来，同时区分单个算子加速和整体运行速度。

  **For quantization, attention, and inference acceleration.** It explains where the system slows down, why existing methods fall short, how each design choice helps, and how local speedups translate to end-to-end performance.

- **author2**：适合写实用型方法论文。它会先说明一个看起来可行的方法为什么在更难的场景下失效，再找出背后的关键原因，并说明新方法怎样解决问题、实际部署需要付出什么代价。

  **For practical ML methods.** It shows why a promising approach breaks in harder cases, identifies the main reason, and connects the proposed fix to its real deployment requirements and trade-offs.

- **author3**：适合写视觉、图像恢复和新型图像问题。它会从真实使用场景和图像是如何受损讲起，再介绍数据如何获得、模型如何设计，以及每个模块具体解决什么问题。

  **For vision and image restoration papers.** It starts from the real capture or usage setting, explains how the image is degraded, and then connects the data, model components, and restoration results in plain terms.

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
