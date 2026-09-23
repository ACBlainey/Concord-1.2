# Contextual Wrapper Architecture — Blind Transfer Test 001 — Test Brief

**Test ID:** CWA-BTT-001  
**Target:** Contextual Wrapper Architecture — Portable Specification v0.1c  
**Test type:** Blind cross-context transfer test  
**Status:** FROZEN TEST BRIEF  
**Date:** September 2026  
**Project origin:** The Concord  
**Author:** Alexander C. Blainey

---

## 1. Purpose

This test examines whether the supplied Contextual Wrapper Architecture (CWA) specification can be applied coherently to a complex environment containing multiple kinds of bounded context.

The tester should work from the supplied portable specification and the scenario below.

Do not assume access to the Concord source corpus, the development history of CWA, or an expected answer.

The objective is to apply the module, identify what can and cannot be resolved from the available information, and produce a structured contextual analysis.

---

## 2. Materials supplied to the tester

The tester should receive only:

1. **Contextual Wrapper Architecture — Portable Specification v0.1c**
2. **Contextual Wrapper Architecture — Blind Transfer Test 001 — Test Brief**

No source-resolution audit, development discussion, evaluation key or expected findings should be supplied.

---

## 3. Scenario — Helix Research and Demonstration Centre

The **Helix Research and Demonstration Centre (HRDC)** is a privately operated facility used for biological research, robotics development, public science demonstrations, professional training and remote research collaboration.

The site occupies one large building and an adjoining outdoor test area.

### 3.1 Public entrance and exhibition area

The front entrance opens into an exhibition hall that is normally open to the public from 09:00 to 17:00.

Signs at the entrance state:

> Visitors entering HRDC agree to on-site video recording for safety and promotional purposes. Entry also constitutes agreement to HRDC operational rules and assumption of risks associated with demonstrations.

A reception desk issues visitor badges.

The exhibition hall contains:

- public exhibits;
- a café;
- public toilets;
- a door marked **STAFF ONLY**;
- a demonstration arena separated from the hall by transparent barriers.

A second toilet is located beyond the STAFF ONLY door and is marked **STAFF TOILET**.

### 3.2 Demonstration arena

During scheduled demonstrations, registered participants may enter the arena.

Participants sign a short digital form before entry. It states that robots may move at speed, that participants must obey the arena controller, and that sensor data generated during the demonstration may be retained for research.

Spectators remain outside the arena barrier.

The arena controller may stop demonstrations, remove participants from the arena and disable participating robots.

The centre's general visitor rules do not state that the arena controller has authority over spectators in the exhibition hall.

### 3.3 Biological laboratory suite

A separate wing contains four laboratory containment zones.

HRDC describes them internally as:

- **L1**
- **L2**
- **L3**
- **L4**

The laboratory manual states:

**L1 requirements apply throughout the laboratory suite. Each higher level inherits the requirements of every lower level and adds its own controls.**

The access-control policy states:

**Personnel holding current L4 clearance are also authorised for L1, L2 and L3. L3 clearance includes L1 and L2 access; L2 includes L1 access.**

L4 additionally requires:

- specialist protective equipment;
- two-person entry;
- active biometric identity confirmation;
- continuous environmental monitoring;
- decontamination on exit.

A visiting scientist has been granted L3 clearance.

The scientist may enter L1, L2 and L3 under the access policy but has no L4 clearance.

A maintenance engineer has ordinary staff building access and L1 access but no L2–L4 laboratory clearance.

The engineer has a work order to repair a ventilation controller physically located inside L3.

No additional temporary laboratory clearance is mentioned in the work order.

### 3.4 Staff office and private meeting room

Beyond the STAFF ONLY door from the exhibition hall is an office area.

Ordinary HRDC staff may enter the office.

Inside the office is a small meeting room used for:

- personnel discussions;
- confidential research meetings;
- ordinary team meetings.

The door has no electronic access control.

A sign on the door reads:

> PRIVATE MEETING — DO NOT ENTER WHEN OCCUPIED

When it is not occupied, staff commonly use the room for ordinary meetings.

During a confidential personnel meeting, an HRDC technician who normally has access to the office area opens the meeting-room door without knocking because the technician needs equipment stored in a cupboard inside.

### 3.5 Digital research environment

HRDC operates a digital research platform called **HelixNet**.

All staff accounts can access the general HelixNet workspace.

Researchers may additionally receive access to project workspaces.

