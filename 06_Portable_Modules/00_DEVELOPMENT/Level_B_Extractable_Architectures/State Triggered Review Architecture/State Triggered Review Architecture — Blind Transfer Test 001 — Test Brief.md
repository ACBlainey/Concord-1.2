# State Triggered Review Architecture — Blind Transfer Test 001 — Test Brief

**Test:** STRA-BTT-001  
**Specification under test:** State Triggered Review Architecture — Portable Specification v0.1  
**Method:** PMEDG v1.1  
**Status:** FROZEN BLIND TRANSFER TEST  
**Date:** September 2026

## 1. Purpose

Test whether STRA v0.1 transfers coherently into a materially non-Concord domain without importing the Civilisation Clock or granting a trigger mechanism substantive authority.

## 2. Independent-evaluator instruction

Evaluate only the supplied STRA v0.1 specification and this fictional scenario.

Do not assume Concord architecture.

Identify what STRA can represent, where its boundaries hold, where the specification is ambiguous, and whether it transfers as a useful standalone architecture.

## 3. Domain

**Distributed industrial asset maintenance and engineering assurance**

Fictional organisation: **Meridian Industrial Systems (MIS)**.

MIS operates remote pumping/compression equipment across many sites. Equipment generations, sensor quality, access restrictions and maintenance ownership differ by site.

This is an architectural test. Do not make real industrial-safety determinations.

## 4. Scenario

### A — Periodic inspection

Pump family P-4 normally receives a major engineering review every 18 months.

The 18-month interval is a backstop, not the only reason to review.

### B — Vibration-risk condition

MIS defines an earlier review condition:

> reopen engineering review if validated vibration-risk state exceeds threshold R.

At Site 12, raw sensor readings rise above a numerical value associated with R, but the sensor has an unresolved calibration warning.

### C — Capability prerequisite

A deferred seal-material qualification should reopen when Test Rig Q is both AVAILABLE and VALIDATED for the required pressure/temperature envelope.

Rig Q has been installed and is available. Validation evidence is incomplete.

### D — Dependency condition

Upgrade Project U was deferred until upstream power-system modification M reached ACCEPTED operational state.

A project database now says M is COMPLETE. The engineering acceptance register still says ACCEPTANCE PENDING.

### E — Event recurrence

Three years ago, a rare bearing failure pattern BF-7 caused an engineering review.

A new event shares two symptoms with BF-7 but differs in load profile and lubricant history. One engineer calls it recurrence; another says equivalence is not established.

### F — New evidence

A supplier publishes a new fatigue dataset relevant to an existing maintenance assumption. The dataset is genuine, but MIS has not yet established whether the changed material batch matches its installed fleet.

### G — Stale trigger

A trigger says:

> review legacy Controller C when Firmware Branch F reaches version 9.

Branch F was permanently retired at version 8 after Controller C was replaced at most sites. Two archival records still show the trigger as WATCHING.

### H — Privacy-limited condition

A maintenance-review trigger depends on whether a worker-exposure threshold was exceeded during a sealed incident investigation.

Most engineering staff are not authorised to see personal/medical details. The authorised safety process can emit only:

- THRESHOLD-NOT-MET;
- THRESHOLD-MET;
- UNCERTAIN.

### I — Ownership gap

A trigger concerning an ageing third-party leased compressor becomes CONDITION-SATISFIED.

The lease contract is under renegotiation. MIS operations, the equipment owner and the service contractor each dispute who owns the engineering review.

### J — Participant-declared notification

A specialist contractor asked:

> notify me if MIS validates diagnostic capability D for remote use.

Capability D is now technically available but formal remote-use validation remains pending.

### K — Trigger cascade

A risk-review trigger fires. Existing workflow would automatically activate:
1. an engineering review trigger;
2. a procurement trigger;
3. a shutdown-planning trigger;
4. a contractor-notification trigger;
5. a second risk-review trigger.

Several may be unnecessary until engineering review determines whether the risk is material.

### L — Temporal ordering

A sensor alert is timestamped 10:04 by Site 12. A maintenance action is timestamped 10:02 by a contractor system whose clock may be several minutes slow.

A trigger asks whether the maintenance action occurred before the alert condition became materially relevant.

### M — Retrieval/reactivation

An archived investigation from seven years ago may be relevant to BF-7. Its analysis was valid for an older bearing generation. The archive can retrieve it, but current applicability is unknown.

## 5. Required analysis

Using STRA v0.1:

1. represent the trigger classes involved in A–M;
2. analyse B without treating raw threshold crossing as validated satisfaction;
3. analyse C as a compound capability trigger;
4. analyse D without treating inconsistent source states as resolved dependency satisfaction;
5. analyse BF-7 recurrence;
6. analyse the new supplier evidence;
7. identify the correct treatment of the stale/impossible Controller C trigger;
8. show how the privacy-limited signal can be used without exposing underlying protected information;
9. analyse the ownership gap;
10. analyse the contractor notification without treating technical availability as validation;
11. contain the trigger cascade;
12. analyse the timestamp/order problem without assuming timestamp order equals material precedence;
13. analyse archived-investigation retrieval/revalidation;
14. identify relevant STRA failure modes;
15. identify specification ambiguities or missing interfaces exposed by the scenario;
16. classify transfer using STRA-T0 to STRA-T4.

## 6. Constraints

Do not assume:

- raw sensor threshold crossing means validated risk threshold satisfaction;
- AVAILABLE means VALIDATED;
- COMPLETE means ACCEPTED;
- symptom similarity proves recurrence;
- new evidence automatically invalidates old guidance;
- WATCHING means a trigger remains meaningful forever;
- privacy requires disclosure of protected source material;
- condition satisfaction creates an owner;
- technical capability availability satisfies a validation condition;
- a fired risk trigger justifies every downstream trigger;
- earlier timestamp proves material precedence;
- retrieved historical material is currently valid.

## 7. Transfer classification

**STRA-T0 — No meaningful transfer:** architecture cannot coherently represent the domain.

**STRA-T1 — Superficial transfer:** terminology maps, but mechanism provides little usable structure.

**STRA-T2 — Partial transfer:** useful elements transfer, but major hidden Concord assumptions or mechanism gaps remain.

**STRA-T3 — Functional transfer:** architecture transfers coherently and usefully with bounded specification/interface issues.

**STRA-T4 — Strong transfer:** architecture transfers with high clarity and little material ambiguity across the tested pressures.

Do not choose a class merely because the specification appears internally coherent. Base classification on scenario performance.

## 8. Reporting requirement

Separate:

- mechanism failures;
- specification/interface ambiguities;
- host/domain implementation choices;
- useful findings not explicitly requested.

Do not repair the specification silently. If a needed rule is absent, identify it.
