
# Awesome Self-Improving FM-Based Agents [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated, continuously updated resource list for **Self-Improvement in Foundation Model Based Agentic Systems**.  
> This repo accompanies the survey paper: _"Self-Improvement in Foundation Model Based Agentic Systems: A Survey"_ (2025).

---

## 🌐 Contents
- [Definition & Scope](#definition--scope)
- [Survey Paper](#survey-paper)
- [Taxonomy](#taxonomy)
- [Key Literature](#key-literature)
- [Benchmarks & Datasets](#benchmarks--datasets)
- [Codebases](#codebases)
- [Evaluation & Metrics](#evaluation--metrics)
- [Chronological Timeline](#chronological-timeline)
- [Contribute](#contribute)
- [Citation](#citation)

---

## 🧩 Definition & Scope
This repository focuses on:
- Foundation-Model-Based Agents
- Autonomous Self-Improvement
- Agentic Reinforcement Learning & Policy Optimization
- Knowledge Accumulation and Skill Growth
- Tool-Augmented Adaptation
- Continual Learning & Self-Correction
- Meta-Learning / Self-Play / Scaling Laws for Agents

---

## 📄 Survey Paper
🔗 **Coming soon** — Preprint in preparation.   
*(Add arXiv link here once uploaded.)*

<p align="center">
  <img src="assets/fig.png" alt="Main figure of the survey" width="95%">
</p>

---

## 🧭 Taxonomy
| Category | Description |
|----------|--------------|
| Architectural Self-Improvement | Structure & capability changes |
| Data Self-Improvement | Synthetic data & feedback loops |
| Training Self-Improvement | RL, meta-learning, gradient-based updates |
| Tool Self-Improvement | Tool use, planner evolution, memory |
| Evaluation Self-Improvement | Self-diagnostics, reward shaping |

> (*Customize according to your paper’s structure.*)

---

## 📚 Key Literature
### Core Papers

<details open>
<summary><b>5.1 Prompt Optimization</b></summary>

- **5.1.1 Black-Box Optimization**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2022 | Large Language Models Are Human-Level Prompt Engineers | arXiv | [paper](https://arxiv.org/abs/2211.01910) | [code](https://github.com/keirp/automatic_prompt_engineer) |
  | 2024 | Large Language Models as Optimizers | ICLR | [paper](https://arxiv.org/abs/2309.03409) | [code](https://github.com/google-deepmind/opro) |

  </details>

- **5.1.2 Iterative Refinement**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2023 | Self-Refine: Iterative Refinement with Self-Feedback | arXiv | [paper](https://arxiv.org/abs/2303.17651) | [code](https://github.com/madaan/self-refine) |
  | 2023 | Chain of Hindsight Aligns Language Models with Feedback | arXiv | [paper](https://arxiv.org/abs/2302.02676) | [code](https://github.com/haoliuhl/chain-of-hindsight) |
  | 2023 | Reflexion: Language Agents with Verbal Reinforcement Learning | NeurIPS  | [paper](https://arxiv.org/abs/2303.11366) | [code](https://github.com/noahshinn/reflexion) |
  | 2024 | Self-Improving Customer Review Response Generation Based on LLMs | COLING  | [paper](https://arxiv.org/abs/2405.03845) | N/A |

  </details>

- **5.1.3 Evolutionary Algorithms**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2024 | EvoPrompt: Connecting LLMs with Evolutionary Algorithms Yields Powerful Prompt Optimizers | ICLR | [paper](https://arxiv.org/abs/2309.08532) | [code](https://github.com/beeevita/EvoPrompt) |
  | 2024 | WizardLM: Empowering large pre-trained language models to follow complex instructions | ICLR | [paper](https://arxiv.org/abs/2304.12244) | [code](https://github.com/nlpxucan/WizardLM) |
  | 2025 | Tournament of Prompts: Evolving LLM Instructions Through Structured Debates and Elo Ratings | KDD | [paper](https://arxiv.org/abs/2506.00178v2) | N/A |
  | 2023 | Promptbreeder: Self-Referential Self-Improvement Via Prompt Evolution | arXiv | [paper](https://arxiv.org/abs/2309.16797) | N/A |

  </details>

- **5.1.4 Textual Gradient**
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
<summary><b>5.2 Memory</b></summary>

- **5.2.1 Memory Object**
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

- **5.2.2 Memory Structure**
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

- **5.2.3 Memory Processing**
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
<summary><b>5.3 Tool</b></summary>

- **5.3.1 Dynamic Tool Routing**
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

- **5.3.2 Iterative Tool Refinement**
  <details open>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2025 | STELLA: Self-Evolving LLM Agent for Biomedical Research | arXiv | [paper](https://arxiv.org/abs/2507.02004) | [code](https://github.com/zaixizhang/STELLA) |
  | 2025 | SkillWeaver: Web Agents can Self-Improve by Discovering and Honing Skills | arXiv | [paper](https://arxiv.org/abs/2504.07079) | [code](https://github.com/OSU-NLP-Group/SkillWeaver) |
  | 2025 | PyVision: Agentic Vision with Dynamic Tooling | arXiv | [paper](https://arxiv.org/abs/2507.07998) | [code](https://github.com/agents-x-project/PyVision) |
  | 2025 | From Exploration to Mastery: Enabling LLMs to Master Tools via Self-Driven Interactions | ICLR | [paper](https://arxiv.org/abs/2410.08197) | [code](https://github.com/quchangle1/DRAFT) |

  </details>

- **5.3.3 Autonomous Tool Creation**
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
<summary><b>5.4 Full Scaffolding</b></summary>

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




### Related Surveys
- ...

---

## 📊 Benchmarks & Datasets
| Name | Task Type | Modality | Link |
|------|------------|-----------|------|

---

## 📦 Codebases
| Framework | Area | Link |
|-----------|------|------|

---

## 🧪 Evaluation & Metrics
- Trajectory improvement
- Self-play capability score
- Return-on-feedback (RoF)
- Scaling-based efficiency measures

---

## ⏳ Chronological Timeline
```

2021 - Early FM-based agents
2023 - Emergence of tool-use agents
2024 - Self-refinement & reflection-led improvement
2025 - Self-improving agent ecosystems

````

---

## 🤝 Contribute
PRs are welcome!  
Please follow `CONTRIBUTE.md` (to be added) and standard Awesome list guidelines.

---

## 📌 Citation
```bibtex
@article{your_survey_2025,
  title={Self-Improvement in Foundation Model Based Agentic Systems: A Survey},
  author={Your Name and ...},
  journal={Preprint},
  year={2025}
}



