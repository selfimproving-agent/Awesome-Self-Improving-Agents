
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

<details>
<summary><b>5.1 Prompt Optimization</b></summary>

- **5.1.1 Black-Box Optimization**
  <details>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2022 | Large Language Models Are Human-Level Prompt Engineers | arXiv | [paper](https://arxiv.org/abs/2211.01910) | [code](https://github.com/keirp/automatic_prompt_engineer) |
  | 2024 | Large Language Models as Optimizers | ICLR | [paper](https://arxiv.org/abs/2309.03409) | [code](https://github.com/google-deepmind/opro) |

  </details>

- **5.1.2 Iterative Refinement**
  <details>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2023 | Self-Refine: Iterative Refinement with Self-Feedback | arXiv | [paper](https://arxiv.org/abs/2303.17651) | [code](https://github.com/madaan/self-refine) |

  </details>

- **5.1.3 Evolutionary Algorithms**
  <details>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2024 | EvoPrompt: Connecting LLMs with Evolutionary Algorithms Yields Powerful Prompt Optimizers | ICLR | [paper](https://arxiv.org/abs/2309.08532) | [code](https://github.com/beeevita/EvoPrompt) |
  | 2024 | WizardLM: Empowering large pre-trained language models to follow complex instructions | ICLR | [paper](https://arxiv.org/abs/2304.12244) | [code](https://github.com/nlpxucan/WizardLM) |

  </details>

- **5.1.4 Textual Gradient**
  <details>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2025 | TextGrad: Automatic "Differentiation" via Text | Nature | [paper](https://arxiv.org/abs/2406.07496) | [code](https://github.com/zou-group/textgrad) |
  | 2025 | metaTextGrad: Automatically optimizing language model optimizers | NeurIPS | [paper](https://arxiv.org/abs/2505.18524) | [code](https://github.com/zou-group/metatextgrad) |

  </details>
  
</details>

<details>
<summary><b>5.2 Memory</b></summary>

- **5.2.1 Memory Object**
  <details>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2024 | Agent Workflow Memory | arXiv | [paper](https://arxiv.org/abs/2409.07429) | [code](https://github.com/zorazrw/agent-workflow-memory) |
  | 2025 | ReasoningBank: Scaling Agent Self-Evolving with Reasoning Memory | arXiv | [paper](https://arxiv.org/abs/2509.25140) | N/A |

  </details>

- **5.2.2 Memory Structure**
  <details>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2025 | SCM: Enhancing Large Language Model with Self-Controlled Memory Framework | DASFAA | [paper](https://arxiv.org/abs/2304.13343) | [code](https://github.com/wbbeyourself/SCM4LLMs) |
  | 2024 | Explore, Select, Derive, and Recall: Augmenting LLM with Human-like Memory for Mobile Task Automation | ACM MobiCom | [paper](https://arxiv.org/abs/2312.03003) | [code](https://github.com/mobilegptsys/MobileGPT) |

  </details>

- **5.2.3 Memory Processing**
  <details>
  <summary>View</summary>

  | 📅 Year | 📝 Title | 🏛️ Venue | 📄 Paper | 💻 Code |
  |------:|--------|--------|--------|--------|
  | 2025 | SEDM: Scalable Self-Evolving Distributed Memory for Agents | ICLR | [paper](https://arxiv.org/abs/2309.08532) | [code](https://github.com/beeevita/EvoPrompt) |
  | 2024 | WizardLM: Empowering large pre-trained language models to follow complex instructions | ICLR | [paper](https://arxiv.org/abs/2509.09498) | N/A |

  </details>
  
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



