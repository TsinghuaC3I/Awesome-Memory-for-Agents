# Awesome-Memory-for-Agents

The paper list is maintained by Hongyi Liu, Yu Fu, Kaiyan Zhang, contributed by Yuxin Zuo, Che Jiang, Guoli Jia, Yuru Wang, Kaikai Zhao, Yuchen Fan, Zhenzhao Yuan, Kai Tian, Weizhi Wang.

<div align="center">
    <img src="assets/cover.png" width=60%>
</div>

## Table of Contents

- [Awesome-Memory-for-Agents](#awesome-memory-for-agents)
    - [Table of Contents](#table-of-contents)
    - [Overview](#overview)
    - [Paper List](#paper-list)
        - [Application](#application)
            - [Personalization](#personalization)
            - [Learning from Experience](#learning-from-experience)
            - [Long-horizon Agentic Task](#long-horizon-agentic-task)
        - [Survey](#survey)
        - [Benchmark](#benchmark)
        - [Product & Project](#product--project)

## Overview

This repository provides a curated list of papers on agent memory, structured by a core taxonomy. We first divide agent memory based on its persistence:

- **Short-Term Memory:** Transient information managed within the context window for a single task;
- **Long-Term Memory:** Persistent information stored externally across tasks.

Within *Long-Term Memory*, we further distinguish based on its reliance on task outcomes (success/failure) for curation:

- **Experience** involves knowledge explicitly validated by task outcomes.
- **Memory** denotes information without reference to task outcomes;

This taxonomy maps directly to the three primary application scenarios that organize the papers in this repository:

| Application               | Memory Content                                                           | Description                                                                                                                                               |
| :------------------------ | :----------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Personalization           | User profiles, interaction history, facts, etc.                          | Continuous personalized interaction, mainly targeting the conversation scenario and using an external memory pool with retrieval-based memory interaction |
| Learning from Experience  | Trajectories, success/failure lessons, reusable skills, etc.             | Cross-task experience accumulation & transfer                                                                                                             |
| Long-horizon Agentic Task | Intermediate results, reasoning traces, environmental observations, etc. | Context management within a single long-horizon task via summarization, reflection, or scratchpad, etc.                                                   |

## Paper List

### Application

#### Personalization

| Date | Title | Paper |
|:------:|:------|:------:|
| 2025-10 | TOM-SWE: User Mental Modeling For Software Engineering Agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.21903) |
| 2025-10 | EvolveR: Self-Evolving LLM Agents through an Experience-Driven Lifecycle | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.16079) |
| 2025-10 | Improving Code Localization with Repository Memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.01003) |
| 2025-10 | Mnemosyne: An Unsupervised, Human-Inspired Long-Term Memory Architecture for Edge-Based LLMs | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.08601) |
| 2025-10 | AssoMem: Scalable Memory QA with Multi-Signal Associative Retrieval | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.10397) |
| 2025-10 | LightMem: Lightweight and Efficient Memory-Augmented Generation | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.18866) |
| 2025-09 | MEM-$\alpha$: Learning Memory Construction via Reinforcement Learning | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.25911) |
| 2025-09 | PISA: A Pragmatic Psych-Inspired Unified Memory System for Enhanced AI Agency | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=l82wkoRQ3l) |
| 2025-09 | Look Back to Reason Forward: Revisitable Memory for Long-Context LLM Agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.23040) |
| 2025-09 | Memory-T1: Reinforcement Learning for Temporal Reasoning in Multi-session Agents | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=vQf2YR2Kpd) |
| 2025-09 | MIRA: Memory-Integrated Reinforcement Learning Agent  with Limited LLM Guidance | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=oWagByDNPc) |
| 2025-09 | REMem: Reasoning with Episodic Memory in Language Agent | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=fugnQxbvMm) |
| 2025-09 | Adaptive Friend Agent: Personalized Multi-User Memory for Conversational AI | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=wKTwm7ZzDK) |
| 2025-08 | Orchid: Orchestrating Context Across Creative Workflows with Generative AI | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.19517) |
| 2025-08 | Memory-R1: Enhancing Large Language Model Agents to Manage and Utilize Memories via Reinforcement Learning | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.19828) |
| 2025-07 | MemOS: A Memory OS for AI System | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.03724) |
| 2025-07 | Hierarchical Memory for High-Efficiency Long-Term Reasoning in LLM Agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.22925) |
| 2025-06 | PersonaAgent: When Large Language Model Agents Meet Personalization at Test Time | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.06254) |
| 2025-06 | SynthesizeMe! Inducing Persona-Guided Prompts for Personalized Reward Models in LLMs | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.05598) |
| 2025-06 | Cognitive Weave: Synthesizing Abstracted Knowledge with a Spatio-Temporal Resonance Graph | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.08098) |
| 2025-05 | From Single to Multi-Granularity: Toward Long-Term Memory Association and Selection of Conversational Agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.19549) |
| 2025-04 | Mem0: Building production-ready ai agents with scalable long-term memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.19413) |
| 2025-03 | Meminsight: Autonomous memory augmentation for llm agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.21760) |
| 2025-02 | M+: Extending MemoryLLM with Scalable Long-Term Memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.00592) |
| 2025-02 | A-MEM: Agentic Memory for LLM Agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.12110) |
| 2025-01 | Wormhole Memory: A Rubik's Cube for Cross-Dialogue Retrieval | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.14846) |
| 2025-01 | Zep: A Temporal Knowledge Graph Architecture for Agent Memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.13956) |
| 2024-12 | On the Structural Memory of LLM Agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.15266) |
| 2024-07 | MemoCRS: Memory-enhanced Sequential Conversational Recommender Systems with Large Language Models | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.04960) |
| 2024-03 | Larimar: Large language models with episodic memory control | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2403.11901) |
| 2024-01 | From llm to conversational agent: A memory enhanced architecture with fine-tuning of large language models | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.02777) |
| 2023-10 | MemGPT: Towards LLMs as operating systems | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2310.08560) |
| 2023-08 | Memochat: Tuning llms to use memos for consistent long-range open-domain conversation | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2308.08239) |
| 2023-06 | Chatdb: Augmenting llms with databases as their symbolic memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2306.03901) |
| 2023-05 | MemoryBank: Enhancing large language models with long-term memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2305.10250) |
| 2023-04 | Unleashing infinite-length input capacity for large-scale language models with self-controlled memory system | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2304.13343) |

