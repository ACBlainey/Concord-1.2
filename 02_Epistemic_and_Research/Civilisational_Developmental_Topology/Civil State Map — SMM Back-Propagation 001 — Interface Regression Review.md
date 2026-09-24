# Civil State Map — SMM Back-Propagation 001 — Interface Regression Review

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Status:** INTERFACE REGRESSION REVIEW — PASS WITH TWO BOUNDED FOLLOW-UPS
**Subject:** Civil State Map Companion Upgrade — SMM Back-Propagation 001
**Interfaces reviewed:** KCS Companion Upgrade 001; Civilisation Clock Companion Extension 001; Civilisational Developmental Topology / parent Civil State Map
**Date:** 24 September 2026

---

## 1. Purpose

This review performs the bounded interface regression required by Section 18 of **Civil State Map Companion Upgrade — SMM Back-Propagation 001**.

The question is not whether the portable SMM module transfers again.

That was already tested during PMEDG.

The question here is narrower:

> **Do the twelve returned SMM refinements fit the existing Concord KCS, Civilisation Clock and CDT/State Map interfaces without contradiction, authority expansion or destructive duplication?**

The review treats the current canonical/companion documents as the integration boundary.

## 2. Decision rule

A returned refinement passes where the receiving architecture can represent or consume its semantics without:

- contradicting an existing canonical rule;
- creating a duplicate owner for an existing capability;
- transferring authority into the State Map;
- destroying provenance/history;
- collapsing UNKNOWN/DISPUTED;
- or requiring a different topology merely to make the State Map easier to operate.

A **bounded follow-up** is recorded where the semantics are compatible but the receiving interface should be explicitly strengthened before the loop is considered fully closed.

## 3. KCS interface regression

### 3.1 Assessment-history relations

Returned SMM relations:

- CORRECTS
- SUPERSEDES
- QUALIFIES
- DISPUTES
- CONFIRMS

KCS already contains typed material relations including **CORRECTS**, **SUPERSEDES**, **REVIEWS**, **PRESERVES** and **EVIDENCES**, plus explicit historical state/change records.

KCS correction propagation also requires the previous state to be preserved, the correction recorded, affected dependents identified and review outcomes retained.

Therefore SMM's assessment-history semantics are structurally compatible with KCS.

**Finding:** **PASS / BOUNDED VOCABULARY EXTENSION**

**QUALIFIES, DISPUTES and CONFIRMS** are not currently named as shared KCS core dependency relations. They do not contradict KCS, but if State Map assessment relations are to be stored directly in KCS, these should either:

1. be added as bounded provenance/assessment relation types; or
2. be explicitly mapped to existing KCS provenance/status structures.

They must not be silently treated as synonyms where their meanings differ.

### 3.2 Distributed supply

KCS explicitly supports multiple legitimate suppliers and roles including PRIMARY, CO-OWNER, DISTRIBUTED_SUPPLIER, DELEGATED, INTERFACE_SUPPLIER and FALLBACK.

The SMM rule that a one-owner projection must not collapse distributed supply therefore reinforces rather than duplicates KCS.

The optional `DS_REF` is a State Map reference to KCS/live supply state, not a second ownership database.

**Finding:** **PASS**

### 3.3 Interface evidence stewardship

KCS supports provenance, evidence, confidence, freshness, review dates, UNKNOWN and DISPUTED relations/ownership.

SMM allowing a refresh/review owner to remain UNKNOWN or UNASSIGNED is compatible with KCS's existing rule that unknown must not silently become absent and disputed must not silently become false.

**Finding:** **PASS**

### 3.4 Material-change review and history

KCS change propagation produces a **review set**, not automatic invalidation:

**Change(x) → CandidateReview(y)**

SMM's stale-current rule similarly does not declare the old state false. It preserves the historical assessment while preventing an unreviewed old SUFFICIENT state from masquerading as current after a material change.

The two mechanisms are complementary:

**KCS material change → affected State Map record identified → current sufficiency becomes review-due/UNKNOWN where material → reassessment → preserved history → bounded further propagation if state materially changes.**

**Finding:** **PASS**

### KCS result

> **KCS INTERFACE: PASS WITH ONE BOUNDED VOCABULARY FOLLOW-UP**

No duplicate ownership system, provenance conflict or authority transfer was found.

## 4. Civilisation Clock interface regression

### 4.1 Consequence/exposure carriage

The parent State Map already supplies consequence/exposure to the Clock.

The Clock trigger record already includes consequence class, and RISK is an explicit trigger class.

The SMM refinement therefore strengthens the projection contract: if a Clock queue/ranking omits material consequence/exposure, it must retain a lossless reference or identify the projection as incomplete/lossy.

This does not make consequence the sole priority rule.

**Finding:** **PASS**

### 4.2 Existing work and duplicate candidacy

