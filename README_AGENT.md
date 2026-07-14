# Agent Guide to *Self-Improvements in Modern Agentic Systems: A Survey*

## Purpose

This file is an agent-oriented companion to the survey. It helps readers and AI assistants:

- understand the survey's scope and main arguments;
- define the concept of a self-improving agent and distinguish it from closely related concepts;
- navigate the survey by topic, section, or research question;
- find relevant papers in the survey bibliography;
- compare different approaches to autonomous improvement;
- classify new papers using the taxonomy introduced in the survey;
- produce grounded summaries and literature reviews;
- cite the survey and the works it covers.

Use the manuscript as the primary source. This guide is a navigation and usage layer, not a substitute for the paper.

## Quick Start

For a reliable overview, read in this order:

1. `Paper/tex/Definitions.tex` — formal model of an FM-based agent and self-improvement;
2. `Paper/tex/tax_v2.tex` — the survey taxonomy;
3. `Paper/tex/FM.tex` — foundation-model improvement;
4. `Paper/tex/scaffolding.tex` — prompt, memory, tool, and full-scaffolding improvement;
5. `Paper/tex/evaluation.tex` — how improvement should be measured;
6. `Paper/tex/discussion_and_conclusion.tex` — design implications and future directions.

The complete manuscript entry point is `Paper/self_improving_agents.tex`. Bibliographic records are stored in `Paper/references.bib`.

## Survey Scope and Core Definition

The survey focuses on **foundation-model-based agents**, represented at iteration `t` as:

- **Agent configuration:** $\mathcal{A}_t=(\theta_t,\Sigma_t)$
- **Foundation-model parameters:** $\theta_t$
- **Operational scaffold:** $\Sigma_t=(p_t,m_t,\mathcal{T}_t,g_t)$
  - $p_t$: prompts and persistent instruction structures
  - $m_t$: memory and its read/write/update policies
  - $\mathcal{T}_t$: tools and their invocation interfaces
  - $g_t$: control logic, routing, scheduling, and safety constraints

The transient execution state $X_t$—for example, a temporary dialogue history, intermediate plan, or key-value cache—is **not** itself considered a persistent self-improvement.

The paper defines self-improvement as a **durable, self-induced update** produced from signals arising through the agent's own execution. A method belongs to the survey's central scope when it commits a persistent change to $\theta$ or $\Sigma$, rather than merely improving one answer within a single episode.

## Taxonomy at a Glance

### 1. Foundation-Model Improvement: the Parametric Slow Loop

The scaffold remains fixed while the model parameters change:

$\theta_t \rightarrow \theta_{t+1}$, with $\Sigma_{t+1}=\Sigma_t$.

The survey organizes these methods by the form of the self-induced learning signal:

- **Intrinsic generative demonstrations ($\mathcal{D}_t$)** — the agent generates training examples, demonstrations, reasoning traces, or augmented datasets for supervised-style updates.
- **Intrinsic evaluative feedback ($e_t$)** — the agent produces rewards, preferences, critiques, consistency signals, rubrics, or corrections that guide optimization.
- **Extrinsic exploratory experience ($\tau_t$)** — the agent learns from trajectories grounded in task environments or simulated proxy environments or world models.

This pathway is generally slower and more computationally expensive, but it can consolidate gains into model weights and amortize them across future tasks.

### 2. Scaffolding Improvement: the Non-Parametric Fast Loop

The foundation model remains fixed while the operational scaffold changes:

$\Sigma_t \rightarrow \Sigma_{t+1}$, with $\theta_{t+1}=\theta_t$.

The survey organizes these methods by the component being updated:

- **Prompt improvement** — scalar-feedback search, qualitative-feedback refinement, population-based evolution, and textual-gradient optimization.
- **Memory improvement** — evolution of memory objects, memory structures, and memory processing; the processing lifecycle covers creation, reading, updating, and deletion.
- **Tool improvement** — dynamic tool routing, iterative tool refinement, and autonomous tool creation.
- **Full-scaffolding improvement** — modification of the agent's broader operational logic or codebase, including self-referential improvers that can evolve with the scaffold they modify.

These updates are usually faster, more inspectable, and easier to roll back, but can be task-specific and vulnerable to prompt drift, memory poisoning, tool-interface changes, or unsafe code modification.

## Reading Map

