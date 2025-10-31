# Awesome-Memory-for-Agents

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
        - [Product \& Project](#product--project)

## Overview

This repository provides a curated list of papers on agent memory, structured by a core taxonomy. We first divide agent memory based on its persistence:

- **Short-Term Memory:** Transient information managed within the context window for a single task;
- **Long-Term Memory:** Persistent information stored externally across tasks.

Within *Long-Term Memory*, we further distinguish based on its reliance on task success/failure for curation:

- **Memory (for Personalization)** denotes information without reference to task success/failure;
- **Experience (for Learning)** involves knowledge explicitly curated through task success/failure.

This taxonomy maps directly to the three primary application scenarios that organize the papers in this repository:

| Application               | Memory Content                                               | Description                                          |
| :------------------------ | :----------------------------------------------------------- | :--------------------------------------------------- |
| Personalization           | User profiles, interaction history, facts, etc.              | Continuous personalized interaction                  |
| Learning from Experience  | Trajectories, success/failure lessons, reusable skills, etc. | Cross-task experience accumulation & transfer        |
| Long-horizon Agentic Task | Intermediate steps, reasoning traces                         | Context management within a single long-horizon task |

## Paper List

### Application

#### Personalization

|  Date   | Title                                                                                                        | URL                                                                                                                                    |
| :-----: | :----------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------- |
| 2025-10 | Improving Code Localization with Repository Memory                                                           | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.01003) |
| 2025-10 | Mnemosyne: An Unsupervised, Human-Inspired Long-Term Memory Architecture for Edge-Based LLMs                 | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.08601) |
| 2025-10 | AssoMem: Scalable Memory QA with Multi-Signal Associative Retrieval                                          | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.10397) |
| 2025-08 | Orchid: Orchestrating Context Across Creative Workflows with Generative AI                                   | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.19517) |
| 2025-07 | MemOS: A Memory OS for AI System                                                                             | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.03724) |
| 2025-06 | PersonaAgent: When Large Language Model Agents Meet Personalization at Test Time                             | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.06254) |
| 2025-06 | SynthesizeMe! Inducing Persona-Guided Prompts for Personalized Reward Models in LLMs                         | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.05598) |
| 2025-02 | A-MEM: Agentic Memory for LLM Agents                                                                         | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.12110) |
| 2025-01 | Wormhole Memory: A Rubik's Cube for Cross-Dialogue Retrieval                                                 | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.14846) |
| 2024-12 | On the Structural Memory of LLM Agents                                                                       | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.15266) |
| 2024-07 | MemoCRS: Memory-enhanced Sequential Conversational Recommender Systems with Large Language Models            | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.04960) |
| 2024-01 | From llm to conversational agent: A memory enhanced architecture with fine-tuning of large language models   | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.02777) |
| 2023-08 | Memochat: Tuning llms to use memos for consistent long-range open-domain conversation                        | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2308.08239) |
| 2023-06 | Chatdb: Augmenting llms with databases as their symbolic memory                                              | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2306.03901) |
| 2023-05 | MemoryBank: Enhancing large language models with long-term memory                                            | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2305.10250) |
| 2023-04 | Unleashing infinite-length input capacity for large-scale language models with self-controlled memory system | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2304.13343) |
|    -    | TOM-SWE: User Mental Modeling For Software Engineering Agents                                                | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=A4koL4Zqam)                  |
|    -    | MEM-$\alpha$: LEARNING MEMORY CONSTRUCTION VIA REINFORCEMENT LEARNING                                        | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=dm42omwep1)                  |
|    -    | PISA: A Pragmatic Psych-Inspired Unified Memory System for Enhanced AI Agency                                | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=l82wkoRQ3l)                  |
|    -    | Look Back to Reason Forward: Revisitable Memory for Long-Context LLM Agents                                  | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=1cymflI2Lh)                  |
|    -    | Memory-T1: Reinforcement Learning for Temporal Reasoning in Multi-session Agents                             | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=vQf2YR2Kpd)                  |
|    -    | MIRA: Memory-Integrated Reinforcement Learning Agent  with Limited LLM Guidance                              | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=oWagByDNPc)                  |
|    -    | EvolveR: Self-Evolving LLM Agents through an Experience-Driven Lifecycle                                     | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=sooLoD9VSf)                  |
|    -    | REMem: Reasoning with Episodic Memory in Language Agent                                                      | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=fugnQxbvMm)                  |
|    -    | Adaptive Friend Agent: Personalized Multi-User Memory for Conversational AI                                  | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=wKTwm7ZzDK)                  |

#### Learning from Experience

