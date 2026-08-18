<h1 align="center">
  Awesome Self-Improving Modern Agentic Systems
</h1>

<p align="center">
  <strong>
    A curated and continuously evolving resource hub for self-improving agentic systems
  </strong>
  <br>
  <sub>
    This repository brings together
    📄 Papers · 📊 Benchmarks · ✍️ Blogs · 🎙️ Podcasts ·
    💬 Interviews · 🎥 Videos · 🧑‍🏫 Workshops & Courses
  </sub>
  <br>
  <sub>
    Contributions are welcome — open a PR to share relevant resources and help grow the community! 🌱
  </sub>
</p>

<p align="center">
  <a href="https://arxiv.org/abs/2607.13104">
    <img
      src="https://img.shields.io/badge/READ_THE_PAPER-arXiv%3A2607.13104-B31B1B?style=for-the-badge&logo=arxiv&logoColor=white"
      alt="Read the paper"
    >
  </a>
  <a href="https://huggingface.co/papers/2607.13104">
    <img
      src="https://img.shields.io/badge/HUGGING_FACE-Daily_Papers-FFD21E?style=for-the-badge&logo=huggingface&logoColor=FFD21E"
      alt="Hugging Face Daily Papers"
    >
  </a>
  <a href="https://selfimproving-agent.github.io/">
    <img
      src="https://img.shields.io/badge/PROJECT_PAGE-Explore-1D4ED8?style=for-the-badge&logo=googlechrome&logoColor=white"
      alt="Project page"
    >
  </a>
  <a href="#-key-literature">
    <img
      src="https://img.shields.io/badge/PAPER_LIST-Browse-0F766E?style=for-the-badge&logo=readthedocs&logoColor=white"
      alt="Paper list"
    >
  </a>
  <a href="https://discord.gg/fn5rYJhgaz">
    <img
      src="https://img.shields.io/badge/COMMUNITY-Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white"
      alt="Discord"
    >
  </a>
</p>

<p align="center">
  <a href="https://awesome.re">
    <img src="https://awesome.re/badge.svg" alt="Awesome">
  </a>
  <a href="LICENSE">
    <img
      src="https://img.shields.io/badge/License-MIT-F59E0B?labelColor=555555"
      alt="MIT License"
    >
  </a>
</p>

<p align="center">
  This repository accompanies
  <a href="https://arxiv.org/abs/2607.13104">
    <em>Self-Improvements in Modern Agentic Systems: A Survey</em>
  </a>.
</p>

---

