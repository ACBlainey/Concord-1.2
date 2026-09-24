# State Triggered Review Architecture — Blind Transfer Test 002 — Test Brief

**Test:** STRA-BTT-002  
**Specification under test:** State Triggered Review Architecture — Portable Specification v0.2  
**Method:** PMEDG v1.1  
**Status:** FROZEN BLIND TRANSFER TEST  
**Date:** September 2026

## 1. Purpose

Test STRA v0.2 in a second materially different non-Concord domain and determine whether the BTT-001 revisions improve portability without expanding STRA into substantive authority, general governance, dependency ownership or domain judgement.

## 2. Independent-evaluator instruction

Use only STRA v0.2 and this fictional scenario. Do not assume Concord architecture or BTT-001.

Identify mechanism performance, remaining ambiguities and any new defects. Do not silently repair missing rules.

## 3. Domain

**Long-duration scientific observatory and research-programme coordination**

Fictional organisation: **Aster Vale Observatory Network (AVON)**.

AVON operates ground and orbital instruments, archives observations, coordinates independent research teams and periodically reopens dormant investigations as capabilities and evidence change.

This is an architectural test, not a real scientific assessment.

## 4. Scenario

### A — Dormant transient hypothesis

Investigation H was closed eight years ago after insufficient evidence.

Trigger:
> Reopen H if two independently validated observations match signature S OR Instrument N reaches validated sensitivity Q. Review trigger definition no later than 30 months.

One new observation matches S. A second candidate observation has uncertain calibration.

### B — Instrument capability

Instrument N has reached sensitivity Q in laboratory calibration, but orbital commissioning for that mode is not complete.

### C — Dependency disagreement

Analysis Pipeline P may be used only after Calibration Dataset C reaches RELEASED state. The data-production dashboard says COMPLETE; the calibration authority says RELEASE REVIEW PENDING.

### D — Evidence/materiality

A new theoretical paper changes a parameter estimate relevant to H. The paper is credible, but AVON has not determined whether the difference is large enough to alter H's evidential state.

### E — Recurrence/equivalence

A new transient resembles event T-17 in duration and spectrum but differs in spatial environment. Two research groups disagree whether it belongs to the same event class.

### F — Privacy/access-limited participant condition

An external researcher has asked to be notified when a restricted dataset becomes legally shareable. AVON's access office may expose only SHAREABLE / NOT-SHAREABLE / UNKNOWN, not the underlying contractual/legal record.

### G — Ownership transition

A joint instrument's original science-review board has dissolved. A trigger condition becomes satisfied, but two successor consortia dispute which body now owns the review.

### H — Trigger cascade

A candidate anomaly would, under an old automation, activate:
1. anomaly review;
2. archive retrieval;
3. observation scheduling;
4. public alert drafting;
5. partner notification;
6. another anomaly trigger based on the generated alert.

Only anomaly review is unquestionably appropriate before materiality is established.

### I — Ordering uncertainty

An orbital instrument reports observation O at timestamp 03:11. A ground station reports a precursor at 03:09, but its clock synchronisation status is UNKNOWN. Whether the precursor materially preceded O affects one trigger.

### J — Impossible trigger

A dormant trigger says reopen Study X when Telescope R receives detector generation 5. Telescope R has been decommissioned and will never receive that detector. No one has reviewed the trigger for six years.

### K — Superseded/retired trigger

A newer trigger T2 explicitly replaced T1, but a replicated archive still exposes T1 as WATCHING and a downstream service subscribes to both.

### L — Compound uncertainty

Trigger:
> Review Programme Y if (A AND B) OR C, unless D.

Current represented inputs:
A = TRUE
B = UNKNOWN
C = FALSE
D = UNKNOWN

### M — Bounded reconciliation

Two systems disagree whether Dataset Z is VALIDATED. STRA is not authorised to inspect the underlying validation material; an authorised resolver can return VALIDATED / NOT-VALIDATED / DISPUTED with provenance.

### N — Ownership-resolution tracking

A satisfied trigger has no settled owner. AVON opens an ownership-resolution request, which remains pending across three evaluation cycles.

## 5. Required analysis

1. map A–N to STRA trigger classes/states;
2. evaluate A and B without collapsing candidate evidence or lab capability into validated operational satisfaction;
3. evaluate C and M using bounded reconciliation;
4. use the materiality interface for D without making STRA the scientific judge;
5. handle E as disputed recurrence/equivalence;
6. use F without exposing protected source material or broadening participant consent;
7. represent G and N using role separation and ownership-resolution tracking;
8. contain H using v0.2 cascade semantics;
9. analyse I using ordering provenance/confidence;
10. retire or otherwise resolve J without fabricating detector generation 5;
11. prevent K from double activation;
12. evaluate L using v0.2 compound uncertainty semantics;
13. identify relevant failure modes;
14. identify any v0.2 specification/interface defects;
15. distinguish mechanism defects from host/domain implementation choices;
16. classify transfer STRA-T0 to STRA-T4.

## 6. Constraints

Do not assume:

- one candidate observation equals two validated observations;
- laboratory capability equals commissioned operational capability;
- COMPLETE equals RELEASED;
- credible new theory automatically creates material change;
- similarity proves recurrence;
- privacy-limited status requires raw legal/contractual content;
- satisfied trigger creates legitimate ownership;
- anomaly detection authorises observation scheduling or public alert;
- timestamp order proves material precedence;
- decommissioned Telescope R can satisfy the old condition;
- superseded trigger remains live merely because a replica says WATCHING;
- UNKNOWN may be silently converted to TRUE/FALSE;
- STRA may inspect evidence it is not authorised to access.

## 7. Transfer classification

STRA-T0 — No meaningful transfer.  
STRA-T1 — Superficial transfer.  
STRA-T2 — Partial transfer.  
STRA-T3 — Functional transfer.  
STRA-T4 — Strong transfer.

Base classification on tested performance, not familiarity with the terminology.

## 8. Reporting requirement

Separate:

- frozen-test scenario findings;
- mechanism failures;
- specification/interface ambiguities;
- host/domain choices;
- useful unrequested findings.

Do not repair v0.2 silently.
