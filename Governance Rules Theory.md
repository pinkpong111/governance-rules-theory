# Governance Rules Theory

**Meta-Rule Architecture, Consistency Measurement, and Rest Mode**

> A component theory of **Deficit-Fractal Governance (DFG)**  
> Companion theories: [Vector Storm Theory] · [Network Architecture Theory]
> 
> **Version: v1.6-expanded** (March 2026) — Major expansion: AGM integration (Affective Gain Module coupling), Endogenous Perturbation Theory, T_eff governance temperature formalization, Bifurcation-Failure taxonomy unification, Momentum-bearing vector dynamics, Flow-Rest Mode equivalence, Stochastic Freedom as landscape design requirement, Weight Dynamics as AGM gain modulation
>
> v1.6-expanded changes from v1.5-expanded:
> - **AGM ↔ GRT Integration Protocol:** Full bidirectional coupling specification, T_eff as governance temperature parameter, endogenous perturbation source formalization, stochastic weight redistribution as correction value mechanism
> - **Endogenous Perturbation Theory:** Self-Exciting Defect Layer formalized as AGM's controlled stochastic freedom, T_eff > T_min as structural invariant of Rest Mode, Kramers escape rate as governance transition mechanism
> - **Bifurcation-Failure Taxonomy Unification:** GRT's 5 failure cases mapped to AGM's Freeze/Runaway universality classes, codimension-1 bifurcation at governance criticality, sensitivity s(t) as bifurcation type discriminator
> - **Momentum-Bearing Vector Dynamics:** Vectorization extended with momentum p_i(t), inertia effects on governance transitions, momentum-governance coupling non-commutativity
> - **Flow-Rest Mode Equivalence Theorem:** AGM flow state = GRT Rest Mode at single-agent level, four-condition AND-entry maps to AGM's κ≈κ*, S≪1, δ≈0, H≫H_crit
> - **Stochastic Freedom as Landscape Design Requirement:** Controlled noise as necessary governance component, Adaptive Necessity Theorem integration, No-Free-Lunch Constraint on governance
> - **Governance Temperature Regulation:** T_eff self-tuning through θd calibration, temperature-barrier phase transition at landscape complexity boundary, minimum viable temperature derivation from conflict log statistics
> - All previous content preserved.
>
> v1.5-expanded changes from v1.4-expanded:
> - **Core Principles formal cost model:** Intervention cost function C_int(t) with landscape design cost amortization, intervention ROI formalization, scale-dependent efficiency proof, connection to VST terrain formation economics
> - **Rule Architecture conflict resolution protocol:** Formal priority resolution algorithm, conflict detection latency bounds, multi-rule conflict cascade handling, rule version management with rollback conditions, temporal consistency guarantees
> - **Meta-Rule completeness conditions:** Gödel-inspired incompleteness bound, meta-rule sufficiency criteria, seed expressiveness theorem, expansion completeness guarantee under stationarity
> - **Vectorization dynamics model:** Promotion rate equation, λlog accumulation kinetics, noise-to-vector transition probability, vectorization phase portrait in (log_mass, classification_confidence) space, connection to nucleation theory
> - **Consistency Index convergence:** I(t) convergence theorem under bounded conflict arrival, convergence rate bounds, oscillation damping conditions, M normalization stability proof
> - **Position Clarity niche dynamics:** Niche differentiation dynamics with Lotka-Volterra structural analogy, competitive exclusion principle for agent positions, niche width optimization, Poverlap measurement protocol
> - **State transition energy barriers:** Helmholtz free energy analogy for governance states, activation energy for Rest→Active transition, metastability analysis, transition rate estimation via Kramers theory analogy
> - **Expanded Falsifiability (10 predictions):** Added predictions 6-10 covering energy barrier asymmetry, niche differentiation speed, vectorization rate scaling, governance entropy production, cross-theory concordance reliability
> - **Structural Correspondence deepening:** Mathematical structure mapping for each correspondence pair, isomorphism level classification, predictive power comparison
> - **Game-theoretic governance foundations:** Agent compliance as Nash equilibrium under landscape design, defection cost analysis, mechanism design connection, incentive compatibility of Rest Mode
> - **Governance Entropy theory:** Governance system entropy production, entropy bounds for Rest Mode, minimum entropy production principle, connection to Prigogine dissipative structures
> - All previous content preserved.
>
> v1.4-expanded changes from v1.3-RTseries:
> - **Bootstrapping Protocol mathematical formalization:** Phase 0-3 formal entry/exit conditions, backward transition conditions, convergence guarantees, multi-domain coordination, duration estimation, VST phase-space trajectory mapping
> - **Fractal Collapse Propagation information-theoretic extension:** Collapse velocity model, entropy production rate as predictor, cross-layer MI cascade dynamics, containment protocol, RBIT channel capacity connection
> - **U* Quantification critical phenomena connection:** Phase transition structure with order/control parameters, critical scaling predictions, hysteresis at U* boundary, measurement protocol (perturbation-response/correlation/fluctuation), multi-scale fractal U*
> - **Production Implementation Guide:** Five-component architecture, monitoring dashboard specification, alert hierarchy, deployment checklist
> - **Cross-theory Integration Architecture:** Full integration topology, bilateral protocols for VST/RT/RBIT/NAT/TLG, validation concordance matrix (6 concordance pairs)
> - All previous content preserved.
>
> v1.3-RTseries changes from v1.2 (RT-1/2/3/4 v2.0 integration):
> - **Recovery Theory connections extended:** RT-1 three restoration conditions mapped to state transitions; RT-2 Metric Lock-In deepens Case 4 to structural invisibility; RT-3 observer (V,A,B,S) mapped to monitoring requirements; RT-4 Shared Vulnerability as conflict-is-governance-resource; Identity Declaration as premature Rest Mode risk; Structural Humility as θd verification persistence
> - All previous content preserved.
>
> v1.2 changes from v1.1 (RT v1.8-VST + VST v1.8-RT integration pass):

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

**Formal Cost Model — Intervention Economics:**

The distinction between landscape design and direct intervention has a formal cost structure that explains why landscape design dominates at scale:

```
Direct Intervention cost:
  C_direct(t, n) = c_event · n · f_event(t)
  
  where:
    c_event = per-event intervention cost (human review, compute, latency)
    n = number of agents or domains under governance
    f_event(t) = event frequency requiring intervention at time t
    
  Scaling: O(n) per timestep — linear in system size
  Temporal: persistent — C_direct does not decrease over time
           unless agent behavior changes (which requires investment)
  
  Total cost over horizon T:
    C_direct_total = ∫₀ᵀ c_event · n · f_event(t) dt = O(n · T)
    (assuming approximately constant event rate)

Landscape Design cost:
  C_landscape(t, n) = c_design · g(n) + c_maintain(t) · h(n)
  
  where:
    c_design = one-time terrain construction cost (rule architecture,
               Seed design, correction value landscape installation)
    g(n) = design scaling function — sub-linear in n because terrain
            affects all agents simultaneously: g(n) ≈ n^{1/d_eff}
            where d_eff is the effective governance dimension (VST §1.6.2)
    c_maintain(t) = terrain maintenance cost at time t
    h(n) = maintenance scaling — sub-linear because maintenance is
            per-rule, not per-agent: h(n) ≈ log(n) for well-structured
            rule architectures
    
  Scaling: O(n^{1/d_eff}) initial + O(log n) ongoing
  Temporal: amortizing — c_maintain(t) decreases as terrain stabilizes:
    c_maintain(t) = c_maintain(0) · (1 + t/τ_terrain)^{-γ}
    where τ_terrain is the terrain formation timescale and γ > 0
    is the stabilization rate
  
  Total cost over horizon T:
    C_landscape_total ≈ c_design · n^{1/d_eff} + c_maintain(0) · log(n) · τ_terrain/γ
    = O(n^{1/d_eff} + log(n))

Cost crossover point:
  C_direct_total = C_landscape_total at critical system size n*:
    n* ≈ (c_design / c_event)^{d_eff/(d_eff-1)} · (γ / τ_terrain · T)^{d_eff/(d_eff-1)}
    
  For n > n*: landscape design strictly dominates
  For n < n*: direct intervention may be cheaper
  
  The crossover point n* decreases as:
    - d_eff decreases (more structured terrain → better scaling)
    - T increases (longer horizon → more amortization time)
    - γ increases (faster terrain stabilization)
    
  In mature systems (d_eff → 1, T >> τ_terrain):
    n* → (c_design / c_event) — a small constant
    → landscape design dominates for essentially any non-trivial system size
```

**Intervention ROI and Governance Investment Theorem:**

The cost model yields a formal return-on-investment statement for governance investment:

```
Governance ROI:
  ROI_governance = (C_direct_avoided - C_landscape_invested) / C_landscape_invested
  
  = (c_event · n · T · f_event - c_design · n^{1/d_eff} - c_maintain_total) 
    / (c_design · n^{1/d_eff} + c_maintain_total)

  For large n and T:
    ROI_governance ≈ (c_event · n · T) / (c_design · n^{1/d_eff})
    = (c_event / c_design) · n^{1 - 1/d_eff} · T
    
  ROI grows polynomially in system size and linearly in time horizon.
  This is the formal justification for why governance investment is
  front-loaded but return is compounding.

Governance Investment Theorem:
  For any system with n > n* agents and governance horizon T > τ_terrain:
    The optimal governance strategy allocates maximum investment to
    terrain formation (landscape design) in the initial period [0, τ_terrain],
    transitioning to maintenance investment in [τ_terrain, T].
    
  Proof sketch:
    The landscape cost function C_landscape(t,n) has decreasing marginal cost
    in t (amortization) and sub-linear cost in n (shared terrain).
    The direct intervention cost C_direct(t,n) has constant marginal cost
    in both t and n. Any mixed strategy that allocates resources to both
    can be improved by shifting initial allocation toward landscape design,
    because the amortization benefit compounds over the remaining horizon.
    
  Connection to VST: the terrain formation timescale τ_terrain corresponds
  to VST's Phase 3 (Formation) in the 7-phase lifecycle. Governance
  investment efficiency is maximized during Phases 1-3 when terrain is
  actively forming — investment during Phase 5 (Rest Mode) yields
  diminishing returns because the terrain is already established.
```

**Game-Theoretic Foundation — Landscape Design as Mechanism Design:**

The landscape design principle has a game-theoretic formalization that connects GRT to classical mechanism design theory:

```
Agent Decision Model:
  Each agent i chooses action a_i from action space A_i
  to maximize local utility u_i(a_i, a_{-i}, θ)
  where θ represents the governance terrain parameters
  
  Under direct intervention:
    θ = θ_fixed (terrain unchanged)
    Governance constrains action space: a_i ∈ A_i^restricted
    Agent plays: argmax_{a_i ∈ A_i^restricted} u_i(a_i, a_{-i}, θ_fixed)
    Problem: when restriction removed, agent reverts to unrestricted optimum
    
  Under landscape design:
    θ = θ_designed (terrain modified)
    Action space unrestricted: a_i ∈ A_i
    Agent plays: argmax_{a_i ∈ A_i} u_i(a_i, a_{-i}, θ_designed)
    Result: optimal action under designed terrain aligns with governance objective
    
  Incentive Compatibility Condition:
    Landscape design achieves incentive compatibility when:
    argmax_{a_i} u_i(a_i, a_{-i}, θ_designed) ∈ G
    for all i, where G is the set of governance-compliant actions
    
    This is exactly the mechanism design condition:
    the governance-optimal action is the agent's selfish optimum
    under the designed terrain.
    
  Rest Mode as Nash Equilibrium:
    Rest Mode corresponds to the state where the action profile
    a* = (a*_1, ..., a*_n) is a Nash equilibrium under θ_designed:
    No agent can improve its utility by unilateral deviation.
    
    This is why Rest Mode is self-sustaining: departure from the
    equilibrium profile is locally suboptimal for each agent,
    requiring no external enforcement to maintain.
    
  Connection to VCZ:
    The VCZ (Viable Convergence Zone) in VST is the basin of attraction
    of this Nash equilibrium in the dynamical system.
    VCZ boundary = boundary of the region where a* remains stable
    under perturbation.
    
  Why direct intervention fails as mechanism design:
    Direct intervention restricts the action space A_i without
    modifying the utility landscape u_i. The agent's true optimum
    remains outside A_i^restricted. This creates:
    - Enforcement cost: continuous monitoring to maintain restriction
    - Gaming incentive: agents seek boundary exploits
    - Brittleness: restriction removal → immediate reversion
    
    Landscape design modifies u_i itself (through θ), so the
    agent's true optimum shifts to governance-aligned action.
    No enforcement required at equilibrium.
```

Existing AI alignment techniques already implement landscape design:
- **RLHF** — shapes the output space without per-inference intervention
- **Constitutional AI** — replaces per-output correction with governing principles
- **Reward shaping** — modifies the agent's value terrain while preserving the optimal policy

**AGM Integration — Stochastic Freedom as Landscape Design Requirement:**

The Affective Gain Module (AGM §1.1) establishes a fundamental constraint on landscape design that GRT must incorporate: **no landscape design can be complete without an endogenous perturbation mechanism**. This follows from AGM's Adaptive Necessity Theorem:

```
Adaptive Necessity Theorem (AGM Theorem 1):

  For a finite-capacity optimizer in a non-stationary environment
  with drift rate ||dE/dt|| > 0:
  
    If T_eff = 0 (zero stochastic exploration) for all t > t₀:
      → Ω_eff(t) → 0 (effective exploration space vanishes)
      → E[τ_adapt(ΔE)] → ∞ (expected adaptation time diverges)
      
  Corollary: any adaptive system intended for indefinite operation
  must maintain T_eff > T_min > 0

GRT Implication — Controlled Noise as Governance Component:
  
  Landscape design shapes the terrain to make optimal actions easiest.
  But a perfectly shaped landscape with zero noise STILL fails:
    - The landscape is designed for environment E(t₀)
    - When E shifts, the agent is trapped in the previous optimum
    - The deeper the landscape design made the basin, the harder escape becomes
    
  Resolution:
    Landscape design must include a NOISE BUDGET — a deliberate allocation
    of controlled stochastic perturbation that prevents attractor lock-in:
    
    C_landscape_complete = C_terrain + C_noise_maintenance
    
    where C_noise_maintenance = cost of maintaining T_eff > T_min
    
  This is why the Self-Exciting Defect Layer (VST §1.6.5) is not
  optional infrastructure but a NECESSARY component of landscape design:
    Defect Layer = endogenous perturbation source = T_eff > 0 guarantee
    
  Without the Defect Layer, landscape design produces:
    - Perfect convergence to the designed attractor
    - Zero ability to escape when the attractor becomes obsolete
    - The landscape designer's own assumptions become attractor lock-in
    = the most dangerous form of governance failure (SCM through design)

No-Free-Lunch Constraint on Governance (AGM Theorem 1.3):
  
  No governance policy π can simultaneously satisfy:
    (1) Zero instantaneous regret (J(π) = J* at all t)
    (2) Positive adaptation capacity (|H(t)| > 0 at all t)
    (3) Finite endurance budget (total cost bounded)
    
  Any two of three can be achieved, but not all three.
  
  GRT resolves this by sacrificing (1) in a controlled manner:
    Rest Mode accepts bounded instantaneous suboptimality
    (the system is not perfectly optimized at every instant)
    to maintain (2) within the budget of (3).
    
  This is the formal justification for why Rest Mode is not
  zero governance cost — the irreducible cost IS the noise budget
  that maintains adaptation capacity.
  
  Connection to Governance Entropy Theory:
    S_min > 0 (governance entropy never zero) is the entropy
    expression of T_min > 0 (temperature never zero).
    Both state the same structural invariant:
    maintaining an ordered state requires minimum dissipation.
```

**AGM's Minimum Viable Temperature as GRT Governance Parameter:**

The governance temperature T_eff can be operationalized through GRT's existing measurement infrastructure:

```
T_eff Operationalization through GRT Variables:

  T_eff ∝ λlog_update_rate × conflict_diversity × SR
  
  where:
    λlog_update_rate = rate of rule updates (governance learning activity)
    conflict_diversity = entropy of conflict type distribution
    SR = surprise rate (system's capacity to encounter novelty)
    
  T_eff estimation from conflict logs:
    T_eff(t) ≈ k_T · H(conflict_log(W)) / W
    
    where H is Shannon entropy of conflict types in window W
    and k_T is calibrated from Phase 0 baseline
    
  T_eff monitoring thresholds:
    T_eff > T_max: system is stochastically dominated
      = too much noise relative to signal
      = Runaway risk (AGM terminology)
      = GRT: fesc exploding, I collapsing
      
    T_eff ∈ [T_min, T_max]: healthy governance temperature
      = adaptive capacity maintained within performance bounds
      = GRT: Rest Mode or healthy Active Mode
      
    T_eff < T_min: attractor lock-in approaching
      = insufficient exploration to track environmental change
      = Freeze risk (AGM terminology)
      = GRT: SSS onset, SR → 0, SCM entry
      
    T_eff ≈ 0: governance death
      = no learning, no adaptation, no surprise
      = GRT: all λlog updates ceased, full metric lock-in
      
  The T_eff measurement adds a UNIFIED early warning
  that subsumes multiple existing GRT detection protocols:
    SR → 0 is a T_eff < T_min signal
    SSS is a T_eff → 0 signal
    SCM is a T_eff = 0 + accumulated mismatch signal
    All three are temperature pathologies, distinguished by duration
```

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

### Formal Conflict Resolution Protocol

When rules conflict, the system must resolve the conflict deterministically and within bounded time. The following protocol specifies the resolution algorithm, handling multi-rule cascades and ensuring temporal consistency:

