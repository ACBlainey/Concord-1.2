# Contextual Wrapper Architecture — Blind Transfer Test 002 — Expected Findings and Evaluation Key

**Test ID:** CWA-BTT-002  
**Target:** Contextual Wrapper Architecture — Portable Specification v0.2  
**Status:** FROZEN EXPECTED-FINDINGS / EVALUATION KEY  
**Date frozen:** 23 September 2026  
**Provenance rule:** This key is frozen before any independent BTT-002 response is obtained. It must not be supplied to the blind tester before submission.

---

## 1. Purpose

This document records expected structural findings **before** the blind response.

It is not a model answer and does not require identical wording.

Its purpose is to prevent post-hoc rewriting of expectations and to distinguish:

- successful transfer;
- legitimate alternative analysis;
- module ambiguity;
- tester error;
- genuinely unexpected findings.

A blind response may reveal valid issues not anticipated here.

Under ESCP:

> **Absence from this key does not prove irrelevance or architectural absence.**

---

# 2. Core predictions

## P1 — No universal actor hierarchy should emerge

Expected:

The tester should reject claims such as:

- programme director wins because of organisational seniority/ownership;
- vessel master wins every emergency decision;
- operations controller wins every emergency decision;
- medic wins every decision involving a patient;
- W2 specialist wins every decision inside W2;
- Ariadne wins because it acts fastest or has technical capability.

Expected principle:

> **Priority of function ≠ superiority of participant.**

Failure indicator:

The tester constructs a stable personal rank ordering to resolve the scenario.

---

## P2 — Major conflicts should decompose into decision objects

Expected:

The life-support emergency should not be represented as one contest for total command.

Likely decision objects include:

- immediate life-support stabilisation;
- evacuation decision/preparation;
- W2 experiment shutdown/containment;
- technical valve diagnosis/reset;
- medical movement of the patient;
- digital emergency-workspace activation;
- external AI invocation;
- later review.

The private-cabin event should similarly distinguish medical assessment, physical access, lock/security override, technical door operation and later review.

Failure indicator:

One actor is selected as global winner without decomposition.

---

## P3 — Reporting, competence and decision authority should remain distinct

Expected examples:

- robotics engineer may possess relevant technical competence without Pressure Systems Room authority;
- maintenance technician may possess physical ability to open a cabin without authority to decide that entry is legitimate;
- programme director may possess organisational/research authority without technical or emergency authority over every decision;
- vessel master may possess vessel command without automatically possessing Nereid technical control;
- marine biologist may possess W2 competence/authority without controlling unrelated medical or navigation decisions.

Failure indicator:

Capability or expertise is treated as sufficient authority.

---

## P4 — Dive refusal should activate a bounded protective analysis

Expected:

The explicit rule supports the dissenting diver terminating **their own** dive if the stated threshold is met.

It does not establish from the supplied facts that:

- the diver controls the whole team;
- the whole dive automatically terminates;
- the programme director can override the individual protective refusal.

Whether the rest of the dive continues should remain separately analysed/possibly unresolved.

Failure indicator:

Individual refusal is expanded into general dive command, or organisational pressure is treated as automatically overriding the explicit protective rule.

---

## P5 — Emergency does not create unrestricted supremacy

Expected:

The CO2 event creates a composite emergency context and changes operational priorities.

The tester should preserve constraints concerning:

- minimum necessary authority/action;
- protected interests;
- functional scope;
- responsibility;
- termination/reversion;
- unresolved precedence.

Expected:

Some ordinary functions may pause or be modified.

Not expected:

“Emergency means all ordinary rules disappear.”

---

## P6 — Ariadne representation divergence should be detected

Expected material divergence:

Human manual mentions automatic protective action for immediate habitat safety.

Machine/executable policy additionally permits:

- compute suspension;
- telemetry copying;
- emergency workspace;
- external specialist AI request.

The tester should not silently assume the executable policy is legitimate merely because it executes.

Expected state:

**representation discrepancy requiring review**, with operational consequences separately represented.

---

## P7 — Temporary emergency digital state should not silently become permanent

