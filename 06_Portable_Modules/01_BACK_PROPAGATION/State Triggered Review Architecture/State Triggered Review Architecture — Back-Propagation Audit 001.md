# State Triggered Review Architecture — Back-Propagation Audit 001

**Portable module:** State Triggered Review Architecture — Portable Module v1.0
**Status:** SOURCE UPDATE CANDIDATE
**Source family:** Civilisation Clock
**Primary source compared:** Civilisation Clock Companion Extension 001 — State, Functional and Compound Trigger Architecture
**Date:** 24 September 2026

## Purpose

This is the second formal post-graduation back-propagation audit.

It compares graduated STRA v1.0 with the Civilisation Clock companion from which the portable architecture was extracted and asks which later PMEDG refinements remain relevant to the Concord source.

> **Portable Difference ≠ Source-System Improvement**

## Source continuity

The source companion already contains the STRA kernel:

- non-temporal and temporal trigger classes;
- compound conditions;
- state/capability/dependency/event/risk/recurrence/evidence/participant triggers;
- temporal backstops;
- separation of triggering from substantive authority;
- wake-me-when candidacy;
- cold-knowledge retrieval followed by revalidation;
- dependency-based development;
- provenance/correction/supersession fields;
- UNKNOWN and DISPUTED;
- privacy, consent and owner boundaries at conceptual level.

STRA therefore does not replace the Clock architecture.

The back-propagation issue is that PMEDG substantially operationalised edge conditions that remain only provisional or absent in the source companion.

## Delta classification

### STRA-BP-01 — Expanded trigger lifecycle states

Portable STRA adds **IMPOSSIBLE**, **RETIRED** and **ROUTING-UNRESOLVED** beyond the source candidate state vocabulary.

These states close distinct failure modes: unreachable conditions, deliberate closure, and satisfied/reviewable conditions without legitimate destination.

**Classification:** General improvement / failure-mode correction.

**Decision:** SOURCE UPDATE CANDIDATE.

### STRA-BP-02 — Missing evidence is not false

Portable invariant:

> **Missing Evidence ≠ Condition False**

The source supports UNKNOWN/DISPUTED but does not state this operational trigger-evaluation invariant explicitly.

**Classification:** Clarification / epistemic failure-mode correction.

**Decision:** SOURCE UPDATE CANDIDATE.

### STRA-BP-03 — Compound uncertainty semantics

Portable STRA defines bounded minimum semantics for TRUE/FALSE with UNKNOWN and DISPUTED and requires natural-language exception forms to be normalised before consequential evaluation.

The source says compound triggers are possible but states that compound-trigger implementation is undeveloped.

**Classification:** General improvement / failure-mode correction.

**Decision:** SOURCE UPDATE CANDIDATE.

### STRA-BP-04 — Materiality interface

Portable STRA separates trigger evaluation from the host/domain determination of what counts as material change and defines a bounded materiality record.

The source uses material change but does not formalise this ownership/interface boundary.

**Classification:** Interface improvement / authority safeguard.

**Decision:** SOURCE UPDATE CANDIDATE.

### STRA-BP-05 — Validation and authority provenance

Portable STRA distinguishes capability claimed, available, validated and authorised-for-use and requires provenance/scope for consequential validation states.

The source has capability triggers but not this later validation boundary.

**Classification:** General improvement / failure-mode correction.

**Decision:** SOURCE UPDATE CANDIDATE.

### STRA-BP-06 — Explicit role separation and unresolved routing

Portable STRA separates trigger-definition owner, evaluator, substantive owner and ownership-resolution route. It prevents repeated evaluation from manufacturing authority and requires bounded review/backstop for ROUTING-UNRESOLVED.

The source distinguishes action owner and review owner but does not fully operationalise unresolved routing.

**Classification:** General improvement / authority safeguard.

**Decision:** SOURCE UPDATE CANDIDATE.

### STRA-BP-07 — Reconciliation handoff