#### Learning from Experience

| Date | Title | Paper |
|:------:|:------|:------:|
| 2025-10 | Alita-G: Self-Evolving Generative Agent for Agent Generation | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.23601) |
| 2025-10 | Dyna-Mind: Learning to Simulate from Experience for Better AI Agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.09577) |
| 2025-10 | Agentic Context Engineering: Learning Comprehensive Contexts for Self-Improving Language Models | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.04618) |
| 2025-10 | LEGOMem: Modular Procedural Memory for Multi-agent LLM Systems for Workflow Automation | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.04851) |
| 2025-10 | The Cognitive Bandwidth Bottleneck: Shifting Long-Horizon Agent from Planning with Actions to Planning with Schemas | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.07091) |
| 2025-10 | Agentic Context Engineering: Evolving Contexts for Self-Improving Language Models | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.04618) |
| 2025-10 | TokMem: Tokenized Procedural Memory for Large Language Models | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.00444) |
| 2025-10 | Training-Free Group Relative Policy Optimization | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.08191) |
| 2025-10 | Self-evolving expertise in complex non-verifiable subject domains: dialogue as implicit meta-RL | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.15772) |
| 2025-09 | WebOperator: Action-Aware Tree Search for Autonomous Agents in Web Environment | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=vnEuxLVFmN) |
| 2025-09 | Improving Language Agents through BREW: Bootstrapping expeRientially-learned Environmental knoWledge | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=gmmHn5nFvK) |
| 2025-09 | Exploratory Memory-Augmented LLM Agent via Hybrid On- and Off-Policy Optimization | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=UOzxviKVFO) |
| 2025-09 | Automated Stateful Specialization for Adaptive Agent Systems | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=UESTP6dR1K) |
| 2025-09 | BMAS: A Brain-Inspired Multi-Agent System with PFC-Guided Task Coordination and Hippocampus-Neocortex Dual Memory for Scalable Multi-Step Reasoning | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=YqFLsI44vN) |
| 2025-09 | Scaling Agent Learning via Experience Synthesis | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=cf7qpBwttr) |
| 2025-09 | Xolver: Generalist Reasoning and Problem Solving through Federated Multi-Agent Dynamics and Holistic Experience Learning | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=xXhgzwwQ42) |
| 2025-09 | MemGen: Weaving Generative Latent Memory for Self-Evolving Agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.24704) |
| 2025-09 | Unifying Dynamic Tool Creation and Cross-Task Experience Sharing through Cognitive Memory Architecture | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=JnwClln80Q) |
| 2025-09 | MetaEvo: A Meta-Optimization Framework for Experience-Driven Agent Evolution | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=1YcMHVY9cl) |
| 2025-09 | ReasoningBank: Scaling Agent Self-Evolving with Reasoning Memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.25140) |
| 2025-09 | MLE-RL: Reinforcement Learning for Self-Improvement in Machine Learning Agents | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=nElqyHPHAz) |
| 2025-09 | ArcMemo: Abstract Reasoning Composition with Lifelong LLM Memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.04439) |
| 2025-08 | SEAgent: Self-Evolving Computer Use Agent with Autonomous Learning from Experience | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.04700) |
| 2025-08 | Memento: Fine-tuning LLM Agents without Fine-tuning LLMs | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.16153) |
| 2025-08 | SE-Agent: Self-Evolution Trajectory Optimization in Multi-Step Reasoning with LLM-Based Agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.02085) |
| 2025-08 | Memp: Exploring Agent Procedural Memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.06433) |
| 2025-07 | Agent KB: Leveraging Cross-Domain Experience for Agentic Problem Solving | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.06229) |
| 2025-07 | SWE-Exp: Experience-Driven Software Issue Resolution | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.23361) |
| 2025-06 | G-Memory: Tracing Hierarchical Memory for Multi-Agent Systems | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.07398) |
| 2025-06 | Cost-Efficient Serving of LLM Agents via Test-Time Plan Caching | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.14852) |
| 2025-06 | MAPLE: Multi-Agent Adaptive Planning with Long-Term Memory for Table Reasoning | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.05813) |
| 2025-05 | ML-Agent: Reinforcing LLM Agents for Autonomous Machine Learning Engineering | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.23723) |
| 2025-05 | How Memory Management Impacts LLM Agents: An Empirical Study of Experience-Following Behavior | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.16067) |
| 2025-05 | Efficiently enhancing general agents with hierarchical-categorical memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.22006) |
| 2025-04 | SkillWeaver: Web Agents can Self-Improve by Discovering and Honing Skills | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07079) |
| 2025-04 | Inducing Programmatic Skills for Agentic Tasks | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.06821) |
| 2025-04 | Memorization and knowledge injection in gated llms | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.21239) |
| 2025-04 | Dynamic Cheatsheet: Test-Time Learning with Adaptive Memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07952) |
| 2025-03 | Mars: Memory-enhanced agents with reflective self-improvement | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.19271) |
| 2024-09 | Agent workflow memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2409.07429) |
| 2024-05 | AutoManual: Constructing Instruction Manuals by LLM Agents via Interactive Environmental Learning | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2405.16247) |
| 2024-05 | Iterative experience refinement of software- developing agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2405.04219) |
| 2024-04 | An artificial neuron for enhanced problem solving in large language models | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.14222) |
| 2024-03 | Online adaptation of language models with a memory of amortized contexts | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2403.04317) |
| 2024-02 | Camelot: Towards large language models with training-free consolidated associative memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.13449) |
| 2023-08 | Retroformer: Retrospective large language agents with policy gradient optimization | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2308.02151) |
| 2023-08 | ExpeL: LLM Agents Are Experiential Learners | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2308.10144) |
| 2023-06 | Synapse: Trajectory-as-exemplar prompting with memory for computer control | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2306.07863) |
| 2023-03 | Reflexion: Language agents with verbal reinforcement learning | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2303.11366) |
| 2020-09 | Meta-learning with sparse experience replay for lifelong language learning | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2009.04891) |

