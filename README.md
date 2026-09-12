<div align="center">

# SmartDSP · Jarvis Research Collection

### Multimodal Agents · Creative AI · Intelligent Image Editing · Image Restoration

A curated collection of **datasets, benchmarks, publications, and research projects** from **SmartDSP Lab**,  
covering multimodal creative agents, intelligent photo editing, human-AI collaboration,  
and image restoration for visual perception.

<br>

**Datasets · Benchmarks · Publications · Open-source Projects · Interactive Demos**

</div>

---

## Overview

The **SmartDSP Jarvis Research Collection** brings together a series of research efforts exploring the evolution of intelligent visual systems from specialized image processing methods toward increasingly general, autonomous, and collaborative multimodal agents.

The collection currently consists of three major components:

- **📦 Datasets & Benchmarks** — Public datasets and evaluation benchmarks for professional photo retouching, intelligent image editing, and adverse-condition image restoration, including **MMArt-PPR10K**, **MMArt-Bench**, **ArtEdit-Bench**, and **CleanBench**.
- **📚 Publications from SmartDSP Lab** — Research works spanning intelligent image restoration, multimodal photo-retouching agents, self-evolving editing agents, personal creative assistants, and canvas-native multimodal agents.
- **🚀 Jarvis Research Projects** — A family of intelligent visual and creative systems, including **JarvisIR**, **JarvisArt**, **JarvisEvo**, **JarvisX-Cowork**, and **JarvisHub**.

Together, these works reflect a continuous research trajectory:

<div align="center">

**Intelligent Image Restoration → Professional Photo Retouching → Self-Evolving Editing → AI Creative Coworkers → Canvas-Native Multimodal Agents**

</div>

The overall goal is to explore how AI systems can move beyond isolated generation or enhancement tasks and become **persistent, interpretable, tool-using, human-steerable collaborators** for visual understanding and creative production.

---

## Table of Contents

