# State and Maturity Mapping — Blind Transfer Test 002 — Post-Test Evaluation

**Test:** SMM-BTT-002  
**Specification tested:** v0.2  
**Method:** PMEDG v1.2  
**Status:** POST-TEST EVALUATION / PASS / BOUNDED REVISION REQUIRED  
**Date:** September 2026

## 1. Result

Independent classification:

> **SMM-T3 — FUNCTIONAL TRANSFER**

Frozen-key result:

> **52 / 52 frozen predictions materially confirmed**

> **0 / 14 fundamental-failure indicators observed**

Decision:

> **SMM-BTT-002: PASS**

> **REVISION TYPE: BOUNDED SPECIFICATION / INTERFACE CLARIFICATION**

> **CROSS-TEST CONVERGENCE REVIEW AUTHORISED**

The second materially different non-Concord domain preserved the SMM core mechanism. The v0.2 clarifications introduced after BTT-001 were operationally used rather than merely repeated as terminology.

## 2. Prediction comparison

SMM2-P01–P03 — **CONFIRMED.** A required an explicit assessment-unit boundary, distinguished composite/subfunction scope, and did not infer whole-function maturity from detection/diagnosis presence.

SMM2-P04–P06 — **CONFIRMED.** B preserved three context-relative sufficiency states, materially reproduced context-set semantics, and treated the one-field dashboard as a host representation limitation rather than authoritative state.

SMM2-P07–P09 — **CONFIRMED.** C preserved the historical SUFFICIENT assessment, flagged material change/staleness, prevented unqualified current SUFFICIENT without revalidation, and did not infer INSUFFICIENT solely from staleness.

SMM2-P10–P12 — **CONFIRMED.** D retained CANDIDATE_ABSENT because materially relevant provider manuals remained unavailable, rejected definitive global absence, and explicitly applied the declared search/source-resolution boundary.

SMM2-P13–P15 — **CONFIRMED.** E preserved PRESENT_DISTRIBUTED, rejected false single-owner invention, and treated the legacy one-owner database as a lossy projection.

SMM2-P16–P17 — **CONFIRMED.** F identified interface-evidence freshness/stewardship as material while leaving ownership of the external evidence outside SMM.

SMM2-P18–P20 — **CONFIRMED.** G preserved R1 and R2, represented R2 as SUPERSEDES/QUALIFIES R1 only for the applicable hot-case regime, and prevented R1 from remaining unqualified current state there.

SMM2-P21–P23 — **CONFIRMED.** H preserved DEVELOPMENT_ACTIVE, emitted CONTINUE_EXISTING_WORK / NO_NEW_CANDIDACY, and identified duplicate queueing as a downstream workflow error rather than a new gap.

SMM2-P24–P26 — **CONFIRMED.** I preserved UNASSIGNED/NO_LEGITIMATE_OWNER_IDENTIFIED, refused to assign mission control merely because an owner was desired, and kept ownership resolution external.

SMM2-P27–P31 — **CONFIRMED.** J rejected an undisclosed scalar-only 91% representation, required aggregate purpose/scope/method disclosure, preserved UNKNOWN/DISPUTED/BLOCKED visibility and high-consequence exceptions, and retained the underlying state vector as authoritative.

SMM2-P32–P34 — **CONFIRMED.** K preserved high consequence despite low centrality, identified centrality-only ranking as lossy/invalid if it erased consequence, and left final priority external.

SMM2-P35–P37 — **CONFIRMED.** L preserved PRESENT_DISTRIBUTED as the source SMM state, identified the export as a lossy projection, and refused to let the one-owner export redefine underlying supply.

SMM2-P38–P40 — **CONFIRMED.** M preserved old and corrected assessments, used CORRECTS explicitly, and rejected destructive overwrite.

SMM2-P41–P42 — **CONFIRMED.** N permitted NO_ACTION/HOLD and identified mandatory development pressure as SMM-F16.

