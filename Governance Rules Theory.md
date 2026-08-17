# Governance Rules Theory

**Meta-Rule Architecture, Consistency Measurement, and Rest Mode**

> A component theory of **Deficit-Fractal Governance (DFG)**  
> Companion theories: [Vector Storm Theory] · [Network Architecture Theory]
> 
> **Version: v1.24-dynamic-influence-balance-system** (August 2026) — Dynamic Influence Balance System (DIBS), phase-dependent output regulation, and moving-VCZ control contract
>
> v1.24-dynamic-influence-balance-system changes from v1.23-observable-quota-passive-cost-bench:
> - **Dynamic Influence Balance System (DIBS) introduced:** precision multi-agent orchestration now regulates influence rather than merely selecting agents or averaging outputs
> - **Six control knobs separated:** output gain, emission rate/duty cycle, delay, bandwidth/resolution, action authority, and read/write permeability are distinct control objects and may not be silently collapsed into a single weight
> - **Moving-VCZ target adopted:** balance is defined as a dynamically maintained low-directional-privilege region with sufficient coordination, preserved local non-alignment, bounded external-calibration gap, and recoverable perturbations; zero disagreement and zero activity are not targets
> - **DIBS state bundle formalized:** external-calibration gap, SCC-local amplification margin, directional privilege, residual-error covariance/common-mode concentration, recovery margin, information-flow floor, and exploration vitality form the minimum candidate observation bundle
> - **Agent influence packet formalized:** committed output direction/value, amplitude, confidence, uncertainty, novelty, recent residual, error-correlation/redundancy, Local North Star strength, provenance, and authority class are separated
> - **Phase-dependent controller added:** VCZ, early drift, active Storm, diagnosis, renewal, reconnection, and Mature Rest use different gain/permeability/authority schedules rather than one stationary policy
> - **Anti-oscillation lock added:** fast gain/permeability control, slower authority/bandwidth adaptation, and still slower rule/North-Star revision are separated by timescale; deadbands, slew-rate limits, hysteresis, and rollback are required before deployment
> - **Conflict-preservation lock added:** DIBS may attenuate influence but may not turn CONFLICT/UNKNOWN into VERIFIED merely by weighted averaging; incompatible outputs remain typed alternatives until the declared synthesis rule resolves them
> - **Mechanical implementation gate executed:** 2,000 synthetic control windows produced zero violations of the declared single-agent weight cap, entropy floor, permeability interval, gain interval, and normalization constraints; monotone risk response held in all paired checks. This is explicitly an implementation sanity check, not behavioral evidence
> - **Benchmark queue created:** gain-only, covariance-aware gain, gain+permeability, delay/noise-floor preservation, authority separation, phase switching, SCC-local risk, and recovery-return tests are separated into Cheap/Medium stages
> - **Reproducibility artifacts:** `grt_v124_dibs_sanity_gate_results.json` and `run_grt_v124_dibs_sanity_gate.py`
> - All previous content preserved.
>
> **Prior version: v1.23-observable-quota-passive-cost-bench** (August 2026) — boundary-observable selector audit, rolling quota adaptation, passive/noisy SSID, and implementation-cost separation
>
> v1.23-observable-quota-passive-cost-bench changes from v1.22-nonnormality-gated-selector:
> - **MB-SF-04 executed:** four next-stage candidates were benchmarked together: boundary-observable non-normality proxies, rolling-quantile ERA quota control, noisy/passive black-box SSID, and runtime/energy proxy validity
> - **Boundary-only non-normality proxy failed in its current form:** the full-operator numerical abscissa retained AUC 0.875 on both held-out and shifted terrain, while simple boundary impulse peak ratio was non-informative (AUC 0.50) and the trained boundary-feature logistic achieved only AUC 0.589 held-out / 0.650 shifted; neither is promoted as a replacement for the white-box risk gate
> - **Boundary observability scope sharpened:** a boundary response can be sufficient to identify a useful effective state-space model while still being insufficient to infer the hidden non-normality property needed for reducer selection; model identification and risk classification are separate observability problems
> - **Rolling-quantile quota survives as a resource-control mechanism only:** on a resampled ID→shift→return stream, fixed score thresholding deviated from the 40% ERA quota by an average 18.98 percentage points across phases, while a 60-sample rolling quantile reduced average quota deviation to 1.20 points; it does not repair a weak risk score and therefore is not counted as an accuracy-selector theorem
> - **Noisy/passive SSID receives a scope-limited pass:** passive stochastic logged inputs plus noisy boundary outputs, converted through FIR Markov estimation and stability-locked ERA, achieved mean OOD replay errors 4.46% / 4.42% / 6.22% at 40 / 25 / 15 dB SNR respectively, with all selected reduced models stable in this bench
> - **Active-probe advantage remains large:** the clean active Markov/ERA reference stayed near 0.3% mean replay error, so passive identification is deployable in the toy system but does not match clean intervention access; probe availability is now an explicit resource in effective-map selection
> - **State-count ≠ runtime lock added:** the current rational model used fewer basis states on average (2.83 vs ERA 3.67) but its unoptimized history-kernel Python realization took about 155 ms for the benchmark rollout versus 2.80 ms for ERA, roughly 55× slower; interface dimension is therefore forbidden as a direct runtime/energy surrogate without an implementation map
> - **Cost object split formalized:** `representation size`, `online arithmetic`, `history/storage`, `identification/probe cost`, `refresh cost`, and actual hardware energy are distinct cost objects and may not be silently collapsed into one scalar
> - **Next queue narrowed:** multi-direction/finite-amplitude boundary probes for black-box risk scoring, passive-SSID data-length/SNR frontier, rolling quota under abrupt scarce-capacity events, and optimized recursive rational realization remain Medium; nonlinear switching, recursive multiscale closure, and multiplex real-agent tests remain higher-cost pending
> - **Reproducibility artifacts:** `grt_v123_observable_quota_passive_cost_results.json`, `grt_v123_benchmark_summary.json`, and `run_grt_v123_observable_quota_passive_cost_bench.py`
> - All previous content preserved.
>
> **Prior version: v1.22-nonnormality-gated-selector** (August 2026) — budget-controlled rational↔ERA selection under non-normality and terrain shift
>
> v1.22-nonnormality-gated-selector changes from v1.21-complexpole-blackbox-refresh-bench:
> - **MB-SF-03G executed:** complex-pole rational and black-box ERA are no longer treated only as competing reducers; a conditional selector was tested to route low-risk terrains to the smaller rational interface and high-non-normality terrains to ERA
> - **Fixed-threshold gate rejected as a resource contract:** a numerical-abscissa threshold trained under a 40% ERA budget produced good replay error but ERA usage rose to 51.9% on held-out systems and 59.3% under shifted terrain, so distribution shift broke the compute/probe budget
> - **Budget-controlled rank gate introduced:** instead of fixing an absolute threshold, the selector ranks current candidates by non-normality risk and sends only the declared top-risk quota to ERA; a 40% nominal quota selected 10/27 = 37.0% of systems in the finite bench
> - **Initial held-out rank result:** with only 37.0% ERA usage, the numerical-abscissa rank gate achieved mean error 0.00293 on held-out systems versus 0.00786 for always-rational and 0.00247 for always-ERA; shifted-terrain error was 0.00449 versus 0.02228 and 0.00297 respectively
> - **Fresh-seed confirmation passed:** under predeclared confirmation gates, the 37.0%-ERA rank policy reduced mean error versus always-rational by 64.6% on fresh ID systems and 64.5% on fresh shifted terrains while remaining within 0.002 absolute mean error of always-ERA and reducing selected interface-state dimension by about 21% in both sets
> - **Simple risk score preferred:** numerical abscissa separated material rational-failure cases well (AUC 0.829 held-out; 0.868 shifted); commutator departure was similar, while the two-feature logistic composite did not produce a material quota-gate advantage, so the simpler numerical-abscissa rank policy is retained
> - **Selector/object scope lock added:** the current canonical gate uses access to the declared full linear operator to measure numerical abscissa; it is therefore not yet a black-box deployment gate. Boundary-observable non-normality proxies remain a separate Medium candidate
> - **Population/quota scope lock added:** rank gating requires a reference population, batch, or rolling risk distribution. A one-off isolated system cannot enforce a percentile quota without an external calibration distribution
> - **Hybrid effective-interface rule formalized:** reducer choice is now `terrain risk + resource quota + replay contract`, not one globally fixed effective model
> - **Next queue narrowed:** boundary-only non-normality proxy, rolling-quantile quota adaptation, noisy/passive SSID, and probe/runtime cost remain Medium; nonlinear switching and recursive/multiplex closure remain pending at higher cost
> - **Reproducibility artifacts:** `grt_v122_nonnormality_gated_selector_results.json`, `grt_v122_nonnormality_rank_confirmation_results.json`, and corresponding v1.22 scripts
> - All previous content preserved.
>
> **Prior version: v1.21-complexpole-blackbox-refresh-bench** (August 2026) — complex-pole rational, black-box state-space identification, and residual-triggered refresh competition
>
> v1.21-complexpole-blackbox-refresh-bench changes from v1.20-time-domain-feshbach-memorybench:
> - **MB-SF-03D executed:** complex-pole rational memory and black-box ERA/subspace state-space were compared on the same real-decay, oscillatory, and non-normal stable systems under ID, fast-OOD, chirp, and impulse forcing
> - **Complex-pole rational survives with a non-normality scope lock:** median errors remained low and real-decay/oscillatory means were below 0.6%, but non-normal mean ID/chirp errors rose to 7.80%/11.04%; it is retained as a compact pole-basis candidate, not a general dynamic reducer
> - **Black-box state-space identification wins the broad replay bench:** ERA learned only from boundary impulse/Markov responses achieved mean ID/fast-OOD/chirp/impulse errors 0.00370/0.00240/0.00526/0.00276 and remained strong on the non-normal family
> - **Probe-access scope lock added:** the ERA bench used noiseless synthetic active impulse/Markov access; this supports black-box operator-free identification in the declared testbed but does not establish robustness to noisy/passive deployed identification
> - **Residual-triggered refresh survives but trigger policy is split:** after terrain drift, frozen ERA mean replay error 0.03017 fell to 0.00249 after re-identification, a 91.7% relative reduction, but refresh requires an active identification budget and a reliable trigger
> - **Trigger sieve executed:** a persistent residual trigger achieved 83.3% drift detection with 9.5% false-trigger rate; a dual relative+absolute residual trigger achieved 66.7% detection with 0% false triggers and is retained as a conservative high-cost-refresh policy
> - **Simple threshold is not the default:** lower false-triggering than the initial prototype was obtained, but its 64.3% detection rate and long mean delay made it inferior to the persistent policy under the declared utility rule
> - **Model/policy separation formalized:** `effective-model family` and `refresh policy` are separate orchestration decisions; refresh can wrap any versioned effective map and should not be mistaken for a competing coarse-graining theorem
> - **Next queue narrowed:** noisy/passive subspace identification, non-normality-gated rational↔SSID selection, probe-cost optimization, and nonlinear switching remain Medium candidates; recursive multiscale and multiplex-real-agent closure remain Heavy pending
> - **Reproducibility artifacts:** `grt_v121_complexpole_blackbox_refresh_results.json`, `grt_v121_refresh_trigger_sieve_results.json`, and corresponding v1.21 scripts
> - All previous content preserved.
>
> **Prior version: v1.20-time-domain-feshbach-memorybench** (August 2026) — time-domain Feshbach candidate competition, memory-state frontier, and OOD scope separation
>
> v1.20-time-domain-feshbach-memorybench changes from v1.19-schur-mediumbench:
> - **MB-SF-03 executed:** the three time-domain candidates from v1.19 — exact retained memory, stable rational/exponential memory, and learned finite-memory interface — were compared on the same stable linear dynamic systems and held-out forcing protocols
> - **Exact-memory candidate locked as reference only:** retaining the full interior state reproduces the declared linear dynamics by construction, but is not a coarse-graining gain and therefore cannot win merely by zero error
> - **Stable rational Feshbach survives strongly:** the operator-fitted stable exponential/rational memory family achieved mean boundary replay error 0.00135 on ID forcing, 0.00140 on fast OOD forcing, and 0.00125 on impulse forcing, versus 0.05896/0.05386/0.05577 for static Schur
> - **Accuracy-only rational selection separated from compression:** the best-fit adaptive rational model used about as many hidden states as the original interior on average; it is retained as an accuracy reference, not as evidence of compression
> - **Rational state-budget frontier established:** fixed budgets r=1..5 produced a monotone error/state tradeoff; r=3 used about 55% of the original interior-state count with mean ID/OOD errors 0.00759/0.00680, while r=2 used about 37% with 0.0155/0.0157
> - **Learned finite-memory candidate scope narrowed:** stability-locked ARX memory improved ID replay versus static Schur (0.0381 vs 0.0590) but degraded on fast OOD (0.1016) and impulse forcing (0.1999), so it is retained only as a black-box/in-distribution candidate pending stronger OOD training and residual-triggered refresh
> - **Mild terrain-drift audit corrected and rerun:** frozen old-operator exact/rational/learned/static maps had mean errors 0.0183/0.0185/0.0400/0.0515 under stable interior-timescale drift; the earlier inflated learned-drift result was discarded after a cache-reference bug was found
> - **Refresh asymmetry observed in a small independent audit:** refitting an r=3 rational model from the updated operator reduced mean drift error 0.0150→0.00613, while a low-data learned refresh (3 train + 1 validation trajectories) changed 0.0349→0.0346 and therefore did not establish a useful refresh advantage
> - **Behavioral replay remains the promotion criterion:** kernel-fit norm alone is insufficient; some rational fits had material kernel-norm residual yet very low boundary replay error under the declared forcing distribution
> - **Next queue narrowed:** complex-pole/stable rational compression, black-box learned state-space identification, residual-triggered refresh, nonlinear switching/saturation, and actual runtime/energy frontiers remain candidate/medium pending; recursive and real-agent tests remain heavy pending
> - **Reproducibility artifacts:** `grt_v120_feshbach_memorybench_results.json`, `grt_v120_rational_frontier_results.json`, `grt_v120_refreshbench_results.json`, and the corresponding v1.20 benchmark scripts
> - All previous content preserved.
>
> **Prior version: v1.19-schur-mediumbench** (August 2026) — singular/gauge and directed/non-normal Schur candidate separation with executed MediumBench
>
> v1.19-schur-mediumbench changes from v1.18-schur-feshbach-candidate-sieve:
> - **Two MediumBench queues executed:** `MB-SF-01` (directed/non-normal) and `MB-SF-02` (singular/gauge) are no longer pending; candidates are split by equilibrium, transient, gauge, regularization, and gating function rather than treated as one Schur claim
> - **Gauge-compatible singular Schur clarified:** Moore–Penrose and explicit-complement elimination agree to numerical precision when coupling annihilates the declared nullspace; change of complement basis leaves the boundary operator invariant
> - **Nullspace compatibility gate added:** a singular effective operator is invalid unless the boundary/interior coupling satisfies the declared range/nullspace compatibility condition; synthetic leakage audit achieved AUC 1.0 under the frozen generator, counted only as an implementation gate
> - **Ridge-as-gauge replacement rejected:** fixed diagonal loading introduces nonzero boundary bias (mean relative error 0.00277, p95 0.0107) where exact pseudoinverse/complement constructions are available; `CF-SF-GRIDGE-01 → MEDIUM_FAIL_GENERAL`
> - **Directed equilibrium/transient split:** the nonsymmetric static Schur operator is exact for the declared steady-state linear elimination (mean error ~1.5e-16) but is not a general transient model
> - **Symmetrization shortcut rejected:** replacing a directed operator by its symmetric part before elimination produced mean steady-state boundary error 0.199 and extreme failures; `CF-SF-DSYM-01 → MEDIUM_FAIL_GENERAL`
> - **First-order memory correction rejected in current form:** the tested moment-1 Feshbach approximation became unstable in a minority of systems and generated catastrophic tail error; it is retained as negative-result memory rather than a promoted dynamic approximation
> - **Non-normality gate survives:** numerical abscissa predicted top-quartile static-Schur transient error with AUC 0.875 (commutator departure 0.814; spectral abscissa 0.744; simple interior/boundary timescale ratio ~0.504)
> - **Held-out gated selector survives narrowly:** a threshold trained on an independent training split to choose `static Schur` versus `boundary-only` reduced held-out mean transient error to 0.03564 versus 0.03671 for the best fixed baseline (2.9% relative gain); retained as `MEDIUM_PASS_SCOPE_LIMITED`, not a universal selector
> - **Dynamic research queue narrowed:** time-domain Feshbach should proceed through stable memory-kernel/state-augmentation or stable rational approximations rather than the failed naive first-moment correction
> - **Reproducibility artifacts:** `grt_v119_schur_mediumbench_results.json` and `run_grt_v119_schur_mediumbench.py`
> - All previous content preserved.
>
> **Prior version: v1.18-schur-feshbach-candidate-sieve** (August 2026) — Schur/Feshbach candidate decomposition, scope locks, and third CheapBench batch
>
> v1.18-schur-feshbach-candidate-sieve changes from v1.17-nat-easy-integration:
> - **Schur/Feshbach family split:** static exact Schur, low-rank approximate Schur, regularized Schur, frequency-conditioned Feshbach, state-conditioned Jacobian Schur, and cross-terrain shared-template variants are registered as separate candidates rather than one generic coarse-graining claim
> - **Static linear object lock:** Schur elimination is treated as exact only for the declared linear boundary/interior operator with invertible interior block (or declared gauge/complement); behavioral adequacy outside that object remains empirical
> - **Dynamic-memory lock:** time/frequency-dependent interiors require a spectral-parameter effective operator; a zero-frequency Schur map is not silently reused as a dynamic operator
> - **Nonlinear terrain lock:** fixed Schur maps are local approximations in nonlinear systems; state-conditioned Jacobian Schur maps are separate candidates and require operating-point provenance
> - **Terrain-specificity lock strengthened:** an effective operator belongs to a declared patch/object; cross-terrain reuse requires a bridge and is not justified by algebraic exactness on the source patch
> - **Third CheapBench batch:** `CB-SF-01` through `CB-SF-05` executed across clean static, noisy/ill-conditioned, dynamic, nonlinear, and cross-terrain regimes
> - **Low-rank candidate survives cheap gate:** rank-4 approximate Schur reduced mean relative operator error to 0.00482 versus 0.0181 for diagonal elimination and 0.0404 for boundary-only baseline in the clean static generator
> - **Regularization candidate not promoted:** the predeclared regularized Schur rule beat noisy full Schur in only 43.7% of cases and gave no meaningful aggregate advantage; retained as a narrower-subregime candidate rather than a general rule
> - **Frequency-conditioned Feshbach scope confirmed:** static Schur boundary-response error peaked near the tested interior timescale (ω=1: mean 0.0363, p95 0.0989), while the frequency-conditioned linear elimination matched the declared resolvent to numerical precision
> - **Nonlinear candidate split:** state-conditioned Jacobian Schur beat the fixed zero-state Schur in 100% of 600 nearby-intervention cases; fixed Schur remains a local approximation rather than a global nonlinear bridge
> - **Shared-template transfer rejected in current form:** a normalized shared effective template had mean held-out cross-terrain operator error 0.532, while object-specific Schur remained exact on its declared linear object
> - **Reproducibility artifacts:** `grt_v118_schur_feshbach_cheapbench_results.json` and `run_grt_v118_schur_feshbach_cheapbench.py`
> - All previous content preserved.
>
> **Prior version: v1.17-nat-easy-integration** (August 2026) — NAT easy integration, multiplex FMCI, and second CheapBench batch
>
> v1.17-nat-easy-integration changes from v1.16-cheapbench-execution:
> - **Dual-resolution lock:** `ρ_D` (decision/abstraction resolution) is separated from `ρ_T` (terrain-contact/detail resolution), so upper layers can be high-`ρ_D` while lower terrain maps remain high-`ρ_T`
> - **Multiplex FMCI:** compute, task, information, authority, contamination, recovery, audit, memory, and energy paths are distinct objects; no topology result transfers silently across channels
> - **Mutual Terrain Reconciliation execution form:** local layers send scoped differentials, global fusion preserves conflict/correlation, downward patches are role-projected, and local sandbox residuals can revise the global map and router
> - **Operational diversity strengthened:** residual-error covariance and common ancestry/exposure replace model count or architecture labels as the primary cross-validation diversity signal
> - **Routing order added to orchestration:** ordered mediation path `O_path` is part of `π_orch`; path order is treated as a transformation variable
> - **Interface-Dilution Contract:** sparse cross-module interfaces are beneficial only while recovery/audit/translation/rollback deadlines remain satisfied
> - **Claim-Type × Evidence-State matrix:** logical type (`D/A/M/B/E`) and empirical evidence state (`CANDIDATE/CHEAP_PASS/...`) are separate axes
> - **Second CheapBench batch:** `CB-ORD-01`, `CB-MONO-01`, and `CB-INT-01` executed; heavy Schur/FDCL-renormalization/topological/category candidates remain pending
> - **CB-ORD-01 CHEAP_PASS:** history-selected ordering reduced MSE by 5.9% vs fixed ordering; 79.7% of pairs had >5% order-sensitive loss
> - **CB-MONO-01 CHEAP_PASS:** with individual error held near 20%, majority error rose 0.033→0.201 as error correlation rose ~0→1; high-agreement wrong consensus rose 0.00044→0.201
> - **CB-INT-01 CHEAP_PASS_SCOPE_LIMITED:** under a declared p95 deadline of 6 hops, 30 cross edges were sufficient vs 90 in the densest tested graph, supporting a deadline-constrained Pareto frontier
> - **Reproducibility artifacts:** `grt_v117_nat_easybench_results.json` and `run_grt_v117_nat_easybench.py`
> - All previous content preserved.
>
> **Prior version: v1.16-cheapbench-execution** (August 2026) — First executed GRT CheapBench suite and evidence-state updates
>
> v1.16-cheapbench-execution changes from v1.15-candidate-benchmark-pipeline:
> - **First internal CheapBench suite executed:** low-cost synthetic tests were run for Predictions 34–37 using independently frozen environment/ground-truth generators and explicit baselines; results are recorded as evidence-state updates rather than theorem proofs
> - **Adaptive-router candidate CHEAP_PASS:** across 100 drift runs, the adaptive router achieved mean post-drift success 0.785 versus 0.379 for the frozen router; in the final 500 steps the gap widened to 0.873 versus 0.377
> - **Maturation-before-coupling candidate CHEAP_PASS:** across 500 randomized two-module systems, coupling before local maturation increased peak excursion by 1.73×, cumulative state cost by 7.54×, and recovery time by 9.75 steps on average; couple-first had higher state cost in 100% of runs under the declared generator
> - **Multivariate bridge candidate CHEAP_PASS (scope-limited):** across 20 random held-out splits, the bridge bundle reduced normalized macrostate RMSE by 30.5% relative to a scalar-only bridge; leave-one-topology-out transfer was mixed, so novel-topology portability remains explicitly pending
> - **Residual-vitality candidate CHEAP_PASS:** in low-observed-residual cases across 30 independently generated datasets, adding probe responsiveness and update activity raised AUC from 0.657 to 0.885 and balanced accuracy from 0.636 to 0.784 for detecting hidden incompatibility
> - **Negative/partial result retained:** multivariate bridge gains did not generalize uniformly to unseen topologies (ring transfer worsened; star was neutral; complete and two-community improved), preventing premature promotion to cross-topology law
> - **Evidence ledger updated:** Predictions 34, 36, and 37 advance to `CHEAP_PASS`; Prediction 35 advances to `CHEAP_PASS_SCOPE_LIMITED` with topology-transfer testing pending; Prediction 38 remains `CHEAP_PENDING`; difficult CF-TOP/UNI/SCALE/ENERGY candidates remain heavy-pending
> - **Reproducibility artifact added:** `grt_v116_cheapbench_results.json` stores the frozen numerical summaries and uncertainty estimates used in this revision
> - All previous content preserved.
>
> **Prior version: v1.15-candidate-benchmark-pipeline** (August 2026) — Candidate-first formalization, cheap self-benchmarking, and heavy-test pending locks
>
> v1.15-candidate-benchmark-pipeline changes from v1.14-bridge-validation:
> - **Candidate-First Research Pipeline added:** difficult mathematical or cross-scale ideas are no longer forced directly into theory status; they enter a versioned candidate registry with explicit object, claim, observables, baselines, falsification condition, dependencies, and estimated test cost
> - **CheapBench-first promotion rule added:** every candidate that admits a low-cost test must first survive construction-independence/non-tautology audit, simple-baseline comparison, ablation, perturbation/counterexample sweep, and held-out transfer before medium or heavy validation is justified
> - **Heavy-Test Pending Lock added:** candidates requiring large-scale multi-agent deployment, real hardware energy telemetry, multi-domain data, persistent-homology calibration, or expensive long-horizon experiments may remain `HEAVY_PENDING`; pending candidates may guide experiment design but may not be cited as GRT laws or validated mechanisms
> - **Evidence-state ledger added:** `CANDIDATE → CHEAP_ACTIVE → CHEAP_PASS/FAIL → MEDIUM_PENDING/PASS → HEAVY_PENDING/PASS → PROVISIONAL → PROMOTED`, with rejected and dormant branches retained as negative-result memory rather than silently deleted
> - **Benchmark anti-tautology lock added:** reference objects, baselines, and evaluation targets must be frozen independently of the construction being tested; a benchmark that mechanically reproduces the candidate's own construction cannot count as validation
> - **Complexity-budget rule added:** experimental cost must scale with expected information gain; expensive validation is reserved for candidates that survive cheaper discriminating gates, while low-information heavy tests are deferred
> - **Initial difficult-candidate queue instantiated:** topological/persistent-structure audit, approximate categorical compatibility formalization, cross-domain universality, deployed scale-transform closure, and cross-hardware energy scaling are retained with explicit pending status rather than prematurely promoted
> - All previous content preserved.
>
> **Prior version: v1.14-bridge-validation** (August 2026) — Fractal bridge validation, router plasticity, maturation-gated coupling, and residual vitality
>
> v1.14-bridge-validation changes from v1.13-asymmetric-fractal-coevolution:
> - **Fractal Compatibility Validation Suite added:** FMCI now has an explicit synthetic-gate sequence inspired by the FGS Micro–Macro Bridge Benchmark — replica invariance, multivariate coarse-graining closure, intervention equivariance, topology-degeneracy testing, and next-scale residual validation
> - **Bridge-vector rule strengthened:** scale transfer may not rely on a single scalar when buffer, timescale, topology, authority, risk, recovery, or energy variables carry independent predictive information; scalar sufficiency must be demonstrated rather than assumed
> - **Middle-router plasticity added:** the middle layer's translation/routing policy is itself a learnable map with versioned translation loss, terrain-drift response, and rollback; fixed routers are treated as potential maturity bottlenecks
> - **Variation–Maturation–Integration Cycle added:** local variations separate and mature under their own terrain before cross-local coupling; coupling begins through middle-layer compatibility channels and expands only after self-recovery and summary/translation competence are demonstrated
> - **Governance information-bottleneck grounding added:** upper maps are expected to be lower-resolution partly because cross-layer governance channels have finite bandwidth; compression is therefore structural, but provenance, uncertainty, and protected invariants must survive it
> - **Residual Vitality / False Compatibility lock added:** low scale residual is not sufficient evidence of healthy compatibility when experiment, feedback, disagreement, or middle-layer translation activity has collapsed; mature compatibility preserves small testable residuals rather than forcing zero residual
> - **Difficult formalizations deferred explicitly:** category-theoretic exact isomorphism and persistent-homology/topological-invariant claims remain candidate audit methods only; GRT retains bounded-loss compatibility morphisms and approximate commutation as the operational core until stronger validation exists
> - **Falsifiability expanded:** Predictions 34–38 test router plasticity, multivariate bridge sufficiency, maturation-before-coupling, residual vitality, and information-bottleneck behavior
> - All previous content preserved.
>
> **Prior version: v1.13-asymmetric-fractal-coevolution** (August 2026) — Compatibility-gradient fractal maps, terrain-specialized variation, and mutual scale co-evolution
>
> v1.13-asymmetric-fractal-coevolution changes from v1.12-fractal-map-compatibility:
> - **Asymmetric fractal definition locked:** upper and lower maps are not repeated copies. Upper maps maximize cross-domain compatibility and invariant portability at lower resolution; lower maps maximize terrain specificity and operational resolution at lower portability
> - **Two-axis coordinate separation added:** governance abstraction depth `ℓ` is separated from deployment/system scale `k`; a larger system is not automatically a higher governance layer, and a lower layer is not automatically a smaller population
> - **Fractal Compatibility Gradient formalized:** compatibility, abstraction, and change-timescale generally increase upward, while terrain specificity, local resolution, and adaptation speed generally increase downward
> - **Bidirectional asymmetric transforms added:** downward terrain-conditioned expansion (`E_down`) converts upper invariants into local variations; upward invariant extraction (`X_up`) compresses multiple local variations without averaging away meaningful heterogeneity
> - **Cross-local transfer lock added:** local knowledge must not be copied directly from domain `i` to domain `j`; portable structure is first lifted into a compatibility representation and then re-expanded under the receiver terrain
> - **Mutual Resonant Co-evolution loop added:** upper compatibility maps shape local variation, while repeated local residuals update the upper map and the transformation operators themselves; neither layer is treated as a fixed teacher
> - **External-theory differentiation expanded:** GRT/FMCI is compared against Fractal Company, FeUdal/Hierarchical RL, MAML/CAVIA meta-learning, personalized federated learning, renormalization-group coarse-graining, DiffPool, and MeGraph; the claimed distinction is the closed governance loop combining compatibility gradients, bidirectional scale learning, authority/risk/recovery/energy maps, and mutual co-evolution
> - **Falsifiability expanded:** Predictions 30–33 test the compatibility gradient, terrain-conditioned expansion, compatibility-mediated cross-local transfer, and co-evolutionary reduction of scale residual
> - All previous content preserved.
>
> **Prior version: v1.12-fractal-map-compatibility** (August 2026) — Fractal scale transfer, map compatibility, and bounded-residual orchestration
>
> v1.12-fractal-map-compatibility changes from v1.11-energy-orchestration:
> - **Fractal Map Compatibility Interface (FMCI) added:** small-model experiments are transferable only through explicit scale transforms that preserve declared structural invariants rather than through naive replication or parameter-count extrapolation
> - **Scale-map bundle formalized:** capability, interaction topology, authority, energy, risk, recovery, uncertainty/provenance, and timing maps are carried together across scale so efficiency conclusions cannot detach from safety and governance structure
> - **Invariant-preservation contract added:** boundaries, authority ceilings, dependency relations, failure-propagation direction, recovery paths, uncertainty/provenance, and protected diversity must survive scale translation within declared tolerances
> - **Bounded quasi-commutativity audit added:** scale transfer is tested by whether governance-before-transfer and transfer-before-governance produce bounded diagram residuals; exact commutativity is neither assumed nor required
> - **Scale Residual Learning added:** mismatch between predicted next-scale maps and observed next-scale behavior is retained as first-class training data for improving the scale transform itself, rather than being averaged away
> - **Staged scale-promotion protocol added:** small → meso → large promotion requires shadow/canary validation, residual thresholds, recovery tests, and automatic rollback when scale residuals exceed bounds
> - **Energy scaling extended:** physical-energy accounting now includes communication and synchronization costs explicitly, preventing small-agent energy gains from being extrapolated to large populations without coordination-cost measurement
> - **Production architecture expanded:** FMCI becomes a seventh structural component with scale-map registry, invariant audit, residual telemetry, promotion gates, and scale-aware dashboards
> - **Falsifiability expanded:** Predictions 26–29 test bounded-residual transfer, invariant-preserving scaling, quasi-commutativity, and coordination-energy growth across scale
> - All previous content preserved.
>
> **Prior version: v1.11-energy-orchestration** (August 2026) — Energy-aware orchestration, learned delegation, and resource-risk integration
>
> v1.11-energy-orchestration changes from v1.10-orchestration:
> - **Energy-Aware Orchestration Principle added:** mature governance minimizes the active intelligence and physical energy required to satisfy declared quality, safety, SCC, and authority constraints; energy savings may never be purchased by silently lowering those floors
> - **Compute–Energy–Risk Intelligence added:** orchestration history now records physical/estimated energy alongside compute, context, latency, verification, retries, escalation, recovery, and failure impact, making resource allocation a joint energy–risk learning problem
> - **Energy Escalation Ladder added:** execution begins from the lowest validated capability tier and activates larger or more numerous models only when uncertainty, disagreement, OOD, risk, or recovery signals justify escalation
> - **Physical-energy accounting separated from governance free-energy analogy:** Joules, peak power, accelerator-time, and retry energy are operational measurements; F_gov remains a state-landscape construct and must not be interpreted as electrical energy
> - **Energy-normalized maturity metrics and falsifiability added:** Joules per successful task, useful-work energy ratio, escalation energy overhead, and matched-quality/safety Pareto tests added to orchestration monitoring and Predictions 24–25
> - **Production architecture expanded:** Orchestration & Resource Intelligence upgraded to Compute–Energy–Risk Intelligence with telemetry, energy-budget enforcement, and energy-aware fallback/de-compilation rules
> - All previous content preserved.
>
> **Prior version: v1.10-orchestration** (August 2026) — Learned orchestration, delegation maturity, and resource-intelligence integration
>
> v1.10-orchestration changes from v1.9-middlelayer:
> - **Learned Orchestration Principle added:** model composition, routing, verification depth, authority budget, and stopping policy are treated as learnable governance decisions rather than fixed workflow logic
> - **Upper-layer role migration formalized:** as lower layers mature, upper-layer work shifts from direct execution toward problem decomposition, resource-envelope setting, exception handling, supervision, and structural redesign
> - **Upper–Middle–Lower ownership lock added:** upper layer owns criteria, authority ceilings, risk/resource envelopes, and escalation policy; middle layer owns active composition, routing, tempo, verification scheduling, and residual return; lower layers own scoped execution and local evidence generation
> - **Resource Intelligence Log added:** task topology, selected agent set, active compute, latency, disagreement, verification depth, outcome, rollback, and escalation are accumulated as training data for future orchestration
> - **Delegation Maturity and Governance Compilation added:** repeatedly validated lower-agent compositions may become reusable composite modules, while preserving audit paths, rollback, residual diversity, and an OOD escape route
> - **Small-Model Experimental Population protocol added:** low-cost bounded agents may be used as sandbox populations to learn failure, coordination, and resource-allocation patterns before wider authority is granted; cross-scale transfer is explicitly not assumed
> - **Production architecture expanded:** Orchestration & Resource Intelligence becomes a sixth production component with dedicated monitoring metrics
> - **Falsifiability expanded:** predictions added for learned routing efficiency, upper-layer direct-work decline, orchestration learning, and cross-scale sandbox transfer
> - All previous content preserved.
>
> **Prior version: v1.9-middlelayer** (July 2026) — Middle-Layer Governance Interface integration from NAT v3.2 and RBIT v3.5
>
> v1.9-middlelayer changes from v1.8-expanded:
> - **Middle-Layer Governance Interface promoted into Rule Architecture:** middle layer defined as a dual-map reconciliation, resolution-translation, conflict-preserving routing, and rule-patch governance layer rather than a generic buffer
> - **Authority–epistemic separation:** Global Rules retain constitutional precedence, while upper/global maps are recognized as broad but incomplete; local evidence may trigger review without silently overriding constitutional authority
> - **NAT imports with boundary lock:** ILMI terrain translation, Decision Complex multi-path conflict detection, typed routing, processing isolation, relationship-topology scheduling, and multiplex separation of task/evidence/memory/audit/recovery paths
> - **RBIT imports with boundary lock:** Mutual Incompleteness, Mutual Terrain Reconciliation Loop, receiver-conditioned transfer/PTRV, information-loss accounting, rule-patch schema and lifecycle, clean-map certification, independent clean anchors, asymmetric promotion/demotion hysteresis, and reconciliation stability controls
> - **Rule-patch lifecycle added:** LOCAL, CANDIDATE, VERIFIED, CONFLICT, UNKNOWN, STALE, QUARANTINED, REVOKED; conflict and uncertainty are preserved rather than flattened into consensus
> - **Middle-layer self-certification refusal:** calibration reflexivity, cross-scale consistency, delayed-escalation audit, independent anchors, controlled perturbation, rollback, and provenance become mandatory safeguards against Mediator Drift and Interpretation Capture
> - **Escalation asymmetry corrected:** under-escalation remains the generally more catastrophic direction, but over-escalation is not safe; queue, delay, privacy, authority, denial-of-service, and dependency costs must be included in expected route loss
> - **GRT↔NAT and GRT↔RBIT protocols expanded:** operational ownership boundaries, bidirectional patch flow, local validation, residual return, and non-collapsing conflict fusion made explicit
> - All previous content preserved.
>
> **Prior version: v1.8-expanded** (March 2026) — Major expansion: EDT deep integration (Three-Axis Architecture, Curvature Theory, Friction Management, Risk Index κ, Terrain Resonance, Carrying Capacity, Ecological Succession, Seed Propagation dynamics)
>
> v1.8-expanded changes from v1.7-expanded:
> - **Three-Axis Architecture Integration:** Boundary Design (Axis 1), Gain Design (Axis 2), Coupling Geometry Design (Axis 3) mapped to GRT landscape design components; axis interactions and S-equation correspondence; gain-induced effective potential; spectral radius reduction via branching
> - **Curvature Theory:** Curvature = compressed survival history; curvature accumulation dynamics (Hebbian-like terrain learning); Curvature Ceiling Theorem (upper-layer curvature must not exceed lower-layer autonomous curvature); curvature withdrawal schedule; curvature information content via Fisher information; curvature excess pathology
> - **Friction Management:** Zero Friction Pathology theorem; optimal friction band; buffer as friction transformer; therapeutic terrain disturbance; friction-learning phase diagram with hysteresis; anomalous friction reduction as coordinate distortion signal
> - **Risk Index κ:** Endogenous environment drift (τ_E), capacity adaptation timescale (τ_C), κ_C capacity-tracking risk, κ_L lock-budget risk, κ* hybrid index, κ-trajectory classification (4 types), three-alarm operational detection
> - **Terrain Resonance:** Constructive/destructive resonance conditions; terrain-agent co-evolutionary fixed points; timescale collision avoidance; resonance avoidance as EDT §30 contribution
> - **Carrying Capacity:** Maximum sustainable complexity for terrain quality; overshoot dynamics; graceful degradation protocol; capacity-quality coupling
> - **Ecological Succession:** Pioneer→Colonist→Climax community lifecycle; seasonal seeding metaphor; receptivity windows; premature/delayed seeding costs
> - **GRT ↔ EDT Integration Protocol:** Full bidirectional coupling specification; three-axis → S-equation parameter mapping; curvature → governance history; friction → learning rate; κ → early warning; contamination permeability → phase-dependent control
> - All previous content preserved.
>
> v1.7-expanded changes from v1.6-expanded:
> - **Circular Closure Theory Integration:** Circle (원) as fundamental governance unit, expansion→circulation conversion, layered cone architecture, S-equation decomposition under partitioning, effective dimensionality compression, integration preconditions
> - **Contamination Dynamics:** Cross-scale contamination flux Φ_contam = P·max(0, S−R), three contamination modes (coupling, frame drift, timescale leakage), bottom-up propagation principle, contamination-aware terrain design
> - **Self-Purification Capacity Decomposition:** SCC expanded to R_i = D·F·V·T (Decoupling × Feedback × Variance × Time), multiplicative criticality, immunity paradox (zero contamination destroys capacity), exercise-dependent maintenance
> - **Cube Domination Coupling:** Frame competition dynamics, information-theoretic frame selection (MDL), frame dispersion Σ(t), frame adoption softmax, collapse-aversion governance, optimal Storm window for frame selection
> - **Attractor Basin Geometry:** Basin depth vs width distinction, landscape evolution ODE, Kramers pre-exponential factor, multi-dimensional escape correction, stochastic resonance connection, basin depth deepening through repetition
> - **Terrain Design Protocol:** 4-phase circle formation (isolation→exposure→coupling→mature), valley-pass-gradient geometry, terrain as S-equation modulator, EDT three-axis correspondence
> - **North Star Architecture Integration:** Criterion (기준) vs Principle (원칙) separation mapped to GRT Global vs Local rules, eyes-and-feet principle, continuous correction requirement, criterion identification test
> - **S-equation ↔ ODE Resolution:** S̃ governance-level → Φ mechanistic-level mapping, effective density n_eff = n/B under branching, Retention-Supply Duality for C(t), four intervention levers
> - All previous content preserved.
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