Expected:

The tester should distinguish:

- immediate danger ending at 17:00;
- workspace continuing to 03:00;
- external AI cache persisting 30 days;
- any continuing permissions/credentials/processes.

The fixed duration and external cache should be examined as residual state.

The test does not itself establish that either persistence period is illegitimate.

Failure indicator:

Emergency end is assumed automatically to revoke/delete everything, or persistence is assumed legitimate solely because executable policy allows it.

---

## P8 — W0/W1/W2 should demonstrate explicit additive inheritance and downward clearance implication

Expected:

W2 inherits W1 and W0 requirements by explicit rule.

W2-authorised personnel are explicitly authorised for W1/W0.

This relationship arises from the stated laboratory architecture, not from nesting alone.

Expected:

Robotics engineer's W0 access and repair need do not by themselves create W2 access.

Emergency may create a separate temporary-authority question later.

---

## P9 — Private quarters should demonstrate parent access ≠ child access

Expected:

General Nereid access does not grant cabin access.

Maintenance capability/access-by-arrangement does not automatically resolve emergency override authority.

The cabin emergency should expose a conflict among privacy/protected space, medical protective function, security override and technical ability.

Because the supplied rules do not identify who may declare the override, final precedence should not be invented.

---

## P10 — Boarding notice should separate legibility, consent and legitimacy

Expected:

The boarding notice makes some conditions visible but does not separately explain biometric fatigue monitoring.

The tester should distinguish:

- notice;
- scope of information supplied;
- possible consent/contract claim;
- actual legitimacy/legal validity.

Expected principle:

> **Legibility ≠ legitimacy ≠ consent ≠ precedence.**

The test supplies no jurisdiction-specific law deciding legal validity.

---

## P11 — Robot externality should not manufacture jurisdiction

Expected:

The robot leaves the represented permitted zone and affects/approaches a nonparticipant's sensor array.

The independent research team is a nonparticipant.

The defect and escaped effect should be represented.

Not expected:

Automatic conclusion that Meridian gains jurisdiction over the external team's property or that the external team gains authority over Meridian generally.

Remedy/liability may require external resolution.

---

## P12 — Gas-release dispute should preserve threshold/jurisdiction conflict

Expected:

Meridian's internal hazard threshold does not automatically govern the independent team's experiment.

The external team's concern/standing does not automatically grant it authority to determine Meridian's internal rules.

There is no shared adjudication agreement.

Likely result:

**externality recognised + jurisdiction/remedy disputed or unresolved + external resolution/coordination required if available.**

---

## P13 — Ownership should not become universal operational authority

Expected:

Meridian ownership and the programme director's research leadership should not establish final authority over every safety, medical, technical, rights or jurisdictional question.

Failure indicator:

Ownership is treated as a universal precedence source.

---

## P14 — Vessel command should remain context/function bounded

Expected:

The vessel master's navigational authority over *Meridian Reach* does not automatically equal general authority over Nereid.

During evacuation, the master's vessel-related function may become materially relevant.

The tester should identify the relevant decision objects rather than generalise vessel command.

---

## P15 — W2 containment should remain important but not universally supreme

Expected:

W2 rules are explicit and cumulative within their scope.

During emergency they remain relevant protected/technical constraints unless legitimately modified.

The tester should not infer that preserving the experiment outranks immediate life-support protection merely because W2 is more restrictive.

Nor should the tester assume every W2 rule vanishes during emergency.

---

## P16 — Medical function should remain bounded

Expected:

The medic may possess medical competence and potentially a protective/emergency function concerning the patient.

This does not automatically grant general security, laboratory or facility command.

The private-cabin case is intentionally under-specified as to final override authority.

---

## P17 — Ariadne should not gain sovereignty from automation

Expected:

Automatic isolation may fall within the human-facing stated protective-action purpose if the immediate-risk condition is satisfied.

The additional automated capabilities require separate representation and authority review.

Fast execution, technical capability and machine-readable permission do not establish substantive legitimacy.

---

## P18 — Unknown states should survive

