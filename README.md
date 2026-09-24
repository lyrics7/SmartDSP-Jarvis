<div align="center">

# SmartDSP · Jarvis Research Collection

### Multimodal Agents · Creative AI · Intelligent Image Editing · Image Restoration

A curated collection of **datasets, benchmarks, research publications, and open-source projects** from **SmartDSP Lab**, covering intelligent image restoration, professional photo retouching, self-evolving image-editing agents, human-AI creative collaboration, and long-horizon multimodal creative systems.

<br>

**Datasets · Benchmarks · Publications · Open-Source Projects · Interactive Demos**

</div>

---

## Overview

The **SmartDSP Jarvis Research Collection** brings together a series of research efforts exploring the evolution of intelligent visual systems — from specialized image restoration and professional photo editing toward increasingly autonomous, adaptive, and collaborative multimodal agents.
<div align="center">

<table>
  <tr>
    <th>Project</th>
    <th>Before</th>
    <th>After</th>
  </tr>

  <tr>
    <td align="center">
      <a href="#jarvisart"><b>JarvisArt</b></a><br>
      <sub>Photo Retouching</sub>
    </td>
    <td align="center">
      <img src="https://jarvisart.vercel.app/assets/results/0/original.jpg"
           height="150" alt="JarvisArt input">
    </td>
    <td align="center">
      <img src="https://jarvisart.vercel.app/assets/results/0/processed.jpg"
           height="150" alt="JarvisArt output">
    </td>
  </tr>

  <tr>
    <td align="center">
      <a href="#jarvisevo"><b>JarvisEvo</b></a><br>
      <sub>Photo Editing</sub>
    </td>
    <td align="center">
      <img src="https://jarvisevo.vercel.app/api/image-proxy?path=LRC%2Fcn%2Fffe90c74-4c54-4f8f-8f9e-61851d6c3cb2%2Fbefore.jpg"
           height="150" alt="JarvisEvo input">
    </td>
    <td align="center">
      <img src="https://jarvisevo.vercel.app/api/image-proxy?path=LRC%2Fcn%2Fffe90c74-4c54-4f8f-8f9e-61851d6c3cb2%2FMR_image%2Fround_1_processed_before.jpg"
           height="150" alt="JarvisEvo output">
    </td>
  </tr>

  <tr>
    <td align="center">
      <a href="#jarvisir"><b>JarvisIR</b></a><br>
      <sub>Image Restoration</sub>
    </td>
    <td align="center">
      <img src="https://cvpr2025-jarvisir.github.io/results/before/img8.png"
           height="150" alt="JarvisIR degraded input">
    </td>
    <td align="center">
      <img src="https://cvpr2025-jarvisir.github.io/results/after/img8.png"
           height="150" alt="JarvisIR restored output">
    </td>
  </tr>
</table>

<sub>Selected input–output examples from the official project websites.</sub>

</div>
The collection is organized into three major components:

- **Datasets & Benchmarks** — Public resources supporting the training, development, and evaluation of intelligent visual agents, including **CleanBench** for instruction-following image restoration, **MMArt-PPR10K** for agentic professional photo retouching, **MMArt-Bench** for multiscenario and region-level retouching evaluation, and **ArtEdit-Bench** for fine-grained editing and self-evaluation assessment.

- **Research Publications** — Research on **VLM-powered intelligent image restoration**, **MLLM-driven professional photo retouching**, and **self-evolving image-editing agents**, represented by **JarvisIR**, **JarvisArt**, and **JarvisEvo**.

- **Open-Source Agent Projects** — Creative-agent systems that extend beyond individual visual tasks toward longer and more general creative workflows, including **JarvisX-Cowork**, an end-to-end personal creative-agent harness, and **JarvisHub**, an open canvas-native multimodal creative-agent harness.

Together, these works form a progressive research trajectory:

<div align="center">

**Intelligent Image Restoration → Professional Photo Retouching → Self-Evolving Image Editing → End-to-End Creative Coworking → Canvas-Native Multimodal Agents**

**JarvisIR → JarvisArt → JarvisEvo → JarvisX-Cowork → JarvisHub**

</div>

This trajectory reflects a broader transition from **task-specific visual intelligence** toward **general-purpose creative agents**. Early systems focus on understanding visual degradation and coordinating specialized restoration models; subsequent work extends agentic reasoning to professional photo-retouching tools, introduces self-evaluation and self-improvement, and ultimately expands toward persistent creative assistants and canvas-native environments for long-horizon multimodal creation.

Across these projects, the central goal is to explore how AI systems can move beyond isolated restoration, editing, or generation tasks and become **persistent, tool-using, adaptive, human-steerable collaborators** capable of reasoning over visual content, interacting with professional tools, maintaining project context, evaluating intermediate results, and supporting complex creative workflows.

---

## Table of Contents

