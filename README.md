# SmartDSP Jarvis Projects

A curated collection of research projects from **SmartDSP Lab** on multimodal agents, 
creative AI, intelligent image editing, image restoration, and human-AI collaboration.

---

## Summary

| Project | Research Direction | Type | Main Focus | Resources |
|---|---|---|---|---|
| **JarvisHub** | Multimodal Creative Agents | Canvas-native agent framework | Long-horizon creative workflows and canvas-native agent interaction | [Project](https://www.jarvishub.site/) / [Paper](https://arxiv.org/abs/2607.23588) / [Code](https://github.com/LYL1015/JarvisHub) / [HF](https://huggingface.co/papers/2607.23588) |
| **JarvisEvo** | Intelligent Photo Editing | Self-evolving multimodal agent | Editor-Evaluator optimization and iterative self-improvement | [Project](https://jarvisevo.vercel.app/) / [Paper](https://arxiv.org/abs/2511.23002) / [Code](https://github.com/LYL1015/JarvisEvo) / [HF](https://huggingface.co/papers/2511.23002) |
| **JarvisX-Cowork** | Creative AI Assistant | Personal multimodal creative agent | End-to-end human-AI creative workflows | [Code](https://github.com/LYL1015/JarvisX-Cowork) / [Demo](https://youtu.be/SiNsTmGbWlo) |
| **JarvisArt** | Intelligent Photo Retouching | Multimodal photo-retouching agent | Translating artistic intentions into professional editing operations | [Project](https://jarvisart.vercel.app/) / [Paper](https://arxiv.org/abs/2506.17612) / [Code](https://github.com/LYL1015/JarvisArt) / [Video](https://www.youtube.com/watch?v=Ol28DQj8wV8) |
| **JarvisIR** | Intelligent Image Restoration | Vision-language-driven restoration agent | Image restoration for robust autonomous-driving perception | [Project](https://cvpr2025-jarvisir.github.io/) / [Paper](https://lyl1015.github.io/papers/CVPR2025_JarvisIR.pdf) / [Code](https://github.com/LYL1015/JarvisIR) / [Demo](https://huggingface.co/spaces/LYL1015/JarvisIR) |

---

## Projects
### JarvisHub: An Open Harness for Canvas-Native Creative Agents

<table>
<tr>
<td width="31%" align="center">

<img src="assets/jarvishub.jpg" width="100%" alt="JarvisHub">

</td>
<td width="69%">

**Project:** JarvisHub: An Open Harness for Canvas-Native Creative Agents  
**Research Direction:** Multimodal Creative Agents  
**Type:** Canvas-native multimodal agent framework  
**Task:** Long-horizon multimodal creative workflows  
**Keywords:** Canvas-Native Agent; Multimodal Agent; Creative AI; Tool Orchestration  
**Links:** [Project](https://www.jarvishub.site/) / [Paper](https://arxiv.org/abs/2607.23588) / [Code](https://github.com/LYL1015/JarvisHub) / [Hugging Face](https://huggingface.co/papers/2607.23588)

**Highlights**

- Introduces a canvas-native paradigm for multimodal creative agents.
- Uses a persistent visual workspace to support long-horizon creative tasks.
- Enables agents to organize and manipulate heterogeneous multimodal content.
- Explores the transition from conversational assistants to workspace-native creative agents.

</td>
</tr>
</table>

**English Introduction:**  
JarvisHub is an open harness for building and studying **canvas-native creative agents**. 
Instead of limiting human-AI interaction to conventional text-based conversations, JarvisHub 
places a persistent visual canvas at the center of the agent workflow. The canvas provides a 
unified workspace where multimodal content can be organized, manipulated, and continuously 
updated throughout long-horizon creative tasks. This design allows intelligent agents to move 
beyond isolated question-answer interactions and participate in persistent, iterative creative 
processes. JarvisHub therefore provides a platform for exploring a new generation of 
workspace-native multimodal agents capable of supporting complex creative workflows.

**中文简介：**  
JarvisHub 是一个面向 **Canvas-Native Creative Agents（画布原生创意智能体）** 的开放式框架，
旨在研究多模态智能体如何在统一的视觉工作空间中完成复杂、长期且持续演化的创作任务。
与传统以聊天窗口为核心的 AI Assistant 不同，JarvisHub 将可持续编辑的 Canvas 置于智能体
工作流程的核心，使多模态内容能够在统一空间中进行组织、操作和持续更新。借助这一机制，
智能体不再局限于完成单次问答或孤立任务，而能够围绕持续存在的工作空间参与长期、多阶段的
创作过程。JarvisHub 进一步探索了 AI 从传统对话式助手向 Workspace-Native / Canvas-Native
Multimodal Agent 演进的新型智能体范式。

---
### JarvisEvo: Towards a Self-Evolving Photo Editing Agent with Synergistic Editor-Evaluator Optimization

<table>
<tr>
<td width="31%" align="center">

<img src="assets/jarvisevo.jpg" width="100%" alt="JarvisEvo">

</td>
<td width="69%">

**Paper:** JarvisEvo: Towards a Self-Evolving Photo Editing Agent with Synergistic Editor-Evaluator Optimization  
**Research Direction:** Intelligent Photo Editing  
**Type:** Self-evolving multimodal editing agent  
**Task:** Autonomous and iterative photo editing  
**Keywords:** Self-Evolving Agent; Photo Editing; Multimodal Reasoning; Editor-Evaluator  
**Links:** [Project](https://jarvisevo.vercel.app/) / [Paper](https://arxiv.org/abs/2511.23002) / [PDF](https://arxiv.org/pdf/2511.23002) / [Code](https://github.com/LYL1015/JarvisEvo) / [Hugging Face](https://huggingface.co/papers/2511.23002)

**Highlights**

- Explores self-evolving intelligence for autonomous photo editing.
- Builds a collaborative Editor-Evaluator optimization paradigm.
- Integrates editing, evaluation, reasoning, and iterative refinement.
- Moves beyond one-shot editing toward self-improving creative agents.

</td>
</tr>
</table>

**English Introduction:**  
JarvisEvo investigates a **self-evolving photo editing agent** that moves beyond conventional 
one-shot instruction following. Its central idea is to establish a synergistic interaction between 
an Editor, which performs image-editing operations, and an Evaluator, which assesses the quality 
of the editing results. Through iterative editing, evaluation, and refinement, the agent can 
progressively improve its outputs and editing behavior. This paradigm advances intelligent photo 
editing from passive instruction execution toward autonomous creative agents equipped with 
evaluation and self-improvement capabilities.

**中文简介：**  
JarvisEvo 面向具有**自我演化能力的智能图像编辑 Agent**，探索如何突破传统“一次指令、
一次编辑”的工作方式。其核心思想是构建 Editor-Evaluator 协同优化机制：Editor 负责执行
具体的图像编辑操作，Evaluator 则负责评价当前编辑结果，两者共同形成“编辑—评价—优化”的
迭代闭环。通过这一机制，智能体不仅能够完成编辑任务，还能够根据评价结果进一步调整和改善
输出。JarvisEvo 将智能图像编辑从被动执行用户指令进一步推进到具有评价、反思和持续优化能力
的自主 Creative Agent 范式。

---
### JarvisX-Cowork: A Personal AI Creative Assistant for End-to-End Creative Workflows

<table>
<tr>
<td width="31%" align="center">

<img src="assets/jarvisx-cowork.jpg" width="100%" alt="JarvisX-Cowork">

</td>
<td width="69%">

**Project:** JarvisX-Cowork: A Personal AI Creative Assistant for End-to-End Creative Workflows  
**Research Direction:** Human-AI Creative Collaboration  
**Type:** Personal multimodal creative assistant  
**Task:** End-to-end AI-assisted creative workflows  
**Keywords:** AI Cowork; Creative Assistant; Multimodal Agent; Human-AI Collaboration  
**Links:** [Code](https://github.com/LYL1015/JarvisX-Cowork) / [Demo Video](https://youtu.be/SiNsTmGbWlo)

**Highlights**

- Provides a personal AI assistant for end-to-end creative workflows.
- Extends AI assistance beyond isolated prompt-response interactions.
- Supports multi-stage creative processes within an integrated workspace.
- Explores AI as a persistent creative collaborator rather than a single-purpose tool.

</td>
</tr>
</table>

**English Introduction:**  
JarvisX-Cowork is a personal AI creative assistant designed to support **end-to-end creative 
workflows**. Real-world creation typically involves multiple stages, including inspiration 
collection, planning, material organization, content generation, revision, and final assembly. 
Instead of assisting with only an isolated step, JarvisX-Cowork explores how an AI agent can 
participate throughout this complete process. The project represents a shift from task-specific 
AI tools toward persistent personal AI coworkers capable of collaborating with users across 
longer and more complex creative workflows.

**中文简介：**  
JarvisX-Cowork 是一个面向个人用户的 **AI 创意协作助手**，重点探索 AI 如何参与端到端的
完整创作流程。现实中的创作任务往往包含灵感收集、内容构思、素材整理、内容生成、修改完善
以及最终成果组织等多个阶段，而传统 AI 工具通常只负责其中某一个孤立环节。
JarvisX-Cowork 希望让 AI Agent 更深入地参与整个创作过程，使其从单一的内容生成工具逐步
发展成为能够持续参与复杂创作任务的 Personal AI Coworker，从而探索更加自然和高效的
Human-AI Creative Collaboration 模式。

---
### JarvisArt: Liberating Human Artistic Creativity via an Intelligent Photo Retouching Agent

<table>
<tr>
<td width="31%" align="center">

<img src="assets/jarvisart.jpg" width="100%" alt="JarvisArt">

</td>
<td width="69%">

**Paper:** JarvisArt: Liberating Human Artistic Creativity via an Intelligent Photo Retouching Agent  
**Research Direction:** Intelligent Photo Retouching  
**Type:** Multimodal photo-retouching agent  
**Task:** Professional AI-assisted photo retouching  
**Keywords:** Photo Retouching; Multimodal Agent; Creative AI; Image Editing  
**Links:** [Project](https://jarvisart.vercel.app/) / [Paper](https://arxiv.org/abs/2506.17612) / [Code](https://github.com/LYL1015/JarvisArt) / [Hugging Face](https://huggingface.co/papers/2506.17612)

**Highlights**

- Bridges high-level artistic intentions and professional photo-editing operations.
- Uses multimodal understanding and reasoning to assist photo retouching.
- Reduces the technical barrier of professional image-editing workflows.
- Positions AI as a creative collaborator while preserving human artistic control.

</td>
</tr>
</table>

**English Introduction:**  
JarvisArt is an intelligent **photo retouching agent** designed to bridge high-level human artistic 
intentions and professional image-editing operations. Professional retouching requires both 
technical knowledge and artistic judgment, making it difficult for non-expert users to translate 
creative ideas into low-level editing parameters. JarvisArt explores how multimodal understanding 
and agentic reasoning can interpret visual content and user intentions, formulate appropriate 
editing strategies, and assist users throughout professional retouching workflows. Rather than 
replacing human creativity with one-shot generation, JarvisArt positions AI as an intelligent 
creative collaborator that helps users realize their artistic intentions.

**中文简介：**  
JarvisArt 是一个面向专业照片修饰场景的**智能修图 Agent**，旨在建立用户高层艺术意图与
专业图像编辑操作之间的桥梁。传统专业修图不仅需要掌握大量图像编辑参数，还需要一定的视觉
审美和专业经验。JarvisArt 利用多模态理解与智能体推理能力，对输入图像和用户编辑意图进行
分析，并将较为抽象的艺术需求转换为具体的编辑策略和操作。与直接生成最终图像的方法不同，
JarvisArt 更强调 AI 对人类创作过程的辅助作用，使 AI 成为专业照片修饰过程中的智能助手和
创意协作者，在降低专业编辑门槛的同时保留用户自身的艺术表达。

**More Resources:**  
[X / Twitter](https://x.com/ling_yunlong/status/1940010865627103419) /
[YouTube](https://www.youtube.com/watch?v=Ol28DQj8wV8) /
[Bilibili](https://www.bilibili.com/video/BV1Sd3nzREvP)

---
### JarvisIR: Elevating Autonomous Driving Perception with Intelligent Image Restoration

<table>
<tr>
<td width="31%" align="center">

<img src="assets/jarvisir.jpg" width="100%" alt="JarvisIR">

</td>
<td width="69%">

**Paper:** JarvisIR: Elevating Autonomous Driving Perception with Intelligent Image Restoration  
**Research Direction:** Intelligent Image Restoration  
**Type:** Vision-language-driven image restoration agent  
**Task:** Image restoration for robust autonomous-driving perception  
**Application:** Autonomous driving under challenging visual conditions  
**Keywords:** Image Restoration; Autonomous Driving; Multimodal Agent; Visual Perception  
**Links:** [Project](https://cvpr2025-jarvisir.github.io/) / [Paper](https://lyl1015.github.io/papers/CVPR2025_JarvisIR.pdf) / [Code](https://github.com/LYL1015/JarvisIR) / [Demo](https://huggingface.co/spaces/LYL1015/JarvisIR)

**Highlights**

- Introduces an agent-oriented formulation for intelligent image restoration.
- Targets challenging visual conditions in autonomous-driving scenarios.
- Uses intelligent reasoning to analyze degradation and coordinate restoration capabilities.
- Connects low-level image restoration with downstream high-level visual perception.

</td>
</tr>
</table>

**English Introduction:**  
JarvisIR investigates intelligent image restoration from an **agent-oriented perspective**, with 
particular attention to robust visual perception in autonomous-driving scenarios. Real-world 
visual systems may encounter diverse image degradations under challenging environmental and 
imaging conditions, potentially affecting downstream perception performance. Instead of treating 
restoration as a single fixed transformation, JarvisIR introduces intelligent analysis and 
decision-making into the restoration process, allowing the system to coordinate restoration 
capabilities according to the observed visual degradation. The project provides a bridge between 
low-level image restoration and high-level autonomous-driving perception.

**中文简介：**  
JarvisIR 是一个面向自动驾驶视觉感知场景的**智能图像恢复 Agent**，重点研究复杂视觉环境
中的图像退化以及智能恢复对下游感知任务的帮助。在真实自动驾驶场景中，视觉系统可能面临
多种复杂成像条件，这些退化会降低输入图像质量，并进一步影响后续视觉感知任务。
JarvisIR 从 Agent 的角度重新思考图像恢复问题，使系统能够分析当前图像的视觉状态，并根据
退化情况协调相应的恢复能力，从而形成更加灵活和自适应的智能恢复流程。该项目进一步探索了
低层图像恢复与自动驾驶高层视觉感知之间的联系。

---