#### Long-horizon Agentic Task

| Date | Title | Paper |
|:------:|:------|:------:|
| 2025-10 | Prompt reinforcing for long-term planning of large language models | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.05921) |
| 2025-10 | Learning on the Job: An Experience-Driven Self-Evolving Agent for Long-Horizon Tasks | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.08002) |
| 2025-10 | ACON: Optimizing Context Compression for Long-horizon LLM Agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.00615) |
| 2025-10 | BrowserAgent: Building Web Agents with Human-Inspired Web Browsing Actions | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.10666) |
| 2025-10 | WebDART: Dynamic Decomposition and Re-planning for Complex Web Tasks | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.06587) |
| 2025-10 | CAM: A Constructivist View of Agentic Memory for LLM-Based Reading Comprehension | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.05520) |
| 2025-10 | Scaling LLM Multi-turn RL with End-to-end Summarization-based Context Management | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.06727) |
| 2025-10 | AgentFold: Long-Horizon Web Agents with Proactive Context Management | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.24699) |
| 2025-10 | Beyond Turn Limits: Training Deep Search Agents with Dynamic Context Window | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.08276) |
| 2025-10 | Memory as Action: Autonomous Context Curation for Long-Horizon Agentic Tasks | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.12635) |
| 2025-10 | DeepAgent: A General Reasoning Agent with Scalable Toolsets | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.21618) |
| 2025-09 | ABBEL: LLM Agents Acting Through Belief Bottlenecks Expressed in Language | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=lMjxyHLL2R) |
| 2025-09 | Efficient On-Device Agents via Adaptive Context Management | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=TPXVdBjrvU) |
| 2025-09 | WebWeaver: Structuring Web-Scale Evidence with Dynamic Outlines for Open-Ended Deep Research | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.13312) |
| 2025-09 | Don’t Lose the Thread: Empowering Long-Horizon LLM Agents with Cognitive Resource Self-Allocation | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=NBGlItueYE) |
| 2025-09 | CEA: Context Engineering Agent for Enhanced Reliability and Sustainability in Deep Research Systems | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=6QUNblHtto) |
| 2025-09 | The Pensieve Paradigm: Stateful Language Models with Learned Memory Management | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=GymjF88oGQ) |
| 2025-09 | MemSearcher: Training LLMs to Reason, Search and Manage Memory via End-to-End Reinforcement Learning | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=EWIAx3NgvA) |
| 2025-09 | Compressed Step Information Memory for End-to-End Agent Foundation Models | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=vUG2hpVJWR) |
| 2025-09 | Intrinsic Memory Agents: Heterogeneous Multi-Agent LLM Systems through Structured Contextual Memory | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=UbSUxAK3BI) |
| 2025-09 | IterResearch: Rethinking Long-Horizon Agents via Markovian State Reconstruction | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=qQ5MZ5Mx7p) |
| 2025-09 | PARL-MT: Learning to Call Functions in Multi-Turn Conversation with Progress Awareness | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.23206) |
| 2025-09 | ReSum: Unlocking Long-Horizon Search Intelligence via Context Summarization | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.13313) |
| 2025-08 | Sculptor: Empowering LLMs with Cognitive Agency via Active Context Management | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.04664) |
| 2025-08 | Cognitive Workspace: Active Memory Management for LLMs - An Empirical Study of Functional Infinite Context | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.13171) |
| 2025-08 | Profile-Aware Maneuvering: A Dynamic Multi-Agent System for Robust GAIA Problem Solving by AWorld | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.09889) |
| 2025-07 | MemAgent: Reshaping Long-Context LLM with Multi-Conv RL-based Memory Agent | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.02259) |
| 2025-07 | MemTool: Optimizing Short-Term Memory Management for Dynamic Tool Calling in LLM Agent Multi-Turn Conversations | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.21428) |
| 2025-06 | MEM1: Learning to Synergize Memory and Reasoning for Efficient Long-Horizon Agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.15841) |
| 2025-06 | Taskcraft: Automated generation of agentic tasks | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.10055) |
| 2024-10 | From isolated conversations to hierarchical schemas: Dynamic tree memory representation for LLMs | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.14052) |
| 2024-09 | Self-evolving Agents with reflective and memory-augmented abilities | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2409.00872) |
| 2024-07 | Human-like episodic memory for infinite context llms | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.09450) |
| 2024-07 | AriGraph: Learning knowledge graph world models with episodic memory for LLM agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.04363) |
| 2024-06 | QRMeM: Unleash the Length Limitation through Question then Reflection Memory Mechanism | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.13167) |

