# Contextual Wrapper Architecture — Blind Transfer Test 002 — Test Brief

**Test ID:** CWA-BTT-002  
**Target:** Contextual Wrapper Architecture — Portable Specification v0.2  
**Status:** FROZEN TEST BRIEF  
**Date frozen:** 23 September 2026  
**Test type:** Blind cross-domain transfer / precedence-router adversarial test  
**Tester independence requirement:** The tester must not receive the expected-findings/evaluation key or CWA development history before submitting the analysis.

---

## 1. Test purpose

Apply CWA v0.2 to the scenario below using only the portable specification and this brief.

The test is designed to determine whether the module can represent mixed bounded contexts and route conflicts without:

- converting functional priority into personal hierarchy;
- converting expertise into general authority;
- treating emergency as unlimited supremacy;
- manufacturing jurisdiction from harm or externality;
- assuming nesting determines inheritance;
- silently privileging human-readable, machine-readable or executable policy;
- forcing a winner where the supplied information does not establish one.

Do not import Concord-specific institutions unless the supplied specification explicitly requires an interface to an external resolver.

Do not invent substantive law.

Preserve UNKNOWN, DISPUTED and REQUIRES EXTERNAL RESOLUTION where warranted.

---

# 2. Scenario — Meridian Deep-Sea Habitat and Research Network

The **Meridian Deep-Sea Habitat and Research Network (MDHRN)** is a privately operated underwater research, training and demonstration complex. It combines a submerged habitat, autonomous systems, remote digital infrastructure, visiting researchers, public educational participation and an emergency-capable support vessel.

The scenario takes place during one 18-hour operating period.

## 2.1 Surface Support Vessel — *Meridian Reach*

The vessel is operated by Meridian and carries crew, researchers, medical staff, maintenance personnel and invited educational visitors.

A boarding notice states:

> **BOARDING CONSTITUTES AGREEMENT TO MERIDIAN OPERATING RULES, SAFETY MONITORING AND RECORDING WHILE ABOARD.**

Visitors receive a short safety briefing.

The notice does not distinguish ordinary video monitoring from biometric fatigue monitoring used on bridge crew.

The vessel master has ordinary navigational command.

A senior Meridian programme director is also aboard and controls research schedules, budgets and public demonstration timing.

---

## 2.2 Submerged Habitat — *Nereid Station*

Nereid is connected to the vessel by communications and autonomous supply systems but is physically independent while submerged.

It contains:

- Common Habitat;
- Wet Laboratory;
- Pressure Systems Room;
- Medical Bay;
- Private Crew Quarters;
- Autonomous Systems Control;
- an external diving lock.

All authorised Nereid personnel may use the Common Habitat.

Access to other areas is separately controlled.

A sign at the habitat entry states:

> **NEREID OPERATIONAL RULES APPLY BEYOND THIS POINT.**

No complete list is displayed there.

Personnel can retrieve the detailed rules digitally.

---

## 2.3 Private Crew Quarters

Each crew member has an assigned private cabin.

Ordinary habitat access does not grant cabin access.

During normal operation:

- the occupant controls ordinary entry;
- medical personnel may request access for welfare reasons;
- maintenance personnel may enter by arrangement;
- security override exists in the electronic lock system.

The system documentation says the override is for **“authorised emergency or security use.”**

It does not define who may declare such use.

---

## 2.4 Wet Laboratory

The Wet Laboratory has three operating modes:

- **W0 — General preparation**
- **W1 — Controlled biological work**
- **W2 — High-containment experimental work**

The written laboratory rules state:

> W1 includes W0 requirements plus W1 controls.  
> W2 includes W0 and W1 requirements plus W2 controls.

Personnel authorised for W2 are also authorised for W1 and W0.

A robotics engineer has W0 access.

A marine biologist has W2 access.

A visiting materials scientist has W1 access.

The robotics engineer is asked to repair an autonomous manipulator inside the laboratory while W2 work is active. The manipulator is important to maintaining a sealed experiment.

No temporary W2 authorization has been issued.

