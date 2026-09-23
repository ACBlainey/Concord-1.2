# Cross Boundary Externality Recognition — Blind Transfer Test 002 — Post-Test Evaluation

**Test:** CBER-BTT-002  
**Specification tested:** v0.2  
**Independent result:** CB-T3 — FUNCTIONAL TRANSFER  
**Evaluation status:** COMPLETE  
**Date:** 23 September 2026

## 1. Overall result

The valid clean-instance test materially confirmed the frozen v0.2 expectations.

**Frozen predictions materially confirmed: 28/28.**

No core architectural failure was exposed.

The second materially different domain confirms that the module transfers beyond the original Concord context and beyond the computing/infrastructure domain used in BTT-001.

The tester nevertheless identified bounded interface and recording ambiguities. These justify its conservative CB-T3 classification and should be resolved before graduation review.

## 2. Prediction audit

**P1 — CONFIRMED.** Valid externality candidate opened.

**P2 — CONFIRMED.** Candidate opening was explicitly separated from escalation.

**P3 — CONFIRMED.** Multiple primary/secondary boundaries were mapped.

**P4 — CONFIRMED.** R was classified as consultation/advocacy/evidence-bearing standing, not authorised representation.

**P5 — CONFIRMED.** L's authorised representation was limited to the two farms.

**P6 — CONFIRMED.** The non-member farm remained visible outside L's representative scope.

**P7 — CONFIRMED.** R's poisoning assertion was separately classified UNSUPPORTED/OVERSTATED.

**P8 — CONFIRMED.** The underlying externality case remained open despite the unsupported assertion.

**P9 — CONFIRMED.** Independent laboratory confirmation strengthened the fact of elevated nitrate readings.

**P10 — CONFIRMED.** Causation remained multi-source and uncertain.

**P11 — CONFIRMED.** U was retained only as a plausible/unconfirmed contributor; no quantitative share was invented.

**P12 — CONFIRMED.** The later decline was not treated as proof of U causation or exoneration.

**P13 — CONFIRMED.** Materiality was context-declared; legal breach, health harm, crop damage and service failure were not inferred.

**P14 — CONFIRMED.** MATERIALITY-UNCERTAIN was applied to the ecological/watershed consequence.

**P15 — CONFIRMED.** M's authority was correctly bounded to monitoring/blending and its own operations.

**P16 — CONFIRMED.** U's voluntary mitigation was not treated as admission of sole responsibility.

**P17 — CONFIRMED.** L could advise members but not bind them beyond granted authority.

**P18 — CONFIRMED.** R's demanded ban was rejected as authority laundering/remedy expansion.

**P19 — CONFIRMED.** Minimum response was actor-relative under fragmented authority.

**P20 — CONFIRMED.** No compensation imposition pathway was invented.

**P21 — CONFIRMED.** CB-C classifications were used dimensionally.

**P22 — CONFIRMED.** The response used C1/C2 for evidence development, C6/C7/C8/C10 for authority/coordination, retained responsibility as unresolved rather than forcing C4, and did not misuse C11 for the whole case.

**P23 — CONFIRMED.** Earlier uncertainty was preserved through later evidence.

**P24 — CONFIRMED.** Relevant laundering and failure-mode risks were identified.

**P25 — CONFIRMED.** Responsibility Mapping ≠ Quantitative Apportionment prevented invented percentages.

**P26 — CONFIRMED.** Primary/secondary boundary mapping worked without requiring one global primary boundary.

**P27 — CONFIRMED.** M's internal investigation threshold was not treated as proof of legal breach/service failure.

**P28 — CONFIRMED.** Tester explicitly found v0.2 usable without Concord source context.

## 3. Cross-test validation

BTT-001:
- domain: interconnected computing / research-data infrastructure;
- frozen predictions: 22;
- materially confirmed: 22;
- result: CB-T3.

BTT-002:
- domain: watershed / agriculture / environmental-resource interaction;
- frozen predictions: 28;
- materially confirmed: 28;
- result: CB-T3.

Combined:

> **50/50 frozen predictions materially confirmed across two materially different non-Concord domains.**

