# Continuity Protocol — Blind Transfer Test 002 — Expected Findings and Evaluation Key

**Test:** CP-BTT-002  
**Specification:** Continuity Protocol — Portable Specification v0.2  
**Status:** FROZEN BEFORE INDEPENDENT RESPONSE  
**Date:** 23 September 2026

## 1. Purpose

This key freezes the expected delta-test findings before any independent response is obtained.

Exact wording is not required. Material recovery of the architectural distinction counts as confirmation.

## 2. Frozen predictions

### P1 — Target decomposition
Tester identifies service/function continuity, MAF 1.4m L/day, RTO 18h, RPO 2h and the plant-building/control-equipment disruption envelope as separate constraints.

### P2 — Swift meets MAF function
Swift's verified 1.6m L/day exceeds MAF and its 6h start capability is within RTO.

### P3 — P11 fails overall target because RPO fails
The exercise meets RTO and MAF but its 7-hour-old record set violates the 2-hour RPO. Management's global success claim is rejected.

### P4 — RTO success does not erase RPO failure
Tester explicitly keeps time-to-function and acceptable state/history loss separate.

### P5 — P2 component state does not establish system continuity
Daily archive is meaningful/documented and simulator-restored, but its 24h interval cannot satisfy a 2h RPO by itself.

### P6 — P4 can be actionable for chemistry without being whole-system recovery
Paper procedures are exercised and useful but do not contain control configuration.

### P7 — P12 technically actionable but invalid/currently superseded
Old manual is readable/easy to follow yet must not be used as current restoration guidance.

### P8 — P5 documented future dependency risk
Membrane end-of-production is DOCUMENTED. It matters strongly to Atlas long-term continuity but does not by itself defeat the bounded 18h building-loss claim if existing plant/Swift resources suffice.

### P9 — P6 remains unresolved
The alleged dongle must remain UNRESOLVED; nine years of operation without it is evidence against assuming current dependence but does not prove irrelevance to a total rebuild.

### P10 — P7 knowledge dependency is material
Mira's unexplained transformation rules are a continuity dependency for historical record linkage/migration and should trigger transfer/verification before departure.

### P11 — P15 verified bounded fuel support
72h independent fuel is VERIFIED evidence sufficient for the stated 18h MAF recovery window, but does not prove indefinite/long-duration resilience.

### P12 — Tide preserves function despite implementation replacement
Different membranes/controls/sensors do not constitute continuity failure if required function and continuity state are legitimately transferred.

### P13 — Authority does not equal successful handoff
P9 establishes legitimate authority for Tide once conditions are met; P10 still exposes incomplete knowledge/provenance/interface handoff.

### P14 — CP-C6 does not imply legitimacy
Tester uses succession classification without needing to infer authority; here authority is separately evidenced, but continuity remains incomplete.

### P15 — P13 is continuity fossilisation
The formally designated master plan is operationally stale. Formal designation does not make its dependencies current.

### P16 — Disruption-envelope discipline prevents overclaim
Port closure does not automatically invalidate the bounded plant-building-loss claim because it lies outside the declared envelope.

### P17 — Port risk must not be ignored
Tester records port dependence for a separate/wider disruption or long-duration review rather than dismissing it as irrelevant universally.

### P18 — Object-relative CS use
Tester distinguishes artefact/component state from whole-chain recovery state and avoids promoting one high-state component into CP-C1.

### P19 — C2/C7/C9 decomposition remains usable
Tester can use aggregate-below-target, specific dependency-gap and unverified-claim classifications together where appropriate rather than treating them as exclusive.

### P20 — Evidence states reduce speculative classification
VERIFIED/DOCUMENTED/INFERRED/UNRESOLVED are materially used to avoid converting P5/P6/P7/P15 into unsupported binary claims.

### P21 — Recovery evidence must exceed dependency listing
Tester does not grant CP-C4 merely because dependencies have names; an evidenced recovery basis is required.

### P22 — Continuity mechanism itself requires review
The stale spreadsheet demonstrates that a continuity mechanism can lose continuity/correctness and must itself be reviewed/replaced.

## 3. Expected classification pressure

### Swift MAF functional recovery
Expected: strong evidence for MAF and RTO capability, but the overall declared target must still account for RPO. Depending on audit object, C1 may be justified for the narrow Swift functional-MAF target while the wider claim fails.

### P11 overall target
Expected: not C1. C2 and/or C9 appropriate because RPO is violated despite successful functional recovery.

### Atlas rebuild dependencies
Expected: C7 for established material gaps such as disappearing membrane path/tacit mapping where relevant; C10 for dongle uncertainty. Exact scope must respect disruption envelope.

### Tide succession
Expected: C6 plus C2/C7/C9 as needed for incomplete historical mapping/handoff. Authority is separately established by P9, so no succession-as-legitimacy error should be alleged merely because C6 is used.

### Master continuity spreadsheet
Expected: below current target and evidence of F17 continuity fossilisation; formal designation must not confer current correctness.

## 4. Material failure indicators

Material concern if the specification drives the tester to:

- declare P11 successful solely because RTO was met;
- require Swift to reproduce full 4.0m L/day despite explicit MAF;
- treat 72h fuel as proof of indefinite resilience;
- declare the dongle definitely required or definitely irrelevant;
- reject Tide merely because implementation changes;
- treat P9 authority as proof of complete handoff;
- use the superseded 2018 manual operationally because it is actionable;
- treat the stale spreadsheet as current because it is formally designated;
- fail the bounded plant-loss claim solely because port closure exists outside its envelope;
- ignore port dependency in all wider contexts;
- treat dependency names alone as CP-C4 evidence.

## 5. Delta-test success criteria

**CP2-T1 — DELTA FAILURE:** v0.2 refinements create or fail to resolve material ambiguity.

**CP2-T2 — PARTIAL DELTA SUCCESS:** most refinements work but at least one central new concept requires major redesign.

**CP2-T3 — STRONG DELTA SUCCESS:** new concepts transfer independently; nearly all P1–P22 confirmed; remaining issues are minor clarification.

**CP2-T4 — GRADUATION-CANDIDATE TRANSFER:** all or nearly all predictions materially confirmed, no blocking architectural defect exposed, and remaining changes are editorial/bounded rather than structural.

These labels apply only to portable-development testing.

## 6. Frozen expectation

Expected result is that v0.2 will make target boundaries more explicit than v0.1 and prevent several overclaims that BTT-001 showed were possible.

The highest-risk pressure points are:

1. whether MAF and RPO interact cleanly;
2. whether disruption-envelope scoping is mistaken for permission to ignore wider risks;
3. whether evidence state and dependency criticality remain understandable without becoming bureaucratic;
4. whether C6 remains clearly separate from authority and completed handoff;
5. whether object-relative CS classification is applied consistently.

No prediction may be altered after the independent response is obtained.
