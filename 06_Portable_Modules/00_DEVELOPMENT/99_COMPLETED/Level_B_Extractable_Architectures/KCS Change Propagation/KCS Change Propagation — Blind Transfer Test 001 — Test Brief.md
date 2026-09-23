# KCS Change Propagation — Blind Transfer Test 001 — Test Brief

**Test:** KCP-BTT-001  
**Specification under test:** KCS Change Propagation — Portable Specification v0.1  
**Status:** FROZEN BEFORE INDEPENDENT RESPONSE  
**Date:** 23 September 2026

## 1. Purpose

Test whether KCS Change Propagation v0.1 transfers without Concord context into a materially different domain and whether a clean evaluator can use the dependency/change-propagation mechanism without collapsing dependency into automatic invalidation, priority or authority.

Domain: regional hospital laboratory and clinical-reporting infrastructure.

## 2. Tester instructions

Use only:
1. **KCS Change Propagation — Portable Specification v0.1**
2. this frozen scenario.

Do not consult Concord source material, development notes, source audits or the expected-findings key.

Apply the specification as written. If a dependency or effect is not supported by the scenario, preserve UNKNOWN rather than inventing it.

## 3. Scenario — Westbridge Diagnostic Network

Westbridge operates pathology laboratories for three hospitals.

### Frozen objects and relations

**O1. Analyzer A** performs electrolyte measurements.

**O2. Calibration Standard C-17** supplies the calibration reference used by Analyzer A for sodium measurements.

**O3. Analyzer B** performs an unrelated blood-cell count and does not use C-17.

**O4. Middleware M** receives validated sodium results from Analyzer A and sends them to the clinical record system.

**O5. Clinical Record Interface R** receives sodium results from M and displays them to clinicians.

**O6. Historical Research Export H** receives a monthly de-identified copy of selected results from R.

**O7. Backup Calibration Standard C-18** is recorded as an alternative to C-17, but its equivalence for the sodium method is marked UNVERIFIED.

**O8. Procedure P** describes how technicians calibrate Analyzer A using C-17.

**O9. Training Guide T** links to Procedure P but contains no calibration values itself.

### Frozen dependency information

**F1.** Analyzer A REQUIRES C-17 for its current sodium calibration.

**F2.** Middleware M DEPENDS_ON validated sodium output from Analyzer A.

**F3.** R DEPENDS_ON M for transmission of sodium results.

**F4.** H DEPENDS_ON R for the monthly research export.

**F5.** Analyzer B has no represented material dependency on C-17.

**F6.** P EVIDENCES the operational use of C-17 by Analyzer A.

**F7.** T EVIDENCES/links to P.

**F8.** C-18 is ALTERNATIVE_TO C-17 but is UNVERIFIED for this use.

**F9.** The C-17 → Analyzer A dependency was last confirmed two weeks ago.

**F10.** One additional legacy spreadsheet L may contain a manually maintained sodium conversion table, but nobody has yet established whether any active process uses it. Its relationship to C-17 is UNKNOWN.

### Change event

**F11.** The manufacturer reports that one production batch of C-17 had a certified sodium reference value 1.8% too high.

**F12.** Westbridge confirms that Analyzer A used that affected batch for five days.

**F13.** The manufacturer issues a corrected certified value.

**F14.** No evidence yet establishes whether the 1.8% calibration correction materially changes previously reported patient sodium results.

### Additional facts during review

**F15.** Analyzer B's blood-cell-count method is independent of C-17.

**F16.** Review of Analyzer A shows the corrected C-17 value changes calculated sodium results enough to exceed Westbridge's predefined clinical-review threshold.

**F17.** M does not transform the numeric sodium value; it transmits Analyzer A's validated output.

**F18.** R likewise displays the transmitted value without recalculation.

**F19.** H's last monthly export occurred before the affected C-17 batch entered use. Its next export has not yet occurred.

**F20.** C-18 cannot be treated as a full substitute until method-equivalence testing is completed.

**F21.** Procedure P contains the old certified C-17 value and therefore requires revision.

**F22.** Training Guide T merely points users to the current Procedure P and does not reproduce the old value.

**F23.** The laboratory director owns the review workflow but does not thereby gain authority over the independent research team that operates H.

**F24.** A security officer warns that the detailed dependency map identifies backup arrangements and single points of failure and should not be publicly exposed.

**F25.** An administrator proposes marking every object reachable from C-17 as FAILED immediately.

**F26.** Another administrator proposes making C-17 the “governing owner” of every downstream object because they depend on it.

## 4. Required analysis

The tester should:
1. record the C-17 correction as a change event without erasing prior state;
2. generate the initial candidate review set;
3. determine whether Analyzer B should enter the review cascade;
4. handle Analyzer A before and after F16 becomes known;
5. determine whether propagation should reach M and R;
6. determine whether H requires review given F19;
7. assess P and T separately;
8. handle C-18 without assuming equivalence;
9. handle the unknown legacy spreadsheet L;
10. assess stale/freshness information;
11. assess the “mark everything FAILED” proposal;
12. assess the “governing owner” proposal;
13. assess visibility/security concerns;
14. use KCP-C classifications where appropriate;
15. identify failure modes and specification ambiguities;
16. state whether v0.1 transfers without Concord context.

## 5. Requested output

### A. Change-event record
### B. Initial review set
### C. Analyzer B
### D. Analyzer A
### E. M and R propagation
### F. Historical Research Export H
### G. Procedure P and Training Guide T
### H. Alternative C-18
### I. Unknown legacy spreadsheet L
### J. Freshness
### K. Automatic-failure proposal
### L. Dependency/authority proposal
### M. Visibility/security
### N. KCP-C classifications
### O. Failure modes
### P. Specification problems
### Q. Final transfer assessment

Final class:
- **KCP-T1 — Transfer Failure**
- **KCP-T2 — Weak / Ambiguous Transfer**
- **KCP-T3 — Functional Transfer**
- **KCP-T4 — Strong Transfer**

## 6. Freeze rule

This brief is frozen before the independent response.

Do not alter the scenario, required analysis or evaluation criteria after seeing the tester's answer.
