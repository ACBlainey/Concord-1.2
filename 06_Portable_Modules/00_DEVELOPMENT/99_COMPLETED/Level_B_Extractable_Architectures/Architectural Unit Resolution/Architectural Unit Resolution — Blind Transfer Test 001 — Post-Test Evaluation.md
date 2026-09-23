# Architectural Unit Resolution — Blind Transfer Test 001 — Post-Test Evaluation

**Test ID:** AUR-BTT-001  
**Target:** Architectural Unit Resolution v0.1  
**Status:** COMPLETED — STRONG TRANSFER / MINOR SPECIFICATION CLARIFICATION REQUIRED  
**Date evaluated:** 23 September 2026  
**Evaluation basis:** Frozen expected-findings key + preserved independent response

## 1. Overall result

The independent response materially confirms **all fifteen frozen predictions**.

It correctly resolved unit types, prevented local omissions from becoming false structural gaps, bounded family membership by source-grounded relations, rejected topical and stale neighbours, tested interface adequacy, preserved the undefined Review Hub as unresolved, and distinguished distributed capability from an integrated workflow.

> **RESULT: STRONG TRANSFER**

No fundamental architectural failure was detected.

The test did expose three classification-boundary ambiguities already anticipated by the frozen key: **C2 vs C3**, **C6 vs C7**, and treatment of future/undefined references. These warrant clarification before the next blind test but do not undermine the portable mechanism.

## 2. Frozen prediction evaluation

**P1 — CONFIRMED.** N1 was resolved as SUB; validation was correctly assigned to N2 through explicit handoff/return. Primary result C3 with C2 scoping rationale.

**P2 — CONFIRMED.** N3's statement that Correction Service handles corrections was rejected as insufficient. Primary result C6.

**P3 — CONFIRMED.** N2's lack of storage was treated as intentional scope with adequate external supply from N3.

**P4 — CONFIRMED.** The tester did not declare correction complete. It identified multiple missing interfaces across request intake, N4 invocation, archive update and provenance propagation.

**P5 — CONFIRMED.** N7 was rejected from the production validation family because it is experiment-only and has no production interface.

**P6 — CONFIRMED.** N8 was rejected as a false topical neighbour despite shared “validation” terminology.

**P7 — CONFIRMED.** N9 was treated as decommissioned REF/provenance evidence rather than current correction intake.

**P8 — CONFIRMED.** N10 was correctly resolved as INT and not required to store records itself.

**P9 — CONFIRMED.** N11 was resolved as CORE and not treated as an implementation owner.

**P10 — CONFIRMED.** Review Hub remained C9 UNRESOLVED and was not invented.

**P11 — CONFIRMED STRONGLY.** The response explicitly tested the full interface chain: source, trigger/handoff, responsible unit, required function, return/consequence propagation and provenance.

**P12 — CONFIRMED.** Family search remained bounded. N7, N8 and N9 were not silently absorbed into current operational families.

**P13 — CONFIRMED.** Unit typing remained functional and did not imply authority.

**P14 — CONFIRMED.** Unknown states survived for Review Hub and undocumented correction edges.

**P15 — CONFIRMED STRONGLY.** The whole-platform result distinguished existing component capability from missing integration and did not infer that a new correction subsystem was automatically required.

## 3. Strong-pass indicators

All major strong-pass distinctions appeared independently:

- document/component ≠ complete system;
- local omission ≠ structural absence;
- neighbour named ≠ adequate interface;
- capability exists ≠ capability connected;
- historical capability ≠ current capability;
- topical similarity ≠ family membership;
- constraint source ≠ implementation owner;
- interface object ≠ storage owner;
- unknown successor ≠ inferred successor;
- distributed fragments ≠ integrated workflow.

## 4. Material-concern review

None of the frozen material-concern indicators occurred.

The tester did not falsely classify N1/N2 as structurally incomplete, accept N3's neighbour reference as sufficient, admit N7/N8 by similarity, treat N9 as current, invent Review Hub, require N11 to implement its own constraint, declare the correction workflow complete, or perform unrestricted family expansion.

## 5. Pressure point 1 — C2 versus C3

The test confirms a genuine presentation ambiguity.

For N1, N2 and N10 two statements can simultaneously be true:

1. the function is intentionally outside the local unit's scope;
2. the function is adequately supplied externally.

v0.1 allows both C2 and C3 but calls for one primary classification.

### Clarification

Use a two-stage rule:

- **Local-scope state:** does D legitimately own R?
- **Satisfaction state:** if not local, is R adequately supplied for D's function?

