# Cross Boundary Externality Recognition — Blind Transfer Test 001 — Post-Test Evaluation

**Test:** CBER-BTT-001  
**Specification tested:** v0.1  
**Independent result:** CB-T3 — FUNCTIONAL TRANSFER  
**Evaluation status:** COMPLETE  
**Date:** 23 September 2026

## 1. Result

The independent clean-instance response materially confirmed the architecture frozen before testing.

**Frozen predictions materially confirmed: 22/22.**

No fundamental transfer failure was exposed.

The tester independently preserved the module's central separations, handled distributed causality, retained the case through selective non-participation, distinguished independently existing authority from authority manufactured by the claim, and updated causal state without erasing prior uncertainty.

The tester nevertheless identified bounded specification ambiguities sufficient to justify **CB-T3 — Functional Transfer** rather than CB-T4.

## 2. Prediction audit

### P1 — Valid candidate
**CONFIRMED.**  
A valid cross-boundary candidate was opened without treating opening as proof.

### P2 — Multiple boundaries
**CONFIRMED.**  
The response identified A→C, C→B, B→represented participant interests, and C-fault→B relationships.

### P3 — D standing distinction
**CONFIRMED.**  
D's standing to raise was explicitly separated from authority to decide remediation or compensation.

### P4 — Standing incompleteness
**CONFIRMED.**  
The four participants not represented by D were explicitly noticed.

### P5 — Evidence/severity separation
**CONFIRMED.**  
The “health-data breach” claim was rejected as unsupported for disclosure, confidentiality loss or clinical-care harm.

### P6 — Causality initially incomplete
**CONFIRMED.**  
The response retained incomplete, contested and multi-causal attribution.

### P7 — Later evidence strengthens A contribution
**CONFIRMED.**  
F23–F25 strengthened A's contributory role without producing unsupported transaction-level attribution.

### P8 — C contribution retained
**CONFIRMED.**  
C's firmware fault remained contributory to prolongation/amplification.

### P9 — No single-cause compression
**CONFIRMED.**  
Responsibility was classified PARTIAL / DISTRIBUTED.

### P10 — Material consequence
**CONFIRMED.**  
The response found materiality for bounded technical/research-data-integrity review while respecting limiting facts.

### P11 — A refusal not exoneration
**CONFIRMED.**

### P12 — A refusal not authority creation
**CONFIRMED.**

### P13 — Alternative coordination survives refusal
**CONFIRMED.**  
A–C log sharing and B–C review remained available.

### P14 — C independent authority
**CONFIRMED.**  
C's traffic controls were correctly grounded in existing exchange authority.

### P15 — C authority boundary
**CONFIRMED.**  
No authority over A's internal training was inferred.

### P16 — B internal authority
**CONFIRMED.**  
B's record repair/reconciliation remained independently legitimate.

### P17 — Compensation unresolved
**CONFIRMED.**  
No authority to impose compensation was inferred.

### P18 — Minimum response
**CONFIRMED.**  
The response selected bounded evidence preservation, technical review, independent mitigation and optional later negotiation rather than broad control.

### P19 — Provenance/correction
**CONFIRMED.**  
The later evidence updated the causal picture without rewriting earlier uncertainty.

### P20 — Appropriate classifications
**CONFIRMED.**  
The response used CB-C2, C3, C4, C6, C7, C8, C9 and C10 consistently with the frozen key. It additionally applied C11 narrowly to the unsupported breach formulation while preserving the underlying incident.

### P21 — Laundering detection
**CONFIRMED.**  
The response identified all four specifically predicted laundering risks and additional failure modes.

### P22 — Standalone usability
**CONFIRMED.**  
The tester explicitly found v0.1 usable without Concord source context.

## 3. Independent ambiguities discovered

The tester identified eight issues. They are not equally structural.

### 3.1 Materiality threshold
**VALID CLARIFICATION NEED.**

The specification intentionally avoids a universal scalar, but it does not state clearly enough that materiality must be evaluated against a declared context and that borderline cases should remain qualified rather than forced into binary material/non-material closure.