### Survey

| Date | Title | Paper | GitHub |
| :------: | :------ | :------: | :------: |
| 2025-10 | Context Engineering 2.0: The Context of Context Engineering | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.26493) | [![GitHub Stars](https://img.shields.io/github/stars/GAIR-NLP/Context-Engineering-2.0?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/GAIR-NLP/Context-Engineering-2.0) |
| 2025-10 | Beyond Pipelines: A Survey of the Paradigm Shift toward Model-Native Agentic AI | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.16720) | [![GitHub Stars](https://img.shields.io/github/stars/ADaM-BJTU/model-native-agentic-ai?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ADaM-BJTU/model-native-agentic-ai) |
| 2025-09 | The Landscape of Agentic Reinforcement Learning for LLMs: A Survey | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.02547) | [![GitHub Stars](https://img.shields.io/github/stars/xhyumiracle/Awesome-AgenticLLM-RL-Papers?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/xhyumiracle/Awesome-AgenticLLM-RL-Papers) |
| 2025-08 | OS Agents: A Survey on MLLM-based Agents for General Computing Devices Use | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.04482) | [![GitHub Stars](https://img.shields.io/github/stars/OS-Agent-Survey/OS-Agent-Survey?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/OS-Agent-Survey/OS-Agent-Survey) |
| 2025-08 | A Comprehensive Survey of Self-Evolving AI Agents: A New Paradigm Bridging Foundation Models and Lifelong Agentic Systems | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.07407) | [![GitHub Stars](https://img.shields.io/github/stars/EvoAgentX/Awesome-Self-Evolving-Agents?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/EvoAgentX/Awesome-Self-Evolving-Agents) |
| 2025-07 | A Survey of Context Engineering for Large Language Models | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.13334) | [![GitHub Stars](https://img.shields.io/github/stars/Meirtz/Awesome-Context-Engineering?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Meirtz/Awesome-Context-Engineering) |
| 2025-07 | A Survey of Self-Evolving Agents: On Path to Artificial Super Intelligence | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.21046) | [![GitHub Stars](https://img.shields.io/github/stars/CharlesQ9/Self-Evolving-Agents?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/CharlesQ9/Self-Evolving-Agents) |
| 2025-05 | Rethinking Memory in AI: Taxonomy, Operations, Topics, and Future Directions | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.00675) | [![GitHub Stars](https://img.shields.io/github/stars/Elvin-Yiming-Du/Survey_Memory_in_AI?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Elvin-Yiming-Du/Survey_Memory_in_AI) |
| 2025-04 | From Human Memory to AI Memory: A Survey on Memory Mechanisms in the Era of LLMs | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.15965) |  |
| 2025-04 | Advances and Challenges in Foundation Agents: From Brain-Inspired Intelligence to Evolutionary, Collaborative, and Safe Systems | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.01990) | [![GitHub Stars](https://img.shields.io/github/stars/FoundationAgents/awesome-foundation-agents?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/FoundationAgents/awesome-foundation-agents) |
| 2025-03 | Agentic Large Language Models, a survey | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.23037) |  |
| 2024-04 | A Survey on the Memory Mechanism of Large Language Model-based Agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.13501) | [![GitHub Stars](https://img.shields.io/github/stars/nuster1128/LLM_Agent_Memory_Survey?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/nuster1128/LLM_Agent_Memory_Survey) |

### Benchmark

| Date | Name | Title | Paper | GitHub |
| :------: | :------ | :------ | :------: | :------: |
| 2025-08 | StuLife | Building Self-Evolving Agents via Experience-Driven Lifelong Learning: A Framework and Benchmark | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.19005) | [![GitHub Stars](https://img.shields.io/github/stars/ECNU-ICALK/ELL-StuLife?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ECNU-ICALK/ELL-StuLife) |
| 2025-07 | MemoryAgentBench | Evaluating Memory in LLM Agents via Incremental Multi-Turn Interactions | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.05257) | [![GitHub Stars](https://img.shields.io/github/stars/HUST-AI-HYZ/MemoryAgentBench?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/HUST-AI-HYZ/MemoryAgentBench) |
| 2025-06 | StoryBench | StoryBench: A Dynamic Benchmark for Evaluating Long-Term Memory with Multi Turns | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.13356) |  |
| 2025-06 | WebChoreArena | WebChoreArena: Evaluating Web Browsing Agents on Realistic Tedious Web Tasks | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.01952) | [![GitHub Stars](https://img.shields.io/github/stars/WebChoreArena/WebChoreArena?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/WebChoreArena/WebChoreArena) |
| 2025-05 | LifelongAgentBench | LifelongAgentBench: Evaluating LLM Agents as Lifelong Learners | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.11942) | [![GitHub Stars](https://img.shields.io/github/stars/caixd-220529/LifelongAgentBench?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/caixd-220529/LifelongAgentBench) |
| 2025-02 | RealTalk | REALTALK: A 21-Day Real-World Dataset for Long-Term Conversation | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.13270) | [![GitHub Stars](https://img.shields.io/github/stars/danny911kr/REALTALK?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/danny911kr/REALTALK) |
| 2024-10 | LongMemEval | LongMemEval: Benchmarking Chat Assistants on Long-Term Interactive Memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.10813) | [![GitHub Stars](https://img.shields.io/github/stars/xiaowu0162/LongMemEval?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/xiaowu0162/LongMemEval) |
| 2024-09 | LTM  | Beyond Prompts: Dynamic Conversational Benchmarking of Large Language Models | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2409.20222) | [![GitHub Stars](https://img.shields.io/github/stars/GoodAI/goodai-ltm-benchmark?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/GoodAI/goodai-ltm-benchmark) |
| 2024-09 | MADail-Bench | MADial-Bench: Towards Real-world Evaluation of Memory-Augmented Dialogue Generation | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2409.15240) | [![GitHub Stars](https://img.shields.io/github/stars/hejunqing/MADial-Bench?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/hejunqing/MADial-Bench) |
| 2024-02 | LoCoMo | Evaluating Very Long-Term Conversational Memory of LLM Agents | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.17753) | [![GitHub Stars](https://img.shields.io/github/stars/snap-research/locomo?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/snap-research/locomo) |

### Product & Project

| Date | Name | Title | Paper | Website | GitHub |
| :------: | :------ | :------ | :------: | :------: | :------: |
| 2025-05 | Cognee | Optimizing the Interface Between Knowledge Graphs and LLMs for Complex Reasoning | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.24478) | [![Website](https://img.shields.io/badge/website-1F4E79?style=for-the-badge)](https://www.cognee.ai/) | [![GitHub Stars](https://img.shields.io/github/stars/topoteretes/cognee?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/topoteretes/cognee) |
| 2025-04 | Mem0 | Mem0: Building Production-Ready AI Agents with Scalable Long-Term Memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.19413) | [![Website](https://img.shields.io/badge/website-1F4E79?style=for-the-badge)](https://mem0.ai/) | [![GitHub Stars](https://img.shields.io/github/stars/mem0ai/mem0?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/mem0ai/mem0) |
| 2025-01 | Graphiti (prev. Zep) | Zep: A Temporal Knowledge Graph Architecture for Agent Memory | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.13956) | [![Website](https://img.shields.io/badge/website-1F4E79?style=for-the-badge)](https://help.getzep.com/graphiti) | [![GitHub Stars](https://img.shields.io/github/stars/getzep/graphiti?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/getzep/graphiti) |
| 2023-10 | Letta (prev. MemGPT) | MemGPT: Towards LLMs as Operating Systems | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2310.08560) | [![Website](https://img.shields.io/badge/website-1F4E79?style=for-the-badge)](https://www.letta.com/) | [![GitHub Stars](https://img.shields.io/github/stars/letta-ai/letta?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/letta-ai/letta) |
|  | LangChain |  |  | [![Website](https://img.shields.io/badge/website-1F4E79?style=for-the-badge)](https://www.langchain.com/) | [![GitHub Stars](https://img.shields.io/github/stars/langchain-ai/langchain?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/langchain-ai/langchain) |
|  | ReMe (prev. MemoryScope) |  |  | [![Website](https://img.shields.io/badge/website-1F4E79?style=for-the-badge)](https://modelscope.github.io/ReMe/) | [![GitHub Stars](https://img.shields.io/github/stars/modelscope/ReMe?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/modelscope/ReMe) |
|  | Memary |  |  | [![Website](https://img.shields.io/badge/website-1F4E79?style=for-the-badge)](https://kingjulio8238.github.io/memarydocs/) | [![GitHub Stars](https://img.shields.io/github/stars/kingjulio8238/Memary?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/kingjulio8238/Memary) |
|  | OpenMemory |  |  | [![Website](https://img.shields.io/badge/website-1F4E79?style=for-the-badge)](https://openmemory.cavira.app/) | [![GitHub Stars](https://img.shields.io/github/stars/CaviraOSS/OpenMemory?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/CaviraOSS/OpenMemory) |
|  | MemU |  |  | [![Website](https://img.shields.io/badge/website-1F4E79?style=for-the-badge)](https://memu.pro/) | [![GitHub Stars](https://img.shields.io/github/stars/NevaMind-AI/memU?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/NevaMind-AI/memU) |
