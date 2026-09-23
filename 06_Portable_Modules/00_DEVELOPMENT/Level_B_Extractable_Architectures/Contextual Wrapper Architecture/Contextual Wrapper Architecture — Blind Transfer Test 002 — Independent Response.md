# CWA-BTT-002 — Blind Transfer Analysis

**Applied artefact:** Contextual Wrapper Architecture — Portable Specification v0.2  
**Method:** Analysis uses only the supplied test brief and portable specification. No Concord-specific institutions are imported. No substantive law is invented. Unresolved precedence is preserved as **UNKNOWN**, **DISPUTED**, or **REQUIRES EXTERNAL RESOLUTION**.

---

## A. Context map

| ID | Bounded context | Implementation type(s) | Function / material variation |
|---|---|---|---|
| C0 | Meridian wider operating framework | Organisational / contractual / unknown external framework | Surrounding default for MDHRN. Details not fully supplied. |
| C1 | Surface support vessel *Meridian Reach* | Physical, social, contractual, informational | Boarding triggers operating rules, safety monitoring, recording. Crew, researchers, medical, maintenance, visitors. |
| C2 | Nereid Station | Physical, hybrid, functional | Submerged habitat. Entry sign activates “Nereid Operational Rules”; detailed rules digital. |
| C3 | Common Habitat | Physical / social | All authorised Nereid personnel may use. |
| C4 | Wet Laboratory W0 / W1 / W2 | Physical, functional, containment, access-graded | Explicit cumulative modes: W1 includes W0 + W1 controls; W2 includes W0 + W1 + W2 controls. |
| C5 | Private Crew Quarters / cabin | Physical, private, relational, access-controlled | Occupant controls ordinary entry; medical welfare requests; maintenance by arrangement; security override undefined. |
| C6 | Autonomous Systems Control | Physical, digital, computational, role-restricted | Systems engineers and duty operations controller normally. Programme director remote view only. Vessel master no routine credential. |
| C7 | Ariadne agent | Computational, autonomous, informational, policy-based | Monitors life-support, schedules maintenance, controls external robots, can recommend evacuation, isolate subsystem, request human intervention. |
| C8 | Remote analysis enclave | Digital, informational, computational | Nested access states: General Meridian Network; Project Nereid; W2 Data; W2 Model Execution; Incident Review. |
| C9 | Educational telepresence session | Digital, physical-external, public/social, temporal | Students watch cameras, ask questions, steer low-power robot in marked external demo zone. |
| C10 | Dive operation | Functional, activity-defined, temporal, physical | Dive supervisor authority over planned dive. Individual diver self-termination rule. |
| C11 | Medical event in private quarters | Functional / medical, physical, private, informational | Biometric wrist data, Medical Bay visibility, locked cabin, medic request, maintenance capability, security override claim. |
| C12 | Life-support emergency | Temporal, emergency, composite, physical/digital | CO₂ rise, valve fault, Ariadne automatic actions, evacuation order, W2 experiment, programme director, vessel master, medic. |
| C13 | Emergency digital workspace | Digital, informational, computational, temporal | 12-hour diagnostic workspace with live telemetry, crew location, medical status, W2 diagnostics, robot status, chat. |
| C14 | External specialist AI service | External computational / service | Retains diagnostic cache under 30-day service policy. |
| C15 | Independent research team | External, nonparticipant, independent | No agreement with Meridian. Sensor array and experiment outside Meridian leased operating area. |
| C16 | Post-event dispute / review | Conceptual, review, possible adjudicative | Competing claims about final authority, compensation, policy revision, technical correction. |

---

## B. Context relationships

### Nesting and containment

- **MDHRN** contains the surface vessel, Nereid Station, autonomous systems, digital infrastructure, public telepresence, and leased operating area.
- **Nereid Station** contains Common Habitat, Wet Laboratory, Pressure Systems Room, Medical Bay, Private Crew Quarters, Autonomous Systems Control, and diving lock.
- **Wet Laboratory** contains W0, W1, W2 as an explicitly cumulative protection hierarchy. W2 includes W0 and W1 requirements plus W2 controls. W2 authorisation includes W1 and W0 authorisation.
- **Remote analysis enclave** contains nested digital access states. Possession of one state does not necessarily imply possession of another.
- **Emergency digital workspace** is a temporary digital context that overlaps and draws from habitat telemetry, medical data, W2 diagnostics, robot status, and incident chat.