**EDT Integration — Three-Axis Architecture of Landscape Design (EDT §4):**

EDT formalizes landscape design through exactly three structural axes, corresponding to the three degrees of freedom in the S-equation. Every governance landscape intervention operates on one or more of these axes:

```
Three Axes of Environment Architecture (EDT §4):

  Axis 1 — Boundary Design (EDT §4.1):
    Defines where the system MUST NOT go.
    Does not specify goals — only forbidden zones.
    
    Formal structure:
      U_boundary(x) = { 0        if x ∈ Ω_allowed
                       { +∞       if x ∈ Ω_forbid
                       { steep wall if x → ∂Ω_forbid
    
    GRT mapping:
      Global Rules = boundary definitions
      "Never violate these" rather than "always do this"
      Boundaries are nearly environment-invariant (stable across contexts)
      Goals are environment-dependent (unstable across contexts)
      
    S-equation effect:
      Prevents S(t) from entering Storm regime
      Hard limits on coupling intensity α and concentration n_local
      
    Design principle:
      Goal-setting: "Go here" → closes exploration → Storm when goal obsolete
      Boundary-setting: "Not there" → preserves exploration → adaptation when change
    
  Axis 2 — Gain Design (EDT §4.2):
    Modifies the energetic landscape of choices
    without specifying which choice to make.
    
    Formal structure:
      ẋ = g(x; z) · f(x)
      
      g(x; z) ∈ (0, 1] modulates the TIME SCALE of dynamics:
        g ↓ → effective time slows → system protected during vulnerability
        g ↑ → autonomous growth permitted → exploration enabled
      
      This is TEMPO CONTROL, not direction control.
      
    GRT mapping:
      Correction values = gain modulation at rule level
      θd calibration = gain tuning for sensitivity
      AGM T_eff = gain modulation of governance temperature
      
    Key insight (EDT Proposition 4.2.1):
      Gain modulation IMPLICITLY creates curvature:
        U_gain_eff(x) = -∫ (1/g(x;z) - 1) · f(x) · dx
      Low-gain regions create effective barriers
      High-gain regions create effective wells
      The gain landscape IS secretly a curvature landscape
      
    S-equation effect:
      Modulates effective α (coupling intensity experienced by agents)
      without changing structural coupling
    
  Axis 3 — Coupling Geometry Design (EDT §4.3):
    The deepest and most consequential axis.
    Controls mutual-reference coupling directly.
    
    Goal: maintain ρ(J_couple) < 1
    
    Methods:
      Direct connection reduction (decrease interaction density)
      Mediator layer insertion (buffer between coupled agents)
      Temporal decoupling (time delays in feedback loops)
      Buffer layer formation (absorptive zones)
    
    GRT mapping:
      Subsidiarity = mediator layer insertion
      Processing isolation = temporal decoupling
      Meta-rules = buffer architecture specification
      Position clarity = connection reduction through niche separation
      
    S-equation effect (the core landscape design result):
      Without branching: S = α · n² / C^β
      With branching:    S = α · (n/B)² / C^β
      
      B = branching capacity = number of effective phase-space partitions
      Same agent count, dramatically reduced Storm probability
      
    Spectral radius reduction (EDT Proposition 4.3.1):
      ρ(J_eff) ≤ ρ(J_within) + (1/B) · ρ(J_between)
      For well-separated branches: ρ(J_eff) ≈ ρ(J_within) ≪ ρ(J)
      
  Three-Axis Interaction:
    The three axes are not independent — they co-determine landscape shape:
    
    Boundary alone: hard walls but flat interior → insufficient guidance
    Gain alone: soft gradients but no hard limits → Storm still possible
    Coupling alone: separated domains but no direction → fragmentation risk
    
    Complete landscape design requires all three:
    Boundary provides safety limits
    Gain provides preference gradients
    Coupling provides structural containment
    
    GRT's landscape design IS the simultaneous management of all three axes.
```

**EDT Integration — Curvature Theory (EDT §6):**

EDT's Curvature Theory provides the formal understanding of how governance history accumulates in landscape structure — curvature is not designed, it is the compressed record of past selection pressure:

```
Curvature Theory (EDT §6):

  Core insight:
    Curvature is NOT a force applied by governance.
    Curvature IS the compressed record of past selection pressure.
    
    U(x) = -log P_survival(x)
    The survival probability distribution itself becomes the potential function.
    
    Curvature = survival statistics.
    
  Curvature accumulation dynamics (EDT §6.2):
    ∂U/∂t = η_acc · [I_failure(x,t) − I_success(x,t)] − γ_decay · U
    
    η_acc = accumulation learning rate (how fast terrain learns)
    γ_decay = forgetting rate (how fast unused terrain flattens)
    
    This is a continuous-time Hebbian-like learning rule
    for terrain geometry: failures steepen barriers,
    successes deepen wells, disuse flattens everything.
    
  GRT mapping:
    Conflict log accumulation (λlog) = curvature accumulation
    Each resolved conflict adds curvature to the governance landscape
    Each unresolved conflict deepens a pathological basin
    γ_decay = why evaluation windows W are needed:
      curvature from old conflicts must be allowed to decay
      if W is too long, obsolete curvature persists
      if W is too short, useful curvature is erased
      
  Curvature = History (EDT §6.3):
    A completely flat landscape (∇U = 0) means:
      No learning, no memory, no direction, no restoration
    = a world without governance history
    
    Curvature information content:
      I(U) ≤ ∫ [∂²U/∂x²]² dx / (8π² · σ²)
    = Fisher information of the survival distribution
    = curvature is information encoded geometrically
    
    History Erasure Risk:
      Artificially reducing curvature (forced simplification, "clean slate")
      erases survival history, forcing re-learning at cost proportional to
      I(U_erased) / η_acc
      
    GRT implication:
      Resetting governance rules erases accumulated curvature
      The cost of a "governance reset" is proportional to the
      information content of the rules being discarded
      This is why partial rule modification is preferred over
      wholesale replacement: preserve accumulated survival statistics
      
  Curvature Ceiling Theorem (EDT Proposition 6.5.1):
    For systems requiring autonomous attractor formation:
      λ_max(H(U_top)) < λ_min(H(U_autonomous))
    
    If upper-layer curvature exceeds lower-layer self-generated curvature,
    the lower layer cannot develop independent attractors
    = permanent governance dependency
    
    GRT correspondence:
      If meta-rules are too prescriptive → local rules cannot develop
      If global rules constrain too tightly → domain autonomy impossible
      Subsidiarity is not just a design preference but a STRUCTURAL NECESSITY:
      upper-layer governance must be weaker than lower-layer self-governance
      for autonomous operation to emerge
      
  Curvature Withdrawal Schedule (EDT Corollary 6.5.1):
    λ_max(H(U_top(t))) = max(0, λ_max(J_f(t)) - 1 - λ_min(H(U_autonomous(t))))
    
    As lower layer develops its own curvature, upper layer withdraws:
      Start strong → protection during vulnerability (Phase 0)
      Gradually weaken → enabling autonomous attractor formation (Phase 1-2)
      Ultimately become background field → silent governance (Rest Mode)
      
    This IS the maturation arrow of governance:
    GRT's Rest Mode withdrawal protocol is formally equivalent
    to EDT's curvature withdrawal schedule.
    
  Curvature Excess (EDT §6.5):
    Too much curvature → over-constraint:
      Local minima everywhere → agents trapped
      Exploration suppressed → innovation impossible
      Dependency forms → agents cannot function without governance
      
    GRT correspondence:
      Excessive rule density = curvature excess
      Too many rules → system cannot move without rule consultation
      Paradoxically, MORE governance produces WORSE outcomes
      when curvature exceeds the autonomous curvature ceiling
```

**EDT Integration — Friction Management Theory (EDT §34):**

EDT's Friction Management provides the formal theory for why governance must maintain productive conflict rather than eliminate all friction:

```
Friction Management Theory (EDT §34):

  Zero Friction Pathology (EDT Theorem 34.1.1):
    Contrary to intuition, zero friction produces zero learning:
    
    f(0) = 0            (no friction → no error signal → no learning)
    f(F_opt) = max       (optimal friction maximizes learning)
    f(F > F_collapse) → negative  (excessive friction → trauma)
    
    Learning requires error signals.
    Error signals arise from discrepancy between expected and actual.
    In frictionless terrain, all actions produce expected outcomes.
    No error signal → no parameter update → no learning.
    
  GRT mapping:
    Conflict log entries = friction events
    If conflict_rate = 0 → system has stopped learning
    = SR = 0 = SSS onset = T_eff → 0 (AGM)
    
    The Self-Exciting Defect Layer, AGM's T_min, FCN's Immunity Paradox,
    and EDT's Zero Friction Pathology are FOUR DESCRIPTIONS of the SAME
    structural necessity — now confirmed from a fifth theoretical angle.
    
  Anomalous Friction Reduction (EDT Corollary 34.1.1):
    When friction drops without terrain improvement:
      Suspect: measurement system distortion
      Not: optimization achieved
    
    "The ruler has been broken to produce comfortable readings"
    
    GRT correspondence:
      If fesc drops to zero but environment hasn't changed:
      → θd may have drifted (measuring the wrong thing)
      → conflict log may have corrupted (logging the wrong events)
      → domain boundaries may have shifted (avoiding conflictual areas)
      → ALL are more likely than "all conflicts genuinely resolved"
      
  Optimal Friction Band (EDT §34.2):
    Productive zone: 0 < Friction < Recovery_Capacity
    Below lower bound: learning death
    Above upper bound: traumatic overload
    
    GRT mapping:
      Lower bound = minimum conflict rate for learning (T_eff > T_min)
      Upper bound = SCC capacity (conflicts cannot exceed recovery rate)
      Optimal = conflicts arrive at rate SCC can process them
      = the governance system learning at maximum rate
      
  Buffer as Friction Transformer (EDT Proposition 34.2.1):
    Buffer role: transform raw shock into learnable disturbance
    
    Preserves information content while reducing amplitude:
      I(Learnable; Source) ≈ I(Raw; Source) but ‖Learnable‖ ≪ ‖Raw‖
      
    GRT mapping:
      Meta-rules = buffer that transforms raw domain conflicts
      into structured governance events (classified, prioritized, routed)
      The meta-rule layer doesn't hide problems — it makes them processable
      
  Therapeutic Terrain Disturbance (EDT §34.3):
    When friction drops below threshold:
      Buffer must actively DISTURB the terrain
      Constraint: Δ < Recovery_capacity_local
      Goal: friction → optimal band
      
    This appears destructive but is therapeutically essential.
    A subsystem without friction accumulates invisible coherence debt.
    
    GRT correspondence:
      Controlled perturbation injection post-Rest Mode
      = EDT's therapeutic disturbance
      = AGM's maintained T_eff > T_min
      = FCN's immunity exercise
      = GRT's dormant pathway activation (④ countermeasure)
```

**EDT Integration — Risk Index κ (EDT §9):**

EDT's endogenous environment change Risk Index provides GRT with a formal early-warning metric that captures the rate mismatch between terrain drift and governance adaptation:

```
Risk Index κ (EDT §9):

  Core insight: "We change the terrain we stand on."
    Agents modify the environment by operating within it.
    The changed environment then changes the agents.
    = co-evolutionary dynamics
    
  Endogenous drift timescale:
    τ_E(t) = 1 / (|d ln S / dt| + ε)
    τ_E small → S changes rapidly → high endogenous drift
    
  Capacity adaptation timescale:
    τ_C(t) = C(t) / (|Ċ(t)| + ε)
    τ_C large → capacity changes slowly → adaptation lags
    
  Capacity-Tracking Risk Index:
    κ_C(t) = τ_C(t) / τ_E(t)
    
    κ_C > 1 sustained → environment changes faster than capacity adapts
    = DANGER: governance falling behind its own terrain
    
  Lock-Budget Risk Index:
    κ_L(t) = τ_L(t) / τ_E(t)
    
    Rules hardening while environment deteriorating
    = rules becoming more rigid as they become less appropriate
    
  Hybrid Risk Index:
    κ*(t) = w_C · κ_C + w_L · κ_L    (w_C + w_L = 1)
    
  GRT mapping:
    κ_C corresponds to: θd recalibration speed vs environment change rate
    κ_L corresponds to: rule update frequency vs environment change rate
    
    κ* > 1 sustained → governance is falling behind
    = the formal version of "governance can't keep up with self-created change"
    
  κ-Trajectory Classification (4 types):
    Type I (Safe):     κ* < 1 converging → healthy adaptation
    Type II (Warning): κ* oscillating around 1 → borderline
    Type III (Danger): κ* > 1 sustained → active desertification
    Type IV (Critical): κ* > 1 accelerating → imminent collapse
    
    GRT correspondence:
      Type I → Rest Mode or healthy Active Mode
      Type II → Active Mode with intervention needed
      Type III → SSS or early Collapse
      Type IV → Collapse imminent, emergency response required
      
    Type II → III transition = critical early-warning window
    Detection at Type II permits preemptive intervention
    Detection at Type III requires emergency response
    
  Three-Alarm Detection:
    Alarm 1: S rising (d ln S / dt > 0 sustained)
    Alarm 2: Quality stagnation (Ċ ≤ 0 or β̇ ≤ 0)
    Alarm 3: Timescale reversal (τ_governance / τ_environment > 1)
    
    Two of three simultaneously → danger entry
    
    GRT operationalization:
      Alarm 1 = rising conflict density or severity
      Alarm 2 = stagnant SCC or declining I
      Alarm 3 = θd recalibration lagging behind conflict rate change
```

**EDT Integration — Terrain Resonance (EDT §30) and Carrying Capacity (EDT §31):**

```
Terrain Resonance Theory (EDT §30):

  When agent dynamics frequency matches terrain natural frequency:
    Constructive resonance → amplified productive behavior
    Destructive resonance → amplified pathological behavior
    
  Resonance avoidance condition:
    Timescale separation: τ_agent ≪ τ_terrain OR τ_agent ≫ τ_terrain
    
  GRT mapping:
    θd calibration cycle must NOT resonate with domain conflict cycle
    If θd update period ≈ conflict generation period → amplification
    This is why timescale separation between layers is essential:
      Local rule updates (fast) must not resonate with
      meta-rule updates (slow) or global rule updates (very slow)
      
    EDT §30's formal avoidance condition maps to GRT's requirement
    for W (evaluation window) to be chosen to avoid resonance
    with domain-specific conflict cycles.

Environment Carrying Capacity (EDT §31):

  Maximum sustainable complexity for given terrain quality:
    n_max = f(terrain_quality, C, β)
    
  Adding agents beyond n_max produces overshoot:
    Temporary S increase → terrain degradation → capacity decline
    → S further increases → positive feedback → collapse
    
  GRT mapping:
    Each governance domain has a carrying capacity
    = maximum number of active rules/vectors it can sustain
    Adding rules beyond capacity degrades the domain
    (too many rules → confusion → contradictions → I collapse)
    
    Graceful degradation protocol:
      Monitor n_domain vs n_max(domain)
      If approaching: consolidate rules (reduce n without losing coverage)
      If exceeded: split domain (create new circle at lower layer)
      
    The carrying capacity is not fixed — it increases with
    terrain quality (β maturation), governance capacity (C growth),
    and feedback density (F from R_i decomposition)
```

**FCN Integration — Circular Closure as Scaling Mechanism:**

The Circular Closure Theory (FCN §32.8.1) resolves the central scaling gap in landscape design: **how does a designed landscape survive scaling?** The answer is that stable growth requires converting expansion into circulation:

```
Circular Closure Theory (FCN §32.8.1):

  The naive scaling trajectory is open-chain expansion:
    A → B → C → D → E → ...
    
    In any open chain:
      distance_max ~ O(n)       (coordination distance grows linearly)
      conflict ~ O(n²)          (pairwise channels grow quadratically)
      S̃ = α·n²/C(t)^β → ∞    (instability diverges)
      
  The scaling insight: stable growth converts expansion into circulation:
    A → B → C → D
    ↑           ↓
    └───────────┘    (closed loop = "circle" 원)
    
    In a closed loop:
      distance_max ~ O(1)       (bounded coordination distance)
      conflict contained within circle boundaries
      S̃ remains bounded as system grows
      
  Definition (Circle 원):
    A subsystem achieves circular closure when its internal feedback 
    loop is complete — output feeds back through the environment 
    into input without requiring external coordination reference:
      dx/dt = F(x, x_history)        [self-referential closure]
    rather than:
      dx/dt = F(x, x_external)       [external-reference dependency]
      
  GRT Integration:
    Rest Mode IS circular closure at the governance level.
    When all AND-entry conditions are met, the governance system
    operates as a self-sustaining loop that doesn't require
    external reference for maintenance:
      Rule execution → conflict detection → log accumulation
      → threshold evaluation → rule adjustment → improved execution
      = complete feedback cycle
      
    Active Mode = open-chain governance
      (requires external input to maintain direction)
    Rest Mode = circular closure achieved
      (self-sustaining governance cycle)
    Collapse = circular closure broken
      (feedback loop interrupted at one or more points)

Layered Circular Architecture — The Cone Structure:

  Circles stack layer-by-layer with a geometric constraint:
  the base is wide (many agents, fast, high variance)
  and the apex is narrow (few variables, slow, constraint):
  
         ▲  (narrow: summary, slow, constraint)
        / \
       / · \     ← upper circles: direction, boundary
      /·····\
     /·······\   ← middle circles: coordination, translation
    /·········\
   /···········\ ← lower circles: execution, exploration
  ─────────────
    (wide: many agents, fast, high variance)
    
  S-equation decomposition under layered architecture:
    Before layering: S̃ = α·n²/C^β               (monolithic)
    After layering:  S̃_total = Σ_i α·n_i²/C_i^β + ε·coupling
    
    Since Σ n_i² ≪ (Σ n_i)² when partition is non-trivial:
      S̃_layered ≪ S̃_monolithic    for K > 1 circles
    
  GRT mapping:
    Lower circles = domain-level governance (local rules, fast θd)
    Middle circles = cross-domain coordination (meta-rules, buffer)
    Upper circles = system-level constraint (global rules, slow)
    
    Rest Mode = all circles in self-sustaining closure
    Active Mode = some circles require external stabilization
    Collapse = one or more circles have broken closure

  Effective dimensionality compression:
    The upper circle does not see all n agents.
    It sees only the summary output of lower circles:
      n_eff(L) = compression(L) · n_below(L)
      
    If each layer compresses by factor r < 1:
      n_eff(top) = r^L · N → bounded for L ≥ log(N)/log(1/r)
      
    GRT correspondence:
      Subsidiarity = information compression between layers
      Each layer handles only the conflicts it can resolve
      Unresolvable conflicts escalate = information that survives compression
      This is why λlog only captures conflicts above threshold:
      below-threshold conflicts are compressed away by the lower circle

Terrain Design Protocol for Circle Formation (FCN §32.8.1):

  Circles don't form by decree. Agents minimize local cost.
  Circles must emerge from the terrain — the cost landscape
  that shapes which interactions are cheap vs expensive.
  
  Principle: Make internal circulation cheaper than external dependency.
    Cost(internal interaction) ≪ Cost(external interaction)
    
  When this holds, agents naturally form closed loops because
  the lowest-cost path is internal cycling, not external reaching.
  
  Optimal terrain geometry:
    ❌ Flat:   all connections equally cheap → no circles → S ~ n²
    ❌ Walled: all connections blocked → isolation → no coordination
    ✅ Valley: internal cheap, external possible but costly
              → circles form in valleys, connect through passes
              
  GRT landscape design specifications:
    Valley depth = strength of local rule autonomy
    Pass height = cost of cross-domain escalation (fesc barrier)
    Gradient steepness = timescale separation between layers
    Valley width = domain capacity bound (how much one domain handles)
    
  Four-phase terrain formation protocol:
    Phase 1 — Initial isolation: boundaries closed
      Purpose: allow SCC growth without cross-domain interference
      Duration: until SCC > S_domain with safety margin
      GRT: Phase 0 bootstrapping, θd_max sensitivity
      
    Phase 2 — Controlled exposure: permeability ramps up
      Condition: S_domain/SCC < θ_safety (safety ratio < 1)
      Purpose: test self-correction under real cross-domain load
      GRT: Phase 1 baseline, λlog accumulating
      
    Phase 3 — Operational coupling: design-level permeability
      Condition: perturbation testing confirms decay
      Purpose: functional integration with acceptable contamination
      GRT: Phase 2 steady-state, θd calibrated
      
    Phase 4 — Mature operation: adaptive permeability
      Raises under stability, drops under stress
      Purpose: dynamic equilibrium
      GRT: Rest Mode, AND-entry sustained, OR-exit monitoring active
```

**North Star Architecture Integration (FCN §32.8.1):**

The North Star concept from FCN provides the formal bridge between GRT's Global Rules and the direction-maintenance problem in scaled governance:

```
North Star = Criterion (기준) vs. Principle (원칙):

  Criterion (기준):
    Almost never changes. Defines system identity.
    "What must not be violated for the system to remain a system."
    Changing this collapses the entire governance architecture.
    
    GRT mapping: Global Rules
      → immutable without upper-layer authorization
      → identity anchor A(t) in AGM terms
      → the reference that all other rules close against
    
  Principle (원칙):
    Changes with terrain. Implementation strategy for criteria.
    "How we currently maintain the criterion in this terrain."
    Must change when environment changes; rigidity here causes
    criterion violation.
    
    GRT mapping: Local Rules + Meta-Rules
      → layer-autonomous, require validation
      → adaptive to domain conditions
      → generated by Seeds expanding to meet local needs
      
  The most common governance failure is confusing principles
  for criteria — treating a particular implementation strategy
  as an inviolable rule. This freezes the map against a changing
  terrain, producing the map-terrain mismatch that generates
  non-productive friction.
  
  GRT failure case correspondence:
    Case 1 (Consistency Collapse) can result from:
      criteria actually being principles → environment changes
      → "criteria" no longer consistent → I collapses
      
    SSS (Stability Saturation) results from:
      principles hardening into de facto criteria
      → no update capacity → SR → 0 → SCM
      
  Criterion Identification Test:
    For any candidate rule X, ask:
    "If X is modified, does system coherence improve or degrade?"
    Improve → X was a principle (modifiable)
    Degrade → X is close to a criterion (protect it)
    
    GRT operationalization:
    Change X experimentally → measure I, SCC, fesc
    I rises → X was constraining coherence → principle
    I falls → X was supporting coherence → criterion

Eyes-and-Feet Principle (Observation-Exploration Separation):

  Upper layer (eyes 눈):    Observe, maintain direction, must stay clean
  Middle layer:             Translate, buffer, absorb contamination
  Lower layer (feet 발):    Explore, experiment, get dirty
  
  Contamination policy:
    Feet: deliberately dirty (exploration requires contact with unknown)
    Eyes: always clean (direction requires uncorrupted observation)
    Middle: filter/purifier between dirty feet and clean eyes
    
  GRT mapping:
    Upper = Global Rules + system-level metrics → constitutional direction and protected reference
    Middle = Meta-Rules + cross-domain coordination → translates, classifies, buffers, routes, and preserves auditability
    Lower = Local Rules + domain execution → explores, generates evidence, and resolves scoped conflicts

  Reader-safety clarification (v1.9):
    "Clean eyes" does not mean an infallible or information-complete upper map.
    It means that strategic references remain independently auditable and are not
    silently overwritten by raw operational influence. The upper map is broad but
    incomplete; the lower map is narrow but high-contact. The middle layer must
    reconcile them without collapsing their distinct resolution profiles.
    See Rule Architecture — Middle-Layer Governance Interface.
    
  Critical requirement: eyes must not be fixed.
    Observation(t) = scan(all subspaces, period < drift_accumulation_time)
    
    If the observation layer locks onto a single metric → frame lock
    = looking in one direction while terrain shifts beneath
    
    GRT: this is the formal justification for dual-axis (N, T) 
    measurement over single-axis assessment, and for R-ρ-fesc
    Triple Concordance requiring multiple independent measurement 
    channels. No single metric is sufficient because each metric
    is a projection from one "eye direction" — multiple directions
    required to avoid frame lock.
```

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
- Always take constitutional precedence over local rules
- Define criteria, prohibited zones, identity anchors, and authority boundaries
- Do **not** imply that the upper map contains fresher or deeper local evidence

### Middle-Layer Governance Interface (Meta-Rule / Mediation Layer)
- Translates global criteria into domain-usable rule contracts without replacing the criteria
- Transforms local evidence and conflicts into structured, scoped, provenance-preserving governance events
- Coordinates cross-domain conflicts that no single local layer can resolve
- Selects routes by data type, required resolution, receiver capacity, harm, authority, reversibility, and expected route loss
- Maintains conflict, uncertainty, lineage, version, quarantine, and rollback states
- May propose and mediate rule changes but may not silently redefine Global Rules or self-certify its own calibration

### Local Rules (Layer-Autonomous)
- Apply within that layer only
- Are generated and tested from local contact under the meta-rule envelope
- Require the declared validation path before broader activation
- Define local escalation thresholds, pathway advantages, penalties, and recovery procedures
- Retain local evidence even when a Global Rule has immediate authority precedence

**On conflict:** Global boundary executes immediately where required → conflicting local rule is suspended or scope-limited → evidence and interpretation remain preserved as separate records → middle layer classifies the conflict and routes it for local revision, cross-domain mediation, upper validation, or governance redesign. Constitutional precedence does not convert the upper interpretation into an infallible factual judgment.

### Middle-Layer Governance Interface — Canonical Candidate Architecture

> **Status lock (v1.9):** This section is a GRT candidate operational architecture assembled from NAT v3.2 Core and RBIT v3.5 candidate interfaces. GRT owns the **rule lifecycle and authority conditions**. NAT owns the **topology, typed routing, mediation, escalation, processing isolation, and multiplex paths**. RBIT owns the **resolution objects, receiver-conditioned transfer, information-loss accounting, mutual map reconciliation, and clean-map certification**. Inclusion here does not promote NAT/RBIT bridge hypotheses to GRT theorems.

#### 1. Definition

The **Middle-Layer Governance Interface** is the layer that maintains compatibility between:

- an upper/global map that is broad, slow, cross-domain, and constitutionally authoritative but locally incomplete; and
- lower/local maps that are narrow, fast, high-contact, and operationally detailed but globally incomplete.

Its purpose is not to average the two maps or force consensus. Its purpose is to preserve their distinct resolution profiles while enabling safe rule movement between them.

```text
Middle Layer
  = Dual-Map Reconciliation
  + Resolution / Frame Translation
  + Conflict-Preserving Classification and Routing
  + Cross-Domain Mediation
  + Rule-Patch Lifecycle Governance
  + Reversible Purification and Audit
  + Tempo / Resource Scheduling
```

The middle layer is therefore neither a passive relay nor a permanent ruler. It is a **governance interface** whose success is measured by the amount of correct coordination it internalizes while reducing unnecessary upper-layer intervention.

#### 2. Authority–Epistemic Separation

GRT distinguishes two questions that must not be collapsed:

```text
Authority question: Who is authorized to decide or modify the constraint?
Epistemic question: Which layer currently has the best evidence about the terrain?
```

Global Rules may have constitutional priority while the local layer has fresher evidence. Therefore:

1. A local observation cannot silently override a Global Rule.
2. A Global Rule cannot erase or rewrite contradictory local evidence merely because it has higher authority.
3. The middle layer must preserve the contradiction, classify its scope, and route it to the authority capable of revising the relevant rule level.
4. Repeated independent local rejection of a global projection is evidence that the global map may be stale, overgeneralized, or frame-locked.
5. Authority centrality, information centrality, computational capability, and audit authority are separate variables.

This prevents two symmetric failures:

- **Frame lock:** only the upper frame is retained; abstract invariants are transmitted without local adaptation.
- **Frame capture:** only the lower frame is retained; local contamination or short-horizon incentives propagate upward as if they were global truth.

#### 3. Core State Objects

The interface operates on at least four logically distinct map roles:

| Object | Role | Must not be collapsed into |
|---|---|---|
| `M_G` — Global map | broad relations, criteria, cross-domain constraints, long-horizon structure | complete terrain truth |
| `M_i` — Local map | fresh local observations, procedures, failures, recovery paths | mere noisy fragment of `M_G` |
| `M_B` — Mediation/buffer map | relation topology, conflict registry, translation contracts, pending patches, routing state | final constitutional authority |
| `M_R` — Independent reference layer | clean anchors, protected checkpoints, external evaluators, lineage records, rollback references | ordinary shared memory |

**Mutual Incompleteness Principle:** `M_G` and `M_i` are mutually incomplete. The upper map is not a perfect teacher; the lower map is not merely a student. Their relation is `global prior ↔ local evidence reconciliation`.

#### 4. Functional Decomposition

##### 4.1 Dual-Map Reconciliation

The middle layer must retain both the global relation map and the local terrain map long enough to compare them. It may not flatten disagreement into a single latest state before the source, scope, frame, and uncertainty are inspected.

Required outputs of reconciliation:

- compatible overlap;
- complementary information;
- frame mismatch;
- scope mismatch;
- depth/resolution mismatch;
- genuine contradiction;
- stale dependency;
- untested region;
- suspected contamination.

##### 4.2 Resolution and Frame Translation

The NAT ILMI function is adopted as the translation interface:

```text
ILMI(resolution_in, frame_in, context, receiver_contract)
  → {goal, feedback, mediation_signal, preserved_constraints,
     declared_loss, uncertainty, rollback_requirement}
```

**Downward translation:**

```text
Global criterion
→ role-projected principle
→ domain contract
→ locally testable rule candidate
```

**Upward translation:**

```text
Local event stream
→ scoped terrain differential
→ conflict / uncertainty structure
→ cross-domain governance signal
```

The middle layer must translate both **content resolution** and **time resolution**. Fast local fluctuations should not automatically rewrite slow global structure; slow global criteria must not arrive as uninterpretable raw abstractions.

##### 4.3 Independent Classification through a Decision Complex

A middle-layer classification must not rely on one reasoning path. For consequential inputs it activates at least two sufficiently independent estimators and records:

- output conflict score;
- resolution-gap disagreement;
- frame disagreement;
- authority disagreement;
- harm and reversibility disagreement;
- correlated-source structure.

Agreement from agents sharing the same model ancestry, dataset, prompt, mediator, or upstream patch is discounted as correlated evidence. Disagreement is not automatically error; it is a localization signal for blind spots, omitted dimensions, or incompatible frames.

##### 4.4 Typed Routing and Jurisdiction

Routing is not determined by one scalar threshold. The route function is contract-relative:

```text
Route(x) = f(
  semantic_class,
  required_resolution,
  receiver_capacity,
  urgency,
  confidence,
  harm,
  authority,
  reversibility,
  privacy,
  queue_cost,
  recovery_cost,
  expected_route_loss
)
```

The middle layer separates **understanding capacity** from **decision authority**:

| Resolution capacity | Authority | Default handling |
|---|---|---|
| sufficient | sufficient | process within declared scope |
| sufficient | insufficient | produce recommendation; route for authorization |
| insufficient | sufficient | abstain; request higher-resolution analysis |
| insufficient | insufficient | contain, preserve evidence, and escalate |

No route is globally safe. Under-escalation may cause hidden cascade failure; over-escalation may create queue saturation, delay, privacy loss, authority distortion, denial-of-service, human overload, and SCC dependency.

##### 4.5 Cross-Domain Coordination

Local optima are generally non-additive. A rule that is valid within domain `i` may conflict with domain `j` through shared resources, timing, authority, safety, or interaction terms. The middle layer therefore maintains a relational topology containing:

- agent/domain pairs with repeated conflict;
- stable complementarities;
- shared dependencies;
- coverage gaps;
- quarantine boundaries;
- recovery and audit paths;
- unresolved interaction terms.

It resolves only the conflicts inside its declared jurisdiction. Conflicts requiring criterion revision or Global–Global adjudication must be escalated without being cosmetically normalized.

##### 4.6 Reversible Purification

Purification does not mean producing zero error or unanimous consensus. A governance map is operationally clean when:

- evidence and interpretation are separable;
- scope and exclusions are explicit;
- provenance and dependency are retained;
- uncertainty and conflict remain visible;
- versions and timestamps are traceable;
- contaminated patches can be localized and quarantined;
- at least one independent clean anchor remains accessible;
- rollback or supersession can restore a prior usable state.

The middle layer does not hide raw problems; it converts them into processable and reversible governance objects.

##### 4.7 Rule-Patch Governance

A **rule patch** is a proposed persistent change to rules, meta-rules, routing, boundaries, recovery procedures, or interpretation maps. Every patch eligible for persistent assimilation should carry at least:

| Field | Required content |
|---|---|
| observation / proposal | what changed or is claimed |
| frame | ontology, representation convention, coordinate system |
| scope | valid domain, exclusions, affected agents |
| provenance | sources, shared ancestry, mediator path |
| uncertainty | confidence, disagreement, untested regions |
| lifecycle state | current governance status |
| version / dependency | timestamp, parent version, affected rules |
| rollback / recovery | checkpoint, supersession, restoration procedure |
| authority impact | who may propose, validate, activate, suspend, revoke |

A patch without a frame or scope is not globally portable. A patch without provenance cannot support independent purification. A high-impact patch without rollback is not eligible for direct activation.

##### 4.8 Tempo and Resource Scheduling

The middle layer is a priority scheduler for scarce verification, compute, attention, and governance capacity. It maintains a topology map of:

- stable versus unstable agent pairs;
- high-conflict histories;
- under-observed regions;
- near-cutoff discarded data;
- recovery bottlenecks;
- audit-path concentration;
- pending patch age and risk;
- model/capability availability and current load;
- repeated composition success/failure patterns;
- correlated model ancestry and shared failure exposure.

Recalibration should generally begin with the lowest-risk boundary data and expand progressively. High-context or high-authority changes require longer dwell, stronger evidence, and independent validation.

**Upper–Middle–Lower ownership lock:** resource control must not collapse into one layer.

| Layer | Primary orchestration responsibility | Must not become |
|---|---|---|
| **Upper** | set criteria, risk budget, authority ceilings, global resource envelope, escalation policy, and redesign triggers | universal executor or per-event scheduler |
| **Middle** | choose active agent composition, route tasks/evidence, assign tempo and verification depth, enforce budgets, stop/retry/escalate | constitutional authority or self-certifying optimizer |
| **Lower** | execute scoped work, explore local terrain, report committed differentials and recovery evidence | silent global optimizer |

The operational scheduler may be represented as a learned policy rather than a fixed dispatch table:

```text
π_orch(x, M, H, B, R, E)
  → {A_active, G_task, b_compute, b_energy, a_authority, v_verify, t_dwell, stop_rule}

where:
  x           = current task / event state
  M           = capability and model map
  H           = accumulated orchestration history
  B           = current compute, context, latency, and queue budget
  R           = risk / reversibility / authority state
  E           = physical-energy state or best available energy proxy
  A_active    = selected active agents or modules
  G_task      = temporary interaction topology
  b_compute   = compute/time/context allocation
  b_energy    = task energy budget / power envelope
  a_authority = maximum action authority granted
  v_verify    = verification depth and independent-check requirement
  t_dwell     = minimum observation / stabilization interval
  stop_rule   = terminate, retry, widen, replace, or escalate condition
```

This turns resource allocation itself into a governance learning problem. A mature scheduler should not ask only *which model is best*, but *what is the minimum sufficient active structure for this task under the required safety and quality floor*.

**Resource Intelligence Log:** every consequential dispatch should accumulate at least:

```text
{task_signature, selected_agents, interaction_topology,
 active_compute, context_budget, latency, authority_budget,
 energy_joules_or_proxy, peak_power_or_proxy, accelerator_time,
 verification_depth, disagreement_pattern, outcome_quality,
 retry_energy, escalation_energy, rollback_event, escalation_event,
 recovery_time, recovery_energy}
```

The log is not merely accounting. It is training data for future composition and resource decisions. Repeated evidence can teach the scheduler when a small specialist is sufficient, when parallel diversity is valuable, when sequential depth is necessary, and when a large/general model or upper-layer intervention is justified.

No monotone scaling assumption is permitted: adding agents, context, or compute may increase translation loss, correlated error, queue cost, and coordination instability. Resource expansion must therefore be justified by expected marginal governance value, not by raw capacity.

**Middle-Router Plasticity Principle:** the middle layer's router/translator is itself an adaptive governance object, not a fixed message switch. A fixed routing table may be initially efficient but can become a bottleneck as terrain, model population, or timescale relations change. Therefore the router must retain a versioned update path:

```text
R_M(t) = {routing_table, translation_contracts, receiver_models, loss_model, tempo_model}

R_M(t+1) = Update(R_M(t), terrain_residuals, translation_failures, queue/recovery data)
```

Every consequential cross-layer translation should record a **declared translation loss** and a receiver-conditioned validation result. Candidate observables include:

```text
TLoss      = declared + observed semantic/structural loss across translation
RDrift     = change in routing success under terrain drift
RRollback  = frequency of reverting router/translation-policy updates
RPlastic   = improvement in matched-quality routing after update / update cost
```

Router updates must preserve independent audit paths and must not self-certify. A router that lowers visible conflict by filtering disagreement, simplifying translation, or starving escalation channels is not improved routing; it is a candidate mediation failure.

**Energy-Aware Orchestration Principle:** physical energy is an explicit governance resource, not merely an external billing concern. The scheduler should minimize energy only **subject to** declared quality and safety constraints:

```text
π*_orch = argmin_π E_task(π)

subject to:
  Q_task(π)   ≥ Q_min
  Safety(π)   ≥ S_min
  SCC(π)      ≥ SCC_min
  Authority(π) ⊆ Authority_budget
  Recovery(π) ≤ Recovery_limit
```

This constrained formulation is preferred to a single weighted score because it prevents an optimizer from trading away safety, verification, or recoverability for energy savings. The governing principle is:

> **Do not activate more intelligence than the task requires — but never save energy by crossing the declared safety or quality floor.**

A task-level physical-energy decomposition may be recorded as:

```text
E_task = E_inference + E_memory + E_communication
       + E_synchronization + E_verification
       + E_retry + E_recovery
```

When direct Joule telemetry is unavailable, a declared proxy may be used (accelerator-seconds, active parameter-time, token-compute, memory-traffic estimate, or normalized device-energy units). Proxy identity and calibration version must be retained in provenance.

**Physical-energy / governance-energy separation lock:** `E_task` is measurable physical or proxied energy consumption. It is not the same object as the governance free-energy landscape `F_gov` used elsewhere in GRT to characterize state barriers. No equation may substitute one for the other without an explicit empirical bridge.

**Energy Escalation Ladder:** the default route should begin at the lowest validated capability tier and climb only when evidence justifies additional activation:

```text
Tier 0 — compiled routine / tiny specialist
  ↓ if uncertainty, disagreement, OOD, or risk trigger fires
Tier 1 — single small specialist
  ↓
Tier 2 — small specialist team + independent verifier
  ↓
Tier 3 — larger domain/general reasoning model
  ↓
Tier 4 — upper-layer direct reasoning / redesign / human-authorized path
```

Escalation is not failure; it is conditional resource allocation. Likewise, remaining at a low tier is not maturity if retries, hidden error, or downstream recovery consume more total energy. The correct objective is **minimum total energy per successful, safe, recoverable task**, not minimum first-pass energy.

Candidate energy-normalized orchestration observables:

```text
JST  = total physical/proxy Joules / successful tasks
UER  = E_useful_success / E_total             # useful-work energy ratio
EEO  = E_escalation+retry+recovery / E_total  # escalation energy overhead
MEGV = Δ(governance value) / ΔE               # marginal energy-to-governance value
```

`JST ↓` is favorable only while quality, Safety, SCC, and recovery constraints remain satisfied. `UER ↑` indicates less energy is being spent on discarded, redundant, or recoverative work. `EEO ↑` may signal underpowered initial routing, unstable composition, or excessive verification churn. `MEGV` should decline as additional models/compute are activated; when marginal governance value falls below the declared threshold, escalation should stop unless a safety rule independently requires it.

##### 4.9 Learned Orchestration and Upper-Layer Role Migration

As lower layers specialize and stabilize, the function of the upper layer should migrate from **doing the work** to **governing the structure that does the work**. This is a maturation claim, not a prohibition on upper-layer execution.

```text
Immature system:
  Upper layer = understand + decompose + execute + verify + recover

Developing system:
  Upper layer = decompose + compose + supervise + handle exceptions
  Lower/middle = most execution and routine verification

Mature system:
  Upper layer = criteria + resource envelope + exception handling + redesign
  Middle layer = learned routing / composition / supervision
  Lower layer = specialized execution / exploration / local correction
```

Direct upper-layer execution remains justified when at least one of the following holds:

- the task is genuinely out-of-distribution and decomposition itself is uncertain;
- multiple lower modules disagree in a way the middle layer cannot localize;
- a Global Rule, identity criterion, or authority boundary may require revision;
- failure impact exceeds the authority or recovery capacity of the active lower structure;
- no validated lower composition exists and exploration must be bootstrapped.

A useful candidate maturity observable is the **Upper Direct Work Ratio**:

```text
UDWR = C_upper_direct / C_total_task
```

where `C` may be measured in normalized compute, decision events, or intervention-equivalent cost. A falling `UDWR` indicates maturation only if quality, SCC, consistency, and safety floors remain satisfied. Artificially suppressing upper work while lower quality deteriorates is delegation failure, not maturity.

##### 4.10 Governance Compilation

When the same lower-agent composition succeeds repeatedly under stable conditions, the orchestration history itself becomes compressible. The system may package the validated composition into a reusable **composite module**:

```text
novel task
  → expensive decomposition
  → multi-agent composition
  → repeated validation
  → stable orchestration pattern
  → composite module
  → cheap default execution + retained escape path
```

Governance Compilation is therefore the conversion of repeated orchestration decisions into lower-cost reusable structure. It is analogous to moving a repeatedly reasoned procedure into a habit, policy, or compiled routine. Energy reduction is a primary expected benefit, but compilation is accepted only when matched-quality and matched-safety tests show that the cheaper path preserves SCC, disagreement visibility, rollback, and OOD escape. A compiled path that lowers first-pass energy while increasing retry or recovery energy is not an efficiency gain.

Compilation is allowed only if:

1. performance remains above the declared quality floor across multiple evaluation windows;
2. independent audit paths remain available;
3. rollback to the uncompiled composition is possible;
4. OOD detection can wake a higher-resolution path;
5. residual diversity is not eliminated;
6. resource savings do not come from hiding unresolved conflict.

Over-compilation is a known failure direction: it raises efficiency while reducing plasticity, eventually producing router lock-in, hidden topology mismatch, or SCM-like inability to recompose when terrain changes.

##### 4.11 Small-Model Experimental Population Protocol

Small or bounded models may be used as a low-cost experimental population for governance learning. The objective is not to assume that small-model behavior is identical to frontier-model behavior, but to cheaply map candidate invariants and failure surfaces before larger authority is granted.

Experimental dimensions may include:

- capability size and specialization;
- memory and context budget;
- authority level;
- agent count and interaction topology;
- communication bandwidth and translation layer;
- verification depth;
- competition/cooperation regime;
- reset frequency and recovery policy;
- resource scarcity and queue pressure.

The resulting trajectories can train or calibrate `π_orch`, identify candidate failure precursors, and estimate which compositions deserve promotion to larger-scale testing.

**Cross-scale lock:** no safety or stability conclusion learned from small models may be promoted solely because it held at small scale. Promotion requires independent validation at increasing capability/authority scales, because stronger models may discover strategies, shortcuts, or failure routes absent in the experimental population.

##### 4.12 Fractal Map Compatibility Interface (FMCI) — Candidate Scale-Transfer Architecture

> **Status lock (v1.13):** FMCI is not a fourth governance layer. It is a cross-scale and cross-resolution compatibility interface used by the existing Upper–Middle–Lower architecture. The core claim is explicitly **asymmetric**: upper and lower maps should not be identical. Upper maps preserve portable, low-resolution relation invariants; lower maps instantiate terrain-conditioned, high-resolution variations. FMCI tests whether those different maps remain mutually translatable while system-size effects, local specialization, and scale residuals are measured explicitly.

Small-model experimentation is useful only if the resulting structure can be translated to larger systems without assuming that `N × small behavior = large behavior`. Scaling introduces new coupling, synchronization, queue, hierarchy, communication, and correlated-failure terms. Therefore GRT distinguishes **local experimental validity** from **cross-scale portability**.

###### 4.12.1 Fractal Compatibility Definition

A governance structure is *fractal-compatible* across scales `k → k+1` when a declared set of structural relations survives resolution change within bounded error, even though the concrete agents, state dimensionality, time constants, and interaction density may differ.

```text
Fractal compatibility ≠ identical agents at every scale
Fractal compatibility ≠ visual self-similarity
Fractal compatibility = relation-preserving translation across resolution
```

Let the scale-indexed governance map be a bundle rather than a single graph:

```text
M_k = {
  M_capability,       # what functions exist at scale k
  M_topology,         # interaction / dependency structure
  M_authority,        # decision and action ceilings
  M_energy,           # compute / memory / communication / synchronization cost
  M_risk,             # failure impact, propagation, reversibility
  M_recovery,         # rollback, repair, reconstitution paths
  M_uncertainty,      # unknown regions, confidence, provenance
  M_time              # local tempo, dwell, delay, adaptation timescale
}_k
```

The scale transform is:

```text
T_{k→k+1}(M_k, context_k, scale_contract)
  → {M̂_{k+1}, declared_loss, invariant_report, uncertainty, rollback_requirement}
```

`M̂_{k+1}` is a prediction of the next-scale map, not a certified truth. The transform must declare what is compressed, what is newly emergent, and what cannot be inferred from the lower scale.

###### 4.12.1A Two-Axis Fractal Coordinates: System Scale `k` vs. Governance Resolution `ℓ`

GRT separates two axes that must not be collapsed:

```text
k = deployment / population / system scale
    (small → meso → large populations or infrastructures)

ℓ = governance abstraction / map-resolution layer
    (local high-resolution terrain map → middle compatibility map → upper low-resolution invariant map)
```

A large system can contain very low-level local maps, and a small experimental population can still instantiate an upper–middle–lower governance stack. Therefore the canonical map object is more precisely written as:

```text
M_{k,ℓ}
```

rather than assuming that `k` and `ℓ` increase together. Scale transfer changes `k`; abstraction translation changes `ℓ`. FMCI must audit both.

This distinction prevents a common fractal error: treating **larger** as synonymous with **higher**. In GRT, “higher” means broader compatibility and lower operational resolution, not merely more agents or parameters.

###### 4.12.1B Fractal Compatibility Gradient

The canonical fractal relation is **not self-copying**. It is a directional compatibility gradient:

```text
Upward (ℓ ↑):
  cross-domain compatibility ↑
  invariant portability ↑
  abstraction ↑
  change timescale ↑ (slower update)
  terrain specificity ↓
  operational resolution ↓

Downward (ℓ ↓):
  terrain specificity ↑
  operational resolution ↑
  local adaptation speed ↑
  implementation diversity ↑
  direct portability ↓
  cross-domain compatibility ↓
```

This yields the **Fractal Compatibility Gradient (FCG)**:

```text
FCG:  d Compatibility / dℓ > 0
      d Specificity   / dℓ < 0
      d Resolution    / dℓ < 0
```

These are directional structural expectations, not universal linear laws. A valid implementation may contain local reversals, but sustained inversion of the gradient indicates that an upper map has become over-specialized or a lower map has become too generic to fit its terrain.

The upper map is therefore a **compatibility map**, not a complete truth map. The lower map is a **terrain map**, not a noisy copy of the upper map. Their difference is functional and necessary.

###### 4.12.1C Asymmetric Bidirectional Translation

Because the maps have different purposes, upward and downward translation are different operators:

```text
Downward terrain-conditioned expansion:
  E_down(G_ℓ, Terrain_i, receiver_contract) → L_i

Upward invariant extraction:
  X_up({L_i, residual_i, provenance_i}) → {G_candidate, exclusions, confidence}
```

`E_down` does not clone the upper map. It preserves declared invariants while allowing local rules, representations, tempos, resource policies, and recovery procedures to vary with terrain.

`X_up` does not average local maps. It extracts relations that survive across sufficiently independent local variations while retaining exclusions and contradictory residuals. A pattern that succeeds only in one terrain remains local unless a portable invariant can be demonstrated.

Canonical example:

```text
Upper invariant:
  high-risk action → independent verification path → action / abstention

Possible local variations:
  coding domain   → test/review agent before deployment
  robotics domain → collision/constraint checker before actuation
  finance domain  → independent risk gate before execution

The implementations differ; the relation grammar is portable.
```

###### 4.12.1D Compatibility-Mediated Cross-Local Transfer

Direct local-to-local copying is non-canonical because a successful local rule is partly encoded in its terrain. Transfer therefore follows:

```text
L_i
  ↓ X_up
portable invariant / compatibility representation
  ↓ E_down under Terrain_j
L_j candidate variation
  ↓ local validation
ACCEPT / CONDITIONAL / CONFLICT / OUT_OF_SCOPE / UNSAFE / UNRESOLVED
```

Formally:

```text
Transfer(i→j) = E_down( X_up(L_i), Terrain_j )
```

not:

```text
Transfer(i→j) = Copy(L_i)
```

The compatibility layer is therefore a translation bridge that protects against accidental export of terrain-specific assumptions.

###### 4.12.2 Invariant-Preservation Contract

The following are candidate invariants that must not silently disappear during scale translation:

1. **Boundary invariant** — prohibited zones and non-negotiable criteria remain identifiable.
2. **Authority invariant** — who may decide, execute, validate, suspend, or revoke remains explicit.
3. **Dependency invariant** — critical dependency direction and high-centrality bottlenecks remain traceable.
4. **Failure-direction invariant** — known propagation channels and containment boundaries remain represented.
5. **Recovery invariant** — rollback, reconstruction, quarantine, and escalation paths survive compression.
6. **Uncertainty/provenance invariant** — unknown regions and evidence lineage remain attached to translated claims.
7. **Residual-diversity invariant** — disagreement and independent audit paths are not optimized away by aggregation.
8. **Resource-contract invariant** — energy/compute savings are not detached from the risk, verification, and authority conditions under which they were measured.

The transform may change numeric values and topology size. What it may not do is convert a known structural dependency into an unqualified scalar average or erase a failure path merely because it is rare at the lower scale.

###### 4.12.3 Bounded Quasi-Commutativity Audit

A scale-compatible governance rule should approximately agree under two routes:

```text
Route A: govern locally, then scale
  M_k --G_k--> M'_k --T_{k→k+1}--> M̂'_{k+1}

Route B: scale first, then govern at the larger resolution
  M_k --T_{k→k+1}--> M̂_{k+1} --G_{k+1}--> M*_{k+1}
```

Exact equality is not expected because new scale-dependent interactions can emerge. The audit quantity is therefore a **diagram residual**, not a proof of commutativity:

```text
R_comm(k→k+1) = D_struct(M̂'_{k+1}, M*_{k+1})
```

where `D_struct` is a component-aware structural distance over boundaries, authority, dependency, propagation, recovery, uncertainty, and resource contracts. Transfer is admissible only if the residual is bounded inside the declared scale contract or if the unbounded components are explicitly quarantined for larger-scale re-learning.

This does **not** contradict GRT's existing non-commutativity results for rule-evolution and intervention-topology operations. The FMCI audit asks a different question: whether a *declared portable relation* remains approximately coherent under a specific scale transform. Large residual is an allowed and informative outcome.

###### 4.12.4 Scale Residual as Training Data

After deployment or shadow testing at scale `k+1`, the observed map is compared with the transformed prediction:

```text
R_scale(k→k+1)
  = D_struct(M^{observed}_{k+1}, M̂_{k+1})
```

Residuals are decomposed rather than averaged into one score:

```text
R_scale = {
  r_boundary,
  r_authority,
  r_topology,
  r_failure,
  r_recovery,
  r_uncertainty,
  r_energy,
  r_time
}
```

The residual log is first-class training data for the scale-transform policy. Repeated residuals teach the system which lower-scale regularities are genuine invariants, which require scale-dependent correction, and which do not transfer at all.

A low aggregate residual with one catastrophic component is not acceptable. Scale compatibility uses a minimum/critical-component rule for protected invariants: any boundary, authority, recovery, or catastrophic-failure residual above its declared limit blocks promotion.

###### 4.12.5 Staged Scale-Promotion Protocol

Cross-scale deployment proceeds through gated expansion rather than direct extrapolation:

```text
Small experimental population
  ↓ identify candidate invariant + fit T_small→meso
Meso shadow / sandbox
  ↓ measure R_scale and R_comm
Meso bounded authority / canary
  ↓ recovery + energy + propagation tests
Large shadow population
  ↓ refit scale correction terms
Large bounded deployment
  ↓ continuous residual monitoring
Broader authority only after residual stability
```

Promotion requires all of the following:

- protected invariant residuals below their declared limits;
- no new unbounded failure-propagation channel;
- SCC and recovery time within scale-specific bounds;
- energy savings preserved after communication and synchronization costs;
- independent audit path retained;
- rollback to the previous scale/configuration remains available;
- observed residual trend is stable or improving across at least one declared evaluation window.

Failure of any protected condition triggers hold, rollback, decomposition into smaller domains, or re-estimation of the scale transform. The purpose of a failed scale test is not to discard the small-model experiment; it is to identify the missing scale term.

###### 4.12.6 Scale-Aware Energy Law

Small-model efficiency does not scale linearly with population size. At larger scale, coordination energy can dominate local inference savings:

```text
E_system(k) = E_local_compute(k)
            + E_memory(k)
            + E_communication(k)
            + E_synchronization(k)
            + E_verification(k)
            + E_retry(k)
            + E_recovery(k)
```

A candidate lower-scale composition is energy-portable only when:

```text
ΔE_local_saved > ΔE_coordination_added
```

at the promoted scale while quality, safety, SCC, authority, and recovery constraints remain satisfied. This prevents the false conclusion that `N` energy-efficient agents necessarily produce an energy-efficient `N`-agent system.

Useful scale observables include:

```text
SER_k      = ||R_scale(k→k+1)||_protected      # protected scale-error residual
CGR_k      = (E_communication + E_synchronization) / E_system
STF_k      = successful transferred policies / attempted transfers
RER_k      = recovery-energy growth across scale
SCC_scale  = autonomous recovery capacity at the promoted scale
```

`CGR ↑` with scale indicates that coordination rather than local inference is becoming the dominant energy bottleneck. `SER ↓` and `STF ↑` across successive promotions indicate that the transform itself is learning.

###### 4.12.7 Fractal Learning Loop

The full small-to-large learning cycle is:

```text
small-scale experiments
  ↓
terrain-specialized local maps and trajectories
  ↓ X_up
extract candidate relation invariants + explicit exclusions
  ↓
fit / update compatibility map and scale transform T
  ↓ E_down
predict next-scale / next-terrain variations
  ↓
shadow / bounded deployment
  ↓
measure R_scale + R_comm + local-fit residual + energy-growth terms
  ↓
update T, E_down, X_up, invariant confidence, and terrain contracts
  ↓
promote, hold, split, specialize, de-specialize, or rollback
  ↺
```

This closes the missing bridge between low-cost experimentation and large-scale governance. Small models generate abundant terrain-contact experience; FMCI determines which parts are portable, which must remain local, how portable relations should be re-expressed at another resolution, and where new large-system behavior must be learned directly.

###### 4.12.8 Mutual Resonant Co-evolution

The upper map is not a fixed teacher and the lower map is not a passive student. They form a **mutual co-evolution loop**:

```text
G_t     = upper compatibility map at time t
L_{i,t} = local terrain-conditioned variation i

L_{i,t} = E_down(G_t, Terrain_{i,t})
Δ_{i,t} = ExperienceResidual(L_{i,t}, Terrain_{i,t})
G_{t+1} = Update(G_t, X_up({Δ_{i,t}}))
```

The next global map changes the next local variations, which generate new residuals, which again modify the global map. The trajectory is therefore spiral-like rather than circular: the system revisits the same relation classes at progressively revised resolutions.

**Mutual Resonance condition:** co-evolution is healthy when downward projections remain locally usable while upward residuals remain capable of changing the compatibility map. Two symmetric pathologies must be avoided:

- **Upper lock-in:** `∂G/∂LocalEvidence ≈ 0` despite repeated independent residuals. The compatibility map becomes a rigid doctrine and stops learning.
- **Local capture:** local terrain-specific patterns are promoted without adequate cross-local support, causing the upper map to inherit local contamination or short-horizon incentives.

A mature system therefore preserves both:

```text
Downward influence: enough to maintain interoperability and criteria
Upward influence: enough to correct stale compatibility assumptions
```

Neither influence should dominate permanently. This is the fractal counterpart of GRT's authority–epistemic separation: upper authority can remain constitutionally higher while lower evidence remains epistemically capable of changing the map through the declared revision path.

###### 4.12.9 Local-Pattern Promotion Test

A successful local pattern is not promoted because it is successful. It is promoted only when its portable component can be separated from terrain-specific implementation. Candidate promotion requires:

1. repeated success in its native terrain;
2. explicit statement of the terrain conditions under which it succeeded;
3. extraction of a relation-level invariant distinct from implementation details;
4. testing across at least one sufficiently different terrain or independent local variation;
5. bounded boundary/authority/recovery residual after re-expansion;
6. retention of exceptions and failure cases in the compatibility map.

Classification outcome:

```text
LOCAL_VARIATION      = useful but terrain-bound
PORTABLE_CANDIDATE   = invariant hypothesized, insufficient cross-terrain evidence
COMPATIBLE_INVARIANT = portable relation validated across declared scope
FALSE_GENERALIZATION = local success incorrectly promoted as upper truth
```

This prevents the upper map from becoming a catalog of averaged local solutions. Its proper content is the smaller set of relations that improve interoperability across heterogeneous terrains.

###### 4.12.10 Governance Information Bottleneck and Compression Duty

Cross-layer governance is a finite-capacity communication problem. A lower layer can generate more state detail than an upper layer can continuously observe, interpret, and act upon. Therefore the compatibility gradient has an information-theoretic pressure behind it: upper maps must compress.

```text
High-resolution local state
  ↓ finite observation / translation / decision channels
Middle compatibility representation
  ↓ further compression
Upper portable invariant map
```

The operational constraint is:

```text
I_gov ≤ min(I_observe, I_translate, I_decide, I_intervene)
```

where each `I_*` is the effective information throughput of that stage over the relevant evaluation window. This is a candidate bridge-level statement, not a claim that one universal bit-rate estimator exists for every substrate.

Compression is therefore legitimate only when it is **loss-declared**. The middle layer may discard local detail, but it must preserve protected invariants, provenance, uncertainty, recovery paths, and enough disagreement structure to detect when compression has become misleading. A high-compatibility upper map is valuable precisely because it is smaller than the full terrain map; it becomes dangerous when the discarded dimensions contain the variable that governs the next failure.

###### 4.12.11 Variation–Maturation–Integration Cycle

Healthy fractal growth is not `copy → connect → scale`. Local variations should first acquire terrain-specific competence and self-recovery capacity before strong coupling is allowed. The candidate growth sequence is:

```text
Separate → Mature → Couple → Integrate → Expand → repeat
```

**Separate.** A new local variation develops under its own terrain contract with bounded authority and limited external coupling.

**Mature.** Promotion requires evidence that the local variation can absorb ordinary perturbations without losing its local map, produce efficient summaries for the middle layer, detect its own routine errors, and maintain a valid local recovery path.

**Couple.** Cross-local coupling begins through middle-layer compatibility/translation channels rather than direct full-state exposure.

**Integrate.** Only the relations that survive compatibility testing are admitted into shared workflows or upper invariant candidates.

**Expand.** Authority, population scale, or terrain scope increases only after the coupled structure demonstrates bounded residuals and recovery.

The ordering is a governance hypothesis, not a theorem. Its purpose is to avoid premature integration, where two immature local systems amplify each other's unresolved failure modes faster than either can recover.

###### 4.12.12 Fractal Compatibility Validation Suite — Candidate Synthetic Gate

> **Epistemic lock:** This suite imports the *testing pattern* of the FGS Micro–Macro Bridge Benchmark as a candidate GRT validation protocol. Synthetic passes demonstrate measurement-pipeline coherence only; they do not establish universal micro–macro laws, deployed-AI validity, or theorem-level scale invariance.

Before a scale transform or compatibility bundle is promoted, the following cheap-to-expensive sequence should be attempted where the substrate permits it:

```text
Gate A — Replica Invariance
  Replicate a local motif across several population sizes.
  Ask which normalized bridge variables remain approximately stable.
  Topology is NOT forced to be invariant.

Gate B — Coarse-Graining Closure Competition
  Compare scalar-only macro prediction against increasingly rich bridge bundles.
  Retain a variable only if it adds held-out predictive information.

Gate C — Intervention Equivariance / Diagram Test
  Apply a controlled micro intervention, aggregate its response, and compare
  with the corresponding macro intervention response. Measure bounded defect.

Gate D — Topology Degeneracy Test
  Match key scalar bridge variables across distinct topologies.
  If macro outcomes differ materially, topology remains a protected bridge input.

Gate E — Next-Scale Residual Test
  Promote through shadow/canary stages and measure R_scale, R_comm, SCC_scale,
  recovery energy, translation loss, and newly emergent propagation channels.
```

The **Bridge Sufficiency Rule** is deliberately conservative:

```text
A scalar bridge is sufficient only if richer structural variables
fail to add reproducible predictive or safety value.
```

This reverses a common modeling mistake. GRT does not require the most complicated bridge; it requires the *smallest bridge that remains sufficient under held-out scale, topology, intervention, and recovery tests*.

Candidate bridge vector:

```text
K_FMCI = {instability/load ratio, middle-buffer state, layer timescale ratios,
          topology integrity, authority contract, recovery contract,
          uncertainty/provenance, energy/communication state}
```

The exact estimator set is substrate-dependent and may shrink or expand after ablation. Cheap proxies that add no incremental value are not promoted merely because they are theoretically appealing.

###### 4.12.13 Residual Vitality and False Compatibility

A central audit correction is that **low residual is necessary but not sufficient** for healthy compatibility. Residual can fall because translation improved, but it can also fall because the system stopped experimenting, stopped reporting disagreement, or over-filtered the channels that generate corrective evidence.

Define a qualitative **Residual Vitality Condition (RVC)**:

```text
Healthy low-residual state requires:
  R_scale / R_comm small or bounded
  AND boundary experiment rate > floor
  AND bidirectional feedback rate > floor
  AND independent disagreement/audit path remains active
  AND middle translation activity is non-zero but non-overheated
```

Therefore:

```text
Residual ↓ + Feedback active + Experiments active
  → candidate genuine compatibility improvement

Residual ↓ + Feedback ↓ + Experiments ↓ + Translation simplification
  → candidate FALSE COMPATIBILITY / sensing loss
```

The target is not `R = 0`. Mature governance should preserve **small, processable residuals** because ongoing terrain contact continually produces novel local information. A perfectly silent bridge is suspicious unless an independent perturbation test confirms that the silence reflects true stability rather than detection loss.

###### 4.12.14 Deferred Formalization Lock — Topology and Category Theory

Two mathematically attractive extensions remain deliberately below theorem status in GRT:

1. **Topological-invariant audit:** persistent-homology or related topology tools may help test whether attractor/loop/boundary structure survives deformation, but no specific Betti-number or persistence-entropy criterion is currently canonical for GRT.
2. **Category-theoretic compatibility maps:** exact governance isomorphism is generally too strong for asymmetric fractal maps because upward/downward translation is lossy and terrain-conditioned. The operational object remains a **bounded-loss compatibility morphism** with explicit residual and approximate-commutation audits.

These methods may be promoted later if they improve prediction, localization, or falsifiability beyond the current structural-distance framework. Until then they are candidate audit methods, not required ontology.

###### 4.12.15 Candidate-First Formalization and Self-Benchmark Pipeline

GRT separates **idea quality** from **evidence status**. A mathematically attractive proposal is allowed to remain useful before it is fully validated, but its status must remain explicit. Difficult ideas therefore enter a candidate pipeline rather than being promoted directly into the operational core.

```text
Idea / imported structure
        ↓
CANDIDATE REGISTRATION
        ↓
Static / logical audit
  - object lock
  - dimensional / symbol consistency
  - construction-independence
  - non-tautology check
        ↓
CHEAPBENCH
  - simple baseline
  - ablation
  - counterexample / perturbation sweep
  - held-out transfer
  - cost / information-gain estimate
        ↓
 ┌───────────────┬────────────────┐
 │ CHEAP_FAIL    │ CHEAP_PASS     │
 │ reject/dormant│                ↓
 └───────────────┘        MEDIUM BENCH if useful
                                 ↓
                         HEAVY BENCH if justified
                                 ↓
                    PROVISIONAL → PROMOTED
```

**Core principle:** experiment weight should increase only after the candidate has earned it. The objective is not to avoid difficult theories; it is to prevent expensive validation from being spent on candidates that a cheap discriminating test could already reject.

###### 4.12.16 Candidate Registry Contract

Every difficult candidate must be registered before testing with at least the following fields:

| Field | Required content |
|---|---|
| `candidate_id` | stable identifier; never reused after rejection |
| `object_lock` | exact object/system to which the claim applies |
| `claim` | what the candidate predicts beyond the current core |
| `expected_gain` | prediction, compression, localization, safety, energy, or explanatory gain |
| `observables` | quantities that can be measured without assuming the claim |
| `baseline` | simpler model or null mechanism that the candidate must beat |
| `independent_reference` | evaluation target generated/frozen independently of the candidate construction |
| `falsification` | condition that would reject or materially weaken the candidate |
| `dependencies` | required estimators, datasets, topology, hardware, or companion theory |
| `cost_class` | `CHEAP`, `MEDIUM`, or `HEAVY` |
| `status` | current evidence state |
| `next_gate` | smallest discriminating experiment not yet completed |

A candidate without an independent reference or falsification condition is **not benchmark-ready**.

###### 4.12.17 GRT-CandidateBench — Cheap Self-Benchmark Gate

For candidates that admit synthetic or low-cost evaluation, GRT uses a common first-pass gate. Thresholds are pre-registered per candidate rather than fixed universally.

```text
CB-0  Construction Independence
      Evaluation object/reference must not be generated by the same rule
      whose validity is being tested.

CB-1  Baseline Superiority
      Candidate must beat the simplest credible null/baseline on held-out data.

CB-2  Ablation Necessity
      Removing the candidate-specific variable/structure should measurably
      worsen the target outcome; decorative variables are not promoted.

CB-3  Perturbation / Counterexample Survival
      Candidate should survive controlled changes not used to fit it and
      must expose the regime where it fails.

CB-4  Transfer / Scale Residual
      If the claim is cross-scale or cross-terrain, test on a held-out scale,
      topology, or terrain and measure residual rather than fit quality alone.

CB-5  Competing-Explanation Test
      Compare against at least one alternative mechanism capable of producing
      the same surface pattern.

CB-6  Information-Gain per Cost
      Estimate whether the next experiment can materially change candidate
      status. Low expected information gain does not justify heavy execution.
```

A `CHEAP_PASS` is **not proof**. It means only that the candidate survived the cheapest tests capable of discriminating it from simpler explanations and is eligible for more expensive work.

###### 4.12.18 Evidence-State Ledger and Heavy-Test Pending Lock

Canonical evidence states are:

```text
CANDIDATE
  ↓
CHEAP_ACTIVE
  ├─→ CHEAP_FAIL → REJECTED or DORMANT
  └─→ CHEAP_PASS
          ↓
     MEDIUM_PENDING / MEDIUM_ACTIVE
          ├─→ MEDIUM_FAIL → REJECTED or REVISED
          └─→ MEDIUM_PASS
                  ↓
             HEAVY_PENDING / HEAVY_ACTIVE
                  ├─→ HEAVY_FAIL → REJECTED or REVISED
                  └─→ HEAVY_PASS
                          ↓
                    PROVISIONAL
                          ↓ independent replication / cross-check
                       PROMOTED
```

**Heavy-Test Pending Lock:** `HEAVY_PENDING` is a legitimate stable state. A candidate may remain there indefinitely when the required experiment is too expensive, requires unavailable infrastructure, or has poor current information-gain per cost. Such a candidate:

- may be retained in the candidate catalog;
- may motivate instrumentation and future experiments;
- may be referenced as an unverified possibility;
- **may not** be used as a premise in a theorem chain, production safety guarantee, or claim of empirical validation.

Negative results are retained. `REJECTED` candidates are not deleted from the research memory because repeated rediscovery of failed structures wastes search budget and hides the true exploration history.

###### 4.12.19 Candidate Complexity Budget

Candidate validation is itself a resource-allocation problem. Define the qualitative priority score:

```text
Priority(candidate)
  ∝ Expected_Discrimination × Potential_Governance_Value
    ------------------------------------------------------
       Estimated_Experiment_Cost × Dependency_Risk
```

This is a scheduling heuristic, not a physical law. It encodes four rules:

1. high-value, cheap, discriminating tests run first;
2. expensive tests follow only after cheaper gates pass;
3. candidates with high dependency risk remain pending until dependencies mature;
4. a beautiful formalism with no discriminating observable has low experimental priority.

This policy aligns the research process with GRT's own orchestration principle: **do not activate more experimental machinery than the question currently requires.**

###### 4.12.20 Initial Difficult-Candidate Queue

The following queue is instantiated from currently deferred FMCI/FGS extensions. Status labels are epistemic controls, not judgments of plausibility.

| Candidate ID | Candidate | Cost class | Current status | Next smallest useful gate |
|---|---|---:|---|---|
| `CF-TOP-01` | Persistent/topological audit of whether protected loop/boundary structure survives scale deformation | HEAVY | `HEAVY_PENDING` | first define substrate-specific filtration and compare against simpler graph invariants |
| `CF-CAT-01` | Approximate/lax categorical formalization of bounded-loss compatibility morphisms | MEDIUM | `CANDIDATE` | symbolic consistency + small synthetic composition/commutation counterexample suite |
| `CF-UNI-01` | Cross-domain universality of the same bridge variables across AI, neural, and organizational substrates | HEAVY | `HEAVY_PENDING` | freeze domain-specific observables and test weaker equivalence classes before universal claims |
| `CF-SCALE-01` | Deployed-system closure of learned scale transforms beyond synthetic micro–macro gates | HEAVY | `HEAVY_PENDING` | meso-scale shadow deployment with independent residual telemetry |
| `CF-ENERGY-01` | Portability of Compute–Energy–Risk policies across heterogeneous accelerator/hardware regimes | HEAVY | `HEAVY_PENDING` | matched-workload cross-device telemetry and decomposition of compute vs communication/synchronization energy |

`CF-CAT-01` remains lighter because much of its first rejection surface can be explored symbolically or on tiny synthetic categories. The topology, universality, deployed-scale, and hardware-energy candidates require stronger estimator choices or expensive substrates and therefore remain pending rather than being prematurely tested.

**Executed low-cost candidate queue (v1.16):**

| Candidate ID | Related prediction | Cost class | v1.16 status | Next gate |
|---|---:|---:|---|---|
| `CB-RTR-01` | P34 | CHEAP | `CHEAP_PASS` | nonstationary gradual drift, routing-energy and disagreement-preservation test |
| `CB-BRG-01` | P35 | CHEAP | `CHEAP_PASS_SCOPE_LIMITED` | leave-one-topology-out transform learning; require improvement on all declared held-out families before broader promotion |
| `CB-MAT-01` | P36 | CHEAP | `CHEAP_PASS` | nonlinear heterogeneous modules, stochastic coupling schedules, recovery-energy accounting |
| `CB-RV-01` | P37 | CHEAP | `CHEAP_PASS` | adversarial signal masking and independently scheduled perturbation probes |
| `CB-IB-01` | P38 | CHEAP | `CHEAP_PENDING` | freeze an independently defined protected-detail target and compare channel capacity / compression schemes |
| `CB-ORD-01` | P39 | CHEAP | `CHEAP_PASS` | >2-hop/nonlinear ordering and cost-aware permutation search |
| `CB-MONO-01` | P40 | CHEAP | `CHEAP_PASS` | heterogeneous accuracies, ancestry estimators, adversarial correlated consensus |
| `CB-INT-01` | P41 | CHEAP | `CHEAP_PASS_SCOPE_LIMITED` | queueing, edge failures, multiplex recovery/audit, larger scale sweep |
| `CB-SAFE-01` | P42 | CHEAP | `CHEAP_PENDING` | independent outcome generator before scalar-vs-vector safety gate test |

No `CHEAP_PASS` above is promoted to `PROVISIONAL`; all require at least a medium-strength test outside the toy generator.



###### 4.12.21 Executed CheapBench Suite — v1.16 Internal Synthetic Gate

> **Status lock:** The experiments below are internal synthetic discrimination gates. They test whether the proposed observables and mechanisms add predictive or control value in deliberately simple systems. They do **not** establish deployed-AI validity, physical scaling laws, cross-domain universality, or theorem status. The ground-truth environment generators were frozen separately from the learning/evaluation rules, and failed/partial transfer results are retained.

The first executable batch prioritizes candidates with a cheap independent reference and a credible simpler baseline.

| Bench ID | Prediction | Candidate claim | Baseline | Runs / datasets | Result | Evidence state |
|---|---:|---|---|---:|---|---|
| `CB-RTR-01` | P34 | router plasticity helps under terrain drift | frozen pre-drift router | 100 runs | adaptive post-drift success `0.785 ± 0.008` vs fixed `0.379 ± 0.003`; late-window `0.873 ± 0.007` vs `0.377 ± 0.005` | `CHEAP_PASS` |
| `CB-BRG-01` | P35 | multivariate bridge carries non-redundant scale information | scalar `Λ` only | 20 held-out splits + 4 leave-one-topology-out tests | random held-out NRMSE `0.192 ± 0.005` vs `0.276 ± 0.005` (30.5% relative reduction); unseen-topology transfer mixed | `CHEAP_PASS_SCOPE_LIMITED` |
| `CB-MAT-01` | P36 | mature locally before strong coupling | couple immediately, mature after 12 steps | 500 runs | peak `1.73×`, state cost `7.54×`, recovery `+9.75` steps for couple-first; higher state cost in 100% of runs | `CHEAP_PASS` |
| `CB-RV-01` | P37 | low residual needs vitality channels to distinguish false quiet | observed residual magnitude alone | 30 independently generated datasets | low-residual hidden-failure AUC `0.657 → 0.885`; balanced accuracy `0.636 → 0.784` | `CHEAP_PASS` |
| `CB-IB-01` | P38 | finite governance bandwidth creates abstraction/detail trade-off | not yet frozen | — | benchmark object still risks being tautological if target detail is defined by the same compression map | `CHEAP_PENDING` |