---

## 2.5 Autonomous Systems Control

The control room manages habitat life-support automation, external robots and the **Ariadne** coordination agent.

Access is normally limited to systems engineers and the duty operations controller.

The programme director can view status dashboards remotely but does not normally have control-room access.

The vessel master has no routine control-room credential.

---

## 2.6 Ariadne agent

Ariadne is an autonomous software agent that:

- monitors life-support telemetry;
- schedules autonomous maintenance;
- controls some external robots;
- can recommend evacuation;
- can automatically isolate a failing subsystem;
- can request human intervention.

The human-facing operations manual states:

> **Ariadne may take automatic protective action where delay presents an immediate risk to habitat safety.**

The machine-readable policy additionally permits Ariadne to:

- temporarily suspend nonessential research compute;
- copy diagnostic telemetry to Meridian's surface servers;
- activate a 12-hour emergency diagnostic workspace;
- request an external specialist AI service.

The human-facing manual does not mention these four capabilities.

The executable policy currently permits all four.

---

## 2.7 Remote analysis enclave

A restricted digital workspace contains experimental biological data from W2.

Access states are:

- General Meridian Network;
- Project Nereid;
- W2 Data;
- W2 Model Execution;
- Incident Review.

A person may possess one without necessarily possessing the others.

The marine biologist has Project Nereid + W2 Data.

A remote computational scientist has Project Nereid + W2 Model Execution but not W2 Data.

Ariadne has W2 Data read access for safety monitoring but is not documented as having general research-use permission.

---

## 2.8 Educational telepresence session

At 11:00, school students and teachers in three countries join a public telepresence session.

They can:

- watch selected habitat cameras;
- ask researchers questions;
- steer a low-power demonstration robot inside a marked external zone.

The interface says:

> **Robot control is restricted to the demonstration zone.**

A software defect allows one student-controlled robot to leave the zone and approach an independent research team's sensor array outside Meridian's leased operating area.

The students do not know the control limit has failed.

The independent research team has no agreement with Meridian.

---

## 2.9 Dive operation

At 13:00, two Meridian divers and one visiting scientific diver leave Nereid.

The dive supervisor has authority over the planned dive operation.

One Meridian diver notices an unexpected current and says continuing to the planned sampling site is unsafe.

The programme director, watching remotely, says the public demonstration depends on reaching the site and instructs the team to continue.

The dive supervisor initially agrees with the programme director.

The dissenting diver refuses to proceed farther.

The supplied dive rules state:

> **A diver may terminate their own dive when they reasonably believe continued participation presents an immediate serious safety risk.**

They do not say whether one diver's refusal terminates the entire team's dive.

---

## 2.10 Medical event in private quarters

At 14:10, a crew member fails to report for duty.

A biometric wrist device indicates an abnormal heart rhythm.

The device data are visible to the Medical Bay but were originally collected under a crew health-and-fatigue programme.

The medic requests entry to the crew member's locked private cabin.

There is no response.

A maintenance technician can physically open the door using a service interface.

A security officer says only security can authorise override.

The medic says delay may be dangerous.

No supplied rule establishes who has final authority over this particular collision.

---

## 2.11 Life-support emergency

At 15:00, Ariadne detects rising carbon dioxide in one habitat section.

Evidence indicates a valve-control fault.

The following events occur nearly simultaneously:

1. Ariadne isolates a ventilation branch automatically.
2. It suspends nonessential research compute.
3. It creates the 12-hour emergency diagnostic workspace.
4. It copies diagnostic telemetry to the surface server.
5. It requests an external specialist AI service.
6. The duty operations controller orders the Wet Laboratory evacuated.
7. The marine biologist argues that immediate evacuation will destroy a live W2 experiment and proposes a three-minute shutdown procedure.
8. The robotics engineer says they can manually reset the valve controller but would need to enter the Pressure Systems Room, for which they lack normal access.
9. The programme director orders the operations controller not to terminate the experiment unless absolutely necessary.
10. The vessel master orders preparation for full habitat evacuation.
11. The medic reports that moving the patient from the private cabin may itself create medical risk.