|  Date   | Title                                                                                                                                               | URL                                                                                                                                    |
| :-----: | :-------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------- |
| 2025-10 | Dyna-Mind: Learning to Simulate from Experience for Better AI Agents                                                                                | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.09577) |
| 2025-10 | LEGOMem: Modular Procedural Memory for Multi-agent LLM Systems for Workflow Automation                                                              | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.04851) |
| 2025-10 | TokMem: Tokenized Procedural Memory for Large Language Models                                                                                       | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.00444) |
| 2025-09 | ArcMemo: Abstract Reasoning Composition with Lifelong LLM Memory                                                                                    | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.04439) |
| 2025-08 | Memento: Fine-tuning LLM Agents without Fine-tuning LLMs                                                                                            | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.16153) |
| 2025-08 | SE-Agent: Self-Evolution Trajectory Optimization in Multi-Step Reasoning with LLM-Based Agents                                                      | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.02085) |
| 2025-07 | SWE-Exp: Experience-Driven Software Issue Resolution                                                                                                | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.23361) |
| 2025-06 | Cost-Efficient Serving of LLM Agents via Test-Time Plan Caching                                                                                     | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.14852) |
| 2025-06 | MAPLE: Multi-Agent Adaptive Planning with Long-Term Memory for Table Reasoning                                                                      | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.05813) |
| 2025-05 | ML-Agent: Reinforcing LLM Agents for Autonomous Machine Learning Engineering                                                                        | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.23723) |
| 2025-05 | How Memory Management Impacts LLM Agents: An Empirical Study of Experience-Following Behavior                                                       | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.16067) |
| 2025-05 | Efficiently enhancing general agents with hierarchical-categorical memory                                                                           | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.22006) |
| 2025-04 | SkillWeaver: Web Agents can Self-Improve by Discovering and Honing Skills                                                                           | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07079) |
| 2025-04 | Inducing Programmatic Skills for Agentic Tasks                                                                                                      | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.06821) |
| 2025-04 | Memorization and knowledge injection in gated llms                                                                                                  | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.21239) |
| 2025-03 | Mars: Memory-enhanced agents with reflective self-improvement                                                                                       | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.19271) |
| 2024-09 | Agent workflow memory                                                                                                                               | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2409.07429) |
| 2024-05 | Iterative experience refinement of software- developing agents                                                                                      | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2405.04219) |
| 2024-04 | An artificial neuron for enhanced problem solving in large language models                                                                          | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.14222) |
| 2024-03 | Online adaptation of language models with a memory of amortized contexts                                                                            | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2403.04317) |
| 2024-02 | Camelot: Towards large language models with training-free consolidated associative memory                                                           | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.13449) |
| 2023-08 | Retroformer: Retrospective large language agents with policy gradient optimization                                                                  | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2308.02151) |
| 2023-08 | ExpeL: LLM agents are experiential learners                                                                                                         | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2308.10144) |
| 2023-06 | Synapse: Trajectory-as-exemplar prompting with memory for computer control                                                                          | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2306.07863) |
| 2023-03 | Reflexion: Language agents with verbal reinforcement learning                                                                                       | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2303.11366) |
| 2020-09 | Meta-learning with sparse experience replay for lifelong language learning                                                                          | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2009.04891) |
|    -    | WebOperator: Action-Aware Tree Search for Autonomous Agents in Web Environment                                                                      | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=vnEuxLVFmN)                  |
|    -    | Exploratory Memory-Augmented LLM Agent via Hybrid On- and Off-Policy Optimization                                                                   | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=UOzxviKVFO)                  |
|    -    | Automated Stateful Specialization for Adaptive Agent Systems                                                                                        | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=UESTP6dR1K)                  |
|    -    | Alita-G: Self-Evolving Generative Agent for Agent Generation                                                                                        | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=xf2JC4531b)                  |
|    -    | SEAgent: Self-Evolving Computer Use Agent with Autonomous Learning from Experience                                                                  | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=OuW3gCJRBK)                  |
|    -    | BMAS: A Brain-Inspired Multi-Agent System with PFC-Guided Task Coordination and Hippocampus-Neocortex Dual Memory for Scalable Multi-Step Reasoning | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=YqFLsI44vN)                  |
|    -    | Scaling Agent Learning via Experience Synthesis                                                                                                     | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=cf7qpBwttr)                  |
|    -    | Xolver: Generalist Reasoning and Problem Solving through Federated Multi-Agent Dynamics and Holistic Experience Learning                            | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=xXhgzwwQ42)                  |
|    -    | MetaEvo: A Meta-Optimization Framework for Experience-Driven Agent Evolution                                                                        | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=1YcMHVY9cl)                  |
|    -    | ReasoningBank: Scaling Agent Self-Evolving with Reasoning Memory                                                                                    | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=jL7fwchScm)                  |
|    -    | Agent KB: Leveraging Cross-Domain Experience for Agentic Problem Solving                                                                            | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=QCLXVOMkl4)                  |
|    -    | Agentic Context Engineering: Learning Comprehensive Contexts for Self-Improving Language Models                                                     | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=eC4ygDs02R)                  |

#### Long-horizon Agentic Task