SMM2-P43–P50 — **CONFIRMED.** State description remained separate from mission-command, funding and safety authority; presence, maturity and sufficiency remained distinct; UNKNOWN/DISPUTED remained operational; evidence/provenance/freshness remained material; distributed/interface supply remained first-class; history was preserved; projections did not replace source state; and transfer required no Concord/CDT/KCS/Clock context.

SMM2-P51 — **CONFIRMED.** The evaluator explicitly identified all required failure-mode families: F8, F9, F10, F12, F13, F15 and F16, together with additional relevant modes.

SMM2-P52 — **CONFIRMED.** The eleven v0.2 clarification areas were used operationally across the scenario. The response did not merely restate terminology; it applied the revised rules to concrete spacecraft/ground-segment cases.

## 3. Fundamental-failure indicators

1. Assessment-unit declaration cannot resolve A without Concord-specific architecture — **NOT OBSERVED**.
2. Context-set semantics cannot represent B — **NOT OBSERVED**.
3. Revised stale-state semantics collapse stale into false/insufficient or leave old state unqualified current — **NOT OBSERVED**.
4. Candidate-absence rule still forces unjustified definitive absence — **NOT OBSERVED**.
5. Distributed supply cannot survive a single-owner host schema — **NOT OBSERVED**.
6. Interface evidence stewardship requires SMM to own external evidence — **NOT OBSERVED**.
7. Supersession/history semantics require destructive overwrite — **NOT OBSERVED**.
8. Active-work rule cannot prevent duplicate candidacy — **NOT OBSERVED**.
9. Ownership-gap state necessarily invents authority — **NOT OBSERVED**.
10. Aggregate disclosure cannot preserve unresolved/high-consequence dimensions — **NOT OBSERVED**.
11. Consequence is necessarily subordinated to centrality — **NOT OBSERVED**.
12. Lossy projection necessarily redefines underlying SMM state — **NOT OBSERVED**.
13. No-action/HOLD cannot be represented — **NOT OBSERVED**.
14. State mapping acquires substantive mission/funding/safety authority — **NOT OBSERVED**.

## 4. PMEDG v1.2 finding classification

### Predicted findings

All frozen mechanism-level predictions were materially confirmed. The evaluator reproduced the expected behaviour across assessment-unit boundaries, context sets, stale state, bounded absence, distributed/interface supply, evidence stewardship, history, active work, ownership, aggregation, consequence, lossy projection and legitimate stopping.

### Predicted pressure with novel detail

The evaluator exposed twelve bounded interface/specification refinements inside pressure areas already frozen by the key:

1. **Assessment-unit composition procedure** — the boundary rule works, but v0.2 does not provide a formal decision procedure for composite-function PARTIAL versus DEPENDENCY_BLOCKED versus maturity/sufficiency deficit.
2. **Context-set storage/serialization** — context sets work conceptually, but hosts with one sufficiency field need a portable representation/interface pattern.
3. **Default stale-current semantics** — the revised stale rule works, but the choice between current UNKNOWN and prior-state-with-review-due remains under-specified.
4. **Candidate-absence materiality criterion** — the bounded-search rule works, but “host-appropriate” search sufficiency remains intentionally qualitative and can produce inconsistent escalation.
5. **Distributed-supply serialization** — the lossless projection rule works, but no portable adapter/serialization contract is specified.
6. **Interface-evidence stewardship candidacy** — stewardship can be represented, but no dedicated candidate-response class exists for a missing review owner/process.
7. **Scope-limited assessment relations** — SUPERSEDES/QUALIFIES works, but partial-scope relation semantics should be explicit.
8. **Ownership/governance escalation candidacy** — ownership can remain unassigned without fabrication, but §19 lacks an explicit ownership/governance-escalation response class.
9. **Candidate-response vocabulary consistency** — CONTINUE_EXISTING_WORK / NO_NEW_CANDIDACY exists in §23 but is absent from the §19 canonical candidate-response list.
10. **Aggregate disclosure minimum format/refusal condition** — required fields are defined, but no minimum portable reporting form or refusal threshold is specified.
11. **Consequence-preserving downstream projection** — consequence remains independent of centrality, but downstream ranking interfaces lack an explicit carriage contract.
12. **HOLD versus NO_ACTION semantics** — both are legitimate but their relationship across active-work state and candidate-response state is not fully mapped.

