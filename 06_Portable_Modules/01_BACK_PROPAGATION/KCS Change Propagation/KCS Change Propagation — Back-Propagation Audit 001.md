# KCS Change Propagation — Back-Propagation Audit 001

**Portable module:** KCS Change Propagation — Portable Module v1.0
**Status:** SOURCE UPDATE CANDIDATE — BOUNDED
**Primary source:** KCS Companion Upgrade 001 — Operational Dependency and Change-Propagation Architecture
**Date:** 24 September 2026

## Purpose

This audit compares the graduated KCS Change Propagation portable module with its Concord source companion after PMEDG development.

It deliberately tests whether the back-propagation process can distinguish a module whose source was already highly developed from the stronger source deltas found in SMM and STRA.

> **Portable Difference ≠ Source-System Improvement**

## Source continuity

The source already contains nearly the entire KCS Change Propagation kernel:

- dependency graph and typed material relations;
- provenance, state and history;
- contextual materiality/criticality;
- upstream/downstream traversal;
- change events;
- CandidateReview rather than AutomaticRejection;
- selective propagation;
- correction propagation;
- supersession;
- alternatives;
- distributed ownership/supply;
- UNKNOWN and DISPUTED;
- freshness/review;
- CDT, State Map, Clock, Continuity and Active Development interfaces;
- privacy/purpose-bounded access;
- anti-centralisation;
- ESCP protection;
- bounded operational testing and falsification.

The graduated portable module therefore does not expose a missing source architecture comparable to the STRA case.

## Delta register

### KCP-BP-01 — REFERENCES relation

Portable v1.0 adds **REFERENCES** to the shared relation vocabulary.

This is materially distinct from **EVIDENCES**: a document may merely point to a current object without itself evidencing the object's substantive state.

**Classification:** Clarification / interface improvement.

**Decision:** INCORPORATE.

### KCP-BP-02 — Document-role distinction

Portable v1.0 explicitly distinguishes a document that:

- contains changed content and may require revision;
- evidences a dependency/state;
- merely references another object.

This prevents reference-only documents from inheriting every substantive downstream change.

**Classification:** General improvement / cascade-control clarification.

**Decision:** INCORPORATE.

### KCP-BP-03 — Dependency record Visibility field

Portable v1.0 adds **Visibility** to the dependency record.

The source already has a strong purpose-bounded access section, so this is not a new privacy principle. It closes the representation gap between the privacy rule and the dependency record.

**Classification:** Clarification / interface improvement.

**Decision:** INCORPORATE SEMANTIC FIELD; implementation remains access-control-system defined.

### KCP-BP-04 — Explicit change type and bounded change scope

Portable v1.0 expands ChangeEvent to include **ChangeType** and **Confidence** and explicitly preserves whether a change applies to an entire object or only a version, deployment, batch, configuration, time interval or other bounded subset.

The source records change events but does not explicitly protect against localised change being interpreted as universal object change.

> **Object Change ≠ Necessarily Every Instance or Every Time Period**

**Classification:** General improvement / failure-mode correction.

**Decision:** INCORPORATE.

### KCP-BP-05 — Changed-property filtering

Portable workflow explicitly asks whether the changed property actually supplies the capability required by the dependent.

The source has selective materiality filtering but not this operational changed-property test.

**Classification:** Clarification / cascade-control improvement.

**Decision:** INCORPORATE.

### KCP-BP-06 — No Transformation ≠ No Material Effect

Portable v1.0 records that storage, transmission, display, publication, caching or other preservation of affected output may justify review even if the downstream object does not transform the payload.

This closes a possible false stopping condition.

**Classification:** General improvement / failure-mode correction.

**Decision:** INCORPORATE.

### KCP-BP-07 — Alternative verification boundary

Portable v1.0 explicitly states that alternative equivalence testing is external unless supplied by the host, and KCS consumes rather than manufactures the verification result.

The source says similar labels do not establish equivalence but does not explicitly assign the verification boundary.