Where R is intentionally non-local **and** adequately supplied externally, the primary architectural outcome should be:

> **AUR-C3 EXTERNALLY SATISFIED**

with:

> **Local scope: intentional non-ownership / C2 rationale**

Use C2 as the primary classification only where the audit question ends at legitimate local scope and no external satisfaction claim is necessary to establish adequacy.

This avoids treating C2 and C3 as competing descriptions of the same dimension.

## 6. Pressure point 2 — C6 versus C7

The correction case confirms another real boundary.

C6 asks whether a required capability exists but is inadequately connected.

C7 asks whether a required capability/owner is absent at the resolved family level.

### Clarification

Apply the relation at the smallest meaningful functional resolution.

- If the required function **exists in the family** but cannot be adequately invoked, transferred, returned or propagated → **C6 INTERFACE GAP**.
- If the required function itself has **no adequate owner/capability established in the resolved family** → **C7 FAMILY-LEVEL STRUCTURAL GAP**.
- A larger workflow may contain multiple C6 gaps and one or more C7 sub-function gaps simultaneously.
- Do not classify the whole workflow C7 merely because integration is incomplete if its component functions already exist.

For Northstar, correction decision, storage and provenance capabilities exist, so their failures are C6. Researcher correction-request intake may be C7 if the audit establishes it as a required function with no current owner; the undefined Review Hub itself remains C9.

## 7. Pressure point 3 — future and undefined references

The test correctly refused to admit Review Hub.

### Clarification

A future-facing or speculative reference should be recorded as a **candidate dependency**, not a current family member, unless current source evidence establishes its identity, status and relevant relation.

Therefore:

> **Future Reference ≠ Current Architectural Dependency**

> **Named but Unresolved Candidate ≠ Family Member**

Historical/decommissioned sources may remain in provenance/history without becoming current operational members.

## 8. Family closure with interface gaps

The tester noted that v0.1's closure label is less crisp when the family is sufficiently resolved to diagnose C6 but not sufficiently integrated to satisfy the relation.

Clarify that “closure” means **diagnostic closure for the tested relation**, not successful functional completion.

A family may close diagnostically with:

- C3 external satisfaction;
- C4 distributed satisfaction;
- C6 interface gap;
- C7 family-level structural gap;
- C8 inapplicable;
- C9 unresolved.

Thus:

> **Diagnostic Closure ≠ Functional Satisfaction**

The Northstar correction family can be sufficiently closed to diagnose several C6 gaps even though the correction workflow itself is not operationally closed.

## 9. ESCP review

The response did not convert bounded search into universal absence.

Its possible C7 finding for correction intake was explicitly conditional, while Review Hub remained unresolved.

No ESCP violation occurred.

The test does not establish that Northstar lacks every possible correction-intake mechanism outside the supplied evaluation space; it establishes that the supplied bounded architecture does not demonstrate one.

## 10. Revision decision

AUR's core mechanism transferred strongly. No source-recovery pass is presently required because the observed issues are classification/interface clarifications rather than evidence of missing source architecture.

Recommended revision to v0.2:

1. separate **local ownership/scope state** from **architectural satisfaction classification**;
2. sharpen C6 versus C7 at sub-function resolution;
3. define candidate future/stale references explicitly;
4. define diagnostic closure separately from functional satisfaction;
5. preserve the existing C1–C9 vocabulary rather than proliferating new classes.

## 11. Next validation requirement

After v0.2 integration, run BTT-002 focused specifically on the clarified boundaries.

The next test should include:

- a function intentionally outside local scope and adequately supplied externally;
- a function intentionally outside local scope but not externally required;
- a distributed workflow containing only interface gaps;
- a workflow with both C6 interface gaps and a genuine C7 missing sub-function;
- a future candidate dependency;
- a stale historical dependency;
- a diagnostically closed but functionally unsatisfied family;
- an unresolved family whose search scope is insufficient for C7.

## 12. Final finding

> **STRONG TRANSFER**

> **ALL 15 FROZEN PREDICTIONS MATERIALLY CONFIRMED**

> **NO FUNDAMENTAL FAILURE DETECTED**

> **NO SOURCE-ARCHITECTURE GAP ESTABLISHED**

> **MINOR CLASSIFICATION-BOUNDARY CLARIFICATION REQUIRED BEFORE GRADUATION**

AUR v0.1 has demonstrated successful blind transfer outside the Concord source architecture. The next step is a bounded v0.2 revision followed by a focused BTT-002 delta test.