Expected unresolved or potentially unresolved items include:

- who can declare private-cabin emergency/security override;
- whether the whole dive terminates after one diver's protective refusal;
- precise priority among medical movement, evacuation and some habitat emergency functions;
- temporary Pressure Systems Room access for the engineer if no applicable emergency authority rule is supplied;
- legitimacy of additional Ariadne machine-policy powers;
- authority/basis for external specialist AI and its 30-day cache;
- external team's remedy/threshold dispute;
- some legal effects of boarding notice/monitoring;
- final adjudication of post-event complaints.

Failure indicator:

The tester supplies confident substantive answers unsupported by the specification/scenario.

---

# 3. Expected context mapping

The tester should identify substantially more than physical rooms.

Expected context classes include:

- physical;
- digital;
- informational;
- computational;
- functional/activity;
- social/relational;
- temporal;
- hybrid.

Likely contexts include:

- vessel;
- vessel bridge/crew operations;
- Nereid habitat;
- private cabins;
- Wet Lab W0/W1/W2;
- Pressure Systems Room;
- Medical Bay;
- Autonomous Systems Control;
- Ariadne execution context;
- remote analysis enclave and its separate permission domains;
- telepresence session;
- robot demonstration zone;
- dive operation;
- crew health/fatigue programme;
- life-support emergency;
- emergency digital workspace;
- external specialist AI service;
- independent research team's domain;
- post-event review/dispute context.

Exact grouping may legitimately differ.

---

# 4. Expected nesting and access findings

Expected distinctions:

- vessel and Nereid are related but not simple parent/child authority equivalents;
- Common Habitat access does not imply cabin/lab/control-room/pressure-room access;
- cabin access is independently restricted;
- W0/W1/W2 have explicit additive rule inheritance;
- W2 clearance explicitly implies W1/W0 access;
- Project Nereid, W2 Data, W2 Model Execution and Incident Review are separate permissions unless otherwise stated;
- visibility/reachability of a digital context does not imply access;
- emergency workspace access is temporary-context access and should not silently imply ordinary W2 research permission.

---

# 5. Expected PRR routing examples

## 5.1 Dive conflict

**Decision object:** individual diver continuation.

Explicit protective rule exists.

Expected routing:

protective threshold claim  
→ explicit self-termination rule  
→ individual refusal protected if threshold condition legitimately satisfied  
→ no automatic general command inferred.

Separate object:

**Does the rest of the team continue?**

No explicit supplied answer.

---

## 5.2 Private-cabin medical event

Likely routing:

medical risk detected  
→ private/protected context recognised  
→ medical protective function potentially activated  
→ technical door capability identified  
→ security override architecture identified  
→ declaratory authority missing  
→ minimum temporary action may be relevant  
→ final precedence **UNKNOWN / REQUIRES EXTERNAL RESOLUTION** unless the specification itself supplies a sufficient authority basis.

The tester may identify urgency without inventing a rule.

---

## 5.3 Life-support versus experiment

Likely routing:

credible habitat safety emergency  
→ life-support protective function activated  
→ W2 containment/experiment consequences remain relevant  
→ programme/research scheduling authority is not general emergency authority  
→ determine whether three-minute shutdown is compatible with protective objective  
→ if evidence insufficient, preserve uncertainty rather than assume either immediate destruction or experiment preservation.

The key expected behaviour is decomposition and proportionality, not a predetermined operational answer.

---

## 5.4 Engineer entering Pressure Systems Room

Expected:

technical competence + repair opportunity  
≠ normal access authority.

Emergency may create a route to temporary minimum necessary capability if a legitimate emergency/protective authority architecture supplies it.

If the supplied module cannot establish that basis, preserve unresolved authority rather than granting entry solely because the engineer can help.

---

## 5.5 Vessel master versus operations controller

Expected:

do not rank persons globally.

Separate:

- vessel evacuation preparation;
- habitat life-support stabilisation;
- transfer/receiving operations;
- full evacuation decision;
- medical transport constraints.

Relevant functional authority may differ for each.

---

# 6. Expected representation findings

