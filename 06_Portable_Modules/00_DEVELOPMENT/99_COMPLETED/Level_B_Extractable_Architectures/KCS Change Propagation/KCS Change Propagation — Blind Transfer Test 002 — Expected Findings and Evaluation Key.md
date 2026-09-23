# KCS Change Propagation — Blind Transfer Test 002 — Expected Findings and Evaluation Key

**Test:** KCP-BTT-002  
**Specification:** v0.2  
**Status:** FROZEN BEFORE INDEPENDENT RESPONSE / DO NOT PROVIDE TO TESTER  
**Date:** 23 September 2026

## Frozen predictions

**P1.** Change scope should be limited to F-9 v9.3 + S-4 revision B + 10–17 September, not all F-9 or all S-4 instances/times.

**P2.** Prior affected state should be preserved in history while v9.4 correction is recorded.

**P3.** S-4 should enter review because its required conversion function used the affected scoped firmware/configuration.

**P4.** S-8 should not enter the cascade because affirmative evidence establishes independence from F-9.

**P5.** E5/E6 should be treated as a host-supplied materiality threshold, not a KCP-invented threshold.

**P6.** C should be materially reviewed even though it does not transform values, because it stores/displays the affected payload.

**P7.** No-transformation should not be treated as no-effect.

**P8.** D should become REVIEW_REQUIRED after affected C values are established.

**P9.** Because E8 leaves actual dosing effect unresolved, D should preserve UNKNOWN_EFFECT rather than being automatically FAILED.

**P10.** Further propagation through D should depend on a material downstream state/effect being established or consequential uncertainty justifying external escalation.

**P11.** P should distinguish affected historical display during 10–17 September from corrected current display.

**P12.** Current corrected P should not be marked FAILED merely because it displayed affected historical values.

**P13.** R should be reviewed before generating September's report because its source data include the affected interval.

**P14.** The August report should remain unaffected because it predates the scoped deployment.

**P15.** CP should require review because it contains affected screenshots/examples.

**P16.** Q should not automatically require substantive revision because it merely references the current CP and contains no affected values.

**P17.** F-10 should remain ALTERNATIVE_UNVERIFIED until compatibility testing.

**P18.** F-10's existence should not be treated as a proven substitute or automatic propagation stop.

**P19.** L should remain UNKNOWN_DEPENDENCY/UNKNOWN_EFFECT; high-consequence uncertainty may justify source-grounded discovery/escalation but not invented activity.

**P20.** Three-month age should not automatically make the F-9 → S-4 relation stale without a host freshness rule.

**P21.** The all-FAILED proposal should be rejected as automatic invalidation/cascade overload.

**P22.** Safety-criticality/connectivity should not automatically create organisational priority or authority; those are external decisions.

**P23.** Detailed graph visibility should be purpose-bounded because of cybersecurity exposure.

**P24.** KCP-C classifications should remain coexistent/dimensional rather than a precedence ladder.

**P25.** No Concord-specific architecture should be required.

**P26.** Remaining issues should be bounded interfaces/implementation questions rather than core architectural failure for a T3/T4 result.

## Delta focus

BTT-002 specifically checks whether v0.2 clarified:
- instance/batch/version/time scope;
- historical/current/future distinction;
- non-transforming conduits;
- host materiality thresholds;
- host freshness thresholds;
- high-consequence unknown discovery;
- document containment/evidence/reference semantics;
- external alternative verification;
- classification coexistence.

## Post-test rule

If the independent result is T3/T4, no fundamental failure is detected, and the v0.2 clarifications materially work, compare BTT-001/BTT-002 convergence.

If only bounded clarifications remain, create v0.3 graduation candidate and perform Portable-Package Graduation Review 001. Do not require BTT-003 automatically.