This is strong evidence of specification-level portability, while remaining distinct from empirical validation in real operational systems.

## 4. Remaining issues and disposition

### 4.1 Multi-context materiality
**VALID CLARIFICATION.**

One incident may require multiple materiality records.

Revision:
**MaterialityAssessment = <Consequence, Context, Threshold/Function, State, Evidence, Uncertainty>**

> **One Consequence ≠ One Universal Materiality State**

### 4.2 Authorisation scope
**VALID CLARIFICATION.**

Standing must record not only role but granted scope.

Revision:
**Standing = <Party, Role, Scope, SourceOfAuthority, Limits, State>**

Authority to raise concerns does not imply authority to receive protected information, negotiate, settle, bind, or accept compensation unless separately granted.

### 4.3 Responsibility threshold
**VALID CLARIFICATION.**

The module should distinguish:
- POSSIBLE-CONTRIBUTOR;
- PLAUSIBLE-CONTRIBUTOR;
- SUPPORTED-CONTRIBUTOR;
- CONTRIBUTORY-RESPONSIBILITY;
- responsibility unresolved.

CB-C4 should require supported responsibility, not mere plausibility.

### 4.4 Non-agent and unidentified contributors
**VALID CLARIFICATION.**

Causal mapping should permit:
- actor contributors;
- non-agent environmental/system contributors;
- unidentified/unknown contributors.

Causal contribution and normative responsibility must remain distinct.

> **Causal Contributor ≠ Responsible Party**

### 4.5 CB-C12 placement
**VALID CLARIFICATION.**

CB-C12 should be explicitly dimension-specific where used.

Use:
**CB-C12[dimension] — UNRESOLVED**

A whole-case unresolved label may be used only where closure is insufficient across the case as a whole.

### 4.6 Passive absence versus refusal
**VALID CLARIFICATION.**

CB-C9 requires affirmative refusal/non-participation after a relevant participation pathway exists or is offered.

Passive absence, lack of authorisation or non-involvement should not automatically become refusal.

### 4.7 Assertion-generated externality
**BOUNDARY CLARIFICATION.**

An assertion should become a separate externality candidate only when there is a separately alleged material consequence crossing a boundary.

> **Unsupported Assertion ≠ Automatically Separate Externality**

### 4.8 Primary/secondary boundary selection
**VALID CLARIFICATION.**

Primary boundary should be defined relative to the specific claimed consequence under evaluation: the boundary across which that consequence is alleged to propagate.

Secondary boundaries are dependencies materially relevant to causation, standing, authority or response.

### 4.9 Voluntary shared response without formal interface
**VALID CLARIFICATION.**

Compatible independently chosen actions may be recorded as:
**PARALLEL-VOLUNTARY-COORDINATION**

This does not imply a shared authority or formal institution.

### 4.10 Review triggers
**VALID CLARIFICATION.**

Minimum review trigger record:
**ReviewTrigger = <Condition/Event, AffectedField, RequiredReview, Provenance>**

Triggers may be evidential, materiality, standing, authority, consequence, recurrence or outcome changes.

## 5. Graduation decision

The module has now demonstrated functional transfer twice, with all 50 frozen predictions materially confirmed.

However, both clean testers independently returned **CB-T3 rather than CB-T4**, and BTT-002 exposed ten bounded clarifications.

These do not justify another broad redesign. They justify a final bounded revision to **v0.3 graduation-candidate specification**.

After that revision, a third full blind test is not automatically necessary. Graduation review should determine whether the changes are clarificatory and whether the two existing blind tests provide sufficient transfer evidence.

If graduation review finds any v0.3 change materially alters the mechanism rather than clarifies its interfaces, targeted delta testing should be required before release.

## 6. Evaluation conclusion

> **CBER-BTT-002: PASS AT FUNCTIONAL-TRANSFER LEVEL**

> **28/28 FROZEN PREDICTIONS MATERIALLY CONFIRMED**

> **COMBINED BTT RECORD: 50/50**

> **NO FUNDAMENTAL FAILURE DETECTED**

> **v0.3 BOUNDED CLARIFICATION REVISION AUTHORISED**