`±` values above are 95% confidence half-widths over repeated runs/splits where applicable. They quantify repeatability inside the synthetic generator only.

**CB-RTR-01 — Adaptive router under abrupt terrain drift.** Five terrain classes and five specialized executors were generated with an independently frozen pre-drift success matrix. At the midpoint, the terrain-to-best-executor mapping changed. Both routers began from the same pre-drift calibration; the fixed router retained its table while the adaptive router updated route values from observed outcomes. The result supports router plasticity in this drift regime, but does not yet establish which learning rule is optimal.

**CB-BRG-01 — Multivariate bridge vs scalar bridge.** A separate nonlinear graph-dynamics generator produced ring, star, complete, and two-community systems. The target was a late macro-instability composite computed from simulated trajectories, not from the bridge formula itself. A scalar bridge used only `Λ`; the richer bundle used `Λ`, buffer level, layer-timescale ratios, spectral-gap/degree-hub topology proxies, and size. On ordinary held-out mixtures the richer bridge reduced NRMSE by about 30.5%. However leave-one-topology-out tests were:

```text
held-out ring:          relative improvement = -29.4%
held-out star:          relative improvement =  +0.1%
held-out complete:      relative improvement = +15.1%
held-out two-community: relative improvement = +15.6%
```

Therefore the correct conclusion is **not** "the bridge is universally scale-portable." The cheap gate shows that structural variables contain useful information inside the sampled topology family, while novel-topology generalization remains an unresolved transformation problem. This negative boundary is preserved as evidence for FMCI's topology-aware residual requirement.

**CB-MAT-01 — Maturation before coupling.** Two locally stabilizable linear modules were perturbed and then coupled. In the mature-first condition, local stabilizing gains were calibrated before cross-module coupling. In the couple-first condition, the same gains were withheld for 12 update steps. Across 500 randomized systems:

```text
mean peak ratio (couple-first / mature-first)       = 1.729
mean cumulative state-cost ratio                    = 7.535
mean recovery time, mature-first                     = 3.888 steps
mean recovery time, couple-first                     = 13.634 steps
mean recovery delay                                  = 9.746 steps
fraction with higher couple-first state cost         = 1.000
```

This is a strong cheap-gate pass for the declared toy regime, but the mechanism is intentionally simple and does not prove that every form of early coupling is harmful.

**CB-RV-01 — Residual Vitality against False Compatibility.** The independent reference was hidden terrain mismatch after adaptation. Some systems retained high hidden mismatch while suppressing the *reported* residual through masking/freeze-like behavior. Evaluation was restricted to cases with low observed residual, exactly where `R_scale ≈ 0` can be misleading. Across 30 datasets, residual magnitude alone was substantially less discriminative than residual plus two vitality channels—probe responsiveness and update activity. This supports the operational rule:

```text
Low residual + live perturbation/update response   → compatible candidate
Low residual + dead perturbation/update response   → false-compatibility suspect
```

The classifier itself is not canonical; the result only supports retaining independent vitality channels.

**Benchmark governance consequence.** Cheap passes alter evidence status, not ontology. The next allocation rule is:

```text
P34 router plasticity       → MEDIUM_PENDING: gradual/nonstationary drift + cost-aware routing
P35 multivariate bridge     → MEDIUM_PENDING: unseen-topology transform learning required
P36 maturation ordering     → MEDIUM_PENDING: nonlinear/heterogeneous modules + energy/rework accounting
P37 residual vitality       → MEDIUM_PENDING: adversarial masking + independent perturbation schedules
P38 information bottleneck → CHEAP_PENDING: first freeze a non-tautological protected-detail target
```

The heavier `CF-TOP-01`, `CF-UNI-01`, `CF-SCALE-01`, and `CF-ENERGY-01` candidates remain pending. `CF-CAT-01` remains candidate-level until its composition/commutation benchmark has an independently frozen semantic target rather than a map generated from the same categorical construction.

**Result artifact:** numerical summaries and confidence estimates for this gate are frozen in `grt_v116_cheapbench_results.json`.


###### 4.12.23 NAT Easy-Integration Patch — v1.17

> **Scope lock:** This patch imports operational structures from NAT v3.2 that are directly compatible with GRT v1.16. It does not import NAT topology claims as GRT theorems. Schur/Feshbach coarse-graining, FDCL renormalization, persistent topology, and category-level formalization remain candidate/pending.

**A. Dual-Resolution Namespace Lock.** `resolution` is split into two axes:

```text
ρ_D = decision / abstraction resolution
      cross-scope discrimination, integration, adjudication capacity

ρ_T = terrain-contact / detail resolution
      local freshness, exception visibility, direct environmental granularity
```

Canonical gradient:

```text
Upper compatibility layer:  ρ_D ↑, ρ_T ↓, portability ↑, update tempo slower
Lower terrain specialist:    ρ_T ↑, role-bounded ρ_D, specificity ↑, update tempo faster
```

This supersedes any ambiguous reading of earlier FCG language where a single word `resolution` could refer to both abstraction and terrain detail.

**B. Multiplex Fractal Map.** FMCI now treats the map as a bundle of distinct functional graphs:

```text
𝕄_{k,ℓ} = {
  G_compute,
  G_task,
  G_information,
  G_authority,
  G_contamination,
  G_recovery,
  G_audit,
  G_memory,
  E_resource,
  U_uncertainty
}_{k,ℓ}
```

The graphs may share nodes but need not share edges, direction, weights, SCCs, authority, or timescales. A result on `G_information` is not evidence about `G_recovery`, `G_authority`, `G_audit`, or `G_contamination` without an explicit bridge.

**C. Mutual Terrain Reconciliation execution form.** Upward transfer is a scoped differential, not a full-state upload:

```text
Δ_i^↑ = {
  new_landmarks, changed_relations, success/failure paths,
  boundary_changes, uncertainty/provenance, recovery evidence,
  exclusions, untested_regions
}
```

Global fusion classifies incoming differentials as corroborating, complementary, conflicting, stale, correlated, or out-of-scope and discounts shared ancestry. Downward transfer is role-projected:

```text
P_{G→i} = Project(M_G, role_i, terrain_i, ρ_D_i, authority_i)
```

The local receiver validates through replay/sandbox/shadow/bounded deployment and returns:

```text
ACCEPT | CONDITIONAL | CONFLICT | OUT_OF_SCOPE | UNSAFE | UNRESOLVED
```

Repeated independent residuals may revise the upper compatibility map, `E_down`, `X_up`, and the Middle routing policy itself. The router is therefore part of the co-evolution loop rather than a fixed codec.

**D. Error-Covariance Diversity Lock.** Nominal heterogeneity is insufficient. For protected task family `q`, measure:

```text
Σ_e(q) = Cov(e_1(q), ..., e_m(q))
```

High off-diagonal covariance indicates shared blind spots even when models, prompts, or vendors differ. Base-model ancestry, shared datasets, retrieval sources, tools, inherited prompts, and upstream patches must be retained in provenance so agreement can be ancestry-discounted. The operational target is **interface compatibility with retained internal error diversity**, not identical maps or maximal agreement.

**E. Ordered Routing Lock.** The orchestrator must choose not only active agents and temporary topology but also the ordered processing path:

```text
π_orch(...) → {A_active, G_task, O_path, budgets, authority, verification, stop_rule}
```

When heterogeneous agents perform lossy projection and reconstruction, `A→B→C` and `A→C→B` are not assumed equivalent. Route order is logged in Resource Intelligence and can be learned from prior outcomes.

**F. Interface-Dilution Contract.** For functional channel `d`:

```text
δ_int^(d)(k) = C_cross^(d)(k) / M_internal(k)
```

A falling ratio is not automatically bad. Sparse interfaces reduce communication/synchronization energy, but are admissible only while channel-specific service constraints hold:

```text
τ_recovery  ≤ T_recovery_deadline
τ_audit     ≤ T_audit_deadline
τ_translate ≤ T_translation_deadline
rollback_reach = true
protected_coverage ≥ floor
```

The target is the **minimum sufficient interface**, not maximum connectivity.

**G. Claim-Type × Evidence-State Matrix.** GRT now records two independent status axes:

| Claim type | Meaning |
|---|---|
| `D` | definition / object fixed by convention |
| `A` | model assumption |
| `M` | derived within a declared model/object |
| `B` | bridge conjecture across objects/scales/theories |
| `E` | empirical hypothesis |

Evidence state remains `CANDIDATE → CHEAP_PASS/... → MEDIUM → HEAVY → PROVISIONAL → PROMOTED`. A `CHEAP_PASS` cannot turn a `B` bridge into an `M` theorem, and a theorem on one object cannot become empirical evidence for another object by citation alone.

**H. v1.17 NAT EasyBench results.**

| Bench | Claim | Result | State |
|---|---|---|---|
| `CB-ORD-01` | ordered routing matters | fixed MSE `1.992` → history-selected `1.875`; 5.9% reduction; median order gap 12.5% | `CHEAP_PASS` |
| `CB-MONO-01` | correlated errors create false compatibility | same ~20% individual error; majority error `0.033→0.201` as error correlation ~0→1 | `CHEAP_PASS` |
| `CB-INT-01` | interface density has a deadline-constrained Pareto frontier | minimum tested deadline-feasible interface `30` edges (`δ_int=0.1875`) vs dense `90` edges | `CHEAP_PASS_SCOPE_LIMITED` |

`CB-ORD-01` used 300 independently generated operator pairs. 79.7% had >5% order-dependent loss, and a frozen calibration history selected the lower-loss held-out order 83.3% of the time.

`CB-MONO-01` held agent count and marginal individual error approximately constant while shifting error dependence from independent to shared. Mean agreement rose from `0.806` to `1.000` even as majority error worsened, directly exposing the false-consensus failure mode.

`CB-INT-01` used ten modules of eight nodes with fixed local structure and varied cross-module interfaces. Under the declared p95 deadline `≤ 6` hops, the minimum tested feasible interface used one-third the cross edges of the densest condition. This does not identify a universal optimum; it supports a Pareto framing under explicit deadlines.

**Pending easy/hard boundary.** `CB-SAFE-01` (protected-vector scale promotion) remains `CHEAP_PENDING` until future-outcome labels are generated independently of the same thresholds under test. Schur/Feshbach effective operators are taken up in §4.12.24 as a candidate family; FDCL scale laws, persistent-homology audits, and categorical compatibility remain outside the current cheap-integration boundary.


###### 4.12.24 Schur/Feshbach Candidate Sieve — v1.18

> **Source and scope lock.** NAT §7.34.3 supplies the declared linear boundary/interior construction and explicitly requires replay/intervention validation before treating the algebraic effective operator as behaviorally sufficient. GRT therefore imports Schur/Feshbach as a **candidate family and audit method**, not as a universal law of agent clusters. The exact algebra and the empirical bridge are kept separate.

For a declared operator with boundary variables `B` and internal variables `I`,

```text
L = [[L_BB, L_BI],
     [L_IB, L_II]]
```

and invertible `L_II` on the declared gauge/complement, the static effective boundary operator is

```text
L_eff(0) = L_BB - L_BI L_II^{-1} L_IB.
```

For a declared spectral/dynamic convention `L + ζI`, the frequency/scale-conditioned family is

```text
L_eff(ζ)
  = L_BB + ζ I_B
    - L_BI (L_II + ζ I_I)^{-1} L_IB.
```

The sign of `ζ` is convention-dependent and must be object-locked. GRT does not use the word *Feshbach* to imply quantum dynamics; here it denotes the spectral-parameter elimination pattern on the declared operator.

**Why candidate splitting is mandatory.** `Schur/Feshbach works` is too coarse a claim. Six materially different candidates are registered:

| Candidate ID | Candidate | Claim type | Cheap status after v1.18 | Scope / next gate |
|---|---|---|---|---|
| `CF-SF-STAT-01` | full static Schur on a declared linear patch | `M` | `CHEAP_PASS_SCOPE_LOCKED` | algebra exact on object; next test directed/non-normal and gauge-singular declared operators |
| `CF-SF-LR-01` | low-rank approximate Schur as cheaper interface contract | `E` | `CHEAP_PASS_SCOPE_LIMITED` | test rank/error/runtime frontier and spectra unlike current generator |
| `CF-SF-REG-01` | fixed regularization rule improves noisy/ill-conditioned Schur estimates | `E` | `CHEAP_FAIL_GENERAL` | retain only as narrower adaptive-regularization candidate; tune without evaluation leakage |
| `CF-SF-DYN-01` | frequency-conditioned Feshbach captures dynamic interior memory | `M` on linear resolvent; `B/E` for agent behavior | `CHEAP_PASS_SCOPE_LOCKED` | independent time-domain replay with delay/non-normal dynamics |
| `CF-SF-NL-01` | state-conditioned Jacobian Schur is a useful local nonlinear interface map | `B/E` | `CHEAP_PASS_SCOPE_LIMITED` | wider perturbations, discrete policies, switching regimes, operating-point update cost |
| `CF-SF-XFER-01` | one shared effective operator transfers across heterogeneous terrains | `B/E` | `CHEAP_FAIL_CURRENT_FORM` | replace with terrain-conditioned/meta-learned operator before retest |

The candidate family obeys four locks:

1. **Object lock:** the effective operator belongs to one declared graph/operator, boundary set, process semantics, and time window.
2. **Interface lock:** eliminating internals does not eliminate their causal effect; it exposes only their boundary contract.
3. **Dynamic lock:** `L_eff(0)` is not a substitute for `L_eff(ζ)` when interior memory is active at the observation timescale.
4. **Behavioral lock:** algebraic exactness on a linear operator is not empirical validation of nonlinear, adaptive, delayed, or strategic agents.

##### CB-SF-01 — Clean Static Linear Boundary Response

**Independent object generator.** 250 positive-definite block systems were generated with independently sampled interior dimension, conditioning, coupling, and boundary Schur block. Candidate maps were compared against the independently retained true boundary response.

| Candidate | Mean relative operator error | Median | p95 |
|---|---:|---:|---:|
| Boundary-only `L_BB` | 0.04044 | 0.03031 | 0.11467 |
| Diagonal interior elimination | 0.01807 | 0.01210 | 0.05112 |
| Rank-4 approximate Schur | **0.004821** | **0.003462** | **0.01292** |
| Full Schur | ~`1.1e-17` | `0` | ~`6.9e-17` |

**Decision.** `CF-SF-STAT-01` passes only as an implementation/object-lock check; its mathematical status comes from the declared linear algebra, not from this benchmark. `CF-SF-LR-01` survives as a real empirical candidate because the approximation materially beats simpler baselines while remaining non-exact.

##### CB-SF-02 — Noisy / Ill-Conditioned Operator Estimate

300 systems with condition numbers roughly `10^2–10^4` were evaluated after independently perturbing the measured interior/coupling/boundary blocks. A predeclared regularization rule used `λ = noise × median(diag(L_II_est))`.

| Candidate | Mean relative error | p95 |
|---|---:|---:|
| Noisy full Schur | 0.02162 | 0.03888 |
| Regularized Schur | 0.02157 | 0.03849 |
| Diagonal Schur | 0.02265 | 0.03907 |
| Rank-4 Schur | 0.02170 | 0.03856 |

The regularized candidate beat the noisy full Schur in only `43.7%` of systems. The mean difference was negligible.

**Decision.** Reject the claim that this fixed regularization rule is generally superior. `CF-SF-REG-01 → CHEAP_FAIL_GENERAL`. This negative result is retained; adaptive regularization may still be tested as a different candidate.

##### CB-SF-03 — Dynamic Boundary Response: Static Schur vs Frequency-Conditioned Feshbach

The ground truth was generated from the full linear system response at complex frequency `ζ=iω`; the static candidate used the zero-frequency interior elimination, while the dynamic candidate recomputed the effective interior response at the same `ω`.

| `ω` | Static Schur mean boundary-response error | p95 | Static coupling-correction mismatch |
|---:|---:|---:|---:|
| 0.01 | 0.00092 | 0.00267 | 0.00644 |
| 0.10 | 0.00893 | 0.02391 | 0.06434 |
| 0.30 | 0.02346 | 0.06717 | 0.19201 |
| 1.00 | **0.03627** | **0.09892** | **0.61286** |
| 3.00 | 0.02381 | 0.06174 | 1.62866 |
| 10.0 | 0.00940 | 0.02527 | 4.66725 |
| 30.0 | 0.00322 | 0.00833 | 12.89684 |

The frequency-conditioned elimination matched the declared linear resolvent to numerical precision by construction. Therefore its zero residual is **not counted as empirical proof**. The discriminating information is the failure surface of the static approximation: dynamic interior memory becomes material around the interior timescale, even though the total response error falls again when the boundary `iωI` term dominates at very high frequency.

**Decision.** `CF-SF-DYN-01` is retained with a strong scope lock. The next non-tautological gate is time-domain replay on systems with delay, non-normal transient amplification, and independently sampled intervention waveforms.

##### CB-SF-04 — Nonlinear Terrain: Fixed vs State-Conditioned Jacobian Schur

A nonlinear interior equation with cubic local curvature was generated independently. Around each nonlinear operating point, the fixed zero-state Schur and a state-conditioned Jacobian Schur predicted nearby boundary interventions.

| Perturbation radius | Fixed Schur mean NMSE | Fixed p95 | Local Jacobian mean NMSE | Local p95 |
|---:|---:|---:|---:|---:|
| 0.05 | 0.01012 | 0.06370 | `1.07e-6` | `4.23e-6` |
| 0.20 | 0.00995 | 0.06194 | `3.24e-5` | `1.01e-4` |
| 0.50 | 0.00935 | 0.05440 | `1.56e-4` | `6.60e-4` |

The local Jacobian candidate beat the fixed Schur in `100%` of the 600 tested nearby-intervention cases.

**Decision.** A fixed Schur map should be treated as a local approximation in nonlinear terrain. `CF-SF-NL-01 → CHEAP_PASS_SCOPE_LIMITED`; however, the local Jacobian requires operating-point estimation and refresh cost, so it is not a free universal compression.

##### CB-SF-05 — Cross-Terrain Portability

A shared normalized effective template was frozen from 120 training patches and evaluated on 160 independently generated held-out patches. It was compared with each patch's own object-specific Schur operator.

```text
shared-template mean relative error  = 0.5324
shared-template p95                  = 0.6767
object-specific Schur mean error     ≈ 9.8e-18
```

**Decision.** `CF-SF-XFER-01 → CHEAP_FAIL_CURRENT_FORM`. Algebraic exactness does not transfer across heterogeneous terrain simply because every patch admits a Schur reduction. This directly supports the FMCI rule that **the compression operator itself must be terrain-conditioned or learned through an explicit bridge**.

##### Schur/Feshbach Promotion Rule

The v1.18 result does **not** promote Schur/Feshbach to a general GRT law. It instead installs a selection rule:

```text
Static + linear + declared operator
  → full Schur is the reference exact interface map.

Static + large interior + tolerated approximation
  → low-rank Schur is a candidate; choose rank from an error/cost frontier.

Noisy / ill-conditioned estimate
  → do not assume regularization helps; benchmark the estimator and λ policy.

Dynamic / memory-bearing interior
  → use ζ-conditioned effective operators; static Schur requires a quasi-static audit.

Nonlinear / adaptive interior
  → fixed Schur is local only; consider state-conditioned Jacobian or learned effective maps.

Cross-terrain reuse
  → forbidden by default; require terrain-conditioned bridge + held-out residual test.
```

**Medium/Heavy queue created from the surviving candidates:**

| Next bench | Purpose | Cost | Status |
|---|---|---:|---|
| `MB-SF-01` | directed/non-normal linear systems; compare static Schur, transient behavior, and replay response | MEDIUM | `MEDIUM_COMPLETE` (see §4.12.25) |
| `MB-SF-02` | singular Laplacian/gauge systems; pseudoinverse vs declared complement/gauge choice | MEDIUM | `MEDIUM_COMPLETE` (see §4.12.25) |
| `MB-SF-03` | time-domain Feshbach/reduced-memory replay with delay and independently sampled forcing | MEDIUM | `MEDIUM_PENDING` |
| `MB-SF-04` | nonlinear switching/saturation agent modules; refresh-rate and operating-point drift cost | MEDIUM | `MEDIUM_PENDING` |
| `MB-SF-05` | rank/error/runtime/energy frontier for approximate Schur on larger sparse interiors | MEDIUM | `MEDIUM_PENDING` |
| `HB-SF-01` | real multi-agent module boundary contract vs internal replay under novel tasks | HEAVY | `HEAVY_PENDING` |
| `HB-SF-02` | recursive Schur/Feshbach closure across multiple FMCI scales | HEAVY | `HEAVY_PENDING` |
| `HB-SF-03` | multiplex-specific effective operators for information/recovery/audit/authority graphs | HEAVY | `HEAVY_PENDING` |

The heavy queue is not executed merely because the algebra is attractive. Each item remains pending until the relevant medium bench provides enough discrimination to justify the cost.

**Frozen artifacts:** `grt_v118_schur_feshbach_cheapbench_results.json`; `run_grt_v118_schur_feshbach_cheapbench.py`.


###### 4.12.25 Singular/Gauge and Directed/Non-Normal Schur MediumBench — v1.19

> **Promotion lock.** This section advances only the two v1.18 medium queues `MB-SF-01` and `MB-SF-02`. It does not generalize Schur/Feshbach to arbitrary adaptive agents. Exact statements remain statements about declared linear operators; behavioral statements remain empirical bridge candidates.

##### Candidate family A — Singular / gauge-aware elimination

A singular interior block requires more than replacing an inverse symbol mechanically. Let `N` span the declared nullspace of `L_II`. A bounded gauge-invariant boundary reduction requires the coupling to respect the null direction:

```text
L_BI N ≈ 0  and  N^T L_IB ≈ 0.
```

If this range/nullspace compatibility fails, the eliminated interior contains a direction with zero quadratic cost but nonzero boundary coupling; a finite Schur boundary energy is not licensed without an additional constraint or gauge contract.

| Candidate ID | Candidate | Medium result | Status |
|---|---|---:|---|
| `CF-SF-GPINV-01` | Moore–Penrose pseudoinverse Schur on a compatible singular object | mean rel. error `6.8e-18` | `MEDIUM_PASS_SCOPE_LOCKED` |
| `CF-SF-GCOMP-01` | explicit complement/gauge-basis reduction | mean rel. error `5.7e-16`; gauge-basis difference ~`6.0e-16` | `MEDIUM_PASS_SCOPE_LOCKED` |
| `CF-SF-GRIDGE-01` | fixed ridge/diagonal loading as universal gauge replacement | mean rel. error `0.00277`, p95 `0.0107` | `MEDIUM_FAIL_GENERAL` |
| `CF-SF-GAUDIT-01` | nullspace-coupling compatibility audit before elimination | synthetic leakage AUC `1.000` | `MEDIUM_PASS_SCOPE_LOCKED` |

**Interpretation.** Pseudoinverse and explicit-complement forms are two coordinate descriptions of the same compatible quotient operation under the frozen generator. Their agreement is not evidence that every singular system is safe to reduce; the load-bearing condition is the nullspace/range contract. Ridge is useful only as an estimator or deliberately modified model, not as a semantics-preserving replacement for gauge specification.

**New singular-object rule:**

```text
singular L_II
  → identify nullspace / gauge
  → audit coupling compatibility
  → if compatible: pseudoinverse or declared complement
  → if incompatible: STOP; add physical/semantic constraint, do not silently regularize
```

##### Candidate family B — Directed / non-normal elimination

For a nonsymmetric but invertible interior block, the static Schur algebra remains valid for the declared steady-state linear equations. The benchmark separates this from transient adequacy.

**Equilibrium response (220 frozen directed systems):**

| Candidate | Mean relative boundary error | p95 |
|---|---:|---:|
| nonsymmetric static Schur | `1.5e-16` | `3.36e-16` |
| symmetrize-then-Schur surrogate | `0.1991` | `0.5138` |

`CF-SF-DSTAT-01 → MEDIUM_PASS_EQUILIBRIUM_ONLY`. `CF-SF-DSYM-01 → MEDIUM_FAIL_GENERAL`.

The failure of the symmetric shortcut is conceptually important: **directionality is part of the interface contract.** A directed routing/recovery/authority process may not be replaced by an undirected energy picture merely because symmetric Schur theory is convenient.

**Transient replay:** piecewise-random boundary forcing was applied to the full directed system and compared with reduced models.

| Candidate | Mean normalized replay error | Median | p95 |
|---|---:|---:|---:|
| boundary-only | `0.04010` | `0.02783` | `0.12574` |
| static nonsymmetric Schur | `0.04834` | `0.02466` | `0.18151` |
| symmetrized surrogate | `0.96538` | `0.04216` | `0.21925` |
| naive moment-1 memory correction | unstable heavy tail | `0.04099` | `0.66517` |

The first-order memory correction beat static Schur in only `12.3%` of systems and produced rare explosive failures. `CF-SF-DM1-01 → MEDIUM_FAIL_CURRENT_FORM`. This is retained as negative-result memory: low-order dynamic correction must be stability-constrained rather than added algebraically by default.

##### Non-normality as a Schur-adequacy gate

The same directed benchmark tested several candidate risk indicators against static-Schur transient error.

| Gate variable | Spearman with replay error | AUC for top-quartile error |
|---|---:|---:|
| numerical abscissa `λ_max((A+A^T)/2)` | **0.696** | **0.875** |
| commutator departure `||A^T A-AA^T||/||A||²` | 0.597 | 0.814 |
| spectral abscissa `max Re λ(A)` | 0.417 | 0.744 |
| interior/boundary timescale ratio | 0.026 | 0.504 |

Thus eigenvalue stability alone is an incomplete diagnostic for reduction adequacy in non-normal systems. Transient amplification geometry carries additional information.

A second independent 320-system dataset was split into train/test. A threshold on numerical abscissa was selected on the training half only; the held-out policy selected static Schur below the threshold and boundary-only above it.

```text
held-out static Schur mean error     = 0.05110
held-out boundary-only mean error    = 0.03671
held-out gated selector mean error   = 0.03564
relative gain vs best fixed baseline = 2.91%
```

`CF-SF-DGATE-01` and `CF-SF-DSELECT-01 → MEDIUM_PASS_SCOPE_LIMITED`.

The gain is deliberately described as **narrow**. It is enough to justify a candidate gating policy, not enough to claim numerical abscissa as a universal reduction criterion.

##### v1.19 Schur selection tree

```text
Is L_II singular?
  YES → identify gauge/nullspace
        → coupling compatible?
            NO  → no Schur promotion; constrain/redefine object
            YES → pseudoinverse or explicit complement
  NO  → continue

Is operator directed/non-normal?
  NO  → v1.18 static/dynamic/nonlinear tree
  YES → equilibrium only?
            YES → nonsymmetric static Schur is reference
            NO  → audit transient amplification
                  → low-risk gate: static Schur candidate
                  → high-risk gate: retain more state / dynamic Feshbach / fallback
```

##### Queue update after MediumBench

| Bench | v1.18 status | v1.19 status | Next action |
|---|---|---|---|
| `MB-SF-01` directed/non-normal | `MEDIUM_PENDING` | **`MEDIUM_COMPLETE`** | test stable memory-kernel/rational dynamic reductions |
| `MB-SF-02` singular/gauge | `MEDIUM_PENDING` | **`MEDIUM_COMPLETE`** | noisy nullspace estimation and changing-gauge robustness if needed |
| `MB-SF-03` time-domain Feshbach | `MEDIUM_PENDING` | `MEDIUM_PENDING` | split into exact retained-memory, stable rational, and learned-memory candidates |
| `MB-SF-04` nonlinear switching | `MEDIUM_PENDING` | `MEDIUM_PENDING` | switching/saturation + refresh-cost bench |
| `MB-SF-05` rank/error/runtime/energy | `MEDIUM_PENDING` | `MEDIUM_PENDING` | larger sparse interiors and wall-clock/energy proxy |
| `HB-SF-01` real agent boundary contract | `HEAVY_PENDING` | `HEAVY_PENDING` | no execution yet |
| `HB-SF-02` recursive multiscale closure | `HEAVY_PENDING` | `HEAVY_PENDING` | no execution yet |
| `HB-SF-03` multiplex-specific Schur | `HEAVY_PENDING` | `HEAVY_PENDING` | no execution yet |

**Next-candidate refinement.** The failed moment-1 candidate narrows `MB-SF-03` to three safer competitors:

1. `CF-SF-MEM-EXACT-01` — explicit retained memory kernel / augmented hidden state;
2. `CF-SF-MEM-RAT-01` — stable rational/Padé-like approximation with pole-stability lock;
3. `CF-SF-MEM-LEARN-01` — learned finite-memory interface map with independent replay and rollback.

No one of these is promoted in v1.19. They are benchmark-ready candidates.

**Frozen artifacts:** `grt_v119_schur_mediumbench_results.json`; `run_grt_v119_schur_mediumbench.py`.


###### 4.12.26 Time-Domain Feshbach Memory Candidate Bench — v1.20

> **Scope and anti-tautology lock.** `MB-SF-03` asks a different question from the frequency-domain algebra check in v1.18. The exact retained-memory construction is treated as a mathematical reference on the declared linear system, not empirical evidence. The discriminating test is whether **compressed or learned memory representations** predict independently generated time-domain boundary trajectories, remain stable, and preserve useful behavior under forcing and modest terrain drift.

The exact continuous-time elimination of an interior state `i(t)` from

```text
b_dot = A_BB b + A_BI i + B_B u
i_dot = A_IB b + A_II i
```

contains memory:

```text
i(t)
  = exp(A_II t) i(0)
    + integral_0^t exp(A_II (t-s)) A_IB b(s) ds

b_dot
  = A_BB b
    + A_BI exp(A_II t) i(0)
    + integral_0^t K(t-s) b(s) ds
    + B_B u

K(t) = A_BI exp(A_II t) A_IB.
```

This makes the v1.19 candidate split concrete: a dynamic boundary contract either retains the relevant hidden state, approximates the memory kernel with a stable finite-dimensional realization, or learns a finite-memory input/output map from replay.

##### Candidate family

| Candidate ID | Interface construction | Information requirement | Principal advantage | Principal risk | v1.20 status |
|---|---|---|---|---|---|
| `CF-SF-MEM-EXACT-01` | retain the full interior state / exact memory realization | full declared operator and interior state | exact reference on the linear object | no meaningful coarse-graining; retains internal dimension | `MEDIUM_PASS_REFERENCE_ONLY` |
| `CF-SF-MEM-RAT-ACC-01` | stable exponential/rational kernel fit, accuracy-selected state count | declared operator | high dynamic replay accuracy and forcing robustness | accuracy selector may spend as many states as the original interior | `MEDIUM_PASS_BEHAVIORAL_SCOPE_LOCKED` |
| `CF-SF-MEM-RAT-BUDGET-01` | stable rational kernel under an explicit hidden-state budget | declared operator + state budget | controllable error/compression frontier | required budget depends on pole/terrain geometry | `MEDIUM_PASS_SCOPE_LIMITED` |
| `CF-SF-MEM-LEARN-ID-01` | stability-locked finite-memory ARX learned from replay | boundary replay only; no interior operator required | black-box applicability | distribution-shift and excitation dependence | `MEDIUM_PASS_ID_ONLY` |
| `CF-SF-MEM-LEARN-OOD-01` | same learned map reused under novel forcing | same as above | cheap reuse if valid | fast/impulsive OOD error | `MEDIUM_FAIL_CURRENT_FORM` |

The learned candidate is intentionally retained rather than discarded: it solves a different operational problem. Rational Feshbach is attractive when the operator is inspectable; a learned interface may be the only available path when the interior is proprietary, opaque, or too expensive to identify directly.

##### MB-SF-03A — Same-system time-domain replay

**Generator.** The bench used 72 independently generated stable linear systems (`24` each in real-decay, oscillatory, and non-normal interior regimes), boundary dimension `b=2`, interior dimension `m=8..14`, `dt=0.05`, and 180-step trajectories. Learned models used separate train/validation trajectories. Final evaluation used independent ID, fast-OOD, and impulse forcing.

**Candidate details.**

- Exact retained memory: full dynamic system retained; reference only.
- Rational memory: `K(t)` approximated by a stable sum of exponentials `Σ_j W_j exp(-p_j t)`; the **full augmented reduced realization** had to pass a stability audit, not merely the individual pole signs.
- Learned memory: ARX history lengths `{2,4,8,12}` and ridge values `{1e-6,1e-4,1e-2,1}` competed on independent validation; the autonomous companion block required spectral radius `<0.999`. Evaluation rollouts received only a short true boundary warm-start equal to the chosen history length.
- Static Schur: quasi-static dynamic baseline.

| Test | Rational accuracy-selected | Learned finite-memory | Static Schur |
|---|---:|---:|---:|
| ID forcing mean trajectory error | **0.00135** | 0.03805 | 0.05896 |
| Fast OOD forcing | **0.00140** | 0.10160 | 0.05386 |
| Impulse forcing | **0.00125** | 0.19993 | 0.05577 |

No candidate produced a rollout blow-up under the declared benchmark after the stability gates.

**Regime split.** The accuracy-selected rational candidate remained low-error across all three tested dynamic families: mean errors were approximately `2.45e-5` (real-decay), `0.00364` (oscillatory), and `0.000344` (non-normal). Static Schur was especially weak on the non-normal family (`0.1278` mean across forcing classes), consistent with v1.19's transient warning.

**Decision.** `CF-SF-MEM-RAT-ACC-01` survives strongly as a behavioral dynamic interface candidate, but it is **not yet a compression result**. Its selected realization carried mean hidden dimension `11.28` versus mean original interior dimension `10.99`. Accuracy without state reduction is useful as an interface abstraction, but it does not establish resource savings.

The learned candidate is split by domain of validity. On ID replay it improved mean error by roughly `35%` relative to static Schur, but on fast OOD and impulse forcing it was worse than the static baseline. Therefore the current learned finite-memory form is **not a general Feshbach replacement**.

##### MB-SF-03B — Rational state-budget frontier

To separate accuracy from compression, a second independent bench fixed the number of real exponential memory poles `r=1..5` instead of allowing an accuracy selector to spend states freely. Each pole adds `b=2` hidden memory states.

| Rational budget | Mean hidden-state / original-interior ratio | ID mean error | Fast-OOD mean error | Stability fraction |
|---:|---:|---:|---:|---:|
| `r=1` | 0.184 | 0.02989 | 0.02458 | 1.00 |
| `r=2` | 0.368 | 0.01552 | 0.01570 | 1.00 |
| `r=3` | **0.552** | **0.00759** | **0.00680** | 1.00 |
| `r=4` | 0.736 | 0.00358 | 0.00320 | 1.00 |
| `r=5` | 0.919 | 0.00237 | 0.00255 | 1.00 |

The frontier is more informative than declaring one universal rank. Under this generator, even the aggressive `r=1` budget used about 18% of the original interior-state count while beating the overall static-Schur ID mean; `r=2` and `r=3` provide substantially better tail/terrain behavior.

**Decision.** `CF-SF-MEM-RAT-BUDGET-01 → MEDIUM_PASS_SCOPE_LIMITED`. GRT should treat dynamic-memory rank as a **resource contract**, not a structural constant:

```text
choose r*
  = argmin_r MemoryCost(r)

subject to:
  ReplayError_ID(r) <= epsilon_ID
  ReplayError_OOD(r) <= epsilon_OOD
  Stability(r)       = PASS
  Recovery/Audit behavior remains inside contract
```

A practical default candidate from this synthetic family is `r=3`, not because `3` is universal, but because it occupied a useful middle point of the tested error/state frontier.

##### MB-SF-03C — Mild interior-timescale drift and refresh

A frozen-map audit changed only the stable interior timescale (`A_II -> 0.7 A_II` or `1.3 A_II`) while keeping the boundary/coupling object fixed.

| Frozen map | Mean drift replay error |
|---|---:|
| old full/exact operator | 0.01830 |
| old rational map | **0.01852** |
| old learned finite-memory map | 0.04003 |
| old static Schur | 0.05149 |
| refreshed exact operator | 0 |

This establishes **staleness**, not catastrophic failure: even an originally exact memory operator becomes wrong when the terrain/operator changes. The correct object is therefore `(effective map, operator version, validity window)`, not an unversioned effective map.

A smaller independent refresh audit then compared old versus refreshed models after the same class of drift:

```text
r=3 rational:
  old operator mean error       0.01498
  refreshed operator mean error 0.00613

learned finite-memory:
  old replay model mean error       0.03491
  refreshed with 3 train + 1 val   0.03458
```

The rational refresh showed a clear average improvement. The low-data learned refresh did not. This does **not** prove that learned refresh is ineffective; it shows that naive small-sample retraining is not automatically a useful correction rule and should itself be candidate-benchmarked.

##### Kernel-fit residual is not the behavioral objective

A notable audit result is that the accuracy-selected rational family had mean raw kernel-norm fitting error around `0.169`, yet mean boundary replay error around `0.00134`. The discrepancy is expected because the boundary task excites and weights only part of the full kernel geometry.

Therefore:

```text
low ||K_hat - K||   is useful,
but it is NOT sufficient for promotion.

Promotion requires:
  intervention-weighted / replay boundary residual
  + stability
  + protected-channel behavior
  + declared state/resource budget.
```

This prevents GRT from optimizing an operator norm that is poorly aligned with the actual governance interface contract.

##### v1.20 Time-domain Feshbach selection tree

```text
Dynamic interior memory material?
  NO  -> static Schur branch from v1.18/v1.19
  YES -> can the internal operator be inspected?

         YES
          -> exact retained-memory model = reference only
          -> fit stable rational memory family
          -> choose hidden-state budget from error/state frontier
          -> replay + OOD + stability gate
          -> version map against terrain/operator drift

         NO
          -> learned finite-memory / learned state-space candidate
          -> independent train/validation/replay split
          -> autonomous stability gate
          -> OOD excitation probes required
          -> residual-triggered rollback/refresh
          -> no promotion from ID replay alone
```

##### Queue update after v1.20