**Classification:** Clarification / authority-interface safeguard.

**Decision:** INCORPORATE.

### KCP-BP-08 — Evaluation-space completeness escalation boundary

Portable v1.0 refines ESCP handling:

- no recorded dependency is not proof of no dependency;
- UNKNOWN does not automatically mean REVIEW_REQUIRED;
- where a consequential decision depends on assumed completeness, source-grounded discovery/external escalation may be required;
- consequence/escalation thresholds remain host inputs.

The source states the first principle but not the later bounded escalation semantics.

**Classification:** General improvement / epistemic safeguard.

**Decision:** INCORPORATE.

### KCP-BP-09 — Freshness thresholds remain host/domain inputs

Portable v1.0 makes explicit that age alone does not create a universal stale threshold.

The source already supports freshness and REVIEW_OVERDUE but leaves this boundary implicit.

**Classification:** Clarification.

**Decision:** INCORPORATE AS EXPLICIT INVARIANT.

### KCP-BP-10 — Dimensional/coexistent output classifications

Portable v1.0 supplies KCP-C1 through KCP-C16 and explicitly states that outputs are dimensional/coexistent rather than a universal precedence ladder.

The source contains most underlying states but no comparable output contract.

**Classification:** Interface improvement / portable formalisation.

**Decision:** PARTIAL INCORPORATION. Preserve the semantic ability for multiple scoped classifications to coexist. The literal KCP-C identifiers need not become mandatory Concord serialization.

### KCP-BP-11 — Scope-bound classifications

Portable v1.0 requires classifications to bind to the relevant instance, version, configuration, batch, deployment, time interval or other bounded subset where scope matters.

This is the downstream counterpart to bounded ChangeEvent scope.

**Classification:** General improvement / failure-mode correction.

**Decision:** INCORPORATE.

### KCP-BP-12 — Explicit ReviewRecord

Portable v1.0 defines a consequential review record preserving changed object, dependent, relation, changed property, materiality, context, alternatives, evidence, confidence, outcome, resulting state, further propagation, reviewer/source and time.

The source describes review flow but not a full review-result record.

**Classification:** Interface improvement / provenance improvement.

**Decision:** INCORPORATE SEMANTIC RECORD; exact implementation schema remains flexible.

## Audit result

The audit identifies **12 material portable/source deltas**.

They are materially different from the SMM and STRA cases:

- the **source kernel is already highly complete**;
- no new dependency/change-propagation architecture is required;
- most deltas are operational precision, scope control, provenance/interface formalisation or failure-mode closure;
- literal portable identifiers/schemas do not need to be imposed on Concord.

Result:

- **8** deltas are source-relevant operational or failure-mode improvements;
- **3** are primarily clarifications/formalisations of source rules;
- **1** is best treated as partial semantic incorporation rather than literal portable serialization;
- **0** require replacement of the KCS companion kernel;
- **0** justify expansion of KCS authority.

## Integration recommendation

Create:

**KCS Companion Upgrade 002 — KCS Change-Propagation Back-Propagation 001**

It should be deliberately small relative to the existing Companion Upgrade 001 and add only the bounded source-relevant refinements above.

Required regression should check:

- Civil State Map/SMM dependency consumption;
- Civilisation Clock/STRA trigger consumption;
- Continuity/recovery dependency use;
- privacy/purpose-bounded visibility;
- Active Development correction/supersession workflow.

## Methodological significance

This audit provides an important third result for the back-propagation method.

SMM and STRA showed substantial post-extraction source improvements.

KCS Change Propagation shows a **weaker but still real delta**: the source architecture was already mature, and the portable programme mainly sharpened edge conditions and operational records.

The method therefore did not treat every difference as evidence that the source needed major reconstruction.

## Status decision

> **KCS CHANGE PROPAGATION BACK-PROPAGATION: SOURCE UPDATE CANDIDATE — BOUNDED**

A small additive companion is justified. A source rewrite is not.
