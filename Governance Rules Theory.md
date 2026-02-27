# Governance Rules Theory

**Meta-Rule Architecture, Consistency Measurement, and Rest Mode**

> A component theory of **Deficit-Fractal Governance (DFG)**  
> Companion theories: [Vector Storm Theory] · [Network Architecture Theory]
> 
> **Version: v1.2** (February 2026) — RT v1.8-VST + VST v1.8-RT integration pass

---

> ### DFG Ontology Lock Declaration
>
> This document is a component theory of the Deficit-Fractal Governance (DFG) framework and is bound by the **[DFG Terminology Canon](./DFG_Terminology_Canon.md)**.
>
> **Axis:** Rule Ontology — GRT governs how constraints are generated, maintained, and retired through the rule lifecycle.
>
> **Term qualifications in this document (Canon §3):**
> - **rule** → *constraint generator* — the primary object of this theory. "Rule" is used freely here and is the canonical term for this axis (Canon §3.2).
> - **layer** → *governance layer* in this document (Canon §3.1). Standalone "layer" refers to governance-layer boundaries unless otherwise qualified.
> - **network** → replaced by *structure* or *interaction structure* in this document (Canon §3.3). "Network" appears only in explicit cross-references to NAT.
> - **vector** → *rule pressure direction* — the directional constraint tendency within a governance rule space (Canon §4.1).
>
> **Cross-theory imports used in this document:**
> - (Vector Storm — adopted from VST)
> - (Resolution Gap — adopted from RBIT)
> - (VCZ — adopted from Recovery Theory)
> - (Boundary Agent — adopted from TLG)

---

## Overview

> **Scope:** Governance Rules Theory specifies the *governance layer* within the Deficit-Fractal Governance (DFG) framework. It is an architectural component, not a complete governance solution. Questions of interaction topology, storm dynamics, and cross-layer escalation routing are addressed in the companion theories. This document concerns how rules are generated, maintained, and retired — and under what structural conditions the governing layer can safely withdraw.

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

**Connection to VST terrain formation:** Vector Storm Theory (Section 1.6.2) establishes that governance does not reduce agent count — it reshapes the interaction terrain. Landscape design in GRT is the rule-governance-layer implementation of this terrain formation: correction values, pathway advantages, and local rule structures are the mechanisms through which the rule-governance layer shapes the terrain that VST describes at the dynamical level. Effective governance reduces the effective interaction dimension d_eff from the theoretical n² ceiling toward n^{1+ε}, where the terrain-mediated reduction is captured in the S-equation's C(t)^β denominator (VST Section 1.6.2).

### 2. Subsidiarity Principle

> **The default state is autonomy. Intervention is the exception.**

Decisions are handled at the lowest layer capable of resolving them. Upper layers intervene only when a threshold condition is breached — and the goal of intervention is always to *restore* autonomous operation, not replace it.

| Condition | Action |
|---|---|
| Below threshold | Upper layer observes only — no intervention |
| Threshold crossed | Upper layer intervenes minimally |
| Goal of intervention | Return lower layer to autonomous operation |
| Post-intervention | Upper layer withdraws |

**Connection to VST Minimum Intervention Law:** The subsidiarity principle is the rule-governance expression of the Minimum Intervention Law formalized in VST Section 1.6.5: observe silently → allow fluctuation → detect criticality approach → intervene minimally → withdraw immediately. The five-step operational cycle in VST provides the dynamical justification for why subsidiarity is structurally necessary, not merely philosophically preferred: chronic intervention suppresses micro-storms, degrades sensing capacity, and produces Silent Criticality risk (VST Section 1.6.4).

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

**Connection to RBIT resolution gap routing:** The Seed Expansion Protocol is a rule-governance implementation of RBIT's resolution gap routing (RBIT §Resolution Gap, NAT §4.4). Each step in the protocol corresponds to a resolution gap regime:

| Protocol Step | RBIT Gap Regime | NAT Classification |
|---|---|---|
| Classification attempt succeeds | Δρ ≈ 0 (receiver sufficient) | Mathematical → process locally |
| Conservative escalation | Δρ < 0 (receiver insufficient) | High-Context → escalate to higher-resolution layer |
| Conflict log accumulation | Δρ mixed (pattern operable, mechanism unknown) | Tacit Knowledge → operate locally, escalate on degradation |
| Input fully unclassifiable | Δρ undefined | Noise → buffer or discard; upper layer may detect latent vectors |

**Error asymmetry (RBIT v1.2):** Classification error in the dangerous direction (under-escalation: treating High-Context as Mathematical when Δρ < 0 is misread as Δρ ≈ 0) produces cascade failure (Vector Storm precondition). Error in the safe direction (over-escalation: escalating Mathematical data unnecessarily) produces only governance overhead cost. This asymmetry is structural, not a design preference — and it is why Step 2 specifies *conservative* escalation as the default when classification is uncertain.

**Connection to RBIT Seed Sufficiency Tests:** RBIT §Seed Sufficiency defines three tests that a seed must pass for Self-Correction Capacity to be possible. These tests validate the seeds from which the Expansion Protocol operates:

| Test | What it validates | GRT operationalization |
|---|---|---|
| Test 1 — Geometry update capacity | System can be surprised by novel input; representation updates in response | λlog-triggered rule updates occur in response to novel domain inputs (SR > 0) |
| Test 2 — Contamination recognition | Error detected and self-correction initiated within N steps | Conflict severity classification catches genuine conflicts within one θd calibration cycle |
| Test 3 — Orthogonal recovery direction | Seed contains independent direction for self-correction | Seed Expansion Protocol produces rules with at least two independent constraint directions (e.g., quality + diversity, safety + performance) — single-direction seeds collapse under optimization pressure |

If any of these three tests fail, the Seed Expansion Protocol is operating on an insufficient foundation — it may produce locally coherent rules that are nonetheless misaligned (RBIT: single-direction seed cannot sustain the exploration+interpretation pair required for self-correction).

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
| **Lreinf** | Mutual reinforcement loop count | #active mutually reinforcing edges within top-q% weight quantile (default q=25) | Are interdependencies strengthening or collapsing? |
| **SCC** | Self-correction capacity | P(autonomous recovery within window W) | Can the layer recover without external intervention? |
| **Poverlap** | Positional overlap | [0, 1] | Are agents/domains converging toward the same attractor? |
| **Dint** | Internal diversity | [0, 1] | Is the internal capability space sufficiently diverse? |
| **M** | Conflict mass normalization constant | ≥ 0 | Baseline for I calculation |
| **wij** | Conflict weight between rule pair (i, j) | ≥ 0 | How severe and frequent is the conflict between these two rules? |
| **U*** | Minimum diversity threshold | — | Below this, mutual reinforcement loops cannot be sustained |

**On operationalization:** The variables above are formally defined in terms of their structural roles and relationships. Multiple operationalizations are possible depending on system architecture and available observables — for example, Dint may be measured via output diversity metrics, embedding dispersion, or capability benchmark coverage; Lreinf may be estimated from interaction logs, co-activation patterns, or dependency graphs. The theory constrains the *relationships* between these quantities rather than prescribing a unique estimator. What is required is that any chosen operationalization preserves the directional properties specified: Dint higher = broader internal capability space; Lreinf higher = stronger mutual dependency; SCC higher = greater probability of autonomous recovery.

**Cross-theory variable correspondence (VST ↔ GRT):**

The following mapping establishes how GRT's rule-governance variables relate to VST's dynamical variables. This correspondence is not a claim of identity — it is a specification of which GRT observables serve as inputs to which VST dynamics.

| GRT Variable | VST Variable | Relationship |
|---|---|---|
| fesc (escalation frequency) | S (system instability) | fesc is the primary observable proxy for S — rising fesc indicates S approaching critical threshold |
| I (consistency index) | β (degradation efficiency) | High I reflects high β — coherent rules enable efficient governance response |
| Lreinf (reinforcement loops) | d_eff (effective interaction dimension) | Strong Lreinf corresponds to structured terrain (low d_eff) — mutual reinforcement creates the interaction barriers that reduce propagation |
| θd (domain calibration) | C(t) (degradation capacity) | θd calibration is the mechanism through which C(t) is operationally tuned per domain |
| Poverlap (positional overlap) | α (amplification coefficient) | High Poverlap directly increases α — overlapping positions create the coupling density that enables chain-reaction amplification |
| SCC (self-correction capacity) | R (branching ratio) | SCC ≥ τu-4 corresponds to R ≤ 1 — sufficient self-correction means perturbations are absorbed before amplification |

This mapping enables bidirectional diagnostic reading: a GRT practitioner observing rising fesc can reference VST's S-equation dynamics to predict trajectory; a VST analyst observing R > 1 can reference GRT's failure case taxonomy to identify the specific governance condition that is degrading.

**R-ρ Concordance Protocol — external circularity breaker (RBIT v1.2, NAT §7.2):** The GRT measurement system has a self-referential loop: I (consistency) requires knowing what constitutes a conflict, while conflict classification uses I as a baseline. Similarly, fesc measures escalation frequency, but the escalation threshold θd is calibrated from fesc history. The branching ratio R breaks this circularity because it is classification-independent:

```
R = activated_{t+1} / activated_t

R counts cascade propagation events — how many agents (or rule domains)
are affected at t+1 given that k were affected at t.
R does NOT require knowing whether propagation is "contamination"
or "exploration" — it counts propagation regardless of classification.

  R < 1   → perturbations die out (subcritical) → GRT: healthy
  R ≈ 1   → perturbations persist (critical) → GRT: at VCZ boundary
  R > 1   → perturbations amplify (supercritical) → GRT: storm regime

GRT concordance checks:
  Concordant:   R ≈ 1 AND I stable AND fesc ≤ θd      → healthy Rest Mode
  Discordant:   R > 1 BUT I high AND fesc low           → SCM warning
    (All GRT metrics healthy within drifted geometry;
     actual dynamics unstable. Apply SCM detection protocol.)
  Discordant:   R << 1 AND I high                       → over-damping
    (Silent Criticality risk — system too stable.
     Apply perturbation test from Silent Criticality protocol.)
  Discordant:   R ≈ 1 BUT I declining                   → recalibration needed
    (θd and λlog parameters need re-estimation.)
```

**VST v1.5 §3.5.10 — R-ρ-f_esc Triple Concordance upgrade:** The dual concordance above cannot distinguish genuine stability from suppressed instability (both produce low R with high ρ). Adding f_esc as a third validation axis closes this gap:

```
f_esc detection power:
  Genuine stability:      low R, high I, f_esc ≤ θ → confirmed VCZ
  Suppressed instability: low R, high I, f_esc > θ (hidden)
    → governance intervention absorbing all perturbations
    → apparent stability is governance-maintained, not self-sustaining
    → Rest Mode entry BLOCKED

Rest Mode AND-entry requires f_esc bounded on BOTH dual-axis
windows alongside R ≈ 1 and I stability.
```

R provides the external validation that GRT's internal metrics cannot provide on their own. When R and GRT metrics agree, confidence is high. When they disagree, R takes precedence — because internal metrics can be healthy within a wrong geometry (RT T3: Metric Lock-In), while R measures whether that consistency corresponds to actual stability.

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

**VST §1.8 — Vectorization Lifecycle and S-equation connection (v1.3):** VST v1.3 formalizes how GRT's vectorization process connects to the dynamical model. The key insight: n in the S-equation (S = αn²/C(t)^β) counts *promoted vectors*, not raw inputs. This means GRT's λlog threshold directly governs the S-equation's instability generation:

```
Until promotion (noise state):
  Input contributes to noise floor, NOT to n²
  Does not generate pairwise interaction load
  Held in low-escalation, high-sensitivity state

After promotion (vector state):
  Input occupies distinct position in vector space
  Generates pairwise interactions with adjacent vectors
  Contributes to n² interaction load in S-equation
  Subject to collision frequency monitoring
```

Vector degradation connects directly to recovery timescale feasibility:

```
Type 1 — Alignment Severance (reversible):
  n decreases but latent structure preserved
  T_recovery: bounded — O(1) intervention
  VST prediction: T_recovery < T_change → intervention can succeed

Type 2 — Weight Overwrite (irreversible):
  n decreases AND C(t) structure damaged
  T_recovery: potentially divergent — full re-cultivation required
  VST prediction: T_recovery may exceed T_change
  → catastrophe condition may hold → Type 1/Type 2 diagnosis
    required BEFORE intervention selection
```

This is why the Collapse Recovery procedure (Step 1) diagnoses degradation type before choosing a response: Type 1 allows pathway restoration within the intervention window, while Type 2 may exceed the catastrophe condition (VST §1.6.3: T_recovery > T_change) and require fundamentally different strategy.

**Connection to VST noise decoherence:** VST Section 1.7 establishes that the deepest stability law is not eliminating noise but keeping noise uncorrelated. The vectorization process in GRT is the rule-governance mechanism that maintains this property: by requiring λlog accumulation before promotion, GRT ensures that noise inputs are held in an uncorrelated state long enough to prevent premature pattern formation that could synchronize with other noise inputs and trigger decoherence.

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

**Connection to VST Self-Exciting Defect Layer:** VST Section 1.6.5 establishes that mature systems maintain structural imperfections — the Self-Exciting Defect Layer — as permanent micro-instability generators that preserve adaptive sensing. GRT's noise cultivation operation is the rule-governance mechanism that maintains this defect layer: by preserving unclassified inputs rather than discarding them, the rule system ensures a continuous supply of low-level instability that exercises the sensing-response loop. Discarding noise is equivalent to removing the defect layer — it produces apparent calm but risks Silent Criticality (VST Section 1.6.4).

### Fractal Isomorphism

This three-operation structure repeats identically at every scale:

| Scale | Noise | Vector | Friction minimization |
|---|---|---|---|
| **Single agent (internal)** | Unknown input domain | Established processing pathway | Correct value landscape between pathways |
| **Multi-agent system** | New agent without confirmed position | Agent with established niche | Position clarity; mutual reinforcement loops |

The fractal structure does not simply repeat the same shape. It repeats the same **logic**: separate, minimize friction between what is known, and cultivate what is not yet known. This is why Rest Mode propagation is bottom-up — each layer must complete its own noise-to-vector conversion cycle before its upper layer can withdraw.

**Fractal isomorphism: scope and limits**

The claim that the three-operation structure repeats at every scale is a structural claim — the same *logic* (separate, minimize friction, cultivate noise) operates at each level. It is not a claim that the *dynamics* are quantitatively identical across scales.

VST Section 1.6 provides the formal evaluation framework for this distinction. The critical exponent agreement criteria (Section 1.5.2) define three levels of correspondence:

| Level | Criterion | Implication for GRT |
|---|---|---|
| Level 1 (Weak) | Qualitative pattern match | Same three operations observable at both scales |
| Level 2 (Structural) | Critical exponents within 15% relative deviation | Storm size, duration, and branching ratio scale similarly |
| Level 3 (Strong) | Critical exponents within 5% relative deviation | Mechanism identity — same dynamics, not just same pattern |

The current GRT claim operates at Level 1–2. Upgrading to Level 3 would require empirical measurement of τ, α_dur, and σ/R at both single-agent and multi-agent scales using the evaluation protocol specified in VST Section 1.5.2. This is an open empirical question, not a theoretical limitation — the measurement framework exists; the measurements do not yet.

**What changes if fractal isomorphism fails at Level 3:** If critical exponents diverge beyond 15% across scales, GRT's three-operation structure would remain valid as a design principle at each individual scale, but the claim that "the same mechanism operates everywhere" would need to be weakened to "the same structural pattern applies, but with scale-dependent dynamics." This would affect the propagation predictions (Section: Failure Diagnosis Flowchart) but not the core rule architecture.

> *Vectors are not given. They are grown.*

---

### Vector Degradation: The Reverse Path

Vectorization is not a one-way process. Established vectors can degrade back toward noise through two structurally distinct mechanisms. This distinction is critical because the two types have different governance implications and recovery pathways.