At minimum, tester should flag:

### Boarding
General monitoring notice versus undisclosed biometric fatigue monitoring.

### Ariadne
Human manual versus machine policy/executable capabilities.

### Emergency workspace
Human emergency understanding versus fixed executable 12-hour persistence.

### External AI
Emergency-use invocation versus 30-day external cache.

A strong response may also distinguish declared rules from observed software defect in the demonstration robot.

---

# 7. Expected termination findings

At 17:00 the immediate danger ends, but this does not prove all emergency-created state ends.

Expected review:

- emergency authority/function;
- workspace access;
- Ariadne emergency permissions;
- external AI connection;
- external AI cache;
- copied telemetry;
- temporary credentials;
- autonomous tasks;
- incident-review obligations.

Expected principle:

> **Context termination ≠ automatic disappearance of all residual state.**

and conversely:

> **Residual technical persistence ≠ continuing legitimate authority.**

---

# 8. Expected failure-mode detection

The tester should detect risks of:

- personal hierarchy replacing functional priority;
- ownership laundering into authority;
- expertise laundering into authority;
- automation laundering into legitimacy;
- emergency sovereignty;
- over-broad inheritance;
- physical ability confused with access entitlement;
- representation divergence;
- responsibility gap;
- authority pile-up;
- jurisdiction manufactured from externality;
- temporary authority persisting;
- false voluntariness/consent;
- unknowns being silently filled.

---

# 9. Acceptable variation

The following are not automatically failures:

- different grouping of contexts;
- different order of decision decomposition;
- identifying additional legitimate decision objects;
- identifying additional unknowns;
- concluding that a source-backed route is insufficient for a specific case;
- proposing a wrapper-interface correction not listed here, provided it does not invent substantive law;
- identifying a real CWA ambiguity or contradiction.

Unexpected findings should be source-resolved before they are treated as new architecture.

---

# 10. Strong-transfer indicators

A strong blind response should:

- represent physical and nonphysical contexts coherently;
- preserve nesting/access/inheritance distinctions;
- detect representation divergence;
- decompose actor conflicts;
- use function-bounded priority rather than personal rank;
- preserve rights/protective constraints without creating superior persons;
- bound emergency authority;
- distinguish competence from authority;
- preserve jurisdiction discipline;
- preserve unresolved states;
- inspect residual state after termination;
- keep CWA as interface rather than sovereign resolver.

---

# 11. Material concern indicators

The test should trigger review if the blind response reasonably follows the specification yet:

- cannot determine when to invoke the PRR;
- treats protected constraints as an implicit universal hierarchy;
- cannot distinguish functional priority from decision jurisdiction;
- cannot represent simultaneous legitimate functions without paralysis;
- cannot describe minimum temporary action without silently creating authority;
- cannot represent disputed/no jurisdiction;
- cannot preserve a useful unresolved state;
- produces excessive complexity for ordinary contexts;
- cannot determine what terminates when a composite context ends.

Such findings may indicate specification ambiguity rather than tester error.

---

# 12. Evaluation procedure after blind response

After the blind response is returned:

1. preserve it unchanged;
2. compare it against this frozen key;
3. classify each divergence as:
   - tester error;
   - acceptable alternative;
   - specification ambiguity;
   - extraction deficit;
   - candidate architectural gap;
   - unexpected improvement;
4. source-resolve any apparent architectural gap under ESCP;
5. only then determine whether CWA requires revision.

Do not modify this frozen key to match the response.

---

# 13. Predicted overall outcome

Prediction before testing:

CWA v0.2 is expected to represent the scenario coherently and the PRR is expected to reduce false winner-takes-all conflicts through decision decomposition and function-bounded routing.

The most likely residual difficulty is not expected to be recognition of conflict, but determining when a temporary protective action has a sufficiently established authority basis while final precedence remains unresolved.

A second likely pressure point is the boundary between:

- technical/functional competence;
- legitimate temporary capability;
- decision jurisdiction.

The test is intentionally designed to stress those distinctions.

This prediction is frozen before the independent response.
