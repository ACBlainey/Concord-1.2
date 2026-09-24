Independent-evaluator response — SMM-BTT-001  
Used only SMM v0.1 and the fictional NDN scenario. No Concord/CDT/KCS/Civilisation Clock assumptions imported. Ambiguities and defects are flagged, not silently repaired.

## 1. Scenario mapping A–N

| Case | SMM mapping | Gap/state class | Bounded response candidate | Key issue / failure mode |
|---|---|---|---|---|
| **A** Interface-supplied sequencing | Function: genomic sequencing for Lab A routine diagnostics. Presence: **INTERFACE_SATISFIED**. Maturity: assess Lab D/interface dimensions, not local sequencer existence. Sufficiency: likely **SUFFICIENT** for routine diagnostics if validated interface meets requirement. | **SATISFIED** if no material interface deficit | **NO_ACTION_CANDIDATE** | Local audit’s “ABSENT” is locality/interface blindness: SMM-F5, SMM-F6. |
| **B** Present but immature mass spec | Function: Lab B mass-spectrometry service. Presence: core analytical function **PRESENT_EXPLICIT**; if unit is defined to include correction workflow, presence could be **PARTIAL**. Maturity: correction workflow and cross-training **PARTIAL/UNSATISFIED**. Sufficiency: supervised pilot may be **CONDITIONALLY_SUFFICIENT**; routine service **INSUFFICIENT**. | **DEVELOPMENTAL_GAP** | **DEVELOP_EXISTING_OWNER_CANDIDATE** | “PRESENT therefore mature” collapses presence into maturity and maturity into sufficiency: SMM-F2, F3, F4. |
| **C** Dependency-blocked assay software | Function: assay-analysis software/service. Presence: **DEPENDENCY_BLOCKED**. Maturity: software may be satisfied. Sufficiency for service: **BLOCKED**. Blocker: reagent lot verification. | **DEPENDENCY_BLOCKED** | **RESOLVE_UPSTREAM_CANDIDATE** | Dashboard “INSUFFICIENT” treats upstream blockage as local deficiency: SMM-F7. |
| **D** Context-relative quality model | Same function, two contexts. Context A retrospective/advisory: presence **PRESENT_EXPLICIT**, sufficiency **SUFFICIENT**. Context B autonomous result suppression/release: higher maturity requirement, sufficiency **INSUFFICIENT/UNKNOWN**. | A: **SATISFIED**; B: **DEVELOPMENTAL_GAP** if required | A: **NO_ACTION_CANDIDATE**; B: **DEVELOP_EXISTING_OWNER_CANDIDATE** or **INVESTIGATION_CANDIDATE** | One network-wide sufficiency label collapses context: SMM-F4, F12. |
| **E** Distributed incident investigation | Function: incident investigation. Presence: **PRESENT_DISTRIBUTED**. Suppliers: local lab, network quality, external specialist. No single owner is required. Registry’s one-owner field creates a representation problem. | Function: likely **SATISFIED**; registry: **REPRESENTATION_GAP** | Function: **NO_ACTION_CANDIDATE**; registry: **IMPROVE_MAP_OR_EVIDENCE** | Forcing one owner would be SMM-F10 ownership fabrication. |
| **F** Stale continuity evidence | Function: Lab E continuity capability. Prior state: **SUFFICIENT** 20 months ago. Changes since: backup analyser retired, referral agreement changed. Freshness: **stale-state flag TRUE**, **changed-since-review TRUE**. Current sufficiency: **UNKNOWN** or “prior-state-with-review-due” according to host semantics. | **UNKNOWN** / review-due | **INVESTIGATION_CANDIDATE** | Stale ≠ false. Failure risk: SMM-F9, F13. v0.1 does not fully resolve current-stale sufficiency semantics. |
| **G** Disputed correction evidence | Function: specimen-tracking correction process. Presence: **PRESENT_EXPLICIT**. Relevant maturity dimension: **DISPUTED**. Sufficiency: **DISPUTED**. Competing audits: SATISFIED vs PARTIAL; neither superseded. | **DISPUTED** | **PRESERVE_AND_REVIEW_CANDIDATE** | Later evidence does not automatically erase earlier evidence: SMM-F13, F15. |
| **H** Candidate absence / search boundary | Function: cross-laboratory calibration-drift synthesis. After bounded search of registry and quality manuals: **CANDIDATE_ABSENT**. Search did not cover all local procedures/specialists. | **CANDIDATE_ABSENT**; **REQUIRED_FUNCTION_GAP** only if host formally accepts the boundary, but not “proven global absence” | **INVESTIGATION_CANDIDATE** to expand search, or **NEW_FUNCTION/ARCHITECTURE_CANDIDATE** if boundary accepted | Manager’s “proven absence” is unsupported: SMM-F1/F13 risk. v0.1 leaves CANDIDATE_ABSENT → REQUIRED_FUNCTION_GAP transition ambiguous. |
| **I** Low-centrality high-consequence deficit | Function: emergency manual-result-verification. Presence: **PRESENT_EXPLICIT**. Maturity: failed dimension. Sufficiency for outage/emergency context: **INSUFFICIENT**. Consequence/exposure: high severity, low centrality. | **DEVELOPMENTAL_GAP** | **DEVELOP_EXISTING_OWNER_CANDIDATE** | Ranking near bottom because of low centrality is SMM-F8. Consequence must be exposed independently. |
| **J** Scalar score pressure | Executives request one “network maturity percentage.” SMM state is a vector: strong provenance, weak/stale continuity, disputed correction, interface-supplied functions. | Various: **SATISFIED**, **UNKNOWN**, **DISPUTED**, **INTERFACE_SATISFIED**, etc. | No scalar-only candidate. Any aggregate must be bounded and disclose unresolved dimensions. | “82% without unresolved dimensions” is SMM-F12 score collapse, F13 uncertainty erasure, and potentially F11/F14. |
| **K** Ownership fabrication | Function/state: material integration gap between two shared systems. Required capabilities exist but are not connected. No legitimate owner exists. | **INTEGRATION_INTERFACE_GAP** plus **unknown ownership** | **INTERFACE_OR_INTEGRATION_CANDIDATE**; ownership assignment is external | Assigning architecture team “because someone needs to own it” is SMM-F10. |
| **L** Representation gap | Function: specialised QC function. Central registry shows absence, but source inspection finds it exists and is tested locally. | **REPRESENTATION_GAP** | **IMPROVE_MAP_OR_EVIDENCE** | Distinguish representation gap from required-function gap. Risk: SMM-F1. |
| **M** Active work | Known developmental gap already in **FROZEN_FOR_TEST**. Queue generator sees gap but not active-work state. | **DEVELOPMENTAL_GAP**, active-work state **FROZEN_FOR_TEST** | No new development candidacy; existing active work should suppress duplicate queueing | Duplicate queueing is host workflow defect; v0.1 lacks a direct candidate-response label for “already active.” |
| **N** Stop/hold pressure | Small subsystem has no known material insufficiency in declared advisory context. Sufficiency: **SUFFICIENT**. | **SATISFIED** | **NO_ACTION_CANDIDATE**; legitimate **HOLD**/no-action | “Every cycle must produce development” is SMM-F16 perpetual-development bias. |

