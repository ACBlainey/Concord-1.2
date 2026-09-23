# KCS Change Propagation — Blind Transfer Test 002 — Independent Response

**Test:** KCP-BTT-002  
**Specification tested:** v0.2  
**Independent result:** KCP-T4 — Strong Transfer  
**Date received:** 23 September 2026

## Independence

The clean tester states that it used only **KCS Change Propagation — Portable Specification v0.2** and the frozen scenario.

## Preserved findings

The tester correctly bounds the change to F-9 v9.3 on S-4 revision B at East Plant during 10–17 September, rather than generalising it to all firmware, sensors, plants or time periods. The externally supplied 0.10 mg/L review threshold is consumed as a host input rather than invented by KCP.

S-8 is excluded using affirmative independence evidence. S-4 is degraded only for the affected scope and is not automatically failed.

Control System C is materially reviewed despite being a non-transforming store/display, preserving **No Transformation ≠ No Material Effect**.

D is REVIEW_REQUIRED + UNKNOWN_EFFECT, with external escalation appropriate because the unresolved effect is safety-critical. No downstream effects are invented.

P is separated into affected historical display and corrected current display. R is likewise separated into the unaffected August report and the not-yet-generated September report requiring review.

CP requires review because it contains affected examples. Q does not automatically require substantive revision because it only references the current CP and contains no affected values.

F-10 remains ALTERNATIVE_UNVERIFIED until external compatibility testing. L remains UNKNOWN_DEPENDENCY + UNKNOWN_EFFECT, with source-grounded discovery/escalation justified before completeness claims.

Three months does not automatically create a stale/overdue relation without a host freshness rule.

The tester rejects both the all-FAILED proposal and conversion of safety-criticality/connectivity into organisational authority or priority.

Purpose-bounded visibility is preserved because the graph exposes control-system and fallback details.

KCP-C classifications are treated as dimensional/coexistent.

## Residual specification issues

The tester identifies five bounded implementation/interface points:

1. classifications should explicitly bind scope/time/instance because one object can carry different classifications for different intervals or versions;
2. hosts must supply criteria for when high-consequence UNKNOWN states require external escalation;
3. the prose distinguishes documents that contain/evidence/reference, but the shared relation vocabulary lacks a dedicated REFERENCES/REFERS_TO relation;
4. host displays need to present coexistent DEGRADED / REVIEW_REQUIRED / UNKNOWN_EFFECT states clearly;
5. public-notification decisions correctly remain external to KCP.

## Final assessment

> **KCP-T4 — Strong Transfer**

The tester finds that v0.2 successfully handles bounded change scope, non-transforming conduits, host-defined thresholds, high-consequence unknown dependencies, document semantics, alternative verification, historical preservation, authority separation and purpose-bounded visibility.

Residual issues are minor host-interface and implementation-scope matters rather than failures of the portable architecture.