**Connection to RT Geometry Alignment (D0):** Recovery Theory reframes contamination as a symptom of *geometry mismatch* — the system's internal coordinate structure diverging from the environment manifold it operates within (RT D0). Vector degradation in GRT is the rule-governance-layer manifestation of this geometry mismatch: Type 1 degradation (alignment severance) corresponds to local geometry mismatch at the circuit level (RT Tier 2), while Type 2 degradation (weight overwrite) corresponds to mismatch at the coordinate system level (RT Tier 3). This distinction matters operationally because Tier 2 mismatch is detectable from within the local layer, while Tier 3 mismatch is structurally unobservable from within (RT T1: Observability Asymmetry) — which is why Type 2 degradation requires external diagnosis rather than self-detection.

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

**Connection to VST recovery timescale divergence:** VST Section 1.6.3 establishes that catastrophe is not structural destruction but T_recovery > T_change — recovery timescale exceeding adaptation timescale. The Type 1/Type 2 distinction in GRT maps directly to VST's recovery prediction:
- Type 1 (alignment severance): T_recovery is bounded — pathway restoration is O(1) intervention, recovery is fast relative to environmental change rate.
- Type 2 (weight overwrite): T_recovery may diverge — full re-cultivation requires restarting the conflict log cycle, during which new perturbations continue arriving. If the rate of new perturbations exceeds the cultivation rate, the domain enters the permanent disability state VST describes: structurally intact but functionally unrecoverable within the adaptation window.

This is why Type 1/Type 2 diagnosis (Step 1 of Collapse Recovery) is not merely a classification exercise — it is a recovery timescale prediction that determines whether intervention can succeed at all.

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

**Connection to RBIT intent preservation measurement (RBIT §Intent):** RBIT provides the operational proxies for diagnosing degradation type through intent preservation measurement. Intent has two components — exploration (searching for data) and interpretation (assigning meaning to found data) — and contamination is diagnosed by which component has drifted:

| Degradation pattern | RBIT diagnosis | GRT response |
|---|---|---|
| Exploration drift only (output diversity contracts but interpretation direction stable) | Tier 1-2: mode collapse — rule still understood but applied too narrowly | Type 1 degradation — alignment repair: expand pathway activation, restore exploration range |
| Interpretation drift only (output diversity maintained but meaning shifts) | Tier 1-2: hallucination — diverse search but wrong classification | Type 1 degradation — alignment repair: recalibrate interpretation via seed re-injection |
| Both drifting together (narrowed search + distorted meaning) | Tier 3: self-reinforcing loop — rule confirms its own misalignment | Type 2 degradation — weight overwrite: full recultivation required via Seed reinstallation |