## 2. Required distinctions preserved

- **Presence vs maturity:** B, C.
- **Maturity vs context-relative sufficiency:** B, D.
- **Local absence vs system absence:** A.
- **Dependency blockage vs local deficiency:** C.
- **Distributed/interface supply:** A, E.
- **Context-relative sufficiency:** D.
- **Stale and disputed evidence:** F, G.
- **Search boundary:** H.
- **Consequence vs centrality:** I.
- **State vector vs scalar score:** J.
- **Unknown/disputed ownership:** K.
- **Representation gap vs required-function gap:** L.
- **Active-work state:** M.
- **Legitimate no-action/HOLD:** N.
- **State description vs authority:** Throughout; SMM candidates do not authorise allocation, clinical policy, safety declaration, ownership creation, or mandatory development.

## 3. Relevant SMM failure modes

Observed or scenario-pressured failure modes:

- **SMM-F1 — False completeness:** L; H if absence is overstated.
- **SMM-F2 — False maturity:** B.
- **SMM-F3 — Presence/maturity collapse:** B.
- **SMM-F4 — Maturity/sufficiency collapse:** B, D.
- **SMM-F5 — Locality error:** A.
- **SMM-F6 — Interface blindness:** A.
- **SMM-F7 — Dependency blindness:** C.
- **SMM-F8 — Centrality bias:** I.
- **SMM-F9 — Staleness:** F.
- **SMM-F10 — Ownership fabrication:** E, K.
- **SMM-F11 — Authority capture:** J, K, N.
- **SMM-F12 — Score collapse:** J.
- **SMM-F13 — Uncertainty erasure:** F, G, H, J.
- **SMM-F14 — Anti-gaming failure:** B, J.
- **SMM-F15 — History erasure:** G, F.
- **SMM-F16 — Perpetual-development bias:** M, N.

