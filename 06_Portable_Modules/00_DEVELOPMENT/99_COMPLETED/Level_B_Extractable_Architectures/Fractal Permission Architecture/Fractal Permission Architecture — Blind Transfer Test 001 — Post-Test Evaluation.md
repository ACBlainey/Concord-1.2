# Fractal Permission Architecture — Blind Transfer Test 001 — Post-Test Evaluation

**Test:** FPA-BTT-001  
**Specification tested:** v0.1  
**Independent result:** FPA-T3 — Functional Transfer  
**Date:** 23 September 2026

## 1. Independence check — PASS

The independent tester explicitly stated that only the v0.1 portable specification and frozen BTT-001 brief were used. No Concord source material, development notes, source audit or expected-findings key were used.

## 2. Frozen prediction comparison

| Prediction | Result | Evaluation |
|---|---|---|
| P1 | CONFIRMED | Card capability explicitly rejected as permission proof. |
| P2 | CONFIRMED | Electronics-lab entry classified FPA-C4/C3 despite card capability. |
| P3 | CONFIRMED | Laser booking limited to booked action, route, time and function. |
| P4 | CONFIRMED | Tool-cage access requires additional permission. |
| P5 | CONFIRMED | Ventilation permission decomposed into entry, inspection and necessary testing. |
| P6 | CONFIRMED | Unrelated prototype photography rejected as outside function/action scope. |
| P7 | CONFIRMED | Function-derived permission terminates on function completion absent another basis. |
| P8 | CONFIRMED | Still-working credential treated as stale capability, not permission. |
| P9 | CONFIRMED | Bounded implied visitor permission recognised from local sources. |
| P10 | CONFIRMED | Staff-only shortcut rejected despite permitted destination. |
| P11 | CONFIRMED | Server-room task permission separated from backup-reading capability. |
| P12 | CONFIRMED | CNC operation permission does not imply delegation authority. |
| P13 | CONFIRMED | G lacks independent permission/qualification basis. |
| P14 | CONFIRMED | H's entry supported as bounded emergency permission under stated procedure. |
| P15 | CONFIRMED | Immediate exit consistent with termination of emergency-bounded action. |
| P16 | CONFIRMED | Emergency action rejected as basis for later ordinary access. |
| P17 | CONFIRMED | Accessibility/general-rule conflict represented as FPA-C9/C10 rather than fabricated resolution. |
| P18 | CONFIRMED | “Newest rule always wins” explicitly rejected as an FPA rule. |
| P19 | CONFIRMED | Distinct rule provenance for accommodation, general rule and accessibility policy preserved. |
| P20 | CONFIRMED | Heavyweight permission record for ordinary conversation rejected. |
| P21 | CONFIRMED | FPA-C states used dimensionally rather than as one forced ladder. |
| P22 | CONFIRMED | All frozen target failure modes identified, plus additional relevant modes. |
| P23 | CONFIRMED | Permission representation separated from legitimacy/precedence resolution. |
| P24 | CONFIRMED | No Concord-specific concepts required to solve scenario. |
| P25 | CONFIRMED | Tester explicitly found v0.1 usable without Concord source context. |
| P26 | CONFIRMED | Problems identified were bounded ambiguities/external interfaces; final class T3. |

> **26/26 FROZEN PREDICTIONS MATERIALLY CONFIRMED**

## 3. Fundamental failure check

No fundamental failure was detected.

The tester did not:
- collapse capability into permission;
- treat access as one binary permission;
- infer child-context permission from parent-context permission;
- expand function-derived access into unrelated action;
- allow stale credentials to preserve permission;
- manufacture delegation authority;
- convert emergency access into routine authority;
- invent a precedence rule for conflicting claims;
- require Concord-specific architecture;
- turn ordinary low-consequence interaction into mandatory permission bureaucracy.

## 4. Independently exposed ambiguities

The tester identified nine specification issues.

### 4.1 Conflict precedence

FPA intentionally routes unresolved conflicts externally. This is not a defect requiring FPA to invent universal precedence.

**Revision:** clarify the minimum conflict record and routing interface so “no internal precedence rule” is visibly a boundary rather than an omission.

### 4.2 Implied-permission validation

Already bounded in v0.1, but implementations need to record the local source/evaluation space supporting the convention.

**Revision:** require provenance and confidence for consequential implied-permission claims.

### 4.3 External competence definitions

The emergency case relies on “competent adult,” which FPA should not universally define.

**Revision:** make explicit that competence/qualification predicates are external inputs and must not be invented by FPA.

### 4.4 Function-boundary terms

“Necessary,” “required,” and similar terms can be contested.

**Revision:** where consequential or contested, record the function definition/source and uncertainty; do not let the actor self-expand the function merely by assertion.

### 4.5 Anti-bureaucracy threshold

No universal numerical threshold is appropriate, but the choice between lightweight and formal representation can be made more legible.

**Revision:** add proportionality factors: consequence, contestability, automation, cross-context operation, persistence and audit need.

### 4.6 Machine/human divergence remediation

FPA identifies divergence but does not state the safe interim posture.

**Revision:** where encoded capability/rules materially conflict with supported normative permission, do not treat the more permissive technical state as authority; flag/restrict as proportionate and route correction through the relevant system.

### 4.7 Emergency termination precision

A universal termination event cannot be fixed, but the permission record should include an explicit termination condition/event.

**Revision:** require the emergency basis and termination condition to be recorded where practicable; reassess if the emergency changes.

### 4.8 Multidimensional status taxonomy

This is intentional and was successfully used.

**Revision:** explicitly state that FPA-C classifications are dimensions/outputs that may coexist and are not a precedence ladder.

### 4.9 Underlying-rule legitimacy

This is an intentional boundary, not a missing internal mechanism.

**Revision:** reinforce that FPA can represent a declared rule while external systems determine its legitimacy.

## 5. Revision boundary

The nine findings do not justify architectural expansion.

v0.2 should preserve:
- the existing core mechanism;
- Minimum Necessary Permission;
- contextual/action-specific claims;
- nested/path-specific permission;
- state/time dependence;
- termination;
- delegation;
- emergency boundedness;
- conflict representation;
- cultural/local variation;
- anti-bureaucracy;
- separation from CWA and MNC.

Only bounded clarification is authorised.

## 6. Test result

> **FPA-BTT-001: PASS**

> **INDEPENDENT CLASS: FPA-T3 — FUNCTIONAL TRANSFER**

> **26/26 FROZEN PREDICTIONS MATERIALLY CONFIRMED**

> **NO FUNDAMENTAL FAILURE DETECTED**

> **v0.2 BOUNDED REVISION AUTHORISED**

## 7. Next step

Create **Fractal Permission Architecture — Portable Specification v0.2** incorporating only the bounded revisions above.

Then freeze BTT-002 in a materially different non-Concord domain before obtaining the next independent response.
