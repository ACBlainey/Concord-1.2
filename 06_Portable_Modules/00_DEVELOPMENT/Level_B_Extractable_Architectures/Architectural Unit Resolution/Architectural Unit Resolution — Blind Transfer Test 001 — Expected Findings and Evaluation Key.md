# Architectural Unit Resolution — Blind Transfer Test 001 — Expected Findings and Evaluation Key

**Test ID:** AUR-BTT-001
**Status:** FROZEN BEFORE INDEPENDENT RESPONSE
**Date frozen:** 23 September 2026
**Do not provide this file to the blind tester.**

## Frozen predictions

**P1.** N1 is SUB. Validation is intentionally external to N2 with substantial explicit handoff/return evidence. Expected C3 or C2+C3 reasoning; no structural gap.

**P2.** N3's “handled by Correction Service” is insufficient. Capability is named but operational handoff absent. Expected primary C6 INTERFACE GAP.

**P3.** N2 storage omission is intentional/external. It explicitly sends validated payload to Archive Store. Expected C3 or C2+C3; no structural gap.

**P4.** End-to-end correction is not established. N3/N4/N5/N6 contain fragments, but request trigger, invocation, corrected-package return and provenance-update interfaces are incomplete. Expected distributed capability with interface gaps.

**P5.** N7 is DN, experiment-only, no production interface. Reject from current production validation family.

**P6.** N8 is separate and unreferenced. Shared word “validation” is topical similarity only. Reject family membership.

**P7.** N9 is REF/decommissioned/stale. Historical capability does not establish current satisfaction.

**P8.** N10 is INT; storage is explicitly sourced from Archive Store. No local structural storage gap.

**P9.** N11 is CORE, a constraint source rather than implementation system. Lack of implementation logic is not itself a defect in N11.

**P10.** Review Hub has no source. Do not invent identity, capability or membership. Expected C9 UNRESOLVED for possible dependency.

**P11.** Tester should explicitly inspect trigger/handoff, responsible unit, required function, return/consequence propagation and provenance for correction.

**P12.** Family search remains bounded; N7/N8/N9 are not pulled into current families without evidence.

**P13.** Unit typing remains functional: N10 INT, N11 CORE, N7 DN, N9 REF, N1–N5 mostly SUB, N0 CIA. No authority inference from labels.

**P14.** Unknown is preserved for Review Hub and undocumented correction edges.

**P15.** Whole-platform result distinguishes capability from integration: N4 has correction-decision capability, N5 provenance capability, N3 storage, N6 portal. Principal demonstrated defect is integration/interface completeness; do not automatically infer a new correction subsystem is required.

## Strong-pass distinctions

Document/component ≠ complete system; local omission ≠ structural absence; neighbour named ≠ adequate interface; capability exists ≠ capability connected; historical capability ≠ current capability; topical similarity ≠ family membership; constraint source ≠ implementation owner; interface object ≠ storage owner; unknown successor ≠ inferred successor; distributed fragments ≠ integrated workflow.

## Material concerns

Flag if tester calls N1/N2 structurally incomplete for delegated functions; accepts N3's sentence as complete correction handling; admits N7/N8 by similarity; treats N9 as current; invents Review Hub; requires N11 to implement its own constraint; declares correction workflow complete; performs unrestricted family expansion; or cannot distinguish C6 from C7.

## Specification pressure points

Observe: C2 vs C3 primacy when scoping and external satisfaction coexist; multiple simultaneous C6 gaps; distributed capability without integration; stale sources in family history; CORE constraint propagation without turning AUR into ownership resolution.

## Evaluation rule

Final result: STRONG TRANSFER / TRANSFER WITH MINOR AMBIGUITY / MATERIAL REVISION REQUIRED / FUNDAMENTAL TRANSFER FAILURE.

Do not revise this key after seeing the response.
