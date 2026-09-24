# Portable-Module Back-Propagation Audit — Development Note 001

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Status:** SUPERSEDED AS CURRENT METHOD / RETAINED FOR DEVELOPMENTAL PROVENANCE
**Validation:** PILOT COMPLETED — METHOD SUBSEQUENTLY FORMALISED AS BPM v1.0
**Origin:** Sketch Idea — Back-Propagation of Graduated Portable-Module Improvements into Concord Systems
**Pilot module:** State and Maturity Mapping (SMM)
**Date:** 24 September 2026
**Superseded by:** Portable-Module Back-Propagation Method — BPM v1.0

---

## 1. Purpose

Portable-module extraction and PMEDG development can improve a method after it has been extracted from its Concord source architecture.

This creates a possible one-way-development problem:

**Concord source → portable extraction → blind transfer → bounded revision → graduated module**

without an automatic return path:

**graduated module → source comparison → justified reintegration**

This Development Note tests whether that problem is real by performing a bounded back-propagation audit of **State and Maturity Mapping (SMM)** against its Concord source architecture, **Civil State Map — Maturity, Sufficiency and Consequence Model**.

The audit does not assume that every portable-module difference belongs in the source system.

> **Portable Difference ≠ Source-System Improvement**

> **Validated Portable Refinement ≠ Automatic Canonical Amendment**

## 2. Source boundary

### Concord source examined

- *Civil State Map — Maturity, Sufficiency and Consequence Model*
- related CDT/Clock interface where needed to understand source ownership

### Portable evidence examined

- *State and Maturity Mapping — Portable Module v1.0*
- *State and Maturity Mapping — Cross-Test Convergence Review*
- *State and Maturity Mapping — v0.3 Evidence and Regression Audit*

The PMEDG evidence is particularly useful because it identifies which v0.3 changes were introduced in response to frozen blind-transfer evidence rather than merely appearing during later rewriting.

## 3. Classification rule

Each material portable/source delta is classified as one of:

- **P — Portability-only:** useful for generic hosts but not required by the Concord source.
- **C — Clarification/formalisation:** source mechanism substantially exists; portable form makes it more precise.
- **G — General improvement:** evidence-supported refinement applicable to the Concord source itself.
- **F — Failure-mode correction:** closes a weakness exposed by testing that also exists in the Concord source.
- **I — Interface improvement:** improves exchange with another Concord system or representation.
- **S — Source-specific review required:** applicability cannot safely be decided from the portable module alone.

Multiple classifications may apply.

The audit asks whether the source should be reviewed for incorporation. It does not silently modify the source.

## 4. SMM pilot result

The pilot finds clear evidence of post-extraction improvements that are relevant to the Civil State Map.

The source architecture already contains the SMM kernel:

- function-based assessment;
- presence distinct from maturity;
- context-sensitive sufficiency;
- dependency/blocker state;
- consequence/exposure;
- uncertainty/dispute;
- active development state;
- evidence/provenance/freshness;
- candidate response;
- stopping conditions;
- anti-gaming and anti-centralisation.

PMEDG did not replace this kernel.

Instead, the transfer tests exposed edge conditions in how the source mechanism behaves at interfaces, under stale evidence, under distributed supply, when ownership is absent, when state is projected into aggregates, and when assessment history changes.

These refinements are not all present in the current Civil State Map.

## 5. Delta register

### BP-SMM-01 — Composite assessment-unit decision rule

**Portable development:** SMM v1.0 explicitly requires declaration of the assessed function boundary and distinguishes missing subfunction, partial supply, dependency blockage, separate function and maturity/sufficiency deficit.

**Source state:** The Civil State Map identifies the default unit as a required civil function or legitimate architectural unit, but does not contain the later bounded composition decision rule.

**Evidence origin:** BTT-001 partial-function pressure; BTT-002 P01–P03.

**Classification:** **G / C**

**Back-propagation finding:** **INCORPORATE.** The rule improves Civil State Map classification without changing its kernel.

---

### BP-SMM-02 — Explicit context-set preservation and CTX_REF

**Portable development:** materially different contexts are preserved as a context set. A restrictive host representation must reference the richer state or declare itself lossy.

**Source state:** The Civil State Map already states that maturity/sufficiency are context-sensitive and records consequence context, but does not specify preservation of multiple simultaneous context states or a reference mechanism.

**Evidence origin:** BTT-001 context-set refinement; BTT-002 P04–P06.

**Classification:** **G / I / F**

**Back-propagation finding:** **INCORPORATE SEMANTIC RULE.** The Concord need not adopt the literal serialization token `CTX_REF` everywhere, but it should preserve the tested rule that a single projected state must not silently erase materially different contexts.

---

### BP-SMM-03 — Candidate-absence escalation boundary