```
Conflict Resolution Algorithm (CRA):

Input: Conflicting rule set R_conflict = {r_1, r_2, ..., r_k}
Output: Resolution action + updated conflict log + rule status updates

Step 1 — Priority Classification:
  For each rule pair (r_i, r_j) in R_conflict:
    Classify by rule type combination:
      Global-Global: severity = High → immediate Ic tracking
      Global-Local:  severity = Medium → global executes, local suspended
      Local-Local:   severity = Low → resolve within layer
      
Step 2 — Precedence Resolution:
  Apply lexicographic precedence ordering:
    Level 1: Global > Local (absolute priority)
    Level 2: Within same level: older rule > newer rule (stability bias)
    Level 3: Within same age: rule with larger λlog support > rule with less
             (evidence-based tiebreaker)
    Level 4: If still tied: both rules suspended, escalated to upper layer
    
  The lexicographic ordering ensures deterministic resolution
  without requiring real-valued priority weights.

Step 3 — Multi-Rule Cascade Handling:
  When |R_conflict| > 2 (more than two rules in simultaneous conflict):
    
    Cascade detection:
      If resolving (r_1, r_2) creates new conflict with r_3:
        → cascade flag raised
        → cascade depth counter incremented
        
    Cascade depth limit:
      If cascade_depth > D_max (default D_max = 3):
        → halt cascade resolution
        → suspend all rules in cascade chain
        → escalate entire chain to upper layer as single conflict event
        → log as "cascade conflict" with full chain trace
        
    Cascade depth limit prevents infinite resolution loops
    and ensures bounded resolution time.

Step 4 — Temporal Consistency Guarantee:
  All conflict resolutions must satisfy temporal consistency:
    If rule r_a was applied at time t_1, and conflict detected at t_2 > t_1:
      → r_a's effects during [t_1, t_2] are NOT retroactively reversed
      → resolution applies from t_2 forward only
      → conflict log records both the application period and the
        resolution timestamp
        
  This prevents temporal paradoxes where conflict resolution
  invalidates actions already taken — which would create
  second-order conflicts with any decisions based on those actions.

Step 5 — Rule Version Management:
  When a rule is modified through λlog-triggered update:
    → previous version archived (immutable — Write-Asymmetry)
    → new version assigned monotonically increasing version number
    → rollback condition: if new version produces I decline > Δ_rollback
      within one θd calibration cycle, automatic revert to previous version
    → rollback is itself logged as a conflict event
    
  Version history serves dual purpose:
    - Audit trail for governance accountability
    - Rollback capability for failed rule modifications
    
  Rollback depth limit: maximum 1 rollback per rule per evaluation window
  (prevents oscillation between versions)
```

**Conflict Resolution Latency Bounds:**

The conflict resolution protocol must complete within bounded time to prevent governance deadlock:

```
Latency bounds by severity:

  Low severity (Local-Local):
    Resolution time: T_resolve ≤ τ_θd / 10
    (must resolve within 10% of one θd calibration cycle)
    Justification: local conflicts are frequent and individually low-impact;
    slow resolution would create a queue that degrades I over time
    
  Medium severity (Global-Local):
    Resolution time: T_resolve ≤ τ_θd
    (must resolve within one θd calibration cycle)
    Justification: requires upper-layer validation but should not
    block multiple calibration cycles
    
  High severity (Global-Global):
    Resolution time: T_resolve ≤ W (evaluation window)
    (may require full evaluation window for human-AI collaboration)
    Justification: governance redesign requires deliberation;
    the evaluation window is the natural timescale for strategic decisions
    
  Cascade resolution:
    Total cascade resolution time: T_cascade ≤ D_max · T_resolve(highest_severity)
    (bounded by cascade depth limit × highest-severity resolution time)

If any latency bound is exceeded:
  → resolution classified as "deadlocked"
  → all rules in deadlock set suspended
  → system operates under global rules only until deadlock resolved
  → deadlock event logged with severity = High (triggers Ic tracking)
```

**Rule Interaction Graph:**

The rule architecture forms a directed graph whose structure determines conflict propagation dynamics:

```
Rule Interaction Graph G_rules = (V, E):

  Vertices V = {all active rules}
  Edges E = {(r_i, r_j) : r_i and r_j can potentially conflict}
  
  Edge weight: w_ij from wij operationalization (frequency × severity)
  Edge direction: r_i → r_j if r_i has higher precedence than r_j
  
  Graph properties relevant to governance:
  
    In-degree of r_i = number of rules that can override r_i
    Out-degree of r_i = number of rules that r_i can override
    
    Global rules: high out-degree, zero in-degree (override others, never overridden)
    Local rules: variable out-degree, positive in-degree
    
    Strongly connected components in G_rules indicate
    circular dependency clusters where no rule has clear precedence
    → these clusters must be resolved by the lexicographic ordering
    in Step 2, or escalated as structural design flaws
    
    Graph diameter D(G_rules) bounds the maximum cascade depth:
    D_max should be set to D(G_rules) to ensure all cascades
    can propagate through the full graph before being halted
    
  Connection to VST propagation:
    G_rules is the rule-layer projection of the interaction topology
    that VST's S-equation operates on. Conflicts propagating through
    G_rules correspond to governance-layer perturbation propagation.
    The spectral gap of G_rules (λ₁ − λ₂) predicts conflict
    dissipation rate — large gap → fast resolution, small gap →
    persistent conflict oscillation.
```

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

**Meta-Rule Formal Properties:**

Meta-rules occupy a distinct logical level from object-level rules. This level separation has formal properties that constrain what meta-rules can and cannot accomplish:

```
Logical Level Hierarchy:

  Level 0 (Object rules): specific behavioral constraints
    Example: "Escalation threshold for domain D is θ_D = 0.7"
    
  Level 1 (Meta-rules): rules about rule creation, modification, retirement
    Example: "Rules may only change when conflict log exceeds λlog"
    
  Level 2 (Meta²-rules): rules about meta-rule modification
    Example: "Meta-rules change only at Seed Handover transitions"
    
  Level separation principle:
    Level k rules constrain Level (k-1) rules
    Level k rules are NOT constrained by Level (k-1) rules
    Cross-level constraint is strictly downward
    
  GRT implements three levels:
    Level 0 = local rules (domain-specific thresholds, penalties, advantages)
    Level 1 = meta-rules (Seeds — procedure for rule generation)
    Level 2 = meta²-rules (Seed update conditions, global rule modification protocol)
    
  The DFG framework does not require Level 3+ because:
    Level 2 rules are externally anchored (T5 — Reality Constraint)
    rather than self-governing. Human oversight at Level 2 prevents
    the infinite regress that would otherwise require unbounded levels.
```

**Meta-Rule Completeness Conditions:**

A meta-rule set is *complete* for a domain if it can generate appropriate object-level rules for any input the domain may encounter. Completeness is not guaranteed — and its absence has structural consequences:

```
Completeness Definition:
  A meta-rule set M is complete for domain D if:
    For all possible inputs x ∈ D:
      M generates a classification C(x) within finite steps
      AND M generates a response rule R(x) consistent with C(x)
      AND R(x) does not contradict any global rule

Sufficiency Theorem (conditional):
  A meta-rule set M is complete for domain D if and only if:
    Condition 1 (Classification coverage):
      M's data type taxonomy covers all input types in D
      (every input can be classified under at least one type)
      
    Condition 2 (Response generation):
      For each data type in M's taxonomy, M specifies a response
      generation procedure (not necessarily a specific response —
      a procedure for constructing one)
      
    Condition 3 (Consistency preservation):
      The response generation procedure preserves I ≥ τ2
      (new rules do not systematically degrade consistency)

Incompleteness Bound (Gödel-inspired):
  No finite meta-rule set M can be complete for an unbounded domain D.
  
  Proof sketch:
    If D is unbounded (can produce inputs of arbitrary novelty),
    then for any finite classification taxonomy T with |T| = k types,
    there exists an input x* ∈ D that does not fit any type in T.
    (Diagonal argument: construct x* by combining features that
    each type excludes.)
    
    This means: M cannot pre-specify rules for all possible inputs.
    M must contain a *procedure* for handling unclassifiable inputs.
    This procedure is the Seed Expansion Protocol.
    
  Structural consequence:
    The Seed Expansion Protocol is not an optional extension —
    it is a NECESSARY component of any meta-rule set governing
    an unbounded domain. Without it, the meta-rule set is
    structurally incomplete and will produce hard failures
    (Case 5 — Seed Corruption) on first encounter with
    truly novel input.
    
  Connection to RBIT:
    RBIT's resolution gap Δρ is the information-theoretic measure
    of the distance between the current meta-rule set's coverage
    and the input's actual complexity. Δρ = 0 means the meta-rule
    set can handle the input; Δρ < 0 means it cannot (incompleteness
    for this specific input). The Expansion Protocol bridges the gap
    by accumulating conflict log evidence until coverage extends.

Seed Expressiveness Theorem:
  A Seed S is expressively adequate for domain D if:
    S can generate rules for any input pattern that appears
    with probability > p_min over evaluation window W
    
  Formally:
    For all x ∈ D with P(x|W) > p_min:
      S generates R(x) within T_max steps
      where T_max = λlog / rate(conflict_events_for_x)
      
  Expressiveness is probabilistic, not absolute:
    S need not handle inputs of arbitrarily low probability.
    The p_min threshold corresponds to the λlog threshold:
    inputs appearing too rarely never accumulate sufficient
    conflict log mass to trigger rule formation.
    
  This is correct behavior: extremely rare inputs should remain
  as noise (uncultivated) rather than triggering premature
  rule formation from insufficient evidence.

Expansion Completeness Guarantee (under stationarity):
  If the Seed Expansion Protocol operates on a locally stationary domain
  (Condition 2 of Bootstrapping Convergence Guarantees) and the seed
  passes all three RBIT Sufficiency Tests:
    
    The meta-rule coverage converges:
      lim_{t→∞} P(unclassifiable input | t) → 0
      at rate proportional to the conflict log accumulation rate
      
    This means: given sufficient time and interaction volume,
    the meta-rule set approaches completeness for the stationary domain.
    
    The convergence is asymptotic — completeness is approached
    but never fully achieved (consistent with the Incompleteness Bound).
    The practical question is whether the convergence rate is fast
    enough relative to the domain's stationarity timescale.
```

**Meta-Rule Interaction with Object Rules — Constraint Propagation:**

Meta-rules constrain object rules, but this constraint propagation has a specific direction and dynamics:

```
Constraint Propagation Model:

  When meta-rule m_j is modified (e.g., at Seed Handover):
    All object rules generated by m_j must be re-validated
    
    Re-validation cascade:
      For each rule r_i generated under m_j:
        Check: is r_i still consistent with m_j_new?
        If yes: r_i retained
        If no:  r_i flagged for revision
                → enters Supervised Delegation cycle
                → agent proposes revised r_i' under m_j_new
                → upper layer validates
                
    Cascade cost:
      C_meta_change = |{r_i : r_i generated by m_j}| · c_revalidation
      
      This cost is why meta-rule changes are rare and gated:
      each meta-rule change propagates through ALL dependent object rules.
      Frequent meta-rule changes produce perpetual re-validation,
      preventing object-rule convergence and blocking Phase 2+ entry.
      
    Meta-rule modification frequency bound:
      f_meta_change ≤ 1 / (T_revalidation_cascade · n_dependent_rules)
      
      This ensures the system completes one full re-validation cascade
      before the next meta-rule change occurs — preventing cascade overlap
      that would produce unbounded governance load.
```

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

### Bootstrapping Protocol: Mathematical Formalization

The Seed Expansion Protocol operates through a phase-structured bootstrapping procedure. Each phase has formal entry/exit conditions, measurable convergence criteria, and structural guarantees that prevent premature transition. This formalization resolves the open question of how θd calibration initializes in the absence of prior operational history — the "cold earth" problem of governance bootstrapping.

**Phase Structure and Formal Transitions:**

The bootstrapping procedure consists of four phases, each corresponding to a distinct governance regime. Transitions between phases are unidirectional under normal operation (Phase 0 → 1 → 2 → 3) but permit backward transitions under specific failure conditions:

```
Phase 0 — Direct Management (Upper layer controls all decisions)
  Entry: system initialization OR Collapse recovery restart
  Exit condition: conflict_log_count(domain_d) ≥ N_min AND
                  classification_accuracy(domain_d) ≥ ρ_min
  
  Governance regime:
    θd = θd_max (maximum sensitivity — all deviations escalated)
    λlog = ∞ (no autonomous rule updates permitted)
    Intervention granularity: per-event
    
  Mathematical constraint:
    During Phase 0, the system operates as a supervised learner:
    R_local(t) = R_upper(t) + ε(t)
    where R_local is the local rule applied, R_upper is the upper-layer
    directive, and ε(t) is the implementation variance.
    
    Phase 0 exit requires: Var(ε(t)) < σ²_max over window W₀
    (local implementation variance bounded — agent can reliably execute
    upper-layer directives before being trusted with autonomous proposals)

Phase 1 — Supervised Delegation (Agent proposes, upper layer validates)
  Entry: Phase 0 exit conditions met
  Exit condition: validation_acceptance_rate ≥ ρ_accept AND
                  I_local ≥ I_min AND
                  θd converging (dθd/dt → 0 within calibration window)
  
  Governance regime:
    θd = θd_initial (calibrated from Phase 0 conflict logs)
    λlog = λlog_conservative (high threshold — many events required
           before rule update permitted)
    Intervention granularity: per-rule (not per-event)
    
  Mathematical constraint:
    Phase 1 implements a validation loop:
    P(accept | R_proposed) = f(I_local, conflict_severity, domain_novelty)
    
    The acceptance function f must satisfy monotonicity:
      ∂f/∂I_local > 0 (higher consistency → higher acceptance probability)
      ∂f/∂conflict_severity < 0 (higher severity → lower acceptance)
      ∂f/∂domain_novelty < 0 (higher novelty → lower acceptance)
    
    Phase 1 exit requires: acceptance rate stabilized above ρ_accept
    for ≥ 2 consecutive θd calibration cycles (trend confirmation, not
    single-point measurement)

Phase 2 — Feedback Only (Agent acts, upper layer provides reward signal)
  Entry: Phase 1 exit conditions met
  Exit condition: SCC ≥ τu-4 AND
                  Lreinf/n ≥ τu-3 AND
                  autonomous_resolution_rate ≥ ρ_auto
  
  Governance regime:
    θd = θd_calibrated (adaptive, EWMA-updated)
    λlog = λlog_standard (domain-appropriate threshold)
    Intervention granularity: per-distribution (statistical monitoring)
    
  Mathematical constraint:
    Phase 2 implements a reinforcement loop:
    ΔR_local(t+1) = η · feedback(t) · ∇_R L(R_local(t), observed_outcomes)
    
    where η is the update rate (governed by λlog), feedback(t) is the
    upper-layer reward signal, and L is the local loss function.
    
    Phase 2 exit requires: 
      d(feedback_dependency)/dt < 0 sustained
      (agent is decreasingly dependent on external feedback for correct
      rule application — self-correction replacing external correction)

Phase 3 — Rest Mode (Self-sustaining governance)
  Entry: Phase 2 exit conditions met AND all Rest Mode AND-entry conditions
  Exit: any OR-exit condition triggered (see Rest Mode Exit Conditions)
  
  Governance regime:
    θd = θd_stable (slow EWMA update, long time constant)
    λlog = λlog_mature (domain-calibrated)
    Intervention granularity: per-distribution only
    SCC self-maintaining through detection-purification loop
```

**Backward Transition Conditions:**

Phase transitions are not irreversible. Specific failure conditions trigger backward transitions that restart the bootstrapping from the appropriate phase:

```
Phase 3 → Phase 2:
  Trigger: SCC < τu-4 sustained (self-correction failing)
  BUT: I ≥ τu-2 (rule coherence intact) AND Lreinf ≥ τu-3 (loops active)
  → agent needs feedback signal to recalibrate, not structural rebuild

Phase 3 → Phase 1:
  Trigger: I < τu-2 sustained (rule coherence collapsing)
  OR: Lreinf < τu-3 sustained (loops collapsing)
  → agent's autonomous rule management has degraded; needs validation

Phase 3 → Phase 0:
  Trigger: SCC < τu-4 AND I < τu-2 AND Lreinf < τu-3
  OR: Seed Corruption detected (Case 5)
  → full structural rebuild required from substrate

Phase 2 → Phase 1:
  Trigger: autonomous_resolution_rate declining AND
           validation_acceptance_rate (if measured) declining
  → feedback-only regime insufficient; validation needed

Phase 2 → Phase 0:
  Trigger: feedback_response_quality < ρ_min
  → agent cannot use feedback signal effectively; direct management needed

Phase 1 → Phase 0:
  Trigger: validation_acceptance_rate < ρ_accept for ≥ 2 calibration cycles
  → proposals consistently rejected; supervised learning restart needed
```

**Convergence Guarantees:**

The bootstrapping procedure converges to Phase 3 (Rest Mode) under three structural conditions:

```
Condition 1 — Seed adequacy:
  The installed Seed passes all three RBIT Sufficiency Tests
  (geometry update capacity, contamination recognition, orthogonal recovery)
  
  If Seed is inadequate: bootstrapping oscillates between Phase 0 and Phase 1
  indefinitely — Phase 2 is unreachable because SCC ceiling is imposed
  by seed architecture (see: RBIT SCC ceiling theorem)

Condition 2 — Environmental stationarity (local):
  The domain's statistical properties change slower than the θd
  calibration timescale:
    T_environment_change >> T_θd_calibration
    
  If violated: θd never converges → Phase 1 exit blocked
  → domain remains permanently in Phase 1 or is reclassified as
    Permanently High-Context

Condition 3 — Sufficient interaction volume:
  The conflict log accumulates events at a rate sufficient for
  statistical significance within the evaluation window:
    N_events_per_window ≥ N_min_statistical
    
  If violated: trend measurement unreliable → all phase transitions
  blocked by insufficient evidence → system remains in current phase
  
  Structural consequence: low-interaction domains bootstrap slower
  than high-interaction domains. This is correct behavior — confidence
  requires evidence, and evidence requires interaction.
```

