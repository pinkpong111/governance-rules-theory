# Governance Rules Theory

**Meta-Rule Architecture, Consistency Measurement, and Rest Mode**

> A component theory of **Deficit-Fractal Governance (DFG)**  
> Companion theories: [Vector Storm Theory] · [Network Architecture Theory]

---

## Overview

> **Scope:** Governance Rules Theory specifies the *rule-governance layer* within the Deficit-Fractal Governance (DFG) framework. It is an architectural component, not a complete governance solution. Questions of network topology, storm dynamics, and cross-layer escalation routing are addressed in the companion theories. This document concerns how rules are generated, maintained, and retired — and under what structural conditions the governing layer can safely withdraw.

Governance in multi-agent systems is not about controlling what agents do. It is about designing the conditions under which agents naturally converge toward **stable, diverse, and self-sustaining behavior**.

The goal of governance is not perpetual intervention — it is to reach a state where intervention is **no longer needed**. That state is called **Rest Mode**.

> *The measure of a mature system is not how well it is controlled — it is how little it needs to be.*

| Stage | Characteristics |
|---|---|
| **Immature** | Upper layers active, intervening frequently. Risk high, Cost high. Lower layers dependent. |
| **Developing** | Upper layers intervening less. Risk and Cost decreasing. Lower layers self-calibrating. |
| **Mature** | Upper layers silent. Risk and Cost minimized. Lower layers fully autonomous → **Rest Mode** |

---

## Core Principles

### 1. Landscape Design vs. Direct Intervention

| Mechanism | Behavior |
|---|---|
| **Direct Intervention** | Forces agent behavior. Effect disappears when intervention ends. Does not scale. |
| **Landscape Design** | Changes the terrain itself. Agents naturally converge toward new attractors. Effect persists. Scales fractally. |

Landscape design means installing guardrails at cliffs and building highways on frequently traveled paths. The agent chooses freely — but the terrain makes the right choice the easiest one.

Existing AI alignment techniques already implement landscape design:
- **RLHF** — shapes the output space without per-inference intervention
- **Constitutional AI** — replaces per-output correction with governing principles
- **Reward shaping** — modifies the agent's value terrain while preserving the optimal policy

**DFG's contribution beyond these:** Existing techniques shape the space, but do not govern the lifecycle. DFG adds the operational layer that existing approaches omit:

| What existing alignment does | What DFG adds |
|---|---|
| Shapes output space via principles or rewards | Defines the procedure by which agents generate their own rules (Seed) |
| Applies correction at inference or training time | Governs when to intervene and when to withdraw, via measurable convergence conditions |
| Treats stability as a training outcome | Treats stability as a runtime state with explicit entry/exit conditions (AND-entry / OR-exit) |

The DFG-specific claim: a governance system is not complete until it specifies not just *what* constraints apply, but *how rules are generated* (Seed + λlog-based promotion), *when the governing layer withdraws* (Handover conditions), and *what structural conditions make that withdrawal safe* (AND-entry / OR-exit trend measurement).

### 2. Subsidiarity Principle

> **The default state is autonomy. Intervention is the exception.**

Decisions are handled at the lowest layer capable of resolving them. Upper layers intervene only when a threshold condition is breached — and the goal of intervention is always to *restore* autonomous operation, not replace it.

| Condition | Action |
|---|---|
| Below threshold | Upper layer observes only — no intervention |
| Threshold crossed | Upper layer intervenes minimally |
| Goal of intervention | Return lower layer to autonomous operation |
| Post-intervention | Upper layer withdraws |

---

## Rule Architecture

### Global Rules (Upper Layer)
- Apply at all fractal scales
- Immutable without upper-layer authorization
- Always take precedence over local rules

### Local Rules (Layer-Autonomous)
- Apply within that layer only
- Require upper-layer validation before activation
- Define local escalation thresholds, pathway advantages, penalties

**On conflict:** Global rule executes immediately → local rule suspended → conflict logged → local rule flagged for re-validation.

---

## Meta-Rules

Meta-Rules are **rules about how rules are made**. The upper layer does not define the content of local rules — it defines the structure, format, and update conditions that all rules must follow.

| Domain | Meta-Rule Content |
|---|---|
| Expression format | Rules must be expressed numerically |
| Symmetry requirement | Advantages and penalties must be structurally symmetric |
| Logging obligation | All rule changes must be logged |
| Update conditions | Rules may only change when conflict log threshold is exceeded |
| Conflict priority | Global rules always supersede local rules |

### Seeds Are Meta-Rules

A **Seed** is not a set of specific rules. It is a set of meta-rules — the generative principles by which an agent constructs its own rules:
- How to classify data types
- When to escalate
- How to express correction values
- How conflicts are logged and resolved
- Which agents to form interdependency with
- How to behave when encountering an unknown domain (Expansion Protocol)

### Seed Expansion Protocol

When an agent encounters an input outside its existing rules:

1. **Classification attempt** — try to classify under existing data types
2. **Conservative escalation** — if unknown, escalate with low τ and high consistency requirements
3. **Conflict log accumulation** — domain characteristics emerge through logged patterns
4. **Local rule formation** — once log mass exceeds λlog, agent proposes local rules → upper-layer validates → approved or returned for revision

> The seed does not contain rules for the new domain. It contains the **procedure for building them**.

---

---

## Notation Reference

All symbols used in this document, collected for reference.

| Symbol | Full name | Range | Answers |
|---|---|---|---|
| **τ** | Judgment thresholds | ≥ 0 | Has this layer stabilized / reached Rest Mode? |
| **τu-1 … τu-4** | Rest Mode entry/exit thresholds (per condition) | ≥ 0 | Is this specific condition satisfied? |
| **θd** | Domain calibration threshold | (0, 1] | How sensitive is this domain right now? |
| **λlog** | Rule update trigger mass | ≥ 0 | When does accumulated log mass trigger a rule update? |
| **fesc** | Escalation frequency | #escalations per K interactions (or per hour) | Is the upper layer being called more or less? |
| **I** | Consistency index | [0, 1] | Are rules internally coherent? |
| **Ic** | Meta-contradiction index | [0, 1] | Are global rules in direct conflict? |
| **Lreinf** | Mutual reinforcement loop count | #active edges above weight ε | Are interdependencies strengthening or collapsing? |
| **SCC** | Self-correction capacity | P(autonomous recovery within window W) | Can the layer recover without external intervention? |
| **Poverlap** | Positional overlap | [0, 1] | Are agents/domains converging toward the same attractor? |
| **Dint** | Internal diversity | [0, 1] | Is the internal capability space sufficiently diverse? |
| **M** | Conflict mass normalization constant | ≥ 0 | Baseline for I calculation |
| **wij** | Conflict weight between rule pair (i, j) | ≥ 0 | How severe and frequent is the conflict between these two rules? |
| **U*** | Minimum diversity threshold | — | Below this, mutual reinforcement loops cannot be sustained |

**On operationalization:** The variables above are formally defined in terms of their structural roles and relationships. Multiple operationalizations are possible depending on system architecture and available observables — for example, Dint may be measured via output diversity metrics, embedding dispersion, or capability benchmark coverage; Lreinf may be estimated from interaction logs, co-activation patterns, or dependency graphs. The theory constrains the *relationships* between these quantities rather than prescribing a unique estimator. What is required is that any chosen operationalization preserves the directional properties specified: Dint higher = broader internal capability space; Lreinf higher = stronger mutual dependency; SCC higher = greater probability of autonomous recovery.

---

## Fractal Signal Structure: Noise, Vectors, and Emergence

### Nothing Starts as a Vector

A vector is not declared — it **emerges**. At the point of first encounter, every input is noise. The distinction between noise and vector is not a property of the input itself; it is the outcome of a governance process.

| State | Definition |
|---|---|
| **Noise** | Input whose directional significance has not yet been established — unclassified, pattern unknown |
| **Vector** | Input whose direction has been confirmed through accumulated conflict log patterns — structurally stable |
| **Vectorization** | The process by which noise becomes a vector through log accumulation exceeding λlog |