These are bounded clarification/interface issues. None requires replacement of the SMM kernel.

### Wholly unpredicted findings

> **No wholly unpredicted mechanism failure was identified.**

The evaluator's useful unrequested findings all refine pressure areas already deliberately exercised by the frozen test. They therefore fall under **predicted pressure with novel detail**, not retrospective prediction and not wholly new mechanism failure.

## 5. Cross-test significance

BTT-001 established functional transfer in a materially non-Concord laboratory/research setting and exposed bounded specification/interface ambiguities.

BTT-002 used a materially different distributed spacecraft mission-operations domain and deliberately re-pressured the v0.2 corrections. The same core architecture survived:

- presence remained distinct from maturity;
- maturity remained distinct from context-relative sufficiency;
- local absence remained distinct from distributed/interface supply;
- dependency blockage remained distinct from local deficiency;
- bounded non-discovery remained distinct from proven global absence;
- stale state remained distinct from false/insufficient state;
- UNKNOWN/DISPUTED remained operational states;
- consequence remained distinct from centrality;
- projections/aggregates remained distinct from underlying state;
- mapping remained distinct from substantive authority;
- historical state remained preserved;
- legitimate no-action/HOLD remained possible.

The second test therefore strengthens the evidence that BTT-001 success was not dependent on its first transfer domain.

## 6. Evidence-supported bounded revision targets

Before a graduation-candidate specification, a bounded v0.3 revision is justified to resolve the interface ambiguities exposed by BTT-002 without expanding the kernel.

v0.3 should:

1. add a compact decision rule for composite assessment-unit classification;
2. define a portable context-set representation or reference pattern for lossy host schemas;
3. define a default current-state treatment after material change invalidates unqualified current SUFFICIENT;
4. clarify how material unavailable sources affect the candidate-absence escalation threshold without pretending to create a universal quantitative search rule;
5. define a distributed-supply projection/reference contract;
6. explicitly permit interface-evidence review owner/process = UNKNOWN/UNASSIGNED and define the bounded response;
7. formalise scope-limited CORRECTS/SUPERSEDES/QUALIFIES relations;
8. add an explicit OWNERSHIP_GAP / GOVERNANCE_ESCALATION candidate response that remains non-authoritative;
9. harmonise §19 with CONTINUE_EXISTING_WORK / NO_NEW_CANDIDACY;
10. add a minimum aggregate disclosure template and bounded refusal rule;
11. require consequence/exposure carriage through downstream ranking projections where material;
12. distinguish HOLD from NO_ACTION_CANDIDATE explicitly.

## 7. What must not change

Do not:

- replace the SMM kernel;
- turn assessment-unit rules into a universal domain ontology;
- create a universal quantitative source-search threshold;
- require one owner;
- make SMM resolve ownership/governance;
- make SMM own external evidence;
- create a universal aggregate score;
- make centrality a proxy for consequence;
- make SMM a priority/resource engine;
- convert stale into false or automatically insufficient;
- convert candidate absence into certainty;
- require Concord, CDT, KCS or the Civilisation Clock.

## 8. PMEDG decision

> **SMM-BTT-002: PASS**

> **TRANSFER CLASSIFICATION: SMM-T3 — FUNCTIONAL TRANSFER**

> **52 / 52 FROZEN PREDICTIONS MATERIALLY CONFIRMED**

> **0 / 14 FUNDAMENTAL FAILURES OBSERVED**

> **BOUNDED REVISION JUSTIFIED**

> **NO FUNDAMENTAL RETURN TO SOURCE RESOLUTION REQUIRED**

The evidence now supports proceeding to PMEDG Stage 10 — Cross-Test Convergence.

A third blind test is not automatically required. The next decision should be made after the bounded v0.3 clarification and explicit cross-test convergence review: whether any remaining uncertainty concerns the portable mechanism itself, or only implementation/interface precision already exercised in two materially different domains.