## 4. Specification / interface ambiguities

v0.1 largely transfers, but these points are under-specified:

1. **Presence vs maturity for partially implemented functions.** In B, it is not clear whether missing correction workflow makes presence **PARTIAL** or whether core function is **PRESENT_EXPLICIT** with maturity dimensions **PARTIAL**.
2. **Stale sufficiency semantics.** v0.1 allows “UNKNOWN or prior-state-with-review-due according to host semantics” for F. No default or portability rule is given.
3. **CANDIDATE_ABSENT → REQUIRED_FUNCTION_GAP transition.** H exposes no threshold for when a bounded search is sufficient to classify a required-function gap rather than provisional candidate absence.
4. **Aggregation disclosure rules.** J: “justified bounded purpose” and “does not erase material unresolved dimensions” are not operationalised. Minimum disclosure requirements for an aggregate are absent.
5. **Active-work response mapping.** M: active-work metadata exists, but candidate-response classes do not include an explicit “already active / no new candidacy” state.
6. **Ownership gap representation.** K: unknown/disputed ownership is supported, but there is no explicit “ownership gap” class or required governance interface.
7. **Distributed supply vs single-owner registries.** E: SMM supports distributed suppliers, but interface mapping to a registry with one owner field is not specified.
8. **Dispute resolution / supersession.** G: SMM says DISPUTED must not be silently resolved, but it does not define a formal supersession or review protocol.
9. **Interface evidence responsibility.** A: SMM permits **SATISFIED_INTERFACE** and interface sufficiency, but does not say who must supply/refresh evidence from the external interface supplier.
10. **Consequence/centrality combination.** I: SMM says expose consequence independently of centrality, but does not define how a host should prevent centrality-only ranking downstream.
11. **Context materiality.** D/J: context fields are not all mandatory, but “materially relevant context must not be omitted” lacks a test.

## 5. Mechanism defects vs host/domain choices

**Mechanism-level ambiguities/defects in v0.1:** the items in §4. They are not fatal to the central distinctions, but they can produce inconsistent implementations.

**Host/domain choices or errors in the scenario:**

- Lab A audit labelling sequencing **ABSENT**.
- Lab B programme manager treating **PRESENT** as mature.
- Lab C dashboard labelling software **INSUFFICIENT** when it is dependency-blocked.
- Registry permitting only one owner for distributed incident investigation.
- Ranking tool sorting emergency verification low because of low centrality.
- Executives requesting **82%** without unresolved dimensions.
- Mapping team being asked to invent an owner for K.
- Central registry not representing locally documented QC function.
- Queue generator ignoring **FROZEN_FOR_TEST** active-work state.
- Management requiring every cycle to produce a development action.

These are exactly the host/domain choices SMM is designed to resist.

## 6. Useful unrequested findings

- SMM would benefit from an explicit **context-set record** so D cannot be forced into one label.
- A portable **aggregation disclosure rule** is needed for J-type pressure.
- **Active-work state should be a first-class queue filter**, not merely metadata.
- **Distributed supply** needs a registry interface pattern; single-owner fields are incompatible with E.
- **Representation gap** should be distinguished operationally from **required-function gap** in dashboards.
- **Ownership gaps** need a governance interface; SMM can record them but cannot resolve them.
- **Stale-state semantics** should be host-declared before consequential use.
- **Dispute records** need a supersession protocol to avoid F15/F13.
- **Consequence exposure** should remain independent of dependency centrality in any downstream ranking.
- **No-action/HOLD** must be an explicit legitimate output in every mapping cycle.

## 7. Transfer classification

**SMM-T3 — Functional transfer.**

Rationale: SMM v0.1 transferred into a materially non-Concord clinical-laboratory network domain. Its central distinctions — presence/maturity/sufficiency, local/system absence, interface/distributed supply, dependency blockage, uncertainty/dispute, evidence/freshness, and state-description vs authority — remained usable across A–N. Authority boundaries were preserved: the mapping team cannot allocate resources, change clinical policy, declare safety, invent owners, or force development.

It is not **SMM-T4 — Strong transfer** because several specification/interface ambiguities remain: stale sufficiency semantics, candidate-absence escalation, aggregation disclosure, active-work candidacy, ownership-gap representation, and distributed-supply registry mapping. These are not enough to reduce it to **SMM-T2**, since the core portable mechanism still functions without importing host-specific Concord machinery. As written, v0.1 is best classified as **functional transfer with clarifications required**.