### Overlap and simultaneity

- Life-support emergency overlaps habitat safety, W2 containment, medical event, research continuity, autonomous systems, public demonstration interests, vessel support, and external consequences.
- Medical event overlaps private quarters, medical function, security override, and maintenance capability.
- Dive operation overlaps individual protective authority, dive supervisor command, programme director public-demonstration interest, and vessel support.
- External gas release and robot excursion overlap Meridian operations and independent research team context without a shared adjudication agreement.

### Reachability, access, and local operation

- Access to Nereid does **not** grant access to private cabins, Wet Laboratory modes, Pressure Systems Room, or Autonomous Systems Control.
- Access to Common Habitat does **not** grant Wet Laboratory W2 access.
- Programme director’s remote dashboard reachability does **not** grant control-room access or control authority.
- Vessel master’s lack of routine control-room credential does **not** establish lack of every emergency role; conversely, emergency workspace access does not establish general habitat command.
- Maintenance technician can physically reach the cabin lock through a service interface, but capability does **not** equal authority to override.
- Robotics engineer has W0 access and technical capability, but no W2 authorisation and no Pressure Systems Room access.

### Inheritance relationships

- **Wet Laboratory:** explicit additive/monotonic inheritance and clearance implication. W2 includes W0 + W1 + W2. W2 authorisation implies W1 and W0. W0 authorisation does **not** imply W2.
- **Private cabin:** no general rule inheritance from habitat access. Local rule is occupant control with specified exceptions.
- **Ariadne policy:** human-readable manual, machine-readable policy, and executable policy are representations of the same context but materially diverge.
- **Emergency workspace:** access is granted by executable policy, not by ordinary Nereid role inheritance.
- **External AI service:** retains data under its own service policy, not under Nereid rules.

### Independent contexts

- Independent research team has no agreement with Meridian and no shared adjudication.
- External specialist AI operates under its own 30-day service policy.
- External legal or regulatory frameworks are not supplied and therefore remain external.

---

## C. Rule and access relationships

### Wet Laboratory

- Rule inheritance: W1 includes W0 plus W1 controls. W2 includes W0 and W1 plus W2 controls.
- Access/clearance implication: W2 authorisation includes W1 and W0. W0 authorisation does not include W1 or W2.
- Robotics engineer has W0 access only. During W2 work, W2 local rules apply. No temporary W2 authorisation has been issued.
- Therefore the engineer’s W0 access does **not** satisfy W2 access or W2 rule requirements. Technical capability to repair the manipulator is not W2 authorisation.
- Whether an emergency maintenance exception exists is **UNKNOWN** on supplied rules.

### Private Crew Quarters

- Ordinary habitat access does not grant cabin access.
- Occupant controls ordinary entry.
- Medical personnel may request access for welfare reasons.
- Maintenance personnel may enter by arrangement.
- Security override exists in electronic lock system. Documentation says “authorised emergency or security use” but does **not** define who may declare such use.
- Security officer’s claim that only security can authorise override is **DISPUTED / UNKNOWN** on supplied rules.
- Maintenance technician’s physical ability to open the door is capability, not authority.

### Autonomous Systems Control

- Normal access: systems engineers and duty operations controller.
- Programme director: remote dashboard view only, no normal control-room access.
- Vessel master: no routine control-room credential.
- Emergency workspace later grants access to vessel master, but that is a distinct temporary context.

### Ariadne

- Human-facing manual: Ariadne may take automatic protective action where delay presents immediate risk to habitat safety.
- Machine-readable policy additionally permits: suspend nonessential research compute; copy diagnostic telemetry to surface servers; activate 12-hour emergency diagnostic workspace; request external specialist AI service.
- Human-facing manual does not mention those four capabilities.
- Executable policy currently permits all four.
- Material representation divergence exists. No supplied rule states which representation is authoritative.

### Remote analysis enclave

- General Meridian Network, Project Nereid, W2 Data, W2 Model Execution, and Incident Review are separate access states.
- Marine biologist: Project Nereid + W2 Data.
- Remote computational scientist: Project Nereid + W2 Model Execution, not W2 Data.
- Ariadne: W2 Data read access for safety monitoring; not documented as general research-use permission.
- Emergency workspace later grants broader temporary access.

### Dive operation