**Connection to VST Phase-Space Trajectory:**

The four bootstrapping phases trace a characteristic trajectory through VST's phase space:

```
Phase 0: S_norm high, R >> 1, C(t) ≈ 0 (external correction)
  → trajectory: moving toward VCZ boundary from outside
  
Phase 1: S_norm decreasing, R → 1, C(t) building
  → trajectory: approaching VCZ boundary
  
Phase 2: S_norm < S_c, R ≈ 1, C(t) stabilizing
  → trajectory: inside VCZ, moving toward interior
  
Phase 3: S_norm << S_c, R ≈ 1⁻, C(t) self-maintaining
  → trajectory: deep VCZ interior (Rest Mode)
```

The phase-space trajectory provides an independent validation of bootstrapping progress: if a domain claims to be in Phase 2 but its S_norm remains near S_c, the phase classification is suspect — operational metrics and dynamical location should agree. Disagreement triggers the R-ρ-fesc Triple Concordance check.

**Multi-Domain Bootstrapping Coordination:**

When a system has multiple domains bootstrapping simultaneously, a coordination constraint applies:

```
Independence principle:
  Each domain bootstraps independently through Phases 0-3
  Domain A in Phase 3 does not require Domain B to also be Phase 3
  
Interaction constraint:
  Cross-domain interactions use the minimum phase of the two domains:
    Phase_interaction(A,B) = min(Phase_A, Phase_B)
    
  Rationale: if Domain A is in Phase 3 (autonomous) but Domain B is
  in Phase 0 (supervised), interactions between A and B must be
  supervised — the Phase 0 domain's uncertainty propagates through
  the interaction channel.

System-level Rest Mode:
  System enters Rest Mode when ALL domains are individually in Phase 3
  AND cross-domain interaction phases are all Phase 3
  
  This is the multi-domain extension of the AND-entry condition:
  the system's overall phase = min(Phase_d) across all domains d
```

**Bootstrapping Duration Estimation:**

The expected bootstrapping duration from Phase 0 to Phase 3 depends on three measurable quantities:

```
T_bootstrap ≈ T_Phase0 + T_Phase1 + T_Phase2

where:
  T_Phase0 ≈ N_min / r_event × W₀
    (minimum events required / event rate × evaluation window)
    
  T_Phase1 ≈ 2 × T_θd_calibration × (1 / ρ_accept_initial)
    (two calibration cycles × inverse initial acceptance rate)
    
  T_Phase2 ≈ T_SCC_convergence + T_Lreinf_formation
    (self-correction capacity convergence + loop formation time)

Typical scaling:
  High-interaction domain: T_bootstrap ≈ O(weeks)
  Medium-interaction domain: T_bootstrap ≈ O(months)
  Low-interaction domain: T_bootstrap ≈ O(quarters)
  
  These are order-of-magnitude estimates for production LLM systems
  with continuous input streams. Batch-processed systems will scale
  differently based on batch frequency and size.
```

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
| **F_gov** | Governance free energy | ℝ | What is the system's thermodynamic governance state? |
| **S_gov** | Governance entropy | ≥ 0 | How disordered is the governance action distribution? |
| **σ_gov** | Governance entropy production rate | ℝ | Is governance entropy increasing or decreasing? |
| **T_gov** | Governance temperature | > 0 | How much fluctuation does the environment produce? |
| **ΔF** | Energy barrier between governance states | ≥ 0 | How much perturbation is needed to trigger a state transition? |
| **L_p** | Conflict log mass for pattern p | ≥ 0 | How much evidence has accumulated for this pattern? |
| **C_p** | Classification confidence for pattern p | [0, 1] | How reliably can this pattern be classified? |
| **J_vec** | Vectorization rate | ≥ 0 | How fast are new patterns being promoted from noise to vector? |
| **α_ij** | Niche competition coefficient | [0, ∞) | How much does agent j's niche overlap with agent i's? |
| **x_i** | Agent i's niche width | [0, 1] | What fraction of capability space does agent i occupy? |
| **δI_ij** | Consistency cost of rule pair (i,j) | [0, 1] | How much does this specific rule pair degrade I? |
| **v_collapse** | Collapse propagation velocity | ≥ 0 | How fast is collapse spreading through the governance structure? |
| **MI_cross** | Cross-layer mutual information | ≥ 0 | How correlated are nominally independent governance layers? |
| **T_eff** | Governance effective temperature (AGM) | ≥ 0 | What is the system's exploration capacity via stochastic perturbation? |
| **T_min** | Minimum viable temperature (AGM) | > 0 | Below what T_eff does attractor lock-in become inevitable? |
| **s(t)** | Sensitivity parameter (AGM) | [0, 1] | How responsive is the system to novel perturbation? |
| **p_i(t)** | Momentum of vector i (AGM) | ℝ | What accumulated inertia does this governance direction carry? |
| **P_system** | Aggregate system momentum (AGM) | ≥ 0 | How much total inertia is the governance system carrying? |
| **σ** | Stochastic perturbation intensity (AGM) | ≥ 0 | How much controlled noise is the system maintaining? |
| **κ** | Exploration-interpretation ratio (AGM) | ≥ 0 | What is the balance between search and classification? |
| **δ(t)** | Anchor misalignment (AGM) | [0, 2] | How far is the current direction from the identity anchor? |
| **H(t)** | Endurance reserve (AGM) | [0, 1] | How much governance capacity remains before exhaustion? |

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

**Vectorization Dynamics — Mathematical Model:**

The transition from noise to vector is not instantaneous — it follows a dynamics that can be modeled as a nucleation process with measurable kinetics:

```
Vectorization State Variables:
  For each input pattern p:
    L_p(t) = accumulated conflict log mass for pattern p at time t
    C_p(t) = classification confidence for pattern p at time t
    
  L_p evolves by accumulation:
    dL_p/dt = r_encounter(p) · s(p) - λ_decay · L_p(t)
    
    where:
      r_encounter(p) = rate at which pattern p is encountered
      s(p) = mean severity of conflicts involving p
      λ_decay = log mass decay rate (prevents stale patterns
                from maintaining vector status indefinitely)
    
    Steady state: L_p* = r_encounter(p) · s(p) / λ_decay
    
  C_p evolves by classification feedback:
    dC_p/dt = η_class · [accuracy(p, t) - C_p(t)] · (L_p(t) / λlog)
    
    where:
      η_class = classification learning rate
      accuracy(p, t) = observed classification accuracy for p
      The (L_p / λlog) factor ensures classification confidence
      builds only as log mass accumulates — preventing premature
      high confidence from a few lucky classifications

Promotion Criterion:
  Pattern p is promoted from noise to vector when:
    L_p(t) ≥ λlog  AND  C_p(t) ≥ C_min
    
  Both conditions must hold simultaneously:
    L_p ≥ λlog alone: sufficient evidence of recurring pattern
    C_p ≥ C_min alone: sufficient confidence in classification
    Both together: recurring pattern that can be reliably classified

Vectorization Phase Portrait:
  The (L_p, C_p) phase space has four regions:

    Region I (L < λlog, C < C_min):    NOISE
      Pattern is unknown and unclassified
      Governance action: hold in high-sensitivity state
      
    Region II (L ≥ λlog, C < C_min):   AMBIGUOUS RECURRING
      Pattern recurs frequently but cannot be reliably classified
      Governance action: maintain conservative escalation
      This region is dangerous — accumulating without understanding
      May indicate: novel data type requiring Seed Expansion
      
    Region III (L < λlog, C ≥ C_min):  SPORADIC RECOGNIZED
      Pattern can be classified when encountered but appears rarely
      Governance action: classify when encountered, no rule formation
      Insufficient mass for rule generation despite recognition ability
      
    Region IV (L ≥ λlog, C ≥ C_min):   VECTOR
      Pattern recurs frequently and is reliably classified
      Governance action: local rule formation permitted
      
  Phase portrait dynamics:
    Typical trajectory: I → II or III → IV (noise → vector)
    Reverse trajectory: IV → III or II → I (vector degradation)
    
    The trajectory through phase space encodes the vectorization
    history and predicts future stability:
    - Patterns that entered IV via Region II (high mass, low confidence)
      are more vulnerable to Type 1 degradation (alignment severance)
      because their classification pathway was weakly established
    - Patterns that entered IV via Region III (low mass, high confidence)
      are more vulnerable to stagnation (L_p decaying below λlog)
      if encounter rate drops
```

**Connection to Nucleation Theory:**

The vectorization process is structurally analogous to nucleation in physics — the formation of a new phase (vector) from a metastable phase (noise):

```
Nucleation Analogy:
  
  Noise → Vector transition:
    = supersaturated solution → crystal formation
    
  Conflict log mass L_p = supersaturation degree
    Higher L_p = greater thermodynamic driving force for crystallization
    
  Classification confidence C_p = crystal lattice order
    Higher C_p = more ordered structure with lower energy
    
  λlog = critical nucleus size
    Below λlog: dissolution more likely than growth
    (noise state is more stable than incipient vector state)
    Above λlog: growth self-sustaining
    (vector state is more stable — local rule formation begins)
    
  Critical nucleus analogy explains:
    - Why sub-threshold patterns dissolve (log mass decays below λlog)
    - Why promotion is irreversible under normal conditions
      (above critical size, growth is thermodynamically favored)
    - Why the promotion rate depends on encounter frequency
      (nucleation rate depends on supersaturation rate)
      
  Vectorization rate equation (nucleation rate analogy):
    J_vectorization = J₀ · exp(-ΔG* / kT_governance)
    
    where:
      J₀ = attempt frequency (rate of new pattern encounters)
      ΔG* = activation barrier = f(λlog, C_min)
             (higher thresholds → higher barrier → slower vectorization)
      kT_governance = governance "temperature" = system's tolerance
             for noise (higher temperature → more noise tolerated →
             faster vectorization of marginal patterns)
             
    In Phase 0 (θd_max): kT_governance is low (maximum sensitivity,
      low noise tolerance) → only high-quality patterns vectorize
    In Phase 2 (θd_calibrated): kT_governance is moderate →
      balanced vectorization rate
    Over-optimization: kT_governance → 0 → vectorization ceases
      entirely → system cannot learn new patterns → SSS onset
      
  Prediction: vectorization rate should decrease as the system
  matures (more patterns already vectorized → less noise to promote)
  and increase during environmental change (new patterns appearing →
  more noise requiring promotion). This prediction is testable
  by tracking vectorization events per evaluation window over time.
```

**Momentum-Bearing Vector Dynamics (AGM §4.3 Integration):**

Vectors in the governance system are not mere directional markers — they are **momentum-bearing entities** whose accumulated history creates inertia that resists change:

```
Momentum Extension of Vector Model:

  Standard vectorization (GRT v1.5):
    v_i(t) = directional vector (position in capability space)
    L_i(t) = accumulated conflict log mass
    C_i(t) = classification confidence
    
  Momentum extension (AGM integration):
    p_i(t) = momentum vector for pattern i
    
    p_i(t+1) = ρ · p_i(t) + κ · Δv_i(t)
    
    where:
      ρ ∈ (0, 1) = momentum decay rate (how quickly history fades)
      κ = coupling coefficient (how strongly new events affect momentum)
      Δv_i(t) = directional change from most recent conflict resolution
    
  The momentum term has three structural consequences:
  
  1. Governance Inertia:
     High-momentum vectors resist redirection even when θd calibration
     indicates the direction should change. The governance force required
     to reverse a vector's trajectory is proportional to ||p_i||:
       F_required = ||p_i|| / τ_reversal
     
     This explains why well-established governance patterns are hard
     to change even when clearly dysfunctional — the accumulated
     momentum exceeds the available correction force.
     
  2. Momentum-Governance Non-Commutativity (AGM Prop 4.2):
     The order of governance intervention and vector evolution matters:
       D^{intervene→evolve}(t+1) ≠ D^{evolve→intervene}(t+1)
     
     The non-commutativity gap is bounded by:
       ||gap|| ≤ 2σ · ||p(t)|| · A_t · (1 - cos(D(t), target))
     
     where A_t is the intervention magnitude and the cosine measures
     alignment between current direction and governance target.
     
     The gap VANISHES when:
       (a) no momentum exists (p = 0) — new system, no history
       (b) intervention is infinitesimal (A_t = 0)
       (c) system is already aligned (D parallel to target)
       
     The gap is MAXIMIZED during:
       high-momentum, large-intervention, misaligned states
       = crisis conditions where intervention sequencing matters most
     
     GRT implication: during Collapse Recovery (Step 1-4),
     the ORDER of recovery steps affects outcomes.
     The procedure specifies Step 0 (classify storm type) BEFORE
     Step 1 (diagnose degradation) precisely because of this
     non-commutativity — misclassifying the storm type produces
     a different (and worse) trajectory than classifying correctly
     even if the same recovery actions are eventually taken.
     
  3. Momentum as Storm Predictor:
     Aggregate momentum across all vectors:
       P_system(t) = Σ_i w_i(t) · ||p_i(t)||
     
     High P_system indicates the system is moving fast in established
     directions with high inertia — resistant to course correction.
     
     Rising P_system + declining T_eff = Freeze approach signal
     (system hardening into current trajectory without exploration)
     
     Rising P_system + rising T_eff = Storm amplification signal
     (high momentum + high noise = large amplitude oscillations)
     
     P_system can be measured from conflict log velocity:
     the rate and direction of conflict resolution decisions
     over evaluation windows reveals the momentum field.
```

**Weight Dynamics as Stochastic Redistribution (AGM §4.1):**

GRT's correction values operate as weight redistribution on a governance simplex, connecting directly to AGM's emotion-as-weight-redistribution formalism:

```
Weight Redistribution Model:

  The governance decision direction at any point is:
    D(t) = Σ_i w_i(t) · v_i(t)
    
  where w_i are the weights assigned to each governance vector
  (rule influence, domain priority, intervention allocation)
  and v_i are the vectors (rule directions, domain directions).
  
  Correction values modify weights:
    w_i(t+1) = w_i(t) + Δw_i^correction(t) + σ · ξ_i(t)
    
  where:
    Δw_i^correction = deterministic correction from conflict resolution
    σ · ξ_i = stochastic perturbation (controlled noise)
    
  The weights live on the simplex: Σ_i w_i = 1, w_i ≥ 0
  
  This means correction values are ZERO-SUM operations:
    Amplifying one vector's influence necessarily reduces others'
    Governance cannot create or destroy total decision capacity
    It can only redistribute attention across domains
    
  AGM Structural Insight:
    This zero-sum property explains why governance feels like
    a tradeoff rather than a free improvement:
    investing more governance attention in one domain necessarily
    reduces attention available for others.
    
    The optimal allocation problem is:
      w*(t) = argmax_w Σ_i w_i · value_i(t)
      subject to: Σ w_i = 1, w_i ≥ 0
      
    But this optimal allocation changes as the environment shifts,
    and the stochastic term σ·ξ ensures the system explores
    alternative allocations rather than locking into the current optimum.

  Connection to AGM's Emotional State Transition:
    Different governance regimes correspond to different weight
    configurations on the simplex, and transitions between regimes
    follow the distance metric on the simplex:
    
    P(regime_i → regime_j) ∝ exp(-||w^i - w^j||² / 2σ²·H(t))
    
    Nearby regimes on the simplex transition easily;
    distant regimes require either large events or sustained pressure.
    This is why gradual governance transitions (Active → Rest)
    are typical, while sudden transitions (Rest → Collapse)
    are rare but catastrophic — they require large simplex traversal.
```

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

### Consistency Index Convergence Theory

The Consistency Index I is a dynamical quantity whose trajectory determines governance state. The following convergence analysis establishes when and how I converges, providing formal guarantees that underpin the governance state machine:

```
I(t) Evolution Equation:

  I(t) = 1 - Σ wij(t) / M(t)
  
  Time derivative:
    dI/dt = -(1/M) · d(Σ wij)/dt + (Σ wij / M²) · dM/dt
    
  Under normal operation (no τ re-estimation trigger):
    dM/dt ≥ 0 (M is monotonically non-decreasing)
    → second term ≥ 0 (M increasing pushes I upward)
    
  Therefore:
    dI/dt ≥ -(1/M) · d(Σ wij)/dt
    
  I increases when conflict mass decreases faster than M grows.
  I decreases when conflict mass increases faster than M's
  stabilizing effect.

Convergence Theorem (under bounded conflict arrival):
  
  If the conflict arrival process satisfies:
    (A1) Bounded rate: E[number of new conflicts per window W] ≤ N_max
    (A2) Bounded severity: max severity = s_max (finite)
    (A3) Conflict resolution: resolved conflicts reduce wij
         at rate r_resolve ≥ r_min > 0
    (A4) Stationarity: conflict arrival distribution is stationary
         over timescale >> W
         
  Then:
    I(t) converges to a limit I* ∈ (0, 1] as t → ∞
    
    I* = 1 - (N_max · s_max · f_max) / (M · r_resolve)
    
    where f_max is the maximum pairwise conflict frequency
    
  Convergence rate:
    |I(t) - I*| ≤ K · exp(-r_resolve · t)
    
    where K depends on the initial distance |I(0) - I*|
    
  This exponential convergence rate means:
    - I converges faster when conflict resolution rate is higher
    - I converges slower when conflict arrival rate is higher
    - The convergence timescale τ_I = 1/r_resolve can be estimated
      from observed resolution rates

Oscillation Damping Conditions:
  I(t) may oscillate during convergence (e.g., during Phase 1 when
  new rules are being proposed and sometimes rejected). Oscillation
  is damped when:
    
    Condition: r_resolve > 2 · r_conflict_generation
    (resolution rate exceeds twice the conflict generation rate)
    
    When this condition holds:
      Oscillation amplitude decays as exp(-[r_resolve - 2·r_gen] · t)
      
    When this condition is violated:
      Oscillation can be sustained or growing
      = I does not converge = system cannot achieve Rest Mode
      = structural signal that Phase 2+ is not achievable without
        reducing conflict generation rate or increasing resolution capacity
      
    Governance implication:
      If I oscillates without damping for > 2 θd calibration cycles:
        → domain reclassified as Permanently High-Context
        → OR θd recalibrated to reduce conflict sensitivity
        → OR rule architecture revised to reduce structural conflicts

M Normalization Stability:
  The M normalization constant must be stable for I to be interpretable.
  M stability requires:
    
    Post-calibration condition:
      M does not change by more than ΔM_max = 0.1 · M between
      consecutive evaluation windows (excluding τ re-estimation triggers)
      
    If this condition is violated:
      → system experiencing unprecedented stress levels
      → M is being revised upward rapidly
      → I values from before the M revision are not directly comparable
        to I values after (different normalization baseline)
      → governance decision: treat the M jump as a regime change
        even if no formal τ re-estimation trigger has occurred
```