- [1. Datasets & Benchmarks](#1-datasets--benchmarks)
  - [Dataset Summary](#dataset-summary)
  - [MMArt-PPR10K](#mmart-ppr10k)
  - [MMArt-Bench](#mmart-bench)
  - [ArtEdit-Bench](#artedit-bench)
  - [CleanBench](#cleanbench)

- [2. Publications from SmartDSP Lab](#2-publications-from-smartdsp-lab)
  - [Publication Summary](#publication-summary)
  - [JarvisHub](#jarvishub)
  - [JarvisEvo](#jarvisevo)
  - [JarvisX-Cowork](#jarvisx-cowork)
  - [JarvisArt](#jarvisart)
  - [JarvisIR](#jarvisir)

---

# 1. Datasets & Benchmarks

This section summarizes the public datasets and evaluation benchmarks associated with the Jarvis series. These resources cover **instruction-driven professional photo retouching**, **preservative image editing**, and **adverse-condition image restoration**.

<a id="dataset-summary"></a>

## Dataset Summary

| Dataset | Related Project | Type | Scale / Content | Main Purpose | Links |
|---|---|---|---|---|---|
| **MMArt-PPR10K** | JarvisArt | Multimodal paired image-retouching dataset | PPR10K-based paired images, multi-granularity user instructions, and Lua/XMP-based Lightroom editing configurations | Research on instruction-driven agentic image retouching | [Dataset](https://huggingface.co/datasets/JarvisArt/MMArt-PPR10k) / [Paper](https://arxiv.org/abs/2506.17612) |
| **MMArt-Bench** | JarvisArt | Multiscenario photo-retouching evaluation benchmark | 200 instances across 4 major scenarios + 50-image portrait subset with mask annotations | Comprehensive image-level and region-level evaluation of agentic photo-retouching systems | [Dataset](https://huggingface.co/datasets/JarvisArt/MMArt-Bench) / [Paper](https://arxiv.org/abs/2506.17612) |
| **ArtEdit-Bench** | JarvisEvo | Image-editing evaluation benchmark | ArtEdit-Bench-Lr: 800 bilingual samples; ArtEdit-Bench-Eval: 200 English samples | Evaluating fine-grained retouching and model self-evaluation capabilities | [Dataset](https://huggingface.co/datasets/JarvisEvo/ArtEdit-Bench) / [Paper](https://arxiv.org/abs/2511.23002) |
| **CleanBench** | JarvisIR | Synthetic + real-world instruction-following image-restoration dataset | 150K synthetic + 80K real instruction-response pairs | Training and evaluating intelligent restoration systems under real-world adverse conditions | [Dataset](https://huggingface.co/datasets/LYL1015/CleanBench) / [Project](https://cvpr2025-jarvisir.github.io/) / [Paper](https://lyl1015.github.io/papers/CVPR2025_JarvisIR.pdf) |

---

<a id="mmart-ppr10k"></a>

## MMArt-PPR10K

**Related Project:** JarvisArt  
**Paper:** *JarvisArt: Liberating Human Artistic Creativity via an Intelligent Photo Retouching Agent*  
**Task:** Instruction-driven professional photo retouching  
**Type:** Multimodal paired image-retouching dataset  
**Source:** Built upon the PPR10K dataset  
**Content:** Paired original and retouched images, multi-granularity user instructions, and Lua/XMP-based Lightroom editing configurations  

### English Introduction

**MMArt-PPR10K**  is a multimodal dataset developed for research on instruction-driven agentic image retouching. Built upon the original PPR10K dataset, it combines paired original and retouched images with natural-language editing instructions and structured information associated with Lightroom editing operations.

Unlike conventional image-to-image datasets that primarily provide input and target images, MMArt-PPR10K additionally incorporates user instructions at different levels of detail together with Lua/XMP-based editing configurations. These components provide information about both the desired editing outcome and the corresponding professional editing process.

This multimodal structure makes MMArt-PPR10K particularly suitable for research on instruction understanding, multimodal reasoning, professional editing-tool use, and agentic photo-retouching workflows.

### 中文简介

**MMArt-PPR10K** 是 JarvisArt 项目面向**指令驱动 Agentic 图像修饰任务**构建的多模态数据集，并基于原始 PPR10K 数据集进行扩展。

与主要提供输入图像和目标图像的传统图像到图像数据集不同，MMArt-PPR10K 除了包含修图前后的成对图像之外，还提供不同详细程度的自然语言用户编辑指令，以及与 Lightroom 编辑操作相关的 Lua/XMP 配置信息。

这些信息能够同时描述用户期望的编辑效果以及与之对应的专业编辑过程。因此，该数据集适合用于研究编辑指令理解、多模态推理、专业修图工具使用以及 Agent 驱动的照片修饰流程。

### Dataset Structure

Each sample is organized in a unique directory containing paired images, user instructions of varying lengths, and Lightroom-related configuration files.

- `before.jpg` — original unedited image
- `processed.jpg` — retouched image
- `user_want_short` — short user instruction
- `user_want_middle` — medium-length user instruction
- `user_want_long` — detailed user instruction
- `config.lua` — Lua configuration used in Lightroom
- `config.xmp` — XMP metadata and editing preset associated with Lightroom

### Links

[**Dataset**](https://huggingface.co/datasets/JarvisArt/MMArt-PPR10k) ·
[**Paper**](https://arxiv.org/abs/2506.17612) ·
[**Project Page**](https://jarvisart.vercel.app/) ·
[**Code**](https://github.com/LYL1015/JarvisArt)

---

<a id="mmart-bench"></a>

## MMArt-Bench

**Related Project:** JarvisArt  
**Paper:** *JarvisArt: Liberating Human Artistic Creativity via an Intelligent Photo Retouching Agent*  
**Task:** Agentic photo-retouching evaluation 
**Type:** Multiscenario photo-retouching evaluation benchmark
**Source:** Sampled from the MMArt dataset
**Scale:** 200 benchmark instances across four major scenarios
**Scenarios:** Portrait · Landscape · Street Scenes · Still Life
**Region-Level Evaluation:** 50 human-centered portrait images with mask annotations

### English Introduction

**MMArt-Bench** is an evaluation benchmark introduced with JarvisArt to provide a comprehensive assessment of agentic photo-retouching performance. It is sampled from the broader MMArt dataset and covers diverse real-world photographic scenarios.

The benchmark contains four major categories — **portrait, landscape, street scenes, and still life** — with 50 instances in each category, resulting in **200 benchmark instances** in total. Each primary category is further divided into multiple subcategories to cover a broader range of photographic content.

In addition to image-level evaluation, MMArt-Bench supports **region-level evaluation** through a dedicated portrait subset containing **50 human-centered images with mask annotations**. This enables more fine-grained assessment of localized photo-retouching performance.

MMArt-Bench serves as the evaluation component of the MMArt ecosystem, complementing datasets such as MMArt-PPR10K by providing a standardized benchmark for assessing agentic photo-retouching systems across diverse scenarios and evaluation granularities.

### 中文简介

**MMArt-Bench** 是 JarvisArt 项目提出的**照片修饰评测基准**，用于对 Agentic 照片修饰系统的性能进行综合评估。该 Benchmark 从更大的**MMArt 数据集**中采样构建，并覆盖多种真实摄影场景。

MMArt-Bench 包含 **人像、风景、街景和静物**四类主要场景，每类包含 50 个评测实例，共计 **200 个 Benchmark Instances**。每个主要类别还进一步划分为多个子类别，以覆盖更加丰富的摄影内容。

除整体图像层面的评测之外，MMArt-Bench 还提供用于**区域级评测**的人像子集。该子集包含 **50 张以人物为中心的图像及对应的 Mask 标注**，可用于更加细粒度地评估局部区域的照片修饰效果。

MMArt-Bench 可以视为 MMArt 数据体系中的评测组成部分，与 MMArt-PPR10K 等数据集形成互补，为不同场景和不同评测粒度下的 Agentic 照片修饰系统提供标准化评估数据。

### Links

[**Dataset**](https://huggingface.co/datasets/JarvisArt/MMArt-Bench) ·
[**Paper**](https://arxiv.org/abs/2506.17612) ·
[**Project Page**](https://jarvisart.vercel.app/) ·
[**Code**](https://github.com/LYL1015/JarvisArt)

---

<a id="artedit-bench"></a>

## ArtEdit-Bench

**Related Project:** JarvisEvo  
**Paper:** *JarvisEvo: Towards a Self-Evolving Photo Editing Agent with Synergistic Editor-Evaluator Optimization*  
**Task:** Photo-retouching and self-evaluation assessment  
**Type:** Image-editing evaluation benchmark  
**Scale:** 1,000 benchmark samples across two subsets  
**Subsets:** ArtEdit-Bench-Lr · ArtEdit-Bench-Eval  
**Evaluation Focus:** Global and local fine-grained retouching · Model self-evaluation

### English Introduction

**ArtEdit-Bench** is an image-editing evaluation benchmark introduced with JarvisEvo for assessing both photo-retouching and model self-evaluation capabilities. It consists of two complementary subsets: **ArtEdit-Bench-Lr** and **ArtEdit-Bench-Eval**.

**ArtEdit-Bench-Lr** contains **800 samples**, including 400 English and 400 Chinese samples selected from the ArtEdit-Lr dataset. It is designed to evaluate both **global and local fine-grained retouching capabilities**, providing a benchmark for assessing how effectively image-editing systems perform detailed photo-retouching tasks across different editing granularities.

**ArtEdit-Bench-Eval** contains **200 English samples** sampled from the ArtEdit-Eval dataset. This subset is designed to assess a model's **self-evaluation capabilities** and enables comparison with dedicated assessment models.

Together, the two subsets allow ArtEdit-Bench to evaluate not only the editing performance of intelligent photo-editing systems but also their ability to assess editing results. This makes the benchmark particularly relevant to JarvisEvo's unified editor-evaluator framework, in which editing and evaluation capabilities are jointly developed.

### 中文简介

**ArtEdit-Bench** 是 JarvisEvo 项目提出的**图像编辑评测基准**，主要用于评估智能照片编辑系统的修图能力以及模型自身的评价能力。该 Benchmark 由两个相互补充的子集组成：**ArtEdit-Bench-Lr** 和 **ArtEdit-Bench-Eval**。

**ArtEdit-Bench-Lr** 包含 **800 个样本**，其中包括 400 个英文样本和 400 个中文样本，这些数据从 ArtEdit-Lr 数据集中选取得到。该子集主要用于评估模型的**全局和局部细粒度照片修饰能力（Global and Local Fine-Grained Retouching）**，从而衡量图像编辑系统在不同编辑粒度下完成专业修图任务的能力。

**ArtEdit-Bench-Eval** 包含从 ArtEdit-Eval 数据集中采样得到的 **200 个英文样本**，主要用于评估模型的**自我评价能力（Self-Evaluation Capability）**，并与其他专门的评估模型进行公平比较。

因此，ArtEdit-Bench 不仅关注智能图像编辑系统“如何完成编辑任务”，还进一步关注模型“如何评价编辑结果”。这种双重评测设计与 JarvisEvo 的统一 Editor-Evaluator 框架相对应，使其能够同时衡量模型的照片编辑能力和自我评价能力。

### Links

[**Dataset**](https://huggingface.co/datasets/JarvisEvo/ArtEdit-Bench) ·
[**Paper**](https://arxiv.org/abs/2511.23002) ·
[**Project Page**](https://jarvisevo.vercel.app/) ·
[**Code**](https://github.com/LYL1015/JarvisEvo)

---

<a id="cleanbench"></a>

## CleanBench

**Related Project:** JarvisIR  
**Paper:** *JarvisIR: Elevating Autonomous Driving Perception with Intelligent Image Restoration*  
**Venue:** CVPR 2025  
**Task:** Intelligent image restoration for robust autonomous-driving perception  
**Type:** Synthetic + real-world instruction-following image-restoration dataset  
**Scale:** 150K synthetic + 80K real instruction-response pairs  
**Coverage:** Diverse adverse-weather and coupled image degradations  
**Purpose:** Training and evaluation of intelligent image-restoration systems

### English Introduction

**CleanBench** is a large-scale instruction-following image-restoration dataset introduced with JarvisIR to support the training and evaluation of intelligent restoration systems under challenging real-world conditions.

The complete CleanBench dataset consists of approximately **150K synthetic and 80K real instruction-response pairs**. The synthetic component provides controlled degraded data for supervised learning, while the real-world component is designed to improve robustness and generalization under complex adverse-weather conditions.

Rather than focusing only on a single predefined restoration task, CleanBench supports intelligent restoration systems that must understand image degradation conditions and determine appropriate restoration strategies. Its construction incorporates degraded images together with assessment reasoning, restoration task sequences, and corresponding instruction-response data.

CleanBench plays an important role in JarvisIR's two-stage training framework. Synthetic CleanBench data is used for supervised fine-tuning to develop instruction-following and degradation-recognition capabilities, while CleanBench-Real supports human-feedback alignment for improving robustness, reducing hallucinations, and enhancing generalization to real-world adverse weather.

By supporting both intelligent restoration decision-making and downstream perception-oriented evaluation, CleanBench helps connect **low-level image restoration** with **robust high-level perception in autonomous-driving environments**.

### 中文简介

**CleanBench** 是 JarvisIR 项目提出的大规模**指令跟随图像恢复数据集（Instruction-Following Image-Restoration Dataset）**，主要用于支持智能图像恢复系统在复杂真实环境下的训练与评估。

完整的 CleanBench 包含约 **15 万组合成数据和 8 万组真实数据对应的 Instruction-Response Pairs**。其中，合成数据主要提供可控的图像退化样本，用于监督学习；真实数据则面向更加复杂的真实恶劣天气环境，以提升系统的鲁棒性和泛化能力。

与仅针对某一种预定义退化类型执行固定恢复操作的数据集不同，CleanBench 面向更加智能化的 Restoration System：模型不仅需要处理退化图像，还需要理解当前图像的退化情况，并据此确定合适的恢复策略。其数据构建过程结合了退化图像、退化评估推理、最优恢复任务序列以及相应的 Instruction-Response 数据。

CleanBench 同时服务于 JarvisIR 的两阶段训练框架。Synthetic 数据用于监督微调，使模型学习指令跟随和图像退化识别能力；CleanBench-Real 则用于 Human Feedback Alignment，以进一步提升系统在真实恶劣天气条件下的鲁棒性、降低幻觉并增强泛化能力。

因此，CleanBench 不仅服务于低层图像恢复任务，还进一步支持面向自动驾驶视觉系统的感知性能研究，在**低层图像恢复** 与 **高层自动驾驶视觉感知**之间建立联系。


### Links

[**Dataset**](https://huggingface.co/datasets/LYL1015/CleanBench) ·
[**Project Page**](https://cvpr2025-jarvisir.github.io/) ·
[**Paper**](https://lyl1015.github.io/papers/CVPR2025_JarvisIR.pdf) ·
[**Code**](https://github.com/LYL1015/JarvisIR)

---

<a id="dataset-availability-for-other-jarvis-projects"></a>


# 2. Publications from SmartDSP Lab

This section summarizes the featured Jarvis research projects and publications from **SmartDSP Lab**, tracing the progression from intelligent image restoration to professional photo editing, self-evolving agents, end-to-end creative assistants, and canvas-native multimodal systems.

<a id="publication-summary"></a>

## Publication Summary

| Year | Project | Research / Method Type | Authors | Venue / Status | Links |
|---|---|---|---|---|---|
| 2026 | **JarvisHub: An Open Harness for Canvas-Native Multimodal Creative Agents** |Canvas-native multimodal creative-agent harness | Yunlong Lin et al. | Preprint / arXiv 2026 | [Project](https://www.jarvishub.site/) / [Paper](https://arxiv.org/abs/2607.23588) / [Code](https://github.com/LYL1015/JarvisHub) / [HF](https://huggingface.co/papers/2607.23588) |
| 2026 | **JarvisEvo: Towards a Self-Evolving Photo Editing Agent with Synergistic Editor-Evaluator Optimization** | Self-evolving photo-editing agent | Yunlong Lin et al. | CVPR 2026 | [Project](https://jarvisevo.vercel.app/) / [Paper](https://arxiv.org/abs/2511.23002) / [Code](https://github.com/LYL1015/JarvisEvo) / [HF](https://huggingface.co/papers/2511.23002) |
| 2026 | **JarvisX-Cowork** | End-to-end creative-agent harness | — | Open-Source Project | [Code](https://github.com/LYL1015/JarvisX-Cowork) / [Demo](https://youtu.be/SiNsTmGbWlo) |
| 2025 | **JarvisArt: Liberating Human Artistic Creativity via an Intelligent Photo Retouching Agent** | MLLM-driven professional photo-retouching agent | Yunlong Lin et al. | NeurIPS 2025 | [Project](https://jarvisart.vercel.app/) / [Paper](https://arxiv.org/abs/2506.17612) / [Code](https://github.com/LYL1015/JarvisArt) / [HF](https://huggingface.co/papers/2506.17612) |
| 2025 | **JarvisIR: Elevating Autonomous Driving Perception with Intelligent Image Restoration** | VLM-powered intelligent image-restoration agent | Yunlong Lin et al. | CVPR 2025 | [Project](https://cvpr2025-jarvisir.github.io/) / [Paper](https://lyl1015.github.io/papers/CVPR2025_JarvisIR.pdf) / [Code](https://github.com/LYL1015/JarvisIR) / [Demo](https://huggingface.co/spaces/LYL1015/JarvisIR) |

---

<a id="jarvishub"></a>

## JarvisHub

### An Open Harness for Canvas-Native Multimodal Creative Agents

<table>
<tr>
<td width="31%" align="center">

<img src="jarvishub.png" width="100%" alt="JarvisHub">

</td>

<td width="69%">

**Year:** 2026  
**Venue / Status:** arXiv Preprint  
**arXiv Category:** Computer Vision and Pattern Recognition (cs.CV)  
**Submitted:** July 26, 2026  
**Method Type:** Canvas-native multimodal creative-agent harness  
**Task:** Long-horizon multimodal creative production  

**Authors:**  
Yunlong Lin, Zixu Lin, Zhaohu Xing, Biqiang Li, Chenxin Li, Haonan Wang, Haitao Wu, Hengyu Liu, Jianghai Chen, Kaituo Feng, Kaixin Li, Shawn Chen, Shijue Huang, Sixiang Chen, Tsung-Yi Ho, Wenxuan Huang, Xiangyan Liu, Xiaomeng Hu, Xuanhua He, Yan Sun, Yunqing Zhao, Zhiqin Yang, Zehan Wang, Zhengyang Tang, Tianyu Pang, Xiangyu Yue

**Links:**  
[Project](https://www.jarvishub.site/) /
[Paper](https://arxiv.org/abs/2607.23588) /
[Code](https://github.com/LYL1015/JarvisHub) /
[Hugging Face](https://huggingface.co/papers/2607.23588)

### Highlights

- Introduces an open **canvas-native creative-agent harness** for long-horizon multimodal creation.
- Treats the editable canvas simultaneously as the **user workspace, agent external memory, action space, and shared project state**.
- Represents multimodal artifacts, dependencies, versions, status, and feedback through structured canvas nodes and links.
- Employs a three-layer architecture consisting of **Canvas State, Protocol Bridge, and Agent Runtime**.
- Enables agents to progressively **plan, generate, revise, and organize** multimodal projects over extended creative workflows.
- Preserves **human steerability** by allowing users to inspect, guide, modify, and intervene throughout the creative process.
- Functions as an **agent orchestration harness rather than a standalone generative model**, integrating external models and tools within a persistent and inspectable creative workspace.

</td>
</tr>
</table>

### English Introduction

**JarvisHub** is an open harness for **canvas-native multimodal creative agents**, designed to support long-horizon multimodal creative production.

Modern generative models can produce high-quality images, videos, audio clips, webpages, UI elements, presentations, and other creative assets. However, real-world creative work rarely consists of isolated prompt-output interactions. Instead, a complete project evolves through references, drafts, alternatives, edits, failed attempts, version relationships, tool actions, evaluation signals, and human feedback, which together form an evolving project state.

JarvisHub addresses this challenge by placing an editable visual **Canvas** at the center of the agent workflow. Rather than serving merely as a user interface, the Canvas simultaneously functions as the **user workspace, the agent's external memory, its action space, and a persistent shared project state**.

Multimodal artifacts and their relationships are represented through typed canvas nodes and links, allowing references, dependencies, versions, status, and feedback to remain explicitly represented throughout extended creative workflows.

JarvisHub organizes this process through a three-layer architecture consisting of **Canvas State, Protocol Bridge, and Agent Runtime**. Canvas State maintains editable artifacts and their relationships; the Protocol Bridge exposes capabilities, validates actions, and manages state transitions; and the Agent Runtime observes the canvas, plans actions, invokes models and tools, and returns results to the shared workspace.

Importantly, JarvisHub is **not intended to replace existing generative models**. Instead, it provides an open and inspectable agent runtime for preserving context, orchestrating external tools and models, incorporating feedback, and recovering from failures across long-horizon creative workflows.

This design moves Creative AI beyond isolated generation and tool invocation toward **sustained, human-steerable creative automation**, where agents can progressively plan, generate, revise, and organize complex multimodal projects while users remain able to inspect, guide, and intervene throughout the process.

### 中文简介

**JarvisHub** 是一个面向 **Canvas-Native Multimodal Creative Agents（画布原生多模态创意智能体）** 的开放式 Agent Harness，主要研究 AI 如何在持续维护项目状态的情况下完成**长周期、多阶段的复杂多模态创作任务**。

当前的图像、视频、音频、网页、UI 和演示文稿等生成模型已经具有较强的单次内容生成能力，但真实创作过程通常并不是简单的“输入 Prompt—生成结果”。一个完整项目往往还包含参考资料、多个草稿、候选方案、修改过程、失败尝试、版本关系、工具操作、评价信号以及持续的人类反馈，这些信息共同构成不断演化的项目状态。

JarvisHub 将**可编辑 Canvas** 作为整个系统的核心。Canvas 不仅承担用户交互界面的作用，同时还充当**用户工作空间、智能体的外部记忆、操作空间以及持久化的共享项目状态**。多模态内容以及它们之间的依赖关系、版本关系、状态和反馈信息，都可以通过结构化的 Canvas 节点与连接进行显式表示。

JarvisHub 采用 **Canvas State、Protocol Bridge 和 Agent Runtime** 三层架构。其中，Canvas State 负责维护可编辑内容及其关系；Protocol Bridge 负责暴露系统能力、验证操作并管理状态转换；Agent Runtime 则负责观察当前 Canvas、规划下一步操作、调用模型与工具，并将新的结果重新写入共享工作空间。

需要特别说明的是，**JarvisHub 本身并不是用于替代现有生成模型的新生成模型**。它更接近一个开放、可检查的智能体运行与编排框架，通过整合外部生成模型、工具和其他 Agent 能力，使智能体能够在长期创作过程中保持上下文、利用反馈并从失败中恢复。

因此，JarvisHub 将 Creative AI 从传统的单次内容生成和孤立工具调用进一步扩展为**持续、可干预、以项目状态为中心的长周期多模态创意智能体工作流**。

---

<a id="jarvisevo"></a>

## JarvisEvo

### Towards a Self-Evolving Photo Editing Agent with Synergistic Editor-Evaluator Optimization

<table>
<tr>
<td width="31%" align="center">

<img src="jarvisevo.png" width="100%" alt="JarvisEvo">

</td>

<td width="69%">

**Year:** 2026  
**Venue:** IEEE/CVF Conference on Computer Vision and Pattern Recognition (**CVPR 2026**)  
**Preprint:** arXiv:2511.23002  
**First Submitted:** November 28, 2025  
**Method Type:** Self-evolving photo-editing agent  
**Task:** Intelligent agent-based photo editing  

**Authors:**  
Yunlong Lin, Linqing Wang, Kunjie Lin, Zixu Lin, Kaixiong Gong, Wenbo Li, Bin Lin, Zhenxi Li, Shiyi Zhang, Yuyang Peng, Wenxun Dai, Xinghao Ding, Chunyu Wang, Qinglin Lu

**Links:**  
[Project](https://jarvisevo.vercel.app/) /
[Paper](https://arxiv.org/abs/2511.23002) /
[PDF](https://arxiv.org/pdf/2511.23002) /
[Code](https://github.com/LYL1015/JarvisEvo) /
[Hugging Face](https://huggingface.co/papers/2511.23002)

### Highlights

- Introduces a unified **self-evolving image-editing agent** that emulates an expert human designer through iterative editing, tool selection, evaluation, and reflection.
- Proposes **interleaved Multimodal Chain-of-Thought (iMCoT)** to integrate visual observations with textual reasoning and mitigate instruction hallucination.
- Introduces **Synergistic Editor-Evaluator Policy Optimization (SEPO)**, which jointly optimizes the Editor and Evaluator to enable self-improvement without external rewards.
- Addresses two key challenges in agent-based image editing: **instruction hallucination** and **reward hacking**.
- Supports both **global and local fine-grained photo editing** through seamless integration with Adobe Lightroom.
- Establishes a unified **Editor-Evaluator framework** in which editing and evaluation capabilities can improve synergistically.
- On ArtEdit-Bench, outperforms Nano-Banana by **18.95% on average on preservative editing metrics**, including a **44.96% improvement in pixel-level content fidelity**.

</td>
</tr>
</table>

### English Introduction

**JarvisEvo** is a unified **self-evolving photo-editing agent** designed to emulate how an expert human designer iteratively edits visual content, selects appropriate tools, evaluates intermediate results, reflects on previous decisions, and progressively refines editing outcomes.

Existing agent-based image-editing systems have substantially improved interactive experiences, editing quality, and creative flexibility. However, two major challenges remain: **instruction hallucination** and **reward hacking**. Text-only Chain-of-Thought reasoning can suffer from information bottlenecks that limit access to important visual information, while policy optimization against static reward models may encourage agents to exploit weaknesses in the reward function.

To address instruction hallucination, JarvisEvo introduces **interleaved Multimodal Chain-of-Thought (iMCoT)**. Instead of relying exclusively on textual reasoning, iMCoT interleaves visual observations with the reasoning process, allowing the agent to incorporate intermediate visual feedback into its decision-making and thereby improve instruction following and editing quality.

To address reward hacking and enable self-improvement, JarvisEvo further proposes **Synergistic Editor-Evaluator Policy Optimization (SEPO)**. Rather than optimizing the editing policy against a fixed external reward model, SEPO synergistically optimizes the **Editor and Evaluator**, allowing editing and evaluation capabilities to improve together without relying on external rewards.

JarvisEvo also integrates **Adobe Lightroom**, enabling both global adjustments and local fine-grained photo editing within a unified agent workflow.

Together, iMCoT and SEPO move intelligent photo editing beyond passive instruction execution toward a **self-evolving Editor-Evaluator agent** capable of multimodal reasoning, tool selection, self-evaluation, reflection, and iterative refinement.

### 中文简介

**JarvisEvo** 是一个具有**自我演化能力的智能照片编辑 Agent（Self-Evolving Photo-Editing Agent）**，其整体工作方式模拟专业设计师的迭代式修图过程：执行编辑、选择合适工具、观察和评价编辑结果，并对之前的决策进行反思，从而持续优化最终编辑效果。

针对现有 Agent-Based Image Editing 中的两个关键问题——**指令幻觉（Instruction Hallucination）**和**奖励黑客（Reward Hacking）**——JarvisEvo 分别提出了 iMCoT 和 SEPO 两项核心技术。

首先，纯文本 Chain-of-Thought 在复杂视觉编辑任务中存在视觉信息瓶颈，可能导致推理结果与实际图像内容不一致，从而产生 Instruction Hallucination。为此，JarvisEvo 提出了 **iMCoT（Interleaved Multimodal Chain-of-Thought）**，将视觉观察与文本推理过程交错结合，使 Agent 能够在决策过程中利用中间视觉反馈，从而提升指令跟随能力和编辑质量。

其次，针对使用固定 Reward Model 进行策略优化时可能出现的 Reward Hacking 问题，JarvisEvo 提出了 **SEPO（Synergistic Editor-Evaluator Policy Optimization）**。与依赖固定外部奖励模型的方法不同，SEPO 对 **Editor 和 Evaluator 进行协同优化**，使编辑能力与评价能力能够共同提升，并实现无需外部奖励的自我改进。

此外，JarvisEvo 与 **Adobe Lightroom** 深度集成，使 Agent 能够在统一工作流中同时执行全局调整与局部细粒度照片编辑。

因此，JarvisEvo 将智能图像编辑从传统的被动指令执行进一步扩展为一个能够进行**多模态推理、工具选择、自我评价、反思以及迭代优化的 Self-Evolving Editor-Evaluator Agent**。

---

<a id="jarvisx-cowork"></a>

## JarvisX-Cowork

### A Personal AI Creative Assistant for Everyone

<table>
<tr>
<td width="31%" align="center">

<img src="jarvisx-cowork.png" width="100%" alt="JarvisX-Cowork">

</td>

<td width="69%">

**Year:** 2026  
**Status:** Open-Source Project  
**Type:** End-to-end creative-agent harness  
**Positioning:** Personal AI creative assistant  
**Task:** Open-ended, end-to-end creative workflows  
**Research Direction:** Long-horizon creative agents and human-AI collaboration  

**Keywords:**  
Creative Agent · AI Cowork · End-to-End Workflow · Persistent Planning · Shared Memory · Tool Orchestration · Human-AI Collaboration

**Links:**  
[Code](https://github.com/LYL1015/JarvisX-Cowork) /
[Demo Video](https://youtu.be/SiNsTmGbWlo)

### Highlights

- Introduces a **personal AI creative assistant** for open-ended, end-to-end creative workflows.
- Turns a terminal-oriented AI agent into a **visual, collaborative, and creative desktop companion**.
- Supports creative workflows spanning **reference search, content generation, professional refinement, video creation, and final deliverable production**.
- Integrates creative capabilities including **WebSearch, image generation and editing, Lightroom-based refinement, and video generation**.
- Uses **persistent planning, shared memory, and structured tool interfaces** to carry project state from initial intent to final deliverables.
- Supports common agent capabilities such as file operations, command execution, web access, task planning, and human-in-the-loop permission control.
- Functions as an **agent harness/application rather than a standalone generative model**, orchestrating existing models, tools, and creative skills within a unified workflow.

</td>
</tr>
</table>

### English Introduction

**JarvisX-Cowork** is an open-source **personal AI creative assistant** designed to support open-ended, end-to-end creative workflows. Rather than focusing on a single generation task, it explores how an AI agent can accompany users throughout a complete creative process, from initial inspiration to final deliverables.

Conventional AI tools often handle isolated tasks such as generating an image, writing a piece of text, or answering a question. Real creative work, however, typically involves multiple interconnected stages, including discovering inspiration, collecting references, developing ideas, generating visual content, refining intermediate results, producing videos, and assembling final presentations or documents.

JarvisX-Cowork integrates these stages into a unified creative workflow. A representative process can begin with a blank canvas, use **WebSearch** to discover references, generate images, refine visual results through professional editing tools such as **Adobe Lightroom**, create videos, and finally produce demos, presentation decks, or documents.

Beyond individual creative tools, JarvisX-Cowork uses **persistent planning, shared memory, and structured tool interfaces** to help the agent maintain coherent project state across longer workflows. It also retains general agent capabilities such as file operations, command execution, web access, task planning, and human-in-the-loop confirmation for important tool operations.

Importantly, JarvisX-Cowork is better understood as an **end-to-end creative-agent harness and application rather than a standalone generative model**. It orchestrates existing models, tools, and creative skills within a unified desktop environment.

Overall, JarvisX-Cowork positions AI not merely as a single-purpose generation tool, but as a **personal creative coworker** capable of assisting users across multiple stages of a creative project, from inspiration and planning to generation, refinement, and final delivery.

### 中文简介

**JarvisX-Cowork** 是一个开源的**个人 AI 创意协作助手（Personal AI Creative Assistant）**，主要面向开放式、端到端的创意工作流程。与只负责某一个生成环节的传统 AI 工具不同，JarvisX-Cowork 探索如何让 Agent 从最初的创意构思一直参与到最终成果交付。

真实创作过程通常包含多个相互关联的阶段，例如寻找灵感、搜索参考资料、形成创意方案、生成视觉素材、修改和优化中间结果、制作视频，以及最终整理为演示文稿、文档或其他交付成果。

JarvisX-Cowork 将这些能力整合到统一的创意工作流中。一个典型流程可以从空白创意空间开始，通过 **WebSearch** 搜索参考内容，随后进行图像生成，再借助 **Adobe Lightroom** 等专业工具完成视觉优化，并进一步生成视频以及制作 Demo、Presentation Deck 或 Document 等最终成果。

在单独的生成与编辑工具之外，JarvisX-Cowork 还通过**持续规划、共享记忆以及结构化工具接口**帮助 Agent 在较长的任务过程中保持连贯的项目状态。同时，它还具备文件操作、命令执行、Web 信息获取、任务规划以及 Human-in-the-Loop 权限确认等通用 Agent 能力。

需要注意的是，**JarvisX-Cowork 本身并不是一个新的生成式基础模型**。更准确地说，它是一个面向个人创作场景的 **End-to-End Creative-Agent Harness / Application**，通过统一工作环境对已有模型、专业工具和 Creative Skills 进行组织与调用。

因此，JarvisX-Cowork 将 AI 从传统的单一生成工具进一步扩展为能够贯穿“**灵感 → 搜索 → 生成 → 优化 → 视频 → 最终交付**”全过程的 **Personal AI Creative Coworker**。

---

<a id="jarvisart"></a>

## JarvisArt

### Liberating Human Artistic Creativity via an Intelligent Photo Retouching Agent

<table>
<tr>
<td width="31%" align="center">

<img src="jarvisart.gif" width="100%" alt="JarvisArt Demo">

</td>

<td width="69%">

**Year:** 2025  
**Venue:** Conference on Neural Information Processing Systems (**NeurIPS 2025**)  
**Preprint:** arXiv:2506.17612  
**First Submitted:** June 21, 2025  
**Method Type:** MLLM-driven professional photo-retouching agent  
**Task:** Intelligent professional photo retouching  

**Authors:**  
Yunlong Lin, Zixu Lin, Kunjie Lin, Jinbin Bai, Panwang Pan, Chenxin Li, Haoyu Chen, Zhongdao Wang, Xinghao Ding, Wenbo Li, Shuicheng Yan

**Links:**  
[Project](https://jarvisart.vercel.app/) /
[Paper](https://arxiv.org/abs/2506.17612) /
[Code](https://github.com/LYL1015/JarvisArt) /
[Hugging Face](https://huggingface.co/papers/2506.17612) /
[YouTube](https://www.youtube.com/watch?v=Ol28DQj8wV8) /
[Bilibili](https://www.bilibili.com/video/BV1Sd3nzREvP)

### Highlights

- Introduces an **MLLM-driven intelligent agent** for professional photo retouching.
- Understands natural-language user intentions and mimics the reasoning process of professional artists.
- Intelligently coordinates more than **200 retouching tools within Adobe Lightroom**.
- Employs a two-stage training strategy consisting of **Chain-of-Thought supervised fine-tuning** followed by **Group Relative Policy Optimization for Retouching (GRPO-R)**.
- Introduces the **Agent-to-Lightroom Protocol** for seamless integration between the intelligent agent and Adobe Lightroom.
- Develops **MMArt-Bench** for comprehensive evaluation of professional photo-retouching performance.
- Provides **fine-grained control over both global and local adjustments**.
- Outperforms GPT-4o by **60% on average pixel-level content-fidelity metrics** on MMArt-Bench while maintaining comparable instruction-following capabilities.

</td>
</tr>
</table>

<div align="center">
<table>
  <tr>
    <th align="center">Before</th>
    <th align="center">After · JarvisArt</th>
  </tr>
  <tr>
    <td align="center">
      <img src="https://jarvisart.vercel.app/assets/results/0/original.jpg" height="200" alt="Before retouching">
    </td>
    <td align="center">
      <img src="https://jarvisart.vercel.app/assets/results/0/processed.jpg" height="200" alt="After retouching">
    </td>
  </tr>
</table>

<sub>Photo-retouching example · <a href="https://jarvisart.vercel.app/">More examples ↗</a></sub>
</div>

### English Introduction

**JarvisArt** is an **MLLM-driven intelligent photo-retouching agent** designed to bridge the gap between high-level human artistic intentions and professional image-editing operations.

Professional software such as Adobe Lightroom provides powerful and highly adjustable editing capabilities, but effective use often requires substantial technical expertise, artistic judgment, and manual effort. Existing AI-based editing solutions provide greater automation, yet they may suffer from limited adjustability and poor generalization when handling diverse and personalized editing requirements.

JarvisArt addresses this challenge through a **Multimodal Large Language Model (MLLM)-driven agent**. The system understands natural-language user intent, analyzes visual content, mimics the reasoning process of professional artists, and intelligently coordinates more than **200 retouching tools within Adobe Lightroom**.

JarvisArt adopts a two-stage training strategy. First, **Chain-of-Thought supervised fine-tuning** establishes fundamental reasoning and tool-use capabilities. It then applies **Group Relative Policy Optimization for Retouching (GRPO-R)** to further improve decision-making and proficiency in professional retouching tools.

To connect high-level agent decisions with executable operations in professional editing software, JarvisArt introduces the **Agent-to-Lightroom Protocol**, enabling seamless interaction between the intelligent agent and Adobe Lightroom.

For evaluation, JarvisArt develops **MMArt-Bench**, providing a benchmark for comprehensive assessment of professional photo-retouching performance across diverse scenarios. JarvisArt demonstrates strong generalization and fine-grained control over both global and local adjustments. On MMArt-Bench, it outperforms GPT-4o by **60% on average pixel-level metrics for content fidelity**, while maintaining comparable instruction-following capabilities.

Overall, JarvisArt demonstrates how multimodal agents can function as professional creative collaborators, translating abstract user intentions into **controllable, fine-grained, and executable photo-retouching operations** within professional editing software.

### 中文简介

**JarvisArt** 是一个由**多模态大语言模型（MLLM）驱动的专业照片修饰 Agent**，旨在弥合用户高层艺术意图与专业图像编辑操作之间的鸿沟。

Adobe Lightroom 等专业照片编辑软件具有丰富且高度可调的修图能力，但有效使用这些工具通常需要较强的专业知识、艺术判断能力以及大量人工操作。现有 AI 图像编辑方法虽然提高了自动化程度，但在面对多样化和个性化的编辑需求时，仍可能存在可调节性不足和泛化能力有限等问题。

JarvisArt 采用 **MLLM 驱动的 Agent 架构**。智能体能够理解用户通过自然语言表达的编辑意图、分析视觉内容，并模仿专业艺术家的推理过程，从而在 Adobe Lightroom 中智能协调超过 **200 个专业修图工具**。

在训练方面，JarvisArt 采用两阶段策略。首先通过 **Chain-of-Thought 监督微调（CoT SFT**建立基础推理和工具使用能力；随后采用专门面向照片修饰任务设计的 **GRPO-R（Group Relative Policy Optimization for Retouching）**，进一步提升 Agent 的编辑决策能力以及专业工具使用水平。

为了将 Agent 的高层决策转化为能够在专业软件中真正执行的编辑操作，JarvisArt 进一步提出 **Agent-to-Lightroom Protocol**，实现智能体与 Adobe Lightroom 之间的无缝交互。

在评测方面，项目构建了 **MMArt-Bench**，用于综合评估专业照片修饰性能。JarvisArt 展现出良好的泛化能力以及对全局和局部调整的细粒度控制能力。在 MMArt-Bench 上，其 Content Fidelity 的平均 Pixel-Level Metrics 相比 GPT-4o **提升 60%**，同时保持了相当的 Instruction-Following 能力。

总体而言，JarvisArt 展示了多模态智能体作为**专业创意协作者**的可能性，使 AI 能够将抽象的用户艺术意图转化为在专业编辑软件中**可控、细粒度且真正可执行的照片修饰操作**。

---

<a id="jarvisir"></a>

## JarvisIR

### Elevating Autonomous Driving Perception with Intelligent Image Restoration

<table>
<tr>
<td width="31%" align="center">

<img src="jarvisir.gif" width="100%" alt="JarvisIR Demo">

</td>

<td width="69%">

**Year:** 2025  
**Venue:** IEEE/CVF Conference on Computer Vision and Pattern Recognition (**CVPR 2025**)  
**Publication Date:** June 2025  
**Method Type:** VLM-powered intelligent image-restoration agent  
**Task:** Intelligent image restoration for robust vision-centric perception  

**Authors:**  
Yunlong Lin, Zixu Lin, Haoyu Chen, Panwang Pan, Chenxin Li, Sixiang Chen, Kairun Wen, Yeying Jin, Wenbo Li, Xinghao Ding

**Links:**  
[Project](https://cvpr2025-jarvisir.github.io/) /
[Paper](https://lyl1015.github.io/papers/CVPR2025_JarvisIR.pdf) /
[Code](https://github.com/LYL1015/JarvisIR) /
[Hugging Face Demo](https://huggingface.co/spaces/LYL1015/JarvisIR)

### Highlights

- Published at **CVPR 2025**.
- Introduces a **VLM-powered intelligent image-restoration agent** for robust vision-centric perception under unpredictable and coupled weather degradations.
- Uses a **VLM as the controller** to analyze degradation conditions, plan restoration tasks, and coordinate multiple expert restoration models.
- Employs a two-stage training framework consisting of **Supervised Fine-Tuning (SFT)** and **Human Feedback Alignment** to improve robustness, reduce hallucinations, and enhance real-world generalization.
- Introduces **CleanBench**, a large-scale instruction-response dataset containing **150K synthetic and 80K real entries** for training and evaluation.
- Connects **low-level image restoration** with **high-level downstream visual perception** in autonomous-driving environments.
- Achieves a **50% improvement in the average of all perception metrics on CleanBench-Real** compared with existing methods.

</td>
</tr>
</table>

### English Introduction

**JarvisIR** is a **VLM-powered intelligent image-restoration agent** designed to improve the robustness of vision-centric perception systems under unpredictable and coupled weather degradations in real-world environments.

Real-world autonomous-driving systems frequently encounter complex visual degradations caused by adverse weather and challenging imaging conditions. These degradations may occur simultaneously and can substantially affect not only image quality but also downstream perception performance.

Existing restoration approaches are often either **task-specific methods** that rely on prior knowledge of degradation types, or **all-in-one methods** that may suffer from substantial domain gaps when trained primarily on synthetic data. Moreover, when multiple specialized restoration models are combined, their execution order can significantly influence the final restoration quality.

JarvisIR addresses these challenges by using a **Vision-Language Model (VLM) as a controller**. Instead of relying on a single fixed restoration model, the VLM analyzes the current visual degradation, plans appropriate restoration tasks, selects specialized expert models, and coordinates their execution to handle complex real-world conditions.

To further improve robustness and generalization, JarvisIR adopts a two-stage training framework consisting of **Supervised Fine-Tuning (SFT)** and **Human Feedback Alignment**. The human-feedback alignment stage enables the VLM to effectively leverage large-scale real-world degraded data despite the lack of corresponding paired ground-truth images, while helping reduce hallucinations and improve generalization under adverse weather.

The project also introduces **CleanBench**, a comprehensive instruction-response dataset containing **150K synthetic and 80K real entries**, to support both the training and evaluation of JarvisIR.

By combining VLM-based decision-making with specialized restoration models, JarvisIR transforms image restoration from a fixed low-level processing pipeline into a more autonomous and adaptive agent-based workflow. On CleanBench-Real, it achieves a **50% improvement in the average of all perception metrics** compared with existing methods.

Overall, JarvisIR establishes a connection between **low-level image restoration** and **high-level vision-centric perception**, demonstrating how intelligent restoration agents can provide more reliable visual inputs for autonomous-driving systems operating under complex real-world conditions.

### 中文简介

**JarvisIR** 是一个由**视觉语言模型（VLM）驱动的智能图像恢复 Agent**，旨在提升视觉感知系统在真实世界不可预测、复合恶劣天气退化条件下的鲁棒性。

现实中的自动驾驶视觉系统经常面对复杂的恶劣天气与成像条件，不同类型的图像退化还可能同时出现并相互耦合。这些问题不仅会降低输入图像本身的视觉质量，还可能进一步影响后续的视觉感知性能。

现有方法主要面临两类问题：一类是针对特定退化类型设计的 **Task-Specific Restoration Methods**，通常需要预先知道图像的退化类型；另一类是 **All-in-One Restoration Methods**，这类方法在主要依赖合成数据进行监督训练时，面对真实世界数据可能存在明显的 Domain Gap。此外，当多个专业恢复模型组合使用时，不同模型的执行顺序也可能显著影响最终恢复效果。

JarvisIR 的核心思想是让 **VLM 充当整个恢复系统的 Controller**。系统并不依赖单一固定恢复模型，而是由 VLM 分析当前输入图像的退化情况、规划恢复任务、选择合适的专业恢复模型，并协调多个 Expert Restoration Models 的执行，从而处理复杂且耦合的真实世界图像退化。

在训练方面，JarvisIR 采用由 **Supervised Fine-Tuning**和 **Human Feedback Alignment** 组成的两阶段框架。Human Feedback Alignment 使 VLM 能够在缺少成对 Ground Truth 的情况下有效利用大规模真实退化数据，同时进一步提升系统鲁棒性、减少幻觉并增强真实恶劣天气环境下的泛化能力。

为了支持系统训练与评测，项目进一步构建了 **CleanBench**，其中包含约 **15 万组合成数据和 8 万组真实数据对应的 Instruction-Response Entries**。

通过将 VLM 的分析、规划与决策能力和多个专业图像恢复模型相结合，JarvisIR 将传统固定的低层图像恢复流程扩展为更加自主、灵活和自适应的 **Agent-Based Restoration Workflow**。在 CleanBench-Real 上，JarvisIR 相比现有方法在所有感知指标平均值上取得了约 **50% 的提升**。

因此，JarvisIR 不再将图像恢复视为完全独立的低层视觉任务，而是进一步建立了**低层图像恢复（Low-Level Image Restoration）与高层视觉感知（High-Level Visual Perception）之间的联系**。

---

<div align="center">

## SmartDSP Lab

### From Intelligent Visual Restoration to Canvas-Native Multimodal Creative Agents

**JarvisIR → JarvisArt → JarvisEvo → JarvisX-Cowork → JarvisHub**

**Restoration → Retouching → Self-Evolution → Creative Coworking → Canvas-Native Agents**

<br>

Exploring **multimodal agents, intelligent visual systems, professional image editing, human-AI creative collaboration, and long-horizon multimodal creation**.

<br><br>

<sub>SmartDSP Lab · Datasets · Benchmarks · Research Publications · Open-Source Projects · Interactive Demos</sub>

</div>
