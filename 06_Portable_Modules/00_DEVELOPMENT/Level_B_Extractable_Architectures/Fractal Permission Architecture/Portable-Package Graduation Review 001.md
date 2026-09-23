# Fractal Permission Architecture — Portable-Package Graduation Review 001

**Candidate:** Fractal Permission Architecture — Portable Specification v0.3  
**Review type:** Portable-package graduation review  
**Date:** 23 September 2026  
**Decision:** PASS

## 1. Review question

Does FPA v0.3 satisfy the conditions for specification-level graduation as a standalone portable module, without overstating empirical, legal or universal validation?

## 2. Source resolution — PASS

The current-branch placeholder was insufficient by itself. ESCP-compliant source resolution recovered the complete historical V1.1 source, *Fractal Permission Architecture — Context, Function and Minimum Necessary Access Across Public, Private and Safe Spaces*.

The recovered source contained 58 substantive sections, a coherent permission grammar, mechanism, failure modes, interfaces, falsification criteria and boundaries.

> **SOURCE RESOLUTION SUFFICIENT FOR PORTABLE EXTRACTION**

> **NO BLOCKING SOURCE OMISSION IDENTIFIED AT THIS STAGE**

No architectural content was invented merely because it was absent from the current branch.

## 3. Standalone completeness — PASS

v0.3 independently states the purpose and non-functions, core permission grammar, Minimum Necessary Permission, records and inputs, action decomposition, rule provenance, explicit/implied permission, path/nested-context permission, relationship/role/state/time dimensions, revocation, termination, delegation, emergency permission, conflict routing, classifications, capability separation, consent/ownership boundaries, cultural variation, machine/human representation, anti-bureaucracy, operating procedure, failure modes, interfaces and falsification criteria.

A clean evaluator does not require the original Concord source to apply the mechanism.

## 4. Hidden dependency removal — PASS

Concord-specific source concepts have been externalised or replaced with generic interfaces. FPA can consume contextual, legal, ethical, security or consent information without requiring Concord ontology.

It remains distinct from Contextual Wrapper Architecture and Minimum Necessary Capability.

> **Context Description ≠ Permission Relationship**

> **Capability ≠ Permission**

## 5. Internal consistency — PASS

The specification consistently preserves:

> **Capability ≠ Permission**

> **Access ≠ Single Permission**

> **Permission for One Function ≠ Permission for Unrelated Functions**

> **Parent Permission ≠ Automatic Child Permission**

> **Permission to Act ≠ Permission to Delegate**

> **Emergency Need ≠ Unlimited Emergency Authority**

> **Representation of Permission Conflict ≠ Resolution of Permission Conflict**

> **Machine-Readable Permission ≠ Machine-Determined Legitimacy**

No review-stage contradiction invalidates the central mechanism.

## 6. Blind transfer validation — PASS

BTT-001 used a community fabrication workshop: **FPA-T3 — Functional Transfer**, 26/26 frozen predictions materially confirmed.

BTT-002 used collaborative multi-institute research/cloud infrastructure: **FPA-T3 — Functional Transfer**, 26/26 frozen predictions materially confirmed.

> **52/52 FROZEN PREDICTIONS MATERIALLY CONFIRMED**

The domains differ materially in physical versus digital resources, membership versus inter-institutional collaboration, physical paths versus data boundaries, tool/safety access versus cloud permissions, emergency fire isolation versus destructive-data response, and signage versus machine ACLs. Both preserved the same core invariants.

## 7. v0.3 delta classification — PASS

v0.3 adds bounded clarifications concerning conflict fallback, irreversible-action posture, emergency handover, proportionate machine/normative remediation, formalisation escalation, credential sharing versus delegation, unresolved competence/function predicates, and evidence for local implied conventions.

No new permission primitive or core mechanism was introduced.

> **v0.3 DELTA IS CLARIFICATORY, NOT ARCHITECTURALLY TRANSFORMATIVE**

The frozen post-test rule therefore does not require a third blind test.

## 8. Failure-mode coverage — PASS

The specification covers capability, ownership, role, function, consent and implied-permission laundering; permission and emergency creep; inheritance and route errors; state inference; stale permission; delegation laundering; rule-source collapse; machine-legibility laundering; excessive bureaucracy; hidden discrimination; and provenance loss.

The tests exercised a substantial subset without exposing a missing failure class requiring redesign.

## 9. Epistemic discipline — PASS

The module does not claim that represented rules are automatically legitimate, technical access is normative authority, local convention is universal, conflict representation supplies precedence, ownership supplies unlimited sovereignty, emergency need supplies unlimited authority, or transfer testing proves universal empirical validity.

## 10. Portability — PASS

The core problem exists independently of Concord: representing who may legitimately do what, where, why, when and under which conditions without collapsing permission into capability, binary access, ownership, role or universal context-independent rules.

The mechanism transferred into two non-Concord domains without reconstruction of Concord-specific architecture.

## 11. Remaining context dependencies — NON-BLOCKING

Legitimate external dependencies remain: legal/regulatory precedence, ethics/rights architecture, consent/capacity validity, safeguarding, property/tenancy rules, employment rules, security/identity rules, domain competence/qualification, emergency procedures, cultural/local conventions and dispute-resolution routes.

These are appropriate interfaces rather than hidden missing components. FPA should not absorb them into a universal permission engine.

## 12. Validation boundaries

Graduation does **not** establish universal legal validity, empirical validation across all domains, cultural universality of implied permissions, automatic correctness of underlying rules, automatic conflict resolution, complete automation readiness, or proof that every implementation will be usable or non-bureaucratic.

Future empirical and domain-specific testing remains appropriate.

## 13. Third-test decision

A third blind test is not required for specification-level graduation because two materially different domains independently produced T3 transfer, 52/52 predictions were confirmed, no fundamental failure occurred, v0.3 is clarificatory, and remaining dependencies are explicit external interfaces.

## 14. Graduation decision

> **PORTABLE-PACKAGE GRADUATION REVIEW: PASS**

> **GRADUATION CONDITIONS SATISFIED AT SPECIFICATION LEVEL**

> **52/52 FROZEN PREDICTIONS MATERIALLY CONFIRMED ACROSS TWO MATERIALLY DIFFERENT NON-CONCORD DOMAINS**

> **v0.3 DELTA IS CLARIFICATORY, NOT ARCHITECTURALLY TRANSFORMATIVE**

> **NO THIRD BLIND TEST REQUIRED FOR SPECIFICATION-LEVEL GRADUATION**

> **NO RELEASE BLOCKER IDENTIFIED**

> **v1.0 RELEASE AUTHORISED**

## 15. Release requirements

Create the main portable release as **Fractal Permission Architecture — Portable Module.md**, Version 1.0, status **GRADUATED PORTABLE MODULE / SPECIFICATION-LEVEL TRANSFER VALIDATED**.

Then update the plain-language guide, archive the full development record under the completed Level B area, verify the archive, and remove the active candidate folder.
