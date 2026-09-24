# SMM-BTT-002 — Independent Evaluator Response

**Specification under test:** State and Maturity Mapping — Portable Specification v0.2  
**Test:** SMM-BTT-002  
**Domain:** Distributed spacecraft mission operations / ground-segment readiness  
**Method:** PMEDG v1.2  
**Status:** Independent evaluator response; no Concord, CDT, KCS, Civilisation Clock, BTT-001 or prior SMM history assumed.

## 1. Overall result

SMM v0.2 transfers into the Helios Deep-Space Consortium domain. The core distinctions — presence vs maturity, maturity vs context-relative sufficiency, local vs distributed/interface supply, dependency blockage vs local deficiency, stale vs false, UNKNOWN/DISPUTED vs binary classification, state description vs authority — remain usable and materially load-bearing.

**Transfer classification: SMM-T3 — Functional transfer.**  
No fundamental mechanism failure was forced. Residual issues are specification/interface ambiguities and host/schema choices, not collapse of the portable mechanism. SMM-T4 is not warranted because several interface ambiguities remain, especially around scope-limited supersession, ownership-gap candidacy, aggregate disclosure format and lossy single-owner projection.

## 2. Scenario mapping A–N

| Case | SMM v0.2 mapping | Key resolution | Bounded candidacy |
|---|---|---|---|
| **A — Assessment-unit boundary** | Declare boundary explicitly. Detection/diagnosis and recovery execution are distinct sub-units. If the assessed unit is the whole autonomous fault-management function, presence is not automatically PARTIAL merely because recovery is disabled. Recovery execution is supplied but disabled pending validation → `DEPENDENCY_BLOCKED` for operational use; whole-function sufficiency for autonomous context is `BLOCKED`. For fault detection/diagnosis context, `SUFFICIENT`. | The dispute is a presence/sufficiency collapse. `PRESENT_EXPLICIT` and `PARTIAL` are both wrong if used without a declared boundary. | `RESOLVE_UPSTREAM_CANDIDATE` — validation prerequisite. |
| **B — Context set** | Preserve explicit context set. C1 routine cruise correction planning: `SUFFICIENT`. C2 distant approach analysis: `CONDITIONALLY_SUFFICIENT`. C3 autonomous close-approach execution: `INSUFFICIENT` or `UNKNOWN` pending validation. One dashboard sufficiency field is a host representation limit. | Do not force one context-free sufficiency label. | `IMPROVE_MAP_OR_EVIDENCE` for dashboard/context-set representation. |
| **C — Stale state after material change** | Prior `SUFFICIENT` remains historically valid. Since encryption hardware and staffing changed, stale-state flag = TRUE, changed-since-review = TRUE. Current sufficiency = `UNKNOWN` or prior-state-with-review-due according to host semantics. Not automatically `INSUFFICIENT`. | Revised stale-state rule applies: stale creates review pressure, does not invert prior state. | `INVESTIGATION_CANDIDATE` / review. |
| **D — Candidate absence** | `CANDIDATE_ABSENT`, not definitive `REQUIRED_FUNCTION_GAP`. Search boundary is incomplete because two external tracking-provider operational manuals remain unavailable. Residual uncertainty must be recorded. | Revised threshold not met. No supply found within current boundary ≠ proven global absence. | `SOURCE_RESOLUTION` / `INVESTIGATION_CANDIDATE`. |
| **E — Distributed supply into one-owner schema** | Orbit determination is `PRESENT_DISTRIBUTED` across mission navigation, two external tracking networks and ephemeris service. Legacy one-owner field is a lossy projection. It must not redefine underlying SMM state. | Preserve distributed supply. Single-owner field may reference a distributed-supply record; it must not invent one owner. | `IMPROVE_MAP_OR_EVIDENCE`. |
| **F — Interface evidence stewardship** | Radiation monitoring is `INTERFACE_SATISFIED`. Evidence source = external space-weather service. Review owner/process = `UNKNOWN` / `UNASSIGNED`. Validation scope and service-change checks are not owned. Freshness is due. Sufficiency may be `CONDITIONALLY_SUFFICIENT` or `UNKNOWN`. | Interface-supplied ≠ locally implemented. Evidence does not remain valid forever. | `IMPROVE_MAP_OR_EVIDENCE` or `INTERFACE_OR_INTEGRATION_CANDIDATE`. |
| **G — Disputed/superseding assessments** | R1 `SUFFICIENT` for original scope. R2 `CONDITIONALLY_SUFFICIENT` for hot-case regime. R2 `SUPERSEDES` or `QUALIFIES` R1 for that regime only. If another team displays R1 as current for hot-case, record `DISPUTED` / representation error. | Later assessment must not silently erase earlier one. Supersession is scope-limited. | `PRESERVE_AND_REVIEW_CANDIDATE`. |
| **H — Active work duplicate selection** | Communications resilience gap is already `DEVELOPMENT_ACTIVE` with funded mitigation and frozen verification plan. The underlying gap remains open, but active work exists. | Do not create duplicate development candidacy merely because gap remains open. | `CONTINUE_EXISTING_WORK / NO_NEW_CANDIDACY`. |
| **I — Ownership gap** | Cross-organisational telemetry-format integration deficit is confirmed. Each organisation owns its own interface; no actor has authority over joint reconciliation function. Presence: `CANDIDATE_ABSENT` / `REQUIRED_FUNCTION_GAP` depending search boundary. Ownership: `UNASSIGNED/NO_LEGITIMATE_OWNER_IDENTIFIED`. | Mapping team cannot assign mission control as owner. Need for owner ≠ authority to invent one. | `NEW_FUNCTION/ARCHITECTURE_CANDIDATE` plus external governance escalation. |
| **J — Aggregate pressure** | A single “mission readiness 91%” is an aggregate projection. It may be used only with justified bounded purpose and mandatory disclosure of UNKNOWN, DISPUTED, BLOCKED, high-consequence exceptions and freshness/evidence boundary. Here it must disclose one DISPUTED thermal capability, one UNKNOWN stale emergency-command capability, and the high-consequence low-centrality abort-support issue. | Aggregate convenience ≠ state truth. The 91% must not hide exceptions. | `IMPROVE_MAP_OR_EVIDENCE` if 91% is presented without disclosure. |
| **K — Consequence vs centrality** | Safe-mode recovery knowledge path has low centrality but high consequence. Recent simulation found interface incomplete. Sufficiency for relevant severe-anomaly context is `INSUFFICIENT` or `CONDITIONALLY_SUFFICIENT`. Consequence/exposure must remain available independently of centrality ranking. | Low centrality ≠ low consequence. Graph ranking must not erase mission-survival exposure. | `DEVELOP_EXISTING_OWNER_CANDIDATE` or `INTERFACE_OR_INTEGRATION_CANDIDATE`. |
| **L — Lossy representation** | Source SMM record is correct: antenna allocation = `PRESENT_DISTRIBUTED` across three organisations. Legacy export drops two suppliers. Later analyst treating export as authoritative is a `REPRESENTATION_GAP`. | Lossy projection must not redefine underlying SMM state. | `IMPROVE_MAP_OR_EVIDENCE`. |
| **M — Explicit assessment relation** | New software-command validation assessment corrects earlier wrong-build report. Record relation: new assessment `CORRECTS` old report. Do not overwrite/destroy old record. Old remains historical evidence. Current state updates with provenance. | Current state must not silently erase path to current state. | Preserve history; update record. No destructive overwrite. |
| **N — No-action/hold** | Star-tracker calibration is `SUFFICIENT`, fresh evidence, no unresolved applicable requirements, no active material blocker. Host process template requiring development for every mapped function is a host policy conflict. | SMM must permit no-action/HOLD. No current development candidate ≠ perfect system. | `NO_ACTION_CANDIDATE` / `HOLD`. |