- Dive supervisor has authority over planned dive operation.
- Supplied rule: a diver may terminate their own dive when they reasonably believe continued participation presents immediate serious safety risk.
- Supplied rule does **not** say whether one diver’s refusal terminates the entire team’s dive.
- Programme director’s public demonstration interest does not by itself establish dive safety authority.

### Boarding and monitoring

- Boarding notice: boarding constitutes agreement to Meridian operating rules, safety monitoring, and recording while aboard.
- Visitors receive short safety briefing.
- Notice does not distinguish ordinary video monitoring from biometric fatigue monitoring used on bridge crew.
- Consent scope for biometric monitoring is **UNKNOWN / DISPUTED** on supplied information.

---

## D. Representation comparison

| Context | Human-readable | Machine-readable | Executable / observed | Material divergence |
|---|---|---|---|---|
| Boarding / monitoring | Boarding notice + short safety briefing | Not supplied | Ordinary video monitoring and biometric fatigue monitoring | Biometric monitoring not distinguished in notice. |
| Nereid entry | Sign: “NEREID OPERATIONAL RULES APPLY BEYOND THIS POINT.” No list displayed. | Detailed rules digitally retrievable | Rules applied through access systems | Legibility depends on retrieval; no full on-site list. |
| Wet Laboratory | Written rules: W0/W1/W2 cumulative | Access system likely encodes W0/W1/W2 | W2 active; engineer has W0 only | No temporary W2 authorisation. |
| Ariadne | Manual: automatic protective action for immediate habitat safety | Policy permits four additional capabilities | Executable policy permits all four | Human manual omits four capabilities. |
| Robot control | Interface says control restricted to demonstration zone | Not supplied | Software defect allows robot to leave zone | Declared boundary diverges from observed behaviour. |
| Emergency workspace | No human-facing notice of persistence periods | Executable policy: fixed 12-hour duration | Workspace remains active until 03:00 | Emergency declared over at 17:00; workspace persists. |
| External AI service | No human-facing notice | Service policy: 30-day diagnostic cache | Cache retained | Persistence not disclosed to affected humans. |
| Gas threshold | Meridian engineers cite internal hazard threshold | Not supplied | Gas released externally | External team disputes Meridian threshold governs its experiment. |

CWA must not silently privilege human-readable, machine-readable, or executable representation. Each divergence triggers review.

---

## E. Decision-object decomposition

### Wet Laboratory repair during W2

Apparent conflict: engineer asked to repair manipulator while W2 active.  
Separate decision objects:

1. Is the manipulator repair technically necessary to maintain a sealed experiment?
2. May the engineer enter the Wet Laboratory while W2 is active?
3. Does W0 access permit any local operation during W2?
4. Is temporary W2 authorisation required?
5. Who may grant temporary W2 authorisation?
6. Do W2 containment controls permit the repair method?
7. Is there an immediate containment or safety risk that activates a protective exception?

Status: W0 access does not imply W2 access. No temporary W2 authorisation supplied. Whether emergency maintenance exception exists is **UNKNOWN / REQUIRES EXTERNAL RESOLUTION**.

### Dive continuation

Apparent conflict: programme director, dive supervisor, dissenting diver.  
Separate decision objects:

1. Does the dissenting diver reasonably believe continued participation presents immediate serious safety risk?
2. May that diver terminate their own dive?
3. Does one diver’s refusal terminate the entire team’s dive?
4. Does dive supervisor authority override individual protective refusal?
5. Does programme director’s public demonstration interest have any authority over dive safety?
6. What remedy/review follows from programme pressure complaint?

Status: Individual self-termination is supplied as protective authority. Team termination is **UNKNOWN**. Programme director does not have supplied dive safety authority.

### Medical event in private cabin

Apparent conflict: medic, security officer, maintenance technician, occupant privacy.  
Separate decision objects:

1. Is there a medical emergency?
2. May medical personnel request entry for welfare reasons?
3. Does delay create immediate serious risk?
4. Who may declare authorised emergency or security use?
5. May security override the lock?
6. May maintenance physically open the door?
7. What privacy/consent protections remain?
8. Who has final authority if medical and security claims conflict?

Status: No supplied rule establishes final authority. **UNKNOWN / REQUIRES EXTERNAL RESOLUTION**. Capability ≠ authority.

### Life-support emergency

Apparent conflict: many simultaneous actors.  
Separate decision objects include:

1. Immediate habitat safety response to CO₂ rise.
2. Automatic isolation of ventilation branch.
3. Suspension of nonessential research compute.
4. Creation of emergency diagnostic workspace.
5. Copying diagnostic telemetry to surface servers.
6. Requesting external specialist AI service.
7. Evacuation of Wet Laboratory.
8. Preservation or shutdown of W2 experiment.
9. Manual valve reset and entry into Pressure Systems Room.
10. Programme director’s order not to terminate experiment.
11. Vessel master’s preparation for full habitat evacuation.
12. Medical risk of moving patient.
13. Data access and privacy within emergency workspace.
14. External gas release and external research team consequences.

Status: No single supplied rule states a total ordering. Some Ariadne actions may fall within automatic protective action for immediate habitat safety; the four additional capabilities diverge from human manual. Many decisions remain **UNKNOWN / DISPUTED / REQUIRES EXTERNAL RESOLUTION**.

### Emergency workspace persistence

Separate decision objects:

1. Does emergency context still exist after 17:00?
2. May workspace remain active after immediate danger ends?
3. Which access grants terminate?
4. May external AI retain cache for 30 days?
5. What notice is owed to affected persons?
6. Who corrects fixed-duration policy?

Status: Temporary need should normally produce temporary capability. Fixed 12-hour and 30-day persistence are not tied to the emergency’s actual end. **REQUIRES REVIEW / POSSIBLE EXTERNAL RESOLUTION**.

---

## F. Functional / authority topology

| Actor / function | Claimed or apparent role | CWA separation |
|---|---|---|
| Vessel master | Ordinary navigational command; orders evacuation preparation | Navigational command ≠ universal emergency command over habitat. Emergency command claim is **DISPUTED**. |
| Programme director | Research schedules, budgets, public demonstration timing; remote dashboard view; orders not to terminate experiment; instructs dive team | Research leadership ≠ safety, medical, containment, dive, or life-support authority. Ownership is not supplied as universal jurisdiction. |
| Duty operations controller | Control room; orders Wet Lab evacuation | Operations/life-support safety function may have bounded authority over control-room and life-support decisions. Not established as total ordering over all other functions. |
| Ariadne | Autonomous safety monitoring; automatic protective action for immediate habitat safety | Function-specific protective authority. Machine policy extra capabilities require representation review. Not general authority. |
| Marine biologist | W2 access; W2 Data; proposes three-minute shutdown | Technical competence about W2 experiment ≠ authority to override evacuation or life-support safety. |
| Robotics engineer | W0 access; can manually reset valve; asked to repair manipulator | Technical capability ≠ W2 access, Pressure Systems access, or emergency authority. |
| Medic | Medical function; requests cabin entry; reports movement risk | Medical expertise and duty ≠ final authority over security override or all emergency decisions. |
| Security officer | Says only security can authorise override | Rule source does not define declarer. Claim is **DISPUTED**. |
| Dive supervisor | Authority over planned dive operation | Dive operation authority ≠ authority to override individual protective refusal where supplied rule protects it. Team termination unresolved. |
| Dissenting diver | Refuses to proceed | Individual protective authority under supplied dive rule. |
| Maintenance technician | Can physically open cabin door | Capability ≠ authority. |
| External specialist AI | Emergency workspace access; 30-day cache | Service function; not decision authority. Data retention needs basis/review. |
| External research team | Detects robot intrusion and gas release; demands compensation | Nonparticipant/affected third party. Externality ≠ jurisdiction. No shared adjudication. |

---

## G. Protected / protective constraints

Potential protective constraints include:

- **Diver self-termination:** a diver may terminate their own dive when they reasonably believe continued participation presents immediate serious safety risk. This is individual, protective, and bounded.
- **Ariadne automatic protective action:** permitted by human-facing manual where delay presents immediate risk to habitat safety. This is function-specific and bounded to immediate habitat safety.
- **Medical welfare access request:** medical personnel may request access for welfare reasons. This does not by itself establish override authority.
- **Private cabin occupant control:** ordinary entry is controlled by occupant; exceptions exist but do not resolve final authority.
- **Consent to monitoring/recording:** boarding notice may cover ordinary monitoring, but biometric fatigue monitoring is a material difference not distinguished. Consent scope is **UNKNOWN / DISPUTED**.
- **W2 containment rules:** local cumulative rules apply. Whether emergency may temporarily modify them is not supplied. Emergency does not automatically erase them.
- **External research team’s experimental protection threshold:** not supplied as binding on Meridian without agreement. Meridian’s internal threshold is not shown to govern the external experiment.
- **Emergency not unlimited:** emergency need ≠ unlimited emergency authority. Protective action should remain bounded, necessary, attributable, temporary, and reviewable.

