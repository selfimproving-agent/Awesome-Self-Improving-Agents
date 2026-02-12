
# Awesome Self-Improving FM-Based Agents 
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![Discord](https://img.shields.io/badge/Discord-Join-blue?logo=discord&logoColor=white)](https://discord.gg/fn5rYJhgaz)


> A curated, continuously updated resource list for **Self-Improvement in Foundation Model Based Agentic Systems**.  
> This repo accompanies the survey paper: _"Self-Improvement in Foundation Model Based Agentic Systems: A Survey"_ (2026).

---

## 🌐 Contents
- [Definition & Scope](#-definition--scope)
- [Survey Paper](#-survey-paper)
- [Taxonomy](#-taxonomy)
- [Key Literature](#-key-literature)
  - [🟦 Foundation Model Improvement](#-foundation-model-improvement)
  - [🟩 Scaffolding Improvement](#-scaffolding-improvement)
- [Contact & Community](#-contact--community)
- [Contribute](#-contribute)
- [Citation](#-citation)

---

## 🧩 Definition & Scope
This repository focuses on:
- **Foundation-Model-Based Agents**: Autonomous entities leveraging LLMs/VLM as core controllers.
- **Autonomous Self-Improvement**: Systems that enhance their own performance through internal mechanisms.
- **Agentic RL & Policy Optimization**: Self-evolving strategies and decision-making.
- **Scaffolding Evolution**: Growth in memory structures, tool-use capability, and prompt refinement.

---

## 📄 Survey Paper
🔗 **Coming soon** — Preprint in preparation.   
*(Add arXiv link here once uploaded.)*

<p align="center">
  <img src="assets/fig.png" alt="Main figure of the survey" width="95%">
  <br>
  <em>Overview of self-improvement mechanisms in foundation model–based agentic systems.</em>
</p>

---

## 🧭 Taxonomy

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
        * 📄 `1.1` Self-Generated Data
        * ⚖️ `1.2` Self-Generated Supervision
        * 🌍 `1.3` Self-Generated Experience
            * 🤖 `1.3.1` Environment-Interactive
            * 🔮 `1.3.2` World Models
    * **🏗️ Scaffolding Improvement**
        * ✍️ `2.1` Prompt Optimization
        * 💾 `2.2` Memory
        * 🛠️ `2.3` Tool
        * ♾️ `2.4` Full Scaffolding

---

## 📚 Key Literature
### Core Papers

#### 🟦 Foundation Model Improvement

<details open>
<summary><b>1.1 Self-Generated Data</b></summary>

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

</details>

<details open>
<summary><b>1.2 Self-Generated Supervision</b></summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2025 | STRIVE: Structured Reasoning for Self-Improvement in Claim Verification | MIR | [paper](https://arxiv.org/abs/2502.11959) | N/A |
  | 2025 | Beyond Accuracy: The Role of Calibration in Self-Improving Large Language Models | arXiv | [paper](https://arxiv.org/abs/2504.02902) | N/A |
  | 2022 | Constitutional AI: Harmlessness from AI Feedback | arXiv | [paper](https://arxiv.org/abs/2212.08073) | [code](https://github.com/anthropics/ConstitutionalHarmlessnessPaper?tab=readme-ov-file) |
  | 2023 | ReST meets ReAct: Self-Improvement for Multi-Step Reasoning LLM Agent | arXiv | [paper](https://arxiv.org/abs/2312.10003) | N/A |
  | 2025 | Self-Evolved Reward Learning for LLMs | ICLR | [paper](https://arxiv.org/abs/2411.00418) | [code](https://github.com/microsoft/DKI_LLM/tree/main/SER) |
  | 2025 | Sample, Predict, then Proceed: Self-Verification Sampling for Tool Use of LLMs | arXiv | [paper](https://arxiv.org/abs/2506.02918v1) | N/A |
  | 2025 | RLSR: Reinforcement Learning from Self Reward | arXiv | [paper](https://arxiv.org/abs/2505.08827) | N/A |

</details>

<details open>
<summary><b>1.3 Self-Generated Experience</b></summary>

- **1.3.1 Environment -Interactive**
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

  </details>

- **1.3.2 World Models**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2025 | Understanding World or Predicting Future? A Comprehensive Survey of World Models | ACM CSUR | [paper](https://arxiv.org/abs/2411.14499) | [code](https://github.com/tsinghua-fib-lab/World-Model) |
  | 2025 | General agents contain world models | ICML | [paper](https://arxiv.org/abs/2506.01622) | N/A |
  | 2025 | WebEvolver: Enhancing Web Agent Self-Improvement with Coevolving World Model | EMNLP | [paper](https://arxiv.org/abs/2504.21024) | [code](https://github.com/Tencent/SelfEvolvingAgent) |
  | 2025 | WebSynthesis: World-Model-Guided MCTS for Efficient WebUI-Trajectory Synthesis | arXiv | [paper](https://arxiv.org/abs/2507.04370) | [code](https://github.com/LucusFigoGao/WebSynthesis) |
  | 2025 | GAWM: Global-Aware World Model for Multi-Agent Reinforcement Learning | arXiv | [paper](https://arxiv.org/abs/2501.10116) | N/A |
  | 2023 | Language Models Meet World Models: Embodied Experiences Enhance Language Models | NeurIPS | [paper](https://arxiv.org/abs/2305.10626) | [code](https://github.com/szxiangjn/world-model-for-language-model) |
  | 2025 | Web Agents with World Models: Learning and Leveraging Environment Dynamics in Web Navigation | ICLR | [paper](https://arxiv.org/abs/2410.13232) | [code](https://github.com/kyle8581/WMA-Agents) |
  | 2024 | Agent Planning with World Knowledge Model | NeurIPS | [paper](https://arxiv.org/abs/2405.14205) | [code](https://github.com/zjunlp/WKM) |

  </details>
  
</details>


#### 🟩 Scaffolding Improvement

<details open>
<summary><b>2.1 Prompt Optimization</b></summary>

- **2.1.1 Black-Box Optimization**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2022 | Large Language Models Are Human-Level Prompt Engineers | arXiv | [paper](https://arxiv.org/abs/2211.01910) | [code](https://github.com/keirp/automatic_prompt_engineer) |
  | 2024 | Large Language Models as Optimizers | ICLR | [paper](https://arxiv.org/abs/2309.03409) | [code](https://github.com/google-deepmind/opro) |

  </details>

- **2.1.2 Iterative Refinement**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2023 | Self-Refine: Iterative Refinement with Self-Feedback | arXiv | [paper](https://arxiv.org/abs/2303.17651) | [code](https://github.com/madaan/self-refine) |
  | 2023 | Chain of Hindsight Aligns Language Models with Feedback | arXiv | [paper](https://arxiv.org/abs/2302.02676) | [code](https://github.com/haoliuhl/chain-of-hindsight) |
  | 2023 | Reflexion: Language Agents with Verbal Reinforcement Learning | NeurIPS  | [paper](https://arxiv.org/abs/2303.11366) | [code](https://github.com/noahshinn/reflexion) |
  | 2024 | Self-Improving Customer Review Response Generation Based on LLMs | COLING  | [paper](https://arxiv.org/abs/2405.03845) | N/A |

  </details>

- **2.1.3 Evolutionary Algorithms**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2024 | EvoPrompt: Connecting LLMs with Evolutionary Algorithms Yields Powerful Prompt Optimizers | ICLR | [paper](https://arxiv.org/abs/2309.08532) | [code](https://github.com/beeevita/EvoPrompt) |
  | 2024 | WizardLM: Empowering large pre-trained language models to follow complex instructions | ICLR | [paper](https://arxiv.org/abs/2304.12244) | [code](https://github.com/nlpxucan/WizardLM) |
  | 2025 | Tournament of Prompts: Evolving LLM Instructions Through Structured Debates and Elo Ratings | KDD | [paper](https://arxiv.org/abs/2506.00178v2) | N/A |
  | 2023 | Promptbreeder: Self-Referential Self-Improvement Via Prompt Evolution | arXiv | [paper](https://arxiv.org/abs/2309.16797) | N/A |

  </details>

- **2.1.4 Textual Gradient**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2025 | TextGrad: Automatic "Differentiation" via Text | Nature | [paper](https://arxiv.org/abs/2406.07496) | [code](https://github.com/zou-group/textgrad) |
  | 2025 | metaTextGrad: Automatically optimizing language model optimizers | NeurIPS | [paper](https://arxiv.org/abs/2505.18524) | [code](https://github.com/zou-group/metatextgrad) |
  | 2023 | Automatic Prompt Optimization with "Gradient Descent" and Beam Search | EMNLP  | [paper](https://arxiv.org/abs/2305.03495) | [code](https://github.com/microsoft/LMOps/tree/main/prompt_optimization) |
  | 2024 | How to Correctly do Semantic Backpropagation on Language-based Agentic Systems | arXiv  | [paper](https://arxiv.org/abs/2412.03624) | [code](https://github.com/HishamAlyahya/semantic_backprop) |

  </details>
  
</details>

<details open>
<summary><b>2.2 Memory</b></summary>

- **2.2.1 Memory Object**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2024 | Agent Workflow Memory | arXiv | [paper](https://arxiv.org/abs/2409.07429) | [code](https://github.com/zorazrw/agent-workflow-memory) |
  | 2025 | ReasoningBank: Scaling Agent Self-Evolving with Reasoning Memory | arXiv | [paper](https://arxiv.org/abs/2509.25140) | N/A |
  | 2024 | ExpeL: LLM Agents Are Experiential Learners | AAAI  | [paper](https://arxiv.org/abs/2308.10144) | [code](https://github.com/LeapLabTHU/ExpeL) |
  | 2024 | A Human-Inspired Reading Agent with Gist Memory of Very Long Contexts | ICML  | [paper](https://arxiv.org/abs/2402.09727) | N/A |
  | 2025 | Seeing, Listening, Remembering, and Reasoning: A Multimodal Agent with Long-Term Memory | arXiv  | [paper](https://arxiv.org/abs/2508.09736) | [code](https://github.com/bytedance-seed/m3-agent) |
  | 2023 | Learning to Reason and Memorize with Self-Notes | NeurIPS  | [paper](https://arxiv.org/abs/2305.00833) | N/A |
  | 2025 | Dynamic Cheatsheet: Test-Time Learning with Adaptive Memory | arXiv  | [paper](https://arxiv.org/abs/2305.00833) | [code](https://github.com/suzgunmirac/dynamic-cheatsheet) |

  </details>

- **2.2.2 Memory Structure**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2025 | SCM: Enhancing Large Language Model with Self-Controlled Memory Framework | DASFAA | [paper](https://arxiv.org/abs/2304.13343) | [code](https://github.com/wbbeyourself/SCM4LLMs) |
  | 2024 | Explore, Select, Derive, and Recall: Augmenting LLM with Human-like Memory for Mobile Task Automation | ACM MobiCom | [paper](https://arxiv.org/abs/2312.03003) | [code](https://github.com/mobilegptsys/MobileGPT) |
  | 2025 | Hierarchical Memory for High-Efficiency Long-Term Reasoning in LLM Agents | arXiv | [paper](https://arxiv.org/abs/2507.22925) | N/A |
  | 2025 | SALM: A Multi-Agent Framework for Language Model-Driven Social Network Simulation | arXiv | [paper](https://arxiv.org/abs/2505.09081) | N/A |
  | 2022 | XMem: Long-Term Video Object Segmentation with an Atkinson-Shiffrin Memory Model | ECCV  | [paper](https://arxiv.org/abs/2207.07115) | [code](https://github.com/hkchengrex/XMem) |
  | 2024 | MovieChat: From Dense Token to Sparse Memory for Long Video Understanding | CVPR | [paper](https://arxiv.org/abs/2307.16449) | [code](https://github.com/rese1f/MovieChat) |
  | 2025 | Mem0: Building Production-Ready AI Agents with Scalable Long-Term Memory | arXiv | [paper](https://arxiv.org/abs/2504.19413) | [code](https://mem0.ai/research) |

  </details>

- **2.2.3 Memory Processing**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2025 | SEDM: Scalable Self-Evolving Distributed Memory for Agents | ICLR | [paper](https://arxiv.org/abs/2309.08532) | [code](https://github.com/beeevita/EvoPrompt) |
  | 2024 | WizardLM: Empowering large pre-trained language models to follow complex instructions | ICLR | [paper](https://arxiv.org/abs/2509.09498) | N/A |
  | 2025 | MemInsight: Autonomous Memory Augmentation for LLM Agents | arXiv | [paper](https://arxiv.org/abs/2503.21760) | N/A |
  | 2025 | MemGen: Weaving Generative Latent Memory for Self-Evolving Agents | arXiv | [paper](https://arxiv.org/abs/2509.24704) | [code](https://github.com/KANABOON1/MemGen) |
  | 2025 | A-MEM: Agentic Memory for LLM Agents | NeurIPS | [paper](https://arxiv.org/abs/2502.12110) | [code](https://github.com/WujiangXu/A-mem-sys) |
  | 2023 | Generative Agents: Interactive Simulacra of Human Behavior | UIST | [paper](https://arxiv.org/abs/2304.03442) | [code](https://github.com/joonspk-research/generative_agents) |
  | 2025 | G-Memory: Tracing Hierarchical Memory for Multi-Agent Systems | arXiv | [paper](https://arxiv.org/abs/2506.07398) | [code](https://github.com/bingreeky/GMemory) |

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
  | 2025 | AgentOrchestra: Orchestrating Hierarchical Multi-Agent Intelligence with the Tool-Environment-Agent(TEA) Protocol | arXiv | [paper](https://arxiv.org/abs/2506.12508) | N/A |
  | 2025 | MetaAgent: Toward Self-Evolving Agent via Tool Meta-Learning | arXiv | [paper](https://arxiv.org/abs/2508.00271) | [code](https://github.com/qhjqhj00/MetaAgent) |
  | 2025 | OrchDAG: Complex Tool Orchestration in Multi-Turn Interactions with Plan DAGs | NeurIPS Workshop | [paper](https://arxiv.org/abs/2510.24663) | N/A |
  | 2025 | AutoTIR: Autonomous Tools Integrated Reasoning via Reinforcement Learning | arXiv | [paper](https://arxiv.org/abs/2507.21836) | [code](https://github.com/weiyifan1023/AutoTIR) |
  | 2025 | MCP-Flow: Facilitating LLM Agents to Master Real-World, Diverse and Scaling MCP Tools | arXiv | [paper](https://arxiv.org/abs/2510.24284) | [code](https://github.com/wwh0411/MCP-Flow) |
  | 2025 | In-the-Flow Agentic System Optimization for Effective Planning and Tool Use | NeurIPS | [paper](https://arxiv.org/abs/2510.05592) | [code](https://github.com/lupantech/AgentFlow) |
  | 2025 | MassTool: A Multi-Task Search-Based Tool Retrieval Framework for Large Language Models | arXiv | [paper](https://arxiv.org/abs/2507.00487) | [code](https://github.com/wxydada/MassTool) |


  </details>

- **2.3.2 Iterative Tool Refinement**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2025 | STELLA: Self-Evolving LLM Agent for Biomedical Research | arXiv | [paper](https://arxiv.org/abs/2507.02004) | [code](https://github.com/zaixizhang/STELLA) |
  | 2025 | SkillWeaver: Web Agents can Self-Improve by Discovering and Honing Skills | arXiv | [paper](https://arxiv.org/abs/2504.07079) | [code](https://github.com/OSU-NLP-Group/SkillWeaver) |
  | 2025 | PyVision: Agentic Vision with Dynamic Tooling | arXiv | [paper](https://arxiv.org/abs/2507.07998) | [code](https://github.com/agents-x-project/PyVision) |
  | 2025 | From Exploration to Mastery: Enabling LLMs to Master Tools via Self-Driven Interactions | ICLR | [paper](https://arxiv.org/abs/2410.08197) | [code](https://github.com/quchangle1/DRAFT) |

  </details>

- **2.3.3 Autonomous Tool Creation**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2025 | Alita: Generalist Agent Enabling Scalable Agentic Reasoning with Minimal Predefinition and Maximal Self-Evolution | arXiv | [paper](https://arxiv.org/abs/2505.20286) | [code](https://github.com/CharlesQ9/Alita) |
  | 2024 | Large Language Models as Tool Makers | arXiv | [paper](https://arxiv.org/abs/2305.17126) | [code](https://github.com/ctlllll/LLM-ToolMaker) |
  | 2025 | Alita-G: Self-Evolving Generative Agent for Agent Generation | arXiv | [paper](https://arxiv.org/abs/2510.23601) | N/A |
  | 2025 | LLM Agents Making Agent Tools | ACL | [paper](https://arxiv.org/abs/2502.11705) | [code](https://github.com/KatherLab/ToolMaker) |
  | 2024 | OS-Copilot: Towards Generalist Computer Agents with Self-Improvement | ICLR | [paper](https://arxiv.org/abs/2402.07456) | [code](https://github.com/OS-Copilot/OS-Copilot) |
  | 2025 | Advanced Tool Learning and Selection System (ATLASS): A Closed-Loop Framework Using LLM | SOSE | [paper](https://arxiv.org/abs/2503.10071) | N/A |
  | 2025 | Code2MCP: Transforming Code Repositories into MCP Services | arXiv | [paper](https://arxiv.org/abs/2509.05941) | [code](https://github.com/DEFENSE-SEU/Code2MCP) |

  </details>

</details>

<details open>
<summary><b>2.4 Full Scaffolding</b></summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2025 | Darwin Godel Machine: Open-Ended Evolution of Self-Improving Agents | arXiv | [paper](https://arxiv.org/abs/2505.22954) | [code](https://github.com/jennyzzt/dgm) |
  | 2025 | Huxley-Gödel Machine: Human-Level Coding Agent Development by an Approximation of the Optimal Self-Improving Machine | arXiv | [paper](https://arxiv.org/abs/2510.21614) | [code](https://github.com/metauto-ai/HGM) |
  | 2025 | Gödel Agent: A Self-Referential Agent Framework for Recursive Self-Improvement | ACL | [paper](https://arxiv.org/abs/2410.04444) | [code](https://github.com/Arvid-pku/Godel_Agent) |
  | 2025 | AlphaEvolve: A coding agent for scientific and algorithmic discovery | arXiv | [paper](https://arxiv.org/abs/2506.13131) | N/A |
  | 2025 | ShinkaEvolve: Towards Open-Ended And Sample-Efficient Program Evolution | arXiv | [paper](https://arxiv.org/abs/2509.19349) | [code](https://github.com/SakanaAI/ShinkaEvolve) |
  | 2024 | Self-Taught Optimizer (STOP): Recursively Self-Improving Code Generation | COLM | [paper](https://arxiv.org/abs/2410.04444) | [code](https://github.com/microsoft/stop) |
  | 2024 | Automated Design of Agentic Systems | NeurIPS | [paper](https://arxiv.org/abs/2408.08435) | [code](https://github.com/ShengranHu/ADAS) |
  | 2024 | Symbolic Learning Enables Self-Evolving Agents | arXiv | [paper](https://arxiv.org/abs/2406.18532) | [code](https://github.com/aiwaves-cn/agents) |
  | 2025 | Live-SWE-agent: Can Software Engineering Agents Self-Evolve on the Fly? | arXiv | [paper](https://arxiv.org/abs/2511.13646) | [code](https://github.com/OpenAutoCoder/live-swe-agent) |
  
</details>

---

## 📬 Contact & Community

- **Discord**: Join our server 👉 https://discord.gg/fn5rYJhgaz
- **WeChat Group**: Scan the QR code below to join. If the QR code expires, please add the WeChat admin (**13488260597**), and we will invite you to the group.

<p align="center">
  <img src="assets/wechat_group_qr.png" alt="WeChat group QR" width="260">
</p>

---

## 🤝 Contribute
PRs are welcome!  

---

## 📌 Citation
```bibtex
@article{your_survey_2026,
  title={Self-Improvement in Foundation Model Based Agentic Systems: A Survey},
  author={Name1 and ...},
  journal={Preprint},
  year={2025}
}