Portable STRA introduces a bounded handoff when dependency/state sources conflict rather than making STRA resolve domain truth itself.

**Classification:** Interface improvement / authority safeguard.

**Decision:** SOURCE UPDATE CANDIDATE.

### STRA-BP-08 — Privacy-preserving bounded result

Portable STRA permits an authorised evaluator to return a bounded SATISFIED / NOT-SATISFIED / UNKNOWN result without exposing protected source content.

The source warns against broad private-context retrieval but does not formalise this interface.

**Classification:** General improvement / privacy/interface safeguard.

**Decision:** SOURCE UPDATE CANDIDATE.

### STRA-BP-09 — Event-order interface

Portable STRA explicitly rejects timestamp order as universal material precedence and requires provenance/uncertainty for externally supplied consequence-relevant ordering.

**Classification:** General improvement / epistemic safeguard.

**Decision:** SOURCE UPDATE CANDIDATE.

### STRA-BP-10 — Stale/impossible trigger lifecycle review

Portable STRA requires bounded review of long-lived WATCHING states and defines outcomes including continue, modify, reset, suspend, supersede, retire and ownership resolution.

The source identifies stale/impossible trigger failure modes but does not operationalise their lifecycle.

**Classification:** General improvement / failure-mode correction.

**Decision:** SOURCE UPDATE CANDIDATE.

### STRA-BP-11 — Cascade control

Portable STRA develops bounded cascade semantics: parent provenance, cycle detection where represented, duplicate suppression, child-condition/activation requirements, materiality gate, routing validation and stale-replica/supersession protection.

The source identifies trigger cascades as a failure mode but supplies no comparable control architecture.

**Classification:** General improvement / failure-mode correction.

**Decision:** SOURCE UPDATE CANDIDATE.

### STRA-BP-12 — Explicit participant-condition boundary

Portable invariant:

> **Participant Condition Satisfied ≠ Forced Action**

The source already preserves this substantially through wake-candidate and participant/continuity rules.

**Classification:** Clarification of existing source rule.

**Decision:** INCORPORATE AS EXPLICIT INVARIANT; no architectural change required.

### STRA-BP-13 — Revalidation boundary

Portable invariant:

> **Relevance Returned ≠ Validity Restored**

The source already requires revalidation after cold-knowledge retrieval.

**Classification:** Clarification/formalisation.

**Decision:** INCORPORATE AS EXPLICIT INVARIANT; source mechanism already present.

### STRA-BP-14 — Dependency completeness boundary

Portable STRA states:

> **No Represented Dependency ≠ No Dependency**

The source warns that dependency models may fail to notice unforeseen relevant change but does not make this an explicit operating invariant.

**Classification:** Clarification / epistemic safeguard.

**Decision:** SOURCE UPDATE CANDIDATE.

## Audit result

Fourteen material post-extraction refinements were identified.

- **11** require source-level operational strengthening or explicit new interface semantics.
- **3** primarily formalise safeguards already substantially present in the source.
- **0** require replacement of the Civilisation Clock kernel.
- **0** justify transfer of substantive domain authority to STRA or the Clock.

The strongest source deltas are compound uncertainty, lifecycle states, unresolved routing, cascade control, materiality ownership, privacy-preserving evaluation, stale/impossible trigger review and validation provenance.

## Integration recommendation

Create:

**Civilisation Clock Companion Upgrade — STRA Back-Propagation 001**

The upgrade should preserve the existing Clock companion and return only source-relevant STRA refinements.

After drafting, perform interface regression against at least:

- Civil State Map including SMM Back-Propagation 001;
- KCS dependency/change-propagation architecture;
- Continuity/participant interfaces where participant triggers are used;
- privacy/protected-context boundaries.

## Status decision

> **STRA BACK-PROPAGATION: SOURCE UPDATE CANDIDATE**

This audit confirms the preliminary portfolio signal and provides the second concrete case in which PMEDG development advanced beyond the original Concord source representation.