**Portable development:** CANDIDATE_ABSENT can become REQUIRED_FUNCTION_GAP only after a declared search/source-resolution boundary; materially unavailable evidence capable of changing the conclusion blocks promotion. No universal quantitative search threshold is imposed.

**Source state:** The Civil State Map requires source resolution before declaring absence and includes CANDIDATE_ABSENT, but does not define this later escalation discipline.

**Evidence origin:** BTT-001 candidate-absence pressure; BTT-002 P10–P12.

**Classification:** **G / F**

**Back-propagation finding:** **INCORPORATE.** This directly strengthens ESCP discipline in the canonical State Map.

---

### BP-SMM-04 — Consequential aggregate disclosure and refusal

**Portable development:** SMM v1.0 defines minimum disclosure for consequential aggregates and permits a projection to be marked **NOT VALID FOR THE PROPOSED USE** if UNKNOWN/DISPUTED/BLOCKED states, high-consequence exceptions or source-state traceability cannot be preserved.

**Source state:** The Civil State Map correctly rejects a universal maturity score but does not define safeguards for cases where a later Concord interface nevertheless produces a summary or aggregate.

**Evidence origin:** BTT-001 aggregation pressure; BTT-002 P27–P31.

**Classification:** **G / F / I**

**Back-propagation finding:** **INCORPORATE.** This closes a real downstream representation weakness without introducing a universal score.

---

### BP-SMM-05 — Consequence carriage through downstream projections

**Portable development:** a ranking/prioritisation projection must carry material consequence/exposure or a lossless reference to it; otherwise it is explicitly lossy and not a complete SMM-derived priority representation.

**Source state:** The Civil State Map warns against centrality bias and supplies consequence/exposure to the Civilisation Clock, but does not state this projection-preservation requirement.

**Evidence origin:** BTT-001 consequence safeguard; BTT-002 P32–P34.

**Classification:** **G / I / F**

**Back-propagation finding:** **INCORPORATE.** Particularly relevant to the Civilisation Clock queue interface.

---

### BP-SMM-06 — Existing-work suppression vocabulary

**Portable development:** where legitimate active work already addresses a deficit, use **CONTINUE_EXISTING_WORK / NO_NEW_CANDIDACY** rather than generating a duplicate development candidate.

**Source state:** The Civil State Map records active development and says the Clock should avoid repeatedly selecting work already in progress, but its response-class table does not explicitly encode this result.

**Evidence origin:** BTT-001 active-work pressure; BTT-002 P21–P23.

**Classification:** **C / G / I**

**Back-propagation finding:** **INCORPORATE.** This formalises behaviour the source already intends.

---

### BP-SMM-07 — Ownership-gap / governance-escalation candidate

**Portable development:** SMM can represent **OWNERSHIP_GAP / GOVERNANCE_ESCALATION_CANDIDATE** while explicitly lacking authority to assign the missing owner.

**Source state:** The Civil State Map says it cannot create ownership and preserves UNKNOWN/DISPUTED, but queue eligibility currently expects a legitimate owner or ownership-resolution route without defining the ownership-gap response itself.

**Evidence origin:** BTT-001 ownership pressure; BTT-002 P24–P26.

**Classification:** **G / F / I**

**Back-propagation finding:** **INCORPORATE WITH AUTHORITY BOUNDARY.** The candidate must route outward to legitimate governance/constitutional machinery; the State Map must not solve the governance question.

---

### BP-SMM-08 — Interface-evidence stewardship may remain UNKNOWN/UNASSIGNED

**Portable development:** interface-satisfied functions may have an unknown or unassigned evidence refresh/review owner; SMM exposes the resulting uncertainty without inventing local ownership.

**Source state:** The Civil State Map supports interface satisfaction, evidence, freshness and unknown ownership separately but does not explicitly combine them for interface-evidence stewardship.

**Evidence origin:** BTT-001 evidence-responsibility pressure; BTT-002 P16–P17.

**Classification:** **G / F**

**Back-propagation finding:** **INCORPORATE.** This is a direct anti-fabrication safeguard.

---

### BP-SMM-09 — Distributed-supply projection and DS_REF

**Portable development:** distributed supply must remain representable when a consuming schema expects one owner. A simplified export may reference an authoritative distributed-supply record and must identify projection loss.

**Source state:** The Civil State Map explicitly supports distributed suppliers but has no rule preventing downstream one-owner representations from collapsing that state.

**Evidence origin:** BTT-001 registry-interface pressure; BTT-002 P13–P15 and P35–P37.

**Classification:** **G / I / F**

**Back-propagation finding:** **INCORPORATE SEMANTIC RULE.** Literal `DS_REF` serialization can remain implementation-defined.

---

### BP-SMM-10 — Default stale-current-state treatment

**Portable development:** after a material context, dependency or capability change, an old SUFFICIENT state cannot remain unqualified current SUFFICIENT without revalidation. Portable default: **current sufficiency = UNKNOWN (REVIEW DUE)** while the prior SUFFICIENT state remains historically preserved.