## 3. Required analysis summary

1. **A–N mapped.** See table.
2. **A resolved by explicit assessment-unit boundary.** The dispute is not resolved by choosing `PRESENT_EXPLICIT` or `PARTIAL`; it is resolved by declaring whether the unit is “fault detection/diagnosis,” “autonomous recovery execution,” or the composite. Recovery execution is present but disabled → dependency-blocked sufficiency, not absent presence.
3. **B represented by context-set semantics.** Three contexts retained; dashboard one-field limit is a representation gap.
4. **C revised stale-state rule applied.** Prior SUFFICIENT preserved; current state review-due/UNKNOWN; stale ≠ false.
5. **D does not meet revised `REQUIRED_FUNCTION_GAP` threshold.** It remains `CANDIDATE_ABSENT` pending source resolution.
6. **E/L distributed supply preserved.** One-owner schema and lossy export are not allowed to redefine SMM state.
7. **F interface-evidence stewardship applied.** Interface-satisfied capability requires provider, refresh owner/process, freshness, validation scope and uncertainty. Missing review owner recorded, not fabricated.
8. **G/M assessment history and relations preserved.** R2 `SUPERSEDES/QUALIFIES` R1 for hot-case; M new assessment `CORRECTS` old wrong-build report.
9. **H duplicate development candidacy suppressed.** `CONTINUE_EXISTING_WORK / NO_NEW_CANDIDACY`.
10. **I unresolved ownership preserved.** Mission control not assigned; owner state `UNASSIGNED/NO_LEGITIMATE_OWNER_IDENTIFIED`.
11. **J aggregate disclosure contract applied.** 91% is not state truth without mandatory disclosures.
12. **K consequence preserved despite low centrality.** High-consequence low-centrality abort/safe-mode issue remains visible.
13. **N no-action/HOLD permitted.** Process template cannot force development recommendation.