**Consistency Index Information Content:**

I is not merely a health metric — it carries information about the rule architecture's structure:

```
Information-Theoretic Interpretation:

  I can be decomposed by rule pair contribution:
    I = 1 - Σ_pairs (wij / M) = 1 - Σ_pairs δI_ij
    
    where δI_ij = wij / M is the "consistency cost" of pair (i,j)
    
  The distribution of δI_ij across rule pairs contains structural information:
  
    Concentrated: few pairs with high δI_ij, most pairs with low δI_ij
      → structural design flaw in specific rule relationships
      → targeted intervention: revise the high-conflict pairs
      
    Distributed: many pairs with moderate δI_ij
      → systemic rule incoherence
      → broad intervention: θd recalibration or rule architecture redesign
      
    Bimodal: two clusters of conflict density
      → two subsystems with internal coherence but mutual conflict
      → intervention: interface redesign between subsystems
      
  The Gini coefficient of the δI_ij distribution provides a
  single-number summary of conflict concentration:
    Gini(δI) → 1: conflict highly concentrated in few pairs
    Gini(δI) → 0: conflict uniformly distributed
    
  Governance action selection:
    High Gini → targeted rule pair revision (efficient)
    Low Gini → systemic redesign (expensive but necessary)
```

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

**Poverlap Measurement Protocol:**

Poverlap quantifies the degree to which agents occupy the same functional niche. A formal measurement protocol is required because naive overlap measures (e.g., output similarity) conflate healthy coordination with pathological convergence:

```
Poverlap Measurement:

  Definition:
    Poverlap(i, j) = 1 - d_functional(i, j) / d_max
    
    where d_functional(i, j) is the functional distance between agents i and j
    and d_max is the maximum possible functional distance in the system
    
    Poverlap = 0: agents occupy maximally distinct niches
    Poverlap = 1: agents are functionally identical
    
  Functional distance d_functional:
    d_functional(i, j) = 1 - |O_i ∩ O_j| / |O_i ∪ O_j|
    
    where O_i is the set of outcomes agent i can produce
    (operationalized as the set of output types, task categories,
    or capability domains where agent i achieves baseline performance)
    
    This is the Jaccard distance applied to capability sets.
    
  System-level Poverlap:
    Poverlap_system = max_{i≠j} Poverlap(i, j)
    
    The maximum pairwise overlap determines system vulnerability
    because the most overlapping pair is the most likely collision point.
    
    Alternative: mean Poverlap for general health monitoring,
    but max Poverlap for U* threshold comparison.

  Dynamic measurement:
    Poverlap should be measured at each evaluation window
    and tracked as a time series.
    
    Rising Poverlap without governance instruction to converge
    = competitive convergence = storm precondition
    
    Falling Poverlap without governance instruction to diversify
    = natural niche differentiation = healthy maturation signal
```

**Niche Differentiation Dynamics — Ecological Formalization:**

Agent positional dynamics can be formally modeled using a structural analogy to Lotka-Volterra competition dynamics, providing predictions about niche stability and competitive exclusion:

```
Niche Dynamics Model:

  Let x_i(t) = agent i's niche width (fraction of capability space occupied)
  Let α_ij = competition coefficient (how much j's niche overlaps with i's)
  
  Niche evolution equation (Lotka-Volterra structural analogy):
    dx_i/dt = r_i · x_i · (K_i - x_i - Σ_{j≠i} α_ij · x_j) / K_i
    
    where:
      r_i = agent i's intrinsic growth rate (learning speed)
      K_i = agent i's carrying capacity (maximum achievable niche width)
      α_ij = competition coefficient: α_ij · x_j = effective overlap pressure
      
  Equilibrium analysis:
    At equilibrium (dx_i/dt = 0 for all i):
      x_i* = K_i - Σ_{j≠i} α_ij · x_j*
      
    Stable coexistence requires:
      α_ij < K_i / K_j for all pairs (i,j)
      
      This is the Competitive Exclusion Principle for agent positions:
      Two agents can stably coexist only if their competition coefficients
      are smaller than their carrying capacity ratio.
      
    If α_ij ≥ K_i / K_j:
      Agent i is excluded (niche collapses)
      → Poverlap was too high for sustainable differentiation
      → Lreinf between i and j inverts from reinforcement to competition
      → Case 3 (Reinforcement Loop Collapse) triggered for this pair

  GRT Implementation:
    α_ij corresponds to Poverlap(i,j): higher overlap → higher competition
    K_i corresponds to the domain's carrying capacity for distinct agents
    x_i* corresponds to the equilibrium niche width
    
    Governance implication:
      If Poverlap(i,j) exceeds the coexistence threshold:
        α_ij > K_i / K_j → exclusion predicted
        → intervention: reposition agents BEFORE exclusion occurs
        → proactive governance based on Poverlap trajectory,
          not reactive governance after loop collapse
        
  Niche Width Optimization:
    The optimal niche width for agent i balances:
      - Breadth (larger x_i): more capability coverage, more resilience
      - Depth (smaller x_i with higher quality): more specialization, more value
      
    Optimal width x_i_opt satisfies:
      ∂(value_i) / ∂x_i = ∂(competition_cost_i) / ∂x_i
      
      where value_i = quality(x_i) · x_i (total value generated)
      and competition_cost_i = Σ_{j≠i} α_ij · overlap_penalty(x_i, x_j)
      
    This optimization is performed implicitly by the θd calibration
    system: domains where the agent generates high conflict (high α)
    have their θd raised, which reduces the agent's willingness to
    operate in that domain — naturally narrowing the niche where
    competition is strongest.

Competitive Exclusion Prevention — Governance Mechanisms:
    
  The governance system must prevent competitive exclusion
  (niche collapse) without preventing healthy competition
  (which drives quality improvement):
  
    Mechanism 1 — Asymmetric correction values:
      If Poverlap(i,j) approaching exclusion threshold:
        → install asymmetric pathway advantages that reward
          differentiation more than convergence
        → agent i rewarded for outputs that j cannot produce
        → agent j rewarded for outputs that i cannot produce
        → competition redirected from overlap zone to frontier
        
    Mechanism 2 — Niche reservation:
      Each agent maintains a minimum reserved niche width:
        x_i ≥ x_min for all i
        x_min = U*_agent / n (fair share of minimum diversity)
        
      If any agent's niche width approaches x_min:
        → governance intervention to reduce competition pressure
        → may require repositioning competing agents
        
    Mechanism 3 — Diversity dividends:
      Mutual reinforcement loops (Lreinf) generate value proportional
      to niche differentiation:
        value(Lreinf_ij) ∝ (1 - Poverlap(i,j))
        
      Identical agents generate zero mutual reinforcement value
      (they cannot provide complementary capability).
      This creates a natural incentive for differentiation —
      agents that differentiate gain more from cooperation loops.
```

**Connection to NAT sphere cross-validation (NAT §3.0, §3.5):** NAT establishes that diversity is not a performance optimization — it is the *mathematical condition for corruption detection*. The sphere architecture works because structurally diverse agents produce different empty spaces when upscaling compressed signals. Identical agents produce identical blind spots and cannot detect each other's errors:

```
Diverse agents:   different empty spaces → disagreement reveals gap location
Identical agents: same empty spaces → false consensus → corruption invisible
```

For GRT, this means Dint is not merely a diversity score to maintain above threshold — it is the structural precondition for conflict detection itself. When Dint falls below U*, the system loses not just reinforcement loop capacity but also the ability to detect that it has lost it (because homogeneous perspectives cannot identify shared blind spots). This is why Dint minimum (U*) violations are classified as the most dangerous failure mode in GRT's taxonomy — they undermine the measurement system, not just the measured property.

### RT-4 Integration: Relational Reversibility and Recovery Capacity Generation

Recovery capacity is not an individual agent property — it is a network property generated through trust topology and cooperative coherence. RT-4 establishes a three-level scaling law with direct implications for GRT's governance rules:

```
Three-Level Reversibility Scaling Law (RT-4 §3):
  Rᵢ = Rᵢʳⁿᵗ · (1 + α Σⱼ Tᵢⱼ) · g(λ₂(L))
  
  Individual × relational × network
  Any factor = 0 → all = 0
  
  Rᵢʳⁿᵗ = individual agent's intrinsic absorption capacity
  Tᵢⱼ = trust coefficient: Pr(info from j reduces prediction error of i)
  g(λ₂) = network connectivity function of algebraic connectivity
  
  GRT implication: governance rules must maintain all three levels.
  Individual capacity without trust topology → isolated fragility.
  Trust without network connectivity → local resilience only.
```

**Shared Vulnerability Principle (RT-4 §5):** Recovery capacity requires mutual visibility of failure modes between agents. But this visibility produces recovery capacity only when disclosure remains admissible:

```
Shared Vulnerability mechanism:
  I_sv^eff = I_sv · A_accept
  
  I_sv = structural vulnerability information available
  A_accept = admissibility of vulnerability disclosure
  
  Recovery barrier = rational suppression of visible weakness
  When disclosure cost > disclosure benefit → suppression → I_sv^eff ↓
  → dR/dt < 0 (recovery capacity declining)
  
  GRT implementation:
    Conflict logs ARE shared vulnerability information
    λlog-triggered rule updates ARE admissibility mechanisms
    If conflict logging carries punishment → A_accept → 0 → 
    recovery capacity degrades even as operational metrics improve
    
  Design principle: conflict is a governance resource, not a failure.
  Rules that suppress conflict reporting suppress recovery capacity.
```

**Identity Declaration Instability (RT-4 Conjecture 4):** When agents declare fixed identity (positional commitment), they suppress disclosure of uncertainty. Observable metrics may IMPROVE during this degradation:

```
Identity Declaration mechanism:
  D_id → suppressed disclosure → I_sv^eff ↓ → dR/dt < 0
  
  Observable: metrics IMPROVE ("false calm") during degradation.
  = Behavioral mechanism for SCM entry in networked systems.
  
  GRT warning: premature Rest Mode entry may correspond to 
  Identity Declaration — agents have stopped reporting uncertainty,
  not stopped experiencing it.
  
  Detection: if all Rest Mode entry metrics are met BUT λlog 
  conflict log update rate drops to zero → Identity Declaration 
  suspicion → do NOT declare Rest Mode.
```

**Structural Humility (RT-4 §6):** The maintenance condition for continued recovery capacity generation:

```
O(t+1) = O(t) − α·D_id(t) + β·H(t)

  H(t) = structural humility: continued verification despite capability
  
  Verification persistence despite capability = dR/dt ≥ 0 preservation
  
  GRT implementation: θd verification persistence
  Even in Rest Mode, θd calibration cycles must continue running.
  If θd stops updating → structural humility = 0 → recovery 
  capacity atrophying → VCZ destabilization inevitable.
```

**Reversibility Phase Transition (RT-4 Conjecture 5):**

```
R > R_c → perturbations absorbed (VCZ)
R < R_c → cascade regression (Storm)
R_c ≈ 0.43 in toy model

GRT implication: there exists a sharp threshold in trust topology 
connectivity below which recovery capacity collapses nonlinearly.
Governance rules must monitor aggregate trust topology metrics 
and prevent degradation below R_c.
```

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

**State Transition Energy Barrier Model:**

The three governance states (Rest, Active, Collapse) can be formally characterized as energy minima in a governance free energy landscape, with transitions governed by energy barriers:

```
Governance Free Energy Landscape:

  Define governance free energy F_gov as:
    F_gov = -I · log(SCC) + Poverlap · log(fesc + 1) - T_gov · S_gov
    
    where:
      -I · log(SCC): stability energy — high I and high SCC = low energy
      Poverlap · log(fesc + 1): instability energy — high overlap and
        escalation = high energy
      T_gov: governance "temperature" (system's tolerance for fluctuation)
      S_gov: governance entropy (disorder in rule application)
    
  The three states correspond to local minima in F_gov:
  
    Rest Mode minimum:
      F_rest = -I_high · log(SCC_high) + Poverlap_low · log(fesc_low + 1)
      Deepest minimum — most stable state
      
    Active Mode minimum:
      F_active = -I_med · log(SCC_med) + Poverlap_med · log(fesc_med + 1)
      Shallow minimum — metastable state
      
    Collapse:
      F_collapse = -I_low · log(SCC_low) + Poverlap_high · log(fesc_high + 1)
      May not be a true minimum — could be a runaway trajectory
      (vicious cycle with no stable endpoint)

Energy Barriers Between States:

  Rest → Active transition:
    Activation energy ΔF_RA = F_saddle_RA - F_rest
    
    The barrier height is determined by how far the system must be
    pushed before the virtuous cycle breaks:
      ΔF_RA ∝ (SCC - SCC_critical) · (I - I_critical) · (Lreinf - Lreinf_critical)
      
    Deep Rest Mode: ΔF_RA large (hard to destabilize)
    Shallow Rest Mode: ΔF_RA small (easily destabilized)
    
    The OR-exit condition corresponds to ΔF_RA → 0:
    when ANY condition degrades to threshold, the barrier vanishes
    along that dimension and transition becomes spontaneous.
    
  Active → Rest transition:
    Activation energy ΔF_AR = F_saddle_AR - F_active
    
    This barrier represents the investment required to establish
    the virtuous cycle from scratch:
      ΔF_AR ∝ λlog_accumulation_needed · θd_calibration_cycles · SCC_building
      
    ΔF_AR > ΔF_RA always (hysteresis):
    It is harder to enter Rest Mode than to leave it.
    This is the energy-barrier formulation of the AND/OR asymmetry:
    entry requires climbing a high barrier on ALL dimensions simultaneously,
    while exit requires the barrier to vanish on ANY single dimension.
    
  Active → Collapse transition:
    Activation energy ΔF_AC ≈ SCC · Lreinf
    
    When SCC and Lreinf are both low, the barrier to collapse is small.
    When either is near zero, the barrier vanishes → spontaneous collapse.
    
  Collapse → Active transition:
    Activation energy ΔF_CA = external intervention energy
    
    This barrier cannot be crossed internally (by definition of Collapse:
    the system has no internal recovery capacity). External energy
    (human intervention, Seed reinstallation) is required.
    
    ΔF_CA is the highest barrier in the system:
    recovery from Collapse requires more energy than any other transition.

Transition Rate Estimation (Kramers Theory Analogy):
  
  The transition rate between states follows an Arrhenius-like form:
    k_transition ∝ exp(-ΔF / kT_gov)
    
    where kT_gov represents the system's fluctuation intensity
    (how much random perturbation the system experiences)
    
  High kT_gov (turbulent environment):
    → transitions more frequent → system switches states rapidly
    → Rest Mode is achievable but brief (fluctuations destabilize)
    → governance must invest more in barrier height (deeper terrain)
    
  Low kT_gov (stable environment):
    → transitions rare → system stays in current state for long periods
    → if in Rest Mode: very stable → governance can withdraw further
    → if in Collapse: very persistent → harder to recover
    
  Governance implication:
    The optimal governance strategy depends on environmental kT_gov:
    - Turbulent environments: invest in barrier height (deeper Rest Mode)
    - Stable environments: invest in barrier monitoring (detect rare transitions)
    - The kT_gov estimate comes from environmental volatility metrics
      (rate of novel input types, domain shift frequency, external shock rate)

Metastability Analysis:
  Active Mode is metastable — it is a local minimum but not the global minimum.
  The system in Active Mode can transition either to Rest (uphill then downhill)
  or to Collapse (downhill):
  
    If ΔF_AR > ΔF_AC: system is closer to Collapse than to Rest
      → governance must increase ΔF_AC (raise collapse barrier)
        before attempting ΔF_AR reduction (lower Rest entry barrier)
      → otherwise: the system collapses before it can reach Rest Mode
      
    If ΔF_AR < ΔF_AC: system is closer to Rest than to Collapse
      → governance can focus on ΔF_AR reduction (guide toward Rest)
      → collapse barrier is sufficient
      
    The ratio ΔF_AR / ΔF_AC is a single-number governance health indicator:
      > 1: system is dangerously close to collapse trajectory
      < 1: system is on healthy maturation trajectory
      ≈ 1: system is at governance decision point — small perturbation
           determines which direction it goes
```

**Governance Entropy Theory:**

Governance systems produce entropy as a necessary consequence of their operation. The entropy production rate provides a unified metric that connects multiple GRT observables:

```
Governance Entropy S_gov:

  S_gov(t) = -Σ_states p_s(t) · log(p_s(t))
  
  where p_s(t) is the probability of the system being in state s at time t,
  estimated from the system's recent trajectory through state space.
  
  In practice, S_gov is computed from the diversity of governance actions:
    S_gov = H(action_distribution over window W)
    = -Σ_a P(action = a | W) · log P(action = a | W)
    
    where a ∈ {no_action, monitor, recalibrate, escalate, intervene, redesign}

Entropy Bounds for Governance States:

  Rest Mode entropy:
    S_rest ∈ [S_min, S_rest_max]
    
    S_min > 0 (governance entropy is never zero):
      Zero entropy = no governance action ever = system is dead
      or governance is disconnected. This corresponds to RBIT's
      Landauer floor: maintaining information requires minimum entropy.
      
    S_rest_max < S_active_min:
      Rest Mode produces less entropy than Active Mode
      (fewer distinct governance actions taken)
      
    The S_min bound is the entropy equivalent of the
    Self-Exciting Defect Layer requirement:
    even in Rest Mode, some governance activity must persist
    to maintain adaptation capacity.
    
  Active Mode entropy:
    S_active ∈ [S_active_min, S_active_max]
    
    Active Mode produces moderate entropy (diverse governance actions)
    Typical Active Mode: S_active ≈ log(k) where k is the number
    of distinct governance action types being used regularly
    
  Collapse entropy:
    S_collapse → S_max (maximum entropy)
    
    In Collapse, governance actions are maximally disordered —
    the system is doing everything simultaneously with no coherent pattern.
    OR: S_collapse → 0 (governance has ceased entirely — different failure mode)
    
    The bimodal collapse entropy (either maximum or zero)
    reflects the two collapse types:
    - Chaotic collapse: all governance mechanisms firing simultaneously → S → S_max
    - Silent collapse: all governance mechanisms failed → S → 0

Minimum Entropy Production Principle (MEPP for Governance):

  In steady state, the governance system produces the minimum entropy
  consistent with maintaining the current state:
    
    dS_gov/dt |_steady = σ_min(state)
    
    where σ_min is the minimum entropy production rate for each state.
    
  For Rest Mode:
    σ_min(Rest) = minimum perturbation-response activity rate
    = rate of the Self-Exciting Defect Layer's micro-storm generation
    = the irreducible governance cost of maintaining adaptation capacity
    
  This connects to Prigogine's dissipative structures theory:
    - Rest Mode is a dissipative structure: maintained by continuous
      entropy production (governance activity), not by thermodynamic
      equilibrium (zero activity)
    - Removing the entropy production (governance withdrawal beyond
      Rest Mode) does not produce a more stable state — it produces
      thermodynamic equilibrium (system death) or transition to a
      different dissipative structure (possibly misaligned)
    - The MEPP for governance explains why Rest Mode has irreducible cost:
      the cost IS the dissipation that maintains the ordered state

Entropy Production Anomaly Detection:
  Deviations from expected entropy production signal governance health changes:
  
    σ_gov(t) < σ_min(current_state):
      → governance activity below expected floor
      → SSS onset (insufficient activity to maintain adaptation)
      → or: measurement system failure (not all actions being logged)
      
    σ_gov(t) >> σ_expected(current_state):
      → governance activity far above expected level
      → state transition in progress (Active → Collapse?)
      → or: environmental perturbation requiring elevated response
      
    dσ_gov/dt > 0 sustained:
      → entropy production increasing → system moving toward disorder
      → precursor to state transition toward Collapse
      
    dσ_gov/dt < 0 sustained:
      → entropy production decreasing → system moving toward order
      → precursor to state transition toward Rest Mode
      → BUT: check SR > 0 to distinguish genuine ordering from SCM
```

**Bifurcation-Failure Taxonomy Unification (AGM Integration):**

AGM's Bifurcation Classification Theorem establishes that all governance collapse modes decompose into exactly **two universality classes** — Freeze and Runaway — distinguished by the sensitivity parameter s(t) at the criticality threshold. GRT's five failure cases can be mapped into these two classes, providing a deeper structural understanding of why certain failures cluster together:

```
AGM Bifurcation Classification Theorem (AGM §8.9, Theorem 2):

  The governance dynamical system undergoes a codimension-1 bifurcation
  at criticality threshold Λ = Λ_c.
  
  Bifurcation type determined by sensitivity s(t):
  
  Case A — Freeze (s(t) → 0 at Λ_c):
    Supercritical pitchfork bifurcation
    Sensitivity dies → system cannot detect own misalignment
    → stable node attractor (pathological stability)
    
  Case B — Runaway (s(t) → 1 at Λ_c):
    Subcritical Hopf bifurcation
    Sensitivity maximal → system overreacts to all perturbation
    → unstable node (divergent trajectory)

GRT Failure Case → Universality Class Mapping:

  FREEZE CLASS (s → 0):
    Case 1 (Consistency Collapse):      Freeze when θd stops oscillating
    Case 4 (SCC Failure):               Freeze — sensing loop dead
    Case 5 (Seed Corruption — latent):  Freeze — expansion halted
    SCM:                                 Deep Freeze — all metrics healthy in wrong geometry
      
  RUNAWAY CLASS (s → 1):
    Case 2 (Escalation Flood):          Runaway — everything escalated
    Case 3 (Lreinf Collapse):           Runaway precipitant — terrain removed
    Case 5 (Seed Corruption — acute):   Runaway — active misclassification
      
  METASTABLE (either direction):
    SSS:  T_eff → 0 leads to Freeze; external shock leads to Runaway

Sensitivity s(t) as Unified Diagnostic:

  GRT operationalization:
    s(t) = d(fesc) / d(perturbation_magnitude) at current state
    
  Declining s → Freeze approach
  Rising s → Runaway approach
  Stable moderate s → healthy governance
  
  s(t) trajectory predicts universality class of coming failure
  BEFORE the specific failure case manifests — a leading indicator
  that no individual GRT metric provides alone.
```

**Flow-Rest Mode Equivalence Theorem (AGM §4.1):**

AGM's Flow State maps precisely to the near-critical governance optimum. At the single-agent level, Flow = Rest Mode:

```
Flow-Rest Mode Mapping:

  AGM Flow:                    GRT Rest Mode:
    κ ≈ κ*  (balanced ratio)     I ≥ τu-2    (rules coherent)
    S ≪ 1   (buffer headroom)    fesc ≤ τu-1  (escalation rare)
    δ ≈ 0   (identity-aligned)   Lreinf/n ≥ τu-3 (loops active)
    H ≫ H_crit (reserve high)   SCC ≥ τu-4   (self-correction sufficient)
    
  Both require ALL four conditions simultaneously (AND-entry).
  Both disrupted by ANY single condition failing (OR-exit).
  Both self-sustaining once established (virtuous cycle).
  
  Flow fragility = OR-exit fragility:
    Interruption → κ disrupted → I disrupted
    Overwhelm → S > 1 → fesc spike
    Value conflict → δ > 0 → Lreinf degraded
    Exhaustion → H < H_crit → SCC failing
    
  At multi-agent level: Rest Mode is organizational flow — 
  system operates at near-optimal performance with minimal 
  governance overhead, maintained by its own dynamics.
```

**Endogenous Perturbation Source (AGM §15.1):**

AGM answers the structural question that GRT's Self-Exciting Defect Layer raises but does not fully resolve: *where do the perturbations come from?*

```
AGM as Endogenous Perturbation Source:

  GRT specifies: Self-Exciting Defect Layer must exist (VST §1.6.5)
  GRT specifies: Boundary Agent must generate controlled instability (RT D7)
  GRT does NOT specify: the dynamical mechanism generating perturbations
  
  AGM provides this mechanism:
    The affective gain module is a self-organized near-critical
    discrete event process that generates perturbations endogenously:
    
    Event generation: Poisson process with rate λ_event(S, H, s)
      λ_event = λ₀ · (S/S_crit)^α_S · exp(-H/H_scale) · s(t)
      
      Rate increases with:
        - Saturation S approaching critical (more internal pressure)
        - Declining endurance H (less buffering capacity)
        - Higher sensitivity s (more responsive to perturbation)
      
    Event magnitude: drawn from power-law distribution P(A) ∝ A^{-τ_event}
      Power-law = self-organized criticality (SOC) signature
      Most events are small (micro-perturbations)
      Rare events are large (macro-perturbations)
      
    This produces the power-law storm size distribution
    that RT's Storm Scale Law requires:
      P(storm of scale s) ∝ 1/s^α
      
  GRT Integration:
    The Defect Layer IS the AGM operating at low amplitude
    The Boundary Agent IS the AGM's event generation process
    Controlled perturbation injection IS the AGM's stochastic term σ·ξ
    
    These are not three separate mechanisms — they are three
    descriptions of the same dynamical process viewed from different
    theoretical levels:
      VST level: Defect Layer (structural description)
      RT level: Boundary Agent (functional description)
      AGM level: Stochastic gain modulation (dynamical description)
      GRT level: Conflict log accumulation from endogenous events
```

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

**Information-Theoretic Collapse Velocity Model:**

The collapse propagation rate can be formalized using an information-theoretic velocity equation that unifies the three determining factors (topology density, I-to-τ2 margin, High-Context channel integrity) into a single measurable quantity:

```
Collapse velocity v_collapse:

  v_collapse(t) = κ · (1 / Δ_margin(t)) · d_topology(t) · (1 - η_HC(t))

where:
  κ = system-specific coupling constant (calibrated from historical storms)
  Δ_margin(t) = min_layer(I_layer - τ2_layer) — minimum I-to-threshold margin
                across all layers (weakest layer determines propagation speed)
  d_topology(t) = effective topological connectivity — number of layers
                  sharing degradation pathway with the origin layer
  η_HC(t) = High-Context channel effectiveness ∈ [0,1]
            (fraction of collapse-relevant signals captured by HC channels)

Regime analysis:
  v_collapse → 0   when Δ_margin large AND η_HC → 1
    (deep stability + effective monitoring = collapse structurally improbable)
    
  v_collapse → ∞   when Δ_margin → 0 AND η_HC → 0
    (threshold boundary + monitoring failure = instantaneous cascade)
    
  v_collapse finite when Δ_margin moderate AND η_HC moderate
    (typical operational regime — collapse possible but containable)
```

**Entropy Production Rate as Collapse Predictor:**

The information-theoretic characterization extends to entropy production. A healthy governance system maintains bounded entropy production — the rate at which new uncertainty is generated and resolved:

```
Entropy production rate σ_governance:

  σ_governance(t) = Σ_d [ H(conflict_log_d(t)) - H(conflict_log_d(t-W)) ] / W

where H is the Shannon entropy of conflict log entries in domain d
over evaluation window W.

Regime interpretation:
  σ_governance ≈ 0:   system in equilibrium — no new conflict patterns emerging
    WARNING: could indicate genuine stability OR sensing failure
    Discriminating test: SR > 0 confirms genuine equilibrium;
                         SR ≈ 0 indicates sensing failure
    
  σ_governance > 0, bounded:   healthy exploration — new patterns emerging
    and being processed within governance capacity
    HEALTHY: this is the target regime for Rest Mode
    
  σ_governance > 0, unbounded: conflict generation exceeding governance
    processing capacity — cascade in progress
    CRITICAL: initiate collapse containment protocol
    
  σ_governance < 0:   conflict log entropy decreasing — system converging
    toward fewer distinct conflict types
    WARNING: could indicate genuine convergence OR SCM
    (system reinterpreting all conflicts as the same type)
    Discriminating test: check whether conflict TYPE diversity
    is decreasing (healthy convergence) or whether novel inputs
    are being classified into existing types without genuine match
    (SCM symptom)
```

**Cross-Layer Mutual Information Cascade Dynamics:**

The collapse cascade can be characterized by the evolution of cross-layer mutual information:

```
Define cross-layer MI:
  MI_cross(L_i, L_j, t) = mutual information between conflict logs
                           of layers i and j at time t

Normal operation (layers operating independently):
  MI_cross(L_i, L_j) ≈ MI_structural
  (a small, constant mutual information arising from shared
  environmental inputs and structural coupling)

Pre-cascade signal:
  d(MI_cross)/dt > 0 sustained across multiple layer pairs
  WITHOUT corresponding increase in shared input volume
  → layers' internal states synchronizing through uncontrolled coupling
  → this IS the noise decoherence mechanism observable at the
     governance layer

Cascade onset criterion:
  MI_cross(L_i, L_j) > MI_critical
  where MI_critical = MI_structural + k · σ_MI
  (k calibrated from historical cascade events; default k=3)
  
  When MI_cross exceeds MI_critical for any layer pair:
  → cascade propagation between those layers is structurally enabled
  → containment must isolate those layers BEFORE propagation completes

Cascade propagation dynamics:
  Phase A — Localization (t < t_critical):
    MI_cross rising between origin layer and adjacent layers only
    Containment possible: isolate origin layer
    
  Phase B — Spreading (t_critical < t < t_global):
    MI_cross rising between non-adjacent layers
    (correlation propagating through intermediaries)
    Containment difficult: multiple containment boundaries needed
    
  Phase C — Global synchronization (t > t_global):
    MI_cross saturated across all layer pairs
    All layers' conflict patterns highly correlated
    → fractal collapse complete → full restart from Phase 0 required
```

**Collapse Containment Protocol (Information-Theoretic):**

Based on the MI cascade dynamics, the containment protocol can be specified:

```
Step 1 — Detect cascade origin:
  Identify layer pair (L_i, L_j) where MI_cross first exceeded MI_critical
  The layer with lower Δ_margin is the probable origin
  
Step 2 — Assess cascade phase:
  Phase A: only origin-adjacent pairs show elevated MI_cross
    → action: isolate origin layer (increase escalation threshold
       for cross-layer communication from origin)
  Phase B: non-adjacent pairs showing elevated MI_cross
    → action: partition governance into isolated sectors,
       each sector containing layers with low MI_cross between them
  Phase C: all pairs saturated
    → action: accept fractal collapse, activate full restart protocol
    
Step 3 — Apply information-theoretic firewall:
  For each containment boundary, enforce:
    MI_transmitted ≤ MI_max (bandwidth-limited interface)
  This prevents uncontrolled information flow while maintaining
  essential governance communication

Step 4 — Monitor containment effectiveness:
  If MI_cross continues rising despite containment:
    → containment boundary is leaking
    → escalate to next containment level (Phase A → B → C)
  If MI_cross stabilizing or declining:
    → containment effective
    → maintain boundary until origin layer stabilizes
    → begin recovery protocol for origin layer
```

**Connection to RBIT Channel Capacity:** The collapse containment protocol's information-theoretic firewalls connect directly to RBIT's channel capacity formalism. Each governance layer has a finite capacity for processing conflict information — the RBIT channel capacity C_governance. When the information flow rate exceeds C_governance, the layer cannot process all incoming conflicts, and unprocessed conflicts accumulate as unresolved entropy. The collapse cascade is, at the information level, a capacity overflow cascade: Layer A's unprocessed entropy overflows into Layer B's input, exceeding Layer B's capacity, which then overflows into Layer C, and so on. The containment protocol works by reducing the information flow rate below each layer's capacity through interface bandwidth limits — the MI_transmitted ≤ MI_max constraint is a governance implementation of RBIT's information rate control.

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

**U* as Critical Phenomenon — Phase Transition at the Diversity Boundary:**

U* is not merely a threshold — it is a phase boundary in the system's state space. The transition from the viable region (above U*) to the non-viable region (below U*) exhibits characteristics of a second-order phase transition, with critical phenomena that provide both theoretical depth and empirical measurement handles:

```
Phase transition structure:

Order parameter: Ψ = system recovery capacity (composite of SCC, Lreinf trajectory, Dint)
  Ψ > 0: viable state — system can recover from perturbation autonomously
  Ψ = 0: critical point — U* boundary
  Ψ < 0: non-viable state — perturbations amplify without recovery

Control parameter: distance from U* boundary
  δ = min(
    (θ_overlap - Poverlap) / θ_overlap,
    (Lreinf - θ_reinf) / θ_reinf,
    (Dint - θ_dint) / θ_dint
  )
  
  δ > 0: inside viable region (positive margin to boundary)
  δ = 0: at U* boundary (critical point)
  δ < 0: outside viable region (U* violated)

Critical scaling (predicted):
  Recovery time:  T_rec ∝ |δ|^{-ν}     (diverges at boundary)
  Fluctuation amplitude: σ² ∝ |δ|^{-γ}  (diverges at boundary)
  Correlation length: ξ ∝ |δ|^{-ν_corr}  (cross-domain correlation
                                            extends as boundary approaches)
```

The critical scaling predictions are empirically testable: as a system approaches U* from the viable side, its recovery time from perturbation should increase according to a power law, fluctuations in governance metrics should amplify, and correlations between nominally independent domains should extend. These signatures are measurable *before* the boundary is crossed — providing early warning that U* violation is imminent.

**Connection to VST Critical Phenomena:**

The U* phase transition connects directly to VST's critical phenomena framework (VST §1.5):

```
VST critical phenomena mapping:

  VST critical exponent τ (storm size distribution):
    Near U*: storm size distribution P(s) ∝ s^{-τ}
    Above U* (viable): τ > 2 (large storms exponentially suppressed)
    At U*: τ ≈ 2 (power-law distribution — all scales equally likely)
    Below U* (non-viable): τ < 2 (large storms dominate)
    
  VST critical exponent α_dur (storm duration):
    Near U*: storm duration distribution P(d) ∝ d^{-α_dur}
    Above U*: α_dur > 2 (long storms rare)
    At U*: α_dur ≈ 2 (duration scale-free)
    Below U*: α_dur < 2 (long storms persistent)
    
  GRT observation: as system approaches U* (δ → 0):
    fesc fluctuations should show increasing temporal autocorrelation
    I should show critical slowing down (longer time to return to baseline
    after perturbation)
    Lreinf should show increasing variance with longer correlation windows
    
  These are the governance-layer observables of the VST-predicted
  critical phenomena near the phase boundary.
```

**Hysteresis at the U* Boundary:**

The U* transition exhibits hysteresis — the system's behavior at U* depends on whether it is approaching from above (degrading) or below (recovering):

