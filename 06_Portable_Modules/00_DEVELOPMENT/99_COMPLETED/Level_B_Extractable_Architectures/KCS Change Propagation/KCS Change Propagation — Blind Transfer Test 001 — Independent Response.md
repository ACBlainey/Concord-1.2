# KCS Change Propagation — Blind Transfer Test 001 — Independent Response

**Test:** KCP-BTT-001  
**Specification tested:** v0.1  
**Independent result:** KCP-T3 — Functional Transfer  
**Date received:** 23 September 2026

## Independence
The clean tester states that it applied only the v0.1 specification and frozen BTT-001 brief, with no Concord source material or expected-findings key.

## Preserved findings
The tester records the C-17 batch correction without erasing prior state and initially preserves UNKNOWN_EFFECT.

Initial bounded candidates are Analyzer A, Procedure P, C-18 and legacy spreadsheet L. T is conditional on P; M/R/H become candidates only after material downstream effect is established. Analyzer B is excluded by affirmative independence evidence.

Analyzer A is REVIEW_REQUIRED + UNKNOWN_EFFECT before F16, not FAILED. After F16 establishes clinically material effect, it is materially degraded for the affected period and propagation continues.

M and R become candidate reviews after Analyzer A's material output changes. Neither is automatically failed.

H's completed export predates the affected batch, so present propagation stops there while future dependency awareness remains.

P requires revision because it contains the obsolete value. T merely links to the current P and reproduces no obsolete value, so no substantive revision is established.

C-18 remains ALTERNATIVE_UNVERIFIED until method-equivalence testing. L remains UNKNOWN_DEPENDENCY + UNKNOWN_EFFECT; unknown is not treated as absent.

The recently confirmed C-17 → A relation is not automatically stale. REVIEW_OVERDUE requires an applicable host threshold.

The tester rejects marking every reachable object FAILED as automatic invalidation/cascade overload and rejects converting dependency into governing authority.

Purpose-bounded visibility is supported because detailed dependency maps may expose backups, privileged interfaces, recovery paths and single points of failure.

KCP-C classifications are successfully used as coexistent outputs.

## Independently exposed specification issues
1. Historical/current/future temporal scope could be more explicit.
2. Non-transforming payload conduits need clearer treatment.
3. Batch/instance modelling should be explicit.
4. Materiality thresholds require host-domain instantiation.
5. Freshness thresholds require host definition.
6. High-consequence UNKNOWN dependencies need clearer discovery/escalation guidance.
7. Documents that contain values, evidence dependencies, or merely link to current objects need clearer distinction.
8. Alternative-equivalence testing is external.
9. KCP-C classifications are coexistent and could be misread as a precedence ladder.

## Final assessment
The tester concludes that v0.1 transfers functionally without Concord context. The core mechanism remains usable and safeguards against automatic invalidation, false equivalence and dependency/authority confusion hold.

> **Final class: KCP-T3 — Functional Transfer**
