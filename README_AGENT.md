# Agent Guide to *Self-Improvements in Modern Agentic Systems: A Survey*

## Purpose

This file is an agent-oriented companion to the survey. It helps readers and AI assistants:

- understand the paper's definitions and taxonomy;
- locate the relevant sections, figures, and cited works;
- compare self-improvement mechanisms on a common basis;
- build grounded reading lists from the survey bibliography; and
- cite the survey without inventing metadata.

Use the manuscript as the primary source. This guide is a navigation layer, not a substitute for the paper.

## Quick Start

For a reliable overview, read in this order:

1. `Paper/tex/Definitions.tex` — formal model of an FM-based agent and self-improvement;
2. `Paper/tex/tax_v2.tex` — the active taxonomy used by the manuscript;
3. `Paper/tex/FM.tex` — foundation-model improvement;
4. `Paper/tex/scaffolding.tex` — prompt, memory, tool, and full-scaffolding improvement;
5. `Paper/tex/evaluation.tex` — how improvement should be measured;
6. `Paper/tex/discussion_and_conclusion.tex` — design implications and future directions.

The complete manuscript entry point is `Paper/self_improving_agents.tex`. Bibliographic records are stored in `Paper/references.bib`.

> **Important:** the main manuscript includes `Paper/tex/tax_v2.tex`. Treat `Paper/tex/taxonomy.tex` as non-canonical unless a maintainer explicitly says otherwise.

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
- **Extrinsic exploratory experience ($\tau_t$)** — the agent learns from trajectories grounded in task environments or simulated proxy environments/world models.

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

### 3. Skills Cut Across Both Pathways

The survey treats a **skill** as a reusable, serialized update rather than a separate substrate. A skill may be stored in model weights, prompts, memory, tools, or control logic. When discussing skills, identify both:

1. the capability or reusable update; and
2. the substrate in which it is retained.

## Reading Map

| Reader's question | Primary source |
|---|---|
| What counts as a self-improving agent? | `Paper/tex/Definitions.tex` |
| What does *not* count as persistent self-improvement? | `Paper/tex/Definitions.tex` and the domain discussions in `applications.tex` |
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

## How to Use the Survey with an AI Agent

An agent can use this repository to perform four common tasks.

### Explain a Concept

Locate the relevant section, explain the concept in the paper's terminology, and distinguish it from nearby concepts. For example, separate:

- persistent scaffold updates from transient in-context adaptation;
- evaluation environments from self-improving methods;
- model-weight updates from prompt, memory, tool, or control-logic updates;
- a reusable skill from the substrate in which the skill is stored.

### Find Relevant Literature

1. Identify the relevant taxonomy branch and subsection.
2. Extract citation keys from the surrounding manuscript text.
3. Resolve those keys in `Paper/references.bib`.
4. Explain why each work is relevant based on the survey's discussion—not only its title.
5. If a detailed claim about an individual paper is required, consult the original paper before attributing that claim to it.

A work should be described as **covered by the survey** only when its citation key appears in the active manuscript source. Its presence in `references.bib` alone is insufficient.

### Compare Methods

Compare methods along explicit dimensions used in the survey:

- update target: $\theta$ or a component of $\Sigma$;
- learning signal: demonstrations, evaluative feedback, trajectories, critiques, scores, or execution errors;
- persistence and reversibility;
- computational and interaction cost;
- transfer beyond the improvement environment;
- attribution of gains;
- regression, reward-hacking, and safety risks.

Do not reduce comparison to final benchmark scores when the paper emphasizes learning trajectories, budgets, transfer, and regressions.

### Build a Reading Path

Start with the taxonomy section, then select the mechanism subsection, application domain, and evaluation protocol most relevant to the reader's goal. Present a short ordered list and explain the role of each paper: foundational concept, representative mechanism, application system, benchmark, or safety/evaluation work.

## Grounding Rules for Agent Responses

When answering from this repository:

1. **Ground claims in the active manuscript.** Name the relevant section or source file.
2. **Separate three layers clearly:**
   - claims made by this survey;
   - claims attributed to papers cited by the survey; and
   - the agent's own synthesis or external knowledge.
3. **Do not infer a paper's contribution from its title alone.** Use the local survey context and, when necessary, the original paper.
4. **Never fabricate references or metadata.** Do not invent authors, titles, venues, dates, DOIs, URLs, or arXiv identifiers.
5. **Do not mix versions.** A preprint and its published version may have different metadata; use one coherent record.
6. **Label additions outside the survey.** If newer or external works are introduced, mark them as “not currently covered by the survey.”
7. **State uncertainty.** If the manuscript does not support an answer, say so rather than filling the gap with speculation.

A useful response structure is:

- **Answer**
- **Evidence from the survey** — section/file and the relevant distinction
- **Relevant cited works** — titles and citation keys
- **Outside-survey additions** — only when requested, clearly labeled
- **Limitations or uncertainty**

## Evaluation Lens Used by the Survey

The paper treats self-improvement as a trajectory over iterations, not a single terminal score. When analyzing an evaluation claim, check whether it reports:

- performance across update iterations under a fixed resource budget;
- held-out transfer beyond the data or signal used for improvement;
- compute, API, tool-use, wall-clock, and human-supervision costs;
- regressions on previously solved tasks;
- safety violations and tail risks;
- attribution to the updated component;
- evaluator independence when an LLM or agent judge is used.

The survey distinguishes **metric-based evaluation** with executable or deterministic checks from **judge-based evaluation** with a parameterized evaluator and rubric. It also distinguishes **mechanism benchmarks**, which isolate an update channel, from **domain benchmarks**, which evaluate complete systems in realistic environments.

## Design Implications and Research Frontiers

The discussion emphasizes three system-level principles:

- use fast scaffold-level exploration together with slower parametric consolidation;
- treat the critic or verifier as governed infrastructure, separate from the generator it evaluates;
- gate persistent updates through layered validation, permission boundaries, regression testing, and rollback.

The six future directions identified by the survey are:

1. test-time continual adaptation;
2. active exploration and curiosity;
3. parametric distillation and joint optimization of $\theta$ and $\Sigma$;
4. resource-constrained improvement dynamics;
5. multi-agent cooperative co-evolution; and
6. robustness under open-world distribution drift.

## Citing the Survey

Use the newest canonical public record linked from the project page:

- Project page: <https://selfimproving-agent.github.io/>
- Repository: <https://github.com/selfimproving-agent/awesome-Self-Improving-Agents>

The manuscript title is:

> **Self-Improvements in Modern Agentic Systems: A Survey**

Before a canonical DOI or arXiv identifier is available, a provisional citation may be written as:

> Zhe Ren et al. “Self-Improvements in Modern Agentic Systems: A Survey.” Preprint, 2026.

Do not invent a DOI, arXiv identifier, venue, acceptance status, or publication date. Once a canonical preprint or published version is listed on the project page, prefer its generated citation metadata. When a peer-reviewed version becomes available, cite that version unless the preprint itself is the object being discussed.

## Example Prompts

```text
Read README_AGENT.md and the survey source. Explain the paper's formal
definition of self-improvement and why transient in-context adaptation alone
does not qualify. Cite the relevant source files and equations.
```

```text
Using the survey's taxonomy, find the works most relevant to self-improving
agent memory. Group them by memory object, structure, and processing, and give
the BibTeX citation key for each work.
```

```text
Compare foundation-model improvement with scaffolding improvement in terms of
update signals, persistence, cost, reversibility, transfer, and safety risks.
Ground the comparison in the survey rather than external intuition.
```

```text
Build a reading path for self-improving software-engineering agents. Separate
benchmarks and evaluation substrates from methods that perform persistent
updates to the model or scaffold.
```

```text
Identify the evaluation requirements this survey recommends for a new
self-improving agent. Turn them into an experiment checklist and state which
requirements are unsupported by the proposed experiment.
```