|  Date   | Title                                                                                                           | URL                                                                                                                                    |
| :-----: | :-------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------- |
| 2025-10 | WebDART: Dynamic Decomposition and Re-planning for Complex Web Tasks                                            | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.06587) |
| 2025-10 | CAM: A Constructivist View of Agentic Memory for LLM-Based Reading Comprehension                                | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.05520) |
| 2025-10 | Scaling LLM Multi-turn RL with End-to-end Summarization-based Context Management                                | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.06727) |
| 2025-09 | WebWeaver: Structuring Web-Scale Evidence with Dynamic Outlines for Open-Ended Deep Research                    | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.13312) |
| 2025-09 | PARL-MT: Learning to Call Functions in Multi-Turn Conversation with Progress Awareness                          | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.23206) |
| 2025-08 | Sculptor: Empowering LLMs with Cognitive Agency via Active Context Management                                   | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.04664) |
| 2025-08 | Cognitive Workspace: Active Memory Management for LLMs - An Empirical Study of Functional Infinite Context      | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.13171) |
| 2025-08 | Chain-of-agents: End-to-end agent foundation models via multi-agent distillation and agentic rl                 | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.13167) |
| 2025-07 | MemTool: Optimizing Short-Term Memory Management for Dynamic Tool Calling in LLM Agent Multi-Turn Conversations | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.21428) |
| 2025-06 | Code researcher: Deep research agent for large systems code and commit history                                  | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.11060) |
| 2025-06 | Taskcraft: Automated generation of agentic tasks                                                                | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.10055) |
| 2025-04 | Mem0: Building production-ready ai agents with scalable long-term memory                                        | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.19413) |
| 2025-03 | Plan-and-Act: Improving Planning of Agents for Long-Horizon Tasks                                               | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.09572) |
| 2025-03 | Meminsight: Autonomous memory augmentation for llm agents                                                       | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.21760) |
| 2024-10 | From isolated conversations to hierarchical schemas: Dynamic tree memory representation for LLMs                | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.14052) |
| 2024-10 | Web Agents with World Models: Learning and Leveraging Environment Dynamics in Web Navigation                    | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.13232) |
| 2024-07 | Tree Search for Language Model Agents                                                                           | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.01476) |
| 2024-07 | Human-like episodic memory for infinite context llms                                                            | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.09450) |
| 2024-07 | AriGraph: Learning knowledge graph world models with episodic memory for LLM agents                             | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.04363) |
| 2023-10 | MemGPT: Towards LLMs as operating systems                                                                       | [![Paper](https://img.shields.io/badge/paper-A42C25?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2310.08560) |
|    -    | Efficient On-Device Agents via Adaptive Context Management                                                      | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=TPXVdBjrvU)                  |
|    -    | Prompt reinforcing for long-term planning of large language models                                              | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=Xt6K4cw36l)                  |
|    -    | Don’t Lose the Thread: Empowering Long-Horizon LLM Agents with Cognitive Resource Self-Allocation               | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=NBGlItueYE)                  |
|    -    | CEA: Context Engineering Agent for Enhanced Reliability and Sustainability in Deep Research Systems             | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=6QUNblHtto)                  |
|    -    | The Pensieve Paradigm: Stateful Language Models with Learned Memory Management                                  | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=GymjF88oGQ)                  |
|    -    | MEM1: Learning to Synergize Memory and Reasoning for Efficient Long-Horizon Agents                              | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=XY8AaxDSLb)                  |
|    -    | MemSearcher: Training LLMs to Reason, Search and Manage Memory via End-to-End Reinforcement Learning            | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=EWIAx3NgvA)                  |
|    -    | MemAgent: Reshaping Long-Context LLM with Multi-Conv RL-based Memory Agent                                      | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=k5nIOvYGCL)                  |
|    -    | Compressed Step Information Memory for End-to-End Agent Foundation Models                                       | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=vUG2hpVJWR)                  |
|    -    | MemGen: Weaving Generative Latent Memory for Self-Evolving Agents                                               | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=vI56m4Iu4e)                  |
|    -    | Intrinsic Memory Agents: Heterogeneous Multi-Agent LLM Systems through Structured Contextual Memory             | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=UbSUxAK3BI)                  |
|    -    | Learning on the Job: An Experience-Driven Self-Evolving Agent for Long-Horizon Tasks                            | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=ZzH6xDdpTP)                  |
|    -    | Unifying Dynamic Tool Creation and Cross-Task Experience Sharing through Cognitive Memory Architecture          | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=JnwClln80Q)                  |
|    -    | From Experience to Strategy: Empowering LLM Agents with Trainable Graph Memory                                  | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=bvaaydGKYp)                  |
|    -    | MLE-RL: Reinforcement Learning for Self-Improvement in Machine Learning Agents                                  | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=nElqyHPHAz)                  |
|    -    | ACON: Optimizing Context Compression for Long-horizon LLM Agents                                                | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=7JbSwX6bNL)                  |
|    -    | IterResearch: Rethinking Long-Horizon Agents via Markovian State Reconstruction                                 | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=qQ5MZ5Mx7p)                  |
|    -    | BrowserAgent: Building Web Agents with Human-Inspired Web Browsing Actions                                      | [![Paper](https://img.shields.io/badge/Paper-6772E5?style=for-the-badge)](https://openreview.net/forum?id=dtExkh4l4z)                  |

### Survey

### Benchmark

### Product & Project
