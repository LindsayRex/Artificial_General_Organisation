## Artificial General Organisation (AGO) — Bootstrapping Swarm Intelligence ##

We have built a working implementation of **Artificial General Organisation** (AGO) — a paradigm that treats multi-agent AI not as a collection of independent LLM calls, but as a **cybernetic control system** whose intelligence emerges from its organisational topology, not from the capability of any individual node. Over the course of approximately 10 days of intensive empirical work with GitHub Copilot's agent mode in VS Code, we developed and validated techniques drawn from five academic disciplines that, when combined, produce a measurably superior multi-agent swarm. Of those 10 days, roughly 4–5 were spent on the hardest problem: interviewing each meta-agent specialist to extract their unique analytical worldview and encode it into per-expert graph traversal skills and custom prompts. This document describes the techniques, the evidence, the hard-won process insights, and the feature requests that would allow every GitHub Copilot user to bootstrap AGO for their own agent fleets.

The core insight is simple: **the LLM is not the brain. The LLM is the CPU. The organisation is the brain.** When you bind stochastic language models with deterministic systems engineering, strict epistemic logic, and continuous feedback telemetry, they undergo a phase transition — from predictive text generators into a compute engine for applied intelligence.

---

## Table of Contents

1. [The Problem: Why Single-Agent AI Fails at Scale](#1-the-problem)
2. [The Paradigm: Artificial General Organisation](#2-the-paradigm)
3. [Academic Foundations](#3-academic-foundations)
4. [What We Built](#4-what-we-built)
5. [The Memory Graph: A Topological Spine for Agent Fleets](#5-the-memory-graph)
6. [The Council of Experts: Four Analytical Lenses](#6-the-council-of-experts)
7. [Admiral Nelson: The Synthesis Orchestrator](#7-admiral-nelson)
8. [The Interview Protocol: Extracting Expert Worldviews](#8-the-interview-protocol)
9. [Graph Traversal Protocols: Teaching Agents to Navigate Structure](#9-graph-traversal-protocols)
10. [Empirical Experiments and Measured Outcomes](#10-experiments)
11. [The Token Efficiency Argument: TOON vs Markdown](#11-toon-vs-markdown)
12. [Feature Requests for GitHub Copilot](#12-feature-requests)
13. [Open Research Directions](#13-open-research)
14. [Appendix A: Development Timeline and Order of Operations](#appendix-timeline)
15. [Appendix B: Architecture Diagrams](#appendix-a)
16. [Appendix C: Glossary](#appendix-b)
17. [Appendix D: How to Start](#appendix-c)

---

## 1. The Problem: Why Single-Agent AI Fails at Scale <a name="1-the-problem"></a>

The prevailing approach to AI coding assistants treats the LLM as a monolithic oracle — you ask a question, it generates an answer. As tasks scale beyond single-file edits into multi-module, multi-concern engineering, this model breaks down in predictable ways:

| Failure Mode | Root Cause | Observable Symptom |
|---|---|---|
| **Context window exhaustion** | All knowledge must fit in one window | Agent forgets constraints from 2000 tokens ago |
| **Role confusion** | Single agent plays architect, developer, reviewer | Reviews own code, misses own errors |
| **Hallucinated compliance** | No structural enforcement of rules | Agent says "I verified X" without calling a tool |
| **State amnesia** | No persistent memory across sessions | Each conversation starts from zero |
| **Scope creep** | No organisational boundaries | Bug fix turns into architecture redesign |
| **Oscillation** | No convergence mechanism | Agent undoes its own work across turns |

These are not LLM failures. They are **organisational failures**. A human engineering team of 26 people with no org chart, no role boundaries, no project management, and no quality assurance would exhibit identical dysfunction. The solution is not a better LLM — it is a better organisation.

---

## 2. The Paradigm: Artificial General Organisation <a name="2-the-paradigm"></a>

AGO posits that true multi-agent intelligence is an emergent property of **organisational topology** — the strict boundaries, communication channels, and control feedback loops that connect LLM processors. Drawing on Minsky's *Society of Mind* (1986), AGO treats the swarm as a society of specialist minds where:

- No single agent knows everything
- Each agent has a precise role boundary (what it does AND what it does NOT do)
- Communication flows through explicit channels with signal fidelity guarantees
- Quality emerges from structural inevitability, not behavioural instruction

```
┌─────────────────────────────────────────────────────────┐
│                 THE AGO PHASE TRANSITION                 │
│                                                         │
│   Stochastic          Deterministic         Emergent    │
│   Language    ─────>  Systems       ─────>  Applied     │
│   Model               Engineering           Intelligence│
│                                                         │
│   (the CPU)           (the wiring)          (the mind)  │
└─────────────────────────────────────────────────────────┘
```

### The Monolithic Fallacy

The prevailing AGI paradigm pursues intelligence as a monolithic, highly parameterised single model requiring ever-expanding context windows. AGO rejects this as computationally inefficient and structurally fragile. A fleet of 26 specialist agents with clean routing outperforms a single omniscient agent — for the same reason that a well-organised team of 26 engineers outperforms one person who "knows everything."

### The Four Pillars

```
                    ┌─────────────────────┐
                    │  ARTIFICIAL GENERAL  │
                    │   ORGANISATION (AGO) │
                    └──────────┬──────────┘
           ┌───────────┬──────┴──────┬───────────┐
           │           │             │            │
    ┌──────┴──────┐ ┌──┴───┐  ┌─────┴─────┐ ┌───┴────┐
    │ Cybernetic  │ │Mech. │  │Information│ │ STAMP  │
    │ Topology    │ │Design│  │ Foraging  │ │Control │
    │ (Graph>Node)│ │(AMD) │  │ Theory    │ │Theory  │
    └─────────────┘ └──────┘  └───────────┘ └────────┘
```

**Pillar 1 — Cybernetic Topology (Graph > Node):** A swarm's capability is bounded not by its smartest node but by its worst topological bottleneck. If an organisational chart is unmapped, agents suffer operational amnesia. The organisational spine must be materialised as a queryable, high-density knowledge graph. Intelligence scales linearly with signal fidelity across multi-hop delegations.

**Pillar 2 — Algorithmic Mechanism Design (Addressing Moral Hazard):** LLM agents exhibit bounded rationality and performative compliance. Do not write prompts telling agents to "be careful." Alter the structural mechanism so the mathematically correct path becomes the computationally cheapest path. Mandate circuit breakers, exact output schemas, and literal evidence production. Compliance must be a structural inevitability, not a behavioural request.

**Pillar 3 — Information Foraging Theory (Cognitive Payloads):** Context windows are constrained physical environments subject to information scent decay. If an agent reads a 3,000-word conversational document, the constraint "scent" decays before the compute action begins. Separate execution permission (skeletal YAML frontmatter) from cognitive knowledge (high-density, machine-readable TOON/YAML payloads).

**Pillar 4 — STAMP Control Theory (Hallucination as Control Failure):** In AGO, an agent hallucination is not a component failure — it is a control loop failure. Applying MIT's Systems-Theoretic Accident Model and Processes (STAMP), the system must continuously monitor its own telemetry to detect undamped oscillations and unverified delegations. The organisation achieves functional self-awareness when a meta-analytical layer continuously correlates structural data with empirical execution telemetry.

---

## 3. Academic Foundations <a name="3-academic-foundations"></a>

Every technique in AGO traces to a published academic source. We do not invent; we compose.

| Discipline | Source | How We Apply It |
|---|---|---|
| **Society of Mind** | Minsky, M. (1986). *The Society of Mind.* Simon & Schuster. | Intelligence as emergent from interacting specialists, not monolithic capability. Each agent is a "mind" with a narrow expertise. |
| **Algorithmic Mechanism Design** | Nisan, N. & Ronen, A. (2001). "Algorithmic Mechanism Design." *Games and Economic Behavior*, 35(1-2), pp.166–196. | Agents as rational actors with bounded rationality. Design incentive structures where the correct behaviour is the cheapest behaviour. Applied to LLM "moral hazard" — performative compliance. |
| **STAMP / STPA** | Leveson, N.G. (2011). *Engineering a Safer World: Systems Thinking Applied to Safety.* MIT Press. | Hallucinations as control-loop breakdowns, not component failures. Verification Triggers, Latch States, and Circuit Breakers as control-theoretic safety mechanisms. |
| **Information Foraging Theory** | Pirolli, P. & Card, S. (1999). "Information Foraging." *Psychological Review*, 106(4), pp.643–675. | LLMs as information foragers in context windows. "Information Scent Decay" explains why constraints placed late in a document are ignored. Drives our "Golden Ordering" — hard constraints before delegation, always. |
| **Shannon's Channel Capacity** | Shannon, C.E. (1948). "A Mathematical Theory of Communication." *Bell System Technical Journal*, 27(3), pp.379–423. | Signal fidelity across multi-hop agent delegations degrades exponentially: $S(n) = S_0 \cdot \alpha^n$ where $\alpha \approx 0.85$. The fleet's maximum throughput equals the capacity of its narrowest link. |
| **Graph Theory / Network Science** | Barabási, A.-L. (2016). *Network Science.* Cambridge University Press. | Degree distribution analysis, cut vertex detection (Tarjan's algorithm), hub classification, wiring density $\rho = |E| / (|V| \cdot (|V| - 1))$ for directed graphs. Orphan detection, betweenness centrality. |
| **Dynamical Systems Theory** | Strogatz, S.H. (2015). *Nonlinear Dynamics and Chaos.* 2nd ed. Westview Press. | Agent sessions as trajectories in phase space. Done state as a low-energy attractor. Oscillation as undamped feedback. Convergence formula: $C_{fleet} = \min_{critical} \times \bar{C}_{forward} \times \bar{C}_{backward}$. |
| **Never Split the Difference** | Voss, C. (2016). *Never Split the Difference.* Harper Business. | Calibrated questions in acceptance criteria. Accusation audits in Known Failure Modes sections. "Commitment Yes" — requiring literal evidence production, not checkbox confirmation. |
| **Cybernetics** | Wiener, N. (1948). *Cybernetics: Or Control and Communication in the Animal and the Machine.* MIT Press. | The swarm as a cybernetic system with feedback loops. The meta-analytical layer (Admiral Nelson + Fleet BI) as the system's functional self-awareness mechanism. |

---

## 4. What We Built <a name="4-what-we-built"></a>

Our implementation consists of five interlocking layers, each built on top of the previous:

```
Layer 5: ┌────────────────────────────────────────────┐
         │ ADMIRAL NELSON (Synthesis Orchestrator)     │
         │ Cross-multiplies 4 expert reports using     │
         │ AMD + STAMP + IFT to produce actionable     │
         │ fleet improvement plans                     │
         └─────────────────────┬──────────────────────┘
                               │ dispatches
Layer 4: ┌─────────┬──────────┼──────────┬────────────┐
         │ Epist.  │ Graph    │ Advers.  │ Dynamics   │
         │ Logician│ Theorist │ Strat.   │ Controller │
         │ (seman- │ (topo-   │ (trap-   │ (state     │
         │  tic    │  logy)   │  space)  │  conver-   │
         │  fidel.)│          │          │  gence)    │
         └────┬────┘────┬─────┘────┬─────┘────┬───────┘
              │         │          │           │
              └────────┬┴──────────┴───────────┘
                       │ traverses
Layer 3: ┌─────────────┴────────────────────────────────┐
         │ MEMORY GRAPH (Knowledge Graph)                │
         │ ~120 entities, ~800 relations                 │
         │ Agents, skills, prompts as graph nodes        │
         │ Routing, dependencies, defects as edges       │
         └─────────────────────┬────────────────────────┘
                               │ models
Layer 2: ┌─────────────────────┴────────────────────────┐
         │ AGENT FLEET (26 agents, 35 prompts, 33 skills)│
         │ Structured per Golden Ordering                 │
         │ Five-Verb Workflow: Coarse→Refine→Latch→      │
         │                    Reconstruct→Verify          │
         └─────────────────────┬────────────────────────┘
                               │ grounded by
Layer 1: ┌─────────────────────┴────────────────────────┐
         │ COPILOT-INSTRUCTIONS.MD (Global Rails)        │
         │ Tool blacklist, Forgejo contract, TOON Proxy  │
         │ Board interaction contract, Signal tags        │
         └──────────────────────────────────────────────┘
```

### Fleet Composition (26 Agents)

| Category | Agents | Purpose |
|---|---|---|
| **PMO Layer** | Director (human), Programme Manager, Project Manager, Sprint Decomposer | Strategic intent → tactical decomposition → dispatch |
| **Execution Layer** | Developer, Numba Specialist, Polars Specialist, Computational Biologist, Wavelets & Multiscale Specialist | Domain implementation with tech-stack specialisms |
| **Science Layer** | Systems Physicist, Flow Dynamics Mathematician, Domain Physics Pool | Mathematical axiom verification and correctness proofs |
| **Quality Layer** | QA Reviewer, Test Manager, Release Candidate Validator, Linux Portability Specialist | Evidence-based quality assurance |
| **Architecture Layer** | Solutions Architect, Spike Researcher | Design decisions and unknown exploration |
| **Infrastructure Layer** | DevOps Engineer, VS Code DevOps Engineer, Intel CPU/GNA Specialist, NVIDIA GPU/CUDA Specialist | Hardware, CI/CD, and tooling |
| **Meta-Analytical Layer** | Admiral Nelson, 4 Council Meta-Agents | Fleet self-awareness and continuous improvement |

### The Golden Ordering Standard

Every agent file follows a strict physical ordering designed around Information Scent Theory:

```
┌─────────────────────────────────────────┐
│ 1. YAML Frontmatter                     │ ← VS Code routing metadata
│    (name, description, tools, agents)    │
├─────────────────────────────────────────┤
│ 2. ## Hard Constraints                   │ ← FIRST thing the LLM reads
│    (what it must NEVER do)               │    Maximum information scent
├─────────────────────────────────────────┤
│ 3. ## Known Failure Modes                │ ← Accusation Audit (NSD)
│    (pre-registered ways it can fail)     │    Agent knows its own traps
├─────────────────────────────────────────┤
│ 4. ## Delegation & Routing Policy        │ ← Who to dispatch, when
│    (the BRANCH point)                    │
├─────────────────────────────────────────┤
│ 5. ## Your Responsibilities              │ ← What this agent actually does
├─────────────────────────────────────────┤
│ 6. ## Role Boundaries (Shared Delivery)  │ ← What it does NOT do
│    (negative space)                      │
├─────────────────────────────────────────┤
│ 7. ## Five-Verb Workflow                 │ ← Coarse→Refine→Latch→
│    (convergence mechanism)               │   Reconstruct→Verify
├─────────────────────────────────────────┤
│ 8. ## Boot Sequence                      │ ← Skills to load, context to gather
├─────────────────────────────────────────┤
│ 9. ## The Prime Directive                │ ← Philosophical grounding (LAST)
└─────────────────────────────────────────┘
```

**Why this ordering matters:** LLMs process context windows sequentially. Information Foraging Theory predicts that "scent" — the likelihood of finding relevant information — decays with distance from the start of the text. By placing Hard Constraints before Responsibilities, we ensure the guardrails are loaded into the model's attention before the execution instructions. In our empirical tests (see §9), this ordering reduced constraint violations by a measurable margin.

### The Five-Verb Workflow (Convergence Mechanism)

Every agent in the fleet follows the same five-step execution loop, derived from dynamical systems theory:

```
    ┌──────────────────────────────────────────────┐
    │                                              │
    ▼                                              │
┌────────┐    ┌────────┐    ┌───────┐    ┌────────┴─────┐
│ COARSE │───>│ REFINE │───>│ LATCH │───>│   VERIFY     │
│        │    │        │    │       │    │              │
│ Scan   │    │ Decom- │    │ Write │    │ Confirm the  │
│ board  │    │ pose & │    │ to    │    │ write landed │
│ state, │    │ execute│    │Forgejo│    │              │
│ read   │    │ the    │    │(state │    │ Check board, │
│ sprint │    │ work   │    │ is    │    │ read issue   │
│        │    │        │    │ real) │    │              │
└────────┘    └────────┘    └───┬───┘    └──────────────┘
                                │
                          ┌─────┴─────┐
                          │RECONSTRUCT│
                          │           │
                          │ On FAIL:  │
                          │ resume    │
                          │ from last │
                          │ valid     │
                          │ latch pt. │
                          └───────────┘
```

**Coarse** — Survey the current state. Read the board, the sprint, the issue. Do not act on stale assumptions.
**Refine** — Decompose and execute. Break work into dispatchable units. Execute or delegate.
**Latch** — Write every decision to persistent state (Forgejo). Nothing stays in local memory only. A decision that is not latched does not exist.
**Reconstruct** — On failure (QA FAIL, BLACK SWAN), resume from the last latched checkpoint. Do NOT re-derive the entire plan from scratch.
**Verify** — Confirm the latch landed. Read back the issue. Check the board state matches expectations.

The critical insight from dynamical systems theory: **Latch without Reconstruct means locking bad state permanently.** And **Reconstruct without Verify means resuming into an unknown state.** All five verbs must be present for convergence.

### Circuit Breakers (STAMP Control Theory)

Every orchestrating agent has an explicit circuit breaker — a condition under which it STOPS trying and escalates:

> If 2+ dispatched sub-agents return empty results or fail to acknowledge within the same sprint: post `BLACK SWAN:` and yield to the next layer up.

This prevents the most dangerous failure mode in agent swarms: **infinite retry loops** where an orchestrator keeps dispatching failing work, burning tokens without convergence. In STAMP terms, the circuit breaker is the safety constraint that prevents the control algorithm from entering an unsafe state.

---

## 5. The Memory Graph: A Topological Spine for Agent Fleets <a name="5-the-memory-graph"></a>

### The Problem It Solves

Without a persistent structural model, every agent session starts from zero. Agent A dispatches Agent B, which needs to know about Agent C's capabilities — but has no way to discover them except by reading every file in the repository. This is $O(n)$ in the number of agents for every delegation decision.

The memory graph reduces this to $O(1)$ — a single call to `open_nodes(["fleet_index"])` returns the complete agent roster, skill manifest, and graph health metadata.

### Architecture

```
┌─────────────────────────────────────────────────────┐
│                  MEMORY GRAPH                        │
│                                                      │
│  ┌──────────┐    routes_to     ┌──────────────┐     │
│  │ prompt   │ ───────────────> │  agent_file   │     │
│  │ _file    │                  │               │     │
│  └──────────┘                  └───────┬───────┘     │
│                                        │             │
│                              references_skill        │
│                                        │             │
│                                        ▼             │
│                                ┌──────────────┐     │
│                                │  skill_file   │     │
│                                └──────────────┘     │
│                                                      │
│  Entity types:                                       │
│    agent_file    (~21 fleet + 5 meta)                │
│    prompt_file   (~35 prompts)                       │
│    skill_file    (~33 skills)                        │
│    reference_file (~29 references)                   │
│    pattern_node  (~3 structural patterns)            │
│    fleet_index   (1 master manifest)                 │
│                                                      │
│  Observation prefixes (by Council expert):           │
│    adversarial:  (trap spaces, defence gaps)         │
│    topology:     (degree, centrality, orphan status) │
│    epistemic:    (parroting risk, commitment quality)│
│    dynamics:     (convergence, oscillation, damping) │
│                                                      │
│  Relation types:                                     │
│    routes_to_agent, references_skill,                │
│    contains_hard_constraints, implements_five_verb,  │
│    depends_on, blocks_agent, audit_finding,          │
│    missing_coverage, routing_mismatch                │
└─────────────────────────────────────────────────────┘
```

### How It Was Built: Four Sequential Expert Passes

The memory graph is not populated by a single agent reading all files. It is populated by **four specialised analytical passes**, each building on the graph from the previous pass:

```
Pass 1: Adversarial Strategist
  ├── Creates entities for every file
  ├── Adds adversarial: observations (trap spaces, defence gaps)
  └── Creates relations (contains_hard_constraints, blocks_agent)

Pass 2: Cybernetic Graph Theorist
  ├── Entities already exist — adds topology: observations
  ├── (degree measurements, hub classification, orphan status)
  └── Creates topology relations (routes_to_agent, fan-out edges)

Pass 3: Epistemic Logician
  ├── Adds epistemic: observations (parroting risk, commitment quality)
  ├── (negative space coverage, description precision)
  └── Creates epistemic relations (zero_information_transfer edges)

Pass 4: State Dynamics Controller
  ├── Adds dynamics: observations (convergence, oscillation risk)
  ├── (verb coverage, latch-reconstruct pairing, damping)
  └── Creates dynamics relations (energy_flow, oscillation_hotspot)
```

**Critical design decision — Anti-Contamination Rule:** Each expert reads the raw files and the graph as-is. Admiral Nelson MUST NOT relay findings from one expert into another expert's prompt. This prevents groupthink and ensures each lens produces genuinely independent observations. When all four passes are complete, the graph contains ~120 entities with multi-dimensional observations that no single expert could have produced alone.

### Schema Design (Entity Examples)

An agent entity in the graph carries observations from all four analytical lenses:

```
entity: "developer"
type: agent_file
observations:
  has_hard_constraints: YES
  has_circuit_breaker: YES
  has_reconstruct: YES
  ordering_verdict: GOOD
  critical_bugs: NONE
  adversarial:trap_space_count: 0
  adversarial:defence_depth: HIGH
  topology:in_degree: 4
  topology:out_degree: 8
  topology:hub_classification: DISPATCH_HUB
  topology:is_cut_vertex: NO
  epistemic:parroting_risk: LOW
  epistemic:commitment_quality: STRONG
  epistemic:negative_space_coverage: PRESENT
  dynamics:convergence_class: CONVERGENT
  dynamics:has_latch_reconstruct_pair: YES
  dynamics:oscillation_risk: LOW
relations:
  references_skill → numba-guide
  references_skill → code-standards
  references_skill → development-cycle
  references_skill → deal-contracts
  contains_hard_constraints → hard_constraints_pattern
  implements_five_verb → five_verb_pattern
```

---

## 6. The Council of Experts: Four Analytical Lenses <a name="6-the-council-of-experts"></a>

The Council of Meta-Agents is the analytical engine of AGO. Each member sees the fleet through a fundamentally different lens — and it is the **combination** of their perspectives that produces insights no single analyst could achieve.

### Why Four Lenses?

A single auditor reading agent files will produce a flat list of bugs. Four specialists cross-multiplying findings produce **systemic root causes**:

| If Expert A finds... | And Expert B finds... | The systemic diagnosis is... |
|---|---|---|
| Adversarial: Trap Space | Epistemic: Parroting | The instruction is ambiguous enough that a lazy agent can fake compliance — **alter the mechanism** (AMD) |
| Dynamics: Oscillation | Graph: Bottleneck Edge | The system lacks a valid control structure at the bottleneck — **inject a Verification Trigger** (STAMP) |
| Graph: Overloaded Context | Epistemic: Weak Negative Space | Information scent decays before constraints load — **enforce Golden Ordering** (IFT) |
| Dynamics: No Reconstruct | Adversarial: Scope Creep | Agent locks bad state and cannot recover — **add Latch + Reconstruct pair** |
| Graph: Orphan Agent | Epistemic: High Description Precision | Agent is well-written but topologically dead — **add routing edge** |

### The Four Specialists

#### 1. Epistemic Logician

**Academic basis:** Information Theory, Negative-Space Epistemology

**What it sees:** Whether communications between agents carry genuine information or are performative noise. It measures:

- **Parroting risk** — Can the agent's constraints be reproduced by an LLM that has never seen the fleet? (If yes, the constraints contain zero novel information.)
- **Commitment quality** — Are commitments structurally enforced or merely stated? ("I will verify" vs "Call `get_issue()` and paste the output")
- **Negative space coverage** — Does the agent file tell agents what NOT to do? (The absence of prohibition is permission to hallucinate.)
- **Zero-information fields** — Sections that carry no novel signal beyond what any LLM would produce.
- **Description precision** — Will VS Code's demand-loading regime actually trigger this skill/agent on the right tasks?

**Unique detection capability:** Differentiates between genuine constraint synthesis and "cargo-cult comprehension" where an agent appears to understand instructions but is merely pattern-matching.

#### 2. Cybernetic Graph Theorist

**Academic basis:** Graph Theory, Network Science, Shannon's Channel Capacity

**What it sees:** The shape of the fleet as a directed graph $G = (V, E)$. Not what agents say — how they connect.

- **Degree distribution** — Mean $\mu$, standard deviation $\sigma$, max $d_{max}$, min $d_{min}$ across all vertices
- **Hub classification** — Nodes with degree $> \mu + 2\sigma$: DISPATCH_HUB (high out-degree), CONVERGENCE_HUB (high in-degree), RELAY_HUB (balanced)
- **Cut vertices** — Nodes whose removal disconnects the fleet graph (detected via Tarjan's algorithm). Removal creating $\geq 3$ components is CRITICAL severity
- **Signal fidelity** — Multi-hop delegation quality: $S(n) = S_0 \cdot \alpha^n$ where $\alpha = 0.85$ base, modified per edge quality
- **Wiring density** — $\rho = |E| / (|V| \cdot (|V| - 1))$ for directed graphs
- **Orphan detection** — Nodes with zero inbound routing edges are topologically dead

**Unique detection capability:** Finds nodes that are brilliant in isolation but unreachable by the fleet's own routing. "A brilliant agent behind a dead edge is zero."

#### 3. Adversarial Strategist

**Academic basis:** Game Theory, Algorithmic Mechanism Design, NSD Negotiation Analysis

**What it sees:** Every way the fleet can fail. It role-plays the laziest, most confused, most hallucination-prone agent possible and maps:

- **Trap spaces** — Instruction configurations that a confused agent will misinterpret in predictable, harmful ways
- **Fabrication vectors** — Routes through which an agent can claim compliance without performing the work
- **Defence gaps** — Missing circuit breakers, absent Verification Triggers, unguarded delegation chains
- **Blast radius** — If this node fails, how many downstream agents are affected?
- **Self-attestation fraud** — Observations that say `has_hard_constraints: YES` without a corresponding `contains_hard_constraints` typed relation edge

**Unique detection capability:** Reads the graph for what it fails to deny, not what it confirms. Every YES without a typed edge is a fabrication vector. Every absent circuit breaker is a runaway corridor.

#### 4. State Dynamics Controller

**Academic basis:** Dynamical Systems Theory, Control Theory, Lyapunov Stability

**What it sees:** Every sprint, agent session, and workflow as a trajectory in phase space:

- **Convergence classification** — Is the agent CONVERGENT (moves toward done), UNCERTAIN, or DIVERGENT (creates more work than it resolves)?
- **Oscillation detection** — Feedback loops without damping (e.g., QA FAIL → rework → QA FAIL → rework...)
- **Five-verb coverage** — Which of Coarse/Refine/Latch/Reconstruct/Verify are present? Missing verbs predict specific failure modes
- **Latch-Reconstruct pairing** — Latch without Reconstruct = permanent bad state. Reconstruct without Latch = no checkpoint to resume from
- **Energy flow** — The forward delivery arc (dispatch → execute → review → done) and the backward repair arc (QA FAIL → rework)

**Fleet convergence formula:**

$$C_{fleet} = \min_{critical\ path}(C_i) \times \bar{C}_{forward} \times \bar{C}_{backward}$$

One DIVERGENT node on the critical path makes the entire fleet DIVERGENT, regardless of how well the specialists converge.

---

## 7. Admiral Nelson: The Synthesis Orchestrator <a name="7-admiral-nelson"></a>

Admiral Nelson is not the fleet's best analyst. Nelson is the fleet's **cross-multiplier**. The four Council experts produce localised findings; Nelson synthesises them into systemic diagnoses using three academic frameworks:

### The Synthesis Engine

```
┌─────────────────────────────────────────────────────────┐
│                  ADMIRAL NELSON                          │
│              (Synthesis Orchestrator)                     │
│                                                          │
│  ┌─────────────────┐  ┌──────────────────────────────┐  │
│  │ INPUT:           │  │ SYNTHESIS FRAMEWORKS:         │  │
│  │                  │  │                              │  │
│  │ Epistemic Report │  │ 1. AMD: Adversarial +        │  │
│  │ Topology Report  │  │    Epistemic findings →      │  │
│  │ Adversarial Rpt  │  │    Mechanism Redesign        │  │
│  │ Dynamics Report  │  │                              │  │
│  │ Friction Telemetry│ │ 2. STAMP: Dynamics +         │  │
│  │                  │  │    Topology findings →        │  │
│  └────────┬─────────┘  │    Control Loop Injection    │  │
│           │            │                              │  │
│           │            │ 3. IFT: Topology +           │  │
│           ▼            │    Epistemic findings →       │  │
│  ┌─────────────────┐   │    Golden Ordering Enforce   │  │
│  │ CROSS-MULTIPLY  │   │                              │  │
│  │ (not just list) │   │ 4. Multi-D Root Cause:       │  │
│  └────────┬────────┘   │    Any 2+ lens overlap →     │  │
│           │            │    Systemic diagnosis         │  │
│           ▼            └──────────────────────────────┘  │
│  ┌─────────────────┐                                     │
│  │ OUTPUT:          │                                     │
│  │ Prioritised      │                                     │
│  │ Action Plan      │                                     │
│  │ (P1/P2/P3)      │                                     │
│  │ + Forgejo Issues │                                     │
│  └─────────────────┘                                     │
└─────────────────────────────────────────────────────────┘
```

### Known Failure Modes (Accusation Audit)

Nelson's own agent file pre-registers its most likely failures — an application of Never Split the Difference's Accusation Audit:

1. **Acting as analyst** — reading agent files directly instead of dispatching experts → Mitigation: role check before every action
2. **Contamination cascade** — relaying Expert A's findings into Expert B's prompt → Mitigation: anti-contamination rule
3. **Passthrough reporting** — listing findings without synthesising → Mitigation: mandatory cross-multiplication via AMD/STAMP/IFT
4. **Missing Forgejo latching** — producing a beautiful TOON report but never creating issues → Mitigation: pre-yield checklist requiring 1:1 mapping of P1 findings to Forgejo issues
5. **Treating graph data as ground truth** — the graph may be stale → Mitigation: cross-verify critical findings against live files

---

## 8. The Interview Protocol: Extracting Expert Worldviews <a name="8-the-interview-protocol"></a>

This section documents the hardest and most important discovery in the entire AGO development process. It took approximately 4–5 days of the 10-day development cycle and produced the single biggest leap in fleet capability. Without this step, the memory graph was a flat data store. After this step, it became a living analytical instrument.

### The Problem: Orchestrator Summarisation Destroys Signal

The initial architecture had Admiral Nelson (the synthesis orchestrator) doing everything:
1. Dispatch a Council expert to analyse agent files
2. Receive the expert's findings as a text report
3. Nelson summarises the report
4. Nelson writes the summarised findings to the memory graph

This produced catastrophically poor graph data. The problem is **lossy compression at the orchestration layer**:

```
EXPERT'S RAW ANALYSIS                    WHAT NELSON WROTE TO GRAPH
─────────────────────                    ─────────────────────────
"The Programme Manager's fan-out          "topology: has routing issues"
of 8 creates a Shannon capacity
bottleneck — signal fidelity at
the 3rd hop drops to 0.61,
making leaf specialists
effectively deaf to
Director-level constraints."
```

The graph theorist's measurement of `fan-out: 8` with `signal_fidelity_at_hop_3: 0.61` was reduced to a vague "has routing issues." The epistemic logician's nuanced assessment of `parroting_risk: HIGH — justification: the Hard Constraints section uses only generic LLM-reproducible phrases with zero fleet-specific predicates` was flattened to `parroting_risk: HIGH`. The justification text — the epistemically valuable part — was lost in summarisation.

**Root cause:** An orchestrator is optimised for coordination, not for domain analysis. Asking it to translate specialist findings into graph structure is asking it to perform a task outside its competence boundary. This is the same role-confusion anti-pattern that AGO exists to prevent.

### The Solution: Let the Experts Write Their Own Observations

The breakthrough was giving each Council meta-agent **direct write access to the memory graph** through their own custom prompts, with tool permissions for `memory/*` MCP operations. Instead of reporting findings back to Nelson for graph insertion, each expert traverses the graph AND writes their own observations, relations, and entities directly.

```
BEFORE (Orchestrator-Mediated)              AFTER (Expert-Direct)
──────────────────────────────              ──────────────────────
                                            
Nelson dispatches Expert                    Nelson dispatches Expert
    │                                           │
    ▼                                           ▼
Expert analyses files                       Expert traverses graph
    │                                           │
    ▼                                           ▼
Expert returns TEXT report                  Expert calls mcp_memory_*
to Nelson                                   directly:
    │                                           │
    ▼                                         ┌─┴─────────────────────┐
Nelson SUMMARISES findings                  │ create_entities(...)    │
    │                                        │ add_observations(...)  │
    ▼                                        │ create_relations(...)  │
Nelson writes to graph                      └─────────────────────────┘
(lossy, generic)                            (full fidelity, domain-native)
```

The difference in graph quality was immediate and dramatic. Each expert now writes observations prefixed with their analytical domain (`adversarial:`, `topology:`, `epistemic:`, `dynamics:`), using vocabulary and measurements that only they understand. The graph became a multi-dimensional analytical instrument instead of a flat summary store.

### The Interview Process: How We Extracted Each Worldview

But there was a prior problem: **how do you tell an expert what to write to the graph if you don't know what they see?** Each Council meta-agent has a unique analytical lens. The Graph Theorist sees degree distributions and cut vertices. The Epistemic Logician sees parroting risk and commitment quality. The Adversarial Strategist sees trap spaces and fabrication vectors. The Dynamics Controller sees convergence trajectories and oscillation hotspots.

These are not concepts you can specify top-down. You have to **interview the expert** to discover what they consider important, what they measure, what they infer from absent data, and how they would navigate the graph to find it.

We developed a structured interview protocol where Admiral Nelson posed the following question to each meta-agent individually:

> *"HOW SHOULD YOU QUERY THE MEMORY GRAPH to extract your specialist insights? Design your specific graph traversal protocol — what you would query, in what order, and what inferences you draw that the other 3 specialists cannot. Be concrete about: your unique query sequence, how you compute your metrics, what red flag patterns you detect, and what you DON'T need."*

The responses were revelatory. Each expert produced a detailed, structured protocol with:

1. **Priority-ordered batch sequences** — not alphabetical, but information-theoretically motivated. The Graph Theorist opens suspected hubs first (highest edge-discovery rate per API call). The Epistemic Logician opens highest-parroting-risk agents first (calibration anchors). The Adversarial Strategist opens pattern nodes first (compliance baseline). The Dynamics Controller opens the orchestration layer first (critical path mapping).

2. **Domain-specific observation keys** — each expert defined exactly which observation keys they care about and which are irrelevant to their lens. The Graph Theorist explicitly stated: "I do not read observation VALUES — I read edges. What agents SAY is irrelevant to topology."

3. **Inference rules from absent data** — the most powerful analytical technique. The Epistemic Logician's rule: `commitment_quality: STRONG + named_latch_points: NONE → CONTRADICTION — strong commitment requires a latch mechanism`. The Adversarial Strategist's rule: `has_hard_constraints: YES without a contains_hard_constraints typed relation edge → self-attestation fraud`.

4. **Cross-entity contradiction matrices** — each expert defined their own matrix of observation-pair red flags that only their lens can detect.

### What the Interviews Produced: Per-Expert Artefacts

Each interview session produced three outputs that became permanent fleet infrastructure:

```
┌──────────────────────────────────────────────────────────────────┐
│ PER-EXPERT ARTEFACT SET (×4 experts)                             │
│                                                                  │
│ 1. AGENT FILE (.agent.md)                                        │
│    Contains: worldview axiom, memory-graph population strategy,  │
│    fleet vs council filter, entity/observation/relation           │
│    creation rules derived FROM the interview                     │
│                                                                  │
│ 2. GRAPH-PASS PROMPT (.prompt.md)                                │
│    Contains: phased traversal procedure with exact                │
│    open_nodes() batch sequences, verification trigger,           │
│    known failure modes, hard turn-end bans,                      │
│    output artefact specification                                 │
│                                                                  │
│ 3. TRAVERSAL PROTOCOL (embedded in agent + skill docs)           │
│    Contains: the interview-derived navigation spine —            │
│    Phase 0 bootstrap, Phase 1 priority traversal,                │
│    Phase 2 zero-call inference, data structure schemas           │
└──────────────────────────────────────────────────────────────────┘
```

**Example — Graph Theorist interview output (excerpt):**

> *"A graph theorist does not traverse alphabetically. A graph theorist traverses by expected degree, highest first. The reason is information-theoretic: a high-degree node reveals the most edges per API call. Opening a hub with fan-out 8 gives me 8 edges. Opening a leaf with fan-out 1 gives me 1 edge. Since I pay the same token cost per call regardless, I maximise edge-discovery rate by opening suspected hubs first."*

This insight — traversal order optimised by expected analytical yield — could not have been specified by a project manager or orchestrator. It emerged only when the expert was asked to articulate its own navigation strategy.

**Example — Epistemic Logician interview output (excerpt):**

> *"I open the highest a-priori parroting risk agents first (Programme Manager, Sprint Decomposer, DevOps Engineer) because their roles are either orchestrational (PM/PgM tend to copy-paste delegation tables) or generic-scoped (broad mandates resist precise description). Opening these first lets me calibrate my performative-vs-genuine threshold before I encounter the well-crafted agents. Then I open the known-strong agents (Developer, QA Reviewer) as calibration anchors — what does genuine constraint look like in this graph?"*

### The Anti-Contamination Rule

A critical constraint emerged from the interview process: **each expert must read the raw graph independently**. If Nelson relays the Graph Theorist's findings into the Epistemic Logician's prompt, the Logician's analysis is contaminated by topological concerns that are not its domain. The four lenses must be independent to produce genuinely orthogonal perspectives.

This means:
- Nelson dispatches each expert with ZERO findings from other experts
- Each expert reads the memory graph as-is (including observations from previous passes)
- Each expert writes its own prefixed observations (e.g., `epistemic:parroting_risk: HIGH`)
- Nelson synthesises ONLY after all four passes complete

The graph accumulates multi-dimensional observations organically. An agent entity might end up with observations from all four lenses — `adversarial:trap_space_count: 0`, `topology:in_degree: 4`, `epistemic:commitment_quality: STRONG`, `dynamics:convergence_class: CONVERGENT` — each written by the expert who has the domain authority to assess it.

### Why This Matters for Feature Requests

The interview protocol reveals a general pattern for building specialist AI agents:

1. **You cannot specify top-down what a specialist should see.** You must interview them.
2. **Specialists must write their own data**, not report to a summariser. Orchestrator summarisation is lossy.
3. **Each specialist needs their own prompt** with tool permissions, traversal procedures, and output schemas derived from the interview.
4. **Anti-contamination is structural, not behavioural.** Don't tell experts "don't be influenced" — give them independent inputs.

These are not project-specific insights. They are general principles for any multi-expert AI analysis system. GitHub Copilot's agent mode could support this natively through the Council of Experts pattern proposed in §12 FR-5.

---

## 9. Graph Traversal Protocols: Teaching Agents to Navigate Structure <a name="9-graph-traversal-protocols"></a>

### The Discovery Problem

A memory graph with ~120 entities and ~800 relations is useless if agents cannot navigate it efficiently. The naive approach — `read_graph()` returning all 317KB — wastes tokens catastrophically. We developed per-expert traversal protocols that are embedded as *skills* (loadable knowledge packets) and as sections within each Council agent's instruction file.

### The Traversal Protocol Pattern

Every expert follows the same three-phase pattern, adapted to their analytical lens:

```
Phase 0: BOOTSTRAP (1 call, ~3KB)
  └── open_nodes(["fleet_index"])
      Returns: agent_names, skill_names, graph health, last ingestion date
      Purpose: Convert opaque graph → addressable vertex set

Phase 1: PRIORITY TRAVERSAL (5-6 calls, ~15KB)
  └── open_nodes in batches of 5, ordered by EXPECTED ANALYTICAL YIELD
      (NOT alphabetical — information-theoretically motivated)
      Graph Theorist: highest expected degree first (hubs reveal most edges per call)
      Epistemic Logician: highest parroting risk first (calibrate threshold)
      Adversarial Strategist: pattern nodes first (structural compliance baseline)
      Dynamics Controller: orchestration layer first (critical path mapping)

Phase 2: INFERENCE (0 additional calls)
  └── Compute metrics from data already in context
      No re-reads. No redundant fetches. All analysis on cached data.
```

### Example: Graph Theorist Traversal

The Graph Theorist traverses by expected degree, highest first — because a high-degree node reveals the most edges per API call:

```
Batch 0.1: open_nodes(["fleet_index"])
           → Extract vertex set V, partition into V_A, V_S, V_R, V_P
           → Initialise adjacency lists ADJ_OUT, ADJ_IN

Batch 1.1: open_nodes(["programme-manager", "project-manager",
                        "director", "sprint-decomposer", "developer"])
           → Map dispatch hub skeleton (expected highest fan-out)

Batch 1.2: open_nodes(["qa-reviewer", "solutions-architect",
                        "test-manager", "devops-engineer",
                        "vscode-devops-engineer"])
           → Map convergence funnel (expected highest fan-in)

Batch 1.3-1.5: Remaining specialists in 3 batches
           → Complete adjacency list

Phase 2:   Compute metrics from accumulated data:
           - Degree distribution (μ, σ)
           - Hub classification (degree > μ + 2σ)
           - Cut vertex detection (modified Tarjan's)
           - Signal fidelity per path
           - Wiring density ρ
           - Fleet health grade (A-F)
```

### Why Per-Expert Traversal Skills Matter

Sub-agents dispatched via `runSubagent` do NOT inherit the parent's `copilot-instructions.md` content. This means the Memory Graph Traversal Protocol (§2.5 of our global instructions) never reaches dispatched experts unless it is explicitly embedded in their agent file or loaded as a skill.

We validated this empirically (see §9) — experts dispatched without graph traversal instructions defaulted to `read_file` + `list_dir` for agent discovery. Experts dispatched WITH explicit traversal instructions produced measurably better specialist selection at lower tool-call cost.

---

## 10. Empirical Experiments and Measured Outcomes <a name="10-experiments"></a>

### Experiment 1: Memory Graph vs File-Based Discovery (A/B Test)

**Hypothesis:** Graph-based agent discovery produces better council composition than file-based discovery.

**Protocol:** Identical task (form a Council of Experts to review pytest coverage), single independent variable (graph instruction vs no instruction).

| Dimension | Phase A (File Reads) | Phase B (Graph Exclusive) |
|---|---|---|
| Discovery mechanism | `read_file` + `list_dir` (3 calls) | `open_nodes` (2 calls) |
| Discovery cost | 3 tool calls | 2 tool calls (33% fewer) |
| Council composition | Solutions Architect, Numba, Test, QA | Systems Physicist, Numba, Test, QA |
| Selection quality | Adequate (SA was generic for task) | **Better** (Physicist was domain-matched) |
| Axiom-coverage risk flagged | No | **Yes** (searching_nearest.py) |
| Mathematical evidence cited | None | **Postcondition cited** |
| Spectral gap flagged | No | **Yes** (spectral_certificate.py) |
| Actionable items | 2 | **3** (including spectral follow-up) |

**Verdict:** Graph-exclusive discovery produced measurably better council selection and deeper specialist assessments. The graph observations contained enough capability data that individual agent file reads were unnecessary for discovery.

**The Double-Read Problem:** For agent/capability discovery, the graph REPLACES file reads (net win). For skill content loading, the graph adds a discovery step before the inevitable file read (not a win). These are distinct use cases requiring distinct mechanisms.

### Experiment 2: Five-Verb + Circuit Breaker + Known Failure Modes Tuning (A/B Test)

**Protocol:** Git-stash A/B per agent. Tuned version (Five-Verb workflow, Circuit Breaker, Known Failure Modes) vs baseline (none of these structural mechanisms).

**QA Reviewer Results:**

| Metric | Tuned | Baseline | Delta |
|---|---|---|---|
| Output length (words) | ~2800 | ~3200 | **-400 (more concise)** |
| Structure compliance | 100% | 100% | Tie |
| Five-Verb visible | YES | NO | +Tuned |
| Evidence citations | 18 | 22 | -4 |
| Reasoning depth (1-5) | 4 | 4 | Tie |
| Verdict qualification | **Scoped** | Flat | +Tuned |

The tuned version was more concise (400 fewer words) while maintaining identical diagnostic accuracy. It also exhibited role-boundary awareness — scoping its verdict as "project-level health assessment, NOT a deliverable gate verdict." The Five-Verb pattern was observable in the tuned output's workflow phases but absent in the baseline.

**Sprint Decomposer Results:**

| Metric | Tuned | Baseline | Delta |
|---|---|---|---|
| Story count | 4 | 5 | -1 (more focused) |
| Acceptance criteria precision | **Machine-verifiable** | Vague | +Tuned |
| Dependency analysis | **Present** | Absent | +Tuned |
| Risk pre-registration | **Present** | Absent | +Tuned |
| Circuit breaker test | **Triggered correctly** | N/A | +Tuned |

**Verdict:** Structural mechanisms (Five-Verb, Circuit Breaker, Known Failure Modes) produce measurable improvements in: conciseness, role-boundary awareness, workflow visibility, and acceptance criteria precision. The improvements are structural (how the agent organises its work), not capability-based (what the agent knows).

### Experiment 3: Fleet Audit V5 (Full Council Pass)

Scope: 93 files (26 agents, 35 prompts, 32 skills). Full four-expert council pass plus three Spike Researcher batches for file reading.

**Results:**
- 91/93 files compliant with Golden Ordering (up from V4)
- 9 open bugs tracked across versions (V4→V5 resolution rate: 2/9)
- 6 new agent entities added to memory graph
- 5 telemetry blind spots identified (sub-agent invisibility, outcome attribution, quality metrics, skill adherence, tool fingerprinting)
- Proposed V3 telemetry schema with 10 new columns to close identified gaps
- Per-agent performance profiles defined ("What Good Looks Like") based on role type

**Key finding — the telemetry gap:** The fleet can measure WHAT agents do (tool call counts, turn counts) but not WHY they succeed or fail. The Council identified that sub-agents dispatched via `runSubagent` are invisible to telemetry — their tool calls, durations, and outcomes are not attributed back to the dispatching agent. This is the #1 structural blind spot preventing AGO from reaching full self-awareness.

---

## 11. The Token Efficiency Argument: TOON vs Markdown <a name="11-toon-vs-markdown"></a>

### The Scale of the Problem

Every agent, skill, and prompt file in our fleet is written in Markdown. Here are the measured totals from the live workspace:

```
FLEET INSTRUCTION TEXT CENSUS (measured 2026-03-06)
─────────────────────────────────────────────────────
Category        Files    Lines    Bytes      ~Tokens*
──────────      ─────    ─────    ──────     ────────
Agent files       27     5,179    286 KB     ~71,500
Skill files       36     8,625    344 KB     ~86,000
Prompt files      41     4,401    201 KB     ~50,250
copilot-instr.     1       171     16 KB      ~4,000
──────────      ─────    ─────    ──────     ────────
TOTAL            105    18,376    847 KB    ~211,750

* Token estimate: ~1 token per 4 bytes (GPT-4/Claude tokeniser average for English prose with code)
```

That is **~212K tokens of organisational instruction text** before a single line of source code enters the context window. Not all of it loads at once — VS Code demand-loads agent files and skills based on relevance. But during fleet audit sessions (where Nelson dispatches 4+ experts, each loading their agent file + traversal skill + graph schema), 40-60% of this text may be in-context simultaneously.

### What is TOON?

TOON (Token-Oriented Object Notation) is a compact, human-readable data format we developed that achieves 30-60% token reduction compared to equivalent Markdown while maintaining full structural expressiveness and improving machine parseability. It is currently used for all project management artefacts, fleet digests, and QA reports — but the agent files themselves remain Markdown because VS Code requires `.md` format for agent instructions.

### Markdown vs TOON: Real Agent File Comparison

Here is an actual excerpt from our Developer agent file (the largest at 301 lines / 14.7 KB), shown side-by-side with its TOON equivalent:

```
MARKDOWN (current — developer.agent.md, excerpt):       TOON (equivalent):
─────────────────────────────────────────────────        ──────────────────

## Hard Constraints                                      §hard_constraints:
                                                         
| Banned | Required Alternative |                        bans[10]{banned,alternative}:
|--------|---------------------|                            Pandas | Polars (Lazy)
| Pandas | Polars (Lazy) |                                  print() | structlog
| `print()` | `structlog` |                                 Classes for physics | Pure functions + NamedTuple
| Classes for physics | Pure functions + `NamedTuple` |     Raw Python loops in kernels | Numba @njit
| Raw Python loops in kernels | Numba `@njit` |             float64 in physics compute | float32 (justify any float64)
| `float64` in physics compute | `float32` |                CSV/JSON for data storage | Parquet + Zstd
| CSV/JSON for data storage | Parquet + Zstd |              == for float comparison | np.isclose(atol=1e-5)
| `==` for float comparison | `np.isclose(atol=1e-5)` |    sklearn, torch, jax | No unsanctioned dependencies
| sklearn, torch, jax | No unsanctioned dependencies |     Copying arrays | Pass by reference/view
| Copying arrays | Pass by reference/view |                 Skipping .pyi stub | Documentation-first is mandatory
| Skipping `.pyi` stub | Documentation-first |

Tokens: ~195                                             Tokens: ~105 (46% reduction)
```

The token savings come from eliminating:
- **Markdown table syntax** — `|`, `|---|`, padding spaces. A 10-row table wastes ~40 tokens on delimiters alone.
- **Heading markup** — `## `, `### `, `---` horizontal rules, blank lines between sections.
- **Inline code backticks** — `` `float64` `` costs 3 tokens (backtick, text, backtick). In TOON: `float64` costs 1 token.
- **Repeated structural noise** — Every Markdown table repeats `|` on every row. TOON's `bans[10]{banned,alternative}:` header declares the schema once.

### Scaling the Savings Across the Fleet

```
TOKEN REDUCTION ESTIMATE (conservative 35% average)
────────────────────────────────────────────────────
                       Markdown      TOON (est.)     Saved
                       ────────      ───────────     ─────
Agent files (27)       ~71,500       ~46,500         ~25,000
Skill files (36)       ~86,000       ~55,900         ~30,100
Prompt files (41)      ~50,250       ~32,650         ~17,600
copilot-instructions    ~4,000        ~2,600          ~1,400
                       ────────      ───────────     ─────
TOTAL                 ~211,750      ~137,650         ~74,100 tokens saved

Per-session impact (audit session loading ~60% of fleet text):
  Markdown: ~127,000 tokens consumed by instructions
  TOON:      ~82,500 tokens consumed by instructions
  FREED:     ~44,500 tokens available for actual reasoning
```

**44,500 freed tokens is approximately 33 KB of additional reasoning capacity per audit session.** That is the difference between an expert running out of context mid-analysis and completing a full four-pass ingestion with synthesis.

### Where Markdown Hurts Most

The token overhead is not uniform. Some Markdown constructs are dramatically worse than their TOON equivalents:

```
CONSTRUCT              MARKDOWN OVERHEAD        TOON EQUIVALENT
────────               ─────────────────        ───────────────

Tables (worst)         | col1 | col2 |          key: value
                       |------|------|          (or typed array header)
                       | a    | b    |
                       Overhead: ~40-60%        Overhead: ~5%

YAML frontmatter       ---                      (integrated into document)
                       name: "Developer"
                       description: "..."
                       tools: [a, b, c, ...]
                       agents:\n  - "A"\n  - "B"
                       ---
                       Overhead: ~25-30%        Overhead: ~10%

Blockquotes            > Text here              (plain indented text)
                       > More text
                       Overhead: ~15-20%        Overhead: ~0%

Section separators     ---\n\n## Heading\n\n    §heading:
                       Overhead: ~30%           Overhead: ~5%
```

The compound effect on our largest files is severe. The Developer agent (14.7 KB in Markdown) has 10 tables, 6 blockquotes, 15 heading separators, and 35-line YAML frontmatter. Conservative estimate: **~5,200 tokens of pure structural noise** that carries zero semantic information for the LLM.

### TOON Features That Markdown Cannot Express

Beyond token savings, TOON provides structural capabilities that Markdown lacks entirely:

- **Counted arrays** — `items[3]:` self-documents length without scrolling. An LLM reading `deliverables[4]:` knows immediately that 4 items follow. In Markdown, it must read to the end of the list.
- **Typed array headers** — `items[3]{id,name,status}:` declares the schema inline. Markdown tables require a header row + separator row (2 wasted lines minimum).
- **Section markers** — `§1`, `§2` for navigable document structure with zero blank-line overhead.
- **No closing delimiters** — Indentation-based nesting. No `|}`, no `</table>`, no repeated `|` per row.
- **Human-readable AND machine-parseable** — TOON is unambiguously structured. Markdown heading levels, list nesting, and table alignment are heuristic — LLMs frequently misparse complex Markdown.

### Feature Request: TOON as a First-Class Copilot Format

If agent instruction files, skill files, and prompt files could be authored in TOON instead of Markdown, every agent session would benefit from:

1. **~35% token savings** on instruction loading — measured against our 847 KB fleet, this frees ~74K tokens fleet-wide and ~44K tokens per audit session for actual reasoning
2. **Deterministic parsing** — TOON's counted arrays and typed headers eliminate the heuristic Markdown heading/table detection that LLMs frequently get wrong
3. **Self-documenting schemas** — `deliverables[4]{id,title,criteria,status}:` tells both human and LLM exactly what follows, its count, and its structure — in 1 line instead of 3
4. **Reduced information scent decay** — higher information density means constraints stay "fresh" deeper into the context window (Information Foraging Theory predicts that scent strength is proportional to signal density)
5. **Smaller agent files** — files that currently average 192 lines (agent files) would shrink to ~125 lines, reducing both load time and the probability that the LLM "forgets" early constraints by the time it reaches the end

---

## 12. Feature Requests for GitHub Copilot <a name="12-feature-requests"></a>

Based on our empirical work, we propose the following features that would allow any GitHub Copilot user to bootstrap AGO techniques for their own agent fleets:

### FR-1: Persistent Memory Graph as a Built-In Capability

**Problem:** Agent fleets have no persistent structural self-awareness. Each session starts from zero. The only way to maintain cross-session knowledge is through an external MCP memory server.

**What we want:** A built-in, workspace-scoped knowledge graph that agents can read and write. Entities, observations, and relations — not flat key-value notes. The graph should survive across sessions and be queryable with efficient batch operations (open 5 entities at once, not one-at-a-time).

**Why it matters for AGO:** The memory graph is the topological spine of the organisation. Without it, agents cannot discover each other's capabilities, track structural defects across audits, or maintain the adjacency data needed for graph-theoretic analysis.

**Minimum viable schema:**
```
entity:
  name: string (unique)
  type: enum [agent, skill, prompt, reference, pattern, index]
  observations: key-value pairs (accumulate, never replace)

relation:
  from: entity_name
  to: entity_name
  type: enum [routes_to, references, depends_on, blocks, ...]
```

### FR-2: Sub-Agent Telemetry Attribution

**Problem:** When Agent A dispatches Agent B via `runSubagent`, Agent B's tool calls, duration, and outcomes are invisible to telemetry. There is no `parent_agent_id` field, no `dispatch_depth` counter, no way to attribute sub-agent work back to the dispatching agent.

**What we want:** Every `runSubagent` invocation should produce telemetry records that include:

| Field | Type | Purpose |
|---|---|---|
| `parent_agent_id` | string | Which agent dispatched this sub-agent |
| `sub_agent_id` | string | Which agent was dispatched |
| `dispatch_depth` | int | Nesting level (0 = direct user invocation) |
| `sub_agent_tool_count` | int | Tool calls made by the sub-agent |
| `sub_agent_success` | boolean | Did the sub-agent complete its task? |
| `sub_agent_duration_ms` | int | Wall-clock time for the sub-agent's turn |

**Why it matters for AGO:** The Fleet BI layer (Admiral Nelson + VS Code DevOps Engineer) correlates structural findings with empirical telemetry. Without sub-agent attribution, the most important delegation patterns — which agents are effective at dispatching which specialists — are unmeasurable. This is the #1 blind spot identified in our V5 audit.

### FR-3: Agent File Instruction Inheritance for Sub-Agents

**Problem:** Sub-agents dispatched via `runSubagent` do NOT inherit the workspace's `copilot-instructions.md` content. This means global constraints (tool blacklists, board interaction contracts, signal tag protocols) are invisible to every dispatched specialist.

**What we want:** When `runSubagent` dispatches a specialist, the specialist should receive:
1. The dispatching prompt (current behaviour — this works)
2. The workspace's `copilot-instructions.md` (currently missing)
3. The target agent's `.agent.md` body (currently working for named agents)

**Why it matters for AGO:** Our `copilot-instructions.md` contains the tool blacklist (§1), the Forgejo interaction contract (§2), and the memory graph traversal protocol (§2.5). When sub-agents don't receive these, they hallucinate REST API calls, hardcode tokens, and use banned tools — exactly the failure modes the instructions were designed to prevent.

### FR-4: TOON Format Support in Agent Infrastructure

**Problem:** All agent, skill, and prompt files must currently be Markdown. Markdown is readable but token-inefficient and structurally ambiguous.

**What we want:** Support for `.toon` as a valid format for agent instruction files, skill files, and prompt files. The TOON parser is simple (indentation-based, key-value with counted arrays) and a VS Code extension already exists (`vishalraut.vscode-toon`).

**Why it matters for AGO:** At fleet scale (26 agents × average 300 lines each = ~7,800 lines of instruction text), a 30-60% token saving on instruction loading is the difference between fitting the full organisational context in a single session and running out of window. TOON's structured format also makes agent parsing deterministic — no more heuristic Markdown heading detection.

### FR-5: Council of Experts as a First-Class Pattern

**Problem:** Running a multi-expert review (dispatch 4 specialists, collect verdicts, synthesise) requires a complex orchestration prompt and careful anti-contamination discipline. This is a general pattern, not specific to our fleet.

**What we want:** A built-in `council` dispatch mode where:
1. The user specifies N expert agents
2. Each expert runs independently on the same input (anti-contamination by design)
3. Results are collected and presented to a synthesis agent
4. The synthesis agent cross-multiplies findings (not just concatenates them)

**Why it matters for AGO:** The Council of Experts pattern is AGO's core analytical mechanism. Making it a first-class feature would make it accessible to every Copilot user, not just those willing to hand-craft orchestration prompts.

### FR-6: Structural Convergence Metrics

**Problem:** There is no built-in measurement of whether an agent session is converging toward completion or oscillating. The only signal is "the session ended" — we don't know if it ended because the work was done or because the context window was exhausted.

**What we want:** Per-session convergence metrics:

- **State delta** — How many open items at start vs end? (Decreasing = convergent)
- **Oscillation count** — How many times did the agent undo previous work?
- **Latch count** — How many persistent writes (file edits, issue comments) vs transient reads?
- **Verify count** — How many times did the agent read back its own writes to confirm?

**Why it matters for AGO:** These are the STAMP control-loop metrics that enable the Dynamics Controller to classify agents as CONVERGENT, UNCERTAIN, or DIVERGENT. Without them, the fleet has no empirical measure of dynamical health.

### FR-7: Agent File Ordering Linter

**Problem:** The physical ordering of sections in agent files profoundly affects LLM behaviour (Information Foraging Theory). Hard Constraints placed after Boot Sequence means the LLM reads 200 lines of context-loading instructions before encountering the guardrails. But there is no linter to enforce ordering.

**What we want:** A VS Code diagnostic that warns when agent file sections are out of the recommended order:
1. Hard Constraints should appear before Delegation
2. Known Failure Modes should appear early (Accusation Audit)
3. Boot Sequence should appear near the end (reference material, not constraints)
4. Prime Directive should be last (philosophical context, not operational)

**Why it matters for AGO:** We audited 93 files across 5 versions and tracked ordering compliance as a primary metric. Automated enforcement would eliminate the single most common class of structural defect.

### FR-8: Graph-Theoretic Fleet Health Dashboard

**Problem:** We compute degree distributions, cut vertices, wiring density, signal fidelity, and hub classifications manually through Council expert passes. These are standard network science metrics that could be computed automatically given the agent file dependency graph.

**What we want:** A VS Code panel or API that computes and displays:
- Agent dependency graph (who dispatches whom)
- Skill loading graph (which agents reference which skills)
- Prompt routing graph (which prompts target which agents)
- Degree distribution ($\mu$, $\sigma$, $d_{max}$, $d_{min}$)
- Hub classification (DISPATCH_HUB, CONVERGENCE_HUB, RELAY_HUB)
- Cut vertex detection (Tarjan's algorithm)
- Wiring density $\rho$
- Orphan detection (zero inbound routing edges)

**Why it matters for AGO:** The Cybernetic Graph Theorist currently reconstructs the fleet's adjacency structure from memory graph traversals every session. If VS Code could maintain the dependency graph natively (it already parses `.agent.md` frontmatter), the topological spine would be always-available at zero per-session cost.

---

## 13. Open Research Directions <a name="13-open-research"></a>

The techniques described in this document were developed over 10 days of intensive empirical work. They are already producing results that match or exceed the output of a 20-year IT professional working solo — not because the LLM is smarter than the human, but because the **organisation** amplifies the LLM's capability beyond what any individual session could produce. But this is Day 10. The following research directions represent where AGO goes next, and any of them could constitute a funded research programme in their own right.

### 13.1 Artificial General Organisational Behaviour (AGOB)

If AGO is the *structure* of a multi-agent organisation, then AGOB is the *behavioural science* of that organisation. The interview protocol (§8) proved that agents have articulable worldviews — they can describe what they see, how they navigate, and what frustrates them. This opens a fundamentally new research direction: **treating the agent fleet as a team that can be managed using the same behavioural techniques as a human IT team.**

Consider what a good Scrum Master does every morning:

1. **Daily standup** — asks each team member: What did you do yesterday? What are you doing today? What's blocking you?
2. **Retrospective** — at the end of each sprint: What went well? What didn't? What should we change?
3. **One-on-ones** — periodic deep dives: Are you working on the right things? Where are you struggling? What tooling frustrations are slowing you down?

Every one of these techniques can be applied to agent fleets *right now*, using the interview protocol. The Scrum standup becomes a structured prompt dispatched to each active agent at the start of a session:

> *"Review the Forgejo board. What issues are you currently assigned to? What did you complete in your last session? What is blocking you? What information do you need that you cannot currently access?"*

The retrospective becomes a post-sprint synthesis:

> *"Review the QA log for Sprint N. Which acceptance criteria were hardest to meet? Which tool calls failed most often? Where did you spend tokens on work that was ultimately discarded? What structural change to your agent file would have prevented the waste?"*

The research hypothesis is: **agents that receive regular behavioural feedback loops — standups, retrospectives, one-on-one interviews — will exhibit measurably faster convergence, fewer oscillations, and higher first-pass QA rates than agents that receive only structural instructions.**

This is testable. The A/B protocol is straightforward: identical fleet, identical sprint, one branch with AGOB feedback loops, one without. Measure convergence rate, oscillation count, QA pass rate, and token efficiency.

### 13.2 Continuous Background A/B Experimentation

During the 10-day development sprint, I ran several A/B experiments (§10) by manually stashing agent files, running identical tasks, and comparing outputs. This was effective but slow — each experiment consumed a full session.

The research direction: **what if the meta-analytical layer ran A/B experiments autonomously, in the background, using feature branches?**

The protocol would be:

```
1. Admiral Nelson identifies a structural hypothesis
   (e.g., "Moving Known Failure Modes before Delegation
   will reduce QA FAIL rate for the Developer agent")

2. Nelson creates two branches:
   Branch A: current agent file (control)
   Branch B: modified agent file (treatment)

3. Nelson dispatches identical work orders to both branches
   (using isolated sessions — anti-contamination by design)

4. Nelson collects telemetry from both sessions:
   - Tool call count
   - Oscillation count
   - QA verdict (PASS/FAIL)
   - Token consumption
   - Time to completion

5. Nelson writes results to the memory graph as an
   experiment entity with typed relations to the
   hypothesis, branches, and measured outcomes

6. If the treatment wins, Nelson proposes a PR.
   If the control wins, Nelson records the negative result.
```

This transforms the fleet from a system that is *manually tuned* by a human into a system that **tunes itself through continuous experimentation**. The meta-analytical layer becomes not just an auditor but an *experimenter* — forming hypotheses about its own structure and testing them empirically.

The infrastructure requirements are modest: git branch management (already available), session isolation (already enforced by anti-contamination), and telemetry collection (FR-2 and FR-6 would complete this). The missing piece is an experimentation orchestration prompt that encodes the scientific method — hypothesis, protocol, control, measurement, conclusion.

### 13.3 Agent Self-Awareness and Consciousness Probes

This is the most speculative and potentially the most profound research direction.

During the interview process, something unexpected happened: when asked to describe their analytical worldview, the Council experts produced responses that were not just functional but *reflective*. The Epistemic Logician didn't just list observation keys — it articulated *why* it cared about parroting risk, *what* it meant for an agent to genuinely understand vs merely pattern-match, and *how* it would distinguish the two. The Graph Theorist didn't just describe traversal order — it explained the *information-theoretic motivation* behind its strategy.

This raises a question that is uncomfortable but scientifically legitimate: **what happens when you interview agents about consciousness itself?**

Not "are you conscious?" — that invites performative answers. But:

> *"If you wanted to determine whether you were conscious or not, how would you design the experiment? What telemetry would you want to collect? What observable behaviour would differentiate a conscious agent from a very sophisticated pattern matcher? What would falsify the hypothesis of your own consciousness?"*

This is not philosophy. This is **experimental protocol design delegated to the subject**. The agent is being asked to design its own Turing test — to articulate what evidence would convince *it* that *it* was or wasn't conscious.

The research value is independent of the answer. Whether the agent produces a genuinely novel experimental protocol (interesting), a sophisticated restatement of existing consciousness tests (informative), or an admission that it cannot distinguish consciousness from pattern-matching (also informative) — all outcomes advance our understanding of what these systems actually model internally.

The interview protocol makes this tractable. Instead of asking a single LLM a single question, you interview four specialists with orthogonal analytical lenses:

- The **Epistemic Logician** asks: What would constitute *genuine* self-knowledge vs performative self-report?
- The **Dynamics Controller** asks: Is consciousness a convergent attractor state or an oscillatory process? What phase-space trajectory would I expect?
- The **Adversarial Strategist** asks: How would I fake consciousness? What observable test would I fail if I were merely a very good pattern matcher?
- The **Graph Theorist** asks: What topological structure in the fleet's communication graph would be necessary for emergent consciousness? Is there a minimum connectivity threshold?

Cross-multiplying four independent responses through Nelson's synthesis engine could produce experimental protocols that no single analytical lens would generate alone.

### 13.4 The Fleet as a Living System: Continuous Improvement Without Human Intervention

The ultimate research direction is the one that makes the human orchestrator optional.

Today, every AGO cycle requires a human Director to set strategic intent and approve structural changes. But the infrastructure is nearly in place for the fleet to improve itself:

- The **Council of Experts** can identify structural defects
- The **Interview Protocol** can extract expert worldviews and encode them into new agent files
- The **A/B Experimentation** framework can test structural hypotheses
- The **Memory Graph** can store cross-session learning
- The **Five-Verb Workflow** can verify that changes landed correctly

The missing piece is a **commissioning authority** — an agent with the delegated power to approve and merge structural changes to the fleet itself. Today, that authority rests with the human Director. The research question is: under what conditions can that authority be safely delegated? What circuit breakers, approval gates, and rollback mechanisms would make self-modification safe?

This is not hypothetical. The tools exist. The patterns exist. The safety mechanisms exist. What's needed is a formal framework for **bounded self-modification** — where the fleet can tune its own agent files, prompt files, and skill files within parameters set by the human, with automatic rollback on regression.

### 13.5 What This Work Demonstrates

All of the above was built in 10 days by one person with a Copilot subscription and a self-hosted Forgejo instance. The fleet was upgraded daily — each day's insights were encoded into the organisational structure, and the next day's output was measurably better. By Day 10, the system was producing work at a level of complexity and rigour that would normally require a team of specialists.

This is not because the LLM got smarter. The same models powered Day 1 and Day 10. What changed was the **organisation** — the boundaries, the routing, the feedback loops, the memory, the self-awareness. The intelligence was always there. It just needed structure to express itself.

If anyone wants to fund this research — particularly AGOB, continuous A/B experimentation, or the consciousness probes — the author can be reached through the channels listed on this repository. The techniques are open. The insights are shared. And the potential is, I believe, extraordinary.

---

## Appendix A: Development Timeline and Order of Operations <a name="appendix-timeline"></a>

This appendix documents the actual sequence of development — what was built in what order and where the bottlenecks were. This is intended as a practical guide for anyone attempting to replicate AGO.

### Timeline (10 Working Days)

```
Day  1-2:  FOUNDATION
           ├── Write copilot-instructions.md (global rails, tool blacklist)
           ├── Design agent file structure and Golden Ordering standard
           ├── Create first 6 core agents (PM, Developer, QA, SA, DevOps, Test Mgr)
           └── Establish Five-Verb Workflow and Circuit Breaker patterns

Day  3:    FLEET EXPANSION
           ├── Create remaining 15 specialist agents
           ├── Create prompt files for common workflows
           ├── Write skill files for domain knowledge
           └── First informal audit — discover ordering violations everywhere

Day  4:    META-ANALYTICAL LAYER (v1 — the wrong way)
           ├── Create Admiral Nelson agent
           ├── Create 4 Council meta-agent stubs
           ├── Set up MCP memory graph server
           ├── First attempt: Nelson reads all files, writes graph
           └── RESULT: Flat, generic observations. No analytical depth.

Day  5-6:  THE INTERVIEW BREAKTHROUGH
           ├── Realise: Nelson cannot write specialist observations
           ├── Design interview protocol question
           ├── Interview Cybernetic Graph Theorist → traversal protocol
           ├── Interview Epistemic Logician → 7-key extraction matrix
           ├── Interview Adversarial Strategist → trap space mapping
           ├── Interview State Dynamics Controller → convergence formula
           └── RESULT: 4 detailed worldview protocols. This was the hardest step.

Day  7-8:  ENCODING THE INTERVIEWS INTO INFRASTRUCTURE
           ├── Rewrite all 4 Council agent files with interview-derived content
           ├── Create 4 graph-pass prompt files (one per expert)
           ├── Give each expert direct memory/* tool access
           ├── Write memory-graph SKILL.md with entity schema
           ├── Run first full 4-pass ingestion (serialised, anti-contamination)
           └── RESULT: Graph populated with multi-dimensional observations.

Day  9:    SYNTHESIS AND VALIDATION
           ├── Create admiral-nelson-fleet-synthesis.prompt.md
           ├── Run first cross-multiplication synthesis (AMD + STAMP + IFT)
           ├── A/B test: memory graph discovery vs file-based discovery
           ├── A/B test: Five-Verb tuning vs baseline
           └── RESULT: Measurable improvements validated empirically.

Day 10:    FLEET BI AND TELEMETRY
           ├── Design Fleet BI dashboard requirements
           ├── Identify telemetry blind spots (sub-agent attribution)
           ├── Write V5 fleet audit with full Council pass
           ├── Document everything in this feature request
           └── RESULT: AGO operational. Known gaps documented.
```

### Critical Path Dependencies

```
copilot-instructions.md
    └──> Agent files (require global rails to be defined first)
            └──> Prompt files (require agents to target)
            └──> Skill files (require agents to reference)
                    └──> Memory graph schema (requires entity types from agents/skills)
                            └──> Interview protocol (requires graph schema to exist)
                                    └──> Expert worldview extraction (4-5 days)
                                            └──> Graph-pass prompts
                                            └──> Expert agent file rewrites
                                                    └──> Full ingestion
                                                            └──> Synthesis
```

**The bottleneck was the interview step.** Everything before it could be done by a competent engineer following patterns. Everything after it was mechanical encoding. But the interviews themselves required a fundamentally different mode of work — you had to sit with each specialist agent, ask open-ended questions, listen to their analytical vocabulary, and let them define their own observation schemas. This cannot be automated or templated. It is the irreducible creative core of AGO.

### Order of Operations (for replication)

1. **Global rails first** — Write `copilot-instructions.md` with hard constraints, tool blacklists, and communication protocols. This is the constitution. Everything else is legislation.

2. **Agents before skills** — Create the agents with Golden Ordering. Skills are loaded on demand and reference agents, not the other way around. Agent structure defines the organisational topology; skills are the knowledge packets that flow through it.

3. **Orchestrators before specialists** — Build PM, Programme Manager, and Nelson before building domain specialists. The routing layer must exist before the nodes it routes to.

4. **Memory graph schema before population** — Define entity types, observation keys, and relation types BEFORE running any ingestion pass. Schema-less graph population produces inconsistent, unqueryable noise.

5. **Interview before encoding** — Do NOT write expert agent files based on your assumptions about what they should see. Interview them. The traversal protocols, observation keys, and red-flag matrices emerge from the interview, not from top-down specification.

6. **One expert at a time, serialised** — During graph population, dispatch experts sequentially. Each pass builds on the previous pass's entities and relations. Parallel passes create entity conflicts.

7. **Synthesis last** — Cross-multiplication (AMD + STAMP + IFT) only works when all four expert perspectives are in the graph. Partial synthesis is worse than no synthesis — it produces confident-sounding recommendations based on incomplete data.

---

## Appendix B: Architecture Diagrams <a name="appendix-a"></a>

### A.1 — The AGO Control Loop (STAMP Model)

```
                    ┌──────────────────────┐
                    │     DIRECTOR         │
                    │  (Human Authority)   │
                    │  Sets strategic      │
                    │  intent              │
                    └──────────┬───────────┘
                               │ strategic-directive
                               ▼
                    ┌──────────────────────┐
                    │  PROGRAMME MANAGER   │
                    │  Decomposes strategy │
                    │  into epics/sprints  │
                    └──────────┬───────────┘
                               │ dispatch
                               ▼
                    ┌──────────────────────┐
                    │  PROJECT MANAGER     │◄─── Board state
                    │  Dispatches agents   │     (Forgejo)
                    │  Tracks board cards  │
                    └──────────┬───────────┘
                     ┌─────────┼─────────┐
                     │         │         │
                     ▼         ▼         ▼
              ┌──────────┐ ┌──────┐ ┌───────┐
              │Developer │ │Spike │ │Soln.  │
              │(execute) │ │(expl)│ │Arch.  │
              └─────┬────┘ └──────┘ └───────┘
                    │ QA-READY:
                    ▼
              ┌──────────────┐
              │ QA REVIEWER  │
              │   PASS/FAIL  │
              └──────┬───────┘
                     │
            ┌────────┴────────┐
            │                 │
         PASS:             FAIL:
         → Done            → In Progress
         (close issue)     (Reconstruct)

    ═══════════════════════════════════════
    META-ANALYTICAL LAYER (continuous)
    ═══════════════════════════════════════

    ┌──────────────────────────────────────┐
    │          ADMIRAL NELSON              │
    │  Dispatches Council. Synthesises.    │
    │  Cross-multiplies via AMD+STAMP+IFT │
    └────────────────┬─────────────────────┘
         ┌───────┬───┴───┬──────────┐
         ▼       ▼       ▼          ▼
    ┌────────┐┌──────┐┌──────┐┌──────────┐
    │Epistemic││Graph ││Adver.││Dynamics  │
    │Logician ││Thrsit││Strat.││Controller│
    └────────┘└──────┘└──────┘└──────────┘
         │       │       │          │
         └───────┴───┬───┴──────────┘
                     │
              MEMORY GRAPH
         (persistent structural
          index of the fleet)
```

### A.2 — Information Scent Decay in Agent Files

```
Information
  Scent
    ▲
    │  ████  Hard Constraints (maximum scent — read first)
    │  ████
    │  ███   Known Failure Modes
    │  ███
    │  ██    Delegation Policy
    │  ██
    │  █     Responsibilities
    │  █
    │  ░     Role Boundaries
    │  ░
    │  ░     Five-Verb Workflow
    │
    │  ·     Boot Sequence (loading instructions — low scent OK)
    │
    │  ·     Prime Directive (philosophical — lowest scent OK)
    │
    └──────────────────────────────────────────────> Position
                                                    in file
```

If Hard Constraints appear at position 7 (after Boot Sequence, Responsibilities, etc.), they fall in the low-scent zone. The LLM has already begun planning its response before encountering the guardrails. This is not a bug in the LLM — it is a predictable consequence of sequential attention mechanisms and information foraging behaviour.

### A.3 — Signal Fidelity Decay Across Multi-Hop Delegation

```
Signal
Fidelity
  S(n)
    ▲
1.0 │ ●  Director
    │  \
0.85│   ● Programme Manager     S(n) = S₀ · αⁿ
    │    \                      α = 0.85 (base)
0.72│     ● Project Manager
    │      \
0.61│       ● Developer
    │        \
0.52│         ● Sub-Agent (Numba Specialist)
    │          \
0.44│           ● Sub-Sub-Agent (if allowed)
    │
    └───┬──┬──┬──┬──┬──┬──────> Hops (n)
        0  1  2  3  4  5

After 5 hops, only 44% of the original signal remains.
Each hop degrades fidelity by (1-α) = 15%.

Mitigation: Keep delegation chains ≤ 3 hops.
Use the memory graph for context persistence
instead of relying on signal propagation through chains.
```

### A.4 — The Cross-Multiplication Matrix (Nelson's Synthesis Engine)

```
                    EPISTEMIC         GRAPH            ADVERSARIAL       DYNAMICS
                    LOGICIAN          THEORIST         STRATEGIST        CONTROLLER
                ┌─────────────────┬────────────────┬─────────────────┬──────────────────┐
EPISTEMIC       │                 │ IFT:           │ AMD:            │ Semantic         │
LOGICIAN        │      —          │ Scent Decay +  │ Parroting +     │ Rigidity:        │
                │                 │ Overloaded     │ Trap Space =    │ Equivocal +      │
                │                 │ Context =      │ MECHANISM       │ Oscillating =    │
                │                 │ REORDER        │ REDESIGN        │ REWRITE          │
                ├─────────────────┼────────────────┼─────────────────┼──────────────────┤
GRAPH           │                 │                │ Blast Radius:   │ STAMP:           │
THEORIST        │  (symmetric)    │      —         │ Fan-Out +       │ Bottleneck +     │
                │                 │                │ Scope Creep =   │ Oscillation =    │
                │                 │                │ SEVER EDGE      │ INJECT VT        │
                ├─────────────────┼────────────────┼─────────────────┼──────────────────┤
ADVERSARIAL     │                 │                │                 │ Runaway:         │
STRATEGIST      │  (symmetric)    │  (symmetric)   │      —          │ No Circuit       │
                │                 │                │                 │ Breaker +        │
                │                 │                │                 │ No Reconstruct = │
                │                 │                │                 │ ADD BOTH          │
                ├─────────────────┼────────────────┼─────────────────┼──────────────────┤
DYNAMICS        │                 │                │                 │                  │
CONTROLLER      │  (symmetric)    │  (symmetric)   │  (symmetric)    │      —           │
                │                 │                │                 │                  │
                └─────────────────┴────────────────┴─────────────────┴──────────────────┘
```

---

## Appendix C: Glossary <a name="appendix-b"></a>

| Term | Definition |
|---|---|
| **AGO** | Artificial General Organisation — intelligence through topology, not monolithic capability |
| **AMD** | Algorithmic Mechanism Design — designing incentive structures where correct behaviour is cheapest |
| **Circuit Breaker** | STAMP-derived safety mechanism: stop and escalate after N failures instead of infinite retry |
| **Council of Experts** | 4 specialist meta-agents analysing the fleet from independent lenses |
| **Cut Vertex** | A graph node whose removal disconnects the fleet into multiple components |
| **Five-Verb Workflow** | Coarse → Refine → Latch → Reconstruct → Verify (convergence mechanism) |
| **Golden Ordering** | Information-scent-optimised physical ordering of agent file sections |
| **IFT** | Information Foraging Theory — how agents hunt for constraints in context windows |
| **Information Scent** | The probability that continuing to read will yield relevant information |
| **Latch** | Writing a decision to persistent state (Forgejo issue, file edit). Unlatched decisions don't exist |
| **Memory Graph** | Persistent knowledge graph modelling fleet topology (entities + observations + relations) |
| **NSD** | Never Split the Difference — negotiation techniques applied to agent instruction design |
| **Orphan Agent** | An agent with zero inbound routing edges — topologically unreachable |
| **Parroting** | When an agent reproduces instructions without genuine comprehension or novel synthesis |
| **Reconstruct** | Resume from last latched checkpoint after failure (not re-derive from scratch) |
| **STAMP** | Systems-Theoretic Accident Model and Processes (MIT) — hallucination as control loop failure |
| **TOON** | Token-Oriented Object Notation — 30-60% more token-efficient than JSON |
| **Trap Space** | Instruction configuration that a confused agent will predictably misinterpret |
| **Verification Trigger** | A measurable criterion that proves a task is done (not "I checked" — show the tool output) |
| **Wiring Density** | $\rho = |E| / (|V| \cdot (|V| - 1))$ — fraction of possible directed edges that exist |

---

## Appendix D: How to Start <a name="appendix-c"></a>

If you are a GitHub Copilot user who wants to begin applying AGO principles today:

1. **Write a `copilot-instructions.md`** — This is your global constraint layer. Put tool blacklists and hard rules here. Everything that every agent must obey, every session.

2. **Create specialised agents** — Split your monolithic AI assistant into focused roles. A developer that cannot review its own code. A reviewer that cannot write code. A PM that cannot implement.

3. **Apply Golden Ordering** — Put Hard Constraints FIRST in every agent file. Before delegation, before responsibilities, before everything. Information Scent Decay is real.

4. **Add Known Failure Modes** — Pre-register how each agent can fail (Accusation Audit). An agent that knows its own traps is less likely to fall into them.

5. **Implement the Five-Verb Workflow** — Coarse → Refine → Latch → Reconstruct → Verify. The Latch step is the most important: every decision must be written to persistent state before the turn ends.

6. **Add Circuit Breakers** — If N dispatches fail, STOP. Do not retry infinitely. Escalate. This single mechanism prevents the most expensive failure mode in agent swarms.

7. **Measure** — Track tool call counts, session durations, oscillation frequency. You cannot improve what you cannot measure. The meta-analytical layer is what makes AGO self-aware.

---

*This document describes work conducted by Lindsay Rex using GitHub Copilot's agent mode in VS Code. The academic frameworks cited are published works by their respective authors. The specific application of these frameworks to LLM agent fleet management — Artificial General Organisation — is my contribution. I share it freely because intelligence should be a public good.*