**Source state:** The Civil State Map says stale state is not automatically false and requires reconsideration, but does not define the current-state default during the interval before reassessment.

**Evidence origin:** BTT-001 stale-state pressure; BTT-002 P07–P09.

**Classification:** **G / F**

**Back-propagation finding:** **INCORPORATE.** This is one of the clearest genuine failure-mode closures produced by PMEDG.

---

### BP-SMM-11 — Scope-limited assessment history relations

**Portable development:** explicit **CORRECTS / SUPERSEDES / QUALIFIES / DISPUTES / CONFIRMS** relations preserve prior assessments and constrain the scope in which a later assessment changes interpretation.

**Source state:** The Civil State Map requires prior state to remain reconstructable and records what changed and why, but does not formalise the relation semantics.

**Evidence origin:** BTT-001 dispute/supersession pressure; BTT-002 P18–P20 and P38–P40.

**Classification:** **G / C / I**

**Back-propagation finding:** **INCORPORATE.** This strengthens KCS/provenance integration.

---

### BP-SMM-12 — HOLD versus NO_ACTION

**Portable development:** HOLD is a workflow state describing existing work that is paused/deferred. NO_ACTION_CANDIDATE is an assessment output stating that no material new action candidate is presently justified. They can coexist and must not be collapsed.

**Source state:** The Civil State Map includes HOLD as an active-development state and NO_ACTION as a response, but does not explicitly state the semantic distinction.

**Evidence origin:** BTT-001 stopping pressure; BTT-002 P41–P42.

**Classification:** **C / G**

**Back-propagation finding:** **INCORPORATE.** This is primarily a clarification but prevents workflow/state confusion.

## 6. Pilot summary

All twelve convergence-authorised SMM refinements were examined.

**Result:**

- **12 / 12** are relevant to the Concord Civil State Map at least as clarification, interface protection or general improvement.
- **0 / 12** require replacement of the Civil State Map kernel.
- **0 / 12** justify transferring authority from legitimate Concord systems into the State Map.
- Several literal portable serialization forms can remain implementation-defined while their semantic safeguards are incorporated.
- The strongest source-level corrections concern stale current state, candidate-absence escalation, lossy context/distributed-supply projections, aggregate disclosure, ownership gaps, evidence stewardship and historical assessment relations.

This is sufficient to establish that back-propagation need is real for SMM.

## 7. Proposed source integration boundary

The Civil State Map should be upgraded additively rather than replaced.

A bounded companion upgrade should:

1. preserve the existing `SM(t) = <N,P,M,Q,D,C,U,A,R>` architecture;
2. preserve the current Civil State Map's Concord-specific maturity dimensions and Clock/KCS interfaces;
3. add the twelve tested refinements where applicable;
4. distinguish semantic requirements from optional serialization patterns;
5. preserve all current authority boundaries;
6. preserve existing historical source provenance;
7. identify the graduated SMM module and PMEDG evidence as the origin of the refinements;
8. require retest of affected State Map/Clock/KCS interfaces after integration.

The source document should not simply be rewritten to look like the portable module. The correct pattern is a **companion upgrade**, followed by integration/retest if the Concord's normal development process supports it.

## 8. Evidence status

The SMM pilot supports the original back-propagation hypothesis:

> **Post-extraction portable-module development can produce evidence-supported refinements that remain absent from the originating Concord architecture and are materially applicable to it.**

This is stronger than the original sketch, but remains bounded.

It does not establish that every graduated portable module requires source modification or that every PMEDG refinement should be copied back.

## 9. Methodological finding

A back-propagation audit is useful only if it preserves four different questions:

1. **What changed after extraction?**
2. **Why did it change?**
3. **Does the change apply to the source architecture?**
4. **What legitimate integration path should carry it back?**

Skipping question 2 risks importing arbitrary portable wording.

Skipping question 3 collapses portability adaptation into source improvement.

Skipping question 4 turns an audit into silent canonical modification.

## 10. Next action for SMM

Create a bounded:

**Civil State Map Companion Upgrade — SMM Back-Propagation 001**

The companion should contain only the source-relevant, evidence-supported refinements identified above.

After drafting, test the integrated State Map against the existing Civilisation Clock and KCS interfaces before treating the refinements as canonical integrated capability.

## 11. Portfolio implication

The SMM pilot provides enough evidence to retain the back-propagation programme as an active methodological task.

The next modules should not automatically be audited in graduation order. A later portfolio pass can prioritise modules by:

- amount of post-extraction development;
- severity of corrected failure modes;
- centrality of the source system;
- number of downstream Concord dependents;
- and likelihood that the source still contains the pre-extraction form.

This pilot therefore validates the need for a controlled audit path while preserving module/source boundaries.