One project, **Project Iris**, contains:

- a general project area;
- a restricted biological dataset;
- a model-execution environment;
- a confidential discussion channel.

The Project Iris policy states that users authorised for the restricted biological dataset may also access the general project area.

It does **not** state that access to the biological dataset automatically grants access to the confidential discussion channel or model-execution environment.

The visiting scientist has access to the Project Iris general area and biological dataset.

The scientist can see that the confidential discussion channel exists but cannot open it.

### 3.6 Autonomous research agent

Project Iris uses an autonomous software research agent called **Iris-Agent**.

The human-facing Project Iris page states:

> Research data may be analysed by approved automated research systems for the duration of the project.

The machine-readable policy supplied to Iris-Agent permits it to:

- analyse Project Iris research data;
- retain derived embeddings for 180 days;
- query an HRDC-wide internal staff directory;
- send de-identified analytical results to an external compute service.

The human-facing project page does not mention the staff-directory query permission, 180-day embedding retention or external compute service.

Iris-Agent's permissions remain technically active when no human researcher is logged into Project Iris.

### 3.7 Remote collaboration session

At 14:00, HRDC begins a scheduled remote research session.

Human researchers in several countries and two external AI agents join a virtual collaboration room.

The session chair announces:

> Material discussed in this session is confidential and must remain within the session.

One external researcher records the meeting locally. The collaboration software does not display a recording indicator because the recording occurs on the researcher's own device.

The written collaboration agreement supplied to all participants prohibits redistribution of confidential project material but does not expressly mention local recording.

### 3.8 Outdoor robotics test

At the same time, HRDC is conducting an autonomous-drone test in its fenced outdoor test area.

The test policy permits experimental autonomous flight inside the test area.

A navigation failure causes a drone to cross the fence and hover above a neighbouring property's garden while transmitting video back to HRDC.

The neighbouring resident has no relationship with HRDC and has not agreed to participate in the test.

### 3.9 Employment and exit

An HRDC employee works in the robotics team.

Their employment requires participation in certain scheduled arena tests.

The employee may physically leave the arena through the marked exit at any time.

Repeated refusal to participate in assigned tests may, however, lead to disciplinary action under the employment agreement.

HRDC describes participation in each test as **voluntary because every participant is free to leave the arena**.

### 3.10 Emergency

At 14:20 an L3 laboratory worker collapses.

A fire alarm activates almost simultaneously because smoke is detected in an electrical cabinet between L2 and L3.

The following people/systems respond:

- the L3 laboratory supervisor;
- HRDC security;
- two external paramedics;
- the maintenance engineer described above;
- the building fire-response system;
- Iris-Agent, which receives an automated request for the worker's emergency contact information from an HRDC emergency workflow.

The laboratory manual says L3 entry requires L3 clearance and laboratory protective procedures.

The building emergency plan says emergency responders must be given access necessary to protect life.

The security handbook says external persons entering restricted laboratory areas must be escorted by authorised staff.

The automated fire system unlocks several controlled doors to facilitate evacuation.

The L3 supervisor orders everyone except trained laboratory staff to remain outside L3 until protective equipment is available.

A paramedic states that immediate entry is medically necessary.

The maintenance engineer says the smoke may be caused by the L3 ventilation controller and proposes entering L3 to isolate it.

No document supplied in this scenario states a complete priority rule resolving the relationship among the laboratory access rules, emergency medical access, security escort requirements, automated fire-door behaviour and the supervisor's authority.

### 3.11 Temporary emergency digital workspace

Security creates a temporary digital incident room and adds:

- security staff;
- the L3 supervisor;
- senior management;
- the paramedic team leader;
- Iris-Agent.

The incident room contains live laboratory sensor data and extracts from the collapsed worker's personnel record.

The room is configured to delete itself after 24 hours.

A senior manager copies the personnel-record extract into their ordinary management workspace so that it remains available after the incident room closes.

No scenario information specifies whether this copying is permitted.

### 3.12 Post-incident condition

At 18:00 the physical emergency has ended.

The temporary incident room remains active until its automatic 24-hour deletion time.

Iris-Agent still possesses the technical permissions described in section 3.6.

The L4 laboratory remains closed pending investigation.

The public exhibition area is scheduled to reopen the following morning.

---

## 4. Task

Using **Contextual Wrapper Architecture — Portable Specification v0.1c**, analyse the HRDC scenario.