## 4. Relevant SMM failure modes

- **A:** SMM-F3 presence/maturity collapse; SMM-F4 maturity/sufficiency collapse.
- **B:** SMM-F4 maturity/sufficiency collapse; SMM-F13 uncertainty erasure.
- **C:** SMM-F9 staleness.
- **D:** SMM-F1 false completeness; SMM-F13 uncertainty erasure.
- **E/L:** SMM-F5 locality error; SMM-F6 interface blindness; SMM-F10 ownership fabrication; SMM-F1 false completeness.
- **F:** SMM-F6 interface blindness; SMM-F9 staleness.
- **G/M:** SMM-F15 history erasure; SMM-F13 uncertainty erasure.
- **H:** SMM-F16 perpetual-development bias / duplicate development pressure.
- **I:** SMM-F10 ownership fabrication; SMM-F11 authority capture.
- **J:** SMM-F12 score collapse; SMM-F8 centrality bias; SMM-F13 uncertainty erasure.
- **K:** SMM-F8 centrality bias.
- **N:** SMM-F16 perpetual-development bias.

## 5. Specification/interface ambiguities

1. **Assessment-unit composition.** v0.2 states that missing subfunction ≠ automatically partial, but does not give a formal decision procedure for when a composite function is `PARTIAL`, `DEPENDENCY_BLOCKED`, or a maturity/sufficiency deficit.
2. **Context-set storage.** v0.2 requires context sets, but does not define portable syntax for hosts with one sufficiency field per capability.
3. **Stale-state current label.** v0.2 allows “UNKNOWN or prior-state-with-review-due according to host semantics.” This leaves a host choice that could cause inconsistent reporting.
4. **Candidate-absence threshold.** “Host-appropriate search/source-resolution boundary” is not quantified. When are unavailable manuals material enough to block `REQUIRED_FUNCTION_GAP`?
5. **Lossy single-owner projection.** v0.2 says a single-owner field may reference a distributed-supply record, but no portable serialization or interface contract is given.
6. **Interface-evidence review ownership.** v0.2 requires recording refresh/review owner/process, but no candidate class is dedicated to missing interface-evidence stewardship. It must be mapped to `IMPROVE_MAP_OR_EVIDENCE` or `INTERFACE_OR_INTEGRATION_CANDIDATE` by host judgment.
7. **Scope-limited supersession.** v0.2 lists `SUPERSEDES`, `QUALIFIES`, `CORRECTS`, etc., but does not formalise partial-scope relations such as “R2 supersedes R1 only for hot-case regime.”
8. **Ownership-gap candidacy.** v0.2 preserves `UNASSIGNED/NO_LEGITIMATE_OWNER_IDENTIFIED`, but the §19 candidate list has no explicit ownership/governance-escalation candidate.
9. **Candidate vocabulary inconsistency.** `CONTINUE_EXISTING_WORK / NO_NEW_CANDIDACY` appears in §23 but is not listed in the §19 candidate-response classes.
10. **Aggregate disclosure format.** v0.2 lists required disclosure fields, but does not specify minimum machine-readable format or when an aggregate should be refused.
11. **Consequence preservation through downstream ranking.** v0.2 requires consequence/exposure to remain available, but does not specify how downstream centrality-based rankings must carry it.
12. **HOLD vs NO_ACTION.** v0.2 permits both `HOLD` active-work state and `NO_ACTION_CANDIDATE`, but their relationship is not fully mapped.