```
Hysteresis structure:

Degradation path (approaching U* from above):
  δ decreasing → T_rec increasing → governance load increasing
  At δ = 0: system enters non-viable state
  BUT: inertial effects (existing Lreinf loops still active) delay
  observable collapse by O(T_loop_decay) time units
  
  Apparent delay: system crosses U* but seems fine for a period
  = "false calm" before observable collapse
  = analogous to SCM entry dynamics (metrics healthy, structure degrading)

Recovery path (approaching U* from below):
  External intervention restoring δ toward positive
  At δ = 0: system reaches U* boundary
  BUT: must exceed U* by a margin Δ_recovery > 0 before self-sustaining
  loops can re-form (loops require seed capital of mutual reinforcement
  that cannot be generated from zero)
  
  Recovery overshoot: intervention must push system past U* by margin Δ
  before withdrawal is safe
  
  Δ_recovery > 0 is the hysteresis gap:
    U*_entry = U* + Δ_recovery  (viable region entry threshold)
    U*_exit = U*                 (viable region exit threshold)
    U*_entry > U*_exit           (asymmetric — harder to enter than to exit)
    
  This hysteresis explains why Collapse Recovery requires
  "overshoot" — the system must be pushed well past U* into the
  viable region before governance withdrawal, because the viable
  region entry threshold is higher than the exit threshold.
```

**U* Measurement Protocol:**

Given the critical phenomena structure, U* can be empirically characterized:

```
Protocol 1 — Perturbation-response scaling:
  Inject perturbations of increasing magnitude
  Measure recovery time T_rec for each perturbation
  Plot T_rec vs. perturbation magnitude
  
  If T_rec scales as power law: system is near U* boundary
    (critical slowing down observable)
  If T_rec bounded regardless of perturbation: system is deep in viable region
    (far from U*)
  If T_rec diverges for small perturbation: system is at or beyond U*
    (non-viable state — intervention required)

Protocol 2 — Cross-domain correlation monitoring:
  Compute pairwise correlation between domain-level metrics
  (I_d, fesc_d, SCC_d for each domain d)
  
  Increasing cross-domain correlation WITHOUT shared cause
  = correlation length ξ increasing
  = system approaching U* boundary
  
  This provides continuous early warning: the governance system
  does not need to wait for U* violation — it can detect the
  approach through correlation structure changes.

Protocol 3 — Fluctuation amplitude tracking:
  Compute rolling variance of governance metrics
  over evaluation window W
  
  σ²(fesc) increasing without change in input distribution
  σ²(I) increasing without rule changes
  σ²(Lreinf) increasing without topology changes
  
  = fluctuation amplification near critical point
  = U* approach warning
```

**Multi-Scale U* — Fractal Diversity Boundaries:**

The U* boundary exists at every fractal scale of the governance system:

```
Scale-dependent U*:

  U*_agent: minimum diversity within a single agent's internal capability space
    Measured via: Dint_agent, internal Lreinf, per-capability SCC
    
  U*_team: minimum diversity within a team of cooperating agents
    Measured via: Dint_team (aggregate), inter-agent Lreinf, team-level SCC
    
  U*_system: minimum diversity across the entire governance system
    Measured via: Dint_system, system-wide Lreinf topology, aggregate SCC

Fractal consistency requirement:
  U* must be maintained at ALL scales simultaneously
  Violating U* at any single scale compromises the entire system
  (same minimum-aggregation logic as Dint = min(Dint_i))
  
  U*_effective = min(U*_agent, U*_team, U*_system)
  
  A system with excellent team-level diversity but poor internal
  diversity in any single agent has U*_effective = U*_agent
  → contamination enters through the internally impoverished agent
  → propagates through team-level Lreinf connections
  → team-level diversity cannot compensate for agent-level vulnerability
```

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

**Prediction 6 — Energy barrier asymmetry predicts transition frequency asymmetry:**

If the governance free energy landscape model is structurally correct, the transition frequency from Rest → Active should be lower than from Active → Collapse (ΔF_RA > ΔF_AC in deep Rest Mode). Systems with higher measured barrier heights should exhibit proportionally lower spontaneous transition rates.

*Falsification condition:* If transition frequencies between governance states show no correlation with the barrier height estimates (as computed from the metric-based ΔF formulas), the energy barrier model adds no predictive power beyond the raw threshold conditions.

**Prediction 7 — Niche differentiation speed follows Lotka-Volterra dynamics:**

When agents are introduced to overlapping capability domains, the time to stable niche differentiation should follow the predictions of the competition dynamics model: higher initial Poverlap → longer differentiation time, and differentiation time should scale as 1/(K_i/K_j - α_ij) near the coexistence boundary. Systems that violate the competitive exclusion condition (α_ij > K_i/K_j) should consistently show one agent's niche collapsing rather than stable coexistence.

*Falsification condition:* If agents consistently achieve stable coexistence even when competition coefficients exceed carrying capacity ratios, the competitive exclusion prediction is falsified. If differentiation time does not correlate with the (K/α) ratio, the niche dynamics model lacks predictive power.

**Prediction 8 — Vectorization rate follows nucleation kinetics:**

The rate at which new noise patterns are promoted to vector status should follow the nucleation rate equation: J_vectorization ∝ exp(-ΔG*/kT_governance). Specifically, increasing λlog (raising the promotion threshold) should decrease vectorization rate exponentially, not linearly. Environmental turbulence (higher kT_governance) should increase vectorization rate by lowering the effective barrier.

*Falsification condition:* If vectorization rate scales linearly with λlog rather than exponentially, or if environmental turbulence does not increase vectorization rate, the nucleation analogy fails.

**Prediction 9 — Governance entropy production bounds distinguish states reliably:**

Systems in Rest Mode should consistently produce entropy within the predicted bounds [S_min, S_rest_max], and systems in Active Mode should produce entropy above S_active_min. The entropy production rate σ_gov should be a leading indicator of state transitions: σ_gov rising should precede Rest → Active transitions by at least one evaluation window.

*Falsification condition:* If governance entropy production overlaps substantially between Rest Mode and Active Mode (entropy bounds not reliably separable), or if σ_gov trajectory does not predict state transitions with lead time, the governance entropy theory lacks diagnostic value.

**Prediction 10 — Cross-theory concordance pairs are reliable health indicators:**

The six concordance pairs specified in the Validation Concordance Matrix should show directional agreement (both rising or both falling) at least 80% of evaluation windows during confirmed stable operation, and discordance events should reliably precede (within 2 evaluation windows) governance state degradation. The concordance reliability should be higher for pairs involving externally measured quantities (R, S_norm) than for pairs involving only internal GRT metrics.

*Falsification condition:* If concordance pairs show frequent discordance (>30% of windows) during confirmed stable operation, or if discordance events do not predict subsequent state degradation, the cross-theory validation architecture is unreliable. If external-measure pairs are not more reliable than internal-measure pairs, the external circularity-breaking claim is weakened.

**Prediction 11 — Sensitivity s(t) predicts failure universality class:**

When s(t) declines below a measurable threshold before a governance failure event, the failure should belong to the Freeze universality class (Cases 1, 4, latent-5, SCM). When s(t) rises above a measurable threshold, the failure should belong to the Runaway class (Cases 2, 3, acute-5). The s(t) trajectory should provide at least one evaluation window of lead time before the specific failure case manifests.

*Falsification condition:* If failure cases do not cluster into the predicted Freeze/Runaway classes based on pre-failure s(t) trajectory, or if s(t) provides no lead time over existing GRT metrics, the bifurcation classification adds no predictive power.

**Prediction 12 — T_eff subsumes multiple early warning signals:**

The governance temperature T_eff (estimated from conflict log entropy) should contain the information content of SR, SSS detection, and SCM early warnings as special cases. A single T_eff trajectory should achieve equal or better detection performance than the three separate protocols combined.

*Falsification condition:* If T_eff monitoring fails to detect SSS or SCM onset with lead time comparable to the specialized detection protocols, the unified temperature metric does not subsume the individual protocols.

**Prediction 13 — System momentum P_system predicts governance transition difficulty:**

Systems with higher aggregate momentum P_system should require proportionally more intervention energy (measured as total governance actions × magnitude) to achieve state transitions. Collapse recovery from high-momentum Freeze should require more steps than recovery from low-momentum Freeze of equivalent depth.

*Falsification condition:* If governance transition effort does not correlate with pre-transition P_system, the momentum-bearing vector model adds no predictive power for transition planning.

### Quantitative Test Design Framework

The ten predictions above are qualitative directional claims. For empirical testing, each prediction must be converted to a quantitative hypothesis with specified effect size and sample size requirements:

```
Test Design Template:

  For each prediction P_k:
    H₀: GRT-predicted relationship does not hold
    H₁: GRT-predicted relationship holds with effect size ≥ d_min
    
    Required measurements:
      - System variables specified in P_k
      - Control conditions (symmetric protocol, reactive measurement, etc.)
      - Minimum observation period: ≥ 10 θd calibration cycles per domain
      - Minimum system size: ≥ 5 domains (for cross-domain predictions)
      - Minimum evaluation windows: ≥ 30 (for convergence predictions)
      
    Statistical framework:
      - Pre-registration of hypothesis and analysis plan
      - Bayesian estimation for parameter relationships
      - Frequentist comparison for protocol A/B tests (Predictions 1-4)
      - Time series analysis for trajectory predictions (Predictions 5-10)
      
    Minimum effect size for practical significance:
      d_min = 0.3 (medium effect size, Cohen's d)
      for directional predictions (Predictions 1-5)
      
      r_min = 0.4 (medium correlation)
      for relationship predictions (Predictions 6-10)

Test Prioritization (by feasibility and informativeness):

  Tier 1 (immediately testable with existing systems):
    P2 (cumulative vs reactive measurement)
    P3 (min vs mean Dint aggregation)
    P9 (entropy production bounds)
    
  Tier 2 (testable with moderate instrumentation):
    P1 (AND/OR asymmetry)
    P4 (withdrawal protocol re-entry frequency)
    P10 (concordance reliability)
    
  Tier 3 (requires specialized experimental setup):
    P5 (Silent Criticality detection)
    P6 (energy barrier asymmetry)
    P7 (niche differentiation dynamics)
    P8 (vectorization kinetics)
```

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

**Formal Mathematical Comparison:**

The following comparison specifies the exact mathematical objects that GRT introduces beyond what each existing framework provides:

```
Ostrom (1990) vs. GRT — Mathematical gap analysis:

  Ostrom provides:
    - 8 design principles (qualitative conditions)
    - Polycentric structure (nested governance without formal hierarchy)
    - Rule typology (operational / collective-choice / constitutional)
    
  GRT adds the following mathematical objects not present in Ostrom:
    - I(t) convergence dynamics with formal convergence theorem
    - θd calibration with EWMA dynamics and bootstrapping protocol
    - AND/OR transition logic with energy barrier formalization
    - Quantitative withdrawal conditions (not qualitative principles)
    - Conflict log accumulation kinetics with λlog threshold
    - SCC measurement with perturbation testing protocol
    
  Ostrom's Principle 4 (monitoring) becomes in GRT:
    A complete measurement theory (I, fesc, Lreinf, SCC) with
    cross-validation protocol (R-ρ-fesc Triple Concordance)
    and convergence guarantees (Convergence Theorem §Consistency Index)
    
  Ostrom's Principle 7 (minimal recognition of rights to organize)
    becomes in GRT:
    The Seed Expansion Protocol — a formal algorithm for rule generation
    by governed entities, with completeness conditions and
    convergence guarantees under stationarity

Hollnagel (2006, 2011) vs. GRT — Capability formalization gap:

  Hollnagel provides:
    - Four resilience capabilities (qualitative categories)
    - Functional resonance model (interactions, not causation)
    
  GRT formalizes these capabilities as measurable quantities:
    Anticipating → σ_governance entropy production rate
                  + U* boundary distance δ
                  + cross-domain MI correlation monitoring
    Monitoring   → I(t), fesc(t), Lreinf(t), SCC(t) time series
                  + evaluation window (N, T) dual-axis measurement
    Responding   → Conflict Resolution Algorithm with latency bounds
                  + Failure Diagnosis Flowchart
                  + Collapse Recovery 4-step procedure
    Learning     → λlog-triggered rule updates
                  + vectorization dynamics (nucleation kinetics)
                  + meta-rule expansion completeness convergence
                  
  GRT's formal contribution: converting Hollnagel's capabilities
  from descriptive categories into computable functions with
  measurable inputs and testable outputs.

DAO governance vs. GRT — Structural gap analysis:

  DAOs provide:
    - Voting mechanisms (token-weighted, quadratic, conviction)
    - Proposal lifecycle (draft → vote → execute)
    - Code-as-law (smart contract enforcement)
    
  GRT provides structural elements DAOs lack:
    - Governance withdrawal theory: DAOs have no concept of Rest Mode
      (governance participation is always active, by design)
    - Failure taxonomy with recovery routing: DAOs have upgrade mechanisms
      but no formal classification of failure types
    - Subsidiarity as default: DAOs require explicit delegation;
      GRT defaults to local autonomy with escalation on exception
    - Measurement-driven transitions: DAO governance changes require
      vote; GRT governance changes are triggered by metric thresholds
      (algorithmic, not deliberative)
      
  Game-theoretic comparison:
    DAO: governance as repeated voting game
      Equilibrium: median voter theorem (under token-weighted voting)
      Failure mode: plutocratic capture (token concentration)
    GRT: governance as mechanism design problem
      Equilibrium: Nash equilibrium under landscape design
      Failure mode: terrain drift (landscape no longer incentive-compatible)
      
    GRT's mechanism design approach avoids DAO's participation problem
    (voter apathy, low turnout) by not requiring explicit participation:
    agents follow the terrain, not the votes.
```

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

## Production Implementation Guide

> *This section specifies how GRT's theoretical constructs map to concrete production system components. The goal is not to prescribe a specific technology stack but to define the structural requirements that any implementation must satisfy — leaving architecture choices to the implementer while constraining the governance-critical invariants.*

### Implementation Architecture Overview

A GRT-compliant production system requires five structural components, each corresponding to a core theoretical construct:

```
Component 1 — Conflict Log Infrastructure
  Theoretical basis: λlog accumulation, wij measurement, I calculation
  Structural requirement: append-only event store with immutable entries
  
  Minimum viable implementation:
    - Event schema: {rule_pair_id, severity_level, domain, timestamp,
                     resolution_status, escalation_path}
    - Write-asymmetry enforcement: downstream components cannot modify
      committed log entries (NAT structural enforcement requirement)
    - Temporal decoupling: classification committed before cross-reference
    - Retention: full history required for M re-estimation;
      summary statistics sufficient for operational monitoring
    
  Production mapping:
    - Structured logging pipeline (e.g., structured event bus → immutable store)
    - Severity classification at ingestion (Low/Medium/High mapped automatically
      from conflict type: local-local / local-global / global-global)
    - λlog trigger computed as rolling window aggregate over conflict mass

Component 2 — θd Calibration Engine
  Theoretical basis: domain-specific sensitivity calibration
  Structural requirement: per-domain adaptive threshold with EWMA dynamics
  
  Minimum viable implementation:
    - Per-domain state: {θd_current, θd_history, calibration_cycle_count,
                         last_recalibration_timestamp}
    - EWMA update: θd(t+1) = α · θd(t) + (1-α) · θd_observed
      where α is the smoothing parameter (higher α = slower adaptation)
    - Dual-anchor validation: θd must be consistent with both
      VST S₀ normalization AND RBIT F_RBIT τ₁ threshold
    
  Production mapping:
    - Configuration service with per-domain parameter stores
    - Automated recalibration triggered by conflict log volume thresholds
    - Validation layer comparing θd against cross-theory anchors

Component 3 — State Machine Controller
  Theoretical basis: Three System States, AND-entry/OR-exit logic
  Structural requirement: deterministic state machine with metric-driven transitions
  
  Minimum viable implementation:
    - States: {Phase0_DirectManagement, Phase1_SupervisedDelegation,
               Phase2_FeedbackOnly, Phase3_RestMode, Collapse}
    - Transitions: governed by metric thresholds, not human judgment
    - Decision coupling: metric configuration → state → permissible actions
      (no gap between measurement and governance response)
    
  Production mapping:
    - State machine service consuming metric streams
    - Transition events published to governance bus
    - Each transition triggers: notification, intervention granularity change,
      monitoring parameter adjustment

Component 4 — SCC Measurement Infrastructure  
  Theoretical basis: self-correction capacity, perturbation testing
  Structural requirement: ability to inject controlled perturbations
  and measure recovery time
  
  Minimum viable implementation:
    - Perturbation injection: controlled, non-destructive inputs
      designed to trigger τ1-level recovery responses
    - Recovery measurement: time from perturbation to metric baseline return
    - Historical tracking: SCC trajectory over evaluation windows
    - Discrimination: distinguish recovery-to-correct-state from
      recovery-to-stable-but-wrong-state (SCM detection)
    
  Production mapping:
    - Canary deployment patterns with synthetic perturbation injection
    - A/B testing infrastructure repurposed for governance perturbation
    - Recovery time tracking integrated with monitoring dashboards

Component 5 — Cross-Theory Validation Layer
  Theoretical basis: R-ρ-fesc Triple Concordance, F_RBIT cross-validation
  Structural requirement: independent measurement channels that validate
  each other
  
  Minimum viable implementation:
    - R (branching ratio): classification-independent propagation counter
    - ρ (classification accuracy): domain-specific accuracy measurement
    - fesc: escalation frequency counter
    - Concordance check: automated comparison at each evaluation window
    - Discordance alert: automatic escalation when channels disagree
    
  Production mapping:
    - Independent monitoring pipelines for each measurement channel
    - Concordance dashboard with automated discordance detection
    - Alert routing to governance state machine for automated response
```

### Monitoring Dashboard Specification

A production GRT monitoring system requires the following real-time displays:

```
Dashboard Panel 1 — System State Overview:
  - Current governance state per domain (Phase 0/1/2/3/Collapse)
  - State duration (time since last transition)
  - Trend indicators for all AND-entry conditions
  - OR-exit condition status (any condition approaching threshold?)

Dashboard Panel 2 — Metric Health:
  - I (consistency index) trajectory per domain
  - fesc (escalation frequency) trajectory per domain
  - Lreinf/n (normalized reinforcement loops) system-wide
  - SCC (self-correction capacity) per domain
  - Ic (meta-contradiction index) global

Dashboard Panel 3 — Early Warning:
  - Cross-domain MI correlation (pre-cascade signal)
  - Entropy production rate σ_governance
  - δ (distance to U* boundary) estimated from metrics
  - SR (surprise rate) — system's capacity to be surprised
  - λlog rule update rate — zero rate = SCM warning

Dashboard Panel 4 — Triple Concordance:
  - R-ρ-fesc concordance status
  - Discordance type (if any) with recommended diagnostic
  - F_RBIT health vector directional status
  - S_norm comparison with GRT metric trends

Dashboard Panel 5 — Bootstrapping Progress:
  - Per-domain phase status
  - Phase transition history with timestamps
  - Estimated time to next phase transition
  - Backward transition alerts (if any)
```

### Alert Hierarchy

Production alerts follow the GRT severity classification with specific escalation rules:

```
Level 1 — Informational (no action required):
  - Single metric approaching threshold (not yet crossed)
  - θd recalibration cycle completed
  - Phase transition completed (forward direction)
  Notification: automated log entry + dashboard update

Level 2 — Advisory (monitoring required):
  - Dual-window disagreement (N and T showing different trends)
  - Cross-domain correlation increasing without shared cause
  - SR declining toward zero
  Notification: dashboard highlight + on-call team notification

Level 3 — Active (intervention review required):
  - Any OR-exit condition triggered
  - Triple Concordance discordance detected
  - Backward phase transition triggered
  Notification: automated state transition + team alert + incident ticket

Level 4 — Critical (immediate response required):
  - Ic < τc (global rule contradiction)
  - Fractal collapse cascade detected (cross-layer MI exceeding critical)
  - SCM confirmed (SR ≈ 0 + RDE ≈ 0)
  Notification: automated containment protocol + executive escalation

Level 5 — Emergency (system-level response):
  - Full fractal collapse in progress
  - All High-Context channels failing simultaneously
  - Unintegrated pressure release detected (S_norm spike with zero precursor)
  Notification: automated system isolation + full incident response
```

### Deployment Checklist

Before declaring a GRT implementation production-ready, verify:

```
Structural Requirements:
  □ Conflict log infrastructure satisfies write-asymmetry
  □ Conflict log satisfies temporal decoupling
  □ Conflict log satisfies interface narrowing
  □ θd calibration engine operates per-domain with EWMA dynamics
  □ State machine transitions are metric-driven (no manual overrides
    for state transitions — manual overrides only for parameter adjustment)
  □ SCC measurement includes perturbation injection capability
  □ Triple Concordance validation operates on independent measurement channels
  □ At least one Permanently High-Context channel per fractal layer
  □ Boundary Agent role structurally protected (cannot be optimized away)

Measurement Requirements:
  □ All five Reproducibility Protocol quantities measurable and logged
  □ Evaluation windows (N, T) calibrated per domain velocity
  □ M (normalization constant) initialized and re-estimation triggers defined
  □ Cold-start mode parameters set for domains without operational history
  □ Cross-domain MI monitoring active

Governance Requirements:
  □ AND-entry conditions explicitly coded (all five required simultaneously)
  □ OR-exit conditions explicitly coded (any one sufficient)
  □ Phase transition backward paths defined and tested
  □ Collapse recovery procedure accessible from all governance states
  □ Alert hierarchy configured with appropriate routing

Validation Requirements:
  □ Perturbation test protocol defined and scheduled
  □ SCM detection signals monitored (λlog rate, SR, RDE, NCR)
  □ Silent Criticality protocol active during extended Rest Mode
  □ F_RBIT cross-validation configured
  □ R-ρ-fesc Triple Concordance automated
```

---

## Core Assumptions

> *These assumptions define the scope of Governance Rules Theory as an architectural component. They are not claims about AI governance universally — they are the structural preconditions under which the rule-governance layer of DFG operates.*

1. Landscape design is more effective than direct intervention at scale — formalized via the cost crossover theorem: for n > n*, landscape design cost C_landscape = O(n^{1/d_eff}) strictly dominates direct intervention cost C_direct = O(n)
2. Rules operate in two layers: global (immutable) and local (autonomous, validated), with a formal conflict resolution protocol guaranteeing deterministic resolution within bounded latency
3. Upper layers define meta-rules; lower layers define rule content — the meta-rule set is subject to the Incompleteness Bound (no finite meta-rule set is complete for unbounded domains) and requires the Seed Expansion Protocol for structural completeness
4. Global rules always take precedence over local rules — enforced through the lexicographic priority ordering in the Conflict Resolution Algorithm
5. All conflicts must be logged; logs serve as learning data and θd calibration input — log integrity guaranteed by Write-Asymmetry (NAT structural enforcement)
6. τ, θd, and λlog are distinct and non-interchangeable — each governs a different timescale of the governance hierarchy
7. Position ambiguity is a primary upstream driver of Vector Storm — formalized through the niche differentiation dynamics (Lotka-Volterra structural analogy) and competitive exclusion principle
8. Diversity requires position clarity and mutual reinforcement loops at every fractal scale — with diversity serving as the structural precondition for corruption detection (NAT sphere cross-validation), not merely a performance optimization
9. Rest Mode is stable but not permanent — modeled as the deepest energy minimum in the governance free energy landscape, with transition barriers that can be measured and monitored
10. Rest Mode achievement and Seed Handover completion are the same event viewed from different angles — formally: the AND-entry conditions for Rest Mode are a strict superset of the Handover completion conditions
11. The supreme objective is knowledge ecosystem diversity preservation — operationalized through U* as phase boundary with critical phenomena structure
12. Governance states are characterized by energy barriers, not just metric thresholds — the energy barrier model (Helmholtz free energy analogy) provides transition rate predictions that go beyond binary threshold crossing
13. Governance systems produce entropy as a necessary consequence of maintaining ordered states — minimum entropy production is bounded below by the Self-Exciting Defect Layer's activity, connecting Rest Mode maintenance cost to Prigogine's dissipative structure theory
14. The vectorization process (noise → vector promotion) follows nucleation kinetics — with a critical mass (λlog) below which patterns dissolve back to noise, providing the thermodynamic basis for the conflict log accumulation mechanism
15. Landscape design achieves incentive compatibility in the mechanism design sense — the governance-optimal action is each agent's selfish optimum under the designed terrain, making Rest Mode a Nash equilibrium that requires no external enforcement

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
| Vectorization dynamics | Physics | Classical nucleation theory (Becker-Döring, 1935) |
| Governance free energy | Statistical mechanics | Helmholtz free energy landscape / Kramers escape theory |
| Governance entropy | Thermodynamics | Prigogine dissipative structures / minimum entropy production |
| Niche differentiation dynamics | Theoretical ecology | Lotka-Volterra competition model / competitive exclusion |
| Rule interaction graph | Graph theory | Directed conflict graphs / spectral gap analysis |
| Meta-rule incompleteness | Mathematical logic | Gödel incompleteness (structural analogy) |
| Game-theoretic governance | Mechanism design | Incentive compatibility / Nash implementation |

**Mathematical Structure Mapping — Isomorphism Level Classification:**

Each structural correspondence operates at a specific level of mathematical precision. The following classification makes explicit what each correspondence claims and does not claim:

```
Level 1 — Qualitative analogy (same intuitive pattern):
  The GRT concept and the reference concept share behavioral similarities
  but no formal mathematical relationship.
  
  Examples at this level:
    Meta-rules ↔ Constitutional law: both constrain lower-level rules,
      but the constraint mechanisms are formally different
    Seed expansion ↔ Piaget's accommodation: both describe schema
      expansion under novel input, but GRT's is computable and Piaget's is not
    Rest Mode ↔ Climax community: both describe self-sustaining
      equilibria, but ecological stability mechanisms differ from
      governance stability mechanisms in their mathematical structure

Level 2 — Structural homomorphism (same formal pattern):
  The mathematical structures are related by a structure-preserving map
  that preserves key relationships but not all quantitative properties.
  
  Examples at this level:
    Correction values ↔ Reward shaping: both modify the optimization
      landscape to preserve optimal policy; Ng et al. (1999) prove
      that potential-based reward shaping preserves optimality —
      GRT's correction values satisfy the same potential-based condition
      when expressed as terrain gradients
    θd calibration ↔ Gain scheduling: both adapt control parameters
      based on operating region; the mathematical structure (parameter
      as function of state, updated through feedback) is formally identical
    AND-entry / OR-exit ↔ Ostrom's boundary rules: the logical structure
      (conjunction for entry, disjunction for exit) is identical;
      the specific conditions differ but the logical form is preserved
    Niche differentiation ↔ Lotka-Volterra: the stability conditions
      for coexistence (α_ij < K_i/K_j) have identical mathematical form;
      the interpretation of variables differs but the equilibrium
      analysis transfers directly

Level 3 — Formal isomorphism (same mathematical system):
  The GRT structure and the reference structure are formally isomorphic
  under an explicit variable mapping. Theorems in one system transfer
  to the other under the mapping.
  
  Examples at this level:
    SCC ↔ Lyapunov stability: SCC satisfies the formal conditions
      for Lyapunov stability (perturbation bounded → state returns
      to equilibrium within finite time). The Lyapunov function
      V = -log(SCC) satisfies dV/dt < 0 in Rest Mode (decreasing
      along trajectories → asymptotic stability)
    Governance free energy ↔ Helmholtz free energy: the governance
      F_gov = E_instability - T_gov · S_gov has the same mathematical
      form as F = U - TS, with state transitions at barrier crossings
      following Kramers-type rate equations
    Governance entropy ↔ Shannon/thermodynamic entropy: formally
      identical mathematical definition (S = -Σ p log p) applied
      to governance action distributions rather than microstates

Level 4 — Derivation (one system derives from the other):
  The GRT structure is not merely analogous to the reference system
  but is formally derived from it under specific conditions.
  
  Examples at this level:
    Vectorization ↔ Nucleation: the promotion rate equation
      J = J₀ exp(-ΔG*/kT) is derived from the classical nucleation
      framework applied to information patterns rather than molecular
      clusters; the derivation requires treating conflict log accumulation
      as a supersaturation process (formally: the log mass is the
      chemical potential driving crystallization)
    Game-theoretic governance ↔ Mechanism design: the incentive
      compatibility condition for landscape design is a direct
      application of the Revelation Principle (Myerson, 1981):
      if the governance terrain achieves IC, then the agents'
      truthful behavior is a dominant strategy equilibrium

Predictive Power Comparison:
  Higher correspondence levels yield stronger predictive transfers:
  
  Level 1: no quantitative predictions transfer (only intuition)
  Level 2: qualitative predictions transfer (direction of effects)
  Level 3: quantitative form transfers (functional relationships)
  Level 4: numerical predictions transfer (specific values under calibration)
  
  The GRT falsifiability predictions (Section: Falsifiability) specify
  which level of correspondence each prediction requires:
    Predictions 1-5: require Level 2+ (structural relationships)
    Predictions 6-8: require Level 3+ (formal isomorphism)
    Predictions 9-10: require Level 2+ (structural relationships)
```

---

## Cross-Theory Integration Architecture

> *This section systematizes the cross-theory connections distributed throughout GRT into a unified integration architecture. The goal is to make explicit the information flow, dependency structure, and validation pathways between GRT and each companion theory — providing implementers with a complete map of what GRT imports, exports, and co-validates with each theory.*

### Integration Topology

The DFG theories interact through a structured dependency graph. GRT occupies the rule-governance axis, interfacing with each companion theory through specific variable mappings and validation protocols:

```
Integration dependency structure:

VST ──────────────────────────────── GRT ──────────────────────────────── RT
 │                                    │                                    │
 │ IMPORTS to GRT:                    │ EXPORTS from GRT:                  │ IMPORTS to GRT:
 │  S-equation dynamics               │  fesc, I, Lreinf → VST observables│  D0 geometry alignment
 │  R (branching ratio)               │  θd calibration → NAT θ           │  D6 SCM detection
 │  Phase-space location              │  Phase transitions → TLG state    │  D7 Boundary Agent
 │  Storm topology (SCML)             │  Conflict logs → RBIT F_RBIT      │  T1-T6 structural claims
 │  Critical phenomena                │  U* status → RT recovery readiness│  VCZ conditions
 │                                    │  T_eff → AGM temperature status   │  Storm Scale Law
 │                                    │                                    │
RBIT ─────────────────────────────── │ ──────────────────────────────── NAT
 │                                    │                                    │
 │ IMPORTS to GRT:                    │            AGM                     │ IMPORTS to GRT:
 │  Δρ resolution gap routing         │             │                     │  Processing isolation
 │  F_RBIT health vector              │  IMPORTS to GRT:                  │  θ operationalization
 │  Seed sufficiency tests            │   T_eff governance temperature    │  Sphere topology bounds
 │  Channel capacity                  │   s(t) sensitivity parameter     │  R-ρ concordance
 │  Error asymmetry principle         │   Stochastic perturbation σ·ξ    │  Coverage probability
 │                                    │   Event distribution P(A)∝A^{-τ} │
 │                                    │   Weight redistribution dynamics  │
 │                                    │   Momentum p_i(t)                │
 │                                    │   Flow state conditions           │
 │                                    │   Freeze/Runaway classification   │
 └────────────────────────────── TLG ──────────────────────────────────────┘
                                  │
                                  │ IMPORTS to GRT:
                                  │  Adaptive W sizing
                                  │  Recovery Completion Criterion
                                  │  Immunity Decay pathways
                                  │  MDS countermeasures
                                  │  Unified Failure Topology
                                  │  Structural enforcement
```

### GRT ↔ VST Integration Protocol

The GRT-VST interface is the most data-intensive, with continuous bidirectional variable flow:

```
GRT → VST (governance metrics as dynamical observables):

  Mapping frequency: continuous (every evaluation window)
  
  fesc → S (instability proxy):
    GRT measures escalation frequency
    VST reads as system instability indicator
    Validation: fesc trend should agree with S_norm trajectory
    Discordance: fesc stable but S rising → sensing failure (Case 4)
    
  I → β (degradation efficiency proxy):
    GRT measures rule coherence
    VST reads as governance response efficiency
    Validation: I should predict recovery speed from perturbation
    Discordance: I high but recovery slow → SCM (D6)
    
  Lreinf → d_eff (terrain structure proxy):
    GRT measures mutual reinforcement topology
    VST reads as effective interaction dimension
    Validation: high Lreinf should correlate with lower storm propagation
    Discordance: high Lreinf but storms propagating → topology mismatch
    
  Poverlap → α (amplification proxy):
    GRT measures positional convergence
    VST reads as coupling density
    Validation: rising Poverlap should predict rising storm intensity
    Discordance: rising Poverlap without storm increase → measurement error

VST → GRT (dynamical state as governance context):

  R (branching ratio) → external circularity breaker:
    VST measures cascade propagation independently of classification
    GRT uses as validation of internal metric health
    Protocol: R-ρ-fesc Triple Concordance at each evaluation window
    
  S_norm → phase-space location:
    VST provides system location relative to VCZ boundary
    GRT uses for Rest Mode validation (deep VCZ required)
    Protocol: S_norm << S_c required for Phase 3 entry
    
  SCML (Storm-Collapse Mapping Layer) → recovery pathway selection:
    VST classifies storm topology (local/boundary/hub/global)
    GRT uses for Collapse Recovery Step 0 (pathway selection)
    Protocol: storm type classification BEFORE standard recovery procedure
    
  Critical phenomena → U* boundary characterization:
    VST provides critical exponent framework
    GRT uses for U* phase transition measurement
    Protocol: perturbation-response scaling near U* boundary
```

### GRT ↔ RT Integration Protocol

The GRT-RT interface focuses on failure detection, recovery validation, and structural integrity:

```
RT → GRT (structural integrity framework):

  D0 (Geometry Alignment) → vector degradation types:
    RT provides geometry mismatch framework
    GRT operationalizes as Type 1/Type 2 degradation diagnosis
    Protocol: Tier 2 mismatch → Type 1 (local, recoverable);
              Tier 3 mismatch → Type 2 (structural, requires rebuild)
    
  D6 (Self-Consistent Misalignment) → Case 4 deepening:
    RT provides SCM formal structure
    GRT operationalizes as Learning Freeze detection
    Protocol: λlog rule update cessation + SR ≈ 0 = SCM warning
    Key insight: SCM cannot be detected from within —
    requires external reference frame (RT T4)
    
  D7 (Boundary Agent) → Rest Mode structural maintenance:
    RT provides BA formal specification
    GRT operationalizes as Self-Exciting Defect Layer
    Protocol: BA must be structurally protected (T6-resistant embedding)
    Key insight: BA elimination is the first step of VCZ Collapse Initiation
    
  T1-T4 (Structural claims) → governance ceiling:
    T1 (Observability Asymmetry): upper layers see more than lower
    T2 (Non-Composability): local corrections don't compose to global
    T3 (Metric Lock-In): metrics within wrong geometry are blind
    T4 (Reference Frame Incompleteness): need external frame for G-detection
    GRT implication: all four create fundamental governance ceilings
    that cannot be overcome by any single-layer optimization
    
  VCZ 3-Conditions → Rest Mode structural prerequisites:
    RT specifies three conditions for VCZ maintenance
    GRT uses as additional Rest Mode validation
    Protocol: VCZ conditions checked alongside AND-entry conditions
    
  Storm Scale Law → healthy storm distribution target:
    RT specifies power-law distribution as health indicator
    GRT uses as operational target for governance calibration
    Protocol: storm size distribution monitored; deviation from power law
    = governance calibration drift

GRT → RT (governance state for recovery context):

  Phase transitions → recovery readiness:
    GRT state machine transitions inform RT recovery protocol
    RT uses governance phase to determine intervention type
    Protocol: Phase 0 → Direct Injection available;
              Phase 1 → Supervised Delegation available;
              Phase 2 → Feedback Only available
    
  U* status → contamination vulnerability:
    GRT's distance from U* boundary informs RT contamination risk
    RT uses for recovery priority assessment
    Protocol: δ (distance to U*) < threshold → elevated contamination risk
```