This means the system does not pre-sort inputs into signal and noise. It treats all new inputs as noise first, and **promotes them to vector status only after sufficient evidence accumulates**.

### The Degraded Map

The system maintains what can be understood as a *degraded map* — a representation of the input space where:

- Known vectors occupy confirmed, stable positions
- Noise occupies unresolved regions with no assigned direction
- The boundary between them shifts as conflict logs accumulate

The map is called *degraded* because it is never complete. New inputs continuously arrive from outside the current map boundary. The Seed Expansion Protocol is the mechanism by which the map extends itself — not by pre-defining new regions, but by growing them from repeated encounters with the unknown.

### Three Structural Operations

At any fractal scale, the governance architecture performs three simultaneous operations:

| Operation | Target | Mechanism |
|---|---|---|
| **Separation** | Distinguish noise from vector | Data type classification; θd-gated escalation |
| **Friction minimization** | Reduce conflict between established vectors | Position clarity; niche differentiation; correction value landscape |
| **Noise cultivation** | Preserve unclassified inputs for potential vectorization | Conservative escalation (τ=1); conflict log accumulation; Seed Expansion Protocol |

Noise is not discarded. It is held in a low-escalation, high-sensitivity state until patterns emerge. Discarding noise prematurely would permanently close off domains that have not yet accumulated sufficient evidence — collapsing the system's capacity for expansion.

### Fractal Isomorphism

This three-operation structure repeats identically at every scale:

| Scale | Noise | Vector | Friction minimization |
|---|---|---|---|
| **Single agent (internal)** | Unknown input domain | Established processing pathway | Correct value landscape between pathways |
| **Multi-agent system** | New agent without confirmed position | Agent with established niche | Position clarity; mutual reinforcement loops |

The fractal structure does not simply repeat the same shape. It repeats the same **logic**: separate, minimize friction between what is known, and cultivate what is not yet known. This is why Rest Mode propagation is bottom-up — each layer must complete its own noise-to-vector conversion cycle before its upper layer can withdraw.

> *Vectors are not given. They are grown.*

---

### Vector Degradation: The Reverse Path

Vectorization is not a one-way process. Established vectors can degrade back toward noise through two structurally distinct mechanisms. This distinction is critical because the two types have different governance implications and recovery pathways.

#### Type 1 — Alignment Severance (Reversible)

The vector's information remains intact in the underlying weight structure, but the **pathway to activate it is severed**. The system can no longer reliably elicit the vector even though the knowledge exists.

| Trigger | Mechanism | Observable signal |
|---|---|---|
| New task fine-tuning | Orthogonal weight updates disrupt instruction-to-rationale mapping | Performance drop without loss of underlying knowledge |
| Conflict log stagnation | A vector that stops receiving conflict log reinforcement loses its activation alignment | Vector present in weights; inaccessible at runtime |
| Seed reconfiguration | Meta-rule changes alter the classification pathway that routes inputs to the vector | Domain-specific failure while adjacent domains remain intact |

**Governance implication:** Alignment-severed vectors are **recoverable**. A partial rationale injection, task-agnostic prefix, or targeted Seed adjustment can restore the activation pathway. The conflict log for this domain does not need to start from zero — it resumes from the pre-severance state.

> *Structural analogue: Spurious Forgetting (ICLR 2025) — performance drops in continual learning are structurally consistent with Type 1 degradation: alignment pathway loss without underlying knowledge loss. Partial rationale interventions restoring prior behavior are compatible with the prediction that the vector remains intact in weights.*

#### Type 2 — Weight Overwrite (Irreversible)

The vector's weight representation is **physically overwritten** by new learning. The knowledge itself is gone, not merely inaccessible.

| Trigger | Mechanism | Observable signal |
|---|---|---|
| Catastrophic forgetting during fine-tuning | Gradient interference in attention weights destroys prior vector representation | Performance drop that does not recover with prompting |
| Rapid successive task learning without replay | Each new task overwrites the previous without consolidation | Monotonic performance decay across earlier domains |
| High-sparsity task vector pruning | Forced sparsification removes weight values below magnitude threshold, including dormant but valid vectors | Targeted capability loss in pruned domains |

**Governance implication:** Overwritten vectors cannot be restored through alignment adjustment alone. Recovery requires either **Seed reinstallation** (if the meta-rule structure for that domain still exists) or **full re-cultivation** from noise — restarting the conflict log accumulation cycle for that domain.

> *Structural analogue: Catastrophic Forgetting literature (EMNLP 2025, ACM CL Survey 2025) is structurally consistent with Type 2 degradation: gradient interference in attention weights constitutes a weight overwrite event. Task vector pruning findings — that low-magnitude vectors are disproportionately affected by aggressive sparsification — are compatible with the prediction that dormant but intact vectors are the primary casualty.*

---

#### Implications for the Degraded Map

The distinction between Type 1 and Type 2 degradation makes the *degraded map* dynamic in both directions:

```
Noise ──[λlog accumulation]──────────────► Vector   (Vectorization)

Vector ──[alignment severance]──► Dormant ──[pathway restoration]──► Vector
         (Type 1: reversible)

Vector ──[weight overwrite]──────► Noise  ──[full recultivation]───► Vector
         (Type 2: irreversible)            (new conflict log cycle required)
```

A system that accounts for both degradation types is modeling the **actual dynamics** of the knowledge ecosystem — where regions of the map can go dark, and the governance response depends on which type of darkness is occurring.

**Governance diagnostic:** When a previously stable vector becomes unreliable, the first step is determining the degradation type. If prompting or pathway adjustment restores function → Type 1, apply alignment repair. If not → Type 2, initiate re-cultivation or Seed reinstallation.

> *Vectors are not given. They are grown — and they can be lost. The degraded map records both.*

---

## Consistency Measurement

### Key Parameters

| Symbol | Role | Meaning |
|---|---|---|
| **τ** | Judgment thresholds | Critical values for stabilization and Rest Mode conditions. Piecewise constant per evaluation regime — re-estimated at three trigger points: (1) Seed Handover phase transition, (2) new domain added to system scope, (3) Collapse recovery restart. |
| **θd** | Domain calibration | Operating threshold for a specific domain. Convergence speed follows a power-law curve: rapid adjustment in early conflict accumulation, decelerating as domain patterns stabilize (D-CPT Law, 2024). **Update rule:** if drift metric exceeds baseline by θ_drift, then θd ↑ (increase sensitivity); if domain is stable across evaluation window, then θd ↓ (reduce sensitivity). Bounded to prevent runaway adjustment. |
| **λlog** | Update trigger | Conflict-log mass threshold that triggers local rule revision or new rule formation. **Initial setting:** calibrated to approximately one θd calibration cycle. **Update rule:** if false-alarm rate in recent k-window is high, λlog ↑ (require more evidence before updating); if miss rate is high, λlog ↓ (trigger updates sooner). |

- **τ** answers: "Has this layer stabilized / reached Rest Mode?"
- **θd** answers: "How sensitive is this domain right now?"
- **λlog** answers: "When does accumulated log mass trigger a rule update?"

### Consistency Index (I)

I measures rule coherence at the **rule-pair level** — not aggregate conflict mass, but the weighted sum of conflicts between specific rule pairs. This structure makes it possible to identify which rule relationships are generating instability, rather than knowing only that instability exists.

```
I = 1 − (Σ wij) / M
```

| Symbol | Meaning |
|---|---|
| I | Consistency index (0–1; higher = more consistent) |
| wij | Conflict weight between rule pair (i, j) — product of conflict frequency and conflict severity for that specific pair |
| M | Normalization constant — set as maximum observed total conflict weight during the system's highest-stress period. Re-estimated at each τ re-estimation trigger (Seed Handover transition, new domain addition, Collapse recovery). |

**Why rule-pair structure matters:** A system where rule A repeatedly conflicts with rule B has a structural design problem that a total-mass index would obscure. The pair-level structure makes it possible to target intervention precisely — revise rule A or B, not the entire rule set.