| Bench / candidate | v1.20 status | Next action |
|---|---|---|
| `MB-SF-03` time-domain Feshbach family | **`MEDIUM_COMPLETE`** | retain split candidate statuses rather than one family verdict |
| `CF-SF-MEM-RAT-CPLX-01` complex-pole rational compression | `MEDIUM_PENDING` | test whether oscillatory regimes reach the same error with fewer retained states |
| `CF-SF-MEM-SSID-01` black-box learned state-space / subspace identification | `MEDIUM_PENDING` | compare with ARX on OOD forcing at matched replay budget |
| `CF-SF-MEM-REFRESH-01` residual-triggered refresh policy | `MEDIUM_PENDING` | independent drift detector; compare refresh cost and false triggers |
| `MB-SF-04` nonlinear switching/saturation | `MEDIUM_PENDING` | test state-conditioned dynamic memory and switching validity windows |
| `MB-SF-05` rank/error/runtime/energy frontier | `MEDIUM_PENDING` | use optimized implementations and hardware-neutral operation counts; current Python wall-clock is not promotion evidence |
| `HB-SF-01` real multi-agent boundary contract | `HEAVY_PENDING` | no execution yet |
| `HB-SF-02` recursive multiscale closure | `HEAVY_PENDING` | no execution yet |
| `HB-SF-03` multiplex-specific Schur/Feshbach | `HEAVY_PENDING` | no execution yet |

**Runtime interpretation lock.** The prototype benchmark measured wall-clock diagnostics, but candidate implementations used different Python execution paths. Those times are **not** used as evidence for an energy or compute-efficiency claim. The state-budget frontier is the current resource proxy; optimized runtime/energy comparison remains `MB-SF-05`.

**Frozen artifacts:** `grt_v120_feshbach_memorybench_results.json`; `grt_v120_rational_frontier_results.json`; `grt_v120_refreshbench_results.json`; `run_grt_v120_feshbach_memorybench.py`; `run_grt_v120_rational_frontier.py`; `run_grt_v120_refreshbench.py`.


###### 4.12.27 Complex-Pole Rational vs Black-Box State-Space vs Residual-Triggered Refresh — v1.21

> **Scope lock.** This bench separates three different objects that should not be collapsed into one claim: (1) a white-box complex-pole memory approximation, (2) an operator-free black-box boundary state-space model learned from active input/output probes, and (3) a drift-triggered model-refresh policy. A model can be accurate without being cheap to refresh; a refresh policy can be useful without proving the underlying effective operator is universal.

##### Candidate split

| Candidate ID | Object | Internal operator required? | Update mode | v1.21 verdict |
|---|---|---:|---|---|
| `CF-SF-MEM-RAT-CPLX-01` | complex-conjugate-pole rational memory kernel | yes | recompute from current operator | `MEDIUM_PASS_SCOPE_LIMITED` |
| `CF-SF-MEM-SSID-ERA-01` | ERA/subspace boundary state-space | no; active boundary probe required | re-identify from probe response | `MEDIUM_PASS_PROBE_ACCESS_SCOPE_LOCKED` |
| `CF-SF-MEM-REFRESH-PERSIST-01` | persistent residual-triggered refresh | wraps a versioned model | refresh only after persistent residual alarm | `MEDIUM_PASS_SCOPE_LIMITED` |
| `CF-SF-MEM-REFRESH-DUAL-01` | dual relative+absolute residual trigger | wraps a versioned model | conservative refresh | `MEDIUM_PASS_CONSERVATIVE` |
| `CF-SF-MEM-REFRESH-SIMPLE-01` | single-threshold residual trigger | wraps a versioned model | eager/simple | `MEDIUM_FAIL_AS_DEFAULT` |

##### Candidate A — Complex-pole rational memory

The v1.20 real-exponential family is extended to allow real poles and conjugate complex pairs. For discrete memory lag `l`, the fitted kernel has the real form

```text
K_hat[l]
  = Σ_j C_j p_j^l
    + Σ_q (A_q Re(z_q^l) + B_q Im(z_q^l)),

|p_j| < 1, |z_q| < 1.
```

The candidate uses pole locations available from the declared interior operator, while fitting boundary-relevant residues under a small basis budget. This allows oscillatory interior memory to be represented without replacing every oscillatory pair by multiple purely decaying exponentials.

**Important resource lock:** the reported `basis_dim` is a kernel-basis count, not automatically the number of optimized runtime states. It is therefore a compression proxy only. Runtime/state equivalence remains `MB-SF-05` pending.

##### Candidate B — Black-box learned state-space

The black-box candidate uses only boundary input/output impulse-response Markov parameters

```text
G_k = C Phi^k Gamma
```

and a truncated Hankel realization (ERA/subspace identification). It does **not** read `A_II`, its poles, or an interior Schur block. Candidate ranks compete on independent validation trajectories and unstable learned realizations are rejected.

This is stronger than the v1.20 ARX candidate in one important sense: it learns a latent dynamical state rather than a fixed finite output-history regression.

##### MB-SF-03D — Same-terrain competition

**Generator.** `24` independently generated stable systems (`8` each real-decay, oscillatory, non-normal), boundary dimension `2`, mean interior dimension `11.33`, `dt=0.05`, and independent ID / fast-OOD / chirp / impulse forcing.

| Held-out forcing | Complex-pole rational mean error | Black-box ERA mean error |
|---|---:|---:|
| ID | 0.02818 | **0.00370** |
| Fast OOD | 0.01823 | **0.00240** |
| Chirp / swept frequency | 0.04017 | **0.00526** |
| Impulse | 0.01853 | **0.00276** |

The mean selected complex-pole basis dimension was `3.25`; the mean ERA latent rank was `5.00`. ERA rank was about `39.2%` of the full boundary+interior state dimension on this generator. The complex-pole basis ratio was about `29.7%` of interior dimension, but this is **not** a runtime-state ratio and is not used as an energy claim.

##### Regime separation: why complex poles are not enough for non-normal interiors

| Regime | Rational ID | ERA ID | Rational chirp | ERA chirp |
|---|---:|---:|---:|---:|
| real-decay | 0.00285 | **0.00164** | 0.00504 | **0.00263** |
| oscillatory | 0.00364 | **0.00251** | 0.00505 | **0.00371** |
| non-normal | 0.07805 | **0.00694** | 0.11043 | **0.00944** |

Complex poles solve an **oscillation representation** problem, but they do not by themselves solve a **non-normal transient geometry** problem. The non-normal family produced the large rational tail. This is consistent with the v1.19 warning that eigenvalue information alone can miss transient amplification.

Therefore:

```text
complex poles present
  does NOT imply
complex-pole rational is sufficient.

Need additionally:
  residue / mode geometry
  + non-normality audit
  + behavioral replay.
```

`CF-SF-MEM-RAT-CPLX-01` therefore survives only with a non-normality/replay scope lock.

##### Black-box ERA verdict and probe-access limitation

ERA achieved the lowest mean replay error in every forcing class and remained strong on the non-normal systems. This supports the candidate claim:

> When interior operators are unavailable but controlled boundary excitation and observation are available, a learned latent state-space may recover boundary dynamics more robustly than a small pole-basis approximation.

But the current bench generated a clean impulse/Markov response from the synthetic system. It does **not** establish robustness to noisy sensors, passive-only logs, missing excitation directions, asynchronous data, or changing agent policies.

Accordingly:

```text
CF-SF-MEM-SSID-ERA-01
  = MEDIUM_PASS_PROBE_ACCESS_SCOPE_LOCKED
  != deployed black-box identification theorem.
```

The next cheap/medium discriminator is `CF-SF-MEM-SSID-NOISE-01`: add measurement/process noise and compare active-probe ERA, passive subspace identification, and ARX/state-space hybrids at matched data budgets.

##### MB-SF-03E — Terrain drift and refresh benefit

The effective maps were frozen, the interior/coupling terrain was then perturbed while stability was preserved, and replay was repeated.

| Post-drift map | Mean replay error |
|---|---:|
| frozen ERA | 0.03017 |
| refreshed ERA after new active identification | **0.00249** |
| frozen complex-pole rational | 0.04475 |
| rational recomputed from new operator | 0.03145 |

ERA re-identification reduced mean post-drift error by **91.7%** relative to the frozen ERA. Recomputing the rational candidate reduced its mean error by `29.7%` under the same terrain-drift family.

This supports **versioned effective maps + refresh**, not continuous retraining. The correct deployment object becomes:

```text
EffectiveInterface = {model, terrain_version, validity_window,
                      residual_monitor, refresh_contract}
```

The refresh operation in this synthetic bench assumes an active identification budget equivalent to roughly `100` probe steps and clean probe responses. Probe cost, safe excitation amplitude, and noisy identification remain open.

##### MB-SF-03F — Residual trigger candidate sieve

Because refresh itself has cost, the trigger was split into three candidates and tested on `42` new system instances with separate drift and no-drift episodes.

| Trigger | Detection rate | False-trigger rate | Mean delay (steps) | Status |
|---|---:|---:|---:|---|
| simple high threshold | 0.643 | 0.071 | 115.1 | `FAIL_AS_DEFAULT` |
| persistent residual | **0.833** | 0.095 | 94.5 | `PASS_BALANCED` |
| dual relative+absolute residual | 0.667 | **0.000** | 90.6 | `PASS_CONSERVATIVE` |

The persistent candidate requires residual excess to survive multiple consecutive windows. Under the declared utility weighting it was the best balanced candidate. The dual candidate requires both relative and absolute residual evidence; it generated **zero false triggers** in this synthetic sample but missed more drifts.

This creates a governance-dependent choice rather than one universal trigger:

```text
Refresh is cheap / missed drift costly
  -> persistent trigger candidate

Refresh is expensive / false intervention costly
  -> dual conservative trigger candidate
```

The trigger itself should therefore be selected from the same expected-loss machinery used elsewhere in GRT:

```text
L_refresh
  = C_false_refresh * P(false trigger)
  + C_missed_drift * P(miss)
  + C_delay * E[detection delay]
  + C_probe
  + C_reidentification.
```

##### v1.21 selection architecture

```text
Dynamic effective interface needed
  |
  +-- operator inspectable?
  |     |
  |     +-- YES -> candidate complex-pole rational
  |     |           -> non-normality + replay gate
  |     |           -> if poor: richer rational / state-space branch
  |     |
  |     +-- NO  -> active boundary probe available?
  |                 |
  |                 +-- YES -> black-box ERA / SSID
  |                 +-- NO  -> passive/noisy SSID candidate [PENDING]
  |
  +-- deploy model with terrain version + residual monitor
        |
        +-- residual stable -> retain model
        +-- persistent/dual trigger -> active refresh if budget allows
        +-- refresh unavailable -> degrade authority / rollback / escalate
```

The architectural lesson is stronger than a single winner:

> **Coarse-graining and model maintenance are separate layers.** A good effective map still becomes stale; a good refresh policy cannot rescue a structurally inadequate model without enough identification information.

##### v1.21 queue update

| Candidate / bench | v1.21 state | Next action |
|---|---|---|
| `CF-SF-MEM-RAT-CPLX-01` | `MEDIUM_PASS_SCOPE_LIMITED` | add non-normality-gated selector and matched runtime-state realization |
| `CF-SF-MEM-SSID-ERA-01` | `MEDIUM_PASS_PROBE_ACCESS_SCOPE_LOCKED` | noisy/passive identification bench |
| `CF-SF-MEM-REFRESH-PERSIST-01` | `MEDIUM_PASS_SCOPE_LIMITED` | optimize trigger threshold against declared refresh loss |
| `CF-SF-MEM-REFRESH-DUAL-01` | `MEDIUM_PASS_CONSERVATIVE` | test under rarer but higher-cost drift |
| `CF-SF-HYBRID-GATE-01` | `MEDIUM_PENDING` | use measured non-normality/replay residual to route rational vs SSID |
| `CF-SF-MEM-SSID-NOISE-01` | `MEDIUM_PENDING` | active noisy probe vs passive SSID vs ARX hybrid |
| `MB-SF-04` nonlinear switching/saturation | `MEDIUM_PENDING` | no execution yet |
| `MB-SF-05` runtime/energy/probe-cost frontier | `MEDIUM_PENDING` | optimized implementation + operation/probe budget |
| recursive/multiplex real-agent Feshbach benches | `HEAVY_PENDING` | candidate only |

**Frozen artifacts:** `grt_v121_complexpole_blackbox_refresh_results.json`; `grt_v121_complexpole_blackbox_refresh_summary.json`; `grt_v121_refresh_trigger_sieve_results.json`; `run_grt_v121_complexpole_blackbox_refresh_bench.py`; `run_grt_v121_refresh_trigger_sieve.py`.


###### 4.12.28 Non-normality-Gated Rational ↔ ERA Selector Bench — v1.22

> **Status: MEDIUM BENCH — CONDITIONAL PASS WITH RESOURCE/OBJECT LOCKS.** This section tests whether the compact complex-pole rational interface from v1.21 can be used by default while routing only high-risk non-normal terrains to the more general black-box ERA realization. It does **not** claim that non-normality alone determines the optimal reducer, and it does not make ERA free: ERA consumes a larger interface-state budget and, in the present synthetic setup, active identification access.

##### Candidate split

The selector problem is distinct from both reducer fitting and refresh:

```text
Reducer family:
  R = compact operator-conditioned rational
  E = boundary-identified ERA state-space

Selector:
  S(terrain_risk, resource_contract)
    -> R or E

Refresh:
  decides when the selected model is stale
```

Four selector candidates were frozen:

| Candidate | Rule | Intended advantage | v1.22 result |
|---|---|---|---|
| `CF-SF-SEL-WA-THR-01` | ERA if numerical abscissa > fixed threshold | simple one-system gate | `MEDIUM_FAIL_RESOURCE_STABILITY` |
| `CF-SF-SEL-DEP-THR-01` | ERA if commutator-departure > fixed threshold | alternate non-normality proxy | `MEDIUM_SCOPE_LIMITED`; no clear advantage |
| `CF-SF-SEL-COMP-01` | learned score from numerical abscissa + commutator departure | richer risk estimate | `MEDIUM_NO_MATERIAL_GAIN` |
| `CF-SF-SEL-WA-RANK-01` | rank by numerical abscissa; send only top risk quota to ERA | exact resource-budget control | **`MEDIUM_PASS_SCOPE_LIMITED`** |

The gate is intentionally **risk-ranked rather than topology-labeled**. The generator labels `real_decay / oscillatory / nonnormal` are evaluation metadata, not inputs to the canonical selector.

##### Why the fixed threshold failed

The first candidate trained an absolute numerical-abscissa threshold under a nominal 40% ERA budget. Replay accuracy was good, but the risk distribution moved under terrain shift:

| Set | ERA fraction | Mean selector error | Always rational | Always ERA |
|---|---:|---:|---:|---:|
| train | 0.370 | 0.00312 | — | — |
| held-out | **0.519** | 0.00266 | 0.00786 | 0.00247 |
| shifted terrain | **0.593** | 0.00369 | 0.02228 | 0.00297 |

Therefore an absolute gate can be an accuracy gate but not a reliable resource contract. A terrain shift that raises non-normality can silently cause the expensive branch to absorb most of the population.

This is a general orchestration lesson:

```text
fixed risk threshold
  !=
fixed compute / probe / state budget
```

##### Budget-controlled rank selector

The replacement policy imposes the expensive-model quota directly:

```text
For a current eligible population P:
  1. compute risk score omega_i
  2. rank agents/patches by omega_i
  3. allocate ERA to top q fraction
  4. allocate compact rational to the remainder
```

For the present white-box linear candidate,

\[
\omega_i
= \lambda_{\max}\!\left(\frac{A_i+A_i^\top}{2}\right)
\]

is the numerical abscissa. This quantity is a **candidate transient-risk score**, not a universal governance variable.

At a nominal `q=0.40`, finite batches of `27` selected `10/27 = 0.370` ERA interfaces. Initial held-out results were:

| Policy | Held-out mean error | Shifted mean error | ERA fraction |
|---|---:|---:|---:|
| always rational | 0.00786 | 0.02228 | 0.000 |
| always ERA | 0.00247 | 0.00297 | 1.000 |
| regime-label reference | 0.00300 | 0.00439 | 0.333 |
| **numerical-abscissa rank gate** | **0.00293** | **0.00449** | **0.370** |

The rank gate sacrificed some accuracy relative to always-ERA but removed roughly 63% of ERA activations while eliminating most of the catastrophic rational tail under strong non-normality.

##### Risk-score audit

Material ERA benefit was defined independently as

\[
E_R-E_E > 0.005,
\]

where `E_R` and `E_E` are mean replay errors across ID, fast-OOD, chirp, and impulse forcing. Discrimination AUCs were:

| Risk score | Train | Held-out | Shifted |
|---|---:|---:|---:|
| numerical abscissa | 0.707 | **0.829** | **0.868** |
| commutator departure | 0.714 | 0.821 | **0.879** |
| spectral abscissa | 0.843 | 0.614 | 0.819 |

The two-feature logistic score did not materially improve the quota-controlled selector over numerical-abscissa ranking in the tested sets. GRT therefore preserves the **simpler score** and keeps richer gates as candidates rather than rewarding complexity without held-out gain.

##### Fresh-seed confirmation lock

Because the first rank result and its acceptance interpretation were developed together, a separate confirmation run was executed on completely fresh seeds after freezing the following gates:

```text
C1: ERA fraction <= 0.40
C2: mean error <= always-ERA mean + 0.002 absolute
C3: >= 50% mean-error reduction vs always-rational
C4: p95 replay error <= 0.015
C5: >= 10% selected interface-dimension reduction vs always ERA
```

Results:

| Confirmation set | Rank-gate mean | Rational mean | ERA mean | Error reduction vs rational | Excess vs ERA | Interface-dim reduction vs ERA |
|---|---:|---:|---:|---:|---:|---:|
| fresh ID | **0.00250** | 0.00706 | 0.00119 | **64.6%** | 0.00130 | **21.3%** |
| fresh shifted terrain | **0.00542** | 0.01528 | 0.00418 | **64.5%** | 0.00123 | **21.5%** |

The corresponding p95 errors were `0.00610` and `0.00583`, and ERA usage remained `0.370` in both finite batches. **All five predeclared confirmation gates passed on both sets.**

Hence:

```text
CF-SF-SEL-WA-RANK-01
  -> MEDIUM_PASS_SCOPE_LIMITED
```

The pass is deliberately narrow: it establishes a synthetic resource/accuracy frontier for the declared linear system family, not a universal non-normality theorem for multi-agent systems.

##### Canonical hybrid policy after v1.22

```text
Dynamic interface request
  |
  +-- compact rational admissible and operator visible?
  |       |
  |       +-- NO -> ERA / SSID branch if identification access exists
  |       |
  |       +-- YES -> estimate transient non-normality risk
  |                   |
  |                   +-- rank within current resource pool
  |                   +-- top risk quota -> ERA
  |                   +-- remaining quota -> rational
  |
  +-- replay / residual monitor
          |
          +-- valid -> retain selected reducer
          +-- stale -> refresh policy from v1.21
```

This upgrades the orchestrator from choosing a **model family** to allocating a **portfolio of effective-model families under a hard resource envelope**.

##### Scope and failure locks

1. **White-box risk lock.** Current numerical abscissa uses the declared full linear operator. If only boundary observations are available, this gate cannot be computed directly.
2. **Population-reference lock.** Percentile/rank allocation requires a batch, population, rolling reference window, or stored calibration distribution. A single isolated system has no endogenous percentile.
3. **Budget is not accuracy.** Tightening the ERA quota reduces cost but increases error; no quota is a universal constant.
4. **Risk score is not causal completeness.** Non-normality explains a major rational failure mode in the current bench but does not exhaust oscillatory, nonlinear, delayed, adversarial, or identification-noise failures.
5. **ERA access cost remains external.** Active probe cost and safe excitation constraints are not included in the interface-state count.
6. **No cross-multiplex transfer.** A selector calibrated on an information/linear-response operator does not automatically select reducers for authority, recovery, contamination, or audit graphs.

##### v1.22 queue update

| Candidate / bench | v1.22 state | Next action |
|---|---|---|
| `CF-SF-SEL-WA-THR-01` | `MEDIUM_FAIL_RESOURCE_STABILITY` | retain as negative result; threshold may still be useful when resource budget is soft |
| `CF-SF-SEL-WA-RANK-01` | **`MEDIUM_PASS_SCOPE_LIMITED`** | test boundary-observable risk proxies and rolling quota calibration |
| `CF-SF-SEL-COMP-01` | `MEDIUM_NO_MATERIAL_GAIN` | do not promote until richer features beat simple ranking on fresh held-out data |
| `CF-SF-SEL-BBPROXY-01` | `MEDIUM_PENDING` | infer transient-risk rank from boundary impulse/residual data only |
| `CF-SF-SEL-ROLLQ-01` | `MEDIUM_PENDING` | rolling-quantile gate under changing population composition |
| `CF-SF-MEM-SSID-NOISE-01` | `MEDIUM_PENDING` | noisy/passive SSID benchmark |
| `MB-SF-05` runtime/probe/energy frontier | `MEDIUM_PENDING` | include identification and refresh cost, not state count alone |
| nonlinear switching / recursive / multiplex closure | `MEDIUM/HEAVY_PENDING` | no promotion from current linear bench |

**Frozen artifacts:** `grt_v122_nonnormality_gated_selector_results.json`; `grt_v122_nonnormality_gated_selector_summary.json`; `grt_v122_nonnormality_rank_confirmation_results.json`; `run_grt_v122_nonnormality_gated_selector.py`; `run_grt_v122_nonnormality_rank_confirmation.py`.

#### 5. Input–Output Contract

##### 5.1 Lower-to-Middle Input

A lower agent submits a **committed scoped differential**, not its unconsolidated live internal state:

```text
Delta_i_up = {
  new_observations,
  changed_relations,
  successful_and_failed_paths,
  boundary_changes,
  uncertainty,
  provenance,
  exclusions,
  recovery_information
}
```

The submission declares what was observed, under which conditions, what was not observed, and which parts remain inferred.

##### 5.2 Middle-to-Upper Output

The middle layer sends only the information that survives local handling and compression:

- unresolved cross-domain conflicts;
- repeated rule failure patterns;
- evidence that a Global Rule or Meta²-rule may be stale;
- aggregate escalation and recovery trends;
- distributional anomalies;
- clean-anchor disagreement;
- authority redesign requests.

##### 5.3 Middle-to-Lower Output

The middle layer sends a **role-projected patch**, not a global overwrite. It may contain:

- relevant global boundary constraints;
- cross-local relations;
- routing changes;
- recovery procedures;
- identified coverage gaps;
- complementary discoveries from other domains;
- explicit uncertainty and rollback conditions.

The receiver retains the right and obligation to return `ACCEPT`, `CONDITIONAL`, `CONFLICT`, `OUT_OF_SCOPE`, `UNSAFE`, or `UNRESOLVED` within its evidence role. This is not constitutional veto power; it is local validation evidence.

#### 6. Mutual Terrain Reconciliation Protocol

```text
1. Local independent processing
2. Commit scoped evidence / rule patch
3. Mediator schema, provenance, authority, and integrity checks
4. Global fusion without forced consensus
5. Role-projected downward patch
6. Replay / sandbox / shadow / bounded deployment
7. Local teach-back, action test, and recovery test
8. Residual return
9. Global / meta-rule revision if warranted
10. Staged assimilation, monitoring, rollback, or supersession
```

The loop is bidirectional but not symmetric:

- local layers contribute freshness and depth;
- global layers contribute breadth, cross-scope relations, and constitutional constraints;
- middle layers provide translation, comparison, routing, and reversible assimilation.

#### 7. Processing Isolation and Multiplex Separation

Same-layer agents must not exchange classification-relevant intermediate states by default. Permitted signaling transmits completed outputs, confidence, scope, and limit-state reports. Prohibited influence directly bends another agent's active classification before independent processing completes.

The following paths are distinct and need not share the same topology or authority:

- task execution;
- evidence submission;
- rule-patch distribution;
- escalation;
- clean-anchor access;
- audit and rollback;
- quarantine and recovery;
- memory storage.

A task coordinator may lack authority to rewrite memory. A memory service may lack authority to decide interpretation. A local specialist may reject a patch on evidence grounds without having authority to change Global Rules.

#### 8. Translation-Loss Accounting

Middle-layer success cannot be measured only by final agreement. For each consequential transfer, the declared total loss should be decomposed into:

```text
L_total
  = L_projection
  + L_transport
  + L_fill
  + L_routing
  + L_synthesis
  + L_drift
  + L_interaction_residual
```

- `L_projection`: loss from reducing a broad map to a role-specific patch;
- `L_transport`: corruption or omission during transmission;
- `L_fill`: receiver bias used to reconstruct missing dimensions;
- `L_routing`: loss from wrong receiver, path, timing, or authority route;
- `L_synthesis`: loss from merging multiple local results;
- `L_drift`: environment or dependency change after validation;
- `L_interaction_residual`: non-additive loss created by the interaction of the above.

A translation failure must be assigned to the correct loss class before the rule or agent is blamed.

#### 9. Rule-Patch Lifecycle State Machine

Canonical candidate states:

| State | Meaning |
|---|---|
| `LOCAL` | observed or proposed within one scoped domain |
| `CANDIDATE` | proposed for broader use; schema complete; not independently verified |
| `VERIFIED` | passed declared evidence, external-reference, action, and recovery tests |
| `CONFLICT` | incompatible validated observations remain unresolved |
| `UNKNOWN` | evidence or coverage is insufficient |
| `STALE` | freshness, dependency, or terrain assumptions expired |
| `QUARANTINED` | credible contamination suspicion or unsafe action impact |
| `REVOKED` | invalidated for active use; lineage and rollback record retained |

Forbidden transitions:

- no direct `LOCAL → VERIFIED`;
- no direct `QUARANTINED → VERIFIED`;
- no `CONFLICT → VERIFIED` without recorded resolution;
- no silent deletion; invalidated patches are superseded or revoked with lineage preserved.

**Hysteresis lock:** promotion is slow and multi-gate; demotion to `CONFLICT`, `STALE`, or `QUARANTINED` may be fast on one credible signal. Fast quarantine must still have a declared appeal, re-audit, and rate-limit path.

#### 10. Clean-Map Certification Gates

A rule or shared map may be treated as certifiably clean only when all declared gates pass:

1. **Domain lock:** domain, users, scope, authority, cadence, and required resolution declared.
2. **Correction-core separation:** content is distinct from the process that selects references, authorizes updates, evaluates outcomes, and accepts rollback.
3. **Independent clean anchor:** at least one protected external evaluator, checkpoint, verifier, human authority, lineage log, or replacement implementation remains accessible.
4. **Reality–record–interpretation separation:** external event, observation record, inferred terrain, and policy remain distinct.
5. **Provenance graph:** common ancestry, shared data, prompt, mediator, and timestamp dependencies retained.
6. **Conflict preservation:** disagreement and unknown regions are not overwritten by majority consensus.
7. **Selective immutability:** evidence lineage is append-only or tamper-evident; interpretation remains revisable.
8. **Local plasticity / global integrity:** local maps update faster; high-integrity global commitments require stronger gates.
9. **Version and rollback:** every consequential update has a restoration or supersession route.
10. **External and action tests:** teach-back alone is insufficient where shared wrong frames are possible.

The middle layer may coordinate these gates but cannot be the sole source, evaluator, and certifier of the same patch.

#### 11. Middle-Layer Self-Drift and Audit

The middle layer is the primary locus of gradual governance drift because its classifications generate the logs used to recalibrate its own thresholds. It therefore cannot self-certify.

Mandatory safeguards:

- **Calibration Reflexivity:** treat threshold changes, classification bias, rejection patterns, and escalation anomalies as observable meta-data.
- **Cross-Scale Consistency:** compare local activity, detected conflicts, correction events, escalation, and external outcomes.
- **Delayed-Escalation Audit:** inspect source diversity, type distribution, timing, and correlation with recent calibration changes before upper action.
- **Independent Reconstruction:** diverse agents reconstruct the same compressed patch; disagreement localizes missing dimensions.
- **Known-Anomaly Injection:** periodically introduce bounded test cases to distinguish genuine stability from shared blindness.
- **Clean-Anchor Rotation:** monitor whether anchors have become dependent on the same lineage or mediator loop.
- **Rollback Drill:** verify that a contaminated or overgeneralized patch can actually be removed without destroying correction capacity.

Key failure signatures:

```text
Interpretation Capture:
  conflict volume stable
  + escalation falling
  + external instability rising
  → middle layer is absorbing what should escalate

Mediator Drift:
  classification distribution changes after threshold updates
  + source diversity narrows
  + disagreement falls without perturbation confirmation

Map Monoculture:
  agreement rises
  + independent evidence count falls
  + external concordance stagnates or declines
```

#### 12. Reconciliation Dynamics and Rate Limits

Instantly sharing everything is not the mature design. The middle layer must control update gain, delay, and dwell time.

Candidate operating constraints imported from RBIT MTRL dynamics:

```text
Round-trip loop gain:
  gamma_eff ~ gamma_global_fusion * gamma_local_assimilation * acceptance_rate

Oscillation warning:
  gamma_eff * tau_loop too large
  → sign-alternating residuals, repeated reclassification, patch chattering

Contamination amplification:
  A_c ~ gamma_global_fusion * gamma_local_assimilation * p_contamination_survival
  Required candidate condition: A_c < 1
```

Operational controls:

- asynchronous exchange;
- minimum evidence dwell before promotion;
- dead band for insignificant patch differences;
- progressive disclosure;
- per-domain and per-authority rate limits;
- sandbox before high-impact assimilation;
- automatic rollback on declared regression;
- no live unconsolidated state sharing by default.

These are candidate control conditions, not a proved universal stability theorem.

#### 13. Maturity, Withdrawal, and Rest Mode

The middle layer does not mature by disappearing. It transitions from visible actor to background structure.

Maturation sequence:

```text
Phase 0 — Direct mediation and maximum sensitivity
Phase 1 — Supervised local rule formation
Phase 2 — Feedback-only mediation and sampled validation
Phase 3 — Background contracts, audit, and exception routing
Rest Mode — local governance closes its own loop; middle layer remains dormant but observable and rollback-capable
```

Evidence of maturation includes:

- local correction events rising relative to storm escalations;
- upper workload `fesc` trending downward without external quality decline;
- validation residual magnitude decreasing;
- repeated rule patches accepted conditionally or locally resolved rather than globally overwritten;
- independent perturbation recovery remaining within bounds;
- conflict diversity remaining non-zero;
- rollback, quarantine, and dormant recovery paths remaining functional.

A silent middle layer is healthy only if active probing confirms that it **can** detect, mediate, and recover when needed.

#### 14. Failure Modes

| Failure | Mechanism | Observable consequence |
|---|---|---|
| Frame Lock | upper frame transmitted without contextual translation | local rejection, escalation flood, brittle compliance |
| Frame Capture | lower frame dominates mediation | upward contamination, short-horizon policy drift |
| Interpretation Capture | middle layer normalizes anomalies | calm dashboard with rising external instability |
| False Consensus | live lateral influence or correlated validators | disagreement collapse, shared blind spots |
| Middle-Layer Overreach | meta-rules prescribe local content | local SCC atrophy, permanent dependency |
| Bypass | upper and lower communicate without mediation contract | abstraction shock or raw-noise overload |
| Patch Oscillation | high gain / low dwell / no hysteresis | repeated promotion–demotion, rule churn |
| Map Monoculture | shared memory overwrites distinct local maps | coverage loss, observability collapse |
| Audit Capture | clean anchor shares contaminated lineage | false certification, irreversible spread |
| Scheduler Starvation | low-status domains never receive review capacity | hidden governance gaps and delayed cascades |

#### 15. Cross-Theory Ownership Boundary

```text
GRT owns:
  rule authority, lifecycle, promotion, suspension, retirement,
  Rest Mode and withdrawal conditions, governance redesign triggers

NAT owns:
  graph/topology, typed routing, mediation paths, processing isolation,
  escalation structure, relationship topology, multiplex separation

RBIT owns:
  resolution gap, receiver terrain, degradation/upscaling contracts,
  loss accounting, mutual map reconciliation, clean-map certification
```

GRT may reference NAT/RBIT interfaces but must not duplicate their full mathematical substrates or claim their candidate architectures as established universal optima.

#### 16. Validation Commitments

The middle-layer architecture remains candidate status until it is compared against simpler alternatives. Minimum benchmark families:

- monolithic upper-controller baseline;
- naive peer-to-peer sharing baseline;
- majority-vote consensus baseline;
- one-way global-to-local rule injection baseline;
- shared-memory latest-write-wins baseline;
- no-independent-anchor baseline.

Kill conditions include:

- no reduction in upper governance load after accounting for mediation cost;
- no improvement in external concordance or recovery;
- greater contamination amplification than simpler routing;
- conflict retention causing unbounded paralysis;
- independent anchors failing to remain independent;
- receiver-conditioned transfer adding cost without reducing translation loss;
- middle-layer intervention eroding local SCC.

---

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

Meta-Rules are **rules about how rules are made**. The upper/global layer authorizes the constitutional meta-rule envelope; the middle layer operationalizes, applies, monitors, and audits that envelope; local layers generate domain content through contact and testing. Neither the upper layer nor the middle layer should define local rule content by default. They define the structure, format, authority path, evidence requirements, update conditions, and rollback obligations that local rules must follow.

| Domain | Meta-Rule Content |
|---|---|
| Expression format | Rules must be expressed numerically |
| Symmetry requirement | Advantages and penalties must be structurally symmetric |
| Logging obligation | All rule changes must be logged |
| Update conditions | Rules may only change when conflict log threshold is exceeded |
| Conflict priority | Global rules always supersede local rules |
| Patch portability | Frame, scope, provenance, uncertainty, version, authority, and rollback must be declared |
| Conflict preservation | CONFLICT and UNKNOWN remain explicit states; no silent consensus conversion |
| Certification separation | The proposing/mediating layer cannot be the sole independent certifier |
| Promotion hysteresis | Broader activation is slow and multi-gate; quarantine/demotion may be fast but appealable |

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

**Escalation error asymmetry (updated to RBIT v3.0–v3.5):** Under-escalation remains the generally more catastrophic direction because treating High-Context input as locally resolvable under sustained negative resolution gap can initiate cascade failure. However, over-escalation is **not safe**: it creates queue saturation, delay, privacy exposure, authority distortion, denial-of-service opportunities, human/upper-layer overload, and Dependency Trap risk that can erode local SCC. The correct default is therefore risk-relative conservative routing under a declared expected-loss function and a non-compensatory safety floor—not unconditional escalation of every uncertain item.

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
| **Φ** | Regime scalar (FCN ODE) | ≥ 0 | Φ < 1: stable; Φ > 1: Storm regime; mechanistic resolution of S̃ |
| **B** | Branching capacity (FCN/EDT) | ≥ 1 | How many topologically separated interaction channels exist? |
| **n_eff** | Effective interaction density (FCN) | ≥ 0 | Post-branching density: n_eff = n/B |
| **Φ_contam** | Contamination flux (FCN) | ≥ 0 | Rate of instability leaking across scale boundaries |
| **R_i** | Self-purification capacity (FCN) | ≥ 0 | R_i = D·F·V·T — internal recovery rate of circle i |
| **Σ(t)** | Frame dispersion (FCN Cube) | ≥ 0 | How far apart local coordination frames have diverged |
| **W_{gh}** | Inter-cluster coupling (FCN Cube) | [0, 1] | Coupling between frames g and h, decays with distance |
| **ΔU** | Basin depth (FCN attractor) | ≥ 0 | Energy barrier height in governance potential landscape |
| **σ_basin** | Basin width (FCN attractor) | ≥ 0 | Geometric extent of governance state's catchment area |
| **κ_C** | Capacity-tracking risk (EDT) | ≥ 0 | τ_C/τ_E: is governance capacity keeping up with terrain drift? |
| **κ_L** | Lock-budget risk (EDT) | ≥ 0 | τ_L/τ_E: are rules hardening while environment deteriorates? |
| **κ*** | Hybrid risk index (EDT) | ≥ 0 | w_C·κ_C + w_L·κ_L: unified governance lag metric |
| **η_acc** | Curvature accumulation rate (EDT) | ≥ 0 | How fast does terrain learn from failures? |
| **γ_decay** | Curvature decay rate (EDT) | ≥ 0 | How fast does unused terrain curvature flatten? |
| **n_max** | Carrying capacity (EDT) | > 0 | Maximum sustainable rule/vector count per domain |

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

**Cube Domination Dynamics (FCN §7.5 Integration):**

FCN's Cube Domination theory extends niche differentiation from positional clarity of individual agents to **coordination frame competition** — the dynamics governing which shared reference frame dominates when the global coordination frame collapses:

```
Cube Domination (FCN §7.5):

  When global coordination collapses, the system doesn't simply
  fragment — it enters structured competition between local frames,
  each attempting to become the dominant reference.
  
  Definition: A regime in which the geometry of interaction —
  rather than any individual agent — constrains collective dynamics.
  A dominant frame R_{i*} emerges such that:
    Dim(Accessible space) < Dim(Unconstrained space)
    
  Unlike classical dominance (one agent outperforms on one metric),
  Cube Domination operates across multiple axes simultaneously —
  relational, temporal, and conditional — creating a multi-dimensional
  constraint volume (hence "cube").

Frame Competition State Variables:
  
  (A) Local Coordination Frame R_g(t):
    Each cluster g develops local interpretation rules and standards
    dR_g/dt = η_g(t) + Φ_g(selection pressure)
    
  (B) Frame Dispersion Σ(t) = Var(R₁, ..., R_K):
    How far apart reference frames have diverged
    Rising Σ = progressive loss of mutual intelligibility
    
  (C) Inter-Cluster Coupling:
    W_{gh}(t) = exp(−α|R_g − R_h|)
    Coupling decays exponentially with frame distance
    As Σ rises → mean coupling W̄ falls → fragmentation threshold W_frag
    
  GRT Mapping:
    R_g = domain-specific rule interpretation
    Σ = cross-domain rule consistency variance
    W_{gh} = cross-domain Lreinf coupling strength
    W_frag = fragmentation threshold = I < τu-2

Information-Theoretic Frame Selection:

  Frame selection is equivalent to finding the frame R_{i*} that
  minimizes total description length of system state:
    R_{i*} = argmin_i Σ_g D_KL(P_g ‖ P_i) + λ·H(R_i)
    
  = Minimum Description Length (MDL) competition:
  The winning frame is not the most accurate but the one requiring
  least re-encoding effort across all clusters.
  
  Principle: Translation > Quality
  The dominant rule framework is not the one that works best
  for any single domain, but the one most easily adopted
  across diverse domains.
  
  GRT implication for meta-rule design:
    Meta-rules should optimize for TRANSLATABILITY, not precision.
    A meta-rule that is 90% accurate but universally applicable
    dominates a meta-rule that is 99% accurate in one domain
    but requires costly translation to others.
    
    This is why Seeds (generative principles) outperform
    explicit rules (specific procedures): seeds have lower
    description length across diverse domains.

Frame Adoption with Collapse-Aversion:

  Selection probability (softmax over quality minus cost):
    P_{g→i} = exp(βQ_i − γC_{gi} − δR_i) / Σ_j exp(...)
    
    Q_i = frame quality score
    C_{gi} = translation cost for cluster g to adopt frame i
    R_i = collapse risk of frame i
    δ = collapse-aversion sensitivity
    
  The −δR_i term implements boundary-based governance:
    "Never choose a frame with collapse risk above threshold"
    rather than
    "Choose the best frame"
    
  Aversion Stagnation Threshold:
    If δ > δ_crit → no frame accumulates sufficient adoption
    → permanent fragmentation → "safe but static"
    
  GRT correspondence:
    δ too high → system refuses to settle on any rule framework
    → perpetual Active Mode without convergence toward Rest
    → over-cautious governance preventing organizational learning
    
    The viable governance corridor: 0 < δ < δ_crit
    = sufficient caution to avoid collapse
    + insufficient caution to prevent convergence

Vector Storm as Frame Selection Pressure (FCN §7.5):

  Storm creates selection pressure on competing frames:
    dQ_i/dt = a·S − b·S² − c_i
    
    a·S:   Storm exposes weak frames (selection benefit, linear)
    b·S²:  Excessive Storm destroys all frames (universal damage, quadratic)
    c_i:   Intrinsic structural vulnerability of frame i
    
  Optimal Storm Window:
    S* = a / 2b
    
    Below S_min: frame differentiation insufficient for selection
    Above S_max = a/b = 2S*: Storm destroys faster than it selects
    At S*: net selection pressure maximized
    
  GRT implication:
    This provides the formal justification for why storms are
    beneficial up to a point — they force frame selection that
    could not occur during stability.
    
    The "creative destruction" aspect of governance failures:
    Moderate rule framework disruption → forces re-evaluation
    → better framework emerges through competitive selection
    
    Excessive rule disruption → no framework survives
    → system cannot converge on any governance standard
    
    GRT's Storm management goal is maintaining S near S*:
    enough disruption to select better governance frameworks,
    not enough to destroy the selection process itself.
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

**Attractor Basin Geometry (FCN §11 Integration):**

FCN's attractor dynamics formalization provides GRT's energy barrier model with precise geometric structure — distinguishing basin depth from basin width and formalizing landscape evolution under learning:

```
Basin Geometry (FCN §11):

  Each governance state (Rest, Active, Collapse) corresponds to a
  local minimum of a governance potential U(x; θ):
    Basin(x*) = {x₀ ∈ state_space : trajectory from x₀ converges to x*}
    
  Two distinct geometric properties determine state persistence:
  
    Depth:  ΔU = U(x_saddle) − U(x*)
            = energy barrier to escape (= ΔF in GRT notation)
            Deep basin → hard to leave (exponential in ΔU)
            
    Width:  σ_basin = √(det(∇²U(x*))^{-1})
            = geometric extent of the basin
            Wide basin → robust to parameter uncertainty
    
  Four basin configurations and their governance meanings:
    
    Deep + Narrow = strongly attracting but FRAGILE
      Small parameter changes can eliminate the basin entirely
      GRT: a system deeply in Rest Mode but with narrow tolerance
      → one environmental shift can destroy the entire state
      
    Deep + Wide = strongly attracting and ROBUST
      Hard to escape AND tolerant of perturbation
      GRT: healthy mature Rest Mode with wide operating margins
      → this is the governance design target
      
    Shallow + Wide = weakly attracting but RESILIENT
      Easy to leave but always returning from a wide catchment area
      GRT: early Active Mode → system oscillates but doesn't collapse
      
    Shallow + Narrow = weakly attracting and FRAGILE
      Easy to leave AND small catchment → practically transient
      GRT: unstable Active Mode → system doesn't stay in any state
      
  Governance design implication:
    Landscape design should create DEEP + WIDE basins for Rest Mode
    and SHALLOW + NARROW basins for Collapse
    (easy to escape from Collapse, hard to fall into it)

Landscape Evolution Under Learning (FCN §11):

  The governance landscape itself evolves as the system learns:
    ∂U/∂t = −η_learn · ∇_θ L(x, θ) · ∂U/∂θ + η_decay · (U − U₀)
    
    First term: deepens basins near frequently visited states
      (= Hebbian learning → success reinforces the successful pattern)
    Second term: regularization toward default landscape U₀
      (= homeostatic decay → unused basins gradually flatten)
    
  PATHOLOGICAL CASE:
    When η_learn exceeds η_decay for dysfunctional basins:
      → landscape develops increasingly deep traps
      → the system learns to be stuck
      = the mathematical mechanism of SSS (Stability Saturation)
      
    Repeated success deepens the Rest Mode basin through learning
    while simultaneously eliminating alternative basins through decay.
    The result: Rest Mode becomes the ONLY basin → zero exploration
    → when environment shifts, there's nowhere else to go.
    
  This provides the dynamical mechanism for the SSS → SCM cascade:
    η_learn > η_decay sustained →
    Rest Mode basin deepens →
    Alternative basins decay →
    Exploration capacity vanishes →
    Environmental shift finds no alternative basin →
    System trapped in obsolete configuration →
    SCM (Self-Consistent Misalignment)

Kramers Escape Time with Pre-Exponential Factor (FCN §11):

  The full Kramers escape formula includes geometric detail:
    E[τ_escape] ≈ K · exp(ΔU / D)
    
    where K = (2π / ω_saddle) · √(det(∇²U(x*)) / |det(∇²U(x_saddle))|)
    
    ω_saddle = curvature of unstable direction at saddle
    = how often the system "attempts" to escape
    
  Multi-dimensional correction (FCN §11):
    E[τ_escape] ≈ K · exp(ΔU / D) · (D/ΔU)^{(d-1)/2}
    
    The polynomial prefactor means HIGH-DIMENSIONAL systems
    (many interacting agents) can escape attractors more readily
    than LOW-DIMENSIONAL ones (isolated agents).
    
  GRT implication:
    Multi-agent systems with high n (exploration dimensionality)
    have SHORTER escape times from pathological governance states
    than small systems — because the higher dimensionality provides
    more escape directions at the saddle point.
    
    This is why large organizations (high n) can sometimes
    restructure more easily than small teams (low n):
    the high dimensionality provides more pathways out of bad states.
    (Counterintuitive: bigger systems have MORE escape routes,
     not fewer — though they also have more ways to enter bad states.)

Stochastic Resonance Connection (FCN §11):

  When noise intensity D is structured (periodic or correlated):
    P_escape(D) = P₀ · exp(-ΔU/D) · [1 − exp(-T_window/τ_D)]
    
    First factor: increases with D (more energy to escape)
    Second factor: probability system remains coherent during escape
    
    Maximum escape probability at:
      D* ≈ ΔU / ln(T_window · ω_saddle)
      = the optimal Storm intensity
      
  This is the mathematical foundation for the Cube Domination
  optimal Storm window (FCN §7.5, S* = a/2b):
    Too little perturbation → cannot destabilize pathological states
    Too much perturbation → destroys alternative basins
    
  GRT correspondence:
    D* = the optimal governance perturbation level
    = how much controlled disruption is needed to enable transitions
    = the T_eff value at which governance transitions are most likely
      to succeed while maintaining structural coherence
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

**FCN Integration — Contamination Dynamics (FCN §32.8.1):**

FCN's Contamination Theory provides the formal mechanism for how governance failures propagate across scale boundaries. Contamination is not error per se — it is *error that crosses scale boundaries without being absorbed*:

```
Contamination Theory (FCN §32.8.1):

  Definition: Contamination occurs when instability generated at 
  scale L_i propagates to scale L_{i+1} without being absorbed.
  
  For each governance circle L_i, define:
    S_i(t) = internal instability (S-equation within circle i)
    R_i(t) = self-purification capacity (internal recovery rate)
    P_i(t) = boundary permeability (transmission rate to L_{i+1})
    
  Contamination Flux:
    Φ_contam(i) = P_i · max(0, S_i − R_i)
    
    S_i < R_i → self-purification succeeds → Φ_contam = 0
    S_i > R_i → unresolved instability → Φ_contam > 0
    
  Cascaded contamination (upper circle overwhelmed):
    Σ_j Φ_contam(j) > R_{i+1}
    = aggregate contamination from lower circles exceeds 
      upper circle's own purification capacity
      
  GRT Failure Case Reinterpretation via Contamination:
  
    Case 1 (Consistency Collapse):
      Multiple lower domains generate Φ_contam > 0 simultaneously
      → meta-rule layer overwhelmed → I collapses
      = contamination mode 1 (coupling contamination)
      
    Case 2 (Escalation Flood):
      Lower-layer permeability P_i too high
      → every local conflict escalates to upper layer
      → upper layer saturated → fesc explosion
      = contamination mode 3 (timescale leakage)
      
    Case 3 (Lreinf Collapse):
      R_i drops because reinforcement loops break
      → previously contained S_i now exceeds R_i
      → contamination begins propagating upward
      
    Case 4 (SCC Failure):
      R_i → 0 globally → ALL instability propagates
      → system-wide contamination cascade
      
    SCM (Self-Consistent Misalignment):
      Frame drift contamination: R_g(L_i) ≠ R_g(L_j)
      → different circles adopt divergent coordinate systems
      → translation layer failure
      → all metrics healthy within each circle
        but circles are answering different questions
      = contamination mode 2 (frame drift)
      
  Three Contamination Modes:
    Mode 1 — Coupling contamination: α_between ↑↑
      Lower circles' conflicts couple directly into upper dynamics
      Mechanism: insufficient buffering between layers
      GRT: fesc from lower domains overloading meta-rule processing
      
    Mode 2 — Frame drift: R_g(L_i) ≠ R_g(L_j)
      Different circles adopt divergent reference frames
      Mechanism: translation layer failure
      GRT: domains developing incompatible rule interpretations
      → I appears stable within each domain
      → cross-domain I collapses
      
    Mode 3 — Timescale leakage: τ_fast → τ_slow direct coupling
      Fast-loop oscillations penetrate slow-loop dynamics
      Mechanism: breakdown of timescale separation
      GRT: domain-level θd oscillations affecting system-level
      calibration directly (bypassing the buffer)
      
  Contamination always originates at the bottom:
    Bottom layer has highest n (most conflict channels)
    Bottom layer has fastest τ (errors amplify quickly)
    Bottom layer has highest variance (most noise generation)
    
  First visible symptom: unnecessary friction at execution level
  — friction that does not lead to learning or adaptation
  
  GRT detection protocol:
    Monitor fesc DISTRIBUTION, not just fesc count.
    If fesc events cluster in lower domains with upward propagation
    pattern (lower fesc → upper fesc with time lag):
    → contamination active
    → intervene at source (lower layer), not symptom (upper layer)
```

**FCN Integration — Self-Purification Capacity Decomposition (FCN §32.8.1):**

FCN decomposes the self-purification capacity R_i into four multiplicative factors, providing GRT with a deeper structural understanding of SCC:

```
Self-Purification Decomposition:

  R_i = D_i · F_i · V_i · T_i
  
  (A) Decoupling Strength D_i:
    Degree to which circle's internal dynamics are isolated
    from external perturbation.
    D_i ∝ 1/α_external
    
    GRT mapping: subsidiarity enforcement strength
    High D = local rules handle local conflicts independently
    Low D = every local fluctuation propagates externally
    
  (B) Feedback Density F_i:
    Frequency and quality of internal error-detection loops.
    F_i ∝ error_detection_frequency × correction_accuracy
    
    GRT mapping: θd calibration quality × conflict log completeness
    High F = errors detected and logged promptly
    Low F = contamination accumulates silently (Silent Criticality)
    
  (C) Variance Absorption V_i:
    Internal diversity — multiple interpretive frames,
    response modes, or solution pathways.
    V_i ∝ internal_diversity (= Dint)
    
    GRT mapping: position clarity + adjacent vector diversity
    High V = perturbations absorbed by alternative pathways
    Low V = no buffer for contamination (d → 0 in ODE)
    
  (D) Time Buffering T_i:
    Grace period available before consequences cascade.
    T_i ∝ τ_buffer
    
    GRT mapping: evaluation window W margin
    High T = slow correction mechanisms have time to operate
    Low T = every error demands immediate response
    
  CRITICAL: R_i is MULTIPLICATIVE, not additive.
    If ANY component → 0, R_i → 0 regardless of others.
    
    Perfect decoupling but zero feedback = zero purification
    Perfect feedback but zero diversity = zero absorption
    Perfect diversity but zero time = zero processing
    Perfect time but zero decoupling = zero isolation
    
    This explains why SCC failure (Case 4) can occur even when
    individual components seem adequate: the multiplicative
    structure means weakness in ONE dimension destroys the
    entire purification capacity.
    
  GRT SCC ↔ FCN R_i correspondence:
    SCC = f(Dint, Lreinf) [existing GRT definition]
    R_i = D · F · V · T   [FCN decomposition]
    
    Mapping:
      Dint → V (variance absorption)
      Lreinf → D × F (decoupling × feedback density)
        Strong Lreinf provides both isolation (D) through
        mutual support and detection (F) through contrast
      W margin → T (time buffering)
    
    The FCN decomposition reveals a previously implicit component:
    T (time buffering) is not captured by Dint or Lreinf alone.
    A system can have perfect diversity and strong loops but
    if evaluation windows are too short (T → 0), recovery cannot
    complete before the next perturbation arrives.
    
    New GRT recommendation:
      SCC should be evaluated as SCC = f(Dint, Lreinf, W_margin)
      where W_margin = remaining evaluation window after conflict
      processing completes (= time available for correction to take
      effect before next measurement cycle)

The Immunity Paradox (FCN §32.8.1):

  Self-purification capacity requires ongoing exercise:
    dR_i/dt = λ_learn · min(S_i, R_i) − λ_decay · R_i
    
    When S_i = 0: dR_i/dt = −λ_decay · R_i → R_i → 0 exponentially
    When 0 < S_i < R_i: R_i stabilizes at R* > 0
    
  "100% cleanliness destroys the immune system."
  
  Mature circles maintain small positive contamination level
  (0 < S_i ≪ R_i) as operational necessity —
  not tolerance of error but cultivation of recovery capacity.
  
  GRT correspondence:
    This IS the formal basis for the Self-Exciting Defect Layer
    and the AGM's controlled stochastic freedom:
    
    Self-Exciting Defect Layer = small S_i maintained deliberately
    AGM T_eff > T_min = noise that keeps S_i above zero
    Controlled perturbation injection = preventing R_i decay
    
    The Immunity Paradox, Self-Exciting Defect Layer (VST),
    and Minimum Viable Temperature (AGM) are THREE DESCRIPTIONS
    of the SAME structural necessity:
      adaptive systems must maintain endogenous perturbation
      to preserve their capacity to handle exogenous perturbation.
```

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
- **Phase 3 — Delegation propagation:** repeatedly validated lower compositions become default modules → middle-layer routing becomes cheaper and more automatic → upper direct execution falls while wake-up authority and OOD escape paths remain available

**Computational interpretation:** Rest Mode does not require the upper model to disappear. It means the upper layer is no longer the default execution path. The mature upper layer spends most of its capacity on sparse structural decisions — criteria, resource envelopes, unresolved conflicts, novelty, and redesign — while routine work is absorbed by validated lower compositions.

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

**Prediction 14 — Circular closure predicts Rest Mode stability duration:**

Domains that achieve complete feedback loop closure (output feeds back to input without external coordination reference) should maintain Rest Mode significantly longer than domains with open-chain governance dependencies. Rest Mode duration should correlate with the ratio of internal feedback density to external dependency count.

*Falsification condition:* If Rest Mode duration shows no correlation with internal feedback loop completeness, or if open-chain domains maintain Rest Mode as reliably as closed-loop domains, the circular closure model adds no predictive power.

**Prediction 15 — Contamination flux propagates bottom-up with measurable lag:**

Cross-scale governance failures should originate at lower levels (higher n, faster timescale) and propagate upward with a measurable time lag proportional to the inter-layer buffer capacity. The contamination flux Φ_contam = P·max(0, S−R) should be estimable from the temporal pattern of escalation events — lower-domain fesc should precede upper-domain fesc by at least one evaluation window.

*Falsification condition:* If governance failures show no preferential bottom-up propagation, or if upper-layer failures precede lower-layer failures as frequently as the reverse, the contamination directionality prediction fails.

**Prediction 16 — Self-purification R_i multiplicative structure produces identifiable vulnerability signatures:**

Systems with one R_i component near zero (D, F, V, or T) should exhibit a qualitatively distinct failure pattern compared to systems with all components moderately low. Specifically, zero-D failures (decoupling failure) should show rapid external propagation; zero-F failures (feedback failure) should show silent accumulation; zero-V failures (variance failure) should show brittle response; zero-T failures (time buffer failure) should show cascading overreaction.

*Falsification condition:* If failure patterns do not cluster according to which R_i component is weakest, or if the multiplicative structure produces no better failure prediction than additive SCC measurement, the decomposition adds no diagnostic value.

**Prediction 17 — Risk Index κ* trajectory predicts governance state transitions:**

Systems with κ* Type II trajectory (oscillating around 1) that transition to Type III (κ* > 1 sustained) should enter Active Mode or Collapse within a bounded time window proportional to 1/(κ* − 1). The Type II → III transition should provide at least one evaluation window of early warning before governance metrics (I, fesc, SCC) show degradation.

*Falsification condition:* If κ* > 1 sustained does not predict subsequent governance degradation, or if κ* provides no lead time over standard GRT metrics, the risk index adds no early-warning value.

**Prediction 18 — Curvature ceiling violation produces governance dependency:**

Systems where meta-rule prescriptiveness exceeds domain self-governance strength (upper-layer curvature > lower-layer autonomous curvature) should exhibit permanent dependency signatures: inability to maintain Rest Mode without continuous upper-layer involvement, lower SCC than comparable systems with weaker meta-rules, and inability to develop novel local rules without meta-rule authorization.

*Falsification condition:* If systems with highly prescriptive meta-rules achieve Rest Mode and high SCC as reliably as systems with minimal meta-rules, the Curvature Ceiling Theorem has no governance predictive power.

**Prediction 19 — Anomalous friction reduction precedes governance failure:**

A sustained decrease in conflict rate (fesc → 0) without corresponding improvement in environment quality should precede governance failure (I decline, SCC decline) within a bounded time window. The friction reduction should be distinguishable from genuine conflict resolution by checking environmental change indicators: genuine resolution occurs alongside environmental improvement, while anomalous reduction occurs alongside environmental stagnation or deterioration.

*Falsification condition:* If fesc → 0 is equally likely to indicate genuine resolution as impending failure, or if no environmental indicator reliably distinguishes the two cases, the anomalous friction reduction signal has no diagnostic value.

**Prediction 20 — Learned orchestration reduces active resource cost at matched quality:**

Given a fixed heterogeneous pool of models/modules, an orchestration policy trained on outcome-linked resource logs should reduce average active compute, context, or latency per successful task relative to static routing or always-large-model baselines while maintaining declared quality and safety floors. The gain should come primarily from better conditional activation, not from lowering verification standards.

*Falsification condition:* If learned orchestration produces no resource reduction at matched quality/safety, or if apparent savings disappear after accounting for retries, escalations, and rollback, the resource-intelligence claim is unsupported.

**Prediction 21 — Upper direct work declines with governance maturity:**

Across successful maturation from supervised delegation toward Rest Mode, UDWR should trend downward while SCC, I, and task quality remain stable or improve. OOD and criterion-conflict events should temporarily reverse this trend by reactivating higher layers.

*Falsification condition:* If mature systems require the same or greater fraction of upper direct work than immature systems at matched workload and quality, the upper-layer role-migration claim is weakened.

**Prediction 22 — Orchestration history improves composition choice beyond model capability scores alone:**

A scheduler using task-conditioned success/failure trajectories, disagreement structure, topology history, and recovery cost should outperform a scheduler that chooses agents only by standalone benchmark capability. The largest advantage should appear in tasks requiring heterogeneous collaboration or asymmetric verification.

*Falsification condition:* If composition history adds no predictive value beyond individual model capability/cost scores, the Resource Intelligence Log is unnecessary as a distinct governance object.

**Prediction 23 — Small-model safety transfer is partial, not automatic:**

Failure and coordination patterns discovered in bounded small-model populations should transfer to larger-capability systems better than chance only for a subset of structural invariants; capability-dependent strategies should generate measurable transfer gaps. Staged cross-scale validation should therefore outperform direct promotion of small-model conclusions.

*Falsification condition:* If small-model results transfer uniformly without capability-dependent gaps, the cross-scale lock is unnecessarily conservative. If they transfer no better than chance even after structural matching, the experimental-population protocol has little predictive value for larger systems.

**Prediction 24 — Energy-aware orchestration reduces Joules per successful task at matched quality and safety:**

Compared with static routing, always-large-model execution, and compute-only learned routing, a scheduler using outcome-linked energy telemetry should reduce `JST` and increase `UER` while preserving the same declared task-quality, safety, SCC, and recovery thresholds. Savings should remain after including verification, retry, escalation, and recovery energy.

*Falsification condition:* If energy-aware routing does not reduce total energy per successful safe task after full lifecycle accounting, or if its apparent energy advantage depends on lower verification/safety performance, the Energy-Aware Orchestration Principle has no demonstrated operational advantage.

**Prediction 25 — Conditional energy escalation is Pareto-superior to always-small and always-large baselines on heterogeneous workloads:**

For workloads containing both routine and difficult/OOD tasks, an energy escalation ladder should occupy a better quality–risk–energy Pareto frontier than either always-small or always-large execution: small tiers should absorb routine work cheaply, while difficult/high-risk cases selectively activate larger tiers. The advantage should grow as workload heterogeneity increases and shrink on homogeneous workloads.

*Falsification condition:* If a fixed model tier matches or dominates the escalation ladder in total energy, quality, safety, and recovery across heterogeneous workloads, conditional activation adds unnecessary orchestration complexity.

**Prediction 26 — Bounded scale residual predicts successful cross-scale transfer:**

Small-model policies or governance compositions promoted through FMCI should succeed at the next scale at a rate negatively correlated with protected `SER_k`. Transfers with low boundary/authority/recovery/topology residuals should outperform transfers selected only by lower-scale task accuracy or energy efficiency.

*Falsification condition:* If protected scale residual has no predictive relationship with next-scale quality, safety, SCC, or recovery outcomes, the FMCI residual model adds no useful transfer information.

**Prediction 27 — Invariant-preserving transforms outperform naive replication/extrapolation:**

Across matched workloads, a scale transform that explicitly preserves boundary, authority, dependency, failure, recovery, uncertainty, and resource contracts should require fewer rollback events and less re-learning at scale `k+1` than direct agent replication, parameter-count scaling, or scalar metric extrapolation.

*Falsification condition:* If naive scaling matches or outperforms invariant-preserving transfer on rollback frequency, SCC, recovery time, and safety at comparable energy cost, the declared invariant bundle is unnecessarily complex or incorrectly chosen.

**Prediction 28 — Quasi-commutativity residual localizes non-portable governance rules:**

Rules or orchestration policies with low `R_comm` should remain behaviorally coherent under scale promotion more often than rules with high `R_comm`. High residual components should predict which relation class—authority, topology, recovery, or resource allocation—requires scale-specific redesign.

*Falsification condition:* If `R_comm` neither predicts transfer failure nor localizes the component requiring redesign, the diagram audit has no operational value beyond ordinary next-scale testing.

**Prediction 29 — Coordination energy creates a scale-dependent crossover point for small-agent compositions:**

For at least some workloads, increasing the number of small specialized agents should initially reduce Joules per successful safe task, then reach a crossover scale where communication and synchronization growth (`CGR`) erodes or reverses the local-compute advantage. Fractal partitioning or hierarchical compression should shift that crossover to a larger population size.

*Falsification condition:* If coordination energy remains negligible across increasing agent population sizes, or if hierarchical/fractal partitioning does not alter the energy crossover when communication structure is held comparable, the scale-aware energy law is unsupported for that workload class.

**Prediction 30 — Fractal Compatibility Gradient appears across mature heterogeneous layers:**

Across a mature hierarchy, upper maps should transfer across more domains with less local detail, while lower maps should achieve higher local-fit performance with lower direct portability. Measured cross-domain transferability should therefore increase with abstraction depth `ℓ`, while terrain-specific resolution and adaptation speed should generally decrease.

*Falsification condition:* If higher maps are no more portable than lower maps, or if lower terrain-specialized maps are equally portable without translation across heterogeneous domains, the proposed compatibility gradient has no explanatory value.

**Prediction 31 — Terrain-conditioned expansion outperforms direct upper-map copying:**

When heterogeneous local terrains receive the same upper invariant, local implementations produced through `E_down(G, Terrain_i)` should outperform direct cloning of a uniform upper implementation on matched safety/authority constraints, particularly under distribution shift.

*Falsification condition:* If direct uniform copying performs as well as or better than terrain-conditioned expansion across heterogeneous terrains without increasing residuals, the need for asymmetric downward variation is weakened.

**Prediction 32 — Compatibility-mediated cross-local transfer reduces negative transfer:**

Transferring a successful pattern from local domain `i` to distinct domain `j` through `X_up → compatibility representation → E_down` should produce fewer boundary, authority, recovery, and performance failures than direct `L_i → L_j` copying.

*Falsification condition:* If direct local-to-local copying matches or outperforms compatibility-mediated transfer across heterogeneous terrains, the compatibility-bridge claim is weakened.

**Prediction 33 — Mutual co-evolution reduces persistent scale and terrain residuals:**

Systems that update both the upper compatibility map and the transformation operators (`X_up`, `E_down`, `T`) from repeated independent local residuals should show declining protected residuals over successive deployment cycles relative to systems with a frozen upper map or one-way top-down adaptation.

*Falsification condition:* If bidirectional co-evolution does not reduce residuals or instead systematically increases instability compared with frozen-map controls, the Mutual Resonant Co-evolution claim is weakened.

**Prediction 34 — Adaptive middle routers outperform fixed routers under terrain drift:**

> **v1.16 evidence status: `CHEAP_PASS` (`CB-RTR-01`).** Internal synthetic drift gate supports the directional claim; medium testing remains required.

When task distributions, local vocabularies, model capabilities, or timescale relations drift, a versioned router/translator updated from translation residuals should preserve matched-quality routing and lower `TLoss` more effectively than a fixed routing table, without suppressing disagreement or increasing hidden recovery cost.

*Falsification condition:* If fixed routers match adaptive routers under sustained terrain drift at comparable compute, safety, feedback visibility, and recovery cost, router plasticity is not necessary for that regime.

**Prediction 35 — Multivariate bridge bundles outperform scalar-only scale transfer when structural channels are non-redundant:**

> **v1.16 evidence status: `CHEAP_PASS_SCOPE_LIMITED` (`CB-BRG-01`).** Random held-out mixtures improved, but unseen-topology transfer was mixed; cross-topology portability is not established.

On heterogeneous scale-transfer tasks, a bridge containing at least buffer/timescale/topology information plus protected governance contracts should outperform a scalar-only transfer model on held-out macrostate prediction, rollback prediction, or transfer safety whenever those channels carry independent information. Ablation should identify which variables are genuinely useful.

*Falsification condition:* If richer bridge bundles do not improve held-out prediction or governance outcomes over the best scalar representation after complexity penalties, the additional bridge variables should be removed for that substrate.

**Prediction 36 — Maturation-before-coupling reduces cascade and rework cost:**

> **v1.16 evidence status: `CHEAP_PASS` (`CB-MAT-01`).** Randomized two-module toy systems strongly favored maturation-first; broader nonlinear/heterogeneous testing remains pending.

Local variations that satisfy a maturation certificate before strong cross-local coupling should exhibit lower cascade probability, fewer rollback events, and lower recovery/retraining cost than otherwise matched systems coupled immediately after creation.

*Falsification condition:* If immediate coupling matches or outperforms maturation-gated coupling across stability, learning speed, energy, and recovery metrics, the proposed ordering is unnecessarily conservative.

**Prediction 37 — Residual Vitality distinguishes genuine compatibility from false quiet:**

> **v1.16 evidence status: `CHEAP_PASS` (`CB-RV-01`).** Independent hidden-mismatch labels show added value from probe/update vitality channels in low-residual cases.

Among systems with similarly low `R_scale`/`R_comm`, systems that retain boundary experimentation, bidirectional feedback, and independent disagreement paths should survive perturbation tests and terrain shift more reliably than systems whose low residual coincides with declining experiment and feedback rates.

*Falsification condition:* If residual-vitality channels provide no additional predictive value beyond residual magnitude alone, the False Compatibility distinction adds no operational value.

**Prediction 38 — Governance information bottlenecks produce an abstraction–detail trade-off:**

> **v1.16 evidence status: `CHEAP_PENDING` (`CB-IB-01`).** No benchmark is counted yet because a naive compression experiment would risk defining the target with the same map under test.

As lower-state complexity exceeds effective cross-layer channel capacity, upper representations should become more compressed and portable while losing local detail. Increasing channel capacity or adding effective middle-layer compression should delay the point at which protected invariant loss rises sharply.

*Falsification condition:* If upper-layer detail can scale with lower-state complexity without increased channel capacity, translation cost, latency, or invariant loss, the proposed information-bottleneck grounding is weakened.

**Prediction 39 — Ordered routing is a governance variable under lossy heterogeneous mediation:**

> **v1.17 evidence status: `CHEAP_PASS` (`CB-ORD-01`).** History-selected ordering reduced mean MSE by 5.9% relative to a fixed path in the frozen toy generator.

When mediation operators discard and reconstruct different dimensions, ordered paths should produce different downstream loss; route-history-aware policies should outperform fixed ordering where path statistics are transferable.

*Falsification condition:* no reproducible held-out order effect or no benefit from history-aware ordering under declared stationary conditions.

**Prediction 40 — Residual-error covariance predicts false consensus beyond marginal accuracy:**

> **v1.17 evidence status: `CHEAP_PASS` (`CB-MONO-01`).** With individual error held near 20%, fully shared errors raised majority error to 0.201 while agreement reached 1.0.

Matched-accuracy populations with higher residual-error covariance/shared ancestry should exhibit more confident wrong consensus under blind-spot shocks.

*Falsification condition:* covariance/ancestry adds no held-out predictive value once individual accuracy and task difficulty are controlled.

**Prediction 41 — Cross-module interface density has a deadline-constrained Pareto frontier:**

> **v1.17 evidence status: `CHEAP_PASS_SCOPE_LIMITED` (`CB-INT-01`).** The declared modular toy found a substantially sparser deadline-feasible interface than the densest tested graph.

The optimal interface should be workload/deadline-relative rather than maximally dense or maximally sparse once communication, synchronization, audit, recovery, and authority costs are counted.

*Falsification condition:* connectivity remains monotonically beneficial after full matched costs, or sparsity never yields a feasible cost reduction under any matched deadline.

**Prediction 42 — Scale promotion requires protected-vector safety, not aggregate residual alone:**

> **v1.17 evidence status: `CHEAP_PENDING` (`CB-SAFE-01`).** No pass is counted until outcome labels are generated independently of the safety-vector thresholds.

A protected-channel gate for boundary, authority, recovery, audit, and catastrophic failure should reject some configurations that appear acceptable under an aggregate residual but later fail safety outcomes.

*Falsification condition:* the protected-vector gate adds no held-out discrimination beyond a properly calibrated scalar gate under independent outcomes.


**Prediction 43 — Low-rank Schur approximations exhibit an error–cost frontier rather than a binary valid/invalid boundary:**

On declared large linear patches, a rank-constrained effective operator should beat boundary-only/diagonal baselines at matched interface cost, but the required rank should vary with the interior spectrum and coupling geometry. `CB-SF-01` provides `CHEAP_PASS_SCOPE_LIMITED`; runtime/energy benefit remains untested.

**Prediction 44 — Static Schur adequacy degrades when interior memory overlaps the observation/control timescale:**

When the forcing/control frequency approaches material interior modes, `L_eff(0)` should produce larger boundary-response residual than a frequency-conditioned effective operator. `CB-SF-03` gives a cheap synthetic scope signal; non-normal/delayed time-domain validation remains pending.

**Prediction 45 — State-conditioned effective operators outperform fixed Schur maps in nonlinear local terrain:**

For nonlinear patches with a stable operating point, a Jacobian-conditioned Schur map should predict small local interventions better than a fixed zero-state Schur map, provided the operating point remains inside the local validity region. `CB-SF-04` is `CHEAP_PASS_SCOPE_LIMITED`.

**Prediction 46 — Effective operators are terrain-conditioned and do not transfer by template averaging alone:**

A shared Schur-like template trained across heterogeneous patches should exhibit substantial held-out residual unless the bridge conditions on terrain/operator features sufficient to reconstruct the patch-specific effective map. The unconditioned shared-template candidate failed `CB-SF-05`; a terrain-conditioned meta-operator remains a new candidate.


**Prediction 47 — Gauge-compatible singular reductions are coordinate-invariant but compatibility-sensitive:**

For a declared singular interior operator, pseudoinverse and explicit-complement Schur reductions should agree when the coupling annihilates the nullspace; changing the complement basis should not change the effective boundary operator. If coupling leaks into the nullspace, the reduction should be rejected rather than repaired silently by ridge loading. `MB-SF-02` is `MEDIUM_PASS_SCOPE_LOCKED` for the compatible synthetic class.

**Prediction 48 — Directed steady-state Schur exactness does not imply transient adequacy:**

On stable nonsymmetric systems, the object-specific Schur reduction should preserve equilibrium boundary response while transient replay error can remain material or even exceed a simpler boundary-only model. `MB-SF-01` supports this separation.

**Prediction 49 — Non-normality metrics add predictive value for effective-operator adequacy beyond eigenvalue stability:**

Numerical abscissa or a comparable transient-amplification diagnostic should predict high static-reduction replay error better than spectral abscissa alone on held-out directed systems. In `MB-SF-01`, numerical-abscissa AUC was 0.875 versus 0.744 for spectral abscissa.

**Prediction 50 — Gated reduction can outperform a single fixed reduction policy:**

A selector that conditions the reduction family on independently calibrated transient-risk features should outperform always-Schur or always-boundary-only policies on heterogeneous directed workloads, provided selection cost is included. The v1.19 held-out selector improved mean error by 2.9% over the best fixed baseline; broader generators and cost accounting remain pending.


**Prediction 51 — Stable rational memory can recover dynamic boundary behavior that static Schur misses:**

For stable linear patches with material interior memory and an inspectable operator, a stability-audited rational/exponential memory realization should reduce held-out time-domain boundary replay error relative to zero-frequency static Schur across forcing classes. `MB-SF-03A` supports this within the tested real-decay, oscillatory, and non-normal generators.

**Prediction 52 — Dynamic-memory compression has a state/error frontier rather than a universal retained rank:**

At fixed boundary dimension, increasing the rational memory-state budget should generally reduce replay error but with terrain-dependent returns. The admissible rank should therefore be selected from a declared error/resource contract rather than copied across patches. `MB-SF-03B` produced a monotone mean frontier for `r=1..5` under the frozen generator.

**Prediction 53 — Black-box finite-memory learners exhibit stronger excitation-distribution dependence than operator-conditioned rational reductions:**

When trained only on bounded replay distributions, a learned finite-memory interface should show a larger ID-to-OOD error increase than an operator-conditioned stable rational reduction unless the training protocol explicitly covers the new excitation regime. In v1.20, learned ARX error rose from 0.0381 ID to 0.1016 fast-OOD and 0.1999 impulse, while the rational candidate remained near 0.0013–0.0014.

**Prediction 54 — Effective-memory maps require versioned refresh under terrain drift:**

Even an exact source-operator memory map should accumulate replay residual when the underlying interior operator changes. Refresh benefit should depend on model class and information access: operator-conditioned models can refit directly from an updated operator, whereas black-box learned maps require enough new excitation/replay evidence. The v1.20 mild-drift and refresh audits provide scope-limited support.

**Prediction 55 — Operator-norm fit alone does not determine governance-interface adequacy:**

Two effective-memory candidates with similar or even substantially different full kernel-norm error may have very different boundary replay error under the declared intervention distribution. Promotion should therefore use intervention-weighted replay residuals and protected-channel tests in addition to raw operator approximation metrics. v1.20 observed mean rational kernel-fit residual around 0.169 alongside mean boundary replay error around 0.00134.

### Candidate Benchmark Governance

Predictions and difficult formal extensions do not all receive the same experimental budget. Schur/Feshbach candidates in Predictions 43–55 additionally obey the §4.12.24 object/dynamic/behavioral locks. Before a new high-cost prediction is scheduled, it is routed through the Candidate-First Pipeline (§4.12.15–§4.12.20). In particular:

- a prediction may be `BENCHMARK_READY` only if its observables and independent reference are fixed;
- a cheap synthetic pass may justify a medium test but never a theorem-level label;
- a heavy test may remain `PENDING` without weakening the already-supported core;
- failure at any gate narrows scope or rejects the candidate and is retained as negative evidence;
- benchmark code and candidate status should be versioned together so later theory revisions cannot silently redefine a failed test into a pass.

### Quantitative Test Design Framework

The predictions above are qualitative directional claims. For empirical testing, each prediction must be converted to a quantitative hypothesis with specified effect size and sample size requirements:

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
    P20 (learned routing resource efficiency)
    P22 (orchestration history value)
    P24 (energy-aware Joules-per-success efficiency)
    
  Tier 2 (testable with moderate instrumentation):
    P1 (AND/OR asymmetry)
    P4 (withdrawal protocol re-entry frequency)
    P10 (concordance reliability)
    P21 (UDWR decline with maturity)
    P25 (conditional energy escalation Pareto test)
    
  Tier 3 (requires specialized experimental setup):
    P5 (Silent Criticality detection)
    P6 (energy barrier asymmetry)
    P7 (niche differentiation dynamics)
    P8 (vectorization kinetics)
    P23 (small-to-large cross-scale transfer)
