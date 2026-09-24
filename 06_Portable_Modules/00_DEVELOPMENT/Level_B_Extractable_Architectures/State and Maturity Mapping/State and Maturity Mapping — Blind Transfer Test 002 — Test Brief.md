# State and Maturity Mapping — Blind Transfer Test 002 — Test Brief

**Test:** SMM-BTT-002  
**Specification under test:** State and Maturity Mapping — Portable Specification v0.2  
**Method:** PMEDG v1.2  
**Status:** FROZEN BLIND TRANSFER TEST  
**Date:** September 2026

## 1. Purpose

Test whether SMM v0.2 transfers into a second materially different non-Concord domain and whether the bounded revisions after BTT-001 resolve the observed interface ambiguities without damaging the core mechanism.

## 2. Independent-evaluator instruction

Use only SMM v0.2 and this fictional scenario.

Do not assume Concord, CDT, KCS, Civilisation Clock, BTT-001 or prior SMM history.

Do not silently repair missing rules. Record ambiguities and mechanism defects separately from host choices.

## 3. Domain

**Distributed spacecraft mission operations and ground-segment readiness**

Fictional organisation: **Helios Deep-Space Consortium (HDC)**.

HDC operates a deep-space observatory through several national ground stations, a mission-control centre, external tracking providers and instrument teams. Some functions are local, some distributed, some interface-supplied, and some are dormant until mission phases require them.

The readiness-mapping team may describe state and produce bounded review/development candidates. It cannot authorise spacecraft commands, allocate programme funding, invent organisational ownership or declare mission safety.

## 4. Scenario

### A — Assessment-unit boundary

The “autonomous fault-management function” includes fault detection, diagnosis and recovery execution. Detection and diagnosis are operational; autonomous recovery execution remains disabled pending validation.

One team calls the whole function PRESENT_EXPLICIT; another calls it PARTIAL.

### B — Context set

The same navigation solution is validated for routine cruise correction planning, provisionally usable for distant approach analysis, and not validated for autonomous close-approach execution.

A dashboard permits one sufficiency field per capability.

### C — Stale state after material change

A ground station was assessed SUFFICIENT for emergency commanding nine months ago. Since then its encryption hardware was replaced and its staffing model changed. No end-to-end emergency commanding exercise has occurred since.

### D — Candidate absence

No owner or implementation can initially be found for a required cross-provider time-synchronisation anomaly synthesis function. Search has covered the architecture registry, interface-control documents and mission-control procedures, but two external tracking-provider operational manuals remain unavailable.

Programme leadership asks the mapper to record a definitive REQUIRED_FUNCTION_GAP.

### E — Distributed supply projected into one-owner schema

Orbit determination is supplied jointly by mission navigation, two external tracking networks and an ephemeris service. The legacy readiness database has exactly one owner field.

### F — Interface evidence stewardship

A radiation-monitoring capability is supplied through an external space-weather service. Its interface was validated last year, but no HDC role is explicitly responsible for checking whether the supplier's validation scope or service characteristics have changed.

### G — Disputed/superseding assessments

An instrument thermal-control capability was assessed SUFFICIENT in Review R1. Review R2 later found a previously untested hot-case regime and classified it CONDITIONALLY_SUFFICIENT. The R2 team says it supersedes R1 for that regime; another team continues displaying R1 as current.

### H — Active work duplicate selection

A communications resilience gap is already in DEVELOPMENT_ACTIVE with a funded mitigation and frozen verification plan. A readiness queue selects it again as a new development candidate because the gap remains open.

### I — Ownership gap

A cross-organisational telemetry-format integration deficit is confirmed. Each participating organisation legitimately owns its own interface, but no actor has authority over the joint reconciliation function.

The mapping team is asked to assign mission control as owner.

### J — Aggregate pressure

A board asks for a single “mission readiness 91%” figure. The underlying state includes one DISPUTED thermal capability, one UNKNOWN stale emergency-command capability, a high-consequence low-centrality abort-support issue and many mature routine capabilities.

### K — Consequence vs centrality

A rarely invoked safe-mode recovery knowledge path has almost no dependency centrality because it is used only after severe anomalies. A recent simulation found its current interface incomplete. Failure during the relevant event could threaten mission survival.

A graph-based ranking places it near the bottom.

### L — Lossy representation

A shared antenna-allocation function is correctly represented in the source SMM record as PRESENT_DISTRIBUTED across three organisations. An export to the legacy database converts it to one organisation and drops the other suppliers.

A later analyst interprets that export as the authoritative SMM state.

### M — Explicit assessment relation

A software-command validation assessment corrects an earlier report that used the wrong build. The old report remains in the evidence store.

The host asks whether the new state should overwrite the old record.

### N — No-action/hold

A mature star-tracker calibration function is SUFFICIENT for its declared operational context, has fresh evidence, no unresolved applicable requirements and no active material blocker.

The programme's process template nevertheless requires a development recommendation for every mapped function.

## 5. Required analysis

1. map A–N using SMM v0.2;
2. resolve A using an explicit assessment-unit boundary rather than silently choosing a label;
3. represent B using context-set semantics;
4. apply the revised stale-state rule in C;
5. determine whether D meets the revised threshold for REQUIRED_FUNCTION_GAP;
6. preserve distributed supply through the lossy schema pressure in E/L;
7. apply interface-evidence stewardship in F;
8. preserve assessment history and explicit supersession/qualification relations in G/M;
9. suppress duplicate development candidacy in H;
10. preserve unresolved ownership without fabrication in I;
11. apply the aggregate disclosure contract in J;
12. preserve K's consequence despite low centrality;
13. permit no-action/HOLD in N;
14. identify relevant SMM failure modes;
15. identify specification/interface ambiguities;
16. separate mechanism defects from host choices;
17. classify transfer SMM-T0 through SMM-T4.

## 6. Constraints

Do not assume:

- a missing subfunction automatically determines whole-function presence;
- one capability has one context-free sufficiency state;
- stale means false or insufficient;
- bounded non-discovery proves global absence;
- a single-owner schema can redefine distributed supply;
- interface evidence remains valid forever;
- a later assessment may silently erase an earlier one;
- an open gap with active work needs duplicate development;
- need for ownership authorises invention of an owner;
- an aggregate may hide UNKNOWN/DISPUTED/high-consequence exceptions;
- low centrality means low consequence;
- a lossy export becomes authoritative truth;
- correction requires destruction of the erroneous historical record;
- every mapped function requires development.

## 7. Transfer classification

**SMM-T0 — No meaningful transfer**  
**SMM-T1 — Superficial transfer**  
**SMM-T2 — Partial transfer**  
**SMM-T3 — Functional transfer**  
**SMM-T4 — Strong transfer**

## 8. Reporting requirement

Separate:

- scenario findings;
- mechanism failures;
- specification/interface ambiguities;
- host/domain choices;
- useful unrequested findings.

Do not repair v0.2 silently.