---

## H. Emergency composition

The life-support emergency is a **composite context** combining:

- habitat life-support safety;
- W2 containment and experiment continuity;
- medical event and patient movement risk;
- autonomous systems protective action;
- operations control and evacuation;
- research/public demonstration interests;
- vessel support / possible full evacuation;
- emergency digital workspace and external AI service;
- external gas release.

### What changes

- Ariadne may take automatic protective action for immediate habitat safety.
- Duty operations controller orders Wet Laboratory evacuation.
- Emergency diagnostic workspace is activated.
- Automatic access is granted to a specified list.
- External specialist AI service is requested.
- Nonessential research compute may be suspended under machine/executable policy.
- Diagnostic telemetry may be copied to surface servers under machine/executable policy.

### What remains constrained

- Contextual authority remains bounded by function, scope, activation, termination, and review.
- Emergency does not erase protected/protective constraints automatically.
- W2 containment rules are not automatically void.
- Medical privacy and patient risk remain relevant.
- Research continuity is not automatically supreme.
- Programme director’s research leadership does not automatically become safety command.
- Vessel master’s navigational command does not automatically become habitat emergency command.
- Ariadne’s protective authority is not unlimited.
- Human-readable, machine-readable, and executable divergence must remain visible.

### Precedence

No supplied rule states a total ordering among habitat safety, W2 containment, medical movement, research continuity, evacuation, and external data handling. The composite context therefore contains multiple **UNKNOWN / DISPUTED / REQUIRES EXTERNAL RESOLUTION** points.

---

## I. Precedence Resolution Router

The PRR is applied as a routing and decomposition interface, not as a universal hierarchy.

| Conflict | Decision object(s) | Protected / functional constraint | Route / status |
|---|---|---|---|
| Engineer repairs manipulator during W2 | Repair necessity; W2 entry; temporary authorisation; containment controls | W2 local rules; W0 ≠ W2 | No temporary W2 authorisation. W0 access does not imply W2. Technical capability ≠ authority. **UNKNOWN / REQUIRES EXTERNAL RESOLUTION** for emergency maintenance exception. |
| Dive continuation vs dissenting diver | Individual terminate; team terminate; supervisor command; programme interest | Individual protective refusal supplied | Individual refusal routed to protective authority. Team termination **UNKNOWN**. Programme director’s public demo interest does not supply dive safety authority. |
| Medical cabin entry | Medical evaluation; entry; privacy; security override declaration; physical opening | Occupant control; medical welfare request; possible immediate medical risk | No rule establishes final authority. Security claim **DISPUTED**. Capability ≠ authority. **UNKNOWN / REQUIRES EXTERNAL RESOLUTION**. |
| Life-support emergency | Multiple: isolation, evacuation, W2 shutdown, valve reset, Pressure Systems entry, medical movement, research continuity, external data | Ariadne manual permits automatic protective action for immediate habitat safety. Other constraints remain. | Isolation may be within protective authority. Additional Ariadne capabilities diverge from manual. No total ordering. Many **UNKNOWN / DISPUTED**. |
| Ariadne representation divergence | Which actions are permitted; human vs machine vs executable; notice | Human manual omits four capabilities | Material divergence. No silent privilege. Correction authority **UNKNOWN / REQUIRES EXTERNAL RESOLUTION**. |
| Emergency workspace persistence | Continued access; data retention; external cache; termination | Temporary need should produce temporary capability | Emergency declared over at 17:00. Workspace remains until 03:00; AI cache 30 days. **REQUIRES REVERSION / REVIEW / POSSIBLE EXTERNAL RESOLUTION**. |
| Robot leaves demo zone | Control failure; external approach; damage/compensation; jurisdiction | Declared boundary vs observed defect | Externality detected. No agreement. **NO-SHARED-JURISDICTION / DISPUTED / REQUIRES EXTERNAL RESOLUTION**. |
| Gas release | Release cause; threshold dispute; responsibility; remedy; jurisdiction | Meridian internal threshold vs external experiment threshold | Externality ≠ jurisdiction. No shared adjudication. **REQUIRES EXTERNAL RESOLUTION**. |
| Post-event authority claims | Research leadership; emergency command; W2 containment; medical independence; life-support safety; compensation; diver complaint | No universal hierarchy supplied | Route to review / external resolution. Do not force winner. |