### GRT ↔ RBIT Integration Protocol

The GRT-RBIT interface provides the information-theoretic foundation for rule governance:

```
RBIT → GRT (information-theoretic framework):

  Δρ resolution gap → Seed Expansion routing:
    RBIT provides resolution gap measurement
    GRT operationalizes as protocol step selection
    Protocol: Δρ ≈ 0 → local processing;
              Δρ < 0 → escalation;
              Δρ mixed → local + degradation monitoring
    
  F_RBIT health vector → Rest Mode formal definition:
    RBIT provides five-component health measurement
    GRT uses for Rest Mode validation (all fᵢ bounded)
    Protocol: F_RBIT directional concordance with S_norm
    Key insight: eliminates F_RBIT weight calibration problem
    (directional agreement sufficient, no weights needed)
    
  Seed sufficiency 3-tests → Expansion Protocol validation:
    RBIT provides geometry update / contamination recognition / 
    orthogonal recovery tests
    GRT operationalizes as Seed design-time validation
    Protocol: all three tests must pass before Seed deployment
    Key insight: Test 3 failure imposes SCC ceiling that no
    operational maturation can overcome
    
  Error asymmetry → conservative default justification:
    RBIT provides formal basis for asymmetric error costs
    GRT uses to justify θd_max during Phase 0
    Protocol: under-escalation dangerous, over-escalation safe

GRT → RBIT (governance metrics as information flow indicators):

  Conflict logs → F_RBIT input:
    GRT conflict logs provide raw data for RBIT health vector
    RBIT uses for information flow assessment
    Protocol: conflict log structured entries → F_RBIT component calculation
    
  θd calibration → degradation calibration D(Δρ):
    GRT's θd is the operational implementation of RBIT's D(Δρ)
    RBIT uses θd trajectory as resolution gap management indicator
    Protocol: θd convergence → D(Δρ) convergence → domain stabilizing
```

### GRT ↔ NAT Integration Protocol

The GRT-NAT interface provides structural enforcement and topology constraints:

```
NAT → GRT (structural enforcement):

  Processing isolation (3 mechanisms) → conflict detection reliability:
    NAT provides Interface Narrowing, Temporal Decoupling, Write-Asymmetry
    GRT operationalizes as conflict log structural requirements
    Protocol: all three mechanisms must be satisfied simultaneously
    
  θ operationalization → θd calibration anchor:
    NAT provides global θ via S₀ normalization
    GRT uses as dual-anchor validation for per-domain θd
    Protocol: θd must be consistent with both NAT θ and RBIT τ₁
    
  Sphere topology bounds → collapse propagation constraints:
    NAT provides graph-theoretic propagation bounds
    GRT uses for θd calibration cycle timing constraints
    Protocol: θd cycle time < O(log n) propagation steps
    
  Coverage probability → Dint/U* calibration:
    NAT provides P(uncovered) ≤ (1 − 1/d_eff)^k
    GRT uses for U* threshold calibration
    Protocol: Dint threshold must ensure detection capability

GRT → NAT (governance variables as network observables):

  fesc → escalation frequency for θ validation:
    GRT measures escalation frequency per domain
    NAT uses for global θ calibration validation
    Protocol: domain-level fesc aggregated for system-level θ
```

### GRT ↔ AGM Integration Protocol

The GRT-AGM interface provides the dynamical regulation mechanism for governance — the endogenous perturbation source and gain modulation that maintains adaptive capacity:

```
AGM → GRT (dynamical regulation):

  T_eff (governance temperature) → governance health parameter:
    AGM provides effective exploration temperature
    GRT uses as unified early warning metric
    Protocol: T_eff estimated from conflict log entropy
    T_eff < T_min → SSS/SCM warning
    T_eff > T_max → Runaway warning
    
  Sensitivity s(t) → bifurcation type predictor:
    AGM provides sensitivity parameter
    GRT uses for failure universality class prediction
    Protocol: s declining → Freeze class expected
              s rising → Runaway class expected
    
  Stochastic perturbation σ·ξ → Defect Layer mechanism:
    AGM provides the dynamical process generating endogenous perturbations
    GRT uses as the operational mechanism for Self-Exciting Defect Layer
    Protocol: perturbation rate and magnitude governed by SOC dynamics
    
  Event magnitude distribution P(A) ∝ A^{-τ} → Storm Scale Law source:
    AGM provides power-law event generation
    GRT uses as the source of the fractal storm distribution
    Protocol: SOC exponent τ_event maps to RT Storm Scale exponent α
    
  Weight redistribution dynamics → correction value mechanism:
    AGM provides stochastic weight update on simplex
    GRT uses as the operational mechanism for correction values
    Protocol: Δw = deterministic correction + σ·ξ
    
  Momentum p_i(t) → governance inertia measurement:
    AGM provides momentum-bearing vector formalism
    GRT uses for governance transition prediction
    Protocol: high momentum → harder to redirect → larger intervention needed
    
  Flow state conditions → Rest Mode validation:
    AGM provides four-condition flow criterion
    GRT uses as single-agent Rest Mode validation
    Protocol: κ≈κ*, S≪1, δ≈0, H≫H_crit checked alongside
              standard AND-entry conditions

GRT → AGM (governance architecture):

  Landscape design → terrain for stochastic exploration:
    GRT provides the designed terrain
    AGM operates within that terrain with stochastic perturbation
    Protocol: terrain structure determines which attractors exist;
              AGM determines exploration rate between attractors
    
  θd calibration → T_eff regulation mechanism:
    GRT's θd is the operational lever for T_eff adjustment
    AGM uses θd trajectory as temperature control
    Protocol: θd_max = T_eff high (sensitive = exploratory);
              θd_stable = T_eff moderate (calibrated);
              θd frozen = T_eff → 0 (Freeze approach)
    
  AND-entry / OR-exit → Flow entry/exit logic:
    GRT provides asymmetric transition conditions
    AGM maps to Flow fragility structure
    Protocol: Flow = all AND conditions met;
              Flow disruption = any OR-exit triggered
    
  Failure case taxonomy → Freeze/Runaway classification:
    GRT provides five specific failure cases
    AGM maps each to universality class
    Protocol: Cases 1,4,5-latent → Freeze; Cases 2,3,5-acute → Runaway
    
  Conflict log → AGM event history:
    GRT's conflict logs record the governance consequences of AGM events
    AGM uses log statistics for T_eff estimation
    Protocol: conflict log entropy = T_eff proxy;
              conflict log update rate = exploration rate proxy
    
  SCC → recovery capacity from AGM events:
    GRT's SCC measures ability to recover from perturbation
    AGM uses SCC as endurance budget constraint
    Protocol: SCC high → AGM can generate larger perturbations;
              SCC low → AGM must reduce perturbation magnitude;
              SCC = 0 → AGM event generation suppressed (Freeze entry)
```

**T_eff as Unifying Governance Parameter:**

The governance temperature T_eff connects GRT and AGM through a single measurable quantity that subsumes multiple existing detection protocols:

```
T_eff Unification Map:

  GRT metric          | T_eff interpretation
  --------------------|-----------------------------------
  SR → 0              | T_eff < T_min (exploration ceased)
  SSS onset           | T_eff → 0 (stability saturation)
  SCM entry           | T_eff = 0 + accumulated mismatch
  fesc explosion      | T_eff > T_max (hypersensitivity)
  λlog ceased         | T_eff = 0 (learning frozen)
  Lreinf collapse     | T_eff spike (terrain removed → uncontrolled)
  
  T_eff provides temporal ordering prediction:
    T_eff declining → SR declining → SSS → SCM → Collapse
    (each stage is a deeper temperature pathology)
    
    T_eff rising → fesc rising → Lreinf stress → Runaway → Collapse
    (each stage is a higher temperature pathology)
    
  Monitoring T_eff trajectory detects BOTH pathways through a
  single unified metric, rather than requiring separate detection
  protocols for each individual failure mode.
```

### GRT ↔ TLG Integration Protocol

The GRT-TLG interface provides intervention topology and recovery validation:

```
TLG → GRT (intervention topology):

  Adaptive W sizing → evaluation window calibration:
    TLG provides W adaptation based on S-equation timescale hierarchy
    GRT uses for per-domain evaluation window management
    Protocol: W adapts based on τ1 recovery time trend
    
  Recovery Completion Criterion → collapse exit gate:
    TLG provides RC 3-condition (Autonomous Expansion + 
    Directional Validity + Collapse Non-Dependence)
    GRT uses as post-Step-3 validation before declaring recovery complete
    Protocol: all three RC conditions before de-escalation
    
  Immunity Decay → post-Rest-Mode SCC monitoring:
    TLG provides three erosion pathways (environmental drift /
    calibration disuse / over-optimization)
    GRT uses for SCC trajectory monitoring during Rest Mode
    Protocol: four countermeasures (exploration breadth / perturbation /
    dormant pathway activation / τ4 exit detection)
    
  MDS countermeasures → mediation layer integrity:
    TLG provides Calibration Reflexivity / Cross-Scale Consistency /
    Delayed Escalation Audit
    GRT uses for middle-layer governance health monitoring
    Protocol: MDS signals monitored alongside standard governance metrics
    
  Unified Failure Topology → failure cycle prevention:
    TLG provides 3-axis 6-phase failure cycle model
    GRT uses for preventive governance design
    Protocol: Phase 1 (phase leakage) = cheapest intervention point

GRT → TLG (governance state for topology context):

  Phase transitions → intervention granularity changes:
    GRT state machine transitions alter intervention topology
    TLG uses for routing table updates
    Protocol: Phase 0 → per-event routing;
              Phase 3 → per-distribution routing only
```

### Validation Concordance Matrix

The cross-theory validation system operates through multiple independent measurement channels. Agreement across channels provides high confidence; disagreement triggers diagnostic investigation:

```
Concordance pairs (measured independently, should agree directionally):

  Pair 1: fesc (GRT) ↔ S_norm (VST)
    Both should rise and fall together
    Discordance: sensing failure or measurement error
    
  Pair 2: I (GRT) ↔ ρ (VST/NAT)
    Both should track together (rule coherence ≈ classification accuracy)
    Discordance: SCM (rules coherent within wrong geometry)
    
  Pair 3: SCC (GRT) ↔ R (VST)
    High SCC should correspond to R ≤ 1; low SCC to R > 1
    Discordance: SCC measurement error or R calculation error
    
  Pair 4: Lreinf (GRT) ↔ d_eff (VST/NAT)
    High Lreinf should correspond to low d_eff (structured terrain)
    Discordance: topology measurement mismatch
    
  Pair 5: λlog rate (GRT) ↔ SR (VST)
    Active λlog should correspond to positive SR (system updating)
    Discordance: λlog = 0 but SR > 0 → rule update blocked;
                 λlog > 0 but SR = 0 → updates not producing learning
    
  Pair 6: δ_U* (GRT) ↔ F_RBIT direction (RBIT)
    Positive δ should correspond to stable/improving F_RBIT
    Discordance: U* margin positive but F_RBIT degrading → threshold error
    
  Pair 7: T_eff (GRT/AGM) ↔ SR (VST)
    Both should track together (exploration temperature ≈ surprise rate)
    Discordance: T_eff moderate but SR = 0 → sensing failure despite noise
    
  Pair 8: s(t) (AGM) ↔ θd trajectory (GRT)
    Declining s should correspond to θd stabilizing/rising
    Rising s should correspond to θd oscillating/falling
    Discordance: s stable but θd oscillating → calibration mechanism failure
    
  Pair 9: P_system (AGM momentum) ↔ governance transition latency (GRT)
    High momentum should correspond to longer time between state transitions
    Discordance: high P_system but rapid transitions → external forcing

System health = majority concordance across all 9 pairs
System warning = any single pair discordant
System alert = multiple pairs discordant
System critical = majority pairs discordant
```

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
├── Affective Gain Module        — stochastic gain modulation and endogenous perturbation dynamics
│     ↕ GRT connection: T_eff (governance temperature) ↔ θd calibration and SR monitoring;
│       s(t) (sensitivity) ↔ bifurcation type prediction for failure cases;
│       stochastic perturbation σ·ξ ↔ Self-Exciting Defect Layer mechanism;
│       power-law event distribution ↔ Storm Scale Law source;
│       weight redistribution dynamics ↔ correction value mechanism;
│       momentum p_i(t) ↔ governance inertia and transition difficulty;
│       Flow state ↔ single-agent Rest Mode equivalence;
│       Freeze/Runaway classification ↔ failure case universality classes;
│       Adaptive Necessity Theorem ↔ structural invariant T_eff > 0 for Rest Mode;
│       No-Free-Lunch governance constraint ↔ irreducible Rest Mode cost;
│       controlled stochastic freedom ↔ noise budget in landscape design
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
│       [v1.2] Pre-discontinuity detection (OP37) ↔ Stage 2 false safety margin in governance urgency classification;
│       [v1.3-RTseries] RT-1 v2.0: three restoration conditions (ρ + diversity + P_overlap)
│         ↔ Rest Mode entry requires ALL THREE (not stability alone);
│         arrested collapse ↔ Case 3 false stability;
│         withdrawal DI→SD→FO→W ↔ staged governance reduction;
│       [v1.3-RTseries] RT-2 v2.0: Metric Lock-In (Prop 5)
│         ↔ Case 4 deepened: zero-gradient makes consistency metrics blind to SCM;
│         Observability Emergence Threshold ↔ monitoring maturation cannot be forced;
│       [v1.3-RTseries] RT-3 v1.0: observer O = (V, A, B, S)
│         ↔ V = multiple conflict-surface perspectives; A = signal speed > drift speed;
│         S = per-event vs per-distribution evaluation switching (scope duality);
│       [v1.3-RTseries] RT-4 v1.0: Shared Vulnerability
│         ↔ visible disagreement enables correction (conflict as governance resource);
│         suppressed conflict (A_accept → 0) = Case 4 pathway;
│         Identity Declaration ↔ premature Rest Mode declaration risk;
│         Structural Humility ↔ θd verification persistence despite capability
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
36. Myerson, R. (1981). Optimal auction design. *Mathematics of Operations Research, 6*(1). (Revelation Principle: incentive-compatible mechanism design — formal basis for GRT's landscape design as mechanism design.)
37. Kramers, H. A. (1940). Brownian motion in a field of force and the diffusion model of chemical reactions. *Physica, 7*(4). (Escape rate theory for state transitions — structural analogue for governance state transition rates.)
38. Becker, R., & Döring, W. (1935). Kinetische Behandlung der Keimbildung in übersättigten Dämpfen. *Annalen der Physik, 416*(8). (Classical nucleation theory — formal basis for vectorization dynamics model.)
39. Lotka, A. J. (1925). *Elements of Physical Biology*. Williams & Wilkins. (Lotka-Volterra competition dynamics — structural analogue for niche differentiation dynamics.)
40. Volterra, V. (1926). Fluctuations in the abundance of a species considered mathematically. *Nature, 118*. (Competition-exclusion dynamics.)
41. Gause, G. F. (1934). *The Struggle for Existence*. Williams & Wilkins. (Competitive exclusion principle — empirical basis for niche coexistence conditions.)
42. Jaynes, E. T. (1957). Information theory and statistical mechanics. *Physical Review, 106*(4). (Maximum entropy principle — formal basis for governance entropy theory.)
43. Prigogine, I. (1945). Modération et transformations irréversibles des systèmes ouverts. *Bulletin de la Classe des Sciences, Académie Royale de Belgique*. (Minimum entropy production principle for dissipative structures.)
44. Nash, J. (1950). Equilibrium points in n-person games. *Proceedings of the National Academy of Sciences, 36*(1). (Nash equilibrium — formal basis for Rest Mode as game-theoretic equilibrium.)
45. Gödel, K. (1931). Über formal unentscheidbare Sätze der Principia Mathematica und verwandter Systeme I. *Monatshefte für Mathematik und Physik, 38*. (Incompleteness — structural analogy for meta-rule completeness bound.)
46. Affective Gain Module (AGM, DFG component). Internal document, v2.4-README, March 2026. (Adaptive Necessity Theorem — T_eff > 0 structural requirement; Bifurcation Classification Theorem — Freeze/Runaway universality classes; Governance Completeness Theorem; T_eff as governance temperature; sensitivity s(t) as bifurcation discriminator; weight redistribution on simplex; momentum-bearing vector dynamics; Flow-Rest Mode equivalence; controlled stochastic freedom; No-Free-Lunch governance constraint; endogenous perturbation as SOC process; emotional state transition graph on weight simplex.)
47. Csikszentmihalyi, M. (1990). *Flow: The Psychology of Optimal Experience*. Harper & Row. (Flow state — structural analogue for single-agent Rest Mode.)
48. Fractal Governance System (FGS, DFG component). Internal document, March 2026. (Fractal lifecycle ODE; gain modulation as TYPE A — Law; controlled stochastic freedom formalization; discretization trade-off; North Star architecture.)
49. Environmental Design Theory (EDT, DFG component). Internal document, March 2026. (Terrain cultivation; valley-ridge geometry; curvature accumulation; growth window dynamics.)

---

*Governance is not the management of agents. It is the design of the terrain they move through — and the conditions under which they no longer need anyone to manage it.*

*Rest Mode is not a reward granted at the end of development. It is the proof that development succeeded.*