## 🌐 Contents
- [Definition & Scope](#-definition--scope)
- [Survey Paper](#-survey-paper)
- [Taxonomy](#-taxonomy)
- [Key Literature](#-key-literature)
  - [🟦 Foundation Model Improvement](#-foundation-model-improvement)
  - [🟩 Scaffolding Improvement](#-scaffolding-improvement)
- [Evaluation & Benchmarking](#evaluation)
- [Related Resources](#-related-resources)
- [Contact & Community](#-contact--community)
- [Contribute](#-contribute)
- [Citation](#-citation)

---

## 🧩 Definition & Scope
This repository focuses on:
- **Foundation-Model-Based Agents**: Autonomous systems that use foundation models as cognitive cores and operate through persistent scaffolds such as prompts, memory, tools, and control logic.
- **Self-Improvement Loops**: Agent-level update loops in which signals or artifacts produced through generation, intrinsic evaluation, or environment interaction are consolidated into persistent components of the agent.
- **Foundation Model Improvement**: Parameter-level updates driven by intrinsic generative demonstrations, intrinsic evaluative feedback, or extrinsic exploratory experience.
- **Scaffolding Improvement**: Persistent updates to prompts, memory, tools, workflows, or full agent scaffolds.

---

## 📄 Survey Paper

|**[Self-Improvements in Modern Agentic Systems: A Survey](https://arxiv.org/abs/2607.13104)** | `arXiv:2607.13104` | [LaTeX source](./Paper/) | [Agent-oriented guide](./README_AGENT.md)|

<p align="center">
  <img src="assets/fig-si-main-001.png" alt="Main figure of the survey" width="95%">
  <br>
  <em>Overview of self-improvement mechanisms in foundation model–based agentic systems.</em>
</p>

---

## 🧭 Taxonomy

If you are not yet familiar with agents, this simple illustration shows how an **FM-based agent** differs from a standalone **foundation model** (e.g., an LLM).

<details open>
  <summary><strong>View the animated comparison</strong></summary>

  <br>

  <p align="center">
    <a href="assets/agentvsfm.gif">
      <img
        src="assets/agentvsfm.gif"
        alt="Animated comparison between a standalone foundation model and an agent"
        width="70%"
      >
    </a>
    <br>
    <em>
      An illustration of the distinction between a standalone foundation model and an FM-Based agent.
    </em>
  </p>
</details>

To ground our taxonomy, we first introduce a formal abstraction of a foundation model–based agent,
which serves as the basic unit for all self-improving agentic systems considered in this survey.

<p align="center">
  <img src="assets/agent_def.png" alt="Formal abstraction of an FM-based agent" width="55%">
  <br>
  <em>Formal abstraction of a foundation model–based agent, consisting of a foundation model and its scaffolding.</em>
</p>

Based on this abstraction, we categorize **self-improving agents** along two orthogonal axes,
depending on **which component is improved** during learning and adaptation.

* **🚀 Self-Improving Agents**
    * **🧠 Foundation Model Improvement**
        * 📄 `1.1` Intrinsic Generative Demonstrations
        * ⚖️ `1.2` Intrinsic Evaluative Feedback
        * 🌍 `1.3` Extrinsic Exploratory Experience
            * 🤖 `1.3.1` Interaction with Grounded Task Environments
            * 🔮 `1.3.2` Interaction with Simulated Proxy Environments
    * **🏗️ Scaffolding Improvement**
        * ✍️ `2.1` Prompt Optimization
        * 💾 `2.2` Memory
        * 🛠️ `2.3` Tool
        * ♾️ `2.4` Full Scaffolding

---

## 📚 Key Literature
### 🛣️ Evolution of Self-Improving Agents

<p align="center">
  <a href="assets/fig-si-rw-001.png">
    <img
      src="assets/fig-si-rw-001.png"
      alt="Timeline of representative self-improving agent systems"
      width="100%"
    >
  </a>
  <br>
  <em>
    Timeline of representative self-improving agent systems, organized by
    foundation model improvement and scaffolding improvement.
  </em>
</p>

### 🔖 Papers List

#### 🟦 Foundation Model Improvement

<details open>
<summary><b>1.1 Intrinsic Generative Demonstrations</b></summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2023 | Self-Instruct: Aligning Language Models with Self-Generated Instructions | ACL | [paper](https://arxiv.org/abs/2212.10560) | [code](https://github.com/yizhongw/self-instruct) |
  | 2023 | Large Language Models Can Self-Improve | EMNLP | [paper](https://arxiv.org/abs/2210.11610) | N/A |
  | 2023 | Orca: Progressive Learning from Complex Explanation Traces of GPT-4 | arXiv | [paper](https://arxiv.org/abs/2306.02707) | [code]( https://aka.ms/orca-lm) |
  | 2024 | SELF: Self-Evolution with Language Feedback | arXiv | [paper](https://arxiv.org/abs/2310.00533) | N/A |
  | 2024 | SELF-GUIDE: Better Task-Specific Instruction Following via Self-Synthetic Finetuning | COLM | [paper](https://arxiv.org/abs/2407.12874) | [code](https://github.com/zhaochenyang20/Prompt2Model-Self-Guide) |
  | 2025 | Improving Model Alignment Through Collective Intelligence of Open-Source LLMS | ICML | [paper](https://arxiv.org/abs/2505.03059) | N/A |
  | 2025 | Superficial Self-Improved Reasoners Benefit from Model Merging | EMNLP | [paper](https://arxiv.org/abs/2503.02103) | [code](https://github.com/xiangchi-yuan/merge_syn) |
  | 2025 | Will Pre-Training Ever End? A First Step Toward Next-Generation Foundation MLLMs via Self-Improving Systematic Cognition | arXiv | [paper](https://arxiv.org/abs/2503.12303) | [code](https://github.com/thunlp/SICOG?tab=readme-ov-file) |
  | 2025 | TaskCraft: Automated Generation of Agentic Tasks | arXiv | [paper](https://arxiv.org/abs/2506.10055) | [code](https://github.com/OPPO-PersonalAI/TaskCraft) |
  | 2025 | Iterative Tool Usage Exploration for Multimodal Agents via Step-wise Preference Tuning | NeurIPS | [paper](https://arxiv.org/abs/2504.21561) | [code](https://github.com/SPORT-Agents/SPORT-Agents) |
  | 2025 | Maximizing Confidence Alone Improves Reasoning | arXiv | [paper](https://arxiv.org/abs/2505.22660) | [code](https://github.com/satrams/rent-rl) |
  | 2025 | DIVE: Diversified Iterative Self-Improvement | arXiv | [paper](https://arxiv.org/abs/2501.00747) | [code](https://github.com/qinyiwei/DIVE) |
  | 2025 | Self-Adapting Language Models | NeurIPS | [paper](https://arxiv.org/abs/2506.10943) | [code](https://github.com/Continual-Intelligence/SEAL) |
  | 2025 | First SFT, Second RL, Third UPT: Continual Improving Multi-Modal LLM Reasoning via Unsupervised Post-Training | NeurIPS | [paper](https://arxiv.org/pdf/2505.22453) | [code](https://github.com/waltonfuture/MM-UPT) |
  | 2025 | LADDER: Self-Improving LLMs Through Recursive Problem Decomposition | arXiv | [paper](https://arxiv.org/abs/2503.00735) | N/A |
  | 2025 | Self-Consistency Preference Optimization | ICML | [paper](https://arxiv.org/abs/2411.04109) | N/A |
  | 2025 | Adapting While Learning: Grounding LLMs for Scientific Problems with Tool Usage Adaptation | ICML | [paper](https://arxiv.org/abs/2411.00412) | [code](https://github.com/Rose-STL-Lab/Adapting-While-Learning) |
  | 2026 | Reinforcing General Reasoning Without Verifiers | ICLR | [paper](https://arxiv.org/abs/2505.21493) | [code](https://github.com/sail-sg/VeriFree) |
  | 2026 | SAGE: Multi-Agent Self-Evolution for LLM Reasoning | arXiv | [paper](https://arxiv.org/abs/2603.15255) | N/A |
  | 2026 | ANDES: Agent Native Data Evolving Synthesis Tool for Autonomous Instruction Alignment | arXiv | [paper](https://arxiv.org/abs/2606.01279) | [code](https://github.com/zzy1127/ANDES) |
  | 2026 | EvoGround: Self-Evolving Video Agents for Video Temporal Grounding | arXiv | [paper](https://arxiv.org/abs/2605.13803) | [code](https://github.com/minjoong507/EvoGround) |

</details>

<details open>
<summary><b>1.2 Intrinsic Evaluative Feedback</b></summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2022 | Constitutional AI: Harmlessness from AI Feedback | arXiv | [paper](https://arxiv.org/abs/2212.08073) | [code](https://github.com/anthropics/ConstitutionalHarmlessnessPaper?tab=readme-ov-file) |
  | 2023 | ReST meets ReAct: Self-Improvement for Multi-Step Reasoning LLM Agent | arXiv | [paper](https://arxiv.org/abs/2312.10003) | N/A |
  | 2025 | STRIVE: Structured Reasoning for Self-Improvement in Claim Verification | MIR | [paper](https://arxiv.org/abs/2502.11959) | N/A |
  | 2025 | Beyond Accuracy: The Role of Calibration in Self-Improving Large Language Models | arXiv | [paper](https://arxiv.org/abs/2504.02902) | N/A |
  | 2025 | Self-Evolved Reward Learning for LLMs | ICLR | [paper](https://arxiv.org/abs/2411.00418) | [code](https://github.com/microsoft/DKI_LLM/tree/main/SER) |
  | 2025 | Sample, Predict, then Proceed: Self-Verification Sampling for Tool Use of LLMs | arXiv | [paper](https://arxiv.org/abs/2506.02918v1) | N/A |
  | 2025 | RLSR: Reinforcement Learning from Self Reward | arXiv | [paper](https://arxiv.org/abs/2505.08827) | N/A |
  | 2025 | Right Question is Already Half the Answer: Fully Unsupervised LLM Reasoning Incentivization | NeurIPS | [paper](https://arxiv.org/abs/2504.05812) | [code](https://github.com/QingyangZhang/EMPO) |
  | 2025 | TTRL: Test-Time Reinforcement Learning | NeurIPS | [paper](https://arxiv.org/abs/2504.16084) | [code](https://github.com/PRIME-RL/TTRL) |
  | 2025 | Can Large Reasoning Models Self-Train? | arXiv | [paper](https://arxiv.org/abs/2505.21444) | [code](https://github.com/tajwarfahim/srt) |
  | 2025 | Self Rewarding Self Improving | arXiv | [paper](https://arxiv.org/abs/2505.08827v1) | N/A |
  | 2025 | Self-Evolving Curriculum for LLM Reasoning | arXiv | [paper](https://arxiv.org/abs/2505.14970) | [code](https://github.com/ServiceNow/sec) |
  | 2025 | Reflect, Retry, Reward: Self-Improving LLMs via Reinforcement Learning | arXiv | [paper](https://arxiv.org/abs/2505.24726) | N/A |
  | 2025 | Adaptive Self-improvement LLM Agentic System for ML Library Development | ICML | [paper](https://arxiv.org/abs/2502.02534) | [code](https://github.com/zhang677/PCL-lite) |
  | 2026 | Learning to Reason without External Rewards | ICLR | [paper](https://arxiv.org/abs/2505.19590) | [code](https://github.com/sunblaze-ucb/Intuitor) |
  | 2026 | Structured Reasoning for Large Language Models | arXiv | [paper](https://arxiv.org/abs/2601.07180) | N/A |
  | 2026 | iReasoner: Trajectory-Aware Intrinsic Reasoning Supervision for Self-Evolving Large Multimodal Models | arXiv | [paper](https://arxiv.org/abs/2601.07180) | [code](https://github.com/meghanaasunil/iReasoner) |
  | 2026 | STRIVE: Structured Reasoning for Self-improvement in Claim Verification | machine intelligence research | [paper](https://link.springer.com/article/10.1007/s11633-025-1598-5) | N/A |
  | 2026 | UniCorn: Towards Self-Improving Unified Multimodal Models through Intrinsic Evaluative Feedback | arXiv | [paper](https://arxiv.org/abs/2601.03193) | [code]([https://github.com/meghanaasunil/iReasoner](https://github.com/Hungryyan1/UniCorn)) |
  | 2026 | Retrospective Progress-Aware Self-Refinement for LLM Agent Training | arXiv | [paper](https://arxiv.org/abs/2606.14302) | N/A |
  | 2026 | EVE-Agent: Evidence-Verifiable Self-Evolving Agents | arXiv | [paper](https://arxiv.org/abs/2605.22905) | N/A |

</details>

<details open>
<summary><b>1.3 Extrinsic Exploratory Experience</b></summary>

- **1.3.1 Interaction with Grounded Task Environments**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2023 | RoboCat: A Self-Improving Generalist Agent for Robotic Manipulation | TMLR | [paper](https://arxiv.org/abs/2306.11706) | [code](https://github.com/keirp/automatic_prompt_engineer) |
  | 2025 | Tool-Star: Empowering LLM-Brained Multi-Tool Reasoner via Reinforcement Learning | arXiv | [paper](https://arxiv.org/abs/2505.16410) | [code](https://github.com/RUC-NLPIR/Tool-Star) |
  | 2025 | CodeARC: Benchmarking Reasoning Capabilities of LLM Agents for Inductive Program Synthesis | COLM | [paper](https://arxiv.org/abs/2503.23145) | [code](https://github.com/Anjiang-Wei/CodeARC) |
  | 2025 | LLMs are Greedy Agents: Effects of RL Fine-tuning on Decision-Making Abilities | arXiv | [paper](https://arxiv.org/abs/2504.16078) | N/A |
  | 2025 | Agent-RLVR: Training Software Engineering Agents via Guidance and Environment Rewards | arXiv | [paper](https://arxiv.org/abs/2506.11425) | N/A |
  | 2025 | WebRL: Training LLM Web Agents via Self-Evolving Online Curriculum Reinforcement Learning | ICLR | [paper](https://arxiv.org/abs/2411.02337) | [code](https://github.com/THUDM/WebRL) |
  | 2025 | Self-Improving Language Models for Evolutionary Program Synthesis: A Case Study on ARC-AGI | ICML | [paper](https://arxiv.org/abs/2507.14172) | [code](https://github.com/flowersteam/SOAR) |
  | 2025 | DeepResearcher: Scaling Deep Research via Reinforcement Learning in Real-world Environments | arXiv | [paper](https://arxiv.org/abs/2504.03160) | [code](https://github.com/GAIR-NLP/DeepResearcher) |
  | 2025 | Agentic Reasoning and Tool Integration for LLMs via Reinforcement Learning | arXiv | [paper](https://arxiv.org/abs/2505.01441v1) | N/A |
  | 2025 | UI-Genie: A Self-Improving Approach for Iteratively Boosting MLLM-based Mobile GUI Agents | NeurIPS | [paper](https://arxiv.org/abs/2505.21496) | [code](https://github.com/Euphoria16/UI-Genie) |
  | 2025 | RAGEN: Understanding Self-Evolution in LLM Agents via Multi-Turn Reinforcement Learning | arXiv | [paper](https://arxiv.org/abs/2504.20073) | [code](https://github.com/mll-lab-nu/RAGEN) |
  | 2025 | SEAgent: Self-Evolving Computer Use Agent with Autonomous Learning from Experience | arXiv | [paper](https://arxiv.org/abs/2508.04700) | [code](https://github.com/SunzeY/SEAgent) |
  | 2026 | WebGym: Scaling Training Environments for Visual Web Agents with Realistic Tasks | arXiv | [paper](https://arxiv.org/abs/2601.02439) | [code](https://github.com/microsoft/webgym) |
  | 2026 | Kevin: Multi-Turn RL for Generating CUDA Kernels | ICLR | [paper](https://openreview.net/pdf?id=xu1XwVZtDi) | N/A |
  | 2026 | Tool-R0: Self-Evolving LLM Agents for Tool-Learning from Zero Data | arXiv | [paper](https://arxiv.org/abs/2602.21320) | [code](https://github.com/emrecanacikgoz/Tool-R0) |
  | 2026 | Socratic-SWE: Self-Evolving Coding Agents via Trace-Derived Agent Skills | arXiv | [paper](https://arxiv.org/abs/2606.07412) | N/A |
  | 2026 | Self-evolving LLM Agents with In-Distribution Optimization | ICML | [paper](https://arxiv.org/abs/2606.07367) | N/A |
  | 2026 | Skill Self-Play: Pushing the Frontier of LLM Capability with Co-Evolving Skills | arXiv | [paper](https://arxiv.org/abs/2607.22529) | [code](https://github.com/Qwen-Applications/skill-self-play) |

  </details>

- **1.3.2 Interaction with Simulated Proxy Environments**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2023 | Language Models Meet World Models: Embodied Experiences Enhance Language Models | NeurIPS | [paper](https://arxiv.org/abs/2305.10626) | [code](https://github.com/szxiangjn/world-model-for-language-model) |
  | 2024 | Agent Planning with World Knowledge Model | NeurIPS | [paper](https://arxiv.org/abs/2405.14205) | [code](https://github.com/zjunlp/WKM) |
  | 2025 | Web Agents with World Models: Learning and Leveraging Environment Dynamics in Web Navigation | ICLR | [paper](https://arxiv.org/abs/2410.13232) | [code](https://github.com/kyle8581/WMA-Agents) |
  | 2025 | Understanding World or Predicting Future? A Comprehensive Survey of World Models | ACM CSUR | [paper](https://arxiv.org/abs/2411.14499) | [code](https://github.com/tsinghua-fib-lab/World-Model) |
  | 2025 | General agents contain world models | ICML | [paper](https://arxiv.org/abs/2506.01622) | N/A |
  | 2025 | WebEvolver: Enhancing Web Agent Self-Improvement with Coevolving World Model | EMNLP | [paper](https://arxiv.org/abs/2504.21024) | [code](https://github.com/Tencent/SelfEvolvingAgent) |
  | 2025 | WebSynthesis: World-Model-Guided MCTS for Efficient WebUI-Trajectory Synthesis | arXiv | [paper](https://arxiv.org/abs/2507.04370) | [code](https://github.com/LucusFigoGao/WebSynthesis) |
  | 2025 | GAWM: Global-Aware World Model for Multi-Agent Reinforcement Learning | arXiv | [paper](https://arxiv.org/abs/2501.10116) | N/A |
  | 2025 | WMPO: World Model-based Policy Optimization for Vision-Language-Action Models | arXiv | [paper](https://arxiv.org/abs/2511.09515) | [code](https://github.com/WM-PO/WMPO) |
  | 2025 | Internalizing World Models via Self-Play Finetuning for Agentic RL | arXiv | [paper](https://arxiv.org/abs/2510.15047) | N/A |
  | 2026 | AlignUSER: Human-Aligned LLM Agents via World Models for Recommender System Evaluation | arXiv | [paper](https://arxiv.org/abs/2601.00930) | N/A |
  | 2026 | WorldEvolver: Self-Evolving World Models for LLM Agent Planning | arXiv | [paper](https://arxiv.org/abs/2606.30639) | N/A |
  | 2025 | NavMorph: A Self-Evolving World Model for Vision-and-Language Navigation in Continuous Environments | ICCV | [paper](https://arxiv.org/abs/2506.23468) | [code](https://github.com/Feliciaxyao/NavMorph) |
  | 2025 | EvoWorld: Evolving Panoramic World Generation with Explicit 3D Memory | arXiv | [paper](https://arxiv.org/abs/2510.01183) | N/A |
  | 2026 | RISE: Self-Improving Robot Policy with Compositional World Model | RSS | [paper](https://arxiv.org/abs/2602.11075) | [code](https://github.com/OpenDriveLab/RISE) |

  </details>
  
</details>


#### 🟩 Scaffolding Improvement

<details open>
<summary><b>2.1 Prompt Optimization</b></summary>

- **2.1.1 Scalar-Feedback Optimization**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2022 | Large Language Models Are Human-Level Prompt Engineers | arXiv | [paper](https://arxiv.org/abs/2211.01910) | [code](https://github.com/keirp/automatic_prompt_engineer) |
  | 2024 | Large Language Models as Optimizers | ICLR | [paper](https://arxiv.org/abs/2309.03409) | [code](https://github.com/google-deepmind/opro) |
  | 2024 | Prompt Refinement with Image Pivot for Text-to-Image Generation | ACL | [paper](https://arxiv.org/abs/2407.00247) | [code](https://github.com/jingtaozhan/PromptReformulate) |
  | 2024 | Learning from Contrastive Prompts: Automated Optimization and Adaptation | arXiv | [paper](https://arxiv.org/abs/2409.15199) | N/A |
  | 2024 | PRompt Optimization in Multi-Step Tasks (PROMST): Integrating Human Feedback and Heuristic-based Sampling | EMNLP | [paper](https://arxiv.org/abs/2402.08702) | [code](https://github.com/yongchao98/PROMST) |
  | 2025 | The Prompt Alchemist: Automated LLM-Tailored Prompt Optimization for Test Case Generation | arXiv | [paper](https://arxiv.org/abs/2501.01329) | N/A |
  | 2025 | DRO-InstructZero: Distributionally Robust Prompt Optimization for Large Language Models | arXiv | [paper](https://arxiv.org/abs/2510.15260) | N/A |
  | 2025 | CoolPrompt: Automatic Prompt Optimization Framework for Large Language Models | FRUCT | [paper](https://ieeexplore.ieee.org/document/11239071) | N/A |
  | 2026 | SePO: Self-Evolving Prompt Agent for System Prompt Optimization | arXiv | [paper](https://arxiv.org/abs/2606.04465) | [code](https://github.com/taowangcheng/SePO) |
  | 2026 | SAGE: Stochastic Prompt Optimization via Agent-Guided Exploration | arXiv | [paper](https://arxiv.org/abs/2606.18902) | N/A |

  </details>

- **2.1.2 Qualitative-Feedback Refinement**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2023 | Self-Refine: Iterative Refinement with Self-Feedback | arXiv | [paper](https://arxiv.org/abs/2303.17651) | [code](https://github.com/madaan/self-refine) |
  | 2023 | Chain of Hindsight Aligns Language Models with Feedback | arXiv | [paper](https://arxiv.org/abs/2302.02676) | [code](https://github.com/haoliuhl/chain-of-hindsight) |
  | 2023 | Reflexion: Language Agents with Verbal Reinforcement Learning | NeurIPS  | [paper](https://arxiv.org/abs/2303.11366) | [code](https://github.com/noahshinn/reflexion) |
  | 2024 | Self-Improving Customer Review Response Generation Based on LLMs | COLING  | [paper](https://arxiv.org/abs/2405.03845) | N/A |
  | 2024 | Prompt Optimization with Human Feedback | ICML Workshop | [paper](https://arxiv.org/abs/2405.17346) | [code](https://github.com/xqlin98/APOHF) |
  | 2024 | Optimizing Instructions and Demonstrations for Multi-Stage Language Model Programs | EMNLP | [paper](https://arxiv.org/abs/2406.11695) | [code](https://dspy.ai/) |
  | 2025 | CriSPO: Multi-Aspect Critique-Suggestion-guided Automatic Prompt Optimization for Text Generation | AAAI | [paper](https://arxiv.org/abs/2410.02748) | [code](https://github.com/amazon-science/CriSPO) |
  | 2025 | Boosting Private Domain Understanding of Efficient MLLMs: A Tuning-free, Adaptive, Universal Prompt Optimization Framework | arXiv | [paper](https://arxiv.org/abs/2412.19684) | N/A |
  | 2026 | GEPA: Reflective Prompt Evolution Can Outperform Reinforcement Learning | ICLR | [paper](https://arxiv.org/abs/2507.19457) | [code](https://github.com/gepa-ai/gepa) |
  | 2026 | FORGE: Self-Evolving Agent Memory With No Weight Updates via Population Broadcast | CAIS | [paper](https://arxiv.org/abs/2605.16233) | N/A |

  </details>

- **2.1.3 Population-Based Evolution**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2023 | Promptbreeder: Self-Referential Self-Improvement Via Prompt Evolution | arXiv | [paper](https://arxiv.org/abs/2309.16797) | N/A |
  | 2024 | EvoPrompt: Connecting LLMs with Evolutionary Algorithms Yields Powerful Prompt Optimizers | ICLR | [paper](https://arxiv.org/abs/2309.08532) | [code](https://github.com/beeevita/EvoPrompt) |
  | 2024 | WizardLM: Empowering large pre-trained language models to follow complex instructions | ICLR | [paper](https://arxiv.org/abs/2304.12244) | [code](https://github.com/nlpxucan/WizardLM) |
  | 2025 | Tournament of Prompts: Evolving LLM Instructions Through Structured Debates and Elo Ratings | KDD | [paper](https://arxiv.org/abs/2506.00178v2) | N/A |
  | 2025 | DelvePO: Direction-Guided Self-Evolving Framework for Flexible Prompt Optimization | arXiv | [paper](https://arxiv.org/abs/2510.18257) | [code](https://github.com/PasaLab/DelvePO) |
  | 2025 | How to Auto-optimize Prompts for Domain Tasks? Adaptive Prompting and Reasoning through Evolutionary Domain Knowledge Adaptation | NeurIPS | [paper](https://arxiv.org/abs/2510.21148) | [code](https://github.com/miemieyanga/EGO-Prompt) |

  </details>

- **2.1.4 Textual Gradient Optimization**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2023 | Automatic Prompt Optimization with "Gradient Descent" and Beam Search | EMNLP  | [paper](https://arxiv.org/abs/2305.03495) | [code](https://github.com/microsoft/LMOps/tree/main/prompt_optimization) |
  | 2024 | How to Correctly do Semantic Backpropagation on Language-based Agentic Systems | arXiv  | [paper](https://arxiv.org/abs/2412.03624) | [code](https://github.com/HishamAlyahya/semantic_backprop) |
  | 2024 | Trace is the Next AutoDiff: Generative Optimization with Rich Feedback, Execution Traces, and LLMs | NeurIPS | [paper](https://arxiv.org/abs/2406.16218) | [code](https://github.com/microsoft/trace) |
  | 2025 | TextGrad: Automatic "Differentiation" via Text | Nature | [paper](https://arxiv.org/abs/2406.07496) | [code](https://github.com/zou-group/textgrad) |
  | 2025 | metaTextGrad: Automatically optimizing language model optimizers | NeurIPS | [paper](https://arxiv.org/abs/2505.18524) | [code](https://github.com/zou-group/metatextgrad) |
  | 2025 | MAPGD: Multi-Agent Prompt Gradient Descent for Collaborative Prompt Optimization | NeurIPS Workshop | [paper](https://openreview.net/pdf?id=FywYwwH5z9) | N/A |
  | 2025 | Scaling Textual Gradients via Sampling-Based Momentum | ICML | [paper](https://arxiv.org/abs/2506.00400) | N/A |
  | 2026 | Pick Your Textual Gradients | arXiv | [paper](https://openreview.net/pdf?id=ydTwv5D536) | N/A |
  | 2026 | SkillOpt: Executive Strategy for Self-Evolving Agent Skills | arXiv | [paper](https://arxiv.org/abs/2605.23904) | [code](https://github.com/microsoft/SkillOpt) |
  | 2026 | VASO: Formally Verifiable Self-Evolving Skills for Physical AI Agents | arXiv | [paper](https://arxiv.org/abs/2606.05395) | N/A |
  | 2026 | Learning to Evolve: A Self-Improving Framework for Multi-Agent Systems | ACL Findings | [paper](https://arxiv.org/abs/2604.20714) | N/A |
  | 2026 | Learning to Learn-at-Test-Time: Language Agents with Learnable Adaptation Policies | arXiv | [paper](https://arxiv.org/abs/2604.00830) | [code](https://github.com/zzzlou/meta-ttl) |

  </details>
  
</details>

<details open>
<summary><b>2.2 Memory</b></summary>

- **2.2.1 Memory Object**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2023 | Learning to Reason and Memorize with Self-Notes | NeurIPS  | [paper](https://arxiv.org/abs/2305.00833) | N/A |
  | 2024 | ExpeL: LLM Agents Are Experiential Learners | AAAI  | [paper](https://arxiv.org/abs/2308.10144) | [code](https://github.com/LeapLabTHU/ExpeL) |
  | 2024 | A Human-Inspired Reading Agent with Gist Memory of Very Long Contexts | ICML  | [paper](https://arxiv.org/abs/2402.09727) | N/A |
  | 2024 | CodeAgent: Enhancing Code Generation with Tool-Integrated Agent Systems for Real-World Repo-level Coding Challenges | ACL | [paper](https://arxiv.org/abs/2401.07339) | N/A |
  | 2024 | MEMORYLLM: Towards Self-Updatable Large Language Models | ICML | [paper](https://arxiv.org/abs/2402.04624) | [code](https://github.com/wangyu-ustc/MemoryLLM) |
  | 2025 | Agent Workflow Memory | ICML | [paper](https://arxiv.org/abs/2409.07429) | [code](https://github.com/zorazrw/agent-workflow-memory) |
  | 2025 | ReasoningBank: Scaling Agent Self-Evolving with Reasoning Memory | arXiv | [paper](https://arxiv.org/abs/2509.25140) | N/A |
  | 2025 | Seeing, Listening, Remembering, and Reasoning: A Multimodal Agent with Long-Term Memory | arXiv  | [paper](https://arxiv.org/abs/2508.09736) | [code](https://github.com/bytedance-seed/m3-agent) |
  | 2025 | Dynamic Cheatsheet: Test-Time Learning with Adaptive Memory | arXiv  | [paper](https://arxiv.org/abs/2305.00833) | [code](https://github.com/suzgunmirac/dynamic-cheatsheet) |
  | 2025 | PRIME: Planning and Retrieval-Integrated Memory for Enhanced Reasoning | AAAI | [paper](https://arxiv.org/abs/2509.22315) | N/A |
  | 2025 | Contextual Memory Reweaving in Large Language Models Using Layered Latent State Reconstruction | arXiv | [paper]() | [code]() |
  | 2025 | MemGen: Weaving Generative Latent Memory for Self-Evolving Agents | arXiv | [paper](https://arxiv.org/abs/2509.24704) | [code](https://github.com/bingreeky/MemGen) |
  | 2025 | M+: Extending MemoryLLM with Scalable Long-Term Memory | arXiv | [paper](https://arxiv.org/abs/2502.00592) | [code](https://github.com/wangyu-ustc/MemoryLLM) |
  | 2026 | Seeing, Listening, Remembering, and Reasoning: A Multimodal Agent with Long-Term Memory | ICLR | [paper](https://arxiv.org/abs/2508.09736) | [code](https://github.com/bytedance-seed/m3-agent) |
  | 2026 | Thought-Retriever: Don't Just Retrieve Raw Data, Retrieve Thoughts for Memory-Augmented Agentic Systems | arXiv | [paper](https://arxiv.org/abs/2604.12231) | N/A |
  | 2026 | Better with Experience: Self-Evolving LLM Agents for Evidence-Grounded Health Community Notes | arXiv | [paper](https://arxiv.org/abs/2606.02215) | N/A |
  | 2026 | Agon: An Autonomous Large-Scale Omnidisciplinary Research System Built on Prompt Economy | arXiv | [paper](https://arxiv.org/abs/2606.24177) | [code](https://github.com/AutoResearch-Factory/Agon) |

  </details>

- **2.2.2 Memory Structure**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2022 | XMem: Long-Term Video Object Segmentation with an Atkinson-Shiffrin Memory Model | ECCV  | [paper](https://arxiv.org/abs/2207.07115) | [code](https://github.com/hkchengrex/XMem) |
  | 2023 | Generative Agents: Interactive Simulacra of Human Behavior | UIST'23 | [paper](https://dl.acm.org/doi/10.1145/3586183.3606763) | N/A |
  | 2024 | MemoryBank: Enhancing Large Language Models with Long-Term Memory | arXiv | [paper](https://arxiv.org/abs/2305.10250) | [code](https://github.com/zhongwanjun/MemoryBank-SiliconFriend) |
  | 2024 | MovieChat: From Dense Token to Sparse Memory for Long Video Understanding | CVPR | [paper](https://arxiv.org/abs/2307.16449) | [code](https://github.com/rese1f/MovieChat) |
  | 2024 | Explore, Select, Derive, and Recall: Augmenting LLM with Human-like Memory for Mobile Task Automation | ACM MobiCom | [paper](https://arxiv.org/abs/2312.03003) | [code](https://github.com/mobilegptsys/MobileGPT) |
  | 2025 | SCM: Enhancing Large Language Model with Self-Controlled Memory Framework | DASFAA | [paper](https://arxiv.org/abs/2304.13343) | [code](https://github.com/wbbeyourself/SCM4LLMs) |
  | 2025 | Hierarchical Memory for High-Efficiency Long-Term Reasoning in LLM Agents | arXiv | [paper](https://arxiv.org/abs/2507.22925) | N/A |
  | 2025 | SALM: A Multi-Agent Framework for Language Model-Driven Social Network Simulation | arXiv | [paper](https://arxiv.org/abs/2505.09081) | N/A |
  | 2025 | Mem0: Building Production-Ready AI Agents with Scalable Long-Term Memory | arXiv | [paper](https://arxiv.org/abs/2504.19413) | [code](https://mem0.ai/research) |
  | 2025 | G-Memory: Tracing Hierarchical Memory for Multi-Agent Systems | NeurIPS | [paper](https://arxiv.org/abs/2506.07398) | [code](https://github.com/bingreeky/GMemory) |
  | 2025 | Zep: A Temporal Knowledge Graph Architecture for Agent Memory | arXiv | [paper](https://arxiv.org/abs/2501.13956) | N/A |
  | 2025 | SGMem: Sentence Graph Memory for Long-Term Conversational Agents | arXiv | [paper](https://arxiv.org/abs/2509.21212) | N/A |
  | 2025 | CausalRAG: Integrating Causal Graphs into Retrieval-Augmented Generation | ACL | [paper](https://arxiv.org/abs/2503.19878) | [code](https://github.com/Pwnb/CausalRAG) |
  | 2025 | GraphVideoAgent: Enhancing Long-form Video Understanding with Entity Relation Graphs | MM'25 | [paper](https://dl.acm.org/doi/abs/10.1145/3746027.3755537) | N/A |
  | 2025 | Decentralizing AI Memory: SHIMI, a Semantic Hierarchical Memory Index for Scalable Agent Reasoning | arXiv | [paper](https://arxiv.org/abs/2504.06135) | N/A |
  | 2025 | From Knowledge to Noise: CTIM-Rover and the Pitfalls of Episodic Memory in Software Engineering Agents | ACL Workshop | [paper](https://arxiv.org/abs/2505.23422v1) | [code](https://github.com/Liqs-v2/ctim-rover) |
  | 2025 | In Prospect and Retrospect: Reflective Memory Management for Long-term Personalized Dialogue Agents | ACL | [paper](https://arxiv.org/abs/2503.08026) | N/A |
  | 2025 | MrSteve: Instruction-Following Agents in Minecraft with What-Where-When Memory | ICLR | [paper](https://openreview.net/pdf?id=CjXaMI2kUH) | [code](https://github.com/frechele/MrSteve) |
  | 2026 | EvolveMem: Self-Evolving Memory Architecture via AutoResearch for LLM Agents | arXiv | [paper](https://arxiv.org/abs/2605.13941) | [code](https://github.com/aiming-lab/SimpleMem) |
  | 2026 | SAGE: A Self-Evolving Agentic Graph-Memory Engine for Structure-Aware Associative Memory | arXiv | [paper](https://arxiv.org/abs/2605.12061) | N/A |
  | 2026 | Prism: An Evolutionary Memory Substrate for Multi-Agent Open-Ended Discovery | arXiv | [paper](https://arxiv.org/abs/2604.19795) | N/A |
  | 2026 | DecentMem: Self-Evolving Multi-Agent Systems via Decentralized Memory | arXiv | [paper](https://arxiv.org/abs/2605.22721) | N/A |
  | 2026 | EXG: Self-Evolving Agents with Experience Graphs | arXiv | [paper](https://arxiv.org/abs/2605.17721) | N/A |
  | 2026 | CLAG: Adaptive Memory Organization via Agent-Driven Clustering for Small Language Model Agents | ACL Findings | [paper](https://arxiv.org/abs/2603.15421) | [code](https://github.com/dmis-lab/CLAG) |

  </details>

- **2.2.3 Memory Processing**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2023 | Generative Agents: Interactive Simulacra of Human Behavior | UIST | [paper](https://arxiv.org/abs/2304.03442) | [code](https://github.com/joonspk-research/generative_agents) |
  | 2024 | WizardLM: Empowering large pre-trained language models to follow complex instructions | ICLR | [paper](https://arxiv.org/abs/2509.09498) | N/A |
  | 2025 | SEDM: Scalable Self-Evolving Distributed Memory for Agents | ICLR | [paper](https://arxiv.org/abs/2309.08532) | [code](https://github.com/beeevita/EvoPrompt) |
  | 2025 | MemInsight: Autonomous Memory Augmentation for LLM Agents | arXiv | [paper](https://arxiv.org/abs/2503.21760) | N/A |
  | 2025 | MemGen: Weaving Generative Latent Memory for Self-Evolving Agents | arXiv | [paper](https://arxiv.org/abs/2509.24704) | [code](https://github.com/KANABOON1/MemGen) |
  | 2025 | A-MEM: Agentic Memory for LLM Agents | NeurIPS | [paper](https://arxiv.org/abs/2502.12110) | [code](https://github.com/WujiangXu/A-mem-sys) |
  | 2025 | G-Memory: Tracing Hierarchical Memory for Multi-Agent Systems | arXiv | [paper](https://arxiv.org/abs/2506.07398) | [code](https://github.com/bingreeky/GMemory) |
  | 2025 | Mem0: Building Production-Ready AI Agents with Scalable Long-Term Memory | arXiv | [paper](https://arxiv.org/abs/2504.19413) | [code](https://mem0.ai/research) |
  | 2025 | Agentic Retrieval-Augmented Generation: A Survey on Agentic RAG | arXiv | [paper](https://arxiv.org/abs/2501.09136) | [code](https://github.com/asinghcsu/AgenticRAG-Survey) |
  | 2025 | Memory OS of AI Agent | EMNLP | [paper](https://arxiv.org/abs/2506.06326) | [code](https://github.com/BAI-LAB/MemoryOS) |
  | 2025 | SCM: Enhancing Large Language Model with Self-Controlled Memory Framework | DASFAA | [paper](https://arxiv.org/abs/2304.13343) | [code](https://github.com/wbbeyourself/SCM4LLMs) |
  | 2025 | Dynamic Cheatsheet: Test-Time Learning with Adaptive Memory | arXiv | [paper](https://arxiv.org/abs/2504.07952) | [code](https://github.com/suzgunmirac/dynamic-cheatsheet) |
  | 2025 | MLC-Agent: Cognitive Model based on Memory-Learning Collaboration in LLM Empowered Agent Simulation Environment | arXiv | [paper](https://arxiv.org/abs/2507.20215) | N/A |
  | 2025 | MemInsight: Autonomous Memory Augmentation for LLM Agents | arXiv | [paper](https://arxiv.org/abs/2503.21760) | N/A |
  | 2026 | Agentic Context Engineering: Evolving Contexts for Self-Improving Language Models | ICLR | [paper](https://arxiv.org/abs/2510.04618) | [code](https://github.com/ace-agent/ace) |
  | 2026 | MemRL: Self-Evolving Agents via Runtime Reinforcement Learning on Episodic Memory | arXiv | [paper](https://arxiv.org/abs/2601.03192) | [code](https://github.com/MemTensor/MemRL) |
  | 2026 | TMEM: Scaling Self-Evolving Agents via Parametric Memory | arXiv | [paper](https://arxiv.org/abs/2606.04536) | N/A |
  | 2026 | MemQ: Integrating Q-Learning into Self-Evolving Memory for LLM Agents | arXiv | [paper](https://arxiv.org/abs/2605.08374) | [code](https://github.com/jwliao-ai/MemQ) |
  | 2026 | Memory Beyond Recall: A Dual-Process Cognitive Memory System for Self-Evolving Agents | arXiv | [paper](https://arxiv.org/abs/2606.09483) | N/A |
  | 2026 | AEL: Agent Evolving Learning for Open-Ended Environments | arXiv | [paper](https://arxiv.org/abs/2604.21725) | [code](https://github.com/WujiangXu/AEL) |
  | 2026 | Metis: Bridging Text and Code Memory for Self-Evolving Agents | arXiv | [paper](https://arxiv.org/abs/2606.24151) | N/A |
  | 2026 | Mem^2Evolve: Towards Self-Evolving Agents via Co-Evolutionary Capability Expansion and Experience Distillation | arXiv | [paper](https://arxiv.org/abs/2604.10923) | [code](https://github.com/BUAA-IRIP-LLM/Mem2Evolve) |

  </details>

</details>

<details open>
<summary><b>2.3 Tool</b></summary>

- **2.3.1 Dynamic Tool Routing**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2023 | Voyager: An Open-Ended Embodied Agent with Large Language Models | arXiv | [paper](https://arxiv.org/abs/2305.16291) | [code](https://github.com/MineDojo/Voyager) |
  | 2024 | ToolNet: Connecting Large Language Models with Massive Tools via Tool Graph | arXiv | [paper](https://arxiv.org/abs/2403.00839) | N/A |
  | 2025 | AgentOrchestra: Orchestrating Hierarchical Multi-Agent Intelligence with the Tool-Environment-Agent(TEA) Protocol | arXiv | [paper](https://arxiv.org/abs/2506.12508) | N/A |
  | 2025 | MetaAgent: Toward Self-Evolving Agent via Tool Meta-Learning | arXiv | [paper](https://arxiv.org/abs/2508.00271) | [code](https://github.com/qhjqhj00/MetaAgent) |
  | 2025 | OrchDAG: Complex Tool Orchestration in Multi-Turn Interactions with Plan DAGs | NeurIPS Workshop | [paper](https://arxiv.org/abs/2510.24663) | N/A |
  | 2025 | AutoTIR: Autonomous Tools Integrated Reasoning via Reinforcement Learning | arXiv | [paper](https://arxiv.org/abs/2507.21836) | [code](https://github.com/weiyifan1023/AutoTIR) |
  | 2025 | MCP-Flow: Facilitating LLM Agents to Master Real-World, Diverse and Scaling MCP Tools | arXiv | [paper](https://arxiv.org/abs/2510.24284) | [code](https://github.com/wwh0411/MCP-Flow) |
  | 2025 | In-the-Flow Agentic System Optimization for Effective Planning and Tool Use | NeurIPS | [paper](https://arxiv.org/abs/2510.05592) | [code](https://github.com/lupantech/AgentFlow) |
  | 2025 | MassTool: A Multi-Task Search-Based Tool Retrieval Framework for Large Language Models | arXiv | [paper](https://arxiv.org/abs/2507.00487) | [code](https://github.com/wxydada/MassTool) |
  | 2025 | AgentOrchestra: Orchestrating Multi-Agent Intelligence with the Tool-Environment-Agent(TEA) Protocol | arXiv | [paper](https://arxiv.org/abs/2506.12508) | N/A |
  | 2025 | Iterative Tool Usage Exploration for Multimodal Agents via Step-wise Preference Tuning | NeurIPS | [paper](https://arxiv.org/abs/2504.21561) | [code](https://github.com/SPORT-Agents/SPORT-Agents) |
  | 2025 | Tool-Star: Empowering LLM-Brained Multi-Tool Reasoner via Reinforcement Learning | arXiv | [paper](https://arxiv.org/abs/2505.16410) | [code](https://github.com/RUC-NLPIR/Tool-Star) |
  | 2025 | MCP-Zero: Active Tool Discovery for Autonomous LLM Agents | arXiv | [paper](https://arxiv.org/abs/2506.01056v4) | [code](https://github.com/xfey/MCP-Zero) |
  | 2025 | AskToAct: Enhancing LLMs Tool Use via Self-Correcting Clarification | arXiv | [paper](https://arxiv.org/abs/2503.01940) | N/A |
  | 2025 | MemTool: Optimizing Short-Term Memory Management for Dynamic Tool Calling in LLM Agent Multi-Turn Conversations | arXiv | [paper](https://arxiv.org/abs/2507.21428) | N/A |
  | 2025 | Tool-Planner: Task Planning with Clusters across Multiple Tools | ICLR | [paper](https://arxiv.org/abs/2406.03807) | [code](https://github.com/OceannTwT/Tool-Planner) |
  | 2025 | Tool-to-Agent Retrieval: Bridging Tools and Agents for Scalable LLM Multi-Agent Systems | arXiv | [paper](https://arxiv.org/abs/2511.01854) | N/A |
  | 2025 | ToolGen: Unified Tool Retrieval and Calling via Generation | ICLR | [paper](https://arxiv.org/abs/2410.03439) | [code](https://github.com/Reason-Wang/ToolGen) |
  | 2026 | ToolACE-R: Model-aware Iterative Training and Adaptive Refinement for Tool Learning | AAAI | [paper](https://arxiv.org/abs/2504.01400) | [code]() |
  | 2026 | DeepAgent: A General Reasoning Agent with Scalable Toolsets | WWW | [paper](https://arxiv.org/abs/2510.21618) | [code](https://github.com/RUC-NLPIR/DeepAgent) |
  | 2026 | DeepEyesV2: Toward Agentic Multimodal Model | ICLR | [paper](https://arxiv.org/abs/2511.05271) | [code](https://github.com/Visual-Agent/DeepEyesV2) |
  | 2026 | In-the-Flow Agentic System Optimization for Effective Planning and Tool Use | ICLR | [paper](https://arxiv.org/abs/2510.05592) | [code](https://github.com/lupantech/AgentFlow) |
  | 2026 | GenericAgent: A Token-Efficient Self-Evolving LLM Agent via Contextual Information Density Maximization | arXiv | [paper](https://arxiv.org/abs/2604.17091) | [code](https://github.com/lsdefine/GenericAgent) |
  | 2026 | ANDES: Agent Native Data Evolving Synthesis Tool for Autonomous Instruction Alignment | arXiv | [paper](https://arxiv.org/abs/2606.01279) | [code](https://github.com/zzy1127/ANDES) |


  </details>

- **2.3.2 Iterative Tool Refinement**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2023 | Voyager: An Open-Ended Embodied Agent with Large Language Models | arXiv | [paper](https://arxiv.org/abs/2305.16291) | [code](https://github.com/MineDojo/Voyager) |
  | 2025 | STELLA: Self-Evolving LLM Agent for Biomedical Research | arXiv | [paper](https://arxiv.org/abs/2507.02004) | [code](https://github.com/zaixizhang/STELLA) |
  | 2025 | SkillWeaver: Web Agents can Self-Improve by Discovering and Honing Skills | arXiv | [paper](https://arxiv.org/abs/2504.07079) | [code](https://github.com/OSU-NLP-Group/SkillWeaver) |
  | 2025 | PyVision: Agentic Vision with Dynamic Tooling | arXiv | [paper](https://arxiv.org/abs/2507.07998) | [code](https://github.com/agents-x-project/PyVision) |
  | 2025 | From Exploration to Mastery: Enabling LLMs to Master Tools via Self-Driven Interactions | ICLR | [paper](https://arxiv.org/abs/2410.08197) | [code](https://github.com/quchangle1/DRAFT) |
  | 2025 | LLMLOOP: Improving LLM-Generated Code and Tests Through Automated Iterative Feedback Loops | ICSME | [paper](https://ieeexplore.ieee.org/document/11185878) | [code](https://github.com/ravinravi03/LLMLOOP) |
  | 2025 | Helping LLMs Improve Code Generation Using Feedback from Testing and Static Analysis | arXiv | [paper](https://arxiv.org/abs/2412.14841) | N/A |
  | 2026 | RewardHarness: Self-Evolving Agentic Post-Training | arXiv | [paper](https://arxiv.org/abs/2605.08703) | [code](https://github.com/TIGER-AI-Lab/RewardHarness) |
  | 2026 | MUSE-Autoskill: Self-Evolving Agents via Skill Creation, Memory, Management, and Evaluation | arXiv | [paper](https://arxiv.org/abs/2605.27366) | N/A |
  | 2026 | CODESKILL: Learning Self-Evolving Skills for Coding Agents | arXiv | [paper](https://arxiv.org/abs/2605.25430) | N/A |
  | 2026 | PFAgent: A Tractable and Self-Evolving Power-Flow Agent for Interactive Grid Analysis | arXiv | [paper](https://arxiv.org/abs/2604.10846) | N/A |

  </details>

- **2.3.3 Autonomous Tool Creation**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2023 | Voyager: An Open-Ended Embodied Agent with Large Language Models | arXiv | [paper](https://arxiv.org/abs/2305.16291) | [code](https://github.com/MineDojo/Voyager) |
  | 2024 | Large Language Models as Tool Makers | arXiv | [paper](https://arxiv.org/abs/2305.17126) | [code](https://github.com/ctlllll/LLM-ToolMaker) |
  | 2024 | OS-Copilot: Towards Generalist Computer Agents with Self-Improvement | ICLR | [paper](https://arxiv.org/abs/2402.07456) | [code](https://github.com/OS-Copilot/OS-Copilot) |
  | 2025 | Alita: Generalist Agent Enabling Scalable Agentic Reasoning with Minimal Predefinition and Maximal Self-Evolution | arXiv | [paper](https://arxiv.org/abs/2505.20286) | [code](https://github.com/CharlesQ9/Alita) |
  | 2025 | Alita-G: Self-Evolving Generative Agent for Agent Generation | arXiv | [paper](https://arxiv.org/abs/2510.23601) | N/A |
  | 2025 | LLM Agents Making Agent Tools | ACL | [paper](https://arxiv.org/abs/2502.11705) | [code](https://github.com/KatherLab/ToolMaker) |
  | 2025 | Advanced Tool Learning and Selection System (ATLASS): A Closed-Loop Framework Using LLM | SOSE | [paper](https://arxiv.org/abs/2503.10071) | N/A |
  | 2025 | Code2MCP: Transforming Code Repositories into MCP Services | arXiv | [paper](https://arxiv.org/abs/2509.05941) | [code](https://github.com/DEFENSE-SEU/Code2MCP) |
  | 2025 | STELLA: Self-Evolving LLM Agent for Biomedical Research | arXiv | [paper](https://arxiv.org/abs/2507.02004) | [code](https://github.com/zaixizhang/STELLA) |
  | 2025 | PyVision: Agentic Vision with Dynamic Tooling | arXiv | [paper](https://arxiv.org/abs/2507.07998) | [code](https://github.com/agents-x-project/PyVision) |
  | 2025 | AgentOrchestra: Orchestrating Multi-Agent Intelligence with the Tool-Environment-Agent(TEA) Protocol | arXiv | [paper](https://arxiv.org/abs/2506.12508) | N/A |
  | 2025 | Enhancing Open-Domain Task-Solving Capability of LLMs via Autonomous Tool Integration from GitHub | ACL | [paper](https://arxiv.org/abs/2312.17294) | [code](https://github.com/OpenBMB/OpenAct) |
  | 2026 | OpenSkill: Open-World Self-Evolution for LLM Agents | arXiv | [paper](https://arxiv.org/abs/2606.06741) | [code](https://github.com/OpenLAIR/OpenSkill) |
  | 2026 | EvoDS: Self-Evolving Autonomous Data Science Agent with Skill Learning and Context Management | arXiv | [paper](https://arxiv.org/abs/2606.03841) | [code](https://github.com/usail-hkust/EvoDS) |
  | 2026 | Autonomous Evolution of EDA Tools: Multi-Agent Self-Evolved ABC | DAC | [paper](https://arxiv.org/abs/2604.15082) | N/A |
  | 2026 | CoEvoSkills: Self-Evolving Agent Skills via Co-Evolutionary Verification | arXiv | [paper](https://arxiv.org/abs/2604.01687) | [code](https://github.com/Zhang-Henry/CoEvoSkills) |

  </details>

</details>

<details open>
<summary><b>2.4 Full Scaffolding</b></summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2024 | Language Agents as Optimizable Graphs | ICML | [paper](https://arxiv.org/abs/2402.16823) | [code](https://github.com/metauto-ai/gptswarm) |
  | 2024 | Self-Taught Optimizer (STOP): Recursively Self-Improving Code Generation | COLM | [paper](https://arxiv.org/abs/2410.04444) | [code](https://github.com/microsoft/stop) |
  | 2024 | Automated Design of Agentic Systems | NeurIPS | [paper](https://arxiv.org/abs/2408.08435) | [code](https://github.com/ShengranHu/ADAS) |
  | 2024 | Symbolic Learning Enables Self-Evolving Agents | arXiv | [paper](https://arxiv.org/abs/2406.18532) | [code](https://github.com/aiwaves-cn/agents) |
  | 2025 | Darwin Godel Machine: Open-Ended Evolution of Self-Improving Agents | arXiv | [paper](https://arxiv.org/abs/2505.22954) | [code](https://github.com/jennyzzt/dgm) |
  | 2025 | Huxley-Gödel Machine: Human-Level Coding Agent Development by an Approximation of the Optimal Self-Improving Machine | arXiv | [paper](https://arxiv.org/abs/2510.21614) | [code](https://github.com/metauto-ai/HGM) |
  | 2025 | Gödel Agent: A Self-Referential Agent Framework for Recursive Self-Improvement | ACL | [paper](https://arxiv.org/abs/2410.04444) | [code](https://github.com/Arvid-pku/Godel_Agent) |
  | 2025 | AlphaEvolve: A coding agent for scientific and algorithmic discovery | arXiv | [paper](https://arxiv.org/abs/2506.13131) | N/A |
  | 2025 | ShinkaEvolve: Towards Open-Ended And Sample-Efficient Program Evolution | arXiv | [paper](https://arxiv.org/abs/2509.19349) | [code](https://github.com/SakanaAI/ShinkaEvolve) |
  | 2025 | Live-SWE-agent: Can Software Engineering Agents Self-Evolve on the Fly? | arXiv | [paper](https://arxiv.org/abs/2511.13646) | [code](https://github.com/OpenAutoCoder/live-swe-agent) |
  | 2026 | AgentDevel: Reframing Self-Evolving LLM Agents as Release Engineering | arXiv | [paper](https://arxiv.org/abs/2601.04620) | N/A |
  | 2026 | JudgeFlow: Agentic Workflow Optimization via Block Judge | arXiv | [paper](https://arxiv.org/abs/2601.07477) | N/A |
  | 2026 | RoboPhD: Self-Improving Text-to-SQL Through Autonomous Agent Evolution | arXiv | [paper](https://arxiv.org/abs/2601.01126) | [code](https://github.com/andborth/RoboPhD) |
  | 2026 | Group-Evolving Agents: Open-Ended Self-Improvement via Experience Sharing | arXiv | [paper](https://arxiv.org/abs/2602.04837) | N/A |
  | 2026 | Hyperagents | arXiv | [paper](https://arxiv.org/abs/2603.19461) | [code](https://github.com/facebookresearch/Hyperagents) |
  | 2026 | CORAL: Towards Autonomous Multi-Agent Evolution for Open-Ended Discovery | COLM | [paper](https://arxiv.org/abs/2604.01658) | [code](https://github.com/Human-Agent-Society/CORAL) |
  | 2026 | Adaptive Auto-Harness: Sustained Self-Improvement for Agentic System Deployment on Open-Ended Task Streams | arXiv | [paper](https://arxiv.org/abs/2606.01770) | [code](https://github.com/A-EVO-Lab/AdaptiveHarness) |
  | 2026 | MOSS: Self-Evolution through Source-Level Rewriting in Autonomous Agent Systems | arXiv | [paper](https://arxiv.org/abs/2605.22794) | [code](https://github.com/dav-joy-thon/MOSS) |
  | 2026 | Recursive Self-Evolving Agents via Held-Out Selection | arXiv | [paper](https://arxiv.org/abs/2606.28374) | N/A |
  | 2026 | Continual Harness: Online Adaptation for Self-Improving Foundation Agents | arXiv | [paper](https://arxiv.org/abs/2605.09998) | [code](https://github.com/sethkarten/continual-harness) |
  | 2026 | Argus: A General-Purpose Agentic Reasoning Runtime for Long-Horizon Tasks | arXiv | [paper](https://arxiv.org/abs/2608.05144) | [code](https://github.com/lbx154/Argus) |
  | 2026 | The Red Queen Gödel Machine: Co-Evolving Agents and Their Evaluators | arXiv | [paper](https://arxiv.org/abs/2606.26294) | N/A |
  | 2026 | Harness-R1: Learning to Edit Executable Runtime Harnesses from Agent Failure Trajectories | arXiv | [paper](https://arxiv.org/abs/2608.02276) | [code](https://github.com/DeepExperience/Harness-R1) |
  | 2026 | LLM-as-Code: Agentic Programming for Agent Harness | KDD AgenticSE Workshop | [paper](https://arxiv.org/abs/2606.15874) | [code](https://github.com/Fzkuji/OpenProgram) |
  | 2026 | Ouroboros: A Self-Developing Frontier Coding Agent with Reviewed Core Evolution | arXiv | [paper](https://arxiv.org/abs/2608.08311) | [code](https://github.com/razzant/ouroboros) |
  | 2026 | Harness Handbook: Making Evolving Agent Harnesses Readable, Navigable, and Editable | arXiv | [paper](https://arxiv.org/pdf/2607.13285) | [code](https://github.com/Ruhan-Wang/Harness_Handbook) |
  
</details>

---

<a id="evaluation"></a>

## 📊 Evaluation & Benchmarking

A representative paper–benchmark matrix for self-improving agents, illustrating which benchmarks are used across different methods. See the **Evaluation** section of our survey for further details.

<p align="center">
  <a href="assets/fig-si-matrix-001.png">
    <img
      src="assets/fig-si-matrix-001.png"
      alt="Paper-benchmark incidence matrix for self-improving agents"
      width="100%"
    >
  </a>
</p>

The literature is organized along two complementary perspectives:

- **Measuring Improvement** studies how agent progress is assessed, either through explicit metrics or learned/agentic judges.
- **Benchmarking Improvement** groups benchmarks by the improvement mechanism they probe or by the application domain they cover.

> [!NOTE]
> A benchmark may appear in more than one subsection because the taxonomy is multi-perspective. For example, a benchmark can provide metric-based measurement while also targeting a specific domain or improvement mechanism.

### 📏 Measuring Improvement

<details open>
<summary><b>Metric-Based Measurement</b></summary>

| 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
|------:|--------|--------|--------|--------|
| 2023 | Mind2Web: Towards a Generalist Agent for the Web | NeurIPS | [paper](https://arxiv.org/abs/2306.06070) | [code](https://github.com/OSU-NLP-Group/Mind2Web) |
| 2023 | ManiSkill2: A Unified Benchmark for Generalizable Manipulation Skills | ICLR | [paper](https://openreview.net/forum?id=b_CQDy9vrD1) | [code](https://github.com/mani-skill/ManiSkill) |
| 2024 | CORE-Bench: Fostering the Credibility of Published Research Through a Computational Reproducibility Agent Benchmark | TMLR | [paper](https://openreview.net/forum?id=BsMMc4MEGS) | [code](https://github.com/siegelz/core-bench) |
| 2024 | SWE-Bench+: Enhanced Coding Benchmark for LLMs | arXiv | [paper](https://arxiv.org/abs/2410.06992) | N/A |
| 2024 | WebLINX: Real-World Website Navigation with Multi-Turn Dialogue | ICML | [paper](https://openreview.net/forum?id=mUSPhG4uDW) | [code](https://github.com/McGill-NLP/weblinx) |
| 2024 | GAIA: A Benchmark for General AI Assistants | ICLR | [paper](https://openreview.net/forum?id=fibxvahvs3) | N/A |
| 2024 | MINT: Evaluating LLMs in Multi-Turn Interaction with Tools and Language Feedback | ICLR | [paper](https://openreview.net/forum?id=jp3gWrMuIZ) | [code](https://github.com/xingyaoww/mint-bench) |
| 2024 | WorkArena: How Capable Are Web Agents at Solving Common Knowledge Work Tasks? | ICML | [paper](https://openreview.net/forum?id=BRfqYrikdo) | [code](https://github.com/ServiceNow/WorkArena) |
| 2025 | AgentGym: Evolving Large Language Model-Based Agents across Diverse Environments | ACL | [paper](https://arxiv.org/abs/2406.04151) | [code](https://github.com/WooooDyy/AgentGym) |
| 2025 | GitTaskBench: A Benchmark for Code Agents Solving Real-World Tasks Through Code Repository Leveraging | arXiv | [paper](https://arxiv.org/abs/2508.18993) | [code](https://github.com/QuantaAlpha/GitTaskBench) |
| 2025 | SafeAgentBench: A Benchmark for Safe Task Planning of Embodied LLM Agents | arXiv | [paper](https://arxiv.org/abs/2412.13178) | [code](https://github.com/shengyin1224/SafeAgentBench) |
| 2026 | DrunkAgent: Stealthy Memory Corruption in LLM-Powered Recommender Agents | WWW | [paper](https://arxiv.org/abs/2503.23804) | N/A |
| 2026 | ST-WebAgentBench: A Benchmark for Evaluating Safety and Trustworthiness in Web Agents | ICLR | [paper](https://openreview.net/forum?id=MuCDzH0ctf) | [code](https://github.com/segev-shlomov/ST-WebAgentBench) |
| 2026 | ClawBench: A Benchmark for Evaluating AI Agents on Real-World Online Tasks | arXiv | [paper](https://arxiv.org/abs/2601.08613) | [code](https://github.com/TIGER-AI-Lab/ClawBench) |

</details>

<details open>
<summary><b>Judge-Based Measurement</b></summary>

| 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
|------:|--------|--------|--------|--------|
| 2025 | Agent-as-a-Judge: Evaluate Agents with Agents | ICML | [paper](https://arxiv.org/abs/2410.10934) | [code](https://github.com/metauto-ai/agent-as-a-judge) |
| 2025 | Evaluation Agent: Efficient and Promptable Evaluation Framework for Visual Generative Models | ACL | [paper](https://aclanthology.org/2025.acl-long.374/) | [code](https://github.com/Vchitect/Evaluation-Agent) |
| 2025 | EvalAgent: Discovering Implicit Evaluation Criteria from the Web | COLM | [paper](https://openreview.net/forum?id=erGpkHCybv) | [code](https://github.com/ManyaWadhwa/EvalAgent) |
| 2025 | Learning to Align Multi-Faceted Evaluation: A Unified and Robust Framework (ARJudge) | ACL Findings | [paper](https://aclanthology.org/2025.findings-acl.494/) | N/A |
| 2025 | VerifiAgent: A Unified Verification Agent in Language Model Reasoning | EMNLP Findings | [paper](https://aclanthology.org/2025.findings-emnlp.891/) | [code](https://github.com/Jiuzhouh/VerifiAgent) |

</details>

### 🧪 Benchmarking Improvement

<details open>
<summary><b>Mechanism Benchmarks</b></summary>

#### Foundation-Model-Level

| 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
|------:|--------|--------|--------|--------|
| 2024 | SWE-Bench+: Enhanced Coding Benchmark for LLMs | arXiv | [paper](https://arxiv.org/abs/2410.06992) | N/A |
| 2024 | Identifying the Risks of LM Agents with an LM-Emulated Sandbox | ICLR | [paper](https://openreview.net/forum?id=GEcwtMk1uA) | [code](https://github.com/ryoungj/ToolEmu) |
| 2025 | GitTaskBench: A Benchmark for Code Agents Solving Real-World Tasks Through Code Repository Leveraging | arXiv | [paper](https://arxiv.org/abs/2508.18993) | [code](https://github.com/QuantaAlpha/GitTaskBench) |

#### Scaffold-Level

| 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
|------:|--------|--------|--------|--------|
| 2024 | MINT: Evaluating LLMs in Multi-Turn Interaction with Tools and Language Feedback | ICLR | [paper](https://openreview.net/forum?id=jp3gWrMuIZ) | [code](https://github.com/xingyaoww/mint-bench) |
| 2024 | TaskBench: Benchmarking Large Language Models for Task Automation | NeurIPS | [paper](https://arxiv.org/abs/2311.18760) | [code](https://github.com/microsoft/JARVIS/tree/main/taskbench) |
| 2024 | MetaTool Benchmark for Large Language Models: Deciding Whether to Use Tools and Which to Use | ICLR | [paper](https://arxiv.org/abs/2310.03128) | [code](https://github.com/HowieHwong/MetaTool) |
| 2025 | The Berkeley Function Calling Leaderboard (BFCL): From Tool Use to Agentic Evaluation of Large Language Models | ICML | [paper](https://openreview.net/forum?id=2GmDdhBdDk) | [code](https://github.com/ShishirPatil/gorilla/tree/main/berkeley-function-call-leaderboard) |
| 2026 | DrunkAgent: Stealthy Memory Corruption in LLM-Powered Recommender Agents | WWW | [paper](https://arxiv.org/abs/2503.23804) | N/A |
| 2026 | RSI-Bench: Multi-Axis Benchmark for Recursive Self-Improvement | GitHub | N/A | [code](https://github.com/sunghunkwag/rsi-bench) |

</details>

<details open>
<summary><b>Domain Benchmarks</b></summary>

#### Software Engineering

| 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
|------:|--------|--------|--------|--------|
| 2024 | SWE-bench: Can Language Models Resolve Real-World GitHub Issues? | ICLR | [paper](https://openreview.net/forum?id=VTF8yNQM66) | [code](https://github.com/SWE-bench/SWE-bench) |
| 2024 | SWE-Bench+: Enhanced Coding Benchmark for LLMs | arXiv | [paper](https://arxiv.org/abs/2410.06992) | N/A |
| 2024 | SWT-Bench: Testing and Validating Real-World Bug-Fixes with Code Agents | NeurIPS | [paper](https://openreview.net/forum?id=9Y8zUO11EQ) | [code](https://github.com/logic-star-ai/swt-bench) |
| 2024 | TDD-Bench Verified: Can LLMs Generate Tests for Issues Before They Get Resolved? | arXiv | [paper](https://arxiv.org/abs/2412.02883) | [code](https://github.com/IBM/TDD-Bench-Verified) |
| 2025 | LoCoBench-Agent: An Interactive Benchmark for LLM Agents in Long-Context Software Engineering | arXiv | [paper](https://arxiv.org/abs/2511.13998) | [code](https://github.com/SalesforceAIResearch/LoCoBench-Agent) |
| 2025 | DevAI: Automated AI Development Benchmark | ICML | [paper](https://arxiv.org/abs/2410.10934) | [code](https://github.com/metauto-ai/agent-as-a-judge) |

#### Web Navigation

| 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
|------:|--------|--------|--------|--------|
| 2023 | Mind2Web: Towards a Generalist Agent for the Web | NeurIPS | [paper](https://arxiv.org/abs/2306.06070) | [code](https://github.com/OSU-NLP-Group/Mind2Web) |
| 2024 | WebArena: A Realistic Web Environment for Building Autonomous Agents | ICLR | [paper](https://openreview.net/forum?id=oKn9c6ytLx) | [code](https://github.com/web-arena-x/webarena) |
| 2024 | VisualWebArena: Evaluating Multimodal Agents on Realistic Visual Web Tasks | ICLR Workshop | [paper](https://openreview.net/forum?id=RPKxrKTJbj) | [code](https://github.com/web-arena-x/visualwebarena) |
| 2024 | WebCanvas: Benchmarking Web Agents in Online Environments | ICML Workshop | [paper](https://arxiv.org/abs/2406.12373) | [code](https://github.com/iMeanAI/WebCanvas) |
| 2026 | ST-WebAgentBench: A Benchmark for Evaluating Safety and Trustworthiness in Web Agents | ICLR | [paper](https://openreview.net/forum?id=MuCDzH0ctf) | [code](https://github.com/segev-shlomov/ST-WebAgentBench) |

#### Gaming & Strategy

| 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
|------:|--------|--------|--------|--------|
| 2023 | clembench: Using Game Play to Evaluate Chat-Optimized Language Models as Conversational Agents | EMNLP | [paper](https://aclanthology.org/2023.emnlp-main.689/) | [code](https://github.com/clp-research/clembench) |
| 2024 | clembench-2024: A Challenging, Dynamic, Complementary, Multilingual Benchmark and Underlying Flexible Framework for LLMs as Multi-Action Agents | arXiv | [paper](https://arxiv.org/abs/2405.20859) | [code](https://github.com/clp-research/clembench) |
| 2024 | GameBench: Evaluating Strategic Reasoning Abilities of LLM Agents | NeurIPS Workshop | [paper](https://arxiv.org/abs/2406.06613) | [code](https://github.com/Joshuaclymer/GameBench) |
| 2024 | LLM-Deliberation: Evaluating LLMs with Interactive Multi-Agent Negotiation Game | ICLR Workshop | [paper](https://openreview.net/forum?id=eE1WHn6qlk) | N/A |
| 2024 | GTBench: Uncovering the Strategic Reasoning Capabilities of LLMs via Game-Theoretic Evaluations | NeurIPS | [paper](https://arxiv.org/abs/2402.12348) | [code](https://github.com/jinhaoduan/GTBench) |

#### Scientific Discovery

| 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
|------:|--------|--------|--------|--------|
| 2024 | CORE-Bench: Fostering the Credibility of Published Research Through a Computational Reproducibility Agent Benchmark | TMLR | [paper](https://openreview.net/forum?id=BsMMc4MEGS) | [code](https://github.com/siegelz/core-bench) |
| 2024 | DiscoveryWorld: A Virtual Environment for Developing and Evaluating Automated Scientific Discovery Agents | NeurIPS Datasets & Benchmarks | [paper](https://openreview.net/forum?id=cDYqckEt6d) | [code](https://github.com/allenai/discoveryworld) |
| 2025 | PaperBench: Evaluating AI's Ability to Replicate AI Research | arXiv | [paper](https://arxiv.org/abs/2504.01848) | [code](https://github.com/openai/frontier-evals/tree/main/project/paperbench) |
| 2025 | PhysGym: Benchmarking LLMs in Interactive Physics Discovery with Controlled Priors | NeurIPS Datasets & Benchmarks | [paper](https://openreview.net/forum?id=w8uII2qAmd) | [code](https://github.com/principia-ai/PhysGym) |
| 2026 | AstaBench: Rigorous Benchmarking of AI Agents with a Scientific Research Suite | ICLR | [paper](https://openreview.net/forum?id=M7TNf5J26u) | [code](https://github.com/allenai/asta-bench) |
| 2026 | MLS-Bench: A Holistic and Rigorous Assessment of AI Systems on Building Better AI | arXiv | [paper](https://arxiv.org/abs/2605.08678) | [code](https://github.com/Imbernoulli/MLS-Bench) |

#### Embodied AI

| 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
|------:|--------|--------|--------|--------|
| 2023 | ManiSkill2: A Unified Benchmark for Generalizable Manipulation Skills | ICLR | [paper](https://openreview.net/forum?id=b_CQDy9vrD1) | [code](https://github.com/mani-skill/ManiSkill) |
| 2025 | SafeAgentBench: A Benchmark for Safe Task Planning of Embodied LLM Agents | arXiv | [paper](https://arxiv.org/abs/2412.13178) | [code](https://github.com/shengyin1224/SafeAgentBench) |
| 2025 | EmbodiedBench: Comprehensive Benchmarking Multi-Modal Large Language Models for Vision-Driven Embodied Agents | ICML | [paper](https://openreview.net/forum?id=DgGF2LEBPS) | [code](https://github.com/EmbodiedBench/EmbodiedBench) |

#### General Computer Control

| 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
|------:|--------|--------|--------|--------|
| 2024 | OSWorld: Benchmarking Multimodal Agents for Open-Ended Tasks in Real Computer Environments | NeurIPS | [paper](https://arxiv.org/abs/2404.07972) | [code](https://github.com/xlang-ai/OSWorld) |
| 2024 | AppWorld: A Controllable World of Apps and People for Benchmarking Interactive Coding Agents | ACL | [paper](https://aclanthology.org/2024.acl-long.850/) | [code](https://github.com/StonyBrookNLP/appworld) |
| 2024 | Identifying the Risks of LM Agents with an LM-Emulated Sandbox | ICLR | [paper](https://openreview.net/forum?id=GEcwtMk1uA) | [code](https://github.com/ryoungj/ToolEmu) |
| 2024 | MetaTool Benchmark for Large Language Models: Deciding Whether to Use Tools and Which to Use | ICLR | [paper](https://arxiv.org/abs/2310.03128) | [code](https://github.com/HowieHwong/MetaTool) |
| 2025 | Windows Agent Arena: Evaluating Multi-Modal OS Agents at Scale | ICML | [paper](https://openreview.net/forum?id=W9s817KqYf) | [code](https://github.com/microsoft/WindowsAgentArena) |
| 2025 | The Berkeley Function Calling Leaderboard (BFCL): From Tool Use to Agentic Evaluation of Large Language Models | ICML | [paper](https://openreview.net/forum?id=2GmDdhBdDk) | [code](https://github.com/ShishirPatil/gorilla/tree/main/berkeley-function-call-leaderboard) |

</details>

---

## 🔗 Related Resources

### ✍️ Blogs

* **Metalearning Machines Learn to Learn (1987–)** — Jürgen Schmidhuber, 2025
  | [Blog](https://people.idsia.ch/~juergen/metalearning.html) |

* **When AI Builds Itself** — Anthropic, 2026
  | [Blog](https://www.anthropic.com/institute/recursive-self-improvement) |

* **AIDE²: The First Evidence of Recursive Self-Improvement** — WeCo, 2026
  | [Blog](https://www.weco.ai/blog/first-evidence-of-recursive-self-improvement) |

* **The What & When of Self-Evolving Agents** — 2026
  | [Blog](https://xinmingtu.cn/blog/2026/self-evolving-agents/) |

* **Automated Weak-to-Strong Researcher** — Anthropic, 2026
  | [Blog](https://alignment.anthropic.com/2026/automated-w2s-researcher/) |

* **The Darwin Gödel Machine: AI That Improves Itself by Rewriting Its Own Code** — Sakana AI, 2025
  | [Blog](https://sakana.ai/dgm/) |

* **AlphaEvolve: A Gemini-Powered Coding Agent for Designing Advanced Algorithms** — Google DeepMind, 2025
  | [Blog](https://deepmind.google/blog/alphaevolve-a-gemini-powered-coding-agent-for-designing-advanced-algorithms/) |

* **FunSearch: Making New Discoveries in Mathematical Sciences Using Large Language Models** — Google DeepMind, 2023
  | [Blog](https://deepmind.google/blog/funsearch-making-new-discoveries-in-mathematical-sciences-using-large-language-models/) |

### 🎙️ Podcasts & Interviews

* **Jürgen Schmidhuber: Gödel Machines, Meta-Learning, and LSTMs | Lex Fridman Podcast #11** — Lex Fridman Podcast, 2018
  | [YouTube Video](https://www.youtube.com/watch?v=3FIo6evmweo) |

* **再访田渊栋：46.5 亿美金估值的 RSI，与 AI 自进化｜Neolabs 特辑【101 视频播客】** — 2026
  | [Bilibili Video](https://www.bilibili.com/video/BV1DY7C6nEWM/) |

* **Agent AI Needs Darwin** — Machine Learning Street Talk, 2025
  | [Podcast](https://dexa.ai/machinelearningstreettalk/d/b6fadb24-ca4c-11ef-b367-275d623b7386) |

* **#75 – Marcus Hutter: Universal Artificial Intelligence, AIXI, and AGI** — Lex Fridman Podcast, 2020
  | [Podcast](https://lexfridman.com/marcus-hutter/) |

### 🎥 Talks & Courses

* **Recursive self-improvement (RSI) and meta learning** — Jürgen Schmidhuber, 2020
  | [Video](https://x.com/SchmidhuberAI/status/2031397968511717584) |

* **2026 北京智源大会｜AI 自进化** — Beijing Academy of Artificial Intelligence, 2026
  | [Bilibili Video](https://www.bilibili.com/video/BV1Bijw65Ec9/) |

* **Recursive Self-Improvement：当 AI 开始进化 AI** — 2026
  | [Bilibili Video](https://www.bilibili.com/video/BV17Z7a6vEVH/) |

* **全球嘉宾共话 Self-Evolving Agents：从学术前沿到产业落地** — 2026
  | [Bilibili Video](https://www.bilibili.com/video/BV1P4LX68EcS/) |

* **【肖仰华 复旦教授】大模型驱动的自进化智能体：研究与实践（Agentic AI Summit·2026·深圳站）** — 2026
  | [Bilibili Video](https://www.bilibili.com/video/BV1tHgY6YEuJ/) |

* **Jeff Clune | Open-Ended and AI-Generating Algorithms in the Era of Foundation Models** — 2025
  | [YouTube Video](https://www.youtube.com/watch?v=gIHAVTj9fjo&t=3037s) |

* **Stanford CS329A: Self-Improving AI Agents** — Stanford University, 2025
  | [Course](https://cs329a.stanford.edu/) | [YouTube Playlist](https://www.youtube.com/playlist?list=PL3058ht9NqT1NG6Y663elpHSDh-AW1TIr) |

* **Open-Ended Agent Learning in the Era of Foundation Models** — Jeff Clune
  | [YouTube Video](https://www.youtube.com/watch?v=EZBuPfu85b8) |

### 🎓 Thesis

- **[Multimodal Agents: From Automation toward Open-Ended Self-Improvement](https://repository.kaust.edu.sa/items/0bff44ae-653f-4381-a25a-78b990c3ab5c)**  
  Mingchen Zhuge, Ph.D. Dissertation, King Abdullah University of Science and Technology (KAUST), 2026.  
  [[Defense page](https://cemse.kaust.edu.sa/events/by-type/phd-dissertation-defense/2026/05/09/multimodal-agents-automation-toward-open-ended)]

### 🧑‍🏫 Workshop

- **[ICLR 2026 Workshop on AI with Recursive Self-Improvement (RSI 2026)](https://recursive-workshop.github.io/)**  
  A workshop dedicated to recursive self-improving AI, held on April 26, 2026, in Rio de Janeiro, Brazil.  
  Lead organizer: Mingchen Zhuge.

---

## 📬 Contact & Community

- [![Discord](https://img.shields.io/badge/Discord-Join-5865F2?logo=discord&logoColor=white)](https://discord.gg/fn5rYJhgaz) **Discord**: Join our server 👉 https://discord.gg/fn5rYJhgaz
- ![WeChat](https://img.shields.io/badge/WeChat-Group-07C160?logo=wechat&logoColor=white) **WeChat Group**: Scan the QR code below to join. If the QR code expires, please add the WeChat admin (**13488260597**), and we will invite you to the group.
  <details>
    <summary>📱 Show WeChat Group QR Code</summary>
  
    <p align="center">
      <img src="assets/20260720.jpg" alt="WeChat group QR" width="160">
    </p>
  </details>

---

## 🤝 Contribute
PRs are welcome!  

---

## 📌 Citation
```bibtex
@misc{ren2026selfimprovementsmodernagenticsystems,
      title={Self-Improvements in Modern Agentic Systems: A Survey}, 
      author={Zhe Ren and Yimeng Chen and Dandan Guo and Guowei Rong and Tonghui Li and R. B. Xiong and Qingfeng Lan and Wenyi Wang and Li Nanbo and Yibo Yang and Mingchen Zhuge and Jürgen Schmidhuber},
      year={2026},
      eprint={2607.13104},
      archivePrefix={arXiv},
      primaryClass={cs.AI},
      url={https://arxiv.org/abs/2607.13104}, 
}
```