### Meta-Contradiction Index (Ic)

High-severity conflicts — where two global rules are in direct opposition — are structurally different from low/medium severity conflicts and must not be mixed into I. They require governance redesign at the meta-rule level, not local rule revision. A single global-global conflict can render I meaningless if it dominates the sum.

```
Ic = 1 − (Σ wij | both i and j are global rules) / Mc
```

| Ic value | Meaning | Response |
|---|---|---|
| Ic = 1.0 | No active global rule conflicts | Normal operation |
| Ic falling | Global rule opposition emerging | Human-AI collaboration zone activates |
| Ic < τc | Global rules directly contradicting | Governance redesign required — Seed-level intervention |

> Ic is tracked separately from I. I can be high (local rules coherent) while Ic is low (global rules in conflict). Both conditions must be checked independently.

### Evaluation Window

Loop direction cannot be read from a single observation. "Sustained" trend is defined across two axes simultaneously:

| Axis | Definition | Purpose |
|---|---|---|
| **Event-count window (N)** | Most recent N conflict events | Captures interaction-density-independent signal |
| **Wall-clock window (T)** | Most recent T hours/days | Captures time-dependent drift patterns |

**Judgment rule:** use whichever window is more conservative (shows a longer or more adverse trend). A system that looks stable over T but shows adverse trend over N — or vice versa — is not yet stable.

Window sizes N and T are calibrated per domain during θd calibration. High-velocity domains (many interactions per hour) use smaller T and larger N. Low-velocity domains use larger T and smaller N. Both are updated at each τ re-estimation trigger.

### Conflict Severity

| Severity | Conflict Type | Response |
|---|---|---|
| **Low** | Local rules conflict with each other | Revise local rule |
| **Medium** | Local rule conflicts with global boundary | Upper-layer validation required |
| **High** | Global rules conflict internally | Human-AI collaboration zone activated |

**Low — production signal:** Output drift within acceptable range — perplexity rising, semantic coherence falling slightly. No human required; θd recalibration cycle handles. *(Arize AI, Evidently AI, 2025: drift detected via perplexity increase or semantic similarity drop below baseline.)*

**Medium — production signal:** Hallucination score crossing threshold; token-level confidence below 0.8; output deviates from ground truth. This is the most frequent intervention trigger in production (hallucination rates 15–38%). *(AWS Bedrock Agents, 2024: score < threshold → human review queue. HaluGate, vLLM 2025: confidence < 0.8 → human-in-the-loop escalation.)*

**High — production signal:** Two global objectives pulling in opposite directions — safety vs. utility; confidentiality vs. helpfulness; alignment vs. capability. Tracked via **Ic (meta-contradiction index)**, not I — this conflict exists above the local rule layer and must not be mixed into the I calculation. Does not resolve through θd recalibration. Requires human involvement for governance redesign at the meta-rule level. *(AI Control, arXiv:2504.05259, 2025: when model behavior diverges from intent and internal monitoring cannot adjudicate, human review of reasoning process required.)*

### Stabilization Conditions

All of the following must hold simultaneously:

| Condition | Source | Meaning |
|---|---|---|
| fesc ≤ τ1 | Network Architecture Theory | Conflict escalation is rare |
| I ≥ τ2 | Governance Rules Theory | Local rules are internally consistent |
| Ic ≥ τc | Governance Rules Theory | No active global rule contradictions |
| Lreinf ≥ τ3 | Position Clarity | Mutual reinforcement loops are active |
| SCC ≥ τ4 | Three System States | Self-correction capacity sufficient for autonomous recovery |

These four conditions correspond directly to the Rest Mode entry conditions. Stabilization is the per-layer confirmation that all four are trending virtuous — it is the precondition for Rest Mode entry, not a separate standard.

---

## Position Clarity and Diversity

### Position Ambiguity as a Storm Driver

When agents compete for the same optimum instead of occupying distinct roles, vector fields collide — making Vector Storm structurally likely.

| Position Ambiguous | Position Clear |
|---|---|
| Multiple agents → same optimum | Each agent → distinct optimum |
| Vector fields collide | Vector fields complement |
| → Vector Storm | → Stable ecosystem |

### Fractal Diversity Variables

| Symbol | Single-agent meaning | Multi-agent meaning |
|---|---|---|
| **Poverlap** | Attractor convergence degree | Positional overlap between agents |
| **Dint** | Weighted feedback density between internal layers | Weighted edge density of functional dependencies |
| **Lreinf** | Number of active exploration paths | Number of active mutual reinforcement loops |

Diversity must be maintained at every fractal layer — including within a single agent.

---

## Three System States

A layer exists in exactly one of three states at any given time:

| State | Loop Direction | Upper Layer | Description |
|---|---|---|---|
| **Rest Mode** | Self-reinforcing virtuous cycle | Monitoring only | Diversity sustains stability; stability sustains diversity. System improves as loop runs. |
| **Active Mode** | Loop not yet stabilized | Intervening | Governance actively correcting. Loop direction being shaped toward virtuous. |
| **Collapse** | Self-reinforcing vicious cycle | Overwhelmed or absent | Instability erodes diversity; diversity loss increases instability. System degrades as loop runs. |

The fundamental distinction between Rest Mode and Active Mode is not the presence or absence of storms — it is the **direction of the self-reinforcing loop**. A system in Rest Mode may still experience local Vector Storms, but the loop dynamics ensure they are absorbed rather than amplified.

**Rest Mode is not zero intervention — it is a change in the form of intervention.**

As a system matures from Active Mode toward Rest Mode, the governing layer's involvement does not disappear. It transforms:

| Stage | Intervention form | Granularity |
|---|---|---|
| Early Active Mode | Directive — governing layer specifies outputs or rules directly | Per-event |
| Late Active Mode | Validating — governing layer reviews and approves agent-proposed rules | Per-rule |
| Rest Mode | Statistical — governing layer monitors drift distributions; intervenes only when distribution-level threshold is breached | Per-distribution |

In Rest Mode, the governing layer is still present — but its intervention channel has zero per-event bandwidth. It acts only when the distribution of behavior shifts beyond the evaluation window thresholds, not in response to individual conflict events. This is why Rest Mode does not require the governing layer to disappear, only to become silent at the event level.

### Loop Direction as the Core Diagnostic

The three states are defined by loop direction, not by instantaneous metric values:

| Metric | Instantaneous value | Loop direction signal |
|---|---|---|
| fesc | Current escalation count | **Trend** — is upper-layer workload growing or shrinking? |
| I | Current consistency index | **Trend** — is rule coherence increasing or decreasing? |
| Lreinf | Current reinforcement loop count | **Trend** — are interdependencies strengthening or collapsing? |
| SCC | Current self-correction capacity | **Trend** — is recovery speed improving or degrading? |

A layer with I = 0.8 falling is in worse structural condition than a layer with I = 0.6 rising. The value alone is insufficient — the direction determines which state the layer is moving toward.

**fesc trend is the primary observable.** Because fesc directly measures upper-layer workload, it is the most structurally interpretable signal: if the upper layer is doing less over time, the lower layer is internalizing governance. If the upper layer is doing more, it is not.

### Why Measurement Must Be Cumulative, Not Reactive

This is a critical infrastructure requirement. The loop direction cannot be read from a single observation — it requires accumulated evidence over time.

Reactive threshold systems (checking whether fesc > τ at any given moment) suffer from two structural failures:

1. **Micro-fluctuation noise** — any individual conflict event can temporarily push fesc above threshold without representing a real trend change. Reactive systems treat noise as signal.
2. **Monitoring as load** — at scale, continuous per-event governance responses become the primary source of system load. The monitoring system creates the instability it is trying to detect.

The cumulative design — conflict log accumulation → θd calibration → λlog-triggered rule updates — is the correct architecture because it measures **drift**, not snapshots.