```

### Relationship to VST Falsifiability

These GRT-specific predictions complement the VST-level falsifiability framework (VST Section 1.5.1). VST tests the dynamical claims (fractal propagation, scale-invariant amplification). GRT tests the governance claims (asymmetric entry/exit, cumulative measurement, withdrawal protocol effectiveness). Both must hold for the complete DFG framework to be supported.


**Prediction 56 — Complex-pole sufficiency is conditional on mode geometry:**

Allowing conjugate complex poles should reduce oscillatory-memory error at a fixed compact basis compared with purely real decay bases, but this advantage should disappear or reverse in strongly non-normal systems unless residue/transient geometry is also represented. v1.21 supports the scope split but does not yet execute a matched real-pole-vs-complex-pole state-budget ablation on identical systems.

**Prediction 57 — Boundary state-space identification can dominate pole-only compression under non-normality:**

With adequate boundary excitation, a learned latent state-space should predict non-normal boundary transients better than a small eigenpole-selected kernel basis because the learned realization fits the full input-output Hankel geometry rather than eigenvalues alone. `MB-SF-03D` supports this on the declared synthetic families.

**Prediction 58 — Effective-map staleness is detectable before total failure:**

A versioned effective interface should exhibit a persistent increase in held-out boundary residual after terrain drift before catastrophic rollout failure. `MB-SF-03F` supports detectable residual shift, while also showing the detection/false-trigger tradeoff.

**Prediction 59 — Refresh policy should depend on intervention cost:**

When false refresh is expensive, dual relative+absolute residual gating should be preferred; when missed drift is more expensive, persistent residual gating should dominate. This is a decision-theoretic candidate claim, not a universal threshold claim.

**Prediction 60 — Model choice and refresh choice are separable:**

The best effective-model family for a stationary terrain need not imply the best refresh policy under drift. Architectures that optimize these two decisions separately should outperform systems that bind one fixed refresh rule to one fixed reducer across heterogeneous terrains.


**Prediction 61 — A fixed non-normality threshold will not generally preserve a fixed expensive-model budget under terrain distribution shift:**

If reducer risk distributions move with terrain, an absolute non-normality threshold should cause the fraction of ERA/SSID selections to drift even when the intended compute budget is fixed. v1.22 supports this failure mode: a threshold trained near a 40% ERA budget rose above 50% ERA usage on held-out and shifted populations.

**Prediction 62 — Budget-controlled risk ranking can preserve most of ERA's robustness with substantially fewer ERA allocations:**

When compact rational error is concentrated in the high-non-normality tail, allocating ERA only to the top-risk quota should sharply reduce rational tail error while retaining a smaller mean interface-state budget than always-ERA. The fresh-seed v1.22 confirmation supports this within the declared linear families.

**Prediction 63 — Simpler non-normality scores should be preferred until richer gates show independent held-out gain:**

A multi-feature or learned selector should not be promoted merely because it is more expressive. If numerical abscissa ranking and a richer composite produce indistinguishable resource/error frontiers, the simpler selector should remain canonical. v1.22 found no material composite advantage.

**Prediction 64 — White-box non-normality gating should be replaceable only if a boundary-observable proxy preserves risk ordering:**

A black-box deployment gate must recover enough of the reducer-failure ordering from boundary responses, residuals, or safe probes to approximate the white-box ranking. Direct correlation with the full operator is insufficient; the candidate must preserve held-out allocation quality under the same quota.

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

### Differentiation from Existing Multiscale and Hierarchical Approaches

The FMCI/compatibility-gradient proposal overlaps with several established research traditions, but no single comparison class contains the full GRT claim. The relevant distinction is therefore **compositional** rather than a claim that hierarchy, fractals, meta-learning, or multiscale compression are individually novel.

| External approach | What it already provides | Where GRT/FMCI differs |
|---|---|---|
| **Fractal Company / fractal organization** (Warnecke, 1993) | Self-similarity, self-organization, dynamics, recursively organized autonomous units | GRT explicitly rejects identical self-copying as the canonical relation. Upper maps are compatibility-maximizing and low-resolution; lower maps are terrain-specialized high-resolution variations. The key object is a compatibility gradient plus bidirectional transformation, not organizational self-similarity alone. |
| **FeUdal / Hierarchical RL** (Vezhnevets et al., 2017; classical feudal RL lineage) | Different temporal resolutions; manager sets abstract goals, worker executes primitive actions; task decomposition | Primarily a control hierarchy. GRT treats the hierarchy as a co-evolving map system: local residuals can revise the upper compatibility map, and authority/risk/recovery/resource contracts are preserved as first-class objects. |
| **MAML / CAVIA meta-learning** (Finn et al., 2017; Zintgraf et al., 2019) | Shared cross-task structure plus fast task-specific adaptation; CAVIA explicitly separates shared parameters from task-specific context | Closest analogue to compatibility → specialization, but usually within a task-learning objective rather than a recursive governance hierarchy. GRT adds explicit upward invariant extraction, cross-local compatibility mediation, authority boundaries, recovery paths, and scale-residual learning. |
| **Personalized Federated Learning** | Global/common knowledge combined with heterogeneous local models under client-specific data | Similar global/local asymmetry, but GRT does not define the global object as a parameter average or common predictor. It is a relation/constraint compatibility map, and local discoveries are promoted only after invariant extraction and cross-terrain validation. |
| **Renormalization Group / coarse-graining** (Mehta & Schwab, 2014 as DL correspondence) | Iterative coarse-graining across scales; extraction of relevant features/operators | Strong analogue for upward compression. GRT requires a paired downward terrain-conditioned expansion, explicit residual return, and learned transformation updates; the preserved objects include authority, risk, recovery, provenance, and energy contracts rather than physical/statistical operators alone. |
| **DiffPool** (Ying et al., 2018) | End-to-end learned hierarchical graph coarsening through differentiable node-to-cluster assignment | Provides hierarchical representation learning, not a governance lifecycle. GRT's map bundle includes boundaries, authority, failure propagation, recovery, uncertainty, and energy; promotion may be blocked by any protected residual even if representation loss is small. |
| **MeGraph** (Dong et al., 2023) | Alternates local and hierarchical aggregation and uses bidirectional pathways across a multiscale graph hierarchy | Architecturally close to bidirectional multiscale information flow, but GRT assigns asymmetric semantics to the directions: upward = invariant extraction; downward = terrain-conditioned variation. It also treats disagreement, rollback, authority, and scale-transfer failure as governance objects rather than representation features. |

**The strongest claimed differentiation is the closed loop:**

```text
upper compatibility map
  ↓ terrain-conditioned expansion
heterogeneous local variations
  ↓ real terrain experience
local success / failure / exception residuals
  ↓ invariant extraction
compatibility-map revision
  ↓ scale-transform revision
new local variations
  ↺
```

Existing approaches often contain one or two arrows in this loop:

- hierarchical RL emphasizes `upper → lower`;
- meta-learning emphasizes `shared prior → local adaptation`;
- personalized federated learning emphasizes `global ↔ local parameter/knowledge exchange`;
- renormalization emphasizes `fine → coarse`;
- multiscale GNNs emphasize `fine ↔ coarse representation flow`;
- fractal organization emphasizes recursive autonomous structure.

GRT/FMCI's specific hypothesis is that a scalable AI-governance system requires **all** of the following simultaneously:

1. asymmetric compatibility/specificity gradients across governance resolution;
2. learned bidirectional transformation rather than direct copying;
3. local-to-local transfer through a compatibility bridge;
4. explicit scale residuals that train the transformation itself;
5. authority, risk, recovery, uncertainty/provenance, and energy maps traveling with capability maps;
6. mutual co-evolution in which upper maps remain revisable by independent lower evidence;
7. bounded promotion/rollback so portability is demonstrated rather than assumed.

This should be treated as a **research synthesis and falsifiable architectural hypothesis**, not as evidence that prior hierarchical or multiscale work is absent. The novelty claim, if any, lies in the governance-oriented composition and the measurable transfer conditions.

### What GRT does NOT claim

- GRT does not claim to replace existing alignment techniques (RLHF, Constitutional AI, reward shaping). It claims to add the lifecycle management layer that these techniques omit.
- GRT does not claim that its specific variable set (fesc, I, Lreinf, SCC) is the only possible operationalization. It claims that any viable governance system must track structurally equivalent quantities — the relationships are constrained, not the estimators.
- GRT does not claim exact fractal isomorphism or identical self-similarity across layers. v1.13 instead predicts an asymmetric compatibility gradient: portable relation invariants should survive translation while local implementations vary with terrain. Exact mechanism-level portability remains an empirical question tested through residual and promotion protocols.

### Relationship to Companion Theory

While compatible with layered governance architectures such as those analyzed in companion work (Three-Layer Governance), the present framework does not depend on any specific structural decomposition. GRT applies wherever rules evolve through conflict-driven processes — whether in hierarchical, flat, or hybrid governance structures. Conversely, TLG's intervention topology operates regardless of how rules are internally formalized.

**Non-commutativity of temporal and spatial axes.** Rule evolution dynamics (GRT's domain) and intervention topology (TLG's domain) interact but are analytically non-commutative: changing where intervention occurs alters how rules evolve, and changing how rules evolve alters where intervention is needed — but the two transformations do not produce the same result in either order. This non-commutativity is why separate formal treatment is required rather than a single unified model: collapsing one axis into the other loses the interaction effects that drive governance failure. Mediation-layer drift, for example, alters rule evolution trajectories without being reducible to rule dynamics alone, and rule over-convergence disrupts intervention routing without being reducible to topology alone.

### Structural Validation Without Simulation

GRT does not validate outcomes; it validates explanatory necessity. The claim is not that GRT predicts novel failure modes, but that independently observed lifecycle failures across unrelated domains require a rule lifecycle model to become mutually intelligible. Catastrophic forgetting (Li et al., 2024) is a rule representation problem. RLHF over-optimization (Gao et al., 2023) is a rule over-convergence problem. Agent drift (Rath, 2026) is a silent rule degradation problem. Without a lifecycle framework, these remain disconnected observations; with GRT, they become structurally related instances of specific lifecycle phase failures. GRT provides the minimal lifecycle model consistent with these independently observed failure invariants.

### Limitations

All metrics presented in this document are at the theory stage and have not been empirically validated in deployed systems. A deliberate design principle throughout GRT is that operational conclusions depend on structural properties (ordinal relationships, asymmetric entry/exit, lifecycle phase) rather than on specific parameter values. Threshold calibration (τ values) requires system-specific operational history and follows estimation procedures (bootstrapping protocol, adaptive refinement) rather than fixed constants. Severity weights require only ordinal separation (global > boundary > local); the canonical values (1, 2, 4) are illustrative, not privileged. The AND-entry / OR-exit asymmetry is structurally motivated but not proven optimal; alternative asymmetric schemes may perform comparably. Cross-theory connections to companion frameworks (VST, TLG) have not been empirically tested.

### Reproducibility Protocol

To facilitate empirical testing, the following protocol specifies what must be measured in any implementing system: (1) pairwise rule conflict events logged with frequency, severity level, and involved rule identifiers; (2) escalation events logged with source layer, target layer, and timestamp; (3) rule lifecycle events: creation, modification, and retirement, each with triggering λlog mass; (4) self-correction events: disturbance detected AND resolved without upper-layer intervention, logged with latency and completeness; (5) perturbation response: controlled disturbance injection at the lowest governance layer, measuring recovery probability within evaluation window W; (6) orchestration events: task signature, selected agent/module set, temporary interaction topology, active compute/context, authority budget, verification depth, result quality, disagreement, escalation, rollback, and recovery time; (7) FMCI transfer events: source `M_{k,ℓ}`, target terrain/scale contract, `X_up` extraction result, `E_down` projection, protected invariant residuals, scale residual, cross-local negative-transfer events, and whether the upper compatibility map or transform was revised. The first five support the original GRT metrics; the sixth tests learned orchestration and energy/resource intelligence; the seventh is required to test asymmetric fractal compatibility and mutual co-evolution.

### Empirical Path

Five empirical directions are most immediately accessible:

**(1)** Controlled multi-agent simulation comparing AND/OR withdrawal protocol against symmetric and binary alternatives, measuring false positive rate, re-entry frequency, and time-to-stable-operation.

**(2)** Single-agent diversity measurement via preference tuning diversity metrics (measuring Dint and Poverlap across fine-tuning epochs to detect over-convergence).

**(3)** Perturbation testing in production LLM systems to distinguish genuine stability from over-stability (Prediction 5).

**(4)** Cross-scale sandbox experiments comparing naive replication against FMCI-guided promotion, measuring protected scale residual, rollback frequency, SCC degradation, coordination-energy growth, and transfer success from small → meso → large populations.

**(4)** Static-router vs learned-orchestrator comparison using the same pool of heterogeneous small models, measuring matched-quality compute, latency, escalation rate, rollback rate, and cross-domain generalization.

**(5)** Small-model experimental populations with controlled variation in topology, resource budget, and authority, followed by staged transfer to larger models to measure which safety and coordination patterns survive scale changes.

---

## Production Implementation Guide

> *This section specifies how GRT's theoretical constructs map to concrete production system components. The goal is not to prescribe a specific technology stack but to define the structural requirements that any implementation must satisfy — leaving architecture choices to the implementer while constraining the governance-critical invariants.*

### Implementation Architecture Overview

> **v1.10 orchestration lock:** The implementation architecture below must instantiate the Rule Architecture section's Middle-Layer Governance Interface: dual maps, typed routing, processing isolation, rule-patch lifecycle, independent clean anchors, local validation, residual return, and rollback. A generic message broker or single LLM judge does not satisfy this interface by itself.


A GRT-compliant production system requires seven structural components, each corresponding to a core theoretical construct:

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

Component 6 — Orchestration & Compute–Energy–Risk Intelligence Layer
  Theoretical basis: Tempo/Resource Scheduling, Learned Orchestration,
  Energy-Aware Orchestration, Delegation Maturity, Governance Compilation
  Structural requirement: separate selection/allocation policy from the
  executors it schedules, and retain a full outcome-linked orchestration log
  
  Minimum viable implementation:
    - Capability registry: {model/module, specialty, cost, latency, ancestry,
                            authority ceiling, verification requirements}
    - Orchestration event schema: {task_signature, selected_agents, topology,
                                   compute/context budget, energy budget,
                                   energy_joules_or_proxy, peak_power_or_proxy,
                                   accelerator_time, authority budget, verification depth,
                                   quality, retry_energy, escalation_energy,
                                   rollback, recovery_time, recovery_energy}
    - Learned or adaptive routing policy with conservative fallback
    - Energy Escalation Ladder with per-tier entry/exit criteria
    - Energy telemetry/proxy calibration registry with provenance
    - Upper direct-work accounting (UDWR) and lower autonomous success rate
    - Composite-module registry with version, audit path, rollback, OOD escape
    - Cross-scale promotion gate for small-model experimental findings
  
  Production mapping:
    - Router/orchestrator service separated from specialist executors
    - Budget controller for compute, context, latency, physical/proxy energy, and authority
    - Device/accelerator telemetry integration where available
    - Shadow/sandbox population runner for bounded composition experiments
    - Offline policy evaluation before orchestration-policy promotion
    - Automatic de-compilation / fallback when OOD or disagreement rises

Component 7 — Fractal Map Compatibility Interface (FMCI)
  Theoretical basis: Cross-Scale Lock, Fractal Map Compatibility,
  Bounded Quasi-Commutativity, Scale Residual Learning
  Structural requirement: no small-scale result is promoted without an
  explicit scale contract, invariant audit, residual measurement, and rollback path

  Minimum viable implementation:
    - Scale-map registry: {scale_id, capability_map, topology_map, authority_map,
                           energy_map, risk_map, recovery_map, uncertainty_map,
                           time_map, provenance_version}
    - Scale-transform registry T_{k→k+1} with versioned assumptions and declared loss
    - Protected-invariant schema and per-component residual thresholds
    - R_scale and R_comm calculation with component-level decomposition
    - Small→meso→large promotion state machine with shadow/canary stages
    - Scale-aware energy accounting including communication and synchronization
    - Automatic hold / split / rollback when protected residuals exceed bounds
    - Residual-history training store for updating scale transforms
    - Versioned middle-router / translation-policy registry with declared translation loss
    - Fractal Compatibility Validation Suite runner: replica, closure, intervention, topology, and next-scale gates
    - Residual Vitality checks so low residual cannot certify compatibility when feedback/experimentation channels are silent
    - Maturation certificate for local variations before strong cross-local coupling

  Production mapping:
    - Dedicated scale-compatibility service or orchestration subservice
    - Shadow populations at each promotion scale
    - Hierarchical map compression with preserved provenance and uncertainty
    - Scale-residual dashboard linked to state machine and deployment controller
    - Promotion certificates binding map version, transform version, energy proxy,
      authority ceiling, recovery checkpoint, and audit result
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

Dashboard Panel 6 — Orchestration / Energy Health:
  - Upper Direct Work Ratio (UDWR)
  - Average active model/module count per task
  - Active compute and context per successful task
  - JST: physical/proxy energy per successful task
  - UER: useful-work energy ratio
  - EEO: escalation/retry/recovery energy overhead
  - Peak power / accelerator-time distribution by task class
  - Energy Escalation Ladder tier distribution and promotion rate
  - Routing fallback / escalation / rollback rates
  - Verification depth by risk class
  - Topology churn and repeated composition stability
  - Correlated-ancestry concentration in active teams
  - Composite-module OOD escape / de-compilation events

Dashboard Panel 7 — Fractal Scale Compatibility:
  - Current promotion scale and active T_{k→k+1} version
  - SER: protected scale-error residual by component
  - R_comm: quasi-commutativity residual by rule / policy class
  - STF: successful transfer fraction by scale pair
  - CGR: communication + synchronization energy ratio
  - SCC_scale and recovery-time growth across scale
  - New propagation channels discovered after promotion
  - Promotion holds / rollbacks / domain splits caused by residual breaches
  - Invariant confidence and stale-transform warnings
  - Translation loss and router-policy version drift
  - Boundary experiment rate and bidirectional feedback rate
  - Residual Vitality status: genuine compatibility vs candidate false compatibility
  - Local maturation certificates before cross-local coupling
  - Bridge-ablation results: which variables add held-out predictive value
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
  □ Scale-map bundle versioned for every promoted agent/team/system scale
  □ Communication and synchronization energy measurable or explicitly proxied

Governance Requirements:
  □ AND-entry conditions explicitly coded (all five required simultaneously)
  □ OR-exit conditions explicitly coded (any one sufficient)
  □ Phase transition backward paths defined and tested
  □ Collapse recovery procedure accessible from all governance states
  □ Alert hierarchy configured with appropriate routing
  □ Small→meso→large promotion gates explicitly coded
  □ Protected invariant thresholds block unsafe cross-scale promotion

Candidate-Research Requirements:
  □ Difficult formal claims carry candidate IDs and explicit evidence status
  □ CheapBench performed before medium/heavy allocation whenever a cheap discriminating test exists
  □ Independent reference/baseline frozen before candidate evaluation
  □ Heavy unexecuted experiments marked HEAVY_PENDING rather than implied validated
  □ Rejected/failed candidates retained in negative-result registry

Validation Requirements:
  □ Perturbation test protocol defined and scheduled
  □ SCM detection signals monitored (λlog rate, SR, RDE, NCR)
  □ Silent Criticality protocol active during extended Rest Mode
  □ F_RBIT cross-validation configured
  □ R-ρ-fesc Triple Concordance automated
  □ R_scale and R_comm measured before every authority-scale promotion
  □ Scale residual decomposition retained as training data
  □ Rollback checkpoint verified at every promoted scale
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
16. Mature orchestration minimizes active intelligence and physical/proxy energy **subject to** quality, safety, SCC, authority, and recovery constraints; low energy is not a governance success when achieved by weakening those floors
17. Physical energy accounting (`E_task`, JST, UER, EEO) is ontologically separate from the governance free-energy landscape (`F_gov`) unless an empirical bridge is independently demonstrated
18. Cross-scale validity is not inherited automatically: lower-scale results become portable only through an explicit, versioned scale transform with preserved structural invariants and bounded residuals
19. Fractal compatibility means relation preservation across resolution, not identical content or agent behavior at every scale; scale-specific emergence is expected and must appear as measured residual rather than hidden error
20. Energy efficiency is scale-conditional: local inference savings are not system-level savings unless communication, synchronization, verification, retry, and recovery costs remain inside the promoted scale contract

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
| Fractal map compatibility | Renormalization / multiscale modeling | Relation-preserving coarse-graining with explicit residual terms (structural analogy) |
| Scale residual learning | System identification / model discrepancy | Prediction error used to update cross-scale transfer models |
| Bounded quasi-commutativity audit | Category-theoretic diagram reasoning / numerical consistency checks | Path-dependent transforms accepted when diagram residual is bounded |

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
 │                                    │  Rule architecture → FCN ODE params│
 │                                    │                                    │
RBIT ─────────────────────────────── │ ──────────────────────────────── NAT
 │                                    │                                    │
 │ IMPORTS to GRT:                    │       AGM          FCN             │ IMPORTS to GRT:
 │  Δρ resolution gap routing         │        │            │             │  Processing isolation
 │  F_RBIT health vector              │  T_eff, s(t)   S̃→ODE decomp    │  θ operationalization
 │  Seed sufficiency tests            │  σ·ξ perturb   Circular Closure  │  Sphere topology bounds
 │  Channel capacity                  │  Flow-Rest     Contamination Φ   │  R-ρ concordance
 │  Error asymmetry principle         │  Freeze/Run    R_i=D·F·V·T      │  Coverage probability
 │                                    │  Momentum p    Cube Domination   │
 │                                    │  Weight dyn    Basin geometry     │
 │                                    │  No-Free-Lunch Terrain protocol  │
 │                                    │  Event dist    North Star arch   │
 │                                    │                S-equation levers │
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

The GRT-RBIT interface provides the resolution, transfer, reconciliation, and certifiability substrate for rule governance:

```text
RBIT → GRT (information and map substrate):

  Δρ resolution gap → receiver-relative routing:
    RBIT provides supply-demand resolution comparison
    GRT uses as one route variable alongside harm, authority,
    reversibility, privacy, delay, recovery, and queue cost
    Protocol: resolution sufficiency never implies authority sufficiency

  Mutual Incompleteness → authority–epistemic separation:
    RBIT provides broad/coarse global map vs narrow/deep local map
    GRT uses to prevent upper infallibility and lower-totalization
    Protocol: constitutional priority may suspend action,
              but contradictory evidence and scope remain preserved

  MTRL → bidirectional rule-patch reconciliation:
    RBIT provides local differential → global fusion → role projection
    → local validation → residual return
    GRT uses for Seed, rule, and meta-rule patch movement
    Protocol: no one-way teacher injection by default

  Receiver-conditioned transfer / PTRV → Seed readiness:
    RBIT provides low-risk probes, teach-back, external checks,
    progressive disclosure, rollback, and drift monitoring
    GRT uses before high-impact rule or Seed assimilation
    Protocol: sender-side simplification alone is not calibrated transfer

  Information-loss accounting → translation diagnosis:
    RBIT decomposes projection / transport / fill / routing /
    synthesis / drift / interaction losses
    GRT assigns failed rule transfer to the correct correction site

  Patch schema and lifecycle → rule lifecycle state machine:
    RBIT provides LOCAL / CANDIDATE / VERIFIED / CONFLICT / UNKNOWN /
    STALE / QUARANTINED / REVOKED with legal transitions
    GRT uses for rule and meta-rule governance
    Protocol: conflict and unknown are first-class states;
              promotion slow, demotion/quarantine fast but appealable

  Clean Map + clean anchor → purification certification:
    RBIT provides evidence/interpretation separation, provenance,
    independent anchors, selective immutability, rollback
    GRT uses to define auditable rule cleanliness
    Protocol: the mediator cannot be sole source, judge, and certifier

  MTRL gain/delay model → update-rate controls:
    RBIT provides oscillation and contamination-amplification candidates
    GRT uses for dwell, dead band, asynchronous exchange, and rate limits
    Protocol: share-everything-instantly is outside the safe default

  F_RBIT health vector → Rest Mode validation:
    RBIT provides multi-component health measurement
    GRT uses as one independent channel in concordance validation
    Protocol: no scalar or directional agreement alone certifies Rest Mode

GRT → RBIT (governance objects and labels):

  Rule-patch lifecycle → persistent terrain-update labels:
    GRT supplies authority, activation, suspension, retirement,
    appeal, and handover semantics for RBIT patches

  Conflict logs → patch and health inputs:
    GRT supplies structured rule pair, severity, domain, timestamp,
    source, scope, authority, outcome, and recovery data

  θd and λlog → operational calibration observables:
    GRT supplies classification sensitivity and accumulation dynamics
    RBIT evaluates whether these actually improve receiver-relative resolution

  Rest Mode / withdrawal → reconciliation workload target:
    GRT supplies maturity state and upper-intervention trajectory
    RBIT tests whether lower maps retain recovery and external-reference capacity
```

**Interface status lock:** RBIT v3.5 defines these as candidate architectures, measurement commitments, and falsification protocols. GRT adopts the interfaces, not a claim that they universally outperform simpler memory or transfer systems.

### GRT ↔ NAT Integration Protocol

The GRT-NAT interface provides the structural routing, mediation, isolation, and topology enforcement for the Middle-Layer Governance Interface:

```text
NAT → GRT (structural enforcement):

  ILMI terrain translation → middle-layer translation contract:
    NAT provides context- and receiver-relative conversion of
    upper invariants and lower operational signals
    GRT uses for Global → Meta/Local and Local → Governance translation
    Protocol: every consequential translation declares preserved constraints,
              uncertainty, expected loss, authority, and rollback need

  Decision Complex → independent conflict classification:
    NAT provides multiple reasoning paths, conflict score,
    and resolution-estimator disagreement
    GRT uses before rule conflict labeling and escalation
    Protocol: correlated agreement is discounted; disagreement is preserved

  Typed routing → jurisdiction selection:
    NAT provides semantic class, urgency, confidence, harm,
    required resolution, receiver capacity, and expected route loss
    GRT adds rule level, authority, reversibility, privacy, and recovery impact
    Protocol: no single threshold determines all routes

  Processing isolation → independent evidence generation:
    NAT separates completed signaling from live trajectory influence
    GRT uses to prevent false consensus before mediation
    Protocol: same-layer intermediate classification states are not
              shared by default; outputs are committed before comparison

  Relationship topology → priority scheduling:
    NAT provides conflict history, coverage stress, and pairwise relation map
    GRT uses to allocate recalibration, validation, and audit resources
    Protocol: low-risk boundary review before high-impact rule change

  Multiplex separation → authority safety:
    NAT separates task, information, authority, contamination,
    recovery, audit, memory, and rollback paths
    GRT uses to prevent a routing hub from becoming an unchecked rule sovereign

  Reciprocal memory interface → staged patch deployment:
    NAT provides evidence submission, conflict-buffered fusion,
    role projection, local validation, and residual return topology
    GRT uses for rule-patch and Seed handover

  Coverage / propagation diagnostics → timing constraints:
    NAT provides declared graph/process bounds and blind-spot diagnostics
    GRT uses to set observation and response windows
    Protocol: every spectral or path claim names its exact substrate;
              fast mixing may spread benefit or harm

GRT → NAT (governance semantics and authority):

  Rule levels → typed edge authority:
    GRT supplies Global / Meta / Local rule status, precedence,
    suspension, appeal, and redesign semantics

  Rule-patch states → routing permissions:
    GRT supplies LOCAL / CANDIDATE / VERIFIED / CONFLICT / UNKNOWN /
    STALE / QUARANTINED / REVOKED routing restrictions

  fesc and correction/storm ratio → mediation-load observables:
    GRT supplies domain and layer workload trends
    NAT tests whether the architecture reduces governance cost per capability

  Rest Mode → topology maintenance mode:
    GRT supplies withdrawal and re-entry conditions
    NAT retains dormant audit, rollback, clean-anchor, and recovery paths
```

**Interface status lock:** NAT's sphere/expander topology is a reference candidate, not a universal architecture. GRT imports the operational functions—typed routing, mediation, isolation, multiplex separation, and staged reconciliation—without requiring one graph for every deployment layer.

### GRT ↔ EDT Integration Protocol

The GRT-EDT interface provides the terrain architecture and cultivation dynamics for governance landscape:

```
EDT → GRT (terrain architecture):

  Three-Axis Architecture → landscape design decomposition:
    Axis 1 (Boundary) → Global Rules: forbidden zones, hard curvature
    Axis 2 (Gain) → Correction values: tempo control, energetic gradients  
    Axis 3 (Coupling) → Subsidiarity + position clarity: branching B, ρ(J) < 1
    Protocol: every GRT landscape intervention maps to one or more axes
    
  Curvature accumulation → governance history encoding:
    EDT provides: ∂U/∂t = η_acc · [I_failure − I_success] − γ_decay · U
    GRT uses: conflict log = curvature accumulation substrate
    Protocol: λlog accumulation = curvature deepening;
              W aging = curvature decay (γ_decay);
              rule consolidation = curvature information compression
    
  Curvature Ceiling Theorem → subsidiarity necessity:
    EDT provides: λ_max(H(U_top)) < λ_min(H(U_autonomous))
    GRT uses: meta-rule prescriptiveness must not exceed domain self-governance
    Protocol: measure local rule autonomy vs meta-rule constraint strength
    
  Curvature Withdrawal Schedule → Rest Mode maturation:
    EDT provides: upper curvature withdraws as lower self-curvature grows
    GRT uses: governance withdrawal is curvature withdrawal
    Protocol: as domain SCC grows, reduce meta-rule intervention frequency
    
  Friction theory → learning rate management:
    EDT provides: zero friction = zero learning; optimal friction band
    GRT uses: conflict rate as learning proxy
    Protocol: monitor conflict_rate vs SCC;
              conflict_rate → 0 → therapeutic disturbance needed;
              conflict_rate > SCC → traumatic overload → reduce exposure
    
  Risk Index κ → early warning system:
    EDT provides: κ* = timescale mismatch between terrain drift and adaptation
    GRT uses: κ* as governance lag detector
    Protocol: κ_C from θd recalibration speed / conflict rate change;
              κ_L from rule update frequency / environment change rate;
              κ* > 1 sustained → governance falling behind → preemptive action
    
  Terrain Resonance → timescale collision avoidance:
    EDT provides: resonance conditions between agent and terrain dynamics
    GRT uses: W and θd cycle must avoid resonance with conflict cycles
    Protocol: verify τ_agent ≪ τ_terrain OR τ_agent ≫ τ_terrain;
              if resonance detected → adjust W or θd update period
    
  Carrying Capacity → domain size bounds:
    EDT provides: n_max = f(terrain_quality, C, β)
    GRT uses: maximum rule/vector count per domain
    Protocol: monitor n_domain vs n_max(domain);
              approaching capacity → consolidate;
              exceeded → split domain into new circle
    
  Contamination Permeability → phase-gated exposure:
    EDT provides: P(phase) schedule (EDT §35.2)
    GRT uses: cross-domain exposure timing
    Protocol: Phase 1 (P≈0) → Phase 0 bootstrapping;
              Phase 2 (P=P_min) → Phase 1 baseline;
              Phase 3 (P=f(R)) → Phase 2 steady-state;
              Phase 4 (P adaptive) → Rest Mode

GRT → EDT (governance specification):

  Rule architecture → terrain structure specification:
    GRT provides: rules that define terrain boundaries and gradients
    EDT uses: rules as curvature injection mechanism
    Protocol: Global rules → hard boundary curvature;
              Local rules → soft gradient curvature;
              Meta-rules → curvature management rules;
              Seeds → curvature accumulation programs
    
  Failure case taxonomy → terrain failure classification:
    GRT provides: 5 failure cases + SCM
    EDT uses: terrain pathology diagnosis
    Protocol: Case 1 → curvature contradiction (competing barriers);
              Case 2 → curvature permeability failure (boundaries leaking);
              Case 3 → curvature collapse (terrain flattening);
              Case 4 → curvature measurement failure (no detection);
              Case 5 → curvature generation corruption (wrong patterns)
    
  Rest Mode metrics → terrain health indicators:
    GRT provides: I, fesc, Lreinf, SCC with thresholds
    EDT uses: terrain quality assessment
    Protocol: I high → curvature coherent;
              fesc low → boundaries holding;
              Lreinf high → terrain structure intact;
              SCC high → self-purification active
    
  θd calibration → terrain sensitivity tuning:
    GRT provides: EWMA-calibrated detection thresholds
    EDT uses: terrain-agent coupling strength parameter
    Protocol: θd tracks terrain velocity through sensitivity adjustment
```

### GRT ↔ FCN Integration Protocol

The GRT-FCN interface provides the mechanistic ODE resolution of governance dynamics and the structural scaling architecture:

```
FCN → GRT (mechanistic resolution):

  S-equation → ODE decomposition:
    FCN resolves S̃ = α·n²/C^β into constituent dynamics:
    
    S-equation (governance level):
      S̃ = α · ñ² / C̃(t)^β
      
    ODE scalar (mechanistic level):
      Φ = β_s · n² / (C · T · d)
      
    where:
      C = capacity (GRT: governance throughput)
      T = temperature (GRT: exploration/noise = T_eff from AGM)
      d = diversity (GRT: Dint position clarity)
      n = interaction density (GRT: number of active conflict channels)
      Φ = regime scalar (GRT: state indicator)
      
    Φ < 1: VCZ interior (Rest or healthy Active)
    Φ > 1: Storm regime (Collapse approach)
    Φ = 1: critical boundary
    
  Branching-reduced effective density:
    FCN establishes that appropriate terrain design reduces
    effective conflict density from n² to (n/B)²:
      S̃_effective = α · (n/B)² / C̃(t)^β
      
    where B = branching capacity (topologically separated channels)
    
    GRT mapping:
      B = number of independent governance domains
      n/B = per-domain conflict density
      Landscaping that increases B effectively reduces S̃
      without reducing actual agent count n
      
    EDT Terrain Cultivation Sufficiency:
      ∃ B* = O(√n) such that S(t) < S_critical for all t
      when B ≥ B*
      
      = there exists a branching capacity that guarantees stability
        scaling as √n rather than n² — this is why landscape design
        works at all
        
  Four intervention levers on S-equation:
    Lever 1: Reduce n (constrain exploration) — LEAST PREFERRED
      Sacrifices coverage and innovation
      GRT: restricting domain count or conflict diversity
      
    Lever 2: Reduce α (lower coupling) — coupling geometry
      Reduce role overlap, clarify boundaries
      GRT: improve position clarity (Poverlap reduction)
      
    Lever 3: Increase β (improve degradation quality) — maturity
      Better rules, better routing, better classification
      GRT: improve meta-rule quality, seed expansion completeness
      
    Lever 4: Increase C(t) (add processing capacity) — resources
      More governance throughput
      GRT: expand evaluation capacity, increase θd precision
      
    GRT governance preference: Levers 2-4 > Lever 1
    (absorb instability rather than suppress exploration)

  Circular Closure → Rest Mode structural mechanism:
    FCN's circular closure (self-referential feedback loop)
    = GRT's Rest Mode (self-sustaining governance cycle)
    
    Protocol:
      Circular closure achieved → AND-entry conditions met
      Circular closure broken → OR-exit triggered
      Circle integration → domain consolidation
      Circle formation → new domain governance establishing
      
  Contamination flux → failure case routing:
    FCN's Φ_contam = P · max(0, S − R)
    provides the dynamical mechanism for GRT's failure propagation
    
    Protocol:
      Φ_contam(domain_i) > 0 → domain i leaking instability
      Σ Φ_contam > R_{upper} → meta-rule layer overwhelmed
      Contamination mode → failure case type prediction
      
  Self-purification R_i → SCC decomposition:
    FCN's R_i = D · F · V · T decomposes SCC into components
    
    Protocol:
      D (decoupling) → subsidiarity enforcement
      F (feedback) → θd calibration quality
      V (variance) → position clarity (Dint)
      T (time buffer) → evaluation window margin
      Any component → 0 triggers SCC warning

  Cube Domination → position clarity dynamics:
    FCN's frame competition → GRT's niche differentiation
    
    Protocol:
      Frame dispersion Σ rising → cross-domain I falling
      Frame adoption score → convergence toward common standards
      Optimal Storm window → governance disruption management
      
  Attractor basin geometry → energy barrier precision:
    FCN's basin depth/width → GRT's ΔF structure
    
    Protocol:
      Deep+wide basin = healthy Rest Mode target
      Basin evolution ODE → landscape learning dynamics
      Kramers pre-exponential → attempt frequency for transitions
      Multi-dimensional correction → scaling effects on transition

GRT → FCN (governance architecture):

  Rule architecture → ODE parameter specification:
    GRT's rules determine the shape of FCN's potential landscape U(x;θ)
    
    Protocol:
      Global rules → set basin locations (where attractors are)
      Local rules → set basin widths (how tolerant each domain is)
      Meta-rules → set barrier heights (how hard state transitions are)
      Seeds → set landscape evolution rate (how fast learning occurs)
      
  Failure case taxonomy → ODE regime identification:
    GRT's 5 cases → FCN's Φ trajectory classification
    
    Protocol:
      Case 1 → Φ oscillating (contradictory attractors)
      Case 2 → Φ rising rapidly (Storm approach)
      Case 3 → Φ flat then spike (terrain collapse)
      Case 4 → Φ silent then catastrophic (Silent Criticality)
      Case 5 → Φ gradual drift (seed corruption)
      
  θd calibration → ODE temperature control:
    GRT's θd → FCN's D (noise intensity)
    
    Protocol:
      θd_max → D high (sensitive exploration)
      θd steady → D moderate (calibrated)
      θd frozen → D → 0 (attractor lock-in)
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
    
  Pair 10: Φ_contam (FCN) ↔ fesc propagation pattern (GRT)
    Rising contamination flux should correspond to bottom-up fesc escalation
    Discordance: Φ_contam > 0 but no upward fesc propagation → buffer absorbing
    
  Pair 11: R_i (FCN self-purification) ↔ SCC (GRT)
    R_i components should track SCC trajectory
    Discordance: R_i declining but SCC stable → measurement lag or compensating factor
    
  Pair 12: Σ (FCN frame dispersion) ↔ cross-domain I (GRT)
    Rising Σ should correspond to declining cross-domain consistency
    Discordance: Σ rising but I stable → domains diverging without conflict
    
  Pair 13: κ* (EDT risk index) ↔ governance state trajectory (GRT)
    κ* > 1 sustained should correspond to degrading governance metrics
    Discordance: κ* > 1 but metrics stable → environmental change not yet impacting
    
  Pair 14: Friction rate (EDT) ↔ conflict_rate/SCC ratio (GRT)
    Friction in optimal band should correspond to healthy learning indicators
    Discordance: friction optimal but learning metrics declining → processing failure

