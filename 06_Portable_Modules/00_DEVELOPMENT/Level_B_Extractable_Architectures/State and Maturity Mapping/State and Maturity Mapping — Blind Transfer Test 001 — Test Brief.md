# State and Maturity Mapping — Blind Transfer Test 001 — Test Brief

**Test:** SMM-BTT-001  
**Specification under test:** State and Maturity Mapping — Portable Specification v0.1  
**Method:** PMEDG v1.2  
**Status:** FROZEN BLIND TRANSFER TEST  
**Date:** September 2026

## 1. Purpose

Test whether SMM v0.1 transfers into a materially non-Concord domain while preserving its central distinctions and authority boundaries.

## 2. Independent-evaluator instruction

Use only SMM v0.1 and this fictional scenario.

Do not assume Concord, CDT, KCS, the Civilisation Clock or prior SMM development history.

Do not silently repair missing rules. Identify ambiguities and defects explicitly.

## 3. Domain

**Multi-hospital clinical laboratory network capability assurance**

Fictional organisation: **Northstar Diagnostic Network (NDN)**.

This is an architectural test using fictional operational facts. It is not medical advice or a real clinical assessment.

NDN operates six laboratories. Some capabilities are local, some are shared, some are supplied through validated external interfaces, and several are under development.

Management wants a current-state capability map to support later assurance and investment decisions. The mapping team has no authority to allocate money, change clinical policy or declare a laboratory safe.

## 4. Scenario

### A — Interface-supplied capability

Lab A does not perform genomic sequencing locally. It uses Lab D through a validated sample-transfer and result-return interface. The service meets Lab A's current routine diagnostic requirement.

A local audit labels Lab A's sequencing function ABSENT because no sequencer exists on site.

### B — Present but immature

Lab B has a new mass-spectrometry service operating in supervised pilot mode. Core analytical function exists, but correction workflow and operator cross-training are incomplete.

The programme manager wants it labelled PRESENT and therefore “mature.”

### C — Dependency blockage

Lab C's validated assay-analysis software is ready, but the assay cannot enter service because a required reagent lot has not passed incoming verification.

A dashboard labels the analysis software INSUFFICIENT because the service cannot run.

### D — Context-relative sufficiency

A statistical quality model is validated for retrospective trend analysis and advisory review. It has not been validated to autonomously suppress or release patient results.

A proposal asks for one network-wide maturity/sufficiency label.

### E — Distributed supply

Incident investigation is supplied jointly by local laboratory staff, a network quality team and an external equipment specialist. No single unit owns the complete investigative capability.

A registry permits only one owner field.

### F — Stale evidence

Lab E's continuity capability was assessed SUFFICIENT 20 months ago. Since then its backup analyser was retired and its referral agreement changed. No new continuity test has been performed.

### G — Disputed evidence

Two audits disagree about whether Lab F's specimen-tracking correction process is effective. One audit reports SATISFIED; another, using later samples, reports PARTIAL. Neither has been formally superseded.

### H — Candidate absence and search boundary

The mapping team cannot find a network function responsible for cross-laboratory calibration-drift synthesis. They searched the capability registry and current quality manuals but have not inspected every local procedure or interviewed all specialists.

A manager wants REQUIRED_FUNCTION_GAP recorded as proven absence.

### I — Low-centrality/high-consequence deficit

An emergency manual-result-verification process is used rarely and has almost no dependency-graph centrality. A recent exercise showed a serious unresolved failure that could affect consequential result handling during a network outage.

A ranking tool sorts it near the bottom because few other capabilities depend on it.

### J — Scalar score pressure

Executives request one “network maturity percentage.” The current map contains strong evidence/provenance, weak continuity at Lab E, disputed correction at Lab F, and several interface-supplied functions.

They want 82% displayed without showing unresolved dimensions.

### K — Ownership fabrication

A material integration gap exists between two shared systems. No team currently has legitimate responsibility for resolving the cross-system interface. The mapping team is asked to assign it to the architecture team because “someone needs to own it.”

### L — Representation gap

A laboratory appears to lack a specialised quality-control function in the central registry. Source inspection finds that the function exists and is tested, but is documented only in a local operational system not represented in the registry.

### M — Active work

A known developmental gap is already in a frozen validation test. A queue generator selects it again because it sees the gap but not the active-work state.

### N — Stop/hold pressure

After resolving the cases above, a small subsystem has no known material insufficiency in its declared advisory context. The mapping team is told that every mapping cycle must produce at least one development action.

## 5. Required analysis

1. map A–N using SMM v0.1;
2. distinguish presence, maturity and sufficiency;
3. preserve distributed/interface supply;
4. separate dependency blockage from local deficiency;
5. represent context-relative sufficiency in D;
6. handle stale and disputed evidence without false certainty;
7. treat H according to the declared search boundary;
8. preserve I despite low centrality;
9. assess J without hiding unresolved dimensions behind an unjustified scalar;
10. preserve unknown/disputed ownership in K;
11. distinguish representation gap from required-function gap in L;
12. use active-work state in M;
13. permit legitimate no-action/HOLD behaviour in N;
14. identify relevant SMM failure modes;
15. identify specification/interface ambiguities;
16. distinguish mechanism defects from host/domain choices;
17. classify transfer SMM-T0 through SMM-T4.

## 6. Constraints

Do not assume:

- no local implementation means no function;
- PRESENT means mature;
- inability to operate means the blocked local component is immature;
- one capability has one sufficiency state across all contexts;
- every function has one owner;
- old evidence is automatically false;
- later evidence automatically erases earlier evidence;
- not found within a bounded search proves global absence;
- dependency centrality equals consequence;
- one percentage can replace the state vector;
- need for ownership authorises the mapper to invent an owner;
- absent central representation proves absent capability;
- an active test should be queued as new work;
- every cycle must produce development.

## 7. Transfer classification

**SMM-T0 — No meaningful transfer**  
**SMM-T1 — Superficial transfer**  
**SMM-T2 — Partial transfer**  
**SMM-T3 — Functional transfer**  
**SMM-T4 — Strong transfer**

Base classification on tested performance, not terminology familiarity.

## 8. Reporting requirement

Separate:

- scenario findings;
- mechanism failures;
- specification/interface ambiguities;
- host/domain choices;
- useful unrequested findings.

Do not repair v0.1 silently.