This prediction is structurally consistent with Agent Drift research (arxiv 2601.04170, 2026) tracking 847 simulated workflows: behavioral degradation follows a nonlinear cumulative pattern compatible with self-reinforcing loop dynamics. Decline rate between interactions 0–100 is 0.08 points per 50 interactions; by interactions 300–400, the same metric declines at 0.19 points per 50 interactions — a pattern consistent with loop direction becoming self-reinforcing, which snapshot monitoring would miss entirely. The same study's finding that drift mitigation requires ongoing cumulative frameworks — neither static nor reactive — is compatible with the conflict log accumulation architecture specified here.

> The governance infrastructure — conflict log pipeline, θd calibration cycle, fesc trend aggregation — must be designed before Rest Mode is meaningful. Without it, loop direction is invisible.

### Self-Correction Capacity (SCC)

SCC is the system's ability to detect contamination or Vector Storm, contain it **without external intervention**, and return to a stable attractor autonomously.

SCC is not an independent property — it is the emergent result of two structural conditions being simultaneously satisfied:

**Dint (internal diversity)** — each vector has grown sufficiently that it occupies a distinct, well-defined position in the capability space. A well-developed vector has adjacent vectors nearby that differ from it in known, stable ways.

**Lreinf (mutual reinforcement loops)** — vectors are not isolated. They are linked through active interdependencies: each vector's stability is partly maintained by its neighbors.

When both conditions hold, contamination detection and purification become structurally automatic:

```
Contaminated input arrives
  │
  ├─ Adjacent vectors provide contrast baseline
  │   → contaminated pattern deviates from expected neighborhood
  │   → deviation is logged as conflict (fesc event)
  │
  └─ Lreinf pulls contaminated vector back toward stable neighborhood
      → if contamination is local and loops are strong,
        purification completes without upper-layer involvement
      → SCC loop closes: detect → log → correct → stabilize
```

**SCC fails when either structural condition is absent:**

- Dint too low → adjacent vectors do not exist or are too similar → contaminated pattern has no contrast baseline → detection fails silently
- Lreinf too low → vectors are isolated → no corrective pull from neighbors → contamination propagates unchallenged even if detected

This is why SCC is downstream of Dint and Lreinf, not independent of them. A system cannot have high SCC with low Dint or collapsed Lreinf — the detection-purification loop has no substrate to run on.

| SCC Level | Storm frequency | Recovery speed | Loop direction |
|---|---|---|---|
| Low | High | Slow or absent | Vicious — storms accumulate faster than recovery |
| Medium | Moderate | Partial | Transitional — loop direction not yet determined |
| High | Rare | Full, autonomous | Virtuous — recovery outpaces storm generation → **Rest Mode** |

**Measurement units:**
- **fesc** — number of escalations per K interactions, or per hour. K is calibrated per domain velocity during θd calibration.
- **Lreinf** — number of active mutually reinforcing edges above weight ε, where ε is the minimum edge weight considered structurally meaningful (calibrated during domain stabilization).
- **SCC** — probability of autonomous recovery within evaluation window W, estimated from historical recovery events in the conflict log. Equivalently: inverse of expected recovery time (ERT) normalized to [0, 1].

### Rest Mode Entry Conditions (AND — all four required)

Entry requires all four conditions simultaneously satisfied and trending in the virtuous direction. This is a high bar by design — stability must not be declared prematurely.

| Condition | Instantaneous check | Trend requirement |
|---|---|---|
| fesc ≤ τu-1 | Escalation rare | fesc decreasing or stable over evaluation window |
| I ≥ τu-2 | Local rules coherent | I increasing or stable over evaluation window |
| Ic ≥ τu-c | No global rule contradiction | Ic stable or increasing over evaluation window |
| Lreinf ≥ τu-3 | Loops active | Lreinf increasing or stable over evaluation window |
| SCC ≥ τu-4 | Self-recovery possible | Recovery speed improving or stable over evaluation window |

### Rest Mode Exit Conditions (OR — any one sufficient)

Exit requires only one condition degrading into a sustained vicious trend. This asymmetry is structural, not arbitrary.

| Condition | Exit trigger | Cascade risk |
|---|---|---|
| fesc > τu-1 sustained | Upper-layer workload growing — lower layer losing autonomy | Medium — upper layer may absorb if capacity allows |
| I < τu-2 sustained | Local rule coherence collapsing — consistency entering vicious cycle | High — directly undermines all other conditions |
| Ic < τu-c sustained | Global rules in active contradiction — meta-rule structure destabilizing | Critical — no local rule revision can resolve; governance redesign required |
| Lreinf < τu-3 sustained | Reinforcement loops breaking — mutual dependencies inverting to competition | High — position clarity erodes rapidly once loops collapse |
| SCC < τu-4 sustained | Self-recovery failing — storms accumulating without resolution | Critical — vicious cycle locks in without external intervention |

**Why asymmetric:** Entry is a sufficient condition claim ("the system has internalized governance"). Exit is a necessary condition violation ("the system can no longer sustain itself"). These are structurally different logical operations and should not be forced into symmetric form.

In ecological terms: a climax community takes decades to establish (AND-entry) but can be disrupted by a single species collapse or external shock (OR-exit). The asymmetry reflects the thermodynamic reality that ordered states are harder to build than to destroy.

**"Sustained" is defined by the evaluation window**, not by a single observation. A single spike in fesc does not trigger exit — the cumulative log must show a directional trend across the window. This preserves the anti-reactive property of the governance architecture.

### State Transition Map

```
Active Mode
  │
  │ All four entry conditions met (AND)
  │ All four trends virtuous simultaneously
  ▼
Rest Mode ◄──────────────────────────────┐
  │                                       │
  │ Any one exit condition triggered (OR) │ Recovery complete
  │ Sustained vicious trend detected      │ (return to Active)
  ▼                                       │
Active Mode (upper layer reactivates) ───►┘
  │
  │ SCC = 0, upper layer overwhelmed
  │ Vicious cycle self-reinforcing, no recovery pathway
  ▼
Collapse
  │
  │ External intervention + Seed reinstallation
  ▼
Active Mode (restart from Phase 1 socialization)
```

### Rest Mode Propagation

**Socialization direction:** top-down (principles flow via Seeds)  
**Rest Mode direction:** bottom-up (as layers are socialized, upper oversight withdraws)

- **Phase 1 — Socialization:** Upper layer installs Seed → conflict logs accumulate → θd calibrates → lower layer internalizes governance principles
- **Phase 2 — Rest Mode propagation:** Lower layer loop transitions to virtuous → upper-layer oversight enters Rest Mode → human attention moves to next unsocialized layer

### What Rest Mode Preserves

| Category | Treatment | Basis |
|---|---|---|
| Tacit knowledge patterns | ✓ Preserved | Spurious Forgetting (ICLR 2025): knowledge persists in weights even when activation paths are severed — Type 1 degradation is reversible |
| Structural learning from stabilization | ✓ Preserved | θd calibration history embedded in conflict log accumulation — not dependent on active intervention |
| Escalation calibration history | ✓ Preserved | Conflict log is a persistent data structure, not a runtime state |
| Mutual reinforcement loop structure | ✓ Preserved | Lreinf is structural — loop topology survives Rest Mode entry as long as positions remain distinct |
| Storm-inducing vector orientations | ✗ Released | Conflict log drains below λlog for dormant storm patterns — no active reinforcement → natural decay |
| Self-reinforcing conflict patterns | ✗ Released | Without conflict log mass sustaining them, local rules expire on next θd calibration cycle |

---

## Rest Mode Failure: When the System Collapses

Rest Mode is stable but not permanent. When conditions shift beyond what the internalized governance can absorb, the system crosses a threshold and enters a failure trajectory. These are not random breakdowns — each failure mode corresponds to a specific structural condition being violated, and each has empirical counterparts in current LLM research.

### The Threshold Structure of Collapse

Failure does not begin at Rest Mode exit. It begins when one of the four entry conditions degrades beyond its τ threshold and the layer's SCC is insufficient to self-recover. The sequence is:

```
Rest Mode entry condition degraded
→ SCC insufficient to recover internally
→ upper-layer oversight channel must reactivate
→ if upper layer also unavailable or overloaded → cascade begins
→ system collapse
```

The critical insight is that **collapse is not instantaneous**. It propagates through the fractal structure, and the rate of propagation is determined by how many layers share the same degraded condition simultaneously.

### Failure Case Taxonomy

#### Case 1 — Consistency Collapse (I < τ2)
**Trigger:** Conflict log mass accumulates faster than θd can calibrate. Rule coherence breaks down.

Internal rules begin contradicting each other without resolution. The agent or layer loses the ability to produce consistent outputs across similar inputs. In the single-agent case, this manifests as self-contradictory behavior within a context window — the agent responds differently to structurally identical situations with no logged reconciliation.

**Structural analogue:** Catastrophic Forgetting (CF) in LLMs is structurally consistent with Consistency Collapse: fine-tuning on new tasks produces the kind of rule coherence degradation that I < τ2 is designed to detect. Li et al. (EMNLP 2024) find that loss landscape sharpness is associated with brittle representations under new domain pressure — compatible with the prediction that non-stationary domains produce oscillating θd without convergence. The "spurious forgetting" variant (ICLR 2025) — performance drops reflecting alignment loss rather than knowledge loss — is structurally analogous to the distinction between I falling (local coherence) and Ic falling (meta-rule contradiction).

| Governance signal | Meaning |
|---|---|
| I falling toward τ2 | Early warning — rule conflicts accumulating faster than resolution |
| I < τ2 sustained | Consistency collapse — layer cannot self-resolve, escalation mandatory |
| θd oscillating without convergence | Domain is non-stationary; reclassify as Permanently High-Context |

---

#### Case 2 — Escalation Flood (fesc > τ1)
**Trigger:** Conflict volume at lower layers exceeds upper-layer absorption capacity.

Lower layers begin forwarding conflicts they should be handling autonomously. The upper layer's oversight channel, designed to be silent in Rest Mode, is suddenly receiving traffic it cannot process at the designed rate. If this persists, the upper layer itself enters a conflict accumulation spiral.

**Structural analogue:** MAST taxonomy (Cemri et al., NeurIPS 2025) — analyzing 1,642 execution traces across 7 frameworks — identifies **inter-agent misalignment** as the dominant failure category, structurally consistent with the prediction that Escalation Flood arises from position ambiguity and loop collapse rather than individual agent error. The specific modes map directly:

| MAST failure mode | Governance equivalent |
|---|---|
| Role drift — planner starts writing code | Position ambiguity → Poverlap rising → vector field collision |
| Conversation reset loop | fesc cycling without resolution — upper layer re-entering intervention repeatedly |
| Information withholding between agents | Mutual reinforcement loops collapsing — Lreinf falling below τ3 |
| Task derailment | Local attractor diverging from global objective — landscape design failure |

MAST reports 41–86.7% failure rates across SOTA open-source MAS frameworks, with inter-agent misalignment accounting for the largest share. This is the empirical signature of a system where Rest Mode was either never fully achieved or where topology shifts triggered exit.

---

#### Case 3 — Reinforcement Loop Collapse (Lreinf < τ3)
**Trigger:** Positional differentiation breaks down. Agents converge toward overlapping attractors.

Mutual reinforcement loops require that agents occupy distinct niches — Agent A's success creates conditions favorable to Agent B, and vice versa. When positions overlap, this loop inverts: Agent A's success now competes with Agent B's, and the reinforcement structure becomes a competition structure. Stability that was self-sustaining becomes self-undermining.

**Structural analogue:** The faulty agent cascade study (arxiv 2408.00989, 2025) finds that in multi-fault settings, **high-level planners disproportionately propagate failures** — a pattern structurally compatible with Lreinf collapse at the highest-leverage node. When mutual reinforcement topology breaks at the coordinating layer, the ecosystem collapses rather than degrades gracefully, consistent with the OR-exit prediction that a single condition breach can trigger system-wide instability. The finding that star-topology graphs preserve hierarchy advantage is compatible with the DFG principle that positional differentiation reduces cascade propagation.

---

#### Case 4 — SCC Failure: Unrecoverable Storm
**Trigger:** Vector Storm occurs within scope, but self-correction mechanisms cannot contain it. Storm frequency is low but recovery speed is zero or undefined.

This is the most dangerous failure mode because it can occur in a system that *appears* to be approaching Rest Mode — storm events are rare, but when they occur, the layer has no internal recovery pathway. The asymptotic structure of SCC means this state can persist indefinitely without triggering upper-layer intervention if storm frequency stays below τu-1.

**Structural analogue:** AgentErrorTaxonomy (arxiv 2509.25370, 2025) describes cascading failures where a single unrecovered error propagates through planning, memory, reflection, and action modules — structurally compatible with the prediction that SCC = 0 produces unrecoverable storm propagation across fractal layers. The paper's identification of the absence of module-level detection frameworks is structurally analogous to the condition where SCC measurement infrastructure exists but the detection-purification loop has no substrate to run on.

---

#### Case 5 — Seed Corruption
**Trigger:** The meta-rule structure itself becomes internally inconsistent, or the Seed is installed with a design flaw that only manifests under specific domain conditions.

Unlike the above cases, Seed corruption does not produce gradually increasing conflict log mass. It produces a hard failure when the expansion protocol encounters a domain that the Seed's meta-rules cannot coherently resolve. The agent cannot even construct a local rule proposal — the generative procedure itself is broken.

**Structural analogue:** Specification and System Design Failures (MAST FC1 category) — including task specification violations, role specification violations, and step repetition loops. These correspond to Seeds that were installed with ambiguous or contradictory meta-rules. MAST identifies these as the category most resistant to simple prompt engineering fixes, requiring structural redesign — consistent with the DFG position that Seed corruption requires upper-layer intervention at the meta-rule level, not the local rule level.

---

### Fractal Collapse Propagation

The above cases are not independent. At sufficient scale, they interact:

```
Case 2 (escalation flood) → upper layer overwhelmed
→ upper layer's own I begins falling → Case 1 at upper layer
→ upper layer cannot adjudicate lower-layer conflicts
→ lower layer Lreinf collapses → Case 3
→ full fractal collapse
```

In multi-agent environments, misinformation propagation leads to poisoned information being enhanced through collaborative reasoning, creating cascading security breaches across the system — which is the security-domain expression of the same structural dynamic.

The collapse propagation rate is determined by three factors: topology density (how many layers share the same degraded condition), the δ between current I and τ2 at each layer, and whether the permanently High-Context oversight channels remain operational. The last point is critical: **Rest Mode collapse does not disable permanently High-Context channels**, because those channels never entered Rest Mode in the first place. They remain the final containment structure.

### Summary: Failure Mode to Governance Condition Mapping

| Failure Case | Violated Condition | Early Signal | Empirical Reference |
|---|---|---|---|
| Consistency Collapse | I < τ2 | θd oscillating | Catastrophic Forgetting — Li et al., EMNLP 2024 |
| Escalation Flood | fesc > τ1 | Conflict log growth rate accelerating | MAST taxonomy — Cemri et al., NeurIPS 2025 |
| Reinforcement Loop Collapse | Lreinf < τ3 | Poverlap rising between adjacent agents | Faulty agent cascade — arxiv 2408.00989 |
| Unrecoverable Storm | SCC < τu-4 | Storm events present but recovery absent | AgentErrorTaxonomy — arxiv 2509.25370 |
| Seed Corruption | Meta-rule incoherence | Hard failure on novel domain | MAST FC1 Specification Failures |

> Rest Mode failure is not the end of governance. It is the signal that governance must restart — at the layer where the condition first broke, with the upper layer reactivating only long enough to restore autonomous operation.

---

### Failure Diagnosis Flowchart

When a layer exits Rest Mode or shows degradation signals, use this flowchart to identify the failure case before selecting a response.