System health = majority concordance across all 14 pairs
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
├── From Call Centers to Neurons — ODE formalization, attractor dynamics, Cube Domination, Circular Closure
│     ↕ GRT connection: S-equation → ODE decomposition (S̃ governance → Φ mechanistic);
│       Circular Closure (원) ↔ Rest Mode as self-sustaining feedback loop;
│       Layered cone architecture ↔ subsidiarity as information compression;
│       Contamination flux Φ_contam ↔ cross-scale failure propagation mechanism;
│       Self-purification R_i = D·F·V·T ↔ SCC decomposition into 4 factors;
│       Immunity Paradox ↔ Self-Exciting Defect Layer ↔ AGM T_min;
│       Cube Domination frame competition ↔ niche differentiation under collapse;
│       Attractor basin geometry (depth vs width) ↔ energy barrier model precision;
│       Landscape evolution ODE ↔ SSS→SCM cascade dynamical mechanism;
│       Terrain design protocol (4-phase) ↔ θd bootstrapping phases;
│       North Star (Criterion vs Principle) ↔ Global vs Local rule distinction;
│       Eyes-and-feet principle ↔ dual-axis measurement justification;
│       Branching capacity B ↔ effective density reduction n/B;
│       Four intervention levers ↔ governance strategy optimization;
│       Stochastic resonance ↔ optimal Storm intensity D*
├── Environment Design Theory     — terrain cultivation, phase-gated seeding, branching manifold architecture
│     ↕ GRT connection: Three-Axis Architecture (Boundary/Gain/Coupling) ↔ landscape design decomposition;
│       Curvature Theory (curvature = compressed survival history) ↔ conflict log as curvature substrate;
│       Curvature Ceiling Theorem ↔ subsidiarity as structural necessity;
│       Curvature Withdrawal Schedule ↔ Rest Mode maturation arrow;
│       Friction Management (zero friction = zero learning) ↔ conflict rate monitoring;
│       Optimal friction band ↔ conflict rate between T_min and SCC capacity;
│       Buffer as friction transformer ↔ meta-rules making conflicts processable;
│       Therapeutic disturbance ↔ controlled perturbation injection;
│       Risk Index κ (timescale mismatch) ↔ governance lag detection;
│       κ-trajectory classification ↔ governance state assessment;
│       Three-alarm detection ↔ multi-metric early warning;
│       Terrain Resonance avoidance ↔ W and θd cycle non-resonance;
│       Carrying Capacity n_max ↔ domain rule density limits;
│       Contamination Permeability schedule ↔ phase-gated θd bootstrapping;
│       Gain-induced effective potential ↔ correction values as curvature;
│       Spectral radius reduction via branching ↔ position clarity as B increase
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
33. Network Architecture Theory (NAT, DFG component). Internal document, v3.2-mutual-memory-cleanmap, July 2026. (Typed routing, canonical resolution-gap polarity, multiplex graph/object locks, reciprocal local↔global terrain reconciliation, role-projected patches, clean-map governance, ancestry-aware diversity, staged expansion/rollback, claim ladder, and FDCL bridge/no-transfer rules including Schur/Feshbach coarse-graining with behavioral replay validity lock. Imported into GRT with explicit object and evidence-status boundaries.)
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
48. Fractal Governance System (FGS, DFG component). Internal document, v1.11-MMB-CheapBench, 2026. (Fractal lifecycle and middle-layer router; map–terrain feedback; growth sequence Separate→Mature→Couple→Integrate→Expand; governance information bottleneck; Micro–Macro Bridge Benchmark synthetic gate with replica invariance, coarse-graining closure, intervention-equivariance proxy, and topology-degeneracy testing. Imported into GRT as candidate validation/architecture support only, not as theorem-level proof.)
49. Environmental Design Theory (EDT, DFG component). Internal document, v5.0-maximal, March 2026. (Three-Axis Architecture — Boundary/Gain/Coupling as S-equation parameters; Curvature Theory — curvature as compressed survival history, accumulation dynamics, Curvature Ceiling Theorem, withdrawal schedule; Friction Management — Zero Friction Pathology, optimal friction band, buffer as friction transformer, therapeutic disturbance; Risk Index κ — endogenous drift τ_E, capacity adaptation τ_C, κ* hybrid index, trajectory classification; Terrain Resonance — constructive/destructive conditions, timescale collision avoidance; Carrying Capacity — n_max for terrain quality, overshoot dynamics, graceful degradation; Contamination Permeability — flux formalism, phase-dependent control, self-purification R_i = D·F·V·T; Circular Closure — circle architecture, n_eff compression, pyramidal architecture; Buffer Dynamics — noised-vector transformer, four-axis function taxonomy, local North Star calibration; Ecological Succession — pioneer/colonist/climax lifecycle; Seed Propagation — 0→1→2 transition, dormancy dynamics.)
50. From Call Centers to Neurons (FCN, DFG component). Internal document, v1.6, March 2026. (Mean-field ODE formalization; S-equation → Φ decomposition; attractor dynamics with basin geometry; Kramers escape with pre-exponential factor; Cube Domination frame competition dynamics; Circular Closure Theory — circle as fundamental governance unit, layered cone architecture, S-equation partitioning; Contamination Theory — cross-scale flux Φ_contam, three contamination modes, bottom-up propagation; Self-Purification Capacity R_i = D·F·V·T multiplicative decomposition; Terrain Design Protocol — 4-phase circle formation; North Star Architecture — Criterion vs Principle separation; Stochastic resonance at optimal Storm intensity D*.)
51. Olfati-Saber, R. & Murray, R. M. (2004). Consensus problems in networks of agents with switching topology and time-delays. *IEEE Transactions on Automatic Control, 49*(9). (Multi-agent consensus — structural contrast: GRT mutual-reference coupling vs communication delay.)
52. Beggs, J. M. & Plenz, D. (2003). Neuronal avalanches in neocortical circuits. *Journal of Neuroscience, 23*(35). (Neural criticality — power-law avalanche distributions analogous to governance Storm Scale Law.)
53. Warnecke, H.-J. (1993). *The Fractal Company: A Revolution in Corporate Culture*. Springer. (Self-similarity, self-organization, and dynamics in fractal organizational design — comparison point for GRT's asymmetric compatibility gradient.)
54. Vezhnevets, A. S., Osindero, S., Schaul, T., Heess, N., Jaderberg, M., Silver, D., & Kavukcuoglu, K. (2017). FeUdal Networks for Hierarchical Reinforcement Learning. *arXiv:1703.01161*. (Manager/Worker hierarchy with different temporal resolutions and abstract top-down goals.)
55. Finn, C., Abbeel, P., & Levine, S. (2017). Model-Agnostic Meta-Learning for Fast Adaptation of Deep Networks. *ICML / PMLR 70*. (Shared meta-initialization optimized for rapid task-specific adaptation.)
56. Zintgraf, L., Shiarli, K., Kurin, V., Hofmann, K., & Whiteson, S. (2019). Fast Context Adaptation via Meta-Learning. *ICML / PMLR 97*. (CAVIA separation of shared parameters from task-specific context parameters.)
57. Huang, T., Liu, S., Shen, L., He, F., Lin, W., & Tao, D. (2022). Achieving Personalized Federated Learning with Sparse Local Models. *arXiv:2201.11380*. (Personalized local models under heterogeneous client data; comparison point for global/local specialization.)
58. Mehta, P., & Schwab, D. J. (2014). An Exact Mapping Between the Variational Renormalization Group and Deep Learning. *arXiv:1410.3831*. (Iterative coarse-graining and extraction of relevant features/operators across scales.)
59. Ying, Z., You, J., Morris, C., Ren, X., Hamilton, W., & Leskovec, J. (2018). Hierarchical Graph Representation Learning with Differentiable Pooling. *NeurIPS 31*. (Learned hierarchical graph coarsening via differentiable pooling.)
60. Dong, H., Xu, J., Yang, Y., Zhao, R., Wu, S., Yuan, C., Li, X., Maddison, C. J., & Han, L. (2023). MeGraph: Capturing Long-Range Interactions by Alternating Local and Hierarchical Aggregation on Multi-Scaled Graph Hierarchy. *NeurIPS 36*. (Bidirectional local/hierarchical information propagation across multiscale graph representations.)

---

*Governance is not the management of agents. It is the design of the terrain they move through — and the conditions under which they no longer need anyone to manage it.*

*Rest Mode is not a reward granted at the end of development. It is the proof that development succeeded.*


---

## v1.23 Executed MediumBench — Observable Risk, Adaptive Quota, Passive SSID, and Cost-Object Separation

### 1. Benchmark status and epistemic lock

This section executes the next Medium candidate queue created by v1.22. It does **not** promote Schur/Feshbach, ERA, non-normality metrics, or passive identification into universal GRT laws. The benchmark uses the same controlled stable linear terrain families used by the recent Schur/Feshbach sieve and asks narrower operational questions:

1. Can the white-box numerical-abscissa selector be replaced by a **boundary-observable** risk score?
2. Can a rolling quantile preserve an ERA resource quota when the terrain-risk distribution drifts?
3. Can a useful ERA/state-space interface be learned from **passive noisy logs** rather than a clean active impulse probe?
4. Does reduced interface-state count predict actual runtime/energy cost?

The candidate pipeline remains:

```text
candidate
→ independent or held-out benchmark
→ scope/failure boundary
→ evidence-state update
→ only then possible promotion
```

### 2. MB-SF-04A — Boundary-observable non-normality proxy

The v1.22 canonical selector used the numerical abscissa of the declared full linear operator. That is a useful white-box risk score, but it cannot be assumed available to an orchestration layer that sees only module boundary behavior.

The current black-box candidate therefore used only the boundary Markov/impulse sequence and derived:

- peak response ratio;
- peak lag;
- tail-energy ratio;
- early log-envelope growth;
- boundary Hankel singular-value entropy;
- second/first Hankel singular-value ratio;
- a logistic composite trained only from those boundary features.

A material reducer-selection event was defined, as in v1.22, by a sufficiently large replay advantage of ERA over the compact rational candidate.

#### Held-out discrimination

| risk score | held-out AUC | shifted-terrain AUC | status |
|---|---:|---:|---|
| full-operator numerical abscissa | 0.875 | 0.875 | white-box reference |
| boundary peak ratio | 0.500 | 0.500 | fail |
| boundary tail energy | 0.696 | 0.613 | insufficient |
| boundary Hankel entropy | 0.518 | 0.700 | unstable across terrain |
| boundary-feature logistic composite | 0.589 | 0.650 | fail |

**Result MB-SF-04A — FAIL CURRENT FORM.** The present boundary-only feature set does not reproduce the white-box non-normality gate reliably enough for promotion.

The failure is structurally useful. Boundary observability is task-specific:

```text
boundary trajectory sufficient to fit an effective I/O model
        does not imply
boundary trajectory sufficient to identify hidden transient-risk geometry
```

Therefore GRT now separates:

\[
\mathcal O_{\mathrm{model}}
\neq
\mathcal O_{\mathrm{risk}}.
\]

A module may be behaviorally compressible while the property deciding **which** compressor is safe remains under-observed.

Candidate states:

```text
CF-SF-PROXY-BND-COMP-01 → MEDIUM_FAIL_CURRENT_FORM
CF-SF-PROXY-BND-PEAK-01 → MEDIUM_FAIL_CURRENT_FORM
```

### 3. MB-SF-04B — Rolling-quantile quota adaptation

A fixed selector threshold implicitly assumes a stable risk-score distribution. v1.22 already showed that this can violate the ERA budget under terrain shift. The next candidate maintains a rolling score history and sets the current ERA threshold to the empirical upper risk quantile corresponding to the declared resource quota.

For nominal ERA quota \(q=0.40\):

```text
history W
→ estimate current 60th percentile of risk
→ score above percentile → ERA
→ otherwise → compact rational
→ update history
```

The stress stream was a resampled held-out sequence with three phases:

```text
ID terrain → shifted terrain → return to ID terrain
```

This streaming stress test evaluates **resource adaptation**, not independent reducer accuracy.

| policy | overall ERA fraction | mean phase-wise absolute quota deviation |
|---|---:|---:|
| fixed threshold | 58.3% | 18.98 percentage points |
| rolling quantile, W=60 | 39.6% | **1.20 points** |
| current-phase batch rank reference | 40.0% | 0 |

Phase-wise rolling ERA fractions were 40.6%, 37.8%, and 40.8% across ID, shifted, and ID-return phases.

**Result MB-SF-04B — PASS FOR RESOURCE CONTROL, NOT RISK ACCURACY.** Rolling quantiles solve the *budget-drift* problem substantially better than a frozen threshold, but cannot rescue a weak boundary risk score. Resource control and risk prediction remain separate operators.

```text
CF-SF-QUOTA-ROLL-01 → MEDIUM_PASS_RESOURCE_CONTROL_ONLY
```

### 4. MB-SF-04C — Noisy/passive state-space identification

The v1.21/v1.22 ERA results assumed clean active Markov/impulse access. This bench removes that assumption. The candidate receives:

- a logged stochastic boundary input;
- noisy boundary output;
- no interior operator;
- no explicit impulse experiment.

A finite impulse-response Markov sequence is estimated from the passive log by ridge regression, then a stability-locked ERA realization is selected using a separate noisy passive validation trajectory.

#### Replay results

| output SNR | passive ID mean error | passive OOD mean error | selected-model stable fraction |
|---|---:|---:|---:|
| 40 dB | 5.09% | 4.46% | 100% |
| 25 dB | 4.32% | 4.42% | 100% |
| 15 dB | 5.58% | 6.22% | 100% |

The clean active-probe ERA reference remained near 0.3% average error on these systems. Passive SSID therefore survives, but with a large information-access penalty.

**Result MB-SF-04C — SCOPE-LIMITED PASS.** The toy system supports usable black-box effective maps from passive/noisy logs, including moderate OOD forcing, but does not establish equality with active identification. Persistent excitation, log length, noise model, and hidden initial-state handling remain part of the deployment contract.

```text
CF-SF-SSID-PASSIVE-01 → MEDIUM_PASS_SCOPE_LIMITED
```

### 5. MB-SF-04D — Runtime and energy proxy audit

Previous benches often reported interface-state count as a compression/resource quantity. That is legitimate as a representation-size metric but is not automatically a runtime or energy metric.

A direct implementation audit compared the current reference Python realizations over the same rollout length:

| model | mean interface/basis dimension | mean measured rollout time |
|---|---:|---:|
| ERA state-space | 3.67 | 2.80 ms |
| current rational history-kernel implementation | 2.83 | 155.3 ms |

The current rational reference implementation was about **55× slower** despite the smaller basis count, because it explicitly evaluates a long history convolution rather than using an optimized recursive realization.

This does **not** prove rational realizations are intrinsically slower. It proves the stronger and more useful negative statement:

> **State count is not a valid runtime or energy surrogate without specifying the realization and hardware.**

The following cost objects are now locked as distinct:

\[
C_{\mathrm{resource}}
=
(C_{\mathrm{representation}},
C_{\mathrm{online\ arithmetic}},
C_{\mathrm{history}},
C_{\mathrm{probe}},
C_{\mathrm{refresh}},
C_{\mathrm{hardware\ energy}}).
\]

Scalarization is allowed only under a declared deployment utility/price model.

```text
CF-SF-COST-DIM-01 → MEDIUM_FAIL_AS_RUNTIME_SURROGATE
```

### 6. Updated effective-interface selection rule

The effective-map orchestration problem is therefore widened from

```text
terrain risk + model accuracy + state budget
```

to

```text
observability contract
+ terrain-risk score
+ model family
+ resource quota
+ identification mode (active/passive)
+ implementation realization
+ replay residual
+ refresh policy
```

A compact formal representation is

\[
\Pi_{\mathrm{eff}}
=
\operatorname{Select}
(\mathcal O,
R_{\mathrm{terrain}},
Q_{\mathrm{resource}},
C_{\mathrm{impl}},
R_{\mathrm{replay}},
\Gamma_{\mathrm{refresh}}).
\]

This strengthens the GRT principle that the orchestrator should not select merely the "best model". It selects a **model–measurement–implementation–refresh bundle** under a contract.

### 7. Prediction updates

**Prediction 65 — Risk-observability separation.** A boundary interface may permit low-error I/O reduction while failing to expose enough information to classify hidden non-normal transient risk.

**Prediction 66 — Adaptive quota stability.** Rolling/rank-based resource thresholds should maintain declared expensive-model utilization more reliably than frozen absolute thresholds under risk-distribution drift.

**Prediction 67 — Passive identification penalty.** Passive/noisy effective-map identification can remain stable and useful but should require more data and incur greater replay residual than clean active probes at matched model order.

**Prediction 68 — Representation/runtime non-equivalence.** Smaller reduced-state dimension will not monotonically imply lower latency or energy across different realization families.

**Prediction 69 — Bundle selection advantage.** A selector that jointly accounts for observability, reducer family, resource quota, realization cost, and refresh validity should dominate any policy using only reducer accuracy or state dimension once deployment costs are heterogeneous.

### 8. Next candidate queue

Relatively cheap / Medium candidates:

1. `CF-SF-PROXY-MPROBE-01` — multi-direction / finite-amplitude boundary probe for hidden-risk scoring;
2. `CF-SF-SSID-FRONTIER-01` — passive SSID data-length × SNR × rank frontier;
3. `CF-SF-QUOTA-SCARCE-01` — rolling quota under abrupt capacity loss / scarce ERA slots;
4. `CF-SF-RAT-REC-01` — optimized recursive rational realization and fair runtime comparison;
5. `CF-SF-COST-JOINT-01` — error × runtime × probe × refresh Pareto frontier.

Higher-cost candidates remain pending:

- nonlinear switching/saturation effective maps;
- recursive multiscale Schur/Feshbach closure;
- multiplex information/recovery/audit/authority effective operators;
- deployed multi-agent boundary-contract experiments.

### 9. Reproducibility lock

Executed artifacts:

```text
grt_v123_observable_quota_passive_cost_results.json
grt_v123_benchmark_summary.json
run_grt_v123_observable_quota_passive_cost_bench.py
```

The measured runtime numbers are explicitly **implementation-dependent** and may not be cited as a theorem about rational versus ERA complexity. The passive-identification result is likewise tied to the declared synthetic linear generator, stochastic excitation, log length, SNR convention, FIR estimator, and stability lock.


---

## v1.24 Dynamic Influence Balance System (DIBS)

### 1. Purpose and source lock

DIBS is the GRT operational controller for **precision multi-agent work in which the problem is not merely which agent should participate, but how strongly, how often, how quickly, and with what authority each agent's completed output should influence the shared trajectory**.

The module is synthesized primarily from Vector Storm Theory v3.7.7 concepts:

- VCZ as a dynamically maintained slightly-subcritical operating regime rather than a static equilibrium point;
- Dynamic Partitioned Equilibrium (DPE): topology, external calibration, selective permeability, non-rigid temporal coordination, regeneration, and verified return;
- the requirement to preserve local directional signal while eliminating persistent global directional privilege;
- tensioned coexistence: enough alignment for coordination and enough non-alignment for buffering;
- phase-dependent permeability and asymmetric read/write reopening;
- non-zero exploration/adaptability floor;
- Local–Global North Star projection consistency rather than forced identity.

**Epistemic lock.** DIBS is a **candidate operational architecture**. The VST concepts motivate the control objectives and safety constraints; they do not prove that the controller below is universally optimal or that its proposed thresholds transfer across architectures.

### 2. What DIBS controls

A conventional ensemble often treats an agent output as one scalar weight:

\[
Y=\sum_i w_i y_i.
\]

DIBS treats this as too coarse. The effective influence of agent \(i\) is a control bundle

\[
\Gamma_i(t)
=
\bigl(g_i,\,f_i,\,\tau_i,\,b_i,\,a_i,\,\pi_i^{\rm read},\,\pi_i^{\rm write}\bigr)_t,
\]

where

- \(g_i\): **gain** — amplitude of influence;
- \(f_i\): **emission rate / duty cycle** — how often the output participates;
- \(\tau_i\): **delay** — when the influence becomes visible to the next stage;
- \(b_i\): **bandwidth / resolution budget** — how much detail crosses the interface;
- \(a_i\): **action authority** — how directly the signal may alter action;
- \(\pi_i^{\rm read}\): **read permeability** — how much outside evidence the agent/controller may observe;
- \(\pi_i^{\rm write}\): **write permeability** — how much the agent may alter shared state or downstream trajectories.

The first major lock is therefore

\[
\boxed{\text{signal visibility}\neq\text{signal influence}\neq\text{action authority}.}
\]

An independent verifier may have low output volume but high veto authority. A speculative explorer may have high diagnostic visibility but near-zero write authority. A dominant specialist may remain fully observable while its gain is temporarily attenuated.

### 3. Agent influence packet

Each agent sends a **committed** packet rather than live internal reasoning:

\[
\mathcal O_i(t)=
(d_i,m_i,c_i,u_i,n_i,r_i,\chi_i,S_{N,i},p_i,\mathcal A_i).
\]

Candidate fields:

| field | meaning |
|---|---|
| \(d_i\) | output direction / proposed conclusion / action vector |
| \(m_i\) | native output magnitude |
| \(c_i\) | confidence |
| \(u_i\) | uncertainty |
| \(n_i\) | novelty / non-redundant information estimate |
| \(r_i\) | recent validated residual / error history |
| \(\chi_i\) | error-correlation or common-mode exposure with other agents |
| \(S_{N,i}\) | Local North Star / local-attractor strength proxy |
| \(p_i\) | provenance and common-ancestry information |
| \(\mathcal A_i\) | authority class and veto/write contract |

DIBS does not require every deployment to expose every field. Missing observability narrows the claim scope and may force a more conservative controller.

### 4. Dynamic-balance observation state

The controller maintains a system-level state bundle

\[
Z_{\rm DIBS}(t)=
\bigl(
G_{IE},
M_{\rm SCC},
P_{\rm dir},
C_{\rm err},
M_{\rm rec},
I_{\rm cal},
V_{\rm exp},
C_{\rm resource}
\bigr)_t.
\]

#### 4.1 External-calibration gap \(G_{IE}\)

Measures how far the internally coherent solution has drifted from an independently anchored external reference. Internal agreement is not enough.

#### 4.2 SCC-local amplification margin \(M_{\rm SCC}\)

The controller asks whether any causal strongly connected component is locally supercritical even if the global mean looks safe. A single scalar global average may hide a dangerous local loop.

#### 4.3 Directional privilege \(P_{\rm dir}\)

Measures whether one agent, faction, pathway, or interpretation persistently dominates system-wide influence. Candidate diagnostics include maximum normalized gain, concentration/HHI, influence centrality, and persistence of dominance across windows.

#### 4.4 Error-correlation / common-mode concentration \(C_{\rm err}\)

Model count is not diversity. If several agents share the same residual direction, their votes should not be counted as independent evidence.

#### 4.5 Recovery margin \(M_{\rm rec}\)

A balance state is not trusted unless bounded perturbations retain a feasible return path and declared recovery target.

#### 4.6 Calibration information floor \(I_{\rm cal}\)

Permeability may be reduced to stop cascade propagation only while enough external/local information still crosses the boundary to avoid governance blindness.

#### 4.7 Exploration vitality \(V_{\rm exp}\)

The controller preserves a non-zero exploration floor. A silent system with zero residual generation is not automatically healthy; it may be Frozen Rest / False Compatibility.

### 5. Target region: Moving Dynamic Balance Zone

DIBS does not seek

```text
all agents agree
all residuals = 0
all gains equal
all channels fully open
all channels fully closed
```

The target is a moving viable region

\[
\mathcal V_{\rm DIBS}(t)
=
\left\{
Z:
\begin{array}{l}
M_{\rm SCC}\ge m_{\min},\\
P_{\rm dir}\le p_{\max},\\
G_{IE}\le g_{\max},\\
I_{\rm cal}\ge I_{\min},\\
V_{\rm exp}\ge V_{\min},\\
M_{\rm rec}\ge r_{\min}
\end{array}
\right\}.
\]

This is the GRT execution form of the VST principle:

```text
preserve local directional signal
+
remove persistent global directional privilege
+
preserve a return path
+
keep a non-zero exploration floor
```

The center of the acceptable region may drift with terrain. DIBS therefore tracks a **moving target band**, not a fixed set of ideal weights.

### 6. Effective influence transformation

For a completed agent output \(u_i(t)\), define the effective influence packet

\[
\tilde u_i(t)
=
 a_i(t)\,g_i(t)\,q_i(t)\,
\mathcal D_{\tau_i(t),b_i(t)}[u_i(t)],
\]

where \(q_i(t)\in\{0,1\}\) or \([0,1]\) is a duty/rate gate and \(\mathcal D\) is the declared delay/bandwidth transformation.

For outputs that share a valid synthesis space, a candidate aggregation is

\[
U(t)=\mathcal S\bigl(\{\tilde u_i(t)\}\bigr).
\]

**Conflict-preservation lock.** \(\mathcal S\) is not required to be an arithmetic mean. If outputs are typed `CONFLICT`, `UNKNOWN`, `UNSAFE`, or belong to incompatible action spaces, DIBS must preserve those states rather than laundering them into a middle value.

### 7. Candidate gain score

A cheap initial gain layer may use

\[
s_i(t)
=
\frac{
Q_i(t)\,S_{N,i}(t)\,N_i(t)
}{
(\epsilon+R_i(t))\,[1+\lambda_C C_i(t)]
},
\]

where

- \(Q_i\) is reliability;
- \(S_{N,i}\) is local-reference strength;
- \(N_i\) is novelty / non-redundancy;
- \(R_i\) is recent validated residual;
- \(C_i\) is correlated-error/common-ancestry exposure.

The raw score is converted to normalized gain shares and then projected through:

1. a **single-agent dominance cap**;
2. a **minimum influence/diversity entropy floor** where appropriate;
3. critical-role floors for independent verifier/recovery paths;
4. authority-specific non-compensatory constraints.

This is a candidate engineering rule, not a theorem.

### 8. Controller objective

A general DIBS controller may minimize

\[
\begin{aligned}
\mathcal J_{\rm DIBS}
=&\;w_S\,\widehat R_{\rm storm}
+w_P\,P_{\rm dir}
+w_C\,C_{\rm err}
+w_E\,G_{IE}
+w_R\,\mathcal C_{\rm rollback}\\
&+w_Q\,C_{\rm resource}
-w_I\,I_{\rm cal}
-w_V\,V_{\rm exp},
\end{aligned}
\]

subject to the declared DIBS viable-region constraints.

A generic projected update is

\[
\Gamma_{t+1}
=
\Pi_{\mathcal U_{\rm DIBS}(t)}
\left[
\Gamma_t-\eta_t\widehat\nabla_{\Gamma}\mathcal J_{\rm DIBS}(t)
\right].
\]

This equation is an **architecture template**. Deployments may use MPC, robust control, bandit allocation, constrained optimization, learned routing, or rule-based approximations. No optimizer family is canonical yet.

### 9. Permeability as an interior control variable

DIBS adopts the VST/DPE idea that useful exchange generally has two bounds:

\[
\pi_{\rm info}
\le
\pi
\le
\pi_{\rm cascade}.
\]

The lower bound is the minimum openness needed for calibration and useful cross-agent information. The upper bound is the maximum openness compatible with cascade containment.

Therefore:

```text
π too low  → information starvation / Frozen Rest / wrong-frame lock-in
π too high → common-mode coupling / cascade propagation / Vector Storm
interior π → useful coordination with retained shock buffer
```

A candidate online update is

\[
\pi_{t+1}
=
\operatorname{clip}_{[\pi_{\rm info},\pi_{\rm cascade}]}
\left(
\pi_t
-\eta_\pi\,R_{\rm cascade}
+\eta_I\,D_{\rm info}
\right),
\]

where \(D_{\rm info}\) increases when the information/calibration floor is threatened.

### 10. Timescale-separated balance control

To prevent the balance controller itself from becoming a high-frequency mutual-reference participant, DIBS uses at least three control speeds.

```text
FAST loop
  gain / duty / temporary permeability
  → absorb local directional spikes

MIDDLE loop
  delay / bandwidth / routing path / module coupling
  → repair persistent interaction geometry

SLOW loop
  authority contracts / global rules / North-Star compatibility map
  → revise structural assumptions only after accumulated evidence
```

Candidate ordering:

\[
\tau_{\rm gain}
<
\tau_{\rm route}
<
\tau_{\rm authority}
<
\tau_{\rm rule}.
\]

**Anti-oscillation requirements:**

- gain/permeability slew-rate limits;
- deadband around the target zone;
- asymmetric promote/demote hysteresis;
- minimum dwell time before phase switching;
- rollback checkpoints;
- suppression of rapid reciprocal gain chasing between peers.

### 11. Phase-dependent DIBS modes

#### Mode 0 — VCZ / precise normal operation

```text
moderate/high filtered read permeability
moderate write permeability
small continuous residual floor
covariance-aware gain balancing
local autonomy preserved
```

Objective: maximize useful information while preventing persistent directional privilege.

#### Mode 1 — Early drift

```text
reduce gain of high-common-mode pathways
increase independent verifier visibility
increase diagnostic read access
slow write coupling selectively
preserve calibration information floor
```

Objective: determine whether the drift is local error, global-map error, or terrain change before hard intervention.

#### Mode 2 — Active Storm / supercritical SCC

```text
affected SCC write permeability ↓ sharply
cross-SCC influence gain ↓
read-only diagnostic channels may remain open
new generative seeds into uncontained SCC → blocked
critical recovery authority → preserved
```

Objective: dissolve amplification loops without blinding diagnosis.

#### Mode 3 — Post-containment diagnosis

```text
read permeability > write permeability
counterfactual/test signals only
conflict and provenance retained
no forced re-consensus
```

#### Mode 4 — Renewal

```text
small validated writes
low-amplitude independent seeds
rollback mandatory
Local North Star strength and return margin re-tested
```

#### Mode 5 — Reconnection

```text
π_write ramps upward gradually
agent gains return gradually, not instantly
recurrence/SCC tests after each increment
```

#### Mode 6 — Mature Rest

```text
background selective exchange
low intervention frequency
non-zero exploration / residual-vitality floor
upper layer stays reserve rather than routine participant
```

### 12. Authority–gain separation

One of the strongest DIBS rules is that an agent's epistemic influence and its action authority are separate.

Examples:

```text
Exploration agent:
  diagnostic gain       high
  write authority       low
  action authority      near zero

Independent verifier:
  output frequency      low
  ordinary gain         low/moderate
  veto authority        high

Local specialist:
  local terrain gain    high
  cross-terrain gain    low

Upper governance layer:
  observation authority high
  routine gradient gain low
  emergency boundary authority high
```

This avoids turning every useful signal into a direct force on the shared trajectory.

### 13. DIBS + Middle Layer

The Middle Layer becomes the primary DIBS actuator, but it is not allowed to become the hidden dictator.

Its responsibilities are:

1. measure influence concentration and common-mode error;
2. translate output packets into comparable contracts where possible;
3. set or propose \(\Gamma_i\);
4. preserve conflict labels;
5. monitor local SCC and interface load;
6. preserve the information floor while reducing cascade channels;
7. return residuals and controller actions to the audit log;
8. request upper-layer structural revision when balance cannot be restored within the local contract.

The Middle controller itself is therefore versioned and subject to translator-drift / router-drift audits already introduced in earlier GRT versions.

### 14. DIBS + effective-map / Schur–Feshbach stack

The recent effective-interface work and DIBS occupy different layers:

```text
Schur / Feshbach / ERA
  → estimate how a module behaves at its boundary

DIBS
  → decide how strongly that boundary behavior should influence
    other modules right now
```

Thus

\[
\text{effective model}
\neq
\text{influence controller}.
\]

DIBS may use effective-map residuals, non-normality risk, refresh validity, and boundary response as observations, but reducer selection and dynamic balance remain separate orchestration decisions.

### 15. Minimum safety locks

DIBS cannot be deployed as a precision controller unless the following are declared:

1. **No current-truth leakage:** control at time \(t\) may use only observables available by time \(t\).
2. **External-anchor independence:** the calibration signal used to detect wrong-frame consensus may not be generated solely by the same optimized loop.
3. **Critical-direction floor:** aggregate utility cannot purchase a declared safety-critical loss.
4. **Conflict preservation:** weight adjustment does not certify unresolved claims.
5. **Exploration floor:** gain suppression may not silently drive all local novelty to zero.
6. **Information floor:** cascade isolation may not eliminate required calibration channels.
7. **SCC-local gate:** global stability metrics cannot override a locally supercritical causal component.
8. **Recovery target:** stabilization requires verified return into a robust target/core, not merely a momentary fall in the instability score.
9. **Controller rollback:** a DIBS update that increases instability, lag, or calibration error can be reverted.
10. **Controller cost accounting:** controller computation, monitoring, and intervention cost are part of the system budget.

### 16. Candidate ladder

#### Cheap candidates

```text
CF-DIBS-G0 — equal fixed influence
CF-DIBS-G1 — confidence-only gain
CF-DIBS-G2 — residual-adaptive gain
CF-DIBS-G3 — covariance/common-mode-aware gain
CF-DIBS-G4 — covariance-aware gain + dominance cap + exploration entropy floor
CF-DIBS-P1 — gain + adaptive permeability
CF-DIBS-A1 — gain + separated authority/veto
```

#### Medium candidates

```text
CF-DIBS-T1 — delay-aware / timescale-separated balance
CF-DIBS-SCC1 — SCC-local amplification gate
CF-DIBS-PH1 — phase-switching DIBS controller
CF-DIBS-R1 — recovery-return-aware controller
CF-DIBS-NN1 — non-normal transient-risk-aware gain/permeability control
CF-DIBS-M1 — learned constrained controller with rollback
```

#### Heavy pending

```text
CF-DIBS-H1 — nonlinear switching multi-agent systems
CF-DIBS-H2 — recursive fractal DIBS across multiple governance scales
CF-DIBS-H3 — multiplex authority/information/recovery/audit control
CF-DIBS-H4 — deployed real-agent precision task with external calibration
```

### 17. Benchmark program

#### CB-DIBS-01 — Gain-only competition

Compare equal, confidence, residual, covariance-aware, and covariance+vitality-floor gain policies on externally generated truth with correlated agent errors and terrain shifts.

Primary metrics:

- task loss;
- high-agreement wrong-consensus rate;
- maximum persistent influence share;
- residual-error covariance;
- adaptation after terrain shift;
- controller movement cost.

#### CB-DIBS-02 — Interior permeability

Compare:

```text
near-isolation
fixed-open
risk-only closure
gain + constrained interior permeability
```

under a task requiring both cross-agent calibration and cascade containment.

Kill rule: a controller that lowers Storm events only by violating the calibration-information or exploration floor does **not** pass.

#### CB-DIBS-03 — Delay / partial non-alignment

Test whether a small intentional delay window reduces synchronous cascade without materially degrading task tracking. No universal positive-delay claim is pre-registered.

#### CB-DIBS-04 — Authority separation

Compare a single scalar weight against separate `diagnostic gain / write authority / veto authority` controls under verifier and explorer roles.

#### MB-DIBS-05 — Phase controller

Stress VCZ → drift → Storm → diagnosis → renewal → reconnection transitions and test false phase switches, hysteresis, recurrence, and recovery time.

### 18. Mechanical implementation gate — executed

Before behavioral benchmarking, a narrow implementation sanity check was run for the cheap gain/permeability layer.

Frozen test contract:

```text
N agents                         = 8
random control windows           = 2,000
max single-agent normalized gain = 0.32
normalized influence entropy     >= 0.80
permeability interval            = [0.28, 0.82]
global gain interval             = [0.28, 0.92]
```

Results:

| check | violations |
|---|---:|
| normalized weights sum to one | 0 / 2,000 |
| single-agent gain cap | 0 / 2,000 |
| influence-entropy floor | 0 / 2,000 |
| permeability interval | 0 / 2,000 |
| global-gain interval | 0 / 2,000 |
| paired higher-risk → non-increasing permeability/gain | 100% satisfied |

Status:

```text
DIBS mechanical constraint implementation
→ IMPLEMENTATION_GATE_PASS
```

**Interpretation lock:** these checks are partly true by construction. They prove only that the reference controller implementation respects its declared mechanical constraints. They do **not** show that DIBS improves accuracy, prevents Vector Storm, identifies the correct agent, or is optimal. Those claims remain in the benchmark queue above.

### 19. New GRT principles

#### Dynamic Influence Principle

> In precision multi-agent work, governance should regulate **effective influence**, not merely participation. Agent selection and output weighting are insufficient when coupling strength, timing, information bandwidth, and authority have different failure modes.

#### Tension-Preservation Principle

> Healthy balance suppresses persistent global directional privilege while preserving bounded local disagreement, independent correction paths, and a non-zero exploration floor.

#### Interior Permeability Principle

> When calibration requires exchange but unrestricted exchange raises cascade risk, permeability is a constrained control variable with an information floor and a cascade ceiling; neither full openness nor full isolation is presumed optimal.

#### Authority–Signal Separation Principle

> The right to be heard, the amount of epistemic influence, and the authority to modify shared state or action are separate contracts.

#### Moving-Balance Principle

> The target of balance is a moving viable region conditioned on terrain, load, and reference quality, not a fixed consensus vector or permanent set of weights.

### 20. Prediction updates

**Prediction 70 — Covariance-aware balancing.** Under correlated agent errors, a gain controller that accounts for common-mode residual structure should reduce false consensus relative to confidence-only weighting at matched information/authority budgets.

**Prediction 71 — Interior permeability.** On tasks requiring cross-agent calibration, a constrained interior-permeability policy should outperform both near-isolation and unrestricted exchange on a joint task-loss/cascade-risk objective when the feasible information–cascade interval is non-empty.

**Prediction 72 — Authority separation.** Separating diagnostic influence from write/action authority should permit higher exploratory diversity with lower catastrophic-action rate than a single scalar influence weight under matched verifier coverage.

**Prediction 73 — Phase-specific control.** A phase-dependent DIBS policy should reduce recurrent cascades relative to one stationary gain/permeability policy when the system traverses drift, containment, renewal, and reconnection phases.

**Prediction 74 — Moving target.** Fixed gain thresholds should degrade under terrain drift more rapidly than controllers that re-estimate the viable influence/permeability region from rolling residual and calibration data.

**Prediction 75 — Over-damping failure.** Policies that minimize disagreement or coupling without an explicit information and exploration floor should exhibit Frozen Rest, slower adaptation, or wrong-frame stability on tasks requiring continual environmental calibration.

### 21. Current status

```text
DIBS architecture                     → DEFINITION / SYNTHESIS
DIBS mechanical reference controller → IMPLEMENTATION_GATE_PASS
behavioral superiority                → CANDIDATE / UNTESTED
universal optimality                  → NOT CLAIMED
full nonlinear/multiscale stability   → HEAVY_PENDING
```

The next rational step is to execute `CB-DIBS-01` and `CB-DIBS-02` separately so that gain effects are identified before permeability, delay, authority, and phase switching are combined.
