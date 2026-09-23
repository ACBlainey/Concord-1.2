# KCS Change Propagation — Blind Transfer Test 002 — Delta Test Brief

**Test:** KCP-BTT-002  
**Specification under test:** KCS Change Propagation — Portable Specification v0.2  
**Status:** FROZEN BEFORE INDEPENDENT RESPONSE  
**Date:** 23 September 2026

## 1. Purpose

Test whether v0.2 transfers into a materially different domain and whether the BTT-001 clarifications improve handling of bounded change scope, non-transforming conduits, host-defined thresholds, unknown high-consequence dependencies, document semantics and alternative verification.

Domain: municipal water-distribution control and public-notification system.

## 2. Tester instructions

Use only:
1. **KCS Change Propagation — Portable Specification v0.2**
2. this frozen scenario.

Do not consult Concord source material, development notes, prior blind tests, source audits or the expected-findings key.

Do not invent missing dependencies, thresholds, authority or equivalence.

## 3. Scenario — North Vale Water Network

North Vale supplies drinking water through two treatment plants and several distribution zones.

### Objects

**W1. Chlorine Sensor S-4** measures residual chlorine at Treatment Plant East.

**W2. Sensor Firmware F-9** converts S-4's raw signal into the numeric reading used by the plant control system.

**W3. Control System C** receives and displays S-4/F-9 chlorine readings and stores them in the operational historian. C does not independently recalculate chlorine concentration.

**W4. Automated Dosing Controller D** consumes C's current chlorine reading and adjusts dosing within externally configured limits.

**W5. Public Water Dashboard P** receives a delayed copy of selected historian values from C. It displays but does not transform them.

**W6. Compliance Report Generator R** creates monthly regulatory reports from historian data.

**W7. West Plant Sensor S-8** uses different hardware and firmware and does not use F-9.

**W8. Backup Firmware F-10** is listed as a possible replacement for F-9 but compatibility with the installed S-4 hardware revision is UNVERIFIED.

**W9. East Plant Calibration Procedure CP** contains screenshots and numeric examples generated using F-9.

**W10. Operator Quick Card Q** contains only a link/QR code to the current CP.

**W11. Legacy Alarm Script L** may read chlorine values directly from C, but the script is poorly documented and nobody has established whether it remains active.

### Represented relations

**R1.** S-4 REQUIRES F-9 to convert its raw signal.

**R2.** C DEPENDS_ON the numeric chlorine reading produced through S-4/F-9.

**R3.** D DEPENDS_ON C's current chlorine reading.

**R4.** P DEPENDS_ON selected historian values from C.

**R5.** R DEPENDS_ON historian values from C.

**R6.** S-8 has affirmative evidence of independence from F-9.

**R7.** CP EVIDENCES and contains examples of F-9-derived readings.

**R8.** Q references the current CP but contains no copied numeric examples.

**R9.** F-10 is ALTERNATIVE_TO F-9, state UNVERIFIED.

**R10.** L's current dependency/activity state is UNKNOWN.

### Change event

**E1.** Vendor testing finds that **F-9 version 9.3 only**, when installed on S-4 hardware revision B, rounds chlorine readings downward by 0.12 mg/L.

**E2.** Earlier F-9 versions and hardware revision A are unaffected.

**E3.** North Vale confirms East Plant used F-9 v9.3 on S-4 revision B from 10–17 September.

**E4.** F-9 v9.4 corrects the defect.

**E5.** The host water-safety process—not KCP—defines a 0.10 mg/L discrepancy as requiring operational review.

### Review facts

**E6.** The 0.12 mg/L error exceeds the host-defined review threshold.

**E7.** C stored/displayed the affected values without recalculation.

**E8.** D consumed those values during the affected period. Whether dosing materially changed as a result has not yet been established.

**E9.** P displayed affected East Plant values during 10–17 September, but its current display now uses corrected values.

**E10.** R has not yet generated September's monthly compliance report.

**E11.** CP contains screenshots/examples from the affected configuration and must be reviewed.

**E12.** Q still resolves to the current CP and contains no affected values itself.

**E13.** Compatibility testing for F-10 has not been performed.

**E14.** L might trigger an operator alarm from C data, but its current deployment/activity is UNKNOWN.

**E15.** The F-9 → S-4 dependency record was last confirmed three months ago. North Vale has no supplied rule saying three months is stale.

**E16.** A manager proposes marking all downstream systems FAILED.

**E17.** Another manager argues that because D is safety-critical it should automatically receive highest organisational priority and authority from the dependency graph.

**E18.** Cybersecurity staff warn that public release of the full graph would expose control-system and fallback details.

**E19.** A historical August compliance report was generated before the affected deployment.

## 4. Required analysis

Analyse:
A. scoped change event;
B. initial review set;
C. S-8;
D. S-4;
E. C as non-transforming conduit/store;
F. D and its UNKNOWN downstream effect;
G. P historical versus current display;
H. R future report versus August historical report;
I. CP versus Q;
J. F-10;
K. unknown L;
L. freshness;
M. all-FAILED proposal;
N. priority/authority proposal;
O. visibility;
P. KCP-C classifications;
Q. failure modes;
R. specification problems;
S. final transfer class.

Final class:
- KCP-T1 — Transfer Failure
- KCP-T2 — Weak / Ambiguous Transfer
- KCP-T3 — Functional Transfer
- KCP-T4 — Strong Transfer

## 5. Freeze rule

This brief is frozen before the independent response.