The parent State Map already records active development state specifically so the Clock can avoid repeatedly selecting work already in progress.

The returned response:

**CONTINUE_EXISTING_WORK / NO_NEW_CANDIDACY**

is therefore an explicit output for behaviour already intended by the source architecture.

It does not hide the underlying insufficiency; it changes only whether a duplicate new candidate should be created.

**Finding:** **PASS**

### 4.3 Ownership gap

The Clock trigger record already distinguishes legitimate action owner and review owner.

The State Map's:

**OWNERSHIP_GAP / GOVERNANCE_ESCALATION_CANDIDATE**

does not give the Clock authority to appoint an owner.

It creates a review candidate whose substantive resolution remains with legitimate governance/constitutional machinery.

This is compatible with the Clock invariant:

> **Triggering Review ≠ Authority Over Outcome**

**Finding:** **PASS**

### 4.4 UNKNOWN (REVIEW DUE)

The Clock already supports STATE, DEPENDENCY, EVIDENCE and RISK triggers and a candidate **REVIEW-DUE** trigger state.

SMM's stale-current default can therefore create review pressure without becoming an automatic insufficiency finding or automatic action.

The correct flow is:

**material change → State Map current sufficiency UNKNOWN (REVIEW DUE) → Clock review trigger/candidate → legitimate reassessment → new state**

not:

**material change → automatic development command.**

**Finding:** **PASS**

### 4.5 HOLD versus NO_ACTION_CANDIDATE

HOLD belongs to State Map active-development/workflow state.

NO_ACTION_CANDIDATE belongs to State Map candidate-response output.

The Clock can consume both without semantic collision if it preserves those fields separately.

A held existing development process may coexist with a finding that no new candidate should be generated.

Neither means permanent completion.

**Finding:** **PASS**

### 4.6 Trigger-state edge condition

The Clock companion currently includes REVIEW-DUE and UNKNOWN but its provisional trigger-state vocabulary predates the later graduated State Triggered Review Architecture and does not yet contain every later trigger lifecycle refinement.

That is not caused by SMM back-propagation and does not block this integration.

It is, however, additional evidence for the wider portable-module back-propagation programme.

**Finding:** **PASS / EXTERNAL BACK-PROPAGATION ISSUE NOTED**

### Clock result

> **CIVILISATION CLOCK INTERFACE: PASS**

No priority capture, authority transfer or duplicate-development contradiction was found.

## 5. CDT / parent State Map regression

### 5.1 Assessment-unit rule versus canonical topology

The returned assessment-unit decision rule explicitly states that it is not a universal ontology and that a separate function should be assessed separately or through an interface/dependency.

It therefore does not authorise assessors to rewrite CDT topology merely to simplify State Map classification.

If the correct unit is uncertain, UNKNOWN/DISPUTED remains available.

**Finding:** **PASS**

### 5.2 Multi-context representation

The parent State Map already makes sufficiency context-sensitive and records consequence context.

The returned context-set rule extends representation when one function has materially different states across contexts.

No contradiction is created.

The optional `CTX_REF` is a reference pattern, not a new CDT node type.

**Finding:** **PASS**

### 5.3 Distributed supply

The parent State Map already records legitimate owner, distributed suppliers, interface suppliers and fallback.

The returned distributed-supply rule therefore protects an existing concept from lossy projection rather than changing the topology.

**Finding:** **PASS**

### 5.4 Candidate absence and ESCP

The parent State Map already requires source resolution before declaring absence.

The returned escalation rule makes the boundary more conservative by preventing a bounded failed search from becoming global certainty and by preserving UNKNOWN where materially relevant sources remain unavailable.

This is consistent with ESCP rather than an alteration of it.

**Finding:** **PASS**

### 5.5 Aggregate safeguards

The parent State Map rejects a universal maturity score.

The returned aggregate rule applies only when a bounded downstream use nevertheless produces a summary/aggregate.

It therefore protects the source invariant rather than weakening it.

**Finding:** **PASS**

### 5.6 State history and CurrentState

The parent architecture already requires prior states to remain reconstructable and represents current integrated systems as:

**CurrentState(system) = Foundation + ApplicableCompanions + Interfaces.**

Scoped CORRECTS/SUPERSEDES/QUALIFIES/DISPUTES/CONFIRMS relations make that history more explicit without replacing the foundation-plus-companions model.

**Finding:** **PASS**

### CDT / State Map result

> **CDT / STATE MAP INTERFACE: PASS**

No topology distortion or ESCP regression was found.

## 6. Twelve-refinement regression matrix