- [1. Datasets & Benchmarks](#1-datasets--benchmarks)
  - [Dataset Summary](#dataset-summary)
  - [MMArt-PPR10K](#mmart-ppr10k)
  - [MMArt-Bench](#mmart-bench)
  - [ArtEdit-Bench](#artedit-bench)
  - [CleanBench](#cleanbench)
  - [Dataset Availability for Other Jarvis Projects](#dataset-availability-for-other-jarvis-projects)

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
| **MMArt-PPR10K** | JarvisArt | Multimodal paired retouching dataset | PPR10K-based multimodal retouching data with images, user instructions, and Lightroom editing configurations | Training instruction-driven professional photo-retouching agents | [Dataset](https://huggingface.co/datasets/JarvisArt/MMArt-PPR10k) / [Paper](https://arxiv.org/abs/2506.17612) |
| **MMArt-Bench** | JarvisArt | Real-world retouching benchmark | 200 benchmark instances across 4 major scenarios + portrait region-level evaluation subset | Evaluating instruction following, retouching quality, and content fidelity | [Dataset](https://huggingface.co/datasets/JarvisArt/MMArt-Bench) / [Paper](https://arxiv.org/abs/2506.17612) |
| **ArtEdit-Bench** | JarvisEvo | Image-editing benchmark | Preservative and instruction-following image-editing evaluation | Evaluating self-evolving image-editing agents | [Dataset](https://huggingface.co/datasets/JarvisEvo/ArtEdit-Bench) / [Paper](https://arxiv.org/abs/2511.23002) |
| **CleanBench** | JarvisIR | Synthetic + real-world restoration dataset | 150K synthetic + 80K real instruction-response pairs | Training and evaluating intelligent restoration agents for autonomous-driving perception | [Dataset](https://huggingface.co/datasets/LYL1015/CleanBench) / [Project](https://cvpr2025-jarvisir.github.io/) / [Paper](https://lyl1015.github.io/papers/CVPR2025_JarvisIR.pdf) |

---

<a id="mmart-ppr10k"></a>

## MMArt-PPR10K

**Related Project:** JarvisArt  
**Paper:** *JarvisArt: Liberating Human Artistic Creativity via an Intelligent Photo Retouching Agent*  
**Task:** Instruction-driven professional photo retouching  
**Type:** Multimodal paired image-retouching dataset  
**Source:** Built upon the PPR10K dataset  
**Content:** Original images, retouched images, user instructions, Lightroom Lua configurations, and XMP editing presets  

### English Introduction

**MMArt-PPR10K** is a multimodal dataset developed for research on instruction-driven agentic photo retouching. It extends the original PPR10K dataset by combining paired before-and-after images with natural-language editing instructions and structured Lightroom editing information.

Unlike conventional image-to-image datasets that only provide input and target images, MMArt-PPR10K additionally describes both **what the user wants** and **how the desired visual result can be achieved using professional editing tools**. This makes the dataset particularly suitable for training multimodal photo-retouching agents that must understand user intent, reason about visual content, and translate natural-language instructions into executable editing operations.

The dataset also provides structured Lua and XMP configurations corresponding to Lightroom editing actions, enabling research on multimodal reasoning, professional tool use, instruction following, and agent-based photo-editing workflows.

### 中文简介

**MMArt-PPR10K** 是 JarvisArt 面向**指令驱动专业修图 Agent**构建的多模态数据集，在原始 PPR10K 数据集基础上进一步扩展得到。

与传统仅包含输入图像与目标图像的数据集不同，MMArt-PPR10K 除了提供修图前后的成对图像之外，还进一步加入了不同长度的用户编辑指令，以及 Adobe Lightroom 对应的 Lua 配置和 XMP 编辑预设。

这些信息能够同时描述“**用户想要什么效果**”以及“**专业修图工具如何实现这一效果**”。因此，该数据集不仅适用于传统图像到图像学习，还非常适合研究自然语言编辑指令理解、多模态推理、专业工具调用以及 Agent 驱动的照片修饰流程。

### Dataset Structure

- `before.jpg` — original unedited image
- `processed.jpg` — professionally retouched image
- `user_want_short` — short user instruction
- `user_want_middle` — medium-length user instruction
- `user_want_long` — detailed user instruction
- `config.lua` — Lightroom Lua editing configuration
- `config.xmp` — Lightroom XMP metadata / editing preset

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
**Task:** Intelligent photo-retouching evaluation  
**Type:** Real-world multimodal benchmark  
**Scale:** 200 benchmark instances across four major scenarios + portrait subset for region-level evaluation  
**Scenarios:** Portrait · Landscape · Street · Still Life  

### English Introduction

**MMArt-Bench** is the evaluation benchmark introduced with JarvisArt for assessing intelligent photo-retouching agents under realistic user-editing scenarios.

The benchmark covers four major categories — **portrait photography, landscape photography, street scenes, and still life** — with 50 evaluation instances in each category, resulting in 200 primary benchmark cases. An additional portrait subset with human-region mask annotations is provided for region-level evaluation.

MMArt-Bench is designed to evaluate more than visual attractiveness alone. It focuses on whether an editing agent can correctly follow a user's editing intention while preserving image structure, semantic identity, and regions that should remain unchanged.

This makes MMArt-Bench particularly useful for evaluating intelligent agents that perform multi-step reasoning and tool-based editing rather than uncontrolled one-shot image generation.

### 中文简介

**MMArt-Bench** 是 JarvisArt 提出的**智能照片修饰评测基准**，主要用于评估多模态修图 Agent 在真实用户编辑场景下的指令理解能力、视觉质量和内容保持能力。

该基准覆盖 **人像、风景、街景和静物**四类主要场景，每一类包含 50 个主要评测实例，共计 200 个核心 Benchmark Cases。此外，还提供带有人物区域 Mask 标注的人像子集，用于更加细粒度的 Region-Level Evaluation。

与只关注最终视觉效果的传统评测方式不同，MMArt-Bench 更强调一个智能修图 Agent 是否能够在正确完成用户修改需求的同时，保持原图的结构、主体身份、局部区域以及其他不应改变的视觉内容。

因此，它非常适合用于评估具有多模态推理、专业工具调用和多阶段决策能力的智能修图系统。

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
**Task:** Intelligent image-editing evaluation  
**Type:** Image-editing benchmark  
**Evaluation Focus:** Instruction following · Preservative editing · Content fidelity  

### English Introduction

**ArtEdit-Bench** is an image-editing benchmark used to evaluate JarvisEvo and other intelligent image-editing systems.

The benchmark focuses not only on whether an agent successfully performs the requested modification, but also on whether unrelated visual content remains unchanged. This capability is especially important for professional and agent-based editing systems, where uncontrolled changes to identity, structure, texture, background, or non-target regions can significantly reduce editing reliability.

ArtEdit-Bench therefore emphasizes **preservative editing** and **content fidelity**, providing a useful evaluation setting for studying the balance between instruction following, visual editing quality, and preservation of original image information.

For self-evolving agents such as JarvisEvo, this benchmark is particularly valuable because it enables systematic evaluation of whether iterative reasoning, self-evaluation, and refinement actually lead to better and more faithful editing results.

### 中文简介

**ArtEdit-Bench** 是 JarvisEvo 使用的**智能图像编辑评测基准**，主要用于评估编辑 Agent 在执行用户编辑指令时的准确性和内容保持能力。

对于智能图像编辑而言，仅仅“完成目标修改”是不够的。如果 Agent 在修改指定对象或区域时，同时改变了人物身份、背景、纹理、结构或其他无关内容，那么这种编辑仍然缺乏足够的可靠性和可控性。

因此，ArtEdit-Bench 特别强调 **Preservative Editing（保持式编辑）** 与 **Content Fidelity（内容保真度）**，用于衡量一个编辑系统是否能够在完成目标修改的同时，最大程度保留原始图像中不应发生变化的内容。

对于 JarvisEvo 这类具有自我评价和自我优化能力的 Editing Agent，ArtEdit-Bench 也能够用于检验其迭代推理、评价和改进机制是否真正提升了最终编辑质量。

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
**Task:** Intelligent image restoration for autonomous-driving perception  
**Type:** Synthetic + real-world adverse-condition restoration dataset  
**Scale:** 150K synthetic + 80K real instruction-response pairs  
**Coverage:** Night · Rain · Fog · Snow · Mixed degradation conditions  

### English Introduction

**CleanBench** is a large-scale training and evaluation resource developed for JarvisIR, targeting intelligent image restoration under adverse visual conditions in autonomous-driving scenarios.

The benchmark contains both synthetic and real-world components. The synthetic portion provides approximately **150K degraded training samples**, while the real-world component contains approximately **80K images** collected under challenging environmental and illumination conditions.

The covered degradation scenarios include night scenes, rain, fog, snow, and combinations of multiple degradation types. This allows an intelligent restoration agent to learn both controlled degradation patterns and complex real-world visual conditions.

CleanBench is designed not only for conventional low-level image restoration, but also for training and evaluating an intelligent restoration system that must first understand the current degradation condition and then coordinate appropriate restoration capabilities.

This makes CleanBench a bridge between **low-level visual restoration** and **high-level autonomous-driving perception**.

### 中文简介

**CleanBench** 是 JarvisIR 构建的大规模**自动驾驶恶劣环境图像恢复数据集与评测基准**，用于训练和评价能够自主分析退化情况并协调不同恢复能力的智能图像恢复 Agent。

CleanBench 同时包含合成数据与真实数据。其中，Synthetic 部分包含约 **15 万组人工构造的退化训练样本**，Real 部分包含约 **8 万张真实复杂环境图像**。

其覆盖场景包括夜间、雨天、雾天、雪天以及多种退化情况组合，使模型既能够学习相对可控的图像退化规律，也能够面对更加复杂的真实世界视觉条件。

与仅面向单一低层图像恢复任务的数据集不同，CleanBench 还服务于智能 Restoration Agent 的训练与评测：系统不仅需要执行恢复操作，还需要首先判断当前视觉问题，并进一步协调合适的恢复能力。

因此，CleanBench 建立了**低层图像恢复与高层自动驾驶视觉感知之间的重要联系**。

### Public Releases

- **CleanBench-Synthetic** — approximately 150K synthetic degraded instruction-response samples
- **CleanBench-Real** — approximately 80K real-world adverse-condition samples
- **CleanBench-Real-80K** — public real-world release
- **CleanBench-Test / Paper Test** — evaluation data used for reproducing paper experiments

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
| 2026 | **JarvisHub: An Open Harness for Canvas-Native Multimodal Creative Agents** | Canvas-native multimodal creative-agent framework | Yunlong Lin et al. | Preprint / arXiv 2026 | [Project](https://www.jarvishub.site/) / [Paper](https://arxiv.org/abs/2607.23588) / [Code](https://github.com/LYL1015/JarvisHub) / [HF](https://huggingface.co/papers/2607.23588) |
| 2026 | **JarvisEvo: Towards a Self-Evolving Photo Editing Agent with Synergistic Editor-Evaluator Optimization** | Self-evolving multimodal photo-editing agent | Yunlong Lin et al. | CVPR 2026 | [Project](https://jarvisevo.vercel.app/) / [Paper](https://arxiv.org/abs/2511.23002) / [Code](https://github.com/LYL1015/JarvisEvo) / [HF](https://huggingface.co/papers/2511.23002) |
| — | **JarvisX-Cowork: A Personal AI Creative Assistant for End-to-End Creative Workflows** | Personal multimodal creative assistant | — | Demo / Open-source Project | [Code](https://github.com/LYL1015/JarvisX-Cowork) / [Demo](https://youtu.be/SiNsTmGbWlo) |
| 2025 | **JarvisArt: Liberating Human Artistic Creativity via an Intelligent Photo Retouching Agent** | MLLM-driven professional photo-retouching agent | Yunlong Lin et al. | NeurIPS 2025 | [Project](https://jarvisart.vercel.app/) / [Paper](https://arxiv.org/abs/2506.17612) / [Code](https://github.com/LYL1015/JarvisArt) / [HF](https://huggingface.co/papers/2506.17612) |
| 2025 | **JarvisIR: Elevating Autonomous Driving Perception with Intelligent Image Restoration** | Intelligent image-restoration agent | Yunlong Lin et al. | CVPR 2025 | [Project](https://cvpr2025-jarvisir.github.io/) / [Paper](https://lyl1015.github.io/papers/CVPR2025_JarvisIR.pdf) / [Code](https://github.com/LYL1015/JarvisIR) / [Demo](https://huggingface.co/spaces/LYL1015/JarvisIR) |

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
**Venue / Status:** arXiv · Computer Vision and Pattern Recognition (cs.CV)  
**Submitted:** July 26, 2026  
**Method Type:** Canvas-native multimodal creative-agent framework  
**Task:** Long-horizon multimodal creative production and workflow orchestration  

**Authors:**  
Yunlong Lin, Zixu Lin, Zhaohu Xing, Biqiang Li, Chenxin Li, Haonan Wang, Haitao Wu, Hengyu Liu, Jianghai Chen, Kaituo Feng, Kaixin Li, Shawn Chen, Shijue Huang, Sixiang Chen, Tsung-Yi Ho, Wenxuan Huang, Xiangyan Liu, Xiaomeng Hu, Xuanhua He, Yan Sun, Yunqing Zhao, Zhiqin Yang, Zehan Wang, Zhengyang Tang, Tianyu Pang, Xiangyu Yue

**Links:**  
[Project](https://www.jarvishub.site/) /
[Paper](https://arxiv.org/abs/2607.23588) /
[Code](https://github.com/LYL1015/JarvisHub) /
[Hugging Face](https://huggingface.co/papers/2607.23588)

### Highlights

- Introduces a **canvas-native creative-agent harness** for long-horizon multimodal creation.
- Treats the editable canvas simultaneously as the **user workspace, external memory, action space, and shared project state**.
- Represents multimodal artifacts, dependencies, versions, and human feedback through structured canvas nodes and links.
- Employs a three-layer architecture consisting of **Canvas State, Protocol Bridge, and Agent Runtime**.
- Enables agents to continuously plan, generate, revise, organize, and maintain multimodal projects.
- Preserves human steerability by allowing users to inspect, guide, modify, and intervene throughout the creative process.

</td>
</tr>
</table>

### English Introduction

**JarvisHub** is an open harness for **canvas-native multimodal creative agents**, designed to support long-horizon creative production.

Modern generative models are capable of producing high-quality images, videos, audio, webpages, UI elements, presentations, and other creative assets. However, real creative work rarely consists of isolated prompt-output interactions. Instead, a complete project evolves through references, drafts, alternatives, edits, failed attempts, version relationships, tool actions, evaluation signals, and human feedback.

JarvisHub addresses this limitation by placing an editable visual **Canvas** at the center of the agent workflow. The Canvas is not merely an interface: it also functions as the agent's external memory, action space, and persistent shared project state.

Multimodal artifacts and their relationships are explicitly represented through typed nodes and links, allowing information to persist throughout a long creative process.

Through its **Canvas State – Protocol Bridge – Agent Runtime** architecture, JarvisHub enables creative agents to work inside an inspectable and editable workspace. This moves Creative AI beyond isolated tool invocation toward sustained, human-steerable automation in which an agent can continuously plan, generate, revise, organize, and maintain complex multimodal projects.

### 中文简介

**JarvisHub** 是一个面向 **Canvas-Native Multimodal Creative Agents（画布原生多模态创意智能体）** 的开放式智能体框架，主要研究 AI 如何完成长周期、多阶段、具有持续项目状态的复杂多模态创作任务。

当前的图像、视频、音频、网页和演示文稿生成模型已经具有较强的单次内容生成能力，但真实创作过程通常并不是简单的“输入 Prompt—生成结果”。一个完整项目往往还包含参考资料、多个草稿、候选方案、修改过程、失败尝试、版本关系、工具操作、评价信号以及持续的人类反馈。

JarvisHub 将**可编辑 Canvas** 作为整个系统的核心。Canvas 不仅承担用户交互界面的作用，同时还充当智能体的外部记忆、操作空间以及共享项目状态。不同多模态内容、版本关系、依赖关系和反馈信息都可以通过结构化节点和连接进行表示。

通过 **Canvas State、Protocol Bridge 和 Agent Runtime** 三层架构，JarvisHub 使智能体能够在透明、可查看、可修改的创意状态中持续工作。

这使 Creative AI 从传统的单次内容生成进一步发展为能够**持续规划、生成、修改、组织和维护复杂项目的长周期多模态创意智能体**。

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

**Authors:**  
Yunlong Lin, Linqing Wang, Kunjie Lin, Zixu Lin, Kaixiong Gong, Wenbo Li, Bin Lin, Zhenxi Li, Shiyi Zhang, Yuyang Peng, Wenxun Dai, Xinghao Ding, Chunyu Wang, Qinglin Lu

**Links:**  
[Project](https://jarvisevo.vercel.app/) /
[Paper](https://arxiv.org/abs/2511.23002) /
[PDF](https://arxiv.org/pdf/2511.23002) /
[Code](https://github.com/LYL1015/JarvisEvo) /
[Hugging Face](https://huggingface.co/papers/2511.23002)

### Highlights

- Introduces a unified image-editing agent that imitates the iterative workflow of a professional human designer.
- Proposes **interleaved Multimodal Chain-of-Thought (iMCoT)** reasoning.
- Introduces **Synergistic Editor-Evaluator Policy Optimization (SEPO)** for self-improvement without external rewards.
- Targets both **instruction hallucination** and **reward hacking** in agent-based image editing.
- Supports global and local fine-grained editing.
- Integrates Adobe Lightroom into the agent workflow.
- Demonstrates strong preservative editing and pixel-level content fidelity on ArtEdit-Bench.

</td>
</tr>
</table>

### English Introduction

**JarvisEvo** is a unified **self-evolving photo-editing agent** designed to emulate how an expert human designer edits, evaluates, reflects, and progressively improves visual content.

Existing editing agents have significantly improved interaction and automation, but important limitations remain. Text-only reasoning can lose critical visual information and lead to instruction hallucination, while policy optimization against static reward models may encourage reward hacking.

JarvisEvo addresses the first problem through **interleaved Multimodal Chain-of-Thought (iMCoT)**, which tightly integrates visual observations with the reasoning process. Rather than reasoning only from textual descriptions, the agent can directly consider intermediate visual states while deciding what to do next.

To address reward hacking and enable self-improvement, JarvisEvo further introduces **Synergistic Editor-Evaluator Policy Optimization (SEPO)**. The Editor and Evaluator improve jointly, forming a closed loop of **editing → evaluation → reflection → refinement**.

Through its integration with Adobe Lightroom, JarvisEvo supports both global and local fine-grained editing, advancing intelligent image editing from passive instruction execution toward agents capable of **visual reasoning, self-evaluation, tool selection, reflection, and iterative self-improvement**.

### 中文简介

**JarvisEvo** 是一个具有**自我演化能力的智能图像编辑 Agent**，其整体工作方式模拟专业设计师在实际修图过程中的行为：理解任务、选择工具、执行编辑、观察结果、评价当前效果，并根据评价结果持续反思和优化后续操作。

针对现有智能编辑 Agent 中存在的两个关键问题，JarvisEvo 提出了对应解决方案。

首先，纯文本 Chain-of-Thought 在复杂视觉编辑任务中容易受到信息瓶颈影响，从而产生指令理解偏差或视觉事实错误。为此，JarvisEvo 提出了 **iMCoT（Interleaved Multimodal Chain-of-Thought）**，将视觉观察与推理过程交错结合，使智能体能够直接依据当前图像状态进行推理和决策。

其次，针对基于固定 Reward Model 的策略优化可能产生的 Reward Hacking 问题，JarvisEvo 提出了 **SEPO（Synergistic Editor-Evaluator Policy Optimization）**。Editor 与 Evaluator 在统一框架中协同优化，使 Agent 能够通过“**编辑—评价—反思—改进**”的闭环实现持续自我提升。

此外，JarvisEvo 与 Adobe Lightroom 集成，可同时支持全局调整和局部精细编辑。

该项目推动智能图像编辑从“一次执行用户指令”的模式进一步发展为具有**视觉推理、自我评价、自我反思和持续优化能力的 Self-Evolving Creative Agent**。

---

<a id="jarvisx-cowork"></a>

## JarvisX-Cowork

### A Personal AI Creative Assistant for End-to-End Creative Workflows

<table>
<tr>
<td width="31%" align="center">

<img src="jarvisx-cowork.png" width="100%" alt="JarvisX-Cowork">

</td>

<td width="69%">

**Status:** Demo / Open-source Project  
**Type:** Personal multimodal creative assistant  
**Task:** End-to-end AI-assisted creative workflows  
**Research Direction:** Human-AI creative collaboration  

**Keywords:**  
Creative Agent · AI Cowork · Multimodal Assistant · Human-AI Collaboration · End-to-End Workflow

**Links:**  
[Code](https://github.com/LYL1015/JarvisX-Cowork) /
[Demo Video](https://youtu.be/SiNsTmGbWlo)

### Highlights

- Provides a personal AI creative assistant for complete end-to-end workflows.
- Goes beyond isolated prompt-response interactions.
- Supports multiple stages of a creative project rather than only a single generation task.
- Combines multimodal understanding, content generation, organization, and workflow assistance.
- Explores AI as a persistent **creative coworker** rather than a single-purpose generation tool.

</td>
</tr>
</table>

### English Introduction

**JarvisX-Cowork** is a personal AI creative assistant designed to support **end-to-end creative workflows**.

Conventional AI tools typically perform isolated tasks such as generating one image, answering one question, or producing one piece of text. Real creative work, however, usually involves a much longer sequence of interconnected stages.

A typical workflow may include discovering inspiration, collecting references, organizing materials, developing concepts, creating visual assets, revising intermediate results, and assembling a final deliverable.

JarvisX-Cowork explores how an AI agent can participate throughout this complete process rather than appearing only at a single generation step.

The project therefore positions AI as a persistent **creative coworker**. By combining multimodal understanding, agentic interaction, content generation, and workflow support, JarvisX-Cowork explores how personal AI systems can collaborate with users throughout longer, more complex, and more realistic creative tasks.

### 中文简介

**JarvisX-Cowork** 是一个面向个人用户的 **AI 创意协作助手（Personal AI Creative Assistant）**，主要目标是让 AI 真正参与完整的端到端创作流程。

传统生成式 AI 工具通常只能完成某一个孤立环节，例如生成一张图片、回答一个问题或生成一段文字。但真实创作过程往往由多个相互关联的阶段组成，包括灵感寻找、参考资料收集、内容构思、素材组织、视觉内容生成、中间结果修改以及最终作品整理。

JarvisX-Cowork 尝试将 Agent 能力融入这一完整流程，使 AI 不再只是一个偶尔调用的生成工具，而是能够在不同创作阶段持续协助用户完成任务的 **Personal AI Coworker**。

因此，该项目重点探索 **Human-AI Creative Collaboration**：如何让多模态 Agent 从传统的单一功能工具进一步发展为能够理解创作上下文、参与多阶段任务并长期协助用户完成复杂目标的智能协作者。

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
- Understands natural-language user intentions and imitates the reasoning process of professional artists.
- Coordinates more than **200 Adobe Lightroom retouching tools**.
- Uses two-stage training with Chain-of-Thought supervised fine-tuning and **GRPO-R**.
- Introduces the **Agent-to-Lightroom Protocol** for seamless interaction with Lightroom.
- Proposes **MMArt-Bench**, constructed from real-world user editing scenarios.
- Supports fine-grained global and local image adjustment.
- Demonstrates strong generalization, controllability, and user-friendly interaction.

</td>
</tr>
</table>

### English Introduction

**JarvisArt** is an intelligent **photo-retouching agent** designed to bridge high-level human artistic intentions and professional image-editing operations.

Professional software such as Adobe Lightroom provides powerful editing capabilities, but effective use requires substantial technical expertise, artistic judgment, and manual effort. Existing AI editing systems offer greater automation, but often suffer from limited controllability and insufficient generalization for diverse and personalized editing requirements.

JarvisArt addresses this gap using a **Multimodal Large Language Model (MLLM)-driven agent**. The system understands natural-language user intent, analyzes visual content, imitates the reasoning process of professional artists, and intelligently coordinates more than **200 retouching tools in Adobe Lightroom**.

The model adopts a two-stage training strategy. First, Chain-of-Thought supervised fine-tuning establishes fundamental visual reasoning and tool-use skills. It then applies **Group Relative Policy Optimization for Retouching (GRPO-R)** to further improve editing decisions and professional tool proficiency.

JarvisArt also introduces the **Agent-to-Lightroom Protocol**, enabling seamless interaction between the intelligent agent and Lightroom.

To evaluate professional photo-retouching performance, the project introduces **MMArt-Bench**, a benchmark constructed from real-world editing scenarios.

Overall, JarvisArt demonstrates how multimodal agents can serve as professional creative collaborators, translating abstract artistic intentions into **controllable, fine-grained, and executable photo-retouching operations**.

### 中文简介

**JarvisArt** 是一个面向专业照片修饰场景的**智能修图 Agent**，旨在解决用户高层艺术意图与专业图像编辑操作之间存在的巨大鸿沟。

Adobe Lightroom 等专业软件虽然具有非常丰富的编辑能力，但用户通常需要掌握大量参数、专业工具和视觉设计知识，才能将自己的审美需求转换为具体操作。传统 AI 图像编辑系统虽然提高了自动化程度，却往往存在可控性不足、泛化能力有限以及难以满足复杂个性化需求等问题。

JarvisArt 采用 **MLLM 驱动的 Agent 架构**。智能体能够理解用户自然语言中的编辑需求，同时分析输入图像，并模仿专业艺术家的推理过程，在 Adobe Lightroom 中智能协调超过 **200 个专业修图工具**。

在训练方面，JarvisArt 采用两阶段方案：首先通过 Chain-of-Thought 监督微调获得基础视觉推理和工具调用能力；随后使用专门针对修图任务设计的 **GRPO-R（Group Relative Policy Optimization for Retouching）**进一步提升决策能力和工具使用水平。

此外，项目提出 **Agent-to-Lightroom Protocol**，实现 Agent 与 Lightroom 之间的无缝交互，并构建来自真实用户编辑场景的 **MMArt-Bench** 作为专业修图评测基准。

JarvisArt 展示了多模态智能体作为专业创意协作者的可能性，使 AI 能够将抽象艺术意图转化为**细粒度、可控且真正可以在专业软件中执行的图像编辑操作**。

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
**Method Type:** Intelligent image-restoration agent  
**Task:** Image restoration for robust autonomous-driving perception  

**Authors:**  
Yunlong Lin, Zixu Lin, Haoyu Chen, Panwang Pan, Chenxin Li, Sixiang Chen, Wen Kairun, Yeying Jin, Wenbo Li, Xinghao Ding

**Links:**  
[Project](https://cvpr2025-jarvisir.github.io/) /
[Paper](https://lyl1015.github.io/papers/CVPR2025_JarvisIR.pdf) /
[Code](https://github.com/LYL1015/JarvisIR) /
[Hugging Face Demo](https://huggingface.co/spaces/LYL1015/JarvisIR)

### Highlights

- Published at **CVPR 2025**.
- Introduces an intelligent image-restoration agent for autonomous-driving perception.
- Targets diverse real-world degradation and adverse visual conditions.
- Uses intelligent analysis and decision-making to coordinate appropriate restoration capabilities.
- Connects low-level image restoration with high-level downstream visual perception.
- Explores an **agent-oriented restoration paradigm** instead of relying on one fixed restoration model.

</td>
</tr>
</table>

### English Introduction

**JarvisIR** explores intelligent image restoration from an **agent-oriented perspective**, with the goal of improving visual perception in autonomous-driving scenarios.

Real-world autonomous systems frequently encounter degraded visual inputs caused by challenging environments and imaging conditions. These degradations reduce image quality and can consequently affect downstream perception tasks.

Traditional image-restoration methods typically rely on fixed models designed for specific degradation types. In contrast, JarvisIR introduces intelligent analysis and decision-making into the restoration workflow.

The system can analyze the degradation condition of an input image and coordinate appropriate restoration capabilities according to the observed visual problem.

This transforms image restoration from a fixed low-level processing pipeline into a more flexible and adaptive intelligent workflow.

By connecting restoration decisions with autonomous-driving perception requirements, JarvisIR establishes a bridge between **low-level image enhancement and restoration** and **high-level visual perception**.

The work was published at the **IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2025**.

### 中文简介

**JarvisIR** 是一个面向自动驾驶视觉感知场景的**智能图像恢复 Agent**，发表于 **CVPR 2025**。该项目重点研究复杂现实环境中的图像退化问题，以及智能图像恢复如何提升自动驾驶视觉系统的可靠性。

现实中的自动驾驶车辆可能遇到多种复杂成像和环境条件。这些视觉退化不仅会降低图像本身的质量，还可能进一步影响目标检测、场景理解以及其他下游视觉感知任务。

传统图像恢复方法通常针对某一种特定退化类型设计固定模型，而 JarvisIR 则从 **Agent-Oriented Image Restoration** 的角度重新组织整个恢复流程。

系统能够主动分析当前输入图像所面临的退化状态，并根据不同问题协调相应的恢复能力，从而形成更加灵活和自适应的智能恢复流程。

因此，JarvisIR 不再将图像恢复视为完全独立的低层视觉任务，而是进一步探索如何将**低层图像恢复与高层自动驾驶视觉感知相结合**，为复杂真实环境中的智能视觉系统提供更加可靠的视觉输入。

---

<div align="center">

## SmartDSP Lab

### From Intelligent Visual Restoration to Canvas-Native Creative Agents

**JarvisIR → JarvisArt → JarvisEvo → JarvisX-Cowork → JarvisHub**

<br>

Exploring **multimodal agents, intelligent visual systems, human-AI collaboration,  
creative AI, and long-horizon multimodal workflows**.

<br><br>

<sub>SmartDSP Lab · Datasets · Benchmarks · Publications · Open-source Research Projects</sub>

</div>