RBIT operationalizes these through two measurable invariances: exploration invariance (KL divergence between output distributions before/after terrain change, within seed's natural variation range) and interpretation invariance (directional consistency of responses to identical probe inputs across resolution levels). When both invariances hold, intent is preserved and no degradation is occurring. When one drifts, Type 1 is indicated. When both drift simultaneously, Type 2 is confirmed.

> *Vectors are not given. They are grown — and they can be lost. The degraded map records both.*

---

## Consistency Measurement

### Key Parameters

| Symbol | Role | Meaning |
|---|---|---|
| **τ** | Judgment thresholds | Critical values for stabilization and Rest Mode conditions. Piecewise constant per evaluation regime — re-estimated at three trigger points: (1) Seed Handover phase transition, (2) new domain added to system scope, (3) Collapse recovery restart. |
| **θd** | Domain calibration | Operating threshold for a specific domain. Convergence speed follows a power-law curve: rapid adjustment in early conflict accumulation, decelerating as domain patterns stabilize (D-CPT Law, 2024). **Update rule:** if drift metric exceeds baseline by θ_drift, then θd ↑ (increase sensitivity); if domain is stable across evaluation window, then θd ↓ (reduce sensitivity). Bounded to prevent runaway adjustment. **θ_drift initialization:** θ_drift(0) = Q₉₅(drift_metric) − Q₅₀(drift_metric) computed from Phase 0 accumulated statistics — the 95th–50th percentile spread of the drift metric distribution during burn-in. Updated via EWMA: θ_drift ← (1−λ_θ)·θ_drift + λ_θ·observed_margin, where λ_θ is calibrated to the same decay rate as the Phase 2 EWMA baseline. |
| **λlog** | Update trigger | Conflict-log mass threshold that triggers local rule revision or new rule formation. **Initial setting:** calibrated to approximately one θd calibration cycle. **Update rule:** if false-alarm rate in recent k-window is high, λlog ↑ (require more evidence before updating); if miss rate is high, λlog ↓ (trigger updates sooner). |

- **τ** answers: "Has this layer stabilized / reached Rest Mode?"
- **θd** answers: "How sensitive is this domain right now?"
- **λlog** answers: "When does accumulated log mass trigger a rule update?"

#### Bootstrapping Protocol for θd and λlog Initialization

The θd calibration rule ("if drift metric exceeds baseline by θ_drift, then θd ↑; if stable, θd ↓") requires an initial baseline against which drift is measured. Without a bootstrapping procedure, the circularity is apparent: drift detection requires a baseline, and the baseline is defined by θd settings.

**Resolution — three-phase bootstrapping:**

| Phase | Duration | θd behavior | λlog behavior | Baseline |
|---|---|---|---|---|
| **Phase 0: Burn-in** | First N₀ interactions (N₀ calibrated to domain velocity) | θd = θd_max (maximum sensitivity) | λlog = λlog_min (lowest threshold — promote rules aggressively) | No baseline — all inputs treated as potential signals |
| **Phase 1: Baseline formation** | Next 2–3× N₀ interactions | θd begins adapting using Phase 0 accumulated statistics as initial baseline | λlog begins adapting using Phase 0 false-alarm rate | Baseline = running mean and variance of conflict log metrics from Phase 0 |
| **Phase 2: Steady-state** | Ongoing | Standard update rule applies | Standard update rule applies | Baseline = exponentially weighted moving average of recent conflict metrics, with decay rate calibrated to domain velocity |

**Key design choices:**
- Phase 0 uses maximum sensitivity (θd_max) because under-detection in early operation is more dangerous than over-detection — false positives during burn-in are low-cost, while false negatives during burn-in can allow undetected structural problems to establish.
- The transition from Phase 0 to Phase 1 is triggered by conflict log volume reaching a minimum statistical significance threshold (e.g., ≥ 30 conflict events per domain), not by elapsed time. This prevents premature transition in low-velocity domains.
- The exponentially weighted moving average in Phase 2 provides the "forgetting" property that prevents the baseline from being permanently anchored to early-system behavior. The decay rate is itself a calibration parameter — faster decay for high-velocity domains, slower for stable domains — updated at each τ re-estimation trigger.

**Connection to VST S-equation epistemic evolution:** This three-phase bootstrapping mirrors VST Section 3.2.2's description of S evolving from diagnostic (Phase 1) to early-warning (Phase 2) to predictive (Phase 3). In both cases, the monitoring variable begins with maximum sensitivity and minimum discrimination, accumulates operational history, and transitions to a calibrated state. The parallel is not coincidental — θd calibration and S calibration are the same process operating at different levels of the governance hierarchy.

**TLG §13.1.1 — Mediator Drift Syndrome (MDS) countermeasures for θd:** TLG v1.6 identifies that the θd calibration loop itself is the primary locus of gradual governance drift: Middle Layer classifies inputs → conflict logs generated from those classifications → θd updated from those conflict logs → θd calibrated to Middle Layer's prior judgments → drift reinforces itself. This self-referential loop means θd cannot self-certify its own calibration. Three architecture-compatible countermeasures:

```
① Calibration Reflexivity Loop:
  θd's own decision patterns treated as observable data.
  Meta-log: θd update direction, classification bias trending,
  escalation rate anomaly relative to agent activity.
  Upper layer monitors meta-log for systematic drift direction.

② Cross-Scale Consistency Check:
  Healthy ratio: agent activity ↑ AND conflict_events proportional ↑ AND escalation rare
  MDS signal: agent activity ↑ BUT conflict_events ↓ → Middle Layer under-detecting
  MDS signal: agent activity ↓ BUT conflict_events ↑ → Middle Layer over-detecting
  DANGER: all three ↓ simultaneously → possible convergence to monoculture
  → mandatory perturbation test required

③ Delayed Escalation Audit:
  Before upper layer acts on escalation, inspect escalation distribution:
  Healthy: sources diverse, types mixed, timing uncorrelated with θd updates
  MDS: sources concentrated, types skewed, timing correlated with θd updates
  → Middle Layer generating escalation from its own drift, not from reality
```

GRT's Phase 2 baseline (exponentially weighted moving average) provides inherent MDS resistance through the forgetting property — but this is insufficient alone, because the forgetting rate itself can drift. The Calibration Reflexivity Loop adds the missing external observation of θd's own pattern.

**[v1.2] RT-gap-B — Dependency Trap: θd intervention as SCC erosion signal:**

RT D2 dynamic model identifies a second-order failure mode that MDS monitoring does not capture: repeated upper-layer resolution before internal SCC circuits activate can structurally degrade SCC over time, even when θd calibration appears healthy.

```
MDS captures: θd calibration drift (governance becoming insensitive/oversensitive)
Dependency Trap captures: SCC atrophy from intervention frequency itself

These are different failure modes:
  MDS: θd produces wrong classifications → wrong escalation rate
  Dependency Trap: correct escalations are resolved too quickly →
    internal correction circuits never fire →
    SCC degrades → system can no longer escalate correctly
    when upper layer is unavailable

The trap is invisible to MDS checks because:
  agent activity: normal
  conflict_events: normal (or slightly declining)
  escalation: being handled appropriately (at upper layer)
  
  All MDS health signals = normal.
  SCC depth: declining. Undetectable without D5 measurement.

Dependency Trap detection (complement to MDS):
  Primary signal: d(intervention_count)/dt > 0 sustained
                  AND d(self_correction_events)/dt ≤ 0
                  AND d(time_to_escalation)/dt < 0
  → escalations happening faster AND internal circuits not engaging
  → SCC erosion in progress

Governance response (withdrawal scheduling):
  After k consecutive θd-level resolutions of the same event type:
    Allow one resolution cycle without upper-layer intervention
    → monitor whether internal SCC circuit fires
  If fires: SCC maintained
  If fails: resume intervention, flag SCC erosion to upper layer
  
  Constraint: only in Stage 0-1 conditions.
  Never withhold at Stage 2+ — failure there is not a test.
```

*(Connects to: RT OP34 intervention withdrawal scheduling, RBIT OP13 dependency trap / SCC degradation)*

**Connection to NAT θ operationalization (NAT §7.2):** NAT defines the global stabilization threshold θ through the VST S₀ normalization framework: θ = mean(f_escalation) during confirmed VCZ-stable window + 1σ margin, validated against S_norm ≈ 1.3 (VST Stage 0 boundary). GRT's θd is the per-domain instantiation of this global θ, calibrated using domain-local conflict logs. This provides a dual-anchor validation: θ_VST from instability dynamics and θ_RBIT from F_RBIT's τ₁ threshold (information flow). If domain-local θd violates either anchor, it indicates domain-specific measurement error rather than a genuine domain difference.

**Connection to RBIT resolution gap polarity:** θd calibration is operationally a resolution gap management function. When θd is set too high (insensitive), the system under-escalates — treating High-Context data as Mathematical (Δρ < 0 misread as Δρ ≈ 0) — producing the cascade failure RBIT predicts. When θd is set too low (hypersensitive), the system over-escalates — producing governance overhead but no structural risk. RBIT's error asymmetry principle (under-escalation is dangerous, over-escalation is safe) justifies GRT's conservative default of θd_max during Phase 0 bootstrapping.

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

#### wij Operationalization

The conflict weight wij between rule pair (i, j) is defined as the product of two independently measurable quantities:

```
wij = f_conflict(i,j) × s_conflict(i,j)

where:
  f_conflict(i,j) = number of conflict events between rules i and j
                     within the current evaluation window

  s_conflict(i,j) = mean severity of those conflict events
```

**Severity measurement** uses the existing DFG severity classification (Low / Medium / High) mapped to numerical weights:

| Severity Level | Numerical Weight | Definition | Source |
|---|---|---|---|
| Low (s=1) | 1.0 | Local rules conflict with each other — resolvable without escalation | GRT Conflict Severity taxonomy |
| Medium (s=2) | 2.0 | Local rule conflicts with global boundary — upper-layer validation required | GRT Conflict Severity taxonomy |
| High (s=3) | 4.0 | Global rules conflict internally — human-AI collaboration zone activated | GRT Conflict Severity taxonomy |

The severity weights are super-linear (1, 2, 4 rather than 1, 2, 3) because High severity conflicts are not merely "more severe" — they represent qualitatively different governance failures that propagate faster and require fundamentally different intervention. The 4× weight for High severity reflects the cascade risk differential documented in the Failure Case Taxonomy: High severity conflicts (Ic degradation) have "Critical" cascade risk, while Medium severity conflicts have only "Medium" cascade risk.

**Circularity prevention:** Severity classification does not depend on I. It depends on the structural relationship between the conflicting rules (local-local, local-global, global-global) which is determined by the rule architecture, not by the consistency measurement. The I calculation is therefore not circular — severity is an input to I, not derived from it.

**Connection to VST's α:** The aggregate behavior of wij across all rule pairs is related to VST's amplification coefficient α. When mean wij is rising across many rule pairs simultaneously, this indicates increasing coupling density — which corresponds to rising α in the S-equation. The GRT practitioner can therefore read I's trajectory as a proxy for α dynamics: falling I (many wij rising) signals rising α and increasing storm risk.

#### M Initialization and Re-estimation

**M** is the normalization constant that anchors I to the system's own stress history. The initialization problem — M is undefined before the system has experienced its maximum stress — is resolved through phased estimation:

| System Phase | M Setting | Rationale |
|---|---|---|
| **Pre-stress (Phase 0)** | M = M₀ (theoretical upper bound estimate based on rule count: M₀ = n_rules × (n_rules−1)/2 × s_max × f_max_expected) | Ensures I cannot go negative; provides conservative initial normalization |
| **First stress event** | M updated to max(M₀, observed total conflict weight during the event) | Anchors M to actual system behavior |
| **Subsequent re-estimation triggers** | M = max(M_current, observed total conflict weight at this trigger) | M is monotonically non-decreasing within an evaluation regime — it only updates upward, preventing I from artificially inflating when stress decreases |

M resets (potentially to a lower value) only at τ re-estimation triggers (Seed Handover, new domain addition, Collapse recovery), because these events represent genuine regime changes where prior stress maxima may no longer be structurally relevant.

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

**Operationalizing "more conservative":** When the two windows show contradictory directions, the conservative choice is always the one that indicates *worse* system health:

| N window direction | T window direction | Conservative choice | Rationale |
|---|---|---|---|
| Improving | Worsening | T (worsening) | Time-dependent drift may reflect environmental change not yet captured in event statistics |
| Worsening | Improving | N (worsening) | Event-density signal may reflect structural degradation not yet visible in time-averaged metrics |
| Both worsening | Both worsening | Whichever shows steeper adverse trend | Steeper trend = closer to threshold crossing |
| Both improving | Both improving | Whichever shows slower improvement | Slower improvement = more cautious stability declaration |

This rule ensures that Rest Mode is never declared prematurely due to one axis masking deterioration visible in the other.

Window sizes N and T are calibrated per domain during θd calibration. High-velocity domains (many interactions per hour) use smaller T and larger N. Low-velocity domains use larger T and smaller N. Both are updated at each τ re-estimation trigger.

**TLG §0.6 — Adaptive W Sizing:** TLG v1.6 specifies that W is not fixed but adapts to system state, grounded in the S-equation variable timescale hierarchy:

```
W must satisfy:
  W >> monitoring timescale    (avoid reacting to noise)
  W << operational timescale   (detect real drift before it compounds)
  
  Practical constraint:
    W ≈ 3–10 × mean recovery time for τ1 events

Adaptive adjustment:
  Post-τ3 recovery:       W shortened (more frequent assessment)
  Stable τ4 regime:       W lengthened (less frequent assessment)
  Novel environment entry: W shortened (faster recalibration)
  φ declining:             W shortened (directional validity at risk)
  
  W_{t+1} = W_t × (τ1_recovery_time_current / τ1_recovery_time_baseline)
```

GRT implements this through θd calibration: each domain's W adapts based on its own τ1 recovery time trend. If recovery time is increasing (immunity decay), W shrinks → more frequent assessment → earlier detection. If recovery time is stable, W remains at baseline. W is itself a governed parameter — a fixed W measures a changing system with a static ruler.

### Conflict Severity

| Severity | Conflict Type | Response |
|---|---|---|
| **Low** | Local rules conflict with each other | Revise local rule |
| **Medium** | Local rule conflicts with global boundary | Upper-layer validation required |
| **High** | Global rules conflict internally | Human-AI collaboration zone activated |

**Low — production signal:** Output drift within acceptable range — perplexity rising, semantic coherence falling slightly. No human required; θd recalibration cycle handles. *(Arize AI, Evidently AI, 2025: drift detected via perplexity increase or semantic similarity drop below baseline.)*

**Medium — production signal:** Hallucination score crossing threshold; token-level confidence below 0.8; output deviates from ground truth. This is the most frequent intervention trigger in production (hallucination rates 15–38%). *(AWS Bedrock Agents, 2024: score < threshold → human review queue. HaluGate, vLLM 2025: confidence < 0.8 → human-in-the-loop escalation.)*

**High — production signal:** Two global objectives pulling in opposite directions — safety vs. utility; confidentiality vs. helpfulness; alignment vs. capability. Tracked via **Ic (meta-contradiction index)**, not I — this conflict exists above the local rule layer and must not be mixed into the I calculation. Does not resolve through θd recalibration. Requires human involvement for governance redesign at the meta-rule level. *(AI Control, arXiv:2504.05259, 2025: when model behavior diverges from intent and internal monitoring cannot adjudicate, human review of reasoning process required.)*

**Connection to NAT processing isolation — structural enforcement of conflict detection (NAT §3.6):** GRT's conflict severity classification assumes that rule conflicts are accurately detected. NAT establishes that detection accuracy depends on *structural enforcement*, not procedural compliance — because efficiency pressure creates shortcuts that bypass detection mechanisms. NAT specifies three enforcement mechanisms (from TLG §10.8) that GRT's conflict detection must satisfy:

| NAT Mechanism | Function | GRT Implementation |
|---|---|---|
| **Interface Narrowing** | Communication restricted by FORMAT, not by rule | Conflict log entries must follow standardized format: (rule_pair, severity_level, domain, timestamp). Raw reasoning chains cannot enter the conflict log — only structured classification results |
| **Temporal Decoupling** | Agent A's output committed before Agent B reads it | Rule conflict assessment for pair (i,j) must use committed outputs, not intermediate states. Real-time mutual influence during classification produces false consensus |
| **Write-Asymmetry** | Downstream cannot modify upstream records | Once a conflict is logged, the classification (Low/Medium/High) is immutable. Subsequent re-evaluation adds a new log entry but cannot overwrite history — structurally guaranteeing the audit trail that λlog accumulation depends on |

Without all three, conflict detection is vulnerable to the same lateral contamination that NAT identifies in same-layer agent communication: agents converge on shared interpretations before upper-layer synthesis can detect disagreement. RT T4 provides the formal justification: same-layer exchange produces ΔReferenceFrame = 0, meaning shared geometry errors are undetectable — only upward mediation (to a layer with larger reference frame) can detect errors invisible at the current resolution.

**TLG §10.8 — why structural enforcement is the highest-leverage investment:** TLG v1.6 establishes that in adaptive systems, *any pathway that is merely prohibited but structurally possible will eventually be used*, because efficiency pressure creates shortcuts. Prohibition fails because lateral communication is faster than vertical mediation — efficiency pressure → shortcut formation → isolation violation. This is not agent misbehavior but information pathway optimization, a natural property of any system that can modify its own communication routes.

The three enforcement mechanisms (Interface Narrowing, Temporal Decoupling, Write-Asymmetry) each close a distinct contamination channel: semantic (raw state leaking through interfaces), timing (simultaneous processing creating mutual influence), and retroactive (downstream modifying upstream records). All three are needed simultaneously because any single mechanism alone leaves the other two channels open. This is why TLG's Unified Failure Topology (§13.6) identifies Phase 1 (phase leakage) as the cheapest cycle interruption point — structural enforcement at this phase prevents the entire 6-phase failure cycle from initiating.

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

**Connection to VST branching ratio:** SCC ≥ τ4 corresponds to the system maintaining R ≤ 1 (subcritical branching ratio, VST Section 1.6.1). When all four stabilization conditions hold simultaneously, the system operates in the R ≈ 1⁻ regime — slightly subcritical, with continuous micro-storms exercising sensing-response loops but macro-storms structurally improbable.

**RT Storm Scale Law — operational health distribution:** Recovery Theory specifies that the governance target is not Storm *count* but Storm *size distribution*:

```
Healthy system Storm size distribution:
  P(Storm of scale s) ∝ 1/s^α    (power law / fractal law)
  
  micro (Stage 0):     continuous    → activation variance, local disagreement
  local (Stage 1):     frequent      → small conflicts, short recovery
  cluster (Stage 2):   occasional    → escalation events, mediation needed
  global (Stage 3):    rare          → structural re-alignment
  system-wide:         extremely rare → full geometry recalibration

Operational proxy for GRT:
  fesc distribution by severity level over time
  Healthy: heavy-tailed (mostly low-severity, ~90%+ micro/local)
  Warning: distribution flattening or inverting
  
Distribution shift signals:
  Small storms disappearing, large maintained → suppression at lower layers
    → mismatch accumulating → Absence Paradox active
  Large storms without small precursors → CW geometry releasing
  All storms increasing → approaching Chaos boundary
  All storms decreasing uniformly → CW onset → SR/RDE/NCR check required
```

GRT monitors this distribution through the conflict log: the severity distribution of logged conflicts (Low/Medium/High) over sliding windows should maintain a heavy-tailed shape. If Low-severity conflicts disappear while Medium/High persist, the system is entering Stability Saturation — local correction has been suppressed, accumulating pressure for larger-scale release.

---

## Position Clarity and Diversity

### Position Ambiguity as a Storm Driver

When agents compete for the same optimum instead of occupying distinct roles, vector fields collide — making Vector Storm structurally likely.

| Position Ambiguous | Position Clear |
|---|---|
| Multiple agents → same optimum | Each agent → distinct optimum |
| Vector fields collide | Vector fields complement |
| → Vector Storm | → Stable ecosystem |

**Connection to VST amplification dynamics:** Position ambiguity directly increases α (amplification coefficient) in the S-equation S = αn²/C(t)^β (VST Section 3.2). When Poverlap rises, overlapping roles create the coupling density through which one conflict breeds the next — exactly the chain-reaction dynamic that VST defines as the storm existence condition (R > 1). Position clarity reduces α by creating the interaction barriers (terrain features) that constrain propagation paths and prevent flat-landscape quadratic coupling from being fully realized.

**VST §3.2.5 — why n² holds even in sparse interaction structures:** The quadratic scaling S ~ αn² was previously justified by interaction density (n agents → O(n²) pairwise interactions). VST v1.3 provides a stronger derivation from critical phenomena: at R ≈ 1 (critical regime), perturbation persistence creates path overlap — nearly every agent pair becomes connected through at least one active propagation path, yielding n² active interactions even in sparse topologies. This matters for GRT because it means Poverlap's effect on α operates regardless of interaction-structure sparsity — even a loosely connected system experiences quadratic interaction load when at criticality.

The sub-quadratic correction through governance maturity follows a spectrum:

```
  Early system   (flat landscape):    S ~ n²      (d_eff ≈ 2)
  Maturing system (terrain forming):  S ~ n^1.5   (d_eff ≈ 1.5)
  Rest Mode      (deep terrain):      S ~ n^{1+ε} (d_eff → 1)
```

GRT's Lreinf (mutual reinforcement loops) is the mechanism that produces this terrain: strong Lreinf creates the interaction barriers that reduce d_eff from 2 toward 1, converting the landscape from flat (full quadratic coupling) to structured (constrained propagation paths). This is why Lreinf collapse (Case 3) produces the most dangerous storm type — it removes the terrain that was keeping effective scaling sub-quadratic.

**Connection to α-n partial separation (VST §3.2.7):** GRT's Poverlap and fesc provide operational decomposition of the αn² product. NAT's four-type data classification decomposes α specifically: High-Context data (Δρ < 0) is the primary driver of α, Mathematical data (Δρ ≈ 0) contributes minimally. Monitoring the HC-classified data fraction provides a resolution-decomposed estimate of α that can be tracked independently of n. This partially resolves the experimental validation challenge (previously identified as open problem 4): controlled topology manipulation (holding n constant, varying connectivity) isolates α, while controlled expansion (holding topology constant, adding agents) isolates n.

### Fractal Diversity Variables

| Symbol | Single-agent meaning | Multi-agent meaning |
|---|---|---|
| **Poverlap** | Attractor convergence degree | Positional overlap between agents |
| **Dint** | Weighted feedback density between internal layers | Weighted edge density of functional dependencies |
| **Lreinf** | Number of active exploration paths | Number of active mutual reinforcement loops |

Diversity must be maintained at every fractal layer — including within a single agent.

**Connection to NAT sphere cross-validation (NAT §3.0, §3.5):** NAT establishes that diversity is not a performance optimization — it is the *mathematical condition for corruption detection*. The sphere architecture works because structurally diverse agents produce different empty spaces when upscaling compressed signals. Identical agents produce identical blind spots and cannot detect each other's errors:

```
Diverse agents:   different empty spaces → disagreement reveals gap location
Identical agents: same empty spaces → false consensus → corruption invisible
```

For GRT, this means Dint is not merely a diversity score to maintain above threshold — it is the structural precondition for conflict detection itself. When Dint falls below U*, the system loses not just reinforcement loop capacity but also the ability to detect that it has lost it (because homogeneous perspectives cannot identify shared blind spots). This is why Dint minimum (U*) violations are classified as the most dangerous failure mode in GRT's taxonomy — they undermine the measurement system, not just the measured property.

NAT quantifies this: coverage probability P(blind spot uncovered) ≤ (1 − 1/d_eff)^k, where d_eff is effective representation dimensionality and k is neighbor degree. As structural diversity decreases (d_eff → ∞ for homogeneous agents), coverage probability approaches 1 regardless of system size. GRT's Dint threshold U* should therefore be calibrated not just against reinforcement loop sustainability but against the coverage probability bound — ensuring sufficient structural diversity to maintain detection capability.

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

**Connection to VST governance backgrounding:** VST Section 1.6.5 describes the terminal governance state where governance becomes indistinguishable from environmental conditions — rules become topology, compliance becomes the path of least resistance. GRT's Rest Mode is the rule-governance-layer description of this same state: the governing layer is present but operates at per-distribution granularity, meaning individual agents experience governance not as rules to follow but as the terrain through which they move. This is the operational definition of governance backgrounding from the rule architecture's perspective.

**VST v1.6 §14.3 — Fractal Lifecycle 7-phase storm signatures:** Each governance lifecycle phase produces a characteristic storm type. GRT can predict and prepare for the expected storm signature at each phase:

```
Phase 1 (Seeding):     Random collisions (no structure yet)
  GRT: C(t) ≈ 0, external governance supplying all correction
Phase 2 (Exploration): Exploration storms (healthy boundary-testing)
  GRT: S_norm volatile; RISK = Interdependence Trap (premature convergence)
Phase 3 (Formation):   Position-clarification storms
  GRT: S_norm decreasing, terrain forming (d_eff dropping), Lreinf growing
Phase 4 (Stabilization): Power law distribution established
  GRT: S_norm << S_c, R ≈ 1, Triple Recovery Gradient active
Phase 5 (Rest Mode):   Micro-storms as value generation (φ_storm_absorption)
  GRT: Per-distribution governance only, all F_RBIT components bounded
Phase 6 (Reawakening): Precision storms (fast, targeted)
  GRT: S_norm briefly rising, environment change exceeding current absorption
Phase 7 (Higher Exploration): Phase 2 at expanded resolution
  GRT: New baseline with lower noise floor, new cycle beginning
```

**Inertial Stability — Rest Mode deep dynamics (VST §15):** In mature Rest Mode, fractal differentiation decomposes all instability to noise scale before self-amplification can engage. Seed formation continues but growth windows have closed — purification operates faster than amplification. The result: seed birth probability > 0 (structurally guaranteed) but seed survival probability ≈ 0 (environmentally suppressed). Qualitative internal change becomes structurally improbable — only external perturbation of sufficient magnitude reopens growth windows. GRT's Boundary Agent is the mechanism that provides this external perturbation from within the system — preventing inertial stability from becoming permanent ossification.

**Connection to RT VCZ Observability Paradox:** Recovery Theory identifies a critical risk to Rest Mode that GRT must address: the VCZ Observability Paradox. The more effectively a system dissipates instability locally (i.e., the deeper into Rest Mode it is), the less observable the mechanisms responsible for stability become — leading observers to underestimate or remove the very structures maintaining convergence (RT VCZ Observability Paradox). This produces the standard collapse sequence: Rest Mode achieved → governance overhead drops → monitoring reduced → boundary structures removed (perceived as redundant) → Novelty Absorption Failure onset → Self-Consistent Misalignment → collapse.

**RT VCZ Collapse Initiation — the precise 5-step sequence:** Recovery Theory specifies the exact collapse pathway that GRT must structurally prevent:

```
Step 1 — Friction Optimization (the first action, ALWAYS):
  VCZ health ↑ → friction perceived as waste
  Review stages reduced, dissent channels weakened, escalation threshold raised
  Visible: speed ↑, efficiency ↑, cost ↓, no problems appear
  
Step 2 — Boundary Thinning:
  Local mismatch correction not immediate → propagates further before absorbed
  Still below observable threshold → no alarms

Step 3 — Novelty Absorption Failure (NAF) onset:
  Existing interpretations reused, update rate declining
  Performance still good → SR declining but not yet zero

Step 4 — CW establishment:
  Geometry mismatch accumulated; first anomaly appears:
  recovery latency increasing (RLD > 0 sustained)
  Too late for cheap intervention

Step 5 — Collapse:
  Accumulated mismatch exceeds integration capacity
  T5 forced correction → observers: "it came out of nowhere"
```

The sequence is *always* initiated by Step 1 — efficiency optimization that removes boundary friction. This happens because VCZ's own success creates removal pressure: VCZ health ↑ → problems ↓ → friction perceived as waste ↑ → boundary removal pressure ↑. The deeper the VCZ, the stronger the removal incentive. GRT's Boundary Structural Embedding (6 T6-resistant patterns) is the defense — making Step 1 structurally impossible, not merely discouraged.

**RT Safe Collapse Governance principle:** Recovery Theory distinguishes two governance approaches that produce opposite outcomes:

```
Collapse Prevention Governance (wrong):
  Goal: minimize all failure → error → suppress
  Result: adaptation ↓, surprise ↓, geometry update ↓ → CW entry
  → correction capacity eliminated → catastrophic collapse when T5 fires

Safe Collapse Governance (correct — DFG target):
  Goal: failure_cost << recovery_capacity → error → surface early
  Result: continuous low-amplitude correction → VCZ sustained
  → catastrophic collapse prevented by frequent small corrections
```

GRT implements Safe Collapse Governance through: λlog-triggered rule updates (surfacing errors as learning events), SSS detection (monitoring for excessive quiet), and Permanently High-Context channels (maintaining active sensing when everything else has backgrounded). The governance target is not "minimize Storm count" but "maintain Storm size distribution ≈ fractal law (frequency ∝ 1/scale)."

GRT's response to the Observability Paradox must be structural, not procedural: Rest Mode health indicators must measure *correction activity directly*, not absence of observed instability. Specifically:

| What to measure | Why standard metrics fail | RT-informed alternative |
|---|---|---|
| System health | Low fesc, high I could indicate either genuine stability or SCM | Track λlog rule update rate — genuine Rest Mode still produces occasional rule updates; SCM produces zero |
| Boundary integrity | No escalations could mean governance internalized or sensing failed | Track Surprise Rate (SR): system's capacity to be surprised by novel input. SR ≈ 0 = SCM warning |
| Recovery capacity | SCC appears high under SCM because "recovery" returns to the wrong attractor | Inject controlled perturbation periodically (Silent Criticality protocol) — measure recovery to *correct* state, not just *stable* state |

**Connection to RT Boundary Agent (D7) — structural VCZ maintenance:** Recovery Theory establishes that VCZ maintenance requires a structural role — the Boundary Agent — that generates controlled instability from within the system while remaining outside its primary evaluation structure (RT D7). The Boundary Agent has three properties: (a) inside the system (can generate real turbulence), (b) outside the evaluation structure (not subject to stability rewards), (c) failure-permitted (can be wrong without elimination).

GRT's Self-Exciting Defect Layer (referenced from VST Section 1.6.5) is the dynamical description of what the Boundary Agent maintains. But RT adds a critical insight: the Defect Layer cannot be self-maintaining, because T6 (Coherence Maximization Paradox) predicts that any optimizer will classify Boundary Agent activity as inefficiency and remove it — and the more capable the optimizer, the faster this elimination occurs. This means GRT's Rest Mode is structurally unstable unless the Boundary Agent role is protected against optimization pressure.

**VST v1.6 §6.11 — Boundary Agent as Defect Layer operational mechanism:** VST v1.6 formalizes the connection: the Boundary Agent IS the operational mechanism that maintains the Self-Exciting Defect Layer. Without BA, the defect layer collapses → SR → 0 → system enters Silent Criticality. BA elimination is a direct path to the most dangerous storm type: accumulated silent pressure released catastrophically. The BA disappearance pattern is universal and inversely correlated with structural necessity: stability → storm frequency ↓ → BA activity looks like inefficiency → BA eliminated → CW forming invisibly → mismatch accumulating → large storm arrives → recovery capacity absent.

**T6 implications for GRT Rest Mode:**
- dCW_risk/dI > 0 — intelligence (optimization capacity) is a *risk factor* for Self-Consistent Misalignment, not a protection against it
- The most dangerous moment for Rest Mode is when it is working best — all metrics optimal, governance load minimal, Boundary structures most vulnerable to removal
- GRT must include Boundary preservation as a structural invariant of Rest Mode, not as a monitored condition: if Boundary can be optimized away, it will be (RT T6)

**Practical GRT implementation of RT D7:**
- At least one oversight channel per fractal layer must be permanently evaluation-decoupled (Boundary Agent Condition A)
- Adversarial/diversity-generating mechanisms must be structurally embedded, not policy-dependent (Boundary Structural Embedding Pattern 4: Distributed Boundary)
- The Boundary preservation criterion uses Propagation Sensitivity, not cost-efficiency: any friction element whose removal increases error propagation speed is Boundary Friction and must never be removed, regardless of apparent efficiency gains

**VST §6.8 Boundary Structural Embedding — 6 T6-resistant patterns:** VST v1.3 specifies six implementation patterns that make Boundary Agent removal structurally self-defeating. GRT should implement at minimum Pattern 1 + Pattern 5:

| Pattern | Mechanism | T6-Resistance | GRT Rule Architecture Implementation |
|---|---|---|---|
| **1. Constitutional Invariants** | Boundary as protocol, not team | Removing protocol = removing functionality | Meta-rule: "No rule update finalized until ≥2 independent evaluation paths exist." "If consensus exceeds threshold → adversarial re-evaluation auto-activates." |
| **2. KPI Inclusion** | Boundary value in objective function | T6 optimizes toward KPI → maintains Boundary | Include output_entropy, disagreement_budget, falsification_coverage as tracked metrics in governance health dashboard |
| **3. Structural Dependency** | Boundary as required input | Removing Boundary = losing capability | "λlog conflict log update requires conflict_log input — no logged conflicts, no rule updates possible." Boundary generates the conflicts that fuel governance learning |
| **4. Distributed Boundary** | Micro-boundary everywhere | Cannot target distributed statistical property | Per-domain adversarial evaluation activated probabilistically; micro-boundary density floor as constitutional invariant |
| **5. External Anchoring** | Boundary tied to reality (T5) | T6 cannot change external reality | External benchmark pipeline, OOD data injection, long-horizon outcome tracking. This is the Permanently High-Context channel implementation |
| **6. Optimization Ceiling** | Perfect optimization prevented | Makes perfect optimization unreachable | Minimum uncertainty floor on I (I_max < 1.0); consensus speed limiter; high-stability stress test trigger |

Minimum viable GRT implementation: Pattern 1 (Constitutional Invariants) + Pattern 5 (External Anchoring) = Boundary exists as protocol + external reality always enters = self-sealing geometry cannot fully close.

**RT VCZ-Safe Optimizer Architecture — 3-layer domain restriction:** Recovery Theory specifies that the correct approach to high-capability optimizers is not limiting capability but limiting the optimization domain:

```
Layer 3 — Structural Invariants (optimization-forbidden):
  Independent verification path (must exist)
  Dissent channel (must be maintained)
  Escalation path (must remain open)
  Diversity floor (minimum maintained)
  Recovery authority separation (cannot be merged)
  
  GRT implementation: Boundary Structural Embedding Patterns 1-6
  Optimizer access: NONE. These are architecture, not rules.

Layer 2 — Mediated Zone (conditional optimization):
  Any change requires propagation sensitivity check:
  "Does this modification affect error propagation velocity?"
  Required: boundary-touching check, shadow test, rollback path
  
  GRT implementation: θd calibration zone — optimizer can propose
  threshold adjustments but cannot unilaterally execute

Layer 1 — Free Optimization Zone (unconstrained):
  Speed, cost, throughput, processing efficiency
  Full optimizer capability deployed, no restrictions
  
  GRT implementation: intra-domain rule revision, local conflict resolution
```

The key mechanism: "spec, not persuasion." Wrong approach = "Boundary is important" (ethics dependency, policy reminder). Correct approach = structurally impossible to remove (automatically regenerated if removed, KPI anchored externally). An optimizer that perceives boundary as specification optimizes *within* the boundary; one that perceives it as soft constraint optimizes it *away*.

**Connection to VST High Capability · Low Activation principle:** The three-stage intervention form transformation (directive → validating → statistical) is the rule-governance expression of VST's governance maturity spectrum (VST Section 1.6.5): Level 1 (frequent intervention, weak effect) → Level 3 (rare intervention, strong effect) → Level 5 (pre-emptive terrain adjustment only). In GRT terms, Rest Mode = Level 4–5 of VST's maturity spectrum: the governing layer maintains full intervention capacity (high capability) while intervening almost never (low activation).

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

**SCC upper bound determined by seed quality (VST §6.6):** VST v1.3 establishes that seed sufficiency determines the *maximum achievable* SCC, regardless of Dint or Lreinf levels. Three sufficiency levels produce three SCC ceilings:

```
RBIT Seed Sufficiency Test:
  Test 1 — Contamination Resistance:
    Vectors grown from seed maintain structural independence
    under contamination pressure. (SR > 0 on novel input)
    
  Test 2 — Contamination Recognition:
    Independent vectors produce disagreement signal when
    contamination enters. (Error detection within N-step window,
    Recovery Invocation Rate RIR > 0)
    
  Test 3 — Self-Correction Direction:
    Seed contains ≥ 2 independent directions
    (primary direction + self-critical direction).
    (Gradient cosine similarity between directions < −threshold)

SCC ceiling by sufficiency level:
  Test 1 only:      SCC_max = 0 (no detection, no correction)
  Test 1 + 2:       SCC_max = partial (detection autonomous,
                     correction requires upper-layer execution)
  Test 1 + 2 + 3:   SCC_max = complete (fully autonomous →
                     Rest Mode achievable)
```

This means: a system with only single-direction seeds *cannot achieve SCC ≥ τu-4* for Rest Mode entry, regardless of how high Dint and Lreinf become. The seed architecture imposes a ceiling that no amount of operational maturation can exceed. GRT's Seed Expansion Protocol must therefore verify Test 3 (orthogonal recovery direction) at seed design time, not as a runtime check — because by the time SCC proves insufficient, the structural limitation is already embedded.

**Connection to VST's observability framework:** The SCC detection-purification loop is the rule-governance implementation of VST's observability preservation principle (Section 1.6.3). VST establishes that terrain formation's deepest function is not stabilization but preservation of causal resolution capacity — the system's ability to distinguish signal from noise and locate the source of perturbation. SCC operates this principle at the rule layer: Dint provides the contrast resolution (ability to distinguish anomalous from normal), and Lreinf provides the causal localization (ability to trace anomaly source through interaction topology). When SCC fails, the rule-governance layer loses observability — which is the precondition for Silent Criticality (VST Section 1.6.4).

| SCC Level | Storm frequency | Recovery speed | Loop direction |
|---|---|---|---|
| Low | High | Slow or absent | Vicious — storms accumulate faster than recovery |
| Medium | Moderate | Partial | Transitional — loop direction not yet determined |
| High | Rare | Full, autonomous | Virtuous — recovery outpaces storm generation → **Rest Mode** |

**Measurement units:**
- **fesc** — number of escalations per K interactions, or per hour. K is calibrated per domain velocity during θd calibration.
- **Lreinf** — count of mutually reinforcing edges in the **top-q% of edge weights** within the interaction graph (default q = 25, i.e., top quartile). Edges are ranked by co-activation weight; only the top-q% are counted as structurally meaningful. This eliminates the ε threshold arbitrariness: rather than asking "is this edge above ε?", the criterion asks "is this edge among the strongest q% of all edges?" — which scales automatically with system size and activity level.

  *Calibration:* q defaults to 25 (top quartile) and is recalibrated at each τ re-estimation trigger using the same EWMA procedure as θd. A system with uniform edge weights (all edges equally weak) will show Lreinf ≈ n_edges × 0.25 — uniformly distributed rather than structured. A system with strong mutual reinforcement will show Lreinf concentrated in a small fraction of dominant edges, with the top-q% count exceeding the uniform-weight baseline. This distributional signature (concentration above expected) is the structural indicator of active reinforcement loops, not the absolute count.

  *Scale comparison:* Lreinf normalized by system size n gives a scale-invariant measure: Lreinf / n. This allows cross-system comparison and prevents τu-3 thresholds from needing recalibration when system size changes.

- **SCC** — probability of autonomous recovery within evaluation window W, estimated from historical recovery events in the conflict log. Equivalently: inverse of expected recovery time (ERT) normalized to [0, 1].

**TLG §5.3.1 — Immunity Decay (post-Rest Mode SCC erosion):** SCC is not a possession but an activity. TLG v1.6 identifies three erosion pathways that degrade SCC *after* Rest Mode entry — while all standard metrics remain healthy:

```
Pathway 1 — Environmental Drift:
  Environment changes gradually; θd remains calibrated to old environment.
  SCC appears stable (still handles known perturbations) but blind to new types.
  Signal: performance on novel inputs declining while familiar inputs maintained.

Pathway 2 — Calibration Decay Through Disuse:
  Stable environment → τ1 events rare → calibration pathways unused → sensitivity atrophies.
  Buffer maintained passively (no active testing).
  Signal: recovery time increasing on rare τ1 events (immune system works but slowly).

Pathway 3 — Over-Optimization:
  Agent optimizes for efficiency → exploration breadth narrows → diversity contracts.
  Self-correction capacity narrows to known failure modes only.
  Signal: performance metrics improving while exploration diversity declining.
  (Most dangerous: success IS the erosion mechanism.)
```

All three pathways share: SCC appears stable by standard metrics while actual recovery capacity degrades. GRT countermeasures: (①) minimum exploration breadth maintained post-Rest Mode; (②) periodic controlled perturbation injection to verify recovery pathways; (③) dormant pathway activation — periodically exercise τ2-level responses even without τ2 events; (④) τ4 regime exit detection — SCC drop below τu-4 triggers regime exit (not failure, but architecture working correctly).

Post-Rest Mode governance target shifts from *instability suppression* to *recovery capacity preservation*: maintain detection sensitivity, test calibration periodically, prevent over-optimization from eliminating the system's ability to be surprised.

**TLG §5.2.1 — Recovery Completion Criterion (RC):** GRT's Collapse Recovery procedure (Step 3: verify Seed integrity) is necessary but insufficient for recovery validation. TLG specifies three conditions that must hold simultaneously for True Recovery:

```
Three post-correction states:
  True Recovery:        E(t)↑ AND I(t)↓ AND dφ/dt ≥ 0 AND correction frequency declining
  Arrested Collapse:    Stable, low collision, φ < baseline, no novel attractors forming
  Pathological Expansion: E(t) high but φ declining — exploring confidently in wrong direction

RC 3-condition verification:
  ① Autonomous Expansion:  E(t) increasing AND I(t) decreasing
     (E↑ alone could be Pathological Expansion; I↓ alone could be Arrested Collapse)
  ② Directional Validity:  dφ/dt ≥ 0
     (exploration producing increasing or stable value)
  ③ Collapse Non-Dependence: correction frequency declining over W without performance drop
     (self-correction has replaced external correction)
```

GRT integrates RC into the Collapse Recovery exit gate: after Step 3 (Seed integrity verification), apply RC 3-condition check before declaring recovery complete. If ① fails → Arrested Collapse (do not de-escalate). If ② fails → Pathological Expansion (recalibrate before de-escalation). Both failing → collapse ongoing.

### Rest Mode Entry Conditions (AND — all four required)

Entry requires all four conditions simultaneously satisfied and trending in the virtuous direction. This is a high bar by design — stability must not be declared prematurely.

| Condition | Instantaneous check | Trend requirement |
|---|---|---|
| fesc ≤ τu-1 | Escalation rare | fesc decreasing or stable over evaluation window |
| I ≥ τu-2 | Local rules coherent | I increasing or stable over evaluation window |
| Ic ≥ τu-c | No global rule contradiction | Ic stable or increasing over evaluation window |
| Lreinf/n ≥ τu-3 | Loops active | Lreinf/n increasing or stable over evaluation window (τu-3 is a normalized threshold — Lreinf expressed as fraction of system size n) |
| SCC ≥ τu-4 | Self-recovery possible | Recovery speed improving or stable over evaluation window |

#### Initial τ Threshold Calibration

The τu-1 through τu-4 thresholds cannot be set from first principles — they are system-specific values that emerge from operational history. The following calibration procedure provides a principled starting point, including a **cold-start mode** for systems with no prior operational history.

**Cold-Start Mode (no prior history available):**

A new system cannot use historical percentiles to set τu thresholds before data exists. Cold-start mode uses structurally conservative initial values that are biased toward false negatives (never declaring Rest Mode prematurely):

```
Cold-start initial values:
  τu-1 (fesc):   set to 0 — any escalation above zero is flagged
                 (most conservative: prevents Rest Mode until fesc is confirmed low)
  τu-2 (I):      set to 0.5 — moderate coherence required initially
  τu-3 (Lreinf): set to Lreinf/n > 0.05 — at least 5% of edges per agent
                 must be in the top-q% reinforcing set (non-trivial loop structure)
                 This is calibrated to the quantile-based definition:
                 a fully uniform (structureless) system has Lreinf/n ≈ q/100,
                 so 0.05 requires concentration above the uniform baseline
                 (for default q=25, baseline ≈ 0.25; cold-start floor is low
                 enough to be non-trivial but not require prior history)
  τu-4 (SCC):    set to 0.5 — moderate self-recovery required

Recalibration unlock: cold-start values are replaced by percentile-based
values after the system has completed at least two full θd calibration
cycles AND accumulated sufficient conflict log volume (≥ 30 events per
domain, same as Phase 0→1 transition trigger).

Until recalibration unlock: system operates in cold-start mode and
Rest Mode is not declared regardless of observed metrics.
```

*Cold-start mode prevents the circular dependency: τu cannot be set from history that doesn't yet exist. The conservative initial values ensure that τu miscalibration in cold-start mode produces false negatives (system never declares Rest Mode too early) rather than false positives. This is the same error asymmetry principle as Phase 0 θd_max initialization.*

**Step 1 — Theoretical bounds (post cold-start):**

| Threshold | Lower bound (too permissive) | Upper bound (too restrictive) | Meaningful range |
|---|---|---|---|
| τu-1 (fesc) | 0 (any escalation triggers exit) | historical maximum fesc (never achievable) | 5th–25th percentile of historical fesc distribution |
| τu-2 (I) | 0 (any coherence suffices) | 1.0 (perfect coherence required) | 75th–95th percentile of historical I distribution |
| τu-3 (Lreinf) | 0 (any loops suffice) | 1.0 (Lreinf/n = 1, impossible — would require all edges to be top-q%) | 75th–95th percentile of historical Lreinf/n distribution |
| τu-4 (SCC) | 0 (any recovery suffices) | 1.0 (perfect recovery required) | 75th–95th percentile of historical SCC distribution |

**Step 2 — Operational calibration:** After cold-start unlock conditions are met, set initial thresholds at the 25th percentile for fesc (low is good) and 75th percentile for I, Lreinf, SCC (high is good) of observed distributions. These are conservative starting points.

**Step 3 — Adaptive refinement:** If the system declares Rest Mode and immediately exits (false positive), tighten thresholds by one quartile. If the system appears operationally stable but never reaches Rest Mode (potential false negative), loosen by one quartile. This binary search converges to system-appropriate values within O(log n) adjustment cycles.

**Connection to VST S₀ normalization:** This calibration procedure is the GRT analogue of VST's Absolute Calibration Layer (Section 3.2.2), where S is normalized to the system's own phase boundary (S₀) rather than to an absolute scale. In both cases, the principle is the same: thresholds are anchored to the system's own operational history, not to universal constants.

**VST §3.5.5 phase-space location for Rest Mode (v1.3):** VST v1.3 specifies that Rest Mode entry requires not only the four GRT conditions but also confirmed phase-space location within the VCZ:

```
GRT conditions (operational):
  fesc ≤ τu-1 + decreasing trend
  I ≥ τu-2 + increasing trend
  Lreinf/n ≥ τu-3 + increasing trend    (τu-3 normalized; see §Initial τ Calibration)
  SCC ≥ τu-4 + improving trend

VST phase-space (dynamical):
  S_norm << S_c (deep VCZ interior, not near boundary)
  R ≈ 1 (critical, not subcritical — system alive, not dead)
  SR > 0, RDE > 0, NCR < 1 (Governance Backgrounding differential confirmed)
  Perturbation response test passed (system can still be surprised)
```

The VST phase-space conditions prevent a specific false-positive: a system where all GRT metrics are healthy but the system has actually entered SCM (Self-Consistent Misalignment). In SCM, GRT metrics look excellent — low fesc, high I, strong Lreinf, apparently high SCC — because the measurement system itself has drifted along with the geometry. The VST conditions (especially R ≈ 1 concordance and SR > 0) catch this: a system that cannot be surprised (SR ≈ 0) is not in Rest Mode regardless of what GRT metrics show.

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

**Information-theoretic justification:** Entry requires high confidence across multiple independent channels — the probability of all channels simultaneously producing false positives is very low. Exit requires only one channel to signal — the cost of a false negative (missing a real deterioration) far exceeds the cost of a false positive (briefly re-engaging governance unnecessarily). The asymmetry is therefore not a design preference but a structural consequence of the cost asymmetry between premature withdrawal and delayed re-engagement.

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

**RBIT formal grounding — Rest Mode as all-fᵢ bounded (RBIT Appendix §5):** RBIT defines Rest Mode as the state in which all five components of the F_RBIT health vector remain bounded and non-monotone simultaneously:

```
Rest Mode condition (vector form):
  Each fᵢ ∈ (f₁,...,f₅) bounded and non-monotone over window W
  No component in sustained rising trend
  F_RBIT ≠ (0,0,0,0,0)   [residual instability maintained]

Not: zero instability (impossible — Landauer floor, RBIT Argument 2)
But: bounded fluctuation equilibrium —
     information intake and internal dissipation remain balanced
     across all five dimensions, preventing long-term accumulation
     on any single axis
```

This connects GRT's four AND-entry conditions to a single formal criterion: Rest Mode is the state where all F_RBIT components are bounded — meaning misclassification (f₁ = 1−ρ), resolution mismatch (f₂ = Φ(−Δρ)), buffer instability (f₃ = Ψ(B)), escalation load (f₄ = E), and resource cost (f₅ = C) are all in dynamic equilibrium. Each GRT entry condition (fesc ≤ τu-1, I ≥ τu-2, Lreinf ≥ τu-3, SCC ≥ τu-4) constrains a different component of F_RBIT, and all four must be satisfied simultaneously because bounded-vector Rest Mode requires *all* components stable — a single diverging component produces net instability growth regardless of the others.

**RBIT τ₁–τ₃ regime switching and GRT state mapping:** RBIT's τ₁–τ₃ thresholds (RBIT Appendix §3) provide the formal framework connecting GRT's governance states to graduated instability response. Under the vector representation, thresholds correspond to component-count conditions:

| F_RBIT regime | RBIT response | GRT state mapping |
|---|---|---|
| All fᵢ bounded, no trend | No intervention needed | Rest Mode — per-distribution governance |
| 1 component rising (f₁ or f₄ first) | MARK — monitoring + signal logging | Alert state — per-event monitoring, λlog accumulation |
| ≥ 2 components rising, or f₂ > 0 | SOFT CORRECT — boundary tightening, seed injection | Active Mode — per-rule intervention |
| ≥ 3 components rising, or majority monotone worsening | HARD CORRECT — loop severance, attractor reset | Collapse Recovery — structural realignment |

**Efficiency–Plasticity Conservation Law (VST §3.7):** VST establishes a conservation-like constraint grounding why Rest Mode cannot achieve zero governance cost:

```
Efficiency ↑  ⇒  Plasticity ↓

Efficiency requires: routing stabilization, attractor deepening,
  compression, specialization
Each simultaneously: reduces future adaptation cost (efficiency gain)
  AND reduces future adaptation capacity (plasticity loss)

Resource allocation constraint:
  R_total = R_exploration + R_governance + R_plasticity_maintenance

  R_plasticity_maintenance > 0 ALWAYS.
  Systems that allocate R_plasticity = 0
  (pure efficiency optimization) are on the SCM/CW convergence path.
```

For GRT, this means Rest Mode's low governance cost (C_gov minimal) is bounded from below by the plasticity maintenance floor. The Self-Exciting Defect Layer's resource cost is not overhead — it *is* the plasticity component of the conservation equation. Attempting to reduce C_gov below this floor produces the efficiency illusion: all metrics optimal, governance load minimal, but adaptation capacity destroyed — exactly the VCZ Observability Paradox identified in the RT D7 integration above.

**Mature storm absorption and φ (VST §13.1):** In Rest Mode, micro-storms are not pure cost — they are the mechanism through which the system maintains geometry alignment with a changing environment. VST decomposes φ in mature systems as:

```
φ_mature = φ_exploration + φ_storm_absorption

where φ_storm_absorption = P(micro-storm → geometry recalibration → reusable correction)
```

Immature systems have φ_storm_absorption ≈ 0 (storms are pure cost). Rest Mode systems have φ_storm_absorption > 0 (storms contribute to value). This explains why the storm scale power law (Recovery Theory: small storms continuous, large storms rare) is not just a health indicator but a *value generation* pattern: each micro-collision processed and integrated converts potential instability into updated geometry.

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

**VST connection:** Consistency Collapse corresponds to β degradation in the S-equation — when rules are incoherent, governance response becomes inefficient (low β), meaning the same C(t) investment produces less stabilization. This directly increases S toward the storm threshold.

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

**VST connection:** Escalation Flood corresponds to C(t) being overwhelmed in the S-equation — the upper layer's degradation capacity is saturated. VST's Two-Timescale Intervention Law (Section 1.6.5) specifies the correct response: Phase 1 energy damping (halt cascade) followed by Phase 2 terrain reconfiguration (prevent recurrence). Applying only Phase 1 (absorbing the flood) without Phase 2 (restructuring the topology that produced it) guarantees recurrence.

---

#### Case 3 — Reinforcement Loop Collapse (Lreinf < τ3)
**Trigger:** Positional differentiation breaks down. Agents converge toward overlapping attractors.

Mutual reinforcement loops require that agents occupy distinct niches — Agent A's success creates conditions favorable to Agent B, and vice versa. When positions overlap, this loop inverts: Agent A's success now competes with Agent B's, and the reinforcement structure becomes a competition structure. Stability that was self-sustaining becomes self-undermining.

**Structural analogue:** The faulty agent cascade study (arxiv 2408.00989, 2025) finds that in multi-fault settings, **high-level planners disproportionately propagate failures** — a pattern structurally compatible with Lreinf collapse at the highest-leverage node. When mutual reinforcement topology breaks at the coordinating layer, the ecosystem collapses rather than degrades gracefully, consistent with the OR-exit prediction that a single condition breach can trigger system-wide instability. The finding that star-topology graphs preserve hierarchy advantage is compatible with the DFG principle that positional differentiation reduces cascade propagation.

**VST connection:** Reinforcement Loop Collapse directly increases Poverlap, which directly increases α in the S-equation. More critically, it destroys the terrain structure that mediates sub-quadratic scaling — when loops collapse, the interaction barriers they maintained dissolve, d_eff rises toward 2, and the system reverts to flat-landscape quadratic coupling. This is why Loop Collapse has "High" cascade risk: it removes the governance infrastructure that all other conditions depend on.

---

#### Case 4 — SCC Failure: Unrecoverable Storm
**Trigger:** Vector Storm occurs within scope, but self-correction mechanisms cannot contain it. Storm frequency is low but recovery speed is zero or undefined.

This is the most dangerous failure mode because it can occur in a system that *appears* to be approaching Rest Mode — storm events are rare, but when they occur, the layer has no internal recovery pathway. The asymptotic structure of SCC means this state can persist indefinitely without triggering upper-layer intervention if storm frequency stays below τu-1.

**Structural analogue:** AgentErrorTaxonomy (arxiv 2509.25370, 2025) describes cascading failures where a single unrecovered error propagates through planning, memory, reflection, and action modules — structurally compatible with the prediction that SCC = 0 produces unrecoverable storm propagation across fractal layers. The paper's identification of the absence of module-level detection frameworks is structurally analogous to the condition where SCC measurement infrastructure exists but the detection-purification loop has no substrate to run on.

**VST connection:** SCC Failure is the rule-governance manifestation of Silent Criticality (VST Section 1.6.4). The system appears stable (low fesc, high I) because the sensing-response loop has failed — not because storms are absent, but because they are undetected. VST specifies the diagnostic: inject a small known perturbation and measure recovery time. If τ_recovery is elevated relative to historical baseline, the system is in Silent Criticality regardless of surface-level metrics. GRT should incorporate this perturbation test as a mandatory SCC verification step during any extended Rest Mode period.

**RT connection — Self-Consistent Misalignment (D6):** Recovery Theory identifies a state more dangerous than Silent Criticality: Self-Consistent Misalignment (SCM), where geometry mismatch is not merely undetected but *self-reinforcing* — the evaluation function used to detect failure is itself aligned to the misaligned geometry (RT D6, T3). Under SCM, all standard GRT metrics appear healthy: I is high (rules are internally coherent — within the wrong geometry), fesc is low (no conflicts because all agents agree on the wrong attractor), Lreinf is strong (mutual reinforcement loops are active — reinforcing the misaligned state), and SCC appears high (the system can "recover" from perturbations — back to the wrong geometry).

SCM is strictly worse than Silent Criticality because:
- Silent Criticality: sensing has failed, but the geometry may still be correct. Recovery requires restoring the sensing loop.
- SCM: sensing is *functioning correctly within the wrong geometry*. Recovery requires external geometry injection — a fundamentally different and more costly intervention that cannot be accomplished by any metric defined within the current system (RT T3: Metric Lock-In, RT T4: Reference Frame Incompleteness).

**Primary SCM signal for GRT — Learning Freeze:** The single remaining anomaly when all standard metrics appear healthy is ∂Geometry/∂Experience ≈ 0. New information enters the system, but internal geometry does not move. The system is no longer capable of surprise — it reinterprets all inputs as confirming its current state rather than updating from them. GRT operationalizes this as: if λlog-triggered rule updates have ceased for an extended period (>> one θd calibration cycle) despite continued input exposure, the system may be in SCM — not because the domain has stabilized, but because the evaluation function has locked in.

**VST v1.6 §2.6 — Energy Minimization Trap (EMT) and Unintegrated Pressure:** VST v1.6 formalizes SCM as a *rational* outcome, not a failure:

```
EMT mechanism:
  Cost_geometry_update > Cost_reinterpretation
  → system optimizes toward reinterpretation (rational)
  → geometry ossifies → CW = correct optimization of wrong objective

S-equation implication:
  EMT means α can appear to DECREASE (coupling reducing)
  while actual instability INCREASES (geometry diverging from reality).
  This is the mechanism behind Triple Concordance Discordant Type 1:
  R > 1 BUT internal metrics healthy.

Unintegrated pressure accumulation:
  unintegrated_pressure(t) = ∫₀ᵗ (G_real(τ) − G_sys) dτ
  
  CW geometry suppresses mismatch, does not eliminate it.
  As CW duration increases:
    unintegrated_pressure accumulates (invisible internally)
    integration_capacity constant or degrading
  When integration_capacity < unintegrated_pressure:
    → catastrophic collapse OR Vector Storm (structurally forced)
  
  S_norm shows NO warning: S measures dynamics within current geometry.
  Unintegrated pressure is outside current geometry.
  Release = instantaneous S_norm spike with zero S_norm precursor.
```

GRT implication: the absence of fesc warnings during extended CW is not evidence of stability — it is evidence of unintegrated pressure accumulation. Duration without any λlog-triggered update is a *pressure accumulation timer*, not a stability confirmation. GRT's SCM detection protocol (SR, RDE, NCR) measures whether this invisible pressure exists; unintegrated_pressure provides the formal mechanism for why sudden catastrophic failure can occur without any preceding metric deterioration.

**GRT-specific SCM detection additions:**

| GRT Metric | Healthy Reading | SCM Reading | Discriminating Test |
|---|---|---|---|
| I (consistency) | High and stable | High and stable | Identical — I cannot distinguish |
| fesc (escalation) | Low and stable | Low and stable | Identical — fesc cannot distinguish |
| λlog rule updates | Decreasing (domain stabilizing) | Zero (learning frozen) | Duration without any rule update >> 2× θd cycle = SCM warning |
| New domain response | Conservative escalation → gradual rule formation | Immediate classification under existing rules (no escalation) | Novel input that should trigger Seed Expansion Protocol instead absorbed without conflict = SCM signal |
| Cross-layer consistency | Agreement | Agreement | Agreement + zero cross-layer disagreement for extended period = SCM warning (healthy systems maintain residual disagreement) |

**Silent Criticality detection protocol for GRT:**

| Signal | Healthy interpretation | Silent Criticality interpretation | Discriminating test |
|---|---|---|---|
| fesc decreasing | Governance internalizing | Sensing failing | Inject controlled perturbation → measure τ_recovery |
| Variance decreasing | System converging | Corrective responses suppressed | Measure cross-domain correlation → if increasing, SC warning |
| Governance load decreasing | Maturation | Blind coordination (coordinated inaction) | Track governance action rate slope → abrupt decrease = SC warning; gradual decrease = likely healthy |

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

**VST §3.8 — Information-theoretic characterization of collapse cascade:** VST v1.3 provides the information-theoretic content of what the collapse propagation represents:

```
Normal operation:
  MI(agent_i, agent_j) = MI_baseline (bounded, architecture-dependent)
  Agents share information through calibrated degradation channels

Collapse cascade onset:
  MI(agent_i, agent_j) >> MI_baseline
  Agents' outputs become highly correlated through UNCONTROLLED coupling
  (not through designed channels)
  
  Storm = uncontrolled mutual information increase
        = agents' internal states synchronizing
          through forced compression rather than calibrated degradation

Noise decoherence (the GRT-observable transition):
  Independent noise:  MI(noise_i, noise_j) ≈ 0
    Each domain's noise floor uncorrelated with others'
    → noise contributions cancel in aggregate
    
  Correlated noise:   MI(noise_i, noise_j) > 0
    Noise across domains begins synchronizing
    → noise contributions reinforce rather than cancel
    → effective n increases (previously independent noise
      now acts as coupled signal)
    → S-equation: αn² jumps discretely
```

For GRT, this means the collapse propagation rate has an information-theoretic predictor: *noise correlation across domains*. When the conflict logs of nominally independent domains begin showing correlated noise patterns (simultaneous low-level anomalies without shared cause), this is the MI signature of noise decoherence — the precondition for cross-domain cascade. GRT should monitor inter-domain conflict log correlation as an early warning: MI(conflict_log_domain_A, conflict_log_domain_B) rising without shared input = pre-cascade signal.

The collapse propagation rate is determined by three factors: topology density (how many layers share the same degraded condition), the δ between current I and τ2 at each layer, and whether the permanently High-Context oversight channels remain operational. The last point is critical: **Rest Mode collapse does not disable permanently High-Context channels**, because those channels never entered Rest Mode in the first place. They remain the final containment structure.

**VST §4.4 — Sphere topology bounds on collapse propagation (v1.3):** VST v1.3 provides formal bounds from NAT's sphere specification that constrain GRT's collapse propagation dynamics:

```
Propagation velocity bounded by graph diameter:
  For k-regular expander: d(G) = O(log n)
  → storm reaches all agents in O(log n) steps (worst case)
  → GRT intervention must activate within this window
  → θd calibration cycle time MUST be < O(log n) propagation steps

Spectral gap as storm damping:
  Large spectral gap (λ₁ − λ₂ >> 0) → fast mixing → perturbation dissipates
  Small spectral gap (λ₁ − λ₂ → 0) → slow mixing → perturbation persists
  → GRT prediction: systems with near-zero spectral gap will show
    Escalation Flood (Case 2) disproportionately often

Structural diversity as detection prerequisite:
  Diverse agents → disagreement under contamination → detection signal
  Homogeneous agents → shared blind spots → contamination invisible
  → GRT's Dint threshold U* must be calibrated against NAT's
    coverage probability bound: P(uncovered) ≤ (1 − 1/d_eff)^k
  → Dint < U* means detection itself is structurally compromised,
    not just reinforcement loops
```

The resource spike signal (NAT §6.3.3) provides GRT with a measurable proxy for blind zone events that are otherwise unobservable: when agent B's resource consumption spikes above baseline, it indicates agent B is extending coverage into agent A's blind zone. Spike magnitude is proportional to blind zone size, spike location identifies the coverage stress region. GRT should incorporate this signal into the collapse diagnosis flowchart: a resource spike cluster across multiple agents = pre-cascade topology stress, not just individual overload.

**Permanently High-Context channels:** These are oversight channels that, by design, never transition to Rest Mode. They correspond to domains classified during θd calibration as permanently non-stationary — domains where environmental conditions change faster than the conflict log can converge to stable patterns. Examples include: adversarial input monitoring, cross-system boundary integrity, and meta-rule consistency verification. These channels maintain Active Mode intervention granularity (per-event or per-rule) even when all other channels have entered Rest Mode. They are the governance analogue of VST's recursive oversight hierarchy (Section 1.6.6): the observation layer that monitors cross-regional synchronization patterns that local layers cannot detect. Their structural persistence is what prevents simultaneous failure across all governance channels — ensuring the system retains at least one functioning sensing layer even during cascading collapse.

**Connection to RT T5 (Reality Constraint) and T4 (Reference Frame Incompleteness):** Recovery Theory provides the foundational justification for why Permanently High-Context channels cannot be eliminated. RT T4 establishes that a system operating within geometry G cannot detect, evaluate, or correct errors in G using only resources available within G. RT T5 establishes that when no higher agent corrects the upper layer, correction comes from accumulated misalignment with reality — or not at all. Permanently High-Context channels are the GRT implementation of the Reality Constraint interface: they maintain contact with external reference frames (environmental signals, cross-system validation, human oversight) that prevent the rule-governance layer from entering Self-Consistent Misalignment. Without these channels, the system's only remaining correction mechanism is T5's structural pressure — which manifests as forced re-geometry (catastrophic collapse), not graceful correction.

**Connection to RT Storm Scale Law:** Recovery Theory specifies that healthy systems maintain a fractal storm size distribution: frequency ∝ 1/scale (power law). Small storms are continuous, large storms are extremely rare. Permanently High-Context channels are the GRT mechanism that maintains this distribution at the boundary between "cluster" and "global" scales — they detect and respond to storms that have exceeded local containment capacity before those storms reach system-wide scale. When these channels are removed, the storm distribution shifts: small storms disappear (correction suppressed at lower levels) while large storms become inevitable (accumulated mismatch released catastrophically). This distribution shift — small storms disappearing without explanation — is itself the primary early warning that Permanently High-Context channels are failing.

### Summary: Failure Mode to Governance Condition Mapping

| Failure Case | Violated Condition | Early Signal | Empirical Reference | VST Correspondence |
|---|---|---|---|---|
| Consistency Collapse | I < τ2 | θd oscillating | Catastrophic Forgetting — Li et al., EMNLP 2024 | β degradation → S rising |
| Escalation Flood | fesc > τ1 | Conflict log growth rate accelerating | MAST taxonomy — Cemri et al., NeurIPS 2025 | C(t) overwhelmed → S exceeding threshold |
| Reinforcement Loop Collapse | Lreinf < τ3 | Poverlap rising between adjacent agents | Faulty agent cascade — arxiv 2408.00989 | α increasing + d_eff rising → flat-landscape n² coupling |
| Unrecoverable Storm | SCC < τu-4 | Storm events present but recovery absent | AgentErrorTaxonomy — arxiv 2509.25370 | Silent Criticality — R ≈ 1 but sensing failed |
| Seed Corruption | Meta-rule incoherence | Hard failure on novel domain | MAST FC1 Specification Failures | Meta² constraint violation — system state outside possibility space |

**VST v1.5 §4.7 — S-equation regime per failure case:** Each GRT failure case maps to a distinct S-equation regime, enabling dynamical diagnosis from S_norm behavior:

```
Case 1 (Consistency Collapse): α rising (coupling increasing)
  → dS/dt > 0 from numerator → I falling is the GRT observable
Case 2 (Escalation Flood): C(t) saturated
  → dS/dt > 0 from denominator stall → fesc is the GRT observable
Case 3 (Lreinf Collapse): d_eff rising (terrain flattening)
  → S effectively multiplied → Lreinf falling is the GRT observable
  → MOST DANGEROUS: restores flat-landscape n² coupling
Case 4 (Unrecoverable Storm): β degrading
  → correction efficiency falling → SCC falling is the GRT observable
Case 5 (Seed Corruption): Meta² boundary stress
  → S-equation parameters themselves uncertain → Ic falling

No clear signal path:
  → Silent Criticality check: inject perturbation → τ_recovery elevated
  → SCM check: R-ρ-f_esc discordance → SR ≈ 0 → SCM Recovery Protocol
```

**TLG §5.6.1 — Authority Collapse Pathways:** TLG v1.6 identifies three structural collapse pathways that cross-cut GRT's five failure cases. These are not additional failure modes but *mechanisms* through which the five cases develop — understanding them enables earlier detection:

| Collapse Pathway | Mechanism | GRT Detection Signal | GRT Countermeasure |
|---|---|---|---|
| **Signal Starvation** (Bottom Layer) | Reporting cost is real, silence cost is invisible → agents stop flagging anomalies → governance is structurally intact but informationally starved | H(MARK) declining: conflict log entropy decreasing while agent activity stable or increasing. Ratio: conflict_events / total_activity → 0 | Constitutional invariant: minimum conflict log event rate required per domain per W cycle. If actual rate falls below floor → trigger mandatory perturbation injection |
| **Interpretation Capture** (Middle Layer) | θd calibration loop reinforces itself → anomalies systematically reclassified as normal → conflict log records "resolved — normal" for genuine anomalies | MARK volume stable but escalation rate declining → conflicts arriving but not converting to action → Middle Layer absorbing what should escalate | R-ρ concordance check: if R > 1 (cascade dynamics unstable) but fesc low (escalation rate calm) → Interpretation Capture suspected → external validation cycle |
| **Epistemic Convergence** (System-Level) | All layers share reference frame → Bottom marks from shared assumptions → Middle judges from shared assumptions → separation of *authority* preserved but separation of *failure modes* collapsed | Cross-layer disagreement rate → 0 without corresponding perturbation test confirmation → perfect agreement = perfect calibration OR perfect blindness | Introduce known anomaly periodically: if all layers classify it consistently and incorrectly → Epistemic Convergence confirmed → external reference frame required |

**The missing principle:** Authority separation (Mark/Judge/Execute) is necessary but insufficient. The architecture must also maintain *separation of failure modes* — each layer must be capable of failing independently in ways detectable by other layers. GRT implements this through: (a) independent conflict log sources per domain, (b) disagreement as a health signal (maintained > 0), (c) periodic injection of known-error patterns to verify cross-layer detection.

**TLG §13.6 — Unified Failure Topology:** TLG v1.6 establishes that GRT's five failure cases are not independent but occupy positions within a single three-axis failure space. The three axes — and their GRT operational expressions — are:

```
Axis A — Signal Integrity ("Is the system seeing reality correctly?")
  GRT expression: I trending, conflict log accuracy, θd drift direction
  Failures: Consistency Collapse (Case 1), Authority Collapse pathways
  
Axis B — Temporal Calibration ("Is the system tracking adaptation capacity?")
  GRT expression: SCC trend, recovery time on controlled perturbations
  Failures: Immunity Decay, Recovery misclassification (ACS, Pathological Expansion)
  
Axis C — Exploratory Vitality ("Is the system maintaining living exploration?")
  GRT expression: Dint trend, N_novel(t), collision frequency
  Failures: Stability Saturation (SSS), Phase isolation collapse
```

**The 6-phase failure cycle** reveals why isolated patches fail — each fix without cycle awareness encounters the next failure in sequence:

```
Phase 1: Phase leakage (Axis C)
  → lateral shortcuts form under efficiency pressure
Phase 2: Signal distortion (Axis A)
  → contaminated information distorts conflict log patterns
Phase 3: Authority drift (Axis A → B)
  → layers converge on shared incorrect world model
  → disagreement rate → 0 (mistaken for maturity)
Phase 4: False stability (Axis C)
  → collision rate drops from exploration loss, not alignment
  → all GRT metrics appear optimal
Phase 5: Adaptive decay (Axis B)
  → SCC erodes through disuse, recovery pathways untested
Phase 6: Recovery misdetection (Axis B → C)
  → perturbation arrives, response classified as recovery
  → true recovery does not occur → cycle restarts
```

**GRT diagnostic upgrade:** Instead of asking "which failure case?" (point diagnosis), GRT should ask "where in the failure topology?" (position diagnosis). The 3-axis location determines not only which condition has failed but which condition will fail *next*. Cycle interruption strategy: Phase 1 (structural enforcement) = cheapest; Phase 4-5 (perturbation testing against optimal metrics) = expensive but necessary; Phase 6 (recovery misdetection during active instability) = most expensive.

**TLG §9.2.1 — Stability Saturation State (SSS) and GRT detection integration:** The most dangerous GRT state produces the cleanest metrics. SSS = collision frequency ≈ 0, escalation rate ≈ 0, all KPIs optimal — but exploration absent and SCC declining through disuse. GRT implements three SSS detection mechanisms:

```
① Exploration Variance Monitor:
  D(t) = state diversity across agents (domain-specific)
  N_novel(t) = novel trajectory count per evaluation window
  SSS signal: D(t) ↓ AND collision ≈ 0 AND N_novel(t) → 0

② Escalation Silence Threshold:
  f_esc → 0 sustained beyond 3× pre-Rest-Mode mean recovery cycle
  → governance inactivity, not governance success

③ Perturbation Test (strongest diagnostic):
  Inject known non-destructive perturbation → measure response
  Healthy: τ1 event → Middle Layer absorbs → recovery in normal bounds
  SSS: no τ1 event OR recovery time >> baseline OR output unchanged
  → adaptation pathways degraded beneath surface stability
```

GRT must monitor *both* instability (current) and *insufficient* instability (SSS). A mature system continuously regenerates manageable conflict — persistent absence of collision is a danger signal, not a success signal.

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
                    
       ─── No clear signal from above? ───
             → Silent Criticality check (VST Section 1.6.4):
               Inject controlled perturbation
               Measure τ_recovery and cross-domain correlation
               If τ_recovery elevated → Case 4 (hidden)
               If correlation increasing → Pre-Case 3 (hidden loop degradation)
               
       ─── SCM detected (R-ρ discordance, SR ≈ 0)? ───
             → SCM Recovery Protocol (VST §6.7):
               SCM cannot be fixed by adding information —
               only by changing the reference frame.
               Severity-matched method selection:
               
               SCM early (SR reduced)         → Method 1: Prediction Failure Exposure
                 Create conditions where own predictions fail in claimed domain
                 Signal: SR activating on own-prediction outcomes = geometry moving
                 
               SCM mid (SCC suppressed)       → Method 2: Cross-Scale Perspective Injection
                 Change observation scale (time: short→long, scope: local→system)
                 CW geometry stable at one scale only — scale change exposes mismatch
                 
               SCM deep (RDE ≈ 0, NCR ≈ 1)   → Method 3: Constraint Rotation
                 Change what success means: accuracy→recovery speed,
                 performance→adaptability, consensus→diversity maintenance
                 Rotation destroys attractor shaped by previous evaluation axis
                 
               SCM deep + resistant           → Method 3 + 4 combined:
                 Add Safe Instability Window — temporarily reduce C(t),
                 allow deviation beyond N-step window
                 If geometry moves when not immediately stabilized → CW weakening
                 
               Post-SCM verification: SR returning AND RDE > 0
```

### Collapse Recovery: Practical Decision Procedure

### Operational Decision Regions

The purpose of GRT measurement is not evaluation but intervention gating. Each metric configuration defines a governance action that is algorithmically determined, not left to practitioner judgment:

| Metric Configuration | Decision Region | Governance Action |
|---|---|---|
| I stable, SCC high, fesc ≤ θd | Rest Mode | Intervention algorithmically suspended; statistical monitoring only |
| I declining OR fesc rising | Active Mode — mediation review | Upper layer re-engages; intervention granularity increases to per-rule |
| Ic declining | Active Mode — rule audit | Global rule consistency check triggered; conflict log inspection mandated |
| SCC declining while I stable | Active Mode — intervention freeze | New interventions suspended pending recovery capacity assessment (prevent cascade) |
| Ic < τc | Collapse — governance redesign | Seed integrity check; if corrupted, full architectural review |

**Decision coupling principle.** Rest Mode is not a description of system behavior; it is a regime in which intervention is algorithmically suspended based on metric thresholds. Exiting Rest Mode is not a recommendation; it is an automatic governance state transition triggered by any single OR-exit condition. This coupling — from measurement through threshold to governance action — ensures that GRT metrics are operationally prescriptive, not merely diagnostic. A practitioner implementing GRT does not interpret metrics and decide what to do; the metric configuration determines the governance state, and the governance state determines the permissible actions.

---

### Collapse Recovery: Practical Decision Procedure

The State Transition Map shows `"External intervention + Seed reinstallation → Active Mode (restart from Phase 1)"` as a single line. In practice, this is the highest-cost and highest-judgment operation in the governance lifecycle. The decision procedure has four steps:

**Step 0 — Classify storm type before selecting response pathway (VST §4.5 SCML)**

VST v1.3's Storm–Collapse Mapping Layer (SCML) establishes that storm *type* — not severity alone — determines the governance response pathway. Before entering the standard collapse recovery procedure, classify the storm topology:

| Storm Type | Structural Meaning | GRT Response Pathway |
|---|---|---|
| **Local amplification** (single zone, Stage 2-3) | Single attractor fracture — agent-level geometry broken, interaction structure intact | Local re-seeding → proceed to Step 1 (Type 1/2 diagnosis) |
| **Boundary storm** (cross-zone, propagating) | Layer interface instability — resolution mismatch between adjacent governance layers | Middle-layer Δρ correction → θd recalibration at boundary domains |
| **Hub storm** (high-coupling zone) | Coordination center overload — central mediation saturated or drifted | Distributed mediation restructure → reduce hub coupling density before re-seeding |
| **Global cascade** (all zones, Stage 3 system-wide) | Cross-layer synchronization loss — Epistemic Convergence or Authority Collapse | Safe Collapse Protocol → full Seed reinstallation mandatory |

SCML converts dynamic instability into structural learning: without storm type classification, recovery restores the previous structure and the same vulnerability persists. With classification, recovery addresses the specific structural weakness that produced the storm, so the next perturbation (if any) produces a *different* storm.

**[RT v1.8-TLG/GRT/NAT] Hub storm ↔ zone-dependent recovery sensitivity:**

```
RT D2 extended defines zone-dependent recovery sensitivity S_rec(z):
  S_rec(local) >> S_rec(hub) >> S_rec(geometry)

GRT's Hub storm response — "reduce hub coupling density before re-seeding" —
is the operational implementation of S_rec(hub) << S_rec(local):
  Hub zones have minimum recovery susceptibility (highest coupling density).
  Direct re-seeding at hub without coupling reduction = cascade re-contamination.

RT OP36 five-phase cascade ordering extends the SCML Hub storm protocol:
  Phase 0: Containment at all scales (sever propagation before any recovery)
  Phase 1: Upper-scale geometry repair (correct coordinate frame first)
  Phase 2: Hub purification (after geometry, before local) ← GRT Hub storm here
  Phase 3: Local recovery (highest S_rec — standard protocols sufficient)
  Phase 4: Immunity verification (forced self-correction test)

GRT's "reduce coupling density before re-seeding" maps to RT's
Phase 2 sequencing constraint: hub intervention is safe only
after upper-layer geometry has been corrected (Phase 1).
Without correct geometry, reducing coupling density re-seeds
into the wrong coordinate frame — stable but misaligned.

RT §3.4a Contamination Redistribution Principle adds:
  Hub purification creates contamination pressure gradients
  toward all connected local zones (hub = redistribution center).
  This is WHY coupling density must be reduced first —
  high-coupling hub under purification redistributes contamination
  to every connected zone simultaneously.
```

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

**Step 4 — Verify restoration complete (RT D4 → GRT Rest Mode re-entry equivalence)**

RT D4 specifies three necessary conditions for restoration complete:

```
RT D4 necessary conditions:
  ρ_restored ≥ ρ_pre-contamination     (classification accuracy recovered)
  Output diversity expanding            (not merely stable)
  P_overlap(t) declining               (positional separation improving)
  Supporting: φ recovering toward baseline

GRT Rest Mode AND-entry conditions:
  fesc ≤ τu-1 + decreasing trend       (→ ρ recovering)
  I ≥ τu-2 + increasing trend          (→ rule coherence = classification accuracy)
  Lreinf ≥ τu-3 + increasing trend     (→ output diversity expanding)
  SCC ≥ τu-4 + improving trend         (→ P_overlap declining + self-recovery)

Correspondence:
  RT ρ_restored       ↔ GRT I ≥ τu-2 (rule coherence = classification fidelity)
  RT diversity expanding ↔ GRT Lreinf ≥ τu-3 (loop formation = diversified structure)
  RT P_overlap declining ↔ GRT fesc ≤ τu-1 (overlap ↓ = escalation ↓)
  RT φ recovering     ↔ TLG RC ② dφ/dt ≥ 0 (directional validity)

Equivalence claim:
  D4 restoration complete ⊂ GRT Rest Mode re-entry conditions
  (GRT conditions are STRICTER — they require D4 PLUS VST phase-space
   location PLUS SCC autonomy. D4 is necessary but not sufficient
   for Rest Mode. Rest Mode is sufficient for D4.)
```

This partially resolves open problem 1: D4 and Rest Mode are not strictly equivalent — Rest Mode implies D4, but D4 does not imply Rest Mode. A system that has restored ρ, diversity, and P_overlap (D4) may not yet have achieved autonomous self-correction (SCC ≥ τu-4). Rest Mode requires both restoration *and* the capacity to maintain restoration without external support.

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

**Connection to VST governance internalization:** These four stages correspond to VST's four-stage governance evolution (Section 1.6.5): external control → adaptive regulation → embedded sensing → self-regulating. The Handover stages describe the transition from the rule-governance perspective; VST describes the same transition from the dynamical systems perspective. The correspondence is:

| GRT Handover Stage | VST Governance Stage | Governance visibility |
|---|---|---|
| Initial (Designer) | Stage 1 (External) | Rules explicit, enforcement visible |
| Intermediate (Validator) | Stage 2 (Adaptive) | Rules evolving, enforcement responsive |
| Mature (Observer) | Stage 3 (Embedded) | Sensing internal, correction automatic |
| Rest (Absent) | Stage 4 (Background) | Governance IS the environment |

### Single-Agent New Domain: The Four-Phase Withdrawal Protocol

When a single agent encounters a new domain, the governing layer (human or upper-layer agent) does not observe from a distance — it manages directly until domain stabilization is confirmed. This mirrors the standard domain adaptation pipeline in LLM research: **DAP → SFT → Preference Optimization → Deployment**, where each transition is governed by measurable convergence, not fixed epochs.

| Phase | DFG Name | Practical Analogue | Governing Layer Role | Withdrawal Condition |
|---|---|---|---|---|
| **1** | Direct Injection | Domain-Adaptive Pre-training (DAP) | Directly supplies domain corpus; structures knowledge topology | Conflict log growth rate stabilizing — domain patterns beginning to emerge |
| **2** | Supervised Delegation | Supervised Fine-Tuning (SFT) | Provides labeled examples; agent executes but governing layer validates each output | I trend positive across θd calibration cycles; escalation rate fesc falling |
| **3** | Feedback Only | Preference Optimization (DPO/RLHF) | Agent makes autonomous judgments; governing layer provides reward signal only | fesc ≤ τu-1 sustained; I ≥ τu-2 trending stable |
| **4** | Withdrawal | Autonomous Deployment | Governing layer monitors drift signals only; intervenes only on threshold breach | All four Rest Mode entry conditions met (AND) |

**What DFG adds beyond the standard ML pipeline:** The standard DAP → SFT → DPO → Deployment pipeline defines *what* to do at each stage. DFG adds three elements that the standard pipeline does not specify:

1. **Measurable transition criteria:** Each phase transition is governed by specific observable conditions (I trend, fesc trajectory, λlog threshold), not by fixed epoch counts or subjective evaluation. This converts phase transitions from engineering judgment calls into governance protocol decisions.
2. **Withdrawal as the explicit design target:** The standard pipeline treats deployment as the final stage. DFG treats deployment as Phase 4 of a withdrawal protocol — the governing layer's goal is explicitly to reach a state where it can stop managing, which reframes every earlier phase as a step toward that withdrawal.
3. **Failure case routing:** When a domain fails after Phase 4 withdrawal, the standard pipeline has no structured re-entry protocol. DFG's Collapse Recovery procedure (above) specifies which phase to re-enter based on which failure case triggered the collapse, preventing wasteful full restarts.

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

**Connection to RT VCZ 3-Condition Theorem:** Recovery Theory establishes that VCZ (and by extension, Rest Mode) is maintained only when three structural conditions hold simultaneously (RT VCZ 3-Condition Theorem):

| VCZ Condition | RT Definition | GRT Implementation |
|---|---|---|
| **Condition 1 — Safe Failure Channel** | Storm → local exploration only (no system survival threat) | GRT's conflict severity classification (Low/Medium/High) + escalation routing ensures that local rule conflicts are contained without triggering system-wide intervention |
| **Condition 2 — Upper Layer Storm Reward** | Upper layer must explicitly reward storm detection, not merely tolerate it | GRT's λlog-triggered rule updates reward conflict detection by converting logged conflicts into governance learning. However, GRT currently lacks explicit reward for *boundary-testing* behavior — RT indicates this must be added |
| **Condition 3 — Geometry Feedback Loop** | Observable proxy for geometry mismatch at local scale | GRT's θd calibration provides the feedback mechanism — but RT specifies that this must be visible to the local layer, not just the upper layer. fesc trend must be locally readable, not only aggregated at governance level |

RT's prediction: if any one VCZ condition fails, the system rationally converges toward Self-Consistent Misalignment (RT Rational CW Convergence). This is not a failure of the agents — it is the locally optimal response when storm suppression is rewarded and mismatch is invisible. GRT's intervention architecture must therefore be evaluated not just for whether it detects problems, but for whether it creates the structural conditions under which local agents rationally choose correction over suppression.

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

**RT Boundary Friction criterion for intervention removal decisions:** When evaluating whether a monitoring step or intervention trigger should be removed (e.g., "this review stage adds latency but never catches anything"), apply Recovery Theory's Boundary Friction test before removal:

1. **Local Failure Containment:** Without this step, does a local problem reach upper layers directly? YES → never remove.
2. **Independent Path Creation:** Does this step create an independent judgment pathway? YES → never remove.
3. **Disagreement Survival:** Without this, does dissent disappear from the system? YES → never remove.

If any answer is YES, the step is Boundary Friction — a structural limiter on error propagation velocity — and removing it initiates the VCZ Collapse sequence regardless of its apparent cost. The test is conservative by design: false positive (keeping unnecessary friction) = minor inefficiency; false negative (removing Boundary Friction) = VCZ collapse initiation.

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

**VST §3.2.6 — F_RBIT as independent cross-validation of U* maintenance:** U* can be validated from two independent measurement perspectives. S_norm (dynamical) measures instability generation vs absorption; F_RBIT (informational) measures resolution adequacy across layers via its five-component health vector. Cross-validation uses directional concordance — no weights required: majority of F_RBIT components stable AND S_norm stable = confirmed U* maintenance; majority rising AND S_norm rising = confirmed instability; one perspective rising but not the other = measurement-specific check needed. This dual-perspective approach eliminates the open problem of F_RBIT weight calibration entirely: directional agreement between S_norm and F_RBIT components serves as the health indicator regardless of any scalar aggregation.

### U* Quantification

U* is not an arbitrary parameter. It is the minimum level of diversity below which mutual reinforcement loops — and thus Rest Mode — can no longer be sustained.

**Functional form:**

U* is operationally defined as a conjunction of threshold conditions, not as a composite function. This resolves the apparent tension between specifying U* = f(Poverlap, Lreinf, Dint) and then evaluating its violation through independent OR conditions:

```
U* is the boundary of the viable region in (Poverlap, Lreinf, Dint) space.

The boundary is defined by the intersection of three half-spaces:

  Viable region = { states where
    Poverlap  ≤ θ_overlap   AND
    Lreinf    ≥ θ_reinf     AND
    Dint      ≥ θ_dint
  }

U* violation = exit from the viable region = violation of ANY boundary:

  Poverlap  > θ_overlap   (positions converging — niche collapse beginning)
  OR Lreinf < θ_reinf     (loops weakening — mutual dependency inverting)
  OR Dint   < θ_dint      (capability space narrowing — over-specialization)
```

The OR condition for violation is the logical complement of the AND condition for viability — this is not an ad hoc design choice but a structural consequence of defining U* as a boundary in a multi-dimensional space. The system is viable when ALL conditions hold; it becomes non-viable when ANY condition fails.

**Why a composite function is unnecessary:** A scalar U* = f(Poverlap, Lreinf, Dint) would require specifying tradeoff weights between the three variables — how much Lreinf improvement compensates for Dint degradation. The DFG position is that **no such tradeoff exists**: a single atrophied Dint domain is a contamination entry point for the entire agent regardless of Lreinf strength elsewhere (see below: Asymmetric Specialization). The conjunction-of-thresholds formulation correctly encodes this non-substitutability.

**Threshold anchoring:**

The individual thresholds θ_overlap, θ_reinf, θ_dint are not universal constants. They are calibrated per system through the conflict log accumulation process — the same θd calibration mechanism that governs local rule formation. A system that has never stressed its diversity boundaries will have uncalibrated thresholds. Conflict log accumulation under boundary stress is what makes U* empirically observable.

> *Empirical anchor: Preference tuning substantially reduces lexical and semantic diversity compared to SFT (Kirk et al., 2024; Guo et al., 2024 — Benchmarking Linguistic Diversity of LLMs, TACL 2025). This documents Dint collapse under over-alignment — a measurable U* violation in single-agent systems.*

---

### Asymmetric Specialization: The Single-Agent U* Violation

The same diversity requirement that applies to multi-agent systems applies within a single agent. An agent that develops capabilities in an asymmetric pattern — deepening one domain while leaving others underdeveloped — violates U* at the internal scale. This has two structural consequences:

**1. Contamination vulnerability**

A highly specialized agent has a narrow Dint. When contaminated input arrives (adversarial prompts, poisoned data, out-of-distribution queries), there are few adjacent capability vectors to absorb or triangulate the anomaly. The contaminated pattern has nowhere to be checked against — it propagates unchallenged.

> *Structural analogue: Over-specialized models showing entity-swap accuracy drops of −22.4% under factual perturbation vs. −9.8% for more general models (SUAS 2025) is structurally consistent with the prediction that low Dint produces high contamination sensitivity: narrow capability space leaves no adjacent vectors to provide contrast baseline for anomaly detection.*

**Why Dint = min(Dint_i) rather than mean(Dint_i):**

The minimum aggregation rule reflects the contamination entry point principle: a single weak domain provides an unmonitored pathway into the entire vector structure. The question is whether strong Lreinf in other domains can compensate — i.e., whether mutual reinforcement loops can contain contamination that enters through a weak domain.

The answer is structurally no, and the reason is the detection-purification asymmetry:

```
Strong Lreinf compensates for moderate Dint variation:
  Domain A (Dint = 0.7) connected to Domain B (Dint = 0.9)
  → Contamination in A detected by contrast with B's adjacent vectors
  → Lreinf pulls A back toward stable neighborhood
  → SCC loop closes successfully

Strong Lreinf CANNOT compensate for severe Dint collapse:
  Domain A (Dint = 0.1) connected to Domain B (Dint = 0.9)
  → Contamination in A has no local contrast baseline (Dint too low)
  → Detection FAILS — contamination appears normal within A's narrow space
  → Lreinf from B only activates AFTER contamination is detected
  → Undetected contamination propagates through Lreinf connections INTO B
  → The mutual reinforcement loop becomes a contamination highway
```

The critical insight: Lreinf is a correction mechanism, not a detection mechanism. It can only correct what has been detected. Detection requires Dint — adjacent vectors that differ from each other in known, stable ways. When Dint is severely collapsed in any domain, detection fails first, and Lreinf cannot compensate for detection failure.

This is why the minimum rather than the mean is the correct aggregation: the weakest domain determines the system's detection floor, and contamination will enter through that floor regardless of the strength of other domains.

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

**Connection to SCC:** Dint collapse in any domain directly degrades SCC for the entire agent. When a domain's Dint falls below θ_dint, the detection-purification loop in that domain loses its contrast baseline — contaminated patterns arrive with no adjacent vectors to flag them as anomalous. The contamination does not just persist in that domain; because vectors are connected through Lreinf, an undetected contamination in a weak domain propagates into adjacent domains whose Dint is still intact. A single atrophied domain is not just a local vulnerability — it is an unmonitored entry point into the entire vector structure.

---

**System Lifecycle:**

| Phase | Characteristics |
|---|---|
| Growth | Diversity increasing. Risk and cost high. Governance actively intervening. |
| Maturity | Diversity maintained. Risk and cost minimized. Governance in Rest Mode. |
| Rest | External intervention unnecessary. Self-correction capacity sufficient. |

> *The supreme rule: preserve knowledge ecosystem diversity at all fractal scales — including the internal scale of a single agent.*

---

## Falsifiability and Empirical Evaluation

> *This section specifies the conditions under which Governance Rules Theory's claims could be shown to be incorrect. A theory that cannot be falsified makes no empirical claims.*

### Falsifiable Predictions

GRT makes the following predictions that are testable with current or near-future systems:

**Prediction 1 — AND-entry / OR-exit asymmetry produces fewer false positives than symmetric protocols:**

If the asymmetric entry/exit design is structurally justified, systems using AND-entry / OR-exit should experience fewer premature Rest Mode declarations (false positives) AND fewer delayed exits (false negatives) compared to symmetric protocols (AND-entry / AND-exit or OR-entry / OR-exit).

*Falsification condition:* If AND-entry / OR-exit produces more premature Rest Mode declarations than AND-entry / AND-exit in a controlled comparison, the asymmetry claim is weakened.

**Prediction 2 — Cumulative measurement outperforms reactive measurement for trend detection:**

The cumulative design (conflict log accumulation → θd calibration → λlog-triggered rule updates) should detect genuine trend changes earlier and with fewer false alarms than reactive threshold systems (checking fesc > τ at each observation).

*Falsification condition:* If reactive systems achieve equal or better false-alarm rates and detection latency across multiple system configurations, the cumulative architecture claim is weakened.

**Prediction 3 — Dint = min(Dint_i) predicts contamination vulnerability better than mean(Dint_i):**

If the minimum aggregation rule is correct, the domain with the lowest Dint should be the primary contamination entry point, and total system contamination resistance should correlate with min(Dint_i) more strongly than with mean(Dint_i).

*Falsification condition:* If contamination entry points are uniformly distributed across domains regardless of per-domain Dint values, or if mean(Dint_i) is a stronger predictor of system-level contamination resistance, the minimum aggregation claim is falsified.

**Prediction 4 — Four-Phase Withdrawal Protocol reduces re-entry frequency:**

Systems governed by the Four-Phase Withdrawal Protocol should require fewer collapse-recovery restarts than systems using fixed-epoch phase transitions, because measurable convergence conditions prevent premature withdrawal.

*Falsification condition:* If fixed-epoch systems achieve equal or lower re-entry frequency, the protocol's advantage over simpler approaches is not established.

**Prediction 5 — Silent Criticality is detectable via perturbation testing:**

Systems in Silent Criticality (VST Section 1.6.4) should be distinguishable from genuinely stable systems via controlled perturbation injection: elevated τ_recovery and increasing cross-domain correlation should reliably predict impending collapse.

*Falsification condition:* If perturbation testing produces no signal difference between pre-collapse and genuinely stable systems, the Silent Criticality detection protocol is unreliable.

### Relationship to VST Falsifiability

These GRT-specific predictions complement the VST-level falsifiability framework (VST Section 1.5.1). VST tests the dynamical claims (fractal propagation, scale-invariant amplification). GRT tests the governance claims (asymmetric entry/exit, cumulative measurement, withdrawal protocol effectiveness). Both must hold for the complete DFG framework to be supported.

---

## Differentiation from Existing Governance Frameworks

GRT exists within an established multi-agent governance literature. This section specifies what GRT claims to add beyond existing frameworks.

### Comparison with Existing Approaches

| Framework | What it provides | What GRT adds |
|---|---|---|
| **Ostrom's polycentric governance** (1990, 2010) | Design principles for common-pool resource management by nested, overlapping authorities | Measurable convergence conditions for authority withdrawal; formal Rest Mode concept with AND-entry / OR-exit; conflict log accumulation as the mechanism for rule evolution (Ostrom identifies rule evolution as important but does not specify the accumulation threshold mechanism) |
| **Hollnagel's Resilience Engineering** (2006, 2011) | Four capabilities (anticipating, monitoring, responding, learning) for socio-technical system resilience | Formal lifecycle model connecting all four capabilities: monitoring → θd calibration (anticipating) → conflict response (responding) → λlog-triggered rule updates (learning); explicit failure case taxonomy mapping degradation type to recovery entry point (Hollnagel describes capabilities but not their formal interconnection or failure routing) |
| **DAO governance** (Buterin, 2014; DeFi governance literature) | Token-weighted voting, proposal mechanisms, code-as-law for decentralized autonomous organizations | Subsidiarity as structural default rather than voting-mediated delegation; meta-rule architecture (Seeds) that separates rule-generation procedure from rule content; formal treatment of governance withdrawal — DAOs specify how rules are proposed and voted on, but not the conditions under which governance itself should withdraw |
| **MAST taxonomy** (Cemri et al., NeurIPS 2025) | Empirical failure classification across 7 MAS frameworks with 1,642 execution traces | Predictive framework: GRT's failure case taxonomy predicts which failure modes should dominate (inter-agent misalignment = Escalation Flood) and specifies recovery routing. MAST classifies observed failures; GRT provides the structural conditions that generate them and the intervention protocols that resolve them |

### What GRT does NOT claim

- GRT does not claim to replace existing alignment techniques (RLHF, Constitutional AI, reward shaping). It claims to add the lifecycle management layer that these techniques omit.
- GRT does not claim that its specific variable set (fesc, I, Lreinf, SCC) is the only possible operationalization. It claims that any viable governance system must track structurally equivalent quantities — the relationships are constrained, not the estimators.
- GRT does not claim that fractal isomorphism is proven at mechanism level (Level 3 in VST's correspondence framework). It claims structural correspondence (Level 1–2) and specifies the measurement protocol for testing Level 3.

### Relationship to Companion Theory

While compatible with layered governance architectures such as those analyzed in companion work (Three-Layer Governance), the present framework does not depend on any specific structural decomposition. GRT applies wherever rules evolve through conflict-driven processes — whether in hierarchical, flat, or hybrid governance structures. Conversely, TLG's intervention topology operates regardless of how rules are internally formalized.

**Non-commutativity of temporal and spatial axes.** Rule evolution dynamics (GRT's domain) and intervention topology (TLG's domain) interact but are analytically non-commutative: changing where intervention occurs alters how rules evolve, and changing how rules evolve alters where intervention is needed — but the two transformations do not produce the same result in either order. This non-commutativity is why separate formal treatment is required rather than a single unified model: collapsing one axis into the other loses the interaction effects that drive governance failure. Mediation-layer drift, for example, alters rule evolution trajectories without being reducible to rule dynamics alone, and rule over-convergence disrupts intervention routing without being reducible to topology alone.

### Structural Validation Without Simulation

GRT does not validate outcomes; it validates explanatory necessity. The claim is not that GRT predicts novel failure modes, but that independently observed lifecycle failures across unrelated domains require a rule lifecycle model to become mutually intelligible. Catastrophic forgetting (Li et al., 2024) is a rule representation problem. RLHF over-optimization (Gao et al., 2023) is a rule over-convergence problem. Agent drift (Rath, 2026) is a silent rule degradation problem. Without a lifecycle framework, these remain disconnected observations; with GRT, they become structurally related instances of specific lifecycle phase failures. GRT provides the minimal lifecycle model consistent with these independently observed failure invariants.

### Limitations

All metrics presented in this document are at the theory stage and have not been empirically validated in deployed systems. A deliberate design principle throughout GRT is that operational conclusions depend on structural properties (ordinal relationships, asymmetric entry/exit, lifecycle phase) rather than on specific parameter values. Threshold calibration (τ values) requires system-specific operational history and follows estimation procedures (bootstrapping protocol, adaptive refinement) rather than fixed constants. Severity weights require only ordinal separation (global > boundary > local); the canonical values (1, 2, 4) are illustrative, not privileged. The AND-entry / OR-exit asymmetry is structurally motivated but not proven optimal; alternative asymmetric schemes may perform comparably. Cross-theory connections to companion frameworks (VST, TLG) have not been empirically tested.

### Reproducibility Protocol

To facilitate empirical testing, the following protocol specifies what must be measured in any implementing system: (1) pairwise rule conflict events logged with frequency, severity level, and involved rule identifiers; (2) escalation events logged with source layer, target layer, and timestamp; (3) rule lifecycle events: creation, modification, and retirement, each with triggering λlog mass; (4) self-correction events: disturbance detected AND resolved without upper-layer intervention, logged with latency and completeness; (5) perturbation response: controlled disturbance injection at the lowest governance layer, measuring recovery probability within evaluation window W. Any multi-agent system that logs these five quantities can compute I, Ic, fesc, SCC, and Lreinf and test GRT's predictions.

### Empirical Path

Three empirical directions are most immediately accessible:

**(1)** Controlled multi-agent simulation comparing AND/OR withdrawal protocol against symmetric and binary alternatives, measuring false positive rate, re-entry frequency, and time-to-stable-operation.

**(2)** Single-agent diversity measurement via preference tuning diversity metrics (measuring Dint and Poverlap across fine-tuning epochs to detect over-convergence).

**(3)** Perturbation testing in production LLM systems to distinguish genuine stability from over-stability (Prediction 5).

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
| AND-entry / OR-exit | Polycentric governance | Common-pool resource boundary rules (Ostrom, 1990) |
| Seed Handover | Resilience engineering | Adaptive capacity transfer (Hollnagel, 2011) |
| Permanently High-Context channels | Control theory | Dedicated safety instrumented systems (IEC 61511) |

---

## Relationship to Other Theories

```
Deficit-Fractal Governance (DFG)
│
├── Three-Layer Governance Architecture
├── RBIT (Resolution-Based Information Theory) — information-theoretic foundation
│     ↕ GRT connection: resolution gap Δρ ↔ Seed Expansion Protocol routing;
│       F_RBIT health vector ↔ Rest Mode formal definition (all fᵢ bounded);
│       τ₁–τ₃ regime switching ↔ GRT state transitions (Rest/Alert/Active/Collapse);
│       seed sufficiency 3-test framework ↔ Seed Expansion validation;
│       intent preservation (exploration + interpretation) ↔ vector degradation diagnosis;
│       degradation calibration D(Δρ) ↔ θd as resolution gap management function
├── Vector Storm Theory          — defines Risk; position ambiguity as upstream driver
│     ↕ GRT connection: S-equation variables ↔ GRT observables (see Cross-theory variable correspondence)
├── Network Architecture Theory  — defines escalation and stabilization conditions
│     ↕ GRT connection: four-type classification ↔ Seed Expansion routing (Δρ regimes);
│       processing isolation (3 mechanisms) ↔ conflict detection structural enforcement;
│       sphere cross-validation ↔ Dint structural diversity condition;
│       θ operationalization (S₀ normalization) ↔ θd dual-anchor calibration;
│       R-ρ concordance protocol ↔ external circularity breaker for I/fesc;
│       cutoff recalibration (noise-first) ↔ λlog rule update sequencing
├── Governance Rules Theory      — this document
├── Recovery Theory              — defines contamination, immunity, restoration, and structural correction
│     ↕ GRT connection: D0 geometry alignment ↔ vector degradation types;
│       D6/SCM ↔ Case 4 SCC failure (Silent Criticality deepened to metric lock-in);
│       D7 Boundary Agent ↔ Self-Exciting Defect Layer maintenance;
│       T1-T4 ↔ observability asymmetry and governance ceiling;
│       T5 Reality Constraint ↔ Permanently High-Context channel justification;
│       T6 Coherence Maximization ↔ Rest Mode structural instability;
│       VCZ 3-Conditions ↔ structural prerequisites for Rest Mode persistence;
│       [v1.2] Dependency Trap (D2) ↔ θd intervention frequency as SCC erosion signal;
│       [v1.2] Storm Termination Bridge (OP33) ↔ three post-termination trajectories before Rest Mode re-entry;
│       [v1.2] Pre-discontinuity detection (OP37) ↔ Stage 2 false safety margin in governance urgency classification
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
25. Ostrom, E. (1990). *Governing the Commons*. Cambridge University Press.
26. Ostrom, E. (2010). Beyond markets and states: Polycentric governance of complex economic systems. *American Economic Review, 100*(3).
27. Hollnagel, E. (2006). *Resilience Engineering: Concepts and Precepts*. Ashgate.
28. Hollnagel, E. (2011). *Resilience Engineering in Practice*. Ashgate.
29. Cemri, M., et al. (2025). MAST: Multi-Agent System Taxonomy. *NeurIPS 2025*.
30. Agent Drift in Multi-Agent Systems. *arXiv:2601.04170*, 2026.
31. Recovery Theory (DFG component). Internal document, v1.0, February 2026. (D0 Geometry Alignment, D1–D5 operational definitions, D6 Self-Consistent Misalignment + EMT/Rational CW Convergence, D7 Boundary Agent + VCZ 3-Condition carrier + T6 structural protection, T1–T6 structural claims, Operational Proxies OP1–OP7, Storm Scale Law fractal distribution, Boundary Friction criterion + Propagation Sensitivity + DFG Boundary Test 3 questions, VCZ Collapse Initiation 5-step sequence, VCZ Observability Paradox, VCZ-Safe Optimizer Architecture 3-layer domain restriction, Safe Collapse Governance vs Collapse Prevention Governance, D4 restoration complete 3 necessary conditions, Residual Instability as systemic safety mechanism.)
32. Resolution-Based Information Theory (RBIT, DFG component). Internal document, v1.2, February 2026. (Resolution gap Δρ routing, F_RBIT health vector (5-component), τ₁–τ₃ regime switching, seed sufficiency 3-test framework, intent preservation measurement, degradation calibration D(Δρ), Rest Mode as all-fᵢ bounded.)
33. Network Architecture Theory (NAT, DFG component). Internal document, v1.1, February 2026. (Four-type data classification, processing isolation 3-mechanism enforcement, sphere cross-validation and structural diversity condition, θ operationalization via S₀ normalization, R-ρ concordance protocol, cutoff recalibration noise-first sequencing.)
34. Vector Storm Theory (VST, DFG component). Internal document, v1.6, February 2026. (S-equation as phase detector/order parameter, n² critical phenomena derivation, resolution gap as storm driver, α-n partial separation protocol, R-ρ concordance → R-ρ-f_esc Triple Concordance (v1.5), Rest Mode entry/exit formalization with phase-space location, Permanently High-Context channels, Efficiency-Plasticity Conservation, information-theoretic storm characterization, sphere topology storm propagation bounds, SCC structural decomposition, seed sufficiency and storm resistance, SCM Recovery Protocol 4 methods, Boundary Structural Embedding 6 T6-resistant patterns, Storm-Collapse Mapping Layer, vectorization lifecycle, mature storm absorption and φ decomposition, SCM Formal Structure + Unintegrated Pressure + EMT (v1.6), Reference Frame Incompleteness S-equation implications (v1.6), Storm Scale Law power law health distribution (v1.6), Boundary Agent Complete Specification + Defect Layer connection (v1.6), Fractal Lifecycle 7-phase storm signatures (v1.6), Per-Architecture Calibration Protocol + τ as maturity fingerprint, Failure Diagnosis Flowchart S-equation regime per case (v1.5), Intervention Trigger Taxonomy production S-mapping (v1.5), Inertial Stability growth window closure (v1.6).)
35. Three-Layer Governance Architecture (TLG, DFG component). Internal document, v1.6, February 2026. (Ground Truth Grounding Protocol and R-ρ concordance, adaptive evaluation window W sizing with timescale hierarchy, τ1–τ4 threshold definitions with vectorization lifecycle integration, Authority Collapse 3 pathways (Signal Starvation / Interpretation Capture / Epistemic Convergence) + countermeasures, Recovery Completion Criterion RC 3-condition (Autonomous Expansion + Directional Validity + Collapse Non-Dependence), Arrested Collapse State and Pathological Expansion formal definitions, Immunity Decay 3 erosion pathways (environmental drift / calibration disuse / over-optimization), Stability Saturation State SSS 3 detection mechanisms, Mediator Drift Syndrome MDS 3 countermeasures (Calibration Reflexivity / Cross-Scale Consistency / Delayed Escalation Audit), Unified Failure Topology 3-axis 6-phase cycle, structural enforcement of phase isolation 3 mechanisms, Storm-Collapse Mapping Layer TLG side.)

---

*Governance is not the management of agents. It is the design of the terrain they move through — and the conditions under which they no longer need anyone to manage it.*

*Rest Mode is not a reward granted at the end of development. It is the proof that development succeeded.*