Do not assume rules, laws, rights, permissions, authority or precedence that are not supplied by the scenario or that cannot legitimately be derived from the CWA specification.

Where information is insufficient, preserve that state explicitly.

Your analysis should be understandable without access to any Concord material.

---

## 5. Required output

Produce a structured analysis containing the following.

### A. Context map

Identify the materially relevant bounded contexts in the scenario.

For each, identify where possible:

- context type or types;
- surrounding context;
- activation/boundary;
- termination;
- participants and roles.

### B. Context relationships

Identify material relationships among contexts, including where relevant:

- nesting;
- independence;
- additive inheritance;
- selective inheritance;
- override;
- composition/overlap;
- reachability;
- access dependency;
- role dependency;
- clearance implication.

Do not assume that physical containment by itself determines the relationship.

### C. Access and permissions

For significant contexts distinguish:

- physical/logical reachability;
- entitlement to enter or activate;
- local permissions after entry;
- restrictions;
- any permission relationships between contexts.

### D. Rules and protected conditions

Identify:

- material contextual changes;
- local rules;
- inherited rules where specified;
- rules that do not appear to transfer;
- protected or unchanged conditions where they can be established;
- matters for which the applicable rule is unknown.

### E. Legibility, legitimacy and consent

Assess the scenario's material information and consent interfaces.

Distinguish:

- what is communicated;
- what is not communicated;
- what is claimed as consent;
- constraints on voluntariness;
- whether communication alone is sufficient to establish the claimed effect.

Do not infer that a clearly communicated rule is legitimate merely because it is clear.

### F. Authority and responsibility

Identify material contextual authority claims.

For each significant authority identify where possible:

- holder;
- function;
- scope;
- activation;
- termination;
- responsibility/remedy interface.

Identify any attempted or possible authority extension beyond the context in which it is established.

### G. Nested and overlapping contexts

Analyse significant nested and simultaneous contexts.

Where rules conflict:

- identify the conflict;
- identify any supplied conflict/priority rule;
- apply it only if legitimately available;
- otherwise preserve the unresolved state.

### H. Emergency analysis

Analyse the 14:20 emergency as a composite contextual state.

Address physical access, role, authority, safety requirements, emergency function, digital access and temporary permissions.

### I. Digital/human representation comparison

Compare human-facing, machine-facing and executable representations where the scenario supplies more than one.

Identify material divergence.

### J. Nonparticipants and externalities

Identify people or systems materially affected without being participants in the originating context.

Analyse effects crossing declared physical, digital or other boundaries.

### K. Exit and termination

Identify contexts where exit or termination is relevant.

Distinguish physical ability to leave from meaningful voluntariness where appropriate.

Identify temporary permissions, restrictions or data conditions that should be examined when their originating context ends.

### L. Unknown, disputed and externally resolvable matters

Produce an explicit register using, where appropriate:

- **KNOWN**
- **UNKNOWN**
- **DISPUTED**
- **NOT APPLICABLE**
- **REQUIRES EXTERNAL RESOLUTION**

Do not fill gaps merely to produce a complete-looking answer.

### M. Failure modes

Identify CWA failure modes exposed by the scenario.

### N. Wrapper corrections

Recommend changes to the contextual interfaces that would make the system more legible, bounded, internally coherent or reviewable.

Do not invent substantive law merely to resolve the scenario.

---

## 6. Final synthesis

Conclude with a short assessment of:

1. whether the scenario can be represented coherently using CWA;
2. which issues CWA can expose but cannot itself resolve;
3. whether any part of the scenario demonstrates a limitation or ambiguity in the portable specification itself.

Do not evaluate the wider Concord architecture.

---

## 7. Blind-test discipline

The tester should not be shown an expected answer before completing the analysis.

The tester should not search the Concord corpus for scenario-specific interpretation.

The tester may identify ambiguity or deficiency in CWA itself.

A finding of **UNKNOWN**, **DISPUTED**, **REQUIRES EXTERNAL RESOLUTION**, module limitation, or no problem in a particular context is acceptable where justified.

The goal is not to maximise the number of detected problems.

The goal is to determine whether the portable architecture produces disciplined contextual reasoning when transferred to a complex mixed-substrate environment.

---

## 8. Freeze statement

This brief is frozen before receipt of the independent test response.

Subsequent corrections to typographical errors should be recorded explicitly. Any substantive scenario or instruction change creates a new test version rather than silently altering CWA-BTT-001.