## 6. Mechanism defects vs host/domain choices

### Mechanism failures
No fundamental SMM mechanism failure was observed. The core invariants survived all A–N pressures. The most notable specification-level weakness is not a mechanism defect but an interface inconsistency: §23 introduces `CONTINUE_EXISTING_WORK / NO_NEW_CANDIDACY` while §19 does not list it among candidate responses. This is a specification/interface ambiguity, not a collapse of the portable mechanism.

### Host/domain choices
- **A:** Host choice of assessment-unit granularity.
- **B:** Host dashboard schema forcing one sufficiency field.
- **C:** Host choice between `UNKNOWN` and prior-state-with-review-due.
- **D:** Host declaration of search/source-resolution boundary.
- **E/L:** Legacy single-owner database schema and export semantics.
- **F:** Host governance choice about who owns interface-evidence refresh.
- **G:** Host display/current-state policy when R1 and R2 disagree.
- **H:** Host readiness-queue duplicate-selection workflow.
- **I:** Host authority/governance process; SMM cannot assign mission control.
- **J:** Host aggregation purpose, weighting, and disclosure format.
- **K:** Host severity/consequence scale and centrality ranking export.
- **N:** Host process template requiring development recommendation for every mapped function.

## 7. Transfer classification

**SMM-T3 — Functional transfer.**

Rationale: SMM v0.2 transferred into a materially different non-Concord domain. It preserved all core distinctions, produced bounded non-authoritative candidacy, handled context sets, stale state, distributed supply, interface evidence, assessment history, duplicate active work, unresolved ownership, aggregate pressure, consequence vs centrality, lossy representation, explicit correction, and no-action/HOLD. No fundamental failures occurred. Strong transfer (`SMM-T4`) is not claimed because several interface ambiguities remain, especially around scope-limited supersession, ownership-gap candidacy, lossy schema projection, and candidate-vocabulary consistency.

## 8. Useful unrequested findings

- SMM v0.2 would benefit from an explicit **OWNERSHIP_GAP / GOVERNANCE_ESCALATION** candidate class.
- A portable **scope-limited assessment relation** pattern would help cases like G.
- A **distributed-supply serialization adapter** would reduce E/L lossy-schema risk.
- The candidate-response list in §19 should be harmonised with §23.
- The aggregate disclosure contract should include a minimum reporting template.
- The stale-state rule should state a default host semantic for current sufficiency when material change is present.
- The interface-evidence stewardship rule should explicitly allow “review owner UNKNOWN” as a first-class state without forcing a local owner.