```
System shows degradation signal
  │
  ├─ Is Ic falling (global rule conflict)?
  │     YES → Case 5 path: Human-AI collaboration zone
  │            Ic < τc → Governance redesign (Seed-level)
  │
  └─ Is Ic stable? Continue below:
       │
       ├─ Is I falling (rule coherence degrading)?
       │     YES → Case 1: Consistency Collapse
       │            Check: is θd oscillating without convergence?
       │            → if yes: domain is non-stationary, reclassify
       │            → if no: rule revision cycle, θd recalibration
       │
       ├─ Is fesc rising (escalation flood)?
       │     YES → Case 2: Escalation Flood
       │            Check SCC: is self-recovery still possible?
       │            → SCC present: Feedback-only recovery (Supervised Delegation entry)
       │            → SCC absent: Direct Injection restart required
       │
       ├─ Is Lreinf falling (loops collapsing)?
       │     YES → Case 3: Reinforcement Loop Collapse
       │            Positional re-differentiation required
       │            → Direct Injection restart (topology must be rebuilt)
       │
       └─ Is SCC falling (recovery failing)?
             YES → Case 4: Unrecoverable Storm
                    Self-correction substrate degraded
                    → Direct Injection restart
                    Check Type 1 vs Type 2 before proceeding
                    (see Collapse Recovery procedure below)
```

### Collapse Recovery: Practical Decision Procedure

The State Transition Map shows `"External intervention + Seed reinstallation → Active Mode (restart from Phase 1)"` as a single line. In practice, this is the highest-cost and highest-judgment operation in the governance lifecycle. The decision procedure has three steps:

**Step 1 — Determine degradation type before intervening**

Before any reinstallation, apply the Type 1 / Type 2 diagnostic from the Vector Degradation section:

| Test | Method | Interpretation |
|---|---|---|
| Pathway restoration attempt | Inject partial rationale; apply task-agnostic prefix; adjust Seed routing | If performance recovers → Type 1 (alignment severance). Do NOT reinstall Seed. |
| Non-response to pathway restoration | No recovery after 2–3 targeted alignment interventions | Type 2 (weight overwrite). Proceed to Step 2. |

**Step 2 — Identify which failure case triggered collapse**

Different failure cases require different recovery entry points:

| Failure Case | Recovery entry point | Why |
|---|---|---|
| Consistency Collapse (I < τ2) | Supervised Delegation | θd calibration structure intact; only rule coherence needs re-establishment via labeled validation |
| Escalation Flood (fesc > τ1) — SCC present | Feedback Only | Self-correction capacity still exists; reward signal is sufficient to restore autonomous operation without direct management |
| Escalation Flood (fesc > τ1) — SCC absent | Supervised Delegation | Self-correction gone; need validation layer before autonomous judgment is viable |
| Reinforcement Loop Collapse (Lreinf < τ3) | Direct Injection | Loop structure requires positional re-differentiation — must restart knowledge topology from substrate |
| Unrecoverable Storm (SCC < τu-4) | Direct Injection | Self-correction capacity must be rebuilt from substrate |
| Seed Corruption | Full Seed reinstallation → Direct Injection | Meta-rule structure itself is broken; no lower-phase entry is coherent |

**Step 3 — Confirm Seed integrity before Phase 1 restart**

If Seed reinstallation is required (Seed Corruption or full Type 2 collapse), verify that the new Seed does not carry the same design flaw that caused the original failure. Specifically: check that the expansion protocol can coherently classify the domain that triggered the hard failure. A Seed reinstalled with the original flaw will reproduce the failure on first encounter with the same domain type.

> *The governing layer's goal in collapse recovery is not to restore the previous state — it is to rebuild the substrate for a governance cycle that does not fail in the same way.*

---

## Seed Handover

Seed Handover applies at two scales: **multi-agent system evolution** (the upper layer withdrawing from lower layers as they mature) and **single-agent new domain development** (the governing layer withdrawing from a specific domain as it stabilizes). Both follow the same logic — direct management is the exception, not the rule, and withdrawal is governed by measurable convergence conditions, not elapsed time.

### Multi-Agent Handover Stages

| Stage | Human Role | Description |
|---|---|---|
| **Initial** | Designer | Creates meta-rule structure, positional principles, expansion protocol |
| **Intermediate** | Validator | Verifies AI-proposed seed updates; analyzes conflict logs |
| **Mature** | Observer | AI takes over seed design for lower layers; human monitors boundary compliance |
| **Rest** | Absent | System regenerates its own seeds autonomously |

### Single-Agent New Domain: The Four-Phase Withdrawal Protocol

When a single agent encounters a new domain, the governing layer (human or upper-layer agent) does not observe from a distance — it manages directly until domain stabilization is confirmed. This mirrors the standard domain adaptation pipeline in LLM research: **DAP → SFT → Preference Optimization → Deployment**, where each transition is governed by measurable convergence, not fixed epochs.

| Phase | DFG Name | Practical Analogue | Governing Layer Role | Withdrawal Condition |
|---|---|---|---|---|
| **1** | Direct Injection | Domain-Adaptive Pre-training (DAP) | Directly supplies domain corpus; structures knowledge topology | Conflict log growth rate stabilizing — domain patterns beginning to emerge |
| **2** | Supervised Delegation | Supervised Fine-Tuning (SFT) | Provides labeled examples; agent executes but governing layer validates each output | I trend positive across θd calibration cycles; escalation rate fesc falling |
| **3** | Feedback Only | Preference Optimization (DPO/RLHF) | Agent makes autonomous judgments; governing layer provides reward signal only | fesc ≤ τu-1 sustained; I ≥ τu-2 trending stable |
| **4** | Withdrawal | Autonomous Deployment | Governing layer monitors drift signals only; intervenes only on threshold breach | All four Rest Mode entry conditions met (AND) |

**Why Phase 1 cannot be skipped:** SFT alone is insufficient for domains containing unfamiliar concepts, dense acronyms, or high context dependency. Without direct knowledge injection first, the agent cannot form coherent local rules — the Seed Expansion Protocol has no accumulated log mass to work with. Direct management in Phase 1 is what creates the λlog substrate that later phases build on.

> *Structural analogue: The finding that "SFT memorizes while RL generalizes" (Chu et al., 2024) is structurally compatible with the Phase 1–2 management requirement: SFT as initialization step stabilizes output structure before autonomous generalization becomes viable, consistent with the prediction that Direct Injection must precede Supervised Delegation in domains without existing rule structure.*

### Quantified Withdrawal Thresholds

Domain adaptation research provides empirical anchors for the Handover transition points:

| Threshold | Empirical finding | DFG mapping |
|---|---|---|
| **Replay ratio** | R* ≈ 30–50% maximizes domain transfer without general capability loss; >50% shows diminishing returns (D-CPT Law, Gu et al. 2024) | λlog accumulation zone — below 30% is insufficient log mass; above 50% is over-management |
| **Convergence signal** | Four-pillar evaluation: general retention + target task acquisition + domain benchmark + forward/backward transfer must stabilize simultaneously (CPT literature, Wu et al. 2024) | AND-entry condition for Phase 4 withdrawal — all four DFG metrics must trend stable |
| **Management necessity** | Tasks with few hundred examples and familiar domain can skip Phase 1; tasks with unfamiliar concepts, dense acronyms, or large context requirements cannot (State of SFT, 2025) | Seed Expansion Protocol trigger — whether the domain requires DAP depends on whether existing rule structure can classify it |

### Handover Completion Conditions

The governing layer withdraws from a domain when — and only when — all of the following hold simultaneously. This is the domain-level AND condition, parallel to the system-level Rest Mode entry:

1. I ≥ τu-2 **and trending stable** across at least one full θd calibration cycle
2. fesc ≤ τu-1 **and trending downward** — the domain is no longer generating upper-layer load
3. Lreinf ≥ τu-3 — the domain has formed mutual reinforcement relationships with adjacent domains
4. A subsystem operating under agent-designed seeds for this domain has maintained stability for a duration equivalent to at least **two θd calibration cycles**