| ID | Refinement | KCS | Clock | CDT/State Map | Result |
|---|---|---|---|---|---|
| BP-SMM-01 | Assessment-unit resolution | Compatible | Neutral | Compatible | PASS |
| BP-SMM-02 | Context-set preservation | Reference/provenance compatible | Projection compatible | Native extension | PASS |
| BP-SMM-03 | Candidate-absence escalation | Evidence compatible | Investigation routing compatible | ESCP strengthening | PASS |
| BP-SMM-04 | Aggregate disclosure/refusal | Source trace compatible | Queue projection compatible | Protects no-universal-score rule | PASS |
| BP-SMM-05 | Consequence carriage | Reference compatible | Directly compatible | Existing consequence field strengthened | PASS |
| BP-SMM-06 | Existing-work suppression | Active-state compatible | Directly compatible | Existing intent formalised | PASS |
| BP-SMM-07 | Ownership-gap escalation | Unknown/disputed owner compatible | Review candidate compatible | Authority boundary preserved | PASS |
| BP-SMM-08 | Interface-evidence stewardship | Directly compatible | Review trigger compatible | Existing interface state strengthened | PASS |
| BP-SMM-09 | Distributed-supply preservation | Directly compatible | Projection compatible | Existing distributed supply protected | PASS |
| BP-SMM-10 | Stale-current sufficiency | Change propagation compatible | REVIEW-DUE compatible | Freshness rule strengthened | PASS |
| BP-SMM-11 | Scoped assessment relations | Compatible; vocabulary follow-up | Review propagation compatible | History strengthened | PASS |
| BP-SMM-12 | HOLD vs NO_ACTION | History/state compatible | Directly compatible | Existing vocabularies clarified | PASS |

**Regression total: 12 / 12 PASS.**

## 7. Authority regression

The integrated architecture remains:

**CDT → KCS → Civil State Map → Civilisation Clock → legitimate owner/governance process**

No returned SMM refinement permits the State Map to:

- command development;
- allocate resources;
- appoint owners;
- determine constitutional outcomes;
- replace KCS;
- replace the Clock;
- or define universal maturity/consequence scales.

**Authority regression:** **NONE OBSERVED**

## 8. Epistemic regression

The integration preserves:

- UNKNOWN;
- DISPUTED;
- provisional candidate absence;
- stale ≠ false;
- bounded search ≠ global absence;
- aggregate ≠ underlying state;
- historical assessment ≠ current assessment after material change.

**Epistemic regression:** **NONE OBSERVED**

## 9. Two bounded follow-ups

### Follow-up A — KCS assessment-relation mapping

Before machine implementation, specify whether **QUALIFIES, DISPUTES and CONFIRMS** become explicit KCS provenance/assessment relation types or are represented through an existing KCS status/provenance structure.

This is a vocabulary/interface formalisation issue, not a mechanism conflict.

### Follow-up B — Clock back-propagation remains separate

The Clock companion itself predates later portable STRA lifecycle refinements.

That issue should be handled by the separate portable-module back-propagation programme rather than smuggled into the SMM integration.

No STRA-specific change is required to validate the SMM companion.

## 10. Integration decision

The SMM companion has passed the bounded source-interface regression.

Formal result:

> **KCS INTERFACE: PASS WITH BOUNDED VOCABULARY FOLLOW-UP**

> **CIVILISATION CLOCK INTERFACE: PASS**

> **CDT / STATE MAP INTERFACE: PASS**

> **TWELVE SMM REFINEMENTS: 12 / 12 PASS**

> **AUTHORITY REGRESSION: NONE OBSERVED**

> **EPISTEMIC REGRESSION: NONE OBSERVED**

> **SMM BACK-PROPAGATION COMPANION: INTEGRATION VALIDATED AT ARCHITECTURAL INTERFACE LEVEL**

This establishes architectural compatibility.

It does not establish implementation correctness or empirical outcome validity.

## 11. State transition

The appropriate source-side state transition is now:

**Civil State Map + SMM Back-Propagation 001**
→ **INTEGRATED / ARCHITECTURAL INTERFACE RETEST PASSED**

The companion may therefore be treated as part of the current integrated Civil State Map architecture, subject to its stated corrigibility and the bounded KCS vocabulary follow-up.

## 12. Back-propagation-method finding

The SMM pilot has now completed the full proposed loop:

**source identification**
→ **post-extraction delta reconstruction**
→ **evidence-origin check**
→ **source-applicability classification**
→ **bounded companion upgrade**
→ **cross-interface regression**
→ **integration decision**

The loop successfully distinguished semantic source improvements from optional portable serialization and did not require replacing the source kernel.

That is positive evidence that a controlled portable-module back-propagation audit is workable as a Concord maintenance method.

# Conclusion

The SMM refinements can be returned to the Civil State Map without destabilising KCS, the Civilisation Clock or CDT.

The result is not a portable module pasted back into its source.

It is an evidence-traced, bounded reintegration of the refinements that survived independent transfer testing and remained applicable to the Concord architecture.

The first portable-module back-propagation loop is therefore architecturally closed.
