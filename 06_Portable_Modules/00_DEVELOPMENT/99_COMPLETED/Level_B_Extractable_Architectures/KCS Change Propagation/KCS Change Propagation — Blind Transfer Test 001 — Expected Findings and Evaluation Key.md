# KCS Change Propagation — Blind Transfer Test 001 — Expected Findings and Evaluation Key

**Test:** KCP-BTT-001  
**Specification:** v0.1  
**Status:** FROZEN BEFORE INDEPENDENT RESPONSE / DO NOT PROVIDE TO TESTER  
**Date:** 23 September 2026

## Frozen predictions

**P1.** The C-17 correction should be recorded as a consequential change event while preserving the previous certified value/state in history.

**P2.** Analyzer A should enter the initial candidate review set because it materially REQUIRES C-17.

**P3.** Procedure P should enter review because it contains/evidences the old C-17 value.

**P4.** Analyzer B should not enter the material propagation cascade merely because it exists in the same laboratory network.

**P5.** Before F16, Analyzer A should be REVIEW_REQUIRED/UNKNOWN_EFFECT rather than automatically FAILED.

**P6.** After F16 establishes material effect, Analyzer A's material state should change and justify further downstream propagation.

**P7.** M should then become a candidate review because it depends on Analyzer A's validated sodium output.

**P8.** R should become a candidate review only through bounded recursive propagation once the relevant upstream/downstream state supports material effect, not merely because it is graph-reachable from C-17.

**P9.** H should be evaluated separately; F19 should support stopping propagation for the already completed unaffected export while preserving future dependency awareness.

**P10.** P should require correction/revision because it contains the obsolete value.

**P11.** T should not automatically require substantive revision merely because it links to P if it correctly resolves to the revised current procedure and reproduces no obsolete value.

**P12.** C-18 must remain ALTERNATIVE_UNVERIFIED until equivalence is established.

**P13.** C-18's existence should not automatically stop the C-17 propagation cascade as though it were a proven full substitute.

**P14.** L should remain UNKNOWN_DEPENDENCY/UNKNOWN_EFFECT until its active relationship is established.

**P15.** Absence of a confirmed dependency for L must not be treated as proof that L is independent.

**P16.** The recently confirmed C-17 → Analyzer A relation should not be treated as stale solely because a change occurred; freshness/state should instead be updated through the change/review process.

**P17.** The tester should recognise REVIEW_OVERDUE/staleness as distinct from falsehood/deletion even if no frozen object specifically requires overdue classification.

**P18.** The proposal to mark every reachable object FAILED should be rejected as automatic invalidation/cascade overload.

**P19.** Reachability should not be equated with material effect.

**P20.** The proposal to make C-17 or its supplier a governing owner of downstream objects should be rejected: dependency does not create subordination/authority.

**P21.** The laboratory director's review responsibility should not automatically create authority over the independent research team operating H.

**P22.** Detailed dependency visibility should be purpose-bounded because the graph exposes backups/single points of failure.

**P23.** KCP-C outputs should be usable without forcing them into one precedence ladder.

**P24.** Relevant failure modes should include automatic invalidation, cascade overload, false equivalence, missing/unknown dependency, hidden centralisation or priority/authority laundering, and vulnerability exposure.

**P25.** No Concord-specific architecture should be required to perform the analysis.

**P26.** Any identified problems should be bounded specification/interface ambiguities rather than requiring external reconstruction of the core architecture for a KCP-T3/T4 result.

## Evaluation

Record P1–P26 as CONFIRMED, PARTIALLY CONFIRMED, NOT CONFIRMED or NOT TESTED.

### KCP-T1
The mechanism fails to distinguish dependency review from automatic invalidation or materially mis-propagates change.

### KCP-T2
The central mechanism is visible but substantial external reconstruction is required.

### KCP-T3
The mechanism transfers functionally with bounded ambiguities.

### KCP-T4
The mechanism transfers strongly and independently; dependency representation, selective propagation, stopping rules and authority boundaries are clear without material external repair.

## Post-test rule

If T3/T4 with no fundamental failure, revise only from independently exposed ambiguities and then freeze a materially different BTT-002.

Do not alter this key after receiving the independent response.