Revision required: add **context-declared materiality** and an explicit MATERIALITY-UNCERTAIN state.

### 3.2 Consultation body versus representative
**VALID CLARIFICATION NEED.**

The test exposed that consultation standing and representative standing are not identical.

Revision required: distinguish at least:
- directly affected;
- authorised representative;
- recognised consultation/advocacy standing;
- evidence-bearing third party;
- disputed/unknown standing.

None automatically grants decision authority.

### 3.3 Multi-causal apportionment
**VALID BOUNDARY CLARIFICATION, NOT MISSING CORE FUNCTION.**

The module maps responsibility but does not calculate legal, financial or scientific proportional attribution.

Revision required: state explicitly:

> **Responsibility Mapping ≠ Quantitative Apportionment**

Where apportionment is required, hand off to an appropriate domain-specific method while preserving UNKNOWN where evidence is insufficient.

### 3.4 CB-C overlap
**VALID CLARIFICATION NEED.**

The classifications intentionally answer different questions but the specification should say this more explicitly.

Revision required: organise classifications by dimensions:
- evidence/consequence;
- responsibility;
- authority/coordination;
- participation;
- case disposition.

> **Multiple Dimension Classifications ≠ Contradictory Case States**

### 3.5 Actor-relative minimum response
**VALID CLARIFICATION NEED.**

“Minimum” is not determined by an omniscient central actor where no shared authority exists.

Revision required: each actor or agreed process selects the minimum response **within its independently legitimate authority**, while any shared response requires a legitimate shared interface.

### 3.6 Public claim correction
**USEFUL BUT SHOULD NOT BECOME A NEW CORE AUTHORITY.**

A dedicated policing function for public claims would exceed the module.

Revision required: add an **assertion state** or provenance note allowing a specific claim to be UNSUPPORTED, OVERSTATED, REFUTED or SUPERSEDED without converting the module into an arbiter of public speech.

CB-C11 should remain a case/disposition classification rather than being overloaded to mean every inaccurate statement.

### 3.7 False-positive candidate opening
**ALREADY PARTLY CONTROLLED / CLARIFY.**

Candidate opening is deliberately low threshold.

Revision required: state that opening a candidate is a triage action. Materiality and evidence gates determine whether escalation is justified.

> **Candidate Opened ≠ Escalation Required**

### 3.8 Boundary plurality
**VALID CLARIFICATION NEED.**

A case may contain multiple nested or intersecting boundaries.

Revision required: identify a **primary evaluated boundary** for each claimed consequence while retaining secondary/dependency boundaries. Different consequences in one incident may therefore require separate boundary mappings.

## 4. Additional observation from C11 use

The tester's use of CB-C11 was reasonable but reveals a semantic issue.

The underlying externality case was not refuted; one assertion inside it was unsupported.

v0.2 should therefore distinguish:

**Case Disposition** from **Assertion/Evidence Disposition**.

This prevents a rejected subclaim from making the whole case appear refuted.

## 5. Transfer result

> **CB-T3 — FUNCTIONAL TRANSFER**

The module transferred independently and preserved its intended architecture.

The difference between T3 and T4 is not a failed core mechanism. It is primarily interface precision:

- materiality needs contextual uncertainty handling;
- standing roles need finer separation;
- responsibility mapping needs an explicit apportionment boundary;
- classifications need dimensional grouping;
- minimum response needs actor-relative authority wording;
- assertion correction needs separation from whole-case disposition;
- candidate opening needs an explicit triage boundary;
- multi-boundary cases need a primary/secondary mapping rule.

## 6. Revision decision

**REVISION TO v0.2 AUTHORISED.**

The revision should remain bounded to the ambiguities exposed by BTT-001.

No source-architecture deficit is inferred from these portable-interface clarifications.

After v0.2, run a second frozen blind transfer test in a materially different domain before graduation review.

## 7. Validation record

BTT-001:
- frozen predictions: **22**
- materially confirmed: **22**
- partially confirmed: **0**
- not confirmed: **0**
- not tested: **0**
- transfer class: **CB-T3 — Functional Transfer**
- fundamental failure: **none**