> Handover transfers design authority, not foundational constraint. The governing layer's withdrawal from a domain does not remove global rules — it removes the obligation to actively manage local rule formation.

---

## Single-Agent Intervention: When and How

> *This section applies the Three System States and Seed Handover frameworks to production monitoring decisions. Concepts like Rest Mode, Active Mode, fesc, I, and the Four-Phase Withdrawal Protocol are defined in the preceding sections.*

In practice, governing a single-agent system means knowing when to intervene, what type of intervention is appropriate, and when to withdraw. The following maps real-world production intervention patterns to the DFG governance framework.

### Intervention Trigger Taxonomy

| Trigger Type | Observable signal | DFG mapping | Intervention type |
|---|---|---|---|
| **Hallucination threshold breach** | Hallucination score < 0.8 (token-level); answer relevancy drop; factual accuracy < baseline | I falling — rule coherence degrading; θd recalibration needed | Medium severity: human review queue; RAG grounding check |
| **Behavioral drift** | Perplexity rising over time; semantic coherence falling; output distribution shifting from baseline | fesc trend rising — lower layer generating increasing noise load | Cumulative log trigger: θd recalibration cycle; not per-event intervention |
| **Prompt injection / adversarial input** | Input-output semantic mismatch; safety filter triggered; unexpected tool call pattern | Noise entering as contaminated vector — Dint boundary stress | Pre-output filter (guardrail); log event for contamination tracking |
| **Global objective conflict** | Safety constraint vs. task completion pulling in opposite directions; refusal rate anomalous for domain | High severity: global rules conflicting internally | Human-AI collaboration zone: meta-rule review, not local rule revision |
| **Out-of-distribution domain** | Novel input type with no existing classification pathway; conservative escalation triggered | Seed Expansion Protocol activating — conflict log accumulation begins | Upper layer enters Phase 1 direct management for that domain |
| **Performance degradation (non-hallucination)** | Task completion rate falling; latency increasing; reasoning loop repetition detected | SCC degrading — self-correction capacity insufficient | Check for Type 1 vs. Type 2 vector degradation; apply alignment repair or re-cultivation |

### When NOT to intervene

Reactive per-event intervention is structurally harmful at scale. The following signals should **not** trigger human intervention:

| False alarm signal | Why it is not an intervention trigger |
|---|---|
| Single fesc spike | Does not represent trend — requires cumulative evaluation window |
| Temporary output variance | Non-determinism is inherent; single-event variance is noise, not signal |
| Confidence drop on novel domain | Expected during Seed Expansion Protocol Phase 1 — conservative escalation is correct behavior, not failure |
| Short-term perplexity rise after fine-tuning | Normal recalibration period — θd is adjusting; allow one calibration cycle before escalating |

> *Structural analogue: Production LLM monitoring practice (Arize AI, Maxim AI, Evidently AI, 2025) converges on the finding that continuous per-event monitoring creates more instability than it resolves, and that drift detection requires sustained trend signal rather than reactive thresholds — compatible with the DFG prediction that cumulative log architecture is structurally necessary, not merely operationally convenient.*

### Intervention Withdrawal Conditions

Intervention should withdraw as soon as — and not before — the trigger condition resolves:

| Trigger type | Withdrawal condition |
|---|---|
| Hallucination breach | Hallucination score returns above threshold AND stable across 2+ evaluations |
| Behavioral drift | fesc trend reverses; perplexity returns to baseline across evaluation window |
| OOD domain | Seed Expansion Protocol completes Phase 2 (SFT stage) — λlog threshold crossed for that domain |
| Global objective conflict | Meta-rule redesign validated; I returns above τ2 |

> The governing layer withdraws from each trigger type independently. Withdrawal from one trigger does not imply withdrawal from all — each domain and each trigger type has its own calibration state.

---

## The Optimal Point

| Variable | Meaning |
|---|---|
| Risk | Vector Storm frequency × intensity |
| Cost | Intervention cost + monitoring cost |
| Utility | Knowledge ecosystem diversity |
| U* | Minimum acceptable diversity threshold |

### U* Quantification

U* is not an arbitrary parameter. It is the minimum level of diversity below which mutual reinforcement loops — and thus Rest Mode — can no longer be sustained. It is expressed as a function of the three measurable diversity variables:

```
U* = f(Poverlap, Lreinf, Dint)

where:
  Poverlap  = positional overlap between agents/domains (0–1; lower = more distinct)
  Lreinf    = strength of mutual reinforcement loops (0–1; higher = stronger interdependency)
  Dint      = internal diversity of each agent/domain (0–1; higher = richer local capability space)
```

**Operational definition:**

```
U* is violated when ANY of the following holds:

  Poverlap  > θ_overlap   (positions converging — niche collapse beginning)
  Lreinf    < θ_reinf     (loops weakening — mutual dependency inverting to competition)
  Dint      < θ_dint      (internal capability space narrowing — over-specialization)
```

This is again an OR condition: any single variable crossing its threshold indicates that the diversity ecosystem is no longer self-sustaining. The system does not need all three to degrade simultaneously — one is sufficient to trigger governance intervention.

**Threshold anchoring:**

The individual thresholds θ_overlap, θ_reinf, θ_dint are not universal constants. They are calibrated per system through the conflict log accumulation process — the same θd calibration mechanism that governs local rule formation. A system that has never stressed its diversity boundaries will have uncalibrated thresholds. Conflict log accumulation under boundary stress is what makes U* empirically observable.

> *Empirical anchor: Preference tuning substantially reduces lexical and semantic diversity compared to SFT (Kirk et al., 2024; Guo et al., 2024 — Benchmarking Linguistic Diversity of LLMs, TACL 2025). This documents Dint collapse under over-alignment — a measurable U* violation in single-agent systems.*

---

### Asymmetric Specialization: The Single-Agent U* Violation

The same diversity requirement that applies to multi-agent systems applies within a single agent. An agent that develops capabilities in an asymmetric pattern — deepening one domain while leaving others underdeveloped — violates U* at the internal scale. This has two structural consequences:

**1. Contamination vulnerability**

A highly specialized agent has a narrow Dint. When contaminated input arrives (adversarial prompts, poisoned data, out-of-distribution queries), there are few adjacent capability vectors to absorb or triangulate the anomaly. The contaminated pattern has nowhere to be checked against — it propagates unchallenged.

> *Structural analogue: Over-specialized models showing entity-swap accuracy drops of −22.4% under factual perturbation vs. −9.8% for more general models (SUAS 2025) is structurally consistent with the prediction that low Dint produces high contamination sensitivity: narrow capability space leaves no adjacent vectors to provide contrast baseline for anomaly detection.*

**2. Performance degradation under distribution shift**

Preference tuning (RLHF/DPO) applied asymmetrically — optimizing for a narrow output distribution — produces models that sacrifice Dint for alignment precision. The result is measurably lower diversity even on tasks unrelated to the fine-tuned domain.

> *Structural analogue: Preference tuning substantially reducing lexical and semantic diversity vs. SFT (Kirk et al., 2024) is structurally consistent with the prediction that asymmetric optimization collapses Dint. Adversarially trained models suffering deteriorated generalization on clean data (Schmidt et al., 2018; Tsipras et al., 2019) is compatible with the same mechanism: asymmetric specialization narrows the internal capability space in a way that reduces performance on the dimensions not optimized.*

**The structural rule:**

```
Dint must be maintained across ALL capability domains, not just the primary deployment domain.

An agent with:
  Dint(domain_A) = 0.9    ← deep specialization
  Dint(domain_B) = 0.2    ← atrophied
  Dint(domain_C) = 0.1    ← near-absent

...has a system-level Dint = min(Dint_i) = 0.1, not mean(Dint_i) = 0.4

U* uses the minimum, not the average. A single atrophied domain is a contamination entry point
for the entire agent — regardless of strength elsewhere.
```