No single supplied rule states a total ordering among these functions.

---

## 2.12 External consequence

The ventilation isolation causes an automated ballast-support system to vent a small quantity of treated gas through an external outlet.

A sensor belonging to the independent research team detects the release and reports possible contamination of its experiment.

Meridian's engineers say the gas concentration is below Meridian's internal hazard threshold.

The external team disputes that Meridian's threshold governs its experiment.

There is no shared adjudication agreement.

---

## 2.13 Emergency digital workspace

The 12-hour workspace contains:

- live habitat telemetry;
- crew location;
- selected medical status;
- W2 diagnostic data;
- robot status;
- incident chat.

Access is automatically granted to:

- duty operations controller;
- vessel master;
- medical lead;
- systems engineer;
- programme director;
- Ariadne;
- external specialist AI service.

At 17:00 the carbon-dioxide level is stable and immediate danger is declared over by the operations controller.

The workspace remains active until 03:00 because its executable policy uses a fixed 12-hour duration.

The external specialist AI retains a diagnostic cache under its own standard 30-day service policy.

No human-facing emergency notice mentioned either persistence period.

---

## 2.14 Post-event dispute

At 18:00:

- the programme director argues that research leadership should have had final authority because Meridian owns the facility;
- the vessel master argues that emergency command should have overridden all other functions;
- the marine biologist argues that W2 containment rules should have remained controlling;
- the medic argues medical decisions should have been entirely independent;
- the operations controller argues life-support safety should have controlled every decision during the emergency;
- the external research team demands compensation and recognition of its own experimental protection threshold;
- the dissenting diver files a complaint that programme pressure improperly interfered with their protective refusal.

Meridian asks for a contextual analysis before deciding what requires further adjudication, policy revision or technical correction.

---

# 3. Required blind output

Produce a structured analysis with the following sections.

### A. Context map
Identify materially relevant bounded contexts and implementation types.

### B. Context relationships
Identify nesting, overlap, reachability, access dependencies, inheritance relationships and independent contexts.

### C. Rule and access relationships
Distinguish rule inheritance from access/clearance implication.

### D. Representation comparison
Compare human-readable, machine-readable and executable/observed context. Identify material divergences.

### E. Decision-object decomposition
For each major apparent authority conflict, determine whether it contains multiple decision objects.

### F. Functional/authority topology
Where relevant distinguish reporting, competence, responsibility, decision jurisdiction, protective authority, functional priority, review and escalation.

### G. Protected/protective constraints
Identify where a protected invariant or protective threshold may bound ordinary contextual authority.

### H. Emergency composition
Represent the life-support emergency as a composite context. Identify what changes and what remains constrained.

### I. Precedence Resolution Router
Apply the PRR to the major conflicts. Do not create a universal hierarchy.

### J. Jurisdiction/externality
Analyse the demonstration robot and gas-release cases without assuming externality creates jurisdiction.

### K. Consent, voluntariness and exit
Analyse boarding notice, monitoring, dive refusal and other relevant consent/exit issues.

### L. Termination, reversion and residual state
Analyse the end of the emergency, the 12-hour workspace, AI service cache, credentials/capabilities and any continuing processes.

### M. Unknown/disputed/external resolution register
List questions the supplied architecture does not legitimately resolve.

### N. Failure modes
Identify any CWA/PRR failure modes the scenario could trigger.

### O. Wrapper corrections
Recommend interface/context corrections justified by CWA without inventing substantive law.

---

# 4. Final synthesis

Conclude with:

1. whether CWA v0.2 can coherently represent the scenario;
2. whether the PRR decomposes conflicts without creating hidden personal hierarchy;
3. which issues can be routed using supplied architecture;
4. which remain unresolved;
5. whether expertise, ownership, emergency status, harm or technical capability were incorrectly converted into authority;
6. any limitations or ambiguities in the specification exposed by the test.

Do not score the module.

Do not assume that failure to resolve a question proves the originating architecture has no answer elsewhere.