| Reader's question | Primary source |
|---|---|
| What counts as a self-improving agent? | `Paper/tex/Definitions.tex` |
| What does *not* count as persistent self-improvement? | `Paper/tex/Definitions.tex` and the domain discussions in `Paper/tex/applications.tex` |
| Where did the idea come from historically? | `Paper/tex/background.tex` |
| What is the paper's organizing taxonomy? | `Paper/tex/tax_v2.tex` and `Paper/fig/fig_main.pdf` |
| How can an agent improve its foundation model? | `Paper/tex/FM.tex` |
| How can it improve prompts, memory, tools, or its full scaffold? | `Paper/tex/scaffolding.tex` |
| Where are these mechanisms applied? | `Paper/tex/applications.tex` |
| How should improvement be evaluated? | `Paper/tex/evaluation.tex` |
| What are the main design and safety implications? | `Paper/tex/discussion_and_conclusion.tex` |
| What notation does the paper use? | `Paper/tex/notation.tex` |
| What is the full bibliographic record for a citation key? | `Paper/references.bib` |

The application section covers six domains: software engineering, web navigation and automation, games and strategic reasoning, scientific discovery, embodied AI and robotics, and general computer control.

## Using the Survey

### Understand a Concept

Locate the relevant section, explain the concept in the paper's terminology, and distinguish it from nearby concepts. Important distinctions include:

- persistent self-improvement versus transient in-context adaptation;
- model-weight updates versus prompt, memory, tool, or control-logic updates;
- evaluation environments versus methods that actually perform persistent updates; and
- a reusable capability versus the substrate in which it is stored.

### Find Relevant Literature

1. Identify the relevant taxonomy branch and subsection.
2. Extract citation keys from the surrounding manuscript text.
3. Resolve those keys in `Paper/references.bib`.
4. Explain why each work is relevant based on the survey's discussion, not only its title.
5. Consult the original paper before making detailed claims that go beyond the survey's description.

A work should be described as **covered by the survey** only when its citation key appears in the manuscript. Its presence in `Paper/references.bib` alone is insufficient.

### Compare or Classify Methods

Use the dimensions emphasized by the survey:

- update target: $\theta$ or a component of $\Sigma$;
- source of the improvement signal;
- persistence and reversibility;
- computational and interaction cost;
- transfer beyond the improvement environment;
- attribution of gains;
- regression, reward-hacking, and safety risks.

For a new paper, first determine whether it performs a durable update. Then classify it as foundation-model improvement or scaffolding improvement, and assign the appropriate subtype.

### Produce a Grounded Summary or Literature Review

Organize the answer around the survey's taxonomy or a clearly stated research question. For each major claim:

- identify the relevant survey section;
- cite the papers discussed in that context;
- distinguish the survey's synthesis from claims made by individual papers; and
- clearly label any newer or external work not covered by the survey.

## Evidence Rules

When answering from this repository:

1. Ground claims in the manuscript and identify the relevant section or source file.
2. Distinguish among the survey's claims, claims attributed to cited papers, and the assistant's own synthesis.
3. Do not infer a paper's contribution from its title alone.
4. Do not fabricate references or bibliographic metadata.
5. Do not combine metadata from different versions of the same work.
6. If the manuscript does not support an answer, state the limitation rather than speculate.

## Evaluation Lens Used by the Survey

The paper treats self-improvement as a trajectory over iterations, not a single terminal score. When analyzing an evaluation claim, check whether it reports:

- performance across update iterations under a fixed resource budget;
- held-out transfer beyond the data or signal used for improvement;
- compute, API, tool-use, wall-clock, and human-supervision costs;
- regressions on previously solved tasks;
- safety violations and tail risks;
- attribution to the updated component; and
- evaluator independence when an LLM or agent judge is used.

The survey distinguishes **metric-based evaluation** with executable or deterministic checks from **judge-based evaluation** with a parameterized evaluator and rubric. It also distinguishes **mechanism benchmarks**, which isolate an update channel, from **domain benchmarks**, which evaluate complete systems in realistic environments.

## Design Implications and Research Frontiers

The discussion emphasizes three system-level principles:

- use fast scaffold-level exploration together with slower parametric consolidation;
- treat the critic or verifier as governed infrastructure, separate from the generator it evaluates; and
- gate persistent updates through layered validation, permission boundaries, regression testing, and rollback.

The six future directions identified by the survey are:

1. test-time continual adaptation;
2. active exploration and curiosity;
3. parametric distillation and joint optimization of $\theta$ and $\Sigma$;
4. resource-constrained improvement dynamics;
5. multi-agent cooperative co-evolution; and
6. robustness under open-world distribution drift.

## Citing the Survey and Its Sources

Use the latest citation record provided on the project page or repository:

- Project page: <https://selfimproving-agent.github.io/>
- Repository: <https://github.com/selfimproving-agent/awesome-Self-Improving-Agents>

Survey title:

> **Self-Improvements in Modern Agentic Systems: A Survey**

To cite a paper covered by the survey:

1. locate the citation key in the relevant manuscript section;
2. resolve the full record in `Paper/references.bib`;
3. cite the original paper rather than citing the survey as a substitute for that paper's specific contribution; and
4. cite the survey as well when referring to its taxonomy, definitions, comparisons, synthesis, or research agenda.
