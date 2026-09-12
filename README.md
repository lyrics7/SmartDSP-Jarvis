<div align="center">

# SmartDSP · Jarvis Project Gallery

### Multimodal Agents · Creative AI · Intelligent Image Editing · Image Restoration

A curated collection of featured research projects from **SmartDSP Lab**,  
covering canvas-native multimodal agents, self-evolving photo editing agents,  
creative AI assistants, intelligent photo retouching, and image restoration.

<br>

[**JarvisHub**](#jarvishub-an-open-harness-for-canvas-native-multimodal-creative-agents) ·
[**JarvisEvo**](#jarvisevo-towards-a-self-evolving-photo-editing-agent-with-synergistic-editor-evaluator-optimization) ·
[**JarvisX-Cowork**](#jarvisx-cowork-a-personal-ai-creative-assistant-for-end-to-end-creative-workflows) ·
[**JarvisArt**](#jarvisart-liberating-human-artistic-creativity-via-an-intelligent-photo-retouching-agent) ·
[**JarvisIR**](#jarvisir-elevating-autonomous-driving-perception-with-intelligent-image-restoration)

</div>

---

# Summary

| Year | Project | Method Type | Authors | Venue / Status | Links |
|---|---|---|---|---|---|
| 2026 | **JarvisHub: An Open Harness for Canvas-Native Multimodal Creative Agents** | Canvas-native multimodal creative agent framework | Yunlong Lin et al. | arXiv 2026 | [Project](https://www.jarvishub.site/) / [Paper](https://arxiv.org/abs/2607.23588) / [Code](https://github.com/LYL1015/JarvisHub) / [HF](https://huggingface.co/papers/2607.23588) |
| 2025 | **JarvisEvo: Towards a Self-Evolving Photo Editing Agent with Synergistic Editor-Evaluator Optimization** | Self-evolving multimodal editing agent | Yunlong Lin et al. | arXiv 2025 | [Project](https://jarvisevo.vercel.app/) / [Paper](https://arxiv.org/abs/2511.23002) / [Code](https://github.com/LYL1015/JarvisEvo) / [HF](https://huggingface.co/papers/2511.23002) |
| — | **JarvisX-Cowork: A Personal AI Creative Assistant for End-to-End Creative Workflows** | Personal multimodal creative assistant | — | Demo / Project | [Code](https://github.com/LYL1015/JarvisX-Cowork) / [Demo](https://youtu.be/SiNsTmGbWlo) |
| 2025 | **JarvisArt: Liberating Human Artistic Creativity via an Intelligent Photo Retouching Agent** | MLLM-driven intelligent photo retouching agent | Yunlong Lin et al. | arXiv 2025 | [Project](https://jarvisart.vercel.app/) / [Paper](https://arxiv.org/abs/2506.17612) / [Code](https://github.com/LYL1015/JarvisArt) / [HF](https://huggingface.co/papers/2506.17612) |
| 2025 | **JarvisIR: Elevating Autonomous Driving Perception with Intelligent Image Restoration** | Intelligent image restoration agent | Yunlong Lin et al. | CVPR 2025 | [Project](https://cvpr2025-jarvisir.github.io/) / [Paper](https://lyl1015.github.io/papers/CVPR2025_JarvisIR.pdf) / [Code](https://github.com/LYL1015/JarvisIR) / [Demo](https://huggingface.co/spaces/LYL1015/JarvisIR) |

---

# JarvisHub: An Open Harness for Canvas-Native Multimodal Creative Agents

<table>
<tr>
<td width="31%" align="center">

<img src="assets/jarvishub.jpg" width="100%" alt="JarvisHub">

</td>

<td width="69%">

**Year:** 2026  
**Venue / Status:** arXiv, Computer Vision and Pattern Recognition (cs.CV)  
**Submitted:** July 26, 2026  
**Method Type:** Canvas-native multimodal creative agent framework  
**Task:** Long-horizon multimodal creative production and workflow orchestration  
**Authors:** Yunlong Lin, Zixu Lin, Zhaohu Xing, Biqiang Li, Chenxin Li, Haonan Wang, Haitao Wu, Hengyu Liu, Jianghai Chen, Kaituo Feng, Kaixin Li, Shawn Chen, Shijue Huang, Sixiang Chen, Tsung-Yi Ho, Wenxuan Huang, Xiangyan Liu, Xiaomeng Hu, Xuanhua He, Yan Sun, Yunqing Zhao, Zhiqin Yang, Zehan Wang, Zhengyang Tang, Tianyu Pang, Xiangyu Yue  

**Links:**  
[Project](https://www.jarvishub.site/) /
[Paper](https://arxiv.org/abs/2607.23588) /
[Code](https://github.com/LYL1015/JarvisHub) /
[Hugging Face](https://huggingface.co/papers/2607.23588)

**Highlights**

- Introduces a **canvas-native creative agent harness** for long-horizon multimodal creation.
- Treats the editable canvas as the user workspace, external memory, action space, and shared project state.
- Represents multimodal artifacts, dependencies, versions, and user feedback using typed canvas nodes and links.
- Employs a three-layer architecture consisting of canvas state, protocol bridge, and agent runtime.
- Enables agents to progressively plan, generate, revise, organize, and maintain complex multimodal projects.
- Preserves human steerability by allowing users to inspect, guide, modify, and intervene throughout the creative process.

</td>
</tr>
</table>

**English Introduction:**  
JarvisHub is an open harness designed for **canvas-native multimodal creative agents** and long-horizon creative production. Modern generative models are already capable of producing high-quality images, videos, audio, slides, webpages, UI components, and other creative assets, but real creative work rarely consists of isolated prompt-output interactions. Instead, a project usually evolves through references, drafts, alternatives, edits, failures, version relationships, tool actions, evaluations, and human feedback.

JarvisHub addresses this limitation by placing an editable visual canvas at the center of the agent workflow. The canvas is not merely an interface; it simultaneously functions as the agent's external memory, action space, and persistent shared project state. Multimodal artifacts and their relationships are represented explicitly through typed nodes and links, allowing the agent to preserve contextual information across a long creative process.

Through its canvas-state, protocol-bridge, and agent-runtime architecture, JarvisHub allows creative agents to operate inside an inspectable and editable workspace. This shifts multimodal AI from isolated tool invocation toward sustained, human-steerable creative automation, where agents can continuously plan, generate, revise, organize, and maintain complex creative projects.

**中文简介：**  
JarvisHub 是一个面向 **Canvas-Native Multimodal Creative Agents（画布原生多模态创意智能体）** 的开放式智能体框架，主要研究 AI 如何完成长周期、多阶段的复杂多模态创作任务。

当前图像、视频、音频、网页和演示文稿等生成模型已经具有较强的单次内容生成能力，但真实创作过程通常并不是简单的“输入 Prompt—生成结果”。一个完整项目往往还包含参考资料、多个草稿、候选方案、修改过程、失败尝试、版本关系、工具操作、评价信号以及用户反馈等大量持续演化的状态。

JarvisHub 将**可编辑 Canvas** 作为整个系统的核心。Canvas 不仅承担用户交互界面的作用，同时还充当智能体的外部记忆、操作空间以及共享项目状态。不同的多模态内容、版本关系、依赖关系以及用户反馈均可以通过结构化节点和连接进行表示。

通过 Canvas State、Protocol Bridge 和 Agent Runtime 三层架构，JarvisHub 使智能体能够在一个透明、可查看、可修改的创意状态中持续工作。用户可以随时查看 Agent 的中间结果，并对其进行指导和干预，从而推动 Creative AI 从传统的单次内容生成进一步发展为**可持续规划、生成、修改和组织复杂项目的长周期创作智能体**。

---

# JarvisEvo: Towards a Self-Evolving Photo Editing Agent with Synergistic Editor-Evaluator Optimization

<table>
<tr>
<td width="31%" align="center">

<img src="assets/jarvisevo.jpg" width="100%" alt="JarvisEvo">

</td>

<td width="69%">

**Year:** 2025  
**Venue / Status:** arXiv, Computer Vision and Pattern Recognition (cs.CV)  
**First Submitted:** November 28, 2025  
**Method Type:** Self-evolving multimodal photo editing agent  
**Task:** Iterative intelligent photo editing and self-improvement  
**Authors:** Yunlong Lin, Linqing Wang, Kunjie Lin, Zixu Lin, Kaixiong Gong, Wenbo Li, Bin Lin, Zhenxi Li, Shiyi Zhang, Yuyang Peng, Wenxun Dai, Xinghao Ding, Chunyu Wang, Qinglin Lu  

**Links:**  
[Project](https://jarvisevo.vercel.app/) /
[Paper](https://arxiv.org/abs/2511.23002) /
[PDF](https://arxiv.org/pdf/2511.23002) /
[Code](https://github.com/LYL1015/JarvisEvo) /
[Hugging Face](https://huggingface.co/papers/2511.23002)

**Highlights**

- Introduces a unified image editing agent that imitates the iterative workflow of a professional human designer.
- Proposes **interleaved Multimodal Chain-of-Thought (iMCoT)** reasoning.
- Introduces **Synergistic Editor-Evaluator Policy Optimization (SEPO)** for self-improvement without external rewards.
- Addresses instruction hallucination and reward-hacking problems in agent-based image editing.
- Supports both global and local fine-grained image editing.
- Integrates Adobe Lightroom into the agent workflow.
- Achieves strong performance on ArtEdit-Bench, including improved preservative editing and pixel-level content fidelity.

</td>
</tr>
</table>

**English Introduction:**  
JarvisEvo is a unified **self-evolving photo editing agent** designed to emulate how an expert human designer edits, evaluates, and progressively improves visual content. Existing editing agents have improved interaction and automation, but they still face important problems such as instruction hallucination and reward hacking. Text-only reasoning may lose critical visual information, while optimization against static reward models may cause an editing policy to exploit weaknesses in the reward function.

To address these issues, JarvisEvo introduces an **interleaved Multimodal Chain-of-Thought (iMCoT)** reasoning mechanism that tightly couples visual observations with the agent's reasoning process. This improves instruction following and allows the agent to reason directly over intermediate visual states rather than relying purely on textual descriptions.

JarvisEvo further proposes **Synergistic Editor-Evaluator Policy Optimization (SEPO)**. Instead of depending entirely on external static reward models, the Editor and Evaluator improve together, creating a self-improvement mechanism in which the agent can edit an image, assess the result, reflect on the current decision, and refine the output.

Through integration with Adobe Lightroom, JarvisEvo supports both global and local fine-grained editing. The project therefore advances image-editing agents from simple instruction executors toward systems capable of visual reasoning, self-evaluation, reflection, tool selection, and iterative self-improvement.

**中文简介：**  
JarvisEvo 是一个具有**自我演化能力的智能图像编辑 Agent**，其整体工作方式模拟专业设计师在实际修图过程中的行为：分析任务、选择工具、执行编辑、观察结果、评价当前效果，并根据评价结果不断反思和优化后续操作。

针对现有智能编辑 Agent 中存在的两类重要问题，JarvisEvo 提出了新的解决方案。首先，纯文本 Chain-of-Thought 在复杂视觉编辑任务中容易受到信息瓶颈影响，从而产生指令理解错误或事实性偏差。为此，JarvisEvo 提出了 **iMCoT（Interleaved Multimodal Chain-of-Thought）**，将视觉观察与推理过程交错结合，使智能体能够直接依据图像中间状态进行推理和决策。

其次，针对传统策略优化中可能出现的 Reward Hacking 问题，JarvisEvo 提出了 **SEPO（Synergistic Editor-Evaluator Policy Optimization）**。Editor 和 Evaluator 在统一框架下协同演化，使模型不再完全依赖固定的外部奖励模型，而是能够通过“编辑—评价—反思—改进”的闭环实现持续自我提升。

此外，JarvisEvo 与 Adobe Lightroom 深度集成，可以同时支持全局调整和局部精细编辑。该项目进一步推动智能图像编辑从“一次执行用户指令”发展到具有**视觉推理、自我评价、自我反思和持续优化能力的 Self-Evolving Creative Agent**。

---

# JarvisX-Cowork: A Personal AI Creative Assistant for End-to-End Creative Workflows

<table>
<tr>
<td width="31%" align="center">

<img src="assets/jarvisx-cowork.jpg" width="100%" alt="JarvisX-Cowork">

</td>

<td width="69%">

**Status:** Demo / Open-source Project  
**Type:** Personal multimodal creative assistant  
**Task:** End-to-end AI-assisted creative workflows  
**Research Direction:** Human-AI creative collaboration  
**Keywords:** Creative Agent; AI Cowork; Multimodal Assistant; Human-AI Collaboration; End-to-End Workflow  

**Links:**  
[Code](https://github.com/LYL1015/JarvisX-Cowork) /
[Demo Video](https://youtu.be/SiNsTmGbWlo)

**Highlights**

- Provides a personal AI creative assistant for complete creative workflows.
- Goes beyond isolated prompt-response interactions.
- Supports multiple stages of a creative project rather than a single generation task.
- Combines multimodal understanding, content generation, organization, and workflow assistance.
- Explores a new form of persistent AI coworker for creative users.

</td>
</tr>
</table>

**English Introduction:**  
JarvisX-Cowork is a **personal AI creative assistant** designed to support end-to-end creative workflows. Unlike conventional AI tools that typically perform isolated tasks such as generating a single image, answering a question, or producing a short piece of text, real creative work often involves a long sequence of interconnected stages.

A typical workflow may include searching for inspiration, collecting references, organizing materials, developing ideas, creating visual assets, revising intermediate results, and assembling a final deliverable. JarvisX-Cowork explores how an AI agent can participate throughout this complete workflow rather than appearing only at a single generation step.

The project therefore positions AI as a persistent **creative coworker**. By combining multimodal understanding with agentic interaction and workflow support, JarvisX-Cowork explores how personal AI systems can assist users throughout longer, more complex, and more realistic creative processes.

**中文简介：**  
JarvisX-Cowork 是一个面向个人用户的 **AI 创意协作助手（Personal AI Creative Assistant）**，主要目标是让 AI 参与完整的端到端创作流程。

传统生成式 AI 工具通常只能完成某一个独立环节，例如生成一张图片、回答一个问题或者生成一段文字。但真实的创作过程往往由多个相互关联的阶段组成，包括灵感寻找、参考资料收集、内容构思、素材组织、图像或其他内容生成、中间结果修改以及最终作品整理等。

JarvisX-Cowork 尝试将 Agent 能力融入这一完整工作流，使 AI 不再只是一个单次使用的生成工具，而是能够在不同创作阶段持续协助用户完成任务的 **Personal AI Coworker**。

该项目重点探索 Human-AI Creative Collaboration，即如何让多模态 Agent 从传统的“工具”进一步发展为能够理解创作上下文、参与多阶段任务并持续协助用户完成复杂创作目标的智能协作者。

---

# JarvisArt: Liberating Human Artistic Creativity via an Intelligent Photo Retouching Agent

<table>
<tr>
<td width="31%" align="center">

<img src="assets/jarvisart.gif" width="100%" alt="JarvisArt Demo">

</td>

<td width="69%">

**Year:** 2025  
**Venue / Status:** arXiv, Computer Vision and Pattern Recognition (cs.CV)  
**Submitted:** June 21, 2025  
**Method Type:** MLLM-driven intelligent photo retouching agent  
**Task:** Professional AI-assisted photo retouching  
**Authors:** Yunlong Lin, Zixu Lin, Kunjie Lin, Jinbin Bai, Panwang Pan, Chenxin Li, Haoyu Chen, Zhongdao Wang, Xinghao Ding, Wenbo Li, Shuicheng Yan  

**Links:**  
[Project](https://jarvisart.vercel.app/) /
[Paper](https://arxiv.org/abs/2506.17612) /
[Code](https://github.com/LYL1015/JarvisArt) /
[Hugging Face](https://huggingface.co/papers/2506.17612) /
[YouTube](https://www.youtube.com/watch?v=Ol28DQj8wV8) /
[Bilibili](https://www.bilibili.com/video/BV1Sd3nzREvP)

**Highlights**

- Introduces an MLLM-driven intelligent agent for professional photo retouching.
- Understands user intentions and imitates the reasoning process of professional artists.
- Coordinates more than **200 Adobe Lightroom retouching tools**.
- Uses two-stage training with Chain-of-Thought supervised fine-tuning and **GRPO-R**.
- Introduces the **Agent-to-Lightroom Protocol** for seamless interaction with Lightroom.
- Proposes **MMArt-Bench**, constructed from real-world user edits.
- Supports fine-grained global and local image adjustments.
- Demonstrates strong generalization and user-friendly interaction.

</td>
</tr>
</table>

**English Introduction:**  
JarvisArt is an intelligent **photo retouching agent** designed to bridge high-level human artistic intentions and professional image-editing operations. Professional tools such as Adobe Lightroom provide powerful retouching capabilities, but effective use often requires considerable technical knowledge, artistic judgment, and manual effort. Existing AI-based editing systems offer greater automation, but frequently provide limited controllability and insufficient generalization for diverse personalized editing requirements.

JarvisArt addresses this gap using a **Multimodal Large Language Model (MLLM)-driven agent**. The system understands user intent, analyzes visual content, imitates the reasoning process of professional artists, and intelligently coordinates more than 200 retouching tools available in Lightroom.

The model adopts a two-stage training strategy. First, Chain-of-Thought supervised fine-tuning establishes fundamental visual reasoning and tool-use capabilities. It then applies **Group Relative Policy Optimization for Retouching (GRPO-R)** to further improve editing decisions and tool proficiency. JarvisArt also introduces the **Agent-to-Lightroom Protocol**, enabling direct interaction between the intelligent agent and Lightroom.

To evaluate intelligent retouching performance, the work introduces **MMArt-Bench**, a benchmark based on real-world user editing behavior. Overall, JarvisArt demonstrates how multimodal agents can serve as professional creative collaborators, translating natural-language artistic intentions into controllable and fine-grained photo-retouching operations.

**中文简介：**  
JarvisArt 是一个面向专业照片修饰场景的**智能修图 Agent**，旨在解决用户高层艺术意图与专业图像编辑操作之间存在的巨大鸿沟。

Adobe Lightroom 等专业修图软件虽然提供了非常丰富的功能，但用户通常需要掌握大量参数、专业工具和视觉设计知识，才能将自己的审美需求转换为具体操作。而传统 AI 图像编辑方法虽然提升了自动化程度，却往往存在可控性不足、泛化能力有限以及难以满足个性化需求等问题。

JarvisArt 采用 **MLLM 驱动的 Agent 架构**。智能体能够理解用户自然语言中的编辑需求，同时分析输入图像，并模仿专业艺术家的推理过程，在 Adobe Lightroom 中智能协调超过 **200 个专业修图工具**。

在训练方面，JarvisArt 采用两阶段方案：首先通过 Chain-of-Thought 监督微调获得基础视觉推理与工具调用能力；随后使用专门针对修图任务设计的 **GRPO-R（Group Relative Policy Optimization for Retouching）**进一步提升决策能力和工具使用水平。

此外，项目提出 **Agent-to-Lightroom Protocol**，实现 Agent 与 Lightroom 之间的无缝交互，并构建了来自真实用户编辑过程的 **MMArt-Bench** 作为评测基准。JarvisArt 展示了多模态智能体作为专业创意协作者的可能性，使 AI 能够将抽象艺术意图转化为细粒度、可控且专业的图像编辑操作。

---

# JarvisIR: Elevating Autonomous Driving Perception with Intelligent Image Restoration

<table>
<tr>
<td width="31%" align="center">

<img src="assets/jarvisir.gif" width="100%" alt="Jarvisir">

</td>

<td width="69%">

**Year:** 2025  
**Venue:** IEEE/CVF Conference on Computer Vision and Pattern Recognition (**CVPR 2025**)  
**Publication Date:** June 2025  
**Method Type:** Intelligent image restoration agent  
**Task:** Image restoration for robust autonomous-driving perception  
**Authors:** Yunlong Lin, Zixu Lin, Haoyu Chen, Panwang Pan, Chenxin Li, Sixiang Chen, Wen Kairun, Yeying Jin, Wenbo Li, Xinghao Ding  

**Links:**  
[Project](https://cvpr2025-jarvisir.github.io/) /
[Paper](https://lyl1015.github.io/papers/CVPR2025_JarvisIR.pdf) /
[Code](https://github.com/LYL1015/JarvisIR) /
[Hugging Face Demo](https://huggingface.co/spaces/LYL1015/JarvisIR)

**Highlights**

- Published at **CVPR 2025**.
- Introduces an intelligent image restoration agent for autonomous-driving perception.
- Addresses diverse real-world visual degradation conditions.
- Uses intelligent analysis and decision-making to coordinate appropriate restoration capabilities.
- Connects low-level image restoration with high-level downstream perception.
- Explores an agent-oriented paradigm instead of a single fixed restoration model.

</td>
</tr>
</table>

**English Introduction:**  
JarvisIR explores intelligent image restoration from an **agent-oriented perspective**, with the goal of improving visual perception in autonomous-driving scenarios. Real-world autonomous systems frequently encounter degraded visual inputs caused by challenging environments and imaging conditions. These degradations can reduce image quality and consequently affect downstream perception systems.

Traditional image-restoration methods often rely on fixed models designed for specific degradation types. In contrast, JarvisIR introduces intelligent analysis and decision-making into the restoration workflow. The system can analyze the degradation condition of an input image and coordinate appropriate restoration capabilities according to the observed visual problem.

This transforms image restoration from a fixed low-level processing pipeline into a flexible intelligent workflow. By connecting restoration decisions with autonomous-driving perception requirements, JarvisIR establishes a bridge between **low-level image enhancement and restoration** and **high-level visual perception**.

The work was published at the **IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2025**.

**中文简介：**  
JarvisIR 是一个面向自动驾驶视觉感知场景的**智能图像恢复 Agent**，并发表于 **CVPR 2025**。该项目重点研究复杂现实环境中的图像退化问题，以及智能图像恢复如何提升自动驾驶视觉系统的可靠性。

现实中的自动驾驶车辆可能遇到多种复杂成像条件，这些视觉退化不仅会降低图像本身的质量，还可能进一步影响目标检测、场景理解以及其他下游视觉感知任务。

传统图像恢复方法通常针对某一种退化类型设计固定模型，而 JarvisIR 则从 **Agent-Oriented Image Restoration** 的角度重新组织整个恢复流程。系统能够分析当前输入图像的退化状态，并根据不同情况协调相应的恢复能力，从而形成更加灵活、自适应的智能恢复流程。

因此，JarvisIR 不再将图像恢复视为一个完全独立的低层视觉任务，而是进一步探索如何将**低层图像恢复与高层自动驾驶视觉感知相结合**，为复杂真实环境中的智能视觉系统提供更加可靠的视觉输入。

---