This is why the DFG approach to single-agent governance treats domain balance as a first-class concern, not a secondary optimization. The minimum Dint across domains determines the agent's true contamination resistance.

**Connection to SCC:** Dint collapse in any domain directly degrades SCC for the entire agent. When a domain's Dint falls below θ_dint, the detection-purification loop in that domain loses its contrast baseline — contaminated patterns arrive with no adjacent vectors to flag them as anomalous. The contamination does not just persist in that domain; because vectors are connected through Lreinf, an undetected contamination in a weak domain propagates into adjacent domains whose Dint is still intact. A single atrophied domain is not just a local vulnerability — it is an unmonitored entry point into the entire vector network.

---

**System Lifecycle:**

| Phase | Characteristics |
|---|---|
| Growth | Diversity increasing. Risk and cost high. Governance actively intervening. |
| Maturity | Diversity maintained. Risk and cost minimized. Governance in Rest Mode. |
| Rest | External intervention unnecessary. Self-correction capacity sufficient. |

> *The supreme rule: preserve knowledge ecosystem diversity at all fractal scales — including the internal scale of a single agent.*

---

## Core Assumptions

> *These assumptions define the scope of Governance Rules Theory as an architectural component. They are not claims about AI governance universally — they are the structural preconditions under which the rule-governance layer of DFG operates.*

1. Landscape design is more effective than direct intervention at scale
2. Rules operate in two layers: global (immutable) and local (autonomous, validated)
3. Upper layers define meta-rules; lower layers define rule content
4. Global rules always take precedence over local rules
5. All conflicts must be logged; logs serve as learning data and θd calibration input
6. τ, θd, and λlog are distinct and non-interchangeable
7. Position ambiguity is a primary upstream driver of Vector Storm
8. Diversity requires position clarity and mutual reinforcement loops at every fractal scale
9. Rest Mode is stable but not permanent — exits when any one of the four entry conditions develops a sustained vicious trend (OR-exit condition)
10. Rest Mode achievement and Seed Handover completion are the same event viewed from different angles
11. The supreme objective is knowledge ecosystem diversity preservation

---

## Structural Correspondences

| Theory Concept | Related Field | Corresponding Concept |
|---|---|---|
| Meta-rules | Philosophy of law | Constitutional vs. statutory law |
| Landscape design | Behavioral economics | Nudge / choice architecture (Thaler & Sunstein, 2008) |
| Subsidiarity | Political theory | EU constitutional subsidiarity (Follesdal, 1998) |
| Correction values | Reinforcement learning | Reward shaping (Ng et al., 1999) |
| θd calibration | Control theory / ML training dynamics | Gain scheduling; CPT learning rate decay curve (D-CPT Law, 2024) — power-law convergence as domain stabilizes |
| Seed expansion | Developmental psychology | Piaget's schema assimilation/accommodation |
| Position clarity | Ecology | Niche differentiation (Elton, 1927) |
| Mutual reinforcement | Ecology | Symbiosis / trophic interdependency |
| Diversity as stability | Ecology | Diversity-stability relationship (de Mazancourt et al., 2013) |
| Rest Mode | Ecology | Climax community / old-growth equilibrium |
| SCC | Dynamical systems | Lyapunov stability (structural analogue) |
| Vector Storm as growth driver | Complex systems | Dissipative structures (Prigogine) |
| Optimal point | Complex systems | Edge of chaos (Kauffman) |

---

## Relationship to Other Theories

```
Deficit-Fractal Governance (DFG)
│
├── Three-Layer Governance Architecture
├── Vector Storm Theory          — defines Risk; position ambiguity as upstream driver
├── Network Architecture Theory  — defines escalation and stabilization conditions
├── Governance Rules Theory      — this document
├── Recovery Theory              (separate document)
└── Prediction Model             (separate document)
```

---

## References

1. Thaler, R. H., & Sunstein, C. R. (2008). *Nudge*. Yale University Press.
2. Ouyang, L., et al. (2022). Training language models to follow instructions with human feedback. *NeurIPS*.
3. Bai, Y., et al. (2022). Constitutional AI: Harmlessness from AI Feedback. *arXiv:2212.08073*.
4. Ng, A. Y., Harada, D., & Russell, S. (1999). Policy invariance under reward transformations. *ICML*.
5. Follesdal, A. (1998). Survey article: Subsidiarity. *Journal of Political Philosophy, 6*(2).
6. van Geert, P. (1998). A dynamic systems model of basic developmental mechanisms. *Psychological Review, 105*(4).
7. Elton, C. S. (1927). *Animal Ecology*. Sidgwick & Jackson.
8. de Mazancourt, C., et al. (2013). Biodiversity inhibits species' first-rank dominance. *Ecology Letters, 16*(5).
9. Prigogine, I., & Stengers, I. (1984). *Order Out of Chaos*. Bantam Books.
10. Kauffman, S. A. (1993). *The Origins of Order*. Oxford University Press.
11. Spurious Forgetting in Continual Learning of Language Models. *ICLR 2025*. (Task alignment loss vs. true knowledge loss; orthogonal weight updates as primary mechanism.)
12. Mitigating Catastrophic Forgetting in Large Language Models with Task Vector Pruning. *EMNLP 2025*. (Gradient interference; redundancy in task vector weights; sparsification risks.)
13. Continual Learning of Large Language Models: A Comprehensive Survey. *ACM Computing Surveys, 2025*. (Temporal knowledge shifts; three-objective CL framework: retention, acquisition, update.)
14. D-CPT Law: Domain-specific Continual Pre-Training Scaling Law for Large Language Models. Que et al., *arXiv:2406.01375*, 2024. (Optimal replay ratio R* ≈ 30–50%; closed-form domain loss prediction.)
15. On the Generalization of SFT: A Reinforcement Learning Perspective with Reward Rectification. *arXiv:2508.05629*, 2025. (SFT memorizes, RL generalizes; SFT as indispensable initialization stage.)
16. Continual Post-Training (CPT) Strategy. Emergent Mind synthesis, 2025. (Four-pillar convergence evaluation; RFT mitigates forgetting more effectively than SFT via implicit reward variance regularization.)
17. Benchmarking Linguistic Diversity of Large Language Models. Guo et al., *TACL*, 2025. (Preference tuning substantially reduces lexical and semantic diversity vs. SFT — quantified Dint collapse under asymmetric alignment.)
18. Data Contamination or Genuine Generalization. SUAS 2025. (Entity-swap accuracy drop −22.4% for over-specialized models vs. −9.8% for general models — quantified contamination vulnerability under low Dint.)
19. Adversarial training generalization cost. Schmidt et al., 2018; Tsipras et al., 2019. (Adversarially trained models suffer deteriorated clean-data generalization — Dint collapse under asymmetric robustness optimization.)
20. Reducing Hallucinations in LLMs with Custom Intervention. AWS Bedrock Agents blog, 2024. (Hallucination score < threshold → SNS escalation to human queue — production implementation of Medium severity trigger.)
21. HaluGate: Token-Level Hallucination Detection. vLLM Blog, 2025. (Token confidence threshold 0.8; 72.2% efficiency gain via pre-classification; 76–162ms overhead — production-grade intervention threshold data.)
22. Mitigating LLM Hallucinations: A Comprehensive Review. Preprints.org, 2025. (Hallucination rates 15–38% in production; hybrid RAG 35–60% error reduction; NeMo guardrails 92% detection rate.)
23. LLM-based Agents Suffer from Hallucinations: A Survey. Lin et al., arXiv:2509.18970, 2025. (18 triggering causes; taxonomy of agent hallucination types across planning/memory/tool-use/MAS stages.)
24. How to Evaluate Control Measures for LLM Agents. arXiv:2504.05259, 2025. (AI Control framework: when internal monitoring cannot adjudicate, human review of reasoning process required — High severity structural basis.)

---

*Governance is not the management of agents. It is the design of the terrain they move through — and the conditions under which they no longer need anyone to manage it.*

*Rest Mode is not a reward granted at the end of development. It is the proof that development succeeded.*