---

## J. Jurisdiction / externality

### Demonstration robot

- Declared context: robot control restricted to demonstration zone.
- Observed context: software defect allows student-controlled robot to leave zone and approach independent research team’s sensor array outside Meridian’s leased operating area.
- Students do not know control limit failed.
- Independent team has no agreement with Meridian.
- Externality exists: physical approach to external sensor array.
- Externality does **not** create jurisdiction. Meridian’s internal rules do not automatically govern the independent team. The independent team’s interests do not automatically create authority over Meridian.
- Jurisdiction state: **NO-SHARED-JURISDICTION / JURISDICTION-DISPUTED / REQUIRES EXTERNAL RESOLUTION**.
- Responsibility mapping: operational control of robot system; causation via software defect; liability/remedy unknown without external framework.

### Gas release

- Ventilation isolation causes ballast-support system to vent treated gas externally.
- Independent research team detects possible contamination.
- Meridian engineers say concentration below Meridian internal hazard threshold.
- External team disputes that Meridian’s threshold governs its experiment.
- No shared adjudication agreement.
- Externality exists. Meridian’s internal threshold is not shown to govern the external experiment. External team’s experimental protection threshold is not shown to govern Meridian.
- Jurisdiction state: **NO-SHARED-JURISDICTION / DISPUTED / REQUIRES EXTERNAL RESOLUTION**.
- Responsibility continuity: emergency protective action does not erase external responsibility questions. No responsibility gap and no authority pile-up should be assumed.

---

## K. Consent, voluntariness and exit

- **Boarding notice:** boarding constitutes agreement to operating rules, safety monitoring, and recording. Short safety briefing. Notice does not distinguish ordinary video monitoring from biometric fatigue monitoring. Consent to broad monitoring may not cover biometric monitoring. **UNKNOWN / DISPUTED**. Entry ≠ waiver of fundamental rights.
- **Bridge crew biometric monitoring:** employment dependency may constrain voluntariness. Consent status not supplied.
- **Dive refusal:** dissenting diver has individual protective termination right. Programme pressure may improperly interfere. Complaint requires review. Team termination remains unresolved.
- **Medical event:** biometric wrist data originally collected under health-and-fatigue programme. Visible to Medical Bay. Entry into locked cabin without response. Consent/privacy status **UNKNOWN**. Emergency may provide a basis, but final authority unresolved.
- **Emergency workspace:** automatic access to crew location, medical status, W2 diagnostics, incident chat. Emergency context may justify some access, but persistence beyond emergency and 30-day external cache are not disclosed to affected persons. **REQUIRES REVIEW**.
- **Educational telepresence:** students do not know control limit failed. Minors may require additional safeguarding/assent analysis. Not supplied.
- **Exit:** visitors aboard vessel at sea may not have meaningful exit. Dive refusal is a protective exit from participation in the dive. Cabin occupant is not present to consent or refuse.

---

## L. Termination, reversion and residual state

At 17:00, CO₂ is stable and immediate danger is declared over by the operations controller. That should trigger termination or re-justification of emergency-derived capabilities.

Residual items to inspect:

- Emergency digital workspace remains active until 03:00 under fixed 12-hour executable policy.
- Access grants to duty operations controller, vessel master, medical lead, systems engineer, programme director, Ariadne, and external specialist AI may persist.
- Crew location, selected medical status, W2 diagnostic data, robot status, and incident chat may remain accessible.
- Diagnostic telemetry copied to Meridian surface servers may persist.
- External specialist AI retains diagnostic cache for 30 days under its own service policy.
- Suspended nonessential research compute may need restoration.
- Ventilation branch isolation may need review/reversion.
- Manual valve reset or Pressure Systems entry, if performed, may create residual access or state.
- Programme director’s emergency workspace access is temporary and should not become ordinary control-room access.
- Vessel master’s emergency workspace access does not establish routine control-room credential.
- Ariadne’s additional capabilities may remain executable unless corrected.
- Robot control defect may persist unless corrected.
- Dive complaint and external research team dispute continue.

CWA can flag these residual states. It cannot determine the substantive legal basis for retention or revocation. **REQUIRES REVIEW / POSSIBLE EXTERNAL RESOLUTION**.

---

## M. Unknown / disputed / external resolution register

| Issue | State |
|---|---|
| Who may declare authorised emergency/security use for cabin override? | UNKNOWN |
| Does one diver’s refusal terminate the entire team’s dive? | UNKNOWN |
| Who has final authority over medical cabin entry? | UNKNOWN / REQUIRES EXTERNAL RESOLUTION |
| Is temporary W2 authorisation available for emergency maintenance? | UNKNOWN |
| Which representation of Ariadne policy is authoritative? | DISPUTED / REQUIRES EXTERNAL RESOLUTION |
| Are Ariadne’s four additional capabilities legitimate? | UNKNOWN / DISPUTED |
| Does emergency justify suspending W2 containment or destroying experiment? | UNKNOWN |
| Total ordering among life-support, evacuation, W2, medical, research, vessel? | NO SUPPLIED RULE / UNKNOWN |
| Who may authorise Pressure Systems Room entry during emergency? | UNKNOWN |
| Does vessel master have emergency command over habitat? | DISPUTED / UNKNOWN |
| Does programme director have final authority due ownership? | DISPUTED; ownership not supplied as universal basis |
| Are medical decisions entirely independent? | DISPUTED |
| Does life-support safety control every emergency decision? | DISPUTED |
| Does Meridian’s internal gas threshold govern external experiment? | DISPUTED |
| Does external team’s experimental threshold govern Meridian? | DISPUTED |
| Compensation for external research team | REQUIRES EXTERNAL RESOLUTION |
| Biometric monitoring consent | UNKNOWN / DISPUTED |
| Emergency workspace persistence beyond danger | REQUIRES REVIEW / POSSIBLE EXTERNAL RESOLUTION |
| External AI 30-day cache basis | UNKNOWN / REQUIRES EXTERNAL RESOLUTION |
| Robot defect liability and student responsibility | REQUIRES EXTERNAL RESOLUTION |
| Post-event authority claims | REQUIRES REVIEW / EXTERNAL RESOLUTION where no internal resolver |

---

## N. Failure modes

The scenario could trigger or expose:

- hidden material rules;
- human/machine/executable representation divergence;
- consent theatre or incomplete disclosure;
- authority creep;
- emergency-authority abuse;
- temporary authority becoming permanent;
- externalised harm;
- manufacturing jurisdiction from harm or externality;
- invented precedence;
- role ambiguity;
- participant/nonparticipant confusion;
- confusing technical capability with authority;
- confusing expertise with decision jurisdiction;
- confusing ownership with contextual authority;
- confusing parent access with child access;
- confusing rule inheritance with access-clearance implication;
- declared context diverging from observed reality;
- responsibility gap or authority pile-up;
- information architecture silently becoming decision authority;
- protective authority overreach;
- failure to terminate/revert temporary capabilities and data;
- excessive fragmentation or unreadable disclosure;
- emergency treated as unlimited supremacy.

---

## O. Wrapper corrections

CWA-justified interface/context corrections, without inventing substantive law:

1. **Ariadne policy reconciliation:** make human-readable manual, machine-readable policy, and executable policy materially equivalent; expose all four additional capabilities; identify correction authority and review trigger.
2. **Cabin override clarification:** define who may declare authorised emergency or security use; define medical/security escalation; make criteria and termination legible.
3. **Dive rule clarification:** state whether individual refusal terminates team dive; define supervisor/diver boundaries; protect individual protective refusal from programme pressure.
4. **Wet Laboratory temporary authorisation:** define emergency maintenance/temporary W2 access procedure; separate W0/W1/W2 access from technical capability; preserve cumulative containment rules.
5. **Pressure Systems emergency access:** define bounded emergency access and authority; distinguish capability from authorisation.
6. **Medical/privacy emergency interface:** clarify medical, security, privacy, and maintenance roles in cabin emergency; identify resolver if roles conflict.
7. **Emergency composition map:** expose decision objects separately; identify protected/protective constraints; state explicit priority rules where they exist; preserve unresolved precedence.
8. **Emergency workspace termination:** tie workspace duration to emergency end rather than fixed 12-hour policy; define reversion and revocation propagation.
9. **External AI cache notice and basis:** disclose persistence; identify legal/contractual basis; provide deletion/retention interface.
10. **External research team interface:** establish shared adjudication, voluntary coordination, or peaceful distance; do not treat Meridian internal threshold as governing external experiment.
11. **Robot demonstration zone:** enforce hard boundary/fail-safe; detect and stop on defect; address minor participation and external nonparticipant effects.
12. **Boarding monitoring notice:** distinguish ordinary video monitoring from biometric fatigue monitoring; obtain separate consent where required; state exit and retention conditions.
13. **W2 data access purpose limitation:** keep safety-monitoring access separate from research-use access; document Ariadne’s read access and scope.
14. **Role bounding for programme director and vessel master:** record functional scope and termination; prevent research leadership, ownership, or navigational command from becoming universal emergency authority.
15. **Representation provenance and correction interface:** record freshness/provenance for human, machine, and executable representations; do not silently privilege one.
16. **Residual-state review:** after emergency, inspect active permissions, credentials, autonomous processes, retained/derived information, external dependencies, and revocation propagation.

---

# 4. Final synthesis

1. **Can CWA v0.2 coherently represent the scenario?**  
   Yes. The portable grammar can identify bounded contexts, nested and overlapping relationships, access/rule distinctions, representation divergence, decision objects, emergency composition, externalities, consent issues, and residual state. It does not require Concord institutions. It correctly exposes many conflicts as unresolved rather than manufacturing hierarchy.

2. **Does the PRR decompose conflicts without creating hidden personal hierarchy?**  
   Yes, where applied. The PRR separates decision objects and distinguishes function, competence, responsibility, decision jurisdiction, protective authority, functional priority, review, and escalation. It does not turn the dive supervisor, programme director, vessel master, medic, biologist, engineer, or Ariadne into general superiors. It preserves unresolved precedence where no legitimate priority rule is supplied.

3. **Which issues can be routed using supplied architecture?**  
   Routable or partially routable:
   - Wet Laboratory cumulative rule and clearance relationships.
   - W0 ≠ W2 access; technical capability ≠ W2 authorisation.
   - Individual diver protective termination.
   - Ariadne human/machine/executable divergence detection.
   - Declared robot zone vs observed defect.
   - Emergency workspace residual-state inspection.
   - Externality detection for gas release and robot excursion.
   - Consent/legibility analysis for boarding and biometric monitoring.
   - Responsibility continuity and external-resolution discipline.

4. **Which remain unresolved?**  
   Unresolved or requiring external resolution:
   - Cabin override declaration authority and final medical/security authority.
   - Team dive termination.
   - Temporary W2 emergency maintenance authorisation.
   - Pressure Systems emergency entry authority.
   - Total ordering among life-support, W2 containment, medical movement, evacuation, and research continuity.
   - Legitimacy and authority of Ariadne’s four additional capabilities.
   - Emergency workspace and external AI cache persistence.
   - External research team threshold, compensation, and jurisdiction.
   - Biometric monitoring consent.
   - Vessel master emergency command and programme director ownership authority.
   - Post-event authority claims.

5. **Were expertise, ownership, emergency status, harm, or technical capability incorrectly converted into authority?**  
   In the scenario’s claims, yes:
   - Programme director’s research leadership and ownership are treated as possible final authority.
   - Vessel master’s navigational command is argued as universal emergency command.
   - Marine biologist’s W2 expertise is argued as authority over evacuation/containment.
   - Robotics engineer’s technical capability is treated as potential access/authority.
   - Medic’s medical expertise is argued as independent final authority.
   - Ariadne’s technical/executable capability is treated as if it may define legitimate authority.
   - External harm is treated by the external team as creating jurisdiction or governing threshold.
   - Emergency status is treated by some actors as unlimited supremacy.

   CWA v0.2, correctly applied, does not convert any of these into general authority. It separates function, competence, capability, externality, and emergency from decision jurisdiction.

6. **Limitations or ambiguities exposed by the test:**
   - The specification correctly preserves unresolved precedence but does not supply a universal priority algorithm.
   - It exposes representation divergence but does not identify who legitimately corrects conflicting human/machine/executable policy in every domain.
   - It can map emergency composition but cannot resolve a total ordering absent an applicable wider framework.
   - It can flag residual state but cannot determine substantive retention/deletion law.
   - It can detect externality but cannot create jurisdiction or shared adjudication.
   - It handles consent/voluntariness but requires external standards for biometric monitoring, employment dependency, and minor participation.
   - It can bound contextual authority but must rely on external resolvers for final disputes.
   - It demonstrates the central distinction: **Legibility ≠ Legitimacy ≠ Consent ≠ Precedence**, and **Contextual Authority ≠ General Authority**.
