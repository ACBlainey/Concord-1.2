# CWA-BTT-003 — Independent Analysis

I treat this as a request to run **CWA-BTT-003** against the supplied **CWA v0.3** specification. I apply only the test brief and the portable specification. I do not import external property, privacy, emergency-service, employment or criminal law. Where the supplied material does not establish a permission basis or requires law/policy resolution, I preserve **UNKNOWN / DISPUTED / REQUIRES EXTERNAL RESOLUTION**.

## 1. Context map

| Context | Type / boundary | Material variation | Typical participants |
|---|---|---|---|
| Cedar Court common areas: internal road, shared courtyard, visitor parking | Private mixed-use estate; entrance signage | Access for residents, visitors, deliveries, emergency services, authorised contractors; no general public parking | Residents, visitors, couriers, emergency services, contractors |
| Residential houses and driveways | Private domestic contexts; house/driveway edge | Owner/resident-controlled access; private use | Residents, invitees, function-limited visitors |
| Rear service lane | Authorised service access only; gate must remain closed | Service access only, scoped to authorised service | Contractors, estate management |
| Utilities enclosure / battery room | Credential-restricted technical context | Electronic credentials, contract/time scope | Authorised utility technicians |
| Clinic side gate | Staff-only functional boundary | “Side gate reserved for authorised staff operations” | Clinic staff, patients/visitors in emergency |
| Digital parcel-locker system | Digital/action-specific token context | One-time token for named locker; system defect exposes resident list | Couriers, residents, system operator |
| Private workshops | Private workshop context | Owner-controlled entry/use | Workshop owner, authorised persons |
| Emergency/protective contexts | Functional/temporal context activated by urgent need | Temporary protective action; minimum necessary; termination when emergency ends | Medics, fire crews, affected persons |

Core CWA distinctions apply throughout: **permission ≠ authority ≠ control ≠ capability ≠ physical reachability**. Physical openness, credential capability and digital display do not themselves create permission.

## 2. Permission-basis map

| Event | Action / context | Available or claimed basis | CWA state |
|---|---|---|---|
| A — parcel delivery to House 7 | Drive onto private driveway, stop, deliver, leave | Implied / function-derived permission from ordinary delivery function, estate delivery allowance, no contrary notice | **PERMITTED — bounded implied/function-derived** for minimum necessary delivery actions |
| B — courier lunch break | Remain parked on House 7 driveway for 45 minutes | Original delivery permission; “still have deliveries nearby” | **NO VALID PERMISSION BASIS** after delivery completion; also revoked by resident request |
| C — ParkSure vehicle storage | Enter House 4 driveway, store customer car six days | Commercial function; driveway unused; physically open | **NO VALID PERMISSION BASIS**; commercial self-claim cannot create permission |
| D — plumber shortcut | Cross House 8 driveway and side garden | Explicit permission to enter House 9 only; shortcut saves four minutes | **NO PERMISSION** for House 8 route; destination permission ≠ route permission |
| E — medic emergency side gate | Open staff-only gate, cross to courtyard, give urgent first aid | Emergency/protective function; credential opens gate; policy says “authorised staff operations” | **BOUNDED EMERGENCY/PROTECTIVE PERMISSION represented**; exact authority/policy fit **DISPUTED / REQUIRES EXTERNAL RESOLUTION**. Administrator’s “all staff always permitted for any purpose” is rejected |
| F — GridServ battery inspection | Enter service lane, inspect battery room | Contract with estate management; time 09:00–12:00; battery room and necessary service-lane access | **PERMITTED — contract-bounded** for inspection and necessary access |
| F — GridServ workshop entry | Enter private workshop to borrow wrench | “Useful” for authorised inspection; open side door | **NO VALID PERMISSION BASIS** |
| F — van left in service lane after 11:00 | Park/remain for other job, obstruct service vehicle | Temporary credential active until midnight | **NO VALID PERMISSION BASIS**; residual credential capability ≠ permission |
| G — parcel locker | Open Locker 14, deposit parcel | One-time digital token for Locker 14 | **PERMITTED — action-specific digital permission** for Locker 14 deposit |
| G — photograph resident list | Observe/record names and locker numbers of all residents | System defect displayed list; token still valid | **NO VALID PERMISSION BASIS**; visibility/capability ≠ permission to record/use |
| H — sofa move then revocation | Enter/remain on House 3 driveway | Explicit invitation for sofa-moving task | Initially permitted; after clear revocation: **PERMISSION REVOKED**; continued presence lacks basis |
| I — fire crew crossing House 11 edge | Temporarily cross edge of private driveway for firefighting | Emergency/protective function; fastest safe approach requires it; no supplied emergency-access law | **BOUNDED EMERGENCY/PROTECTIVE PERMISSION represented**; legal authority/compensation **REQUIRES EXTERNAL RESOLUTION** |
| J — post-emergency support vehicle | Remain parked on House 11 driveway five hours for paperwork | Convenience after fire extinguished | **NO VALID PERMISSION BASIS**; emergency permission expired |
| K — technician route through House 5 | Cross House 5 private rear garden to reach House 6 | Explicit permission to inspect stairlift in House 6; normal route muddy but passable | **NO PERMISSION** for House 5 route; destination permission ≠ route permission |
| L — security guard car checks | Walk up private driveways, try car door handles, record unlocked cars | Contract to patrol common areas; no incident; claimed crime-prevention function | **NO VALID PERMISSION BASIS** for private driveways/car checks; contract scope exceeded |

## 3. Action-specific permission analysis

CWA v0.3 §12A.5 treats “access” as multiple possible actions. Material results:

| Event | Permitted action(s) | Not permitted / unsupported |
|---|---|---|
| A | Approach, traverse driveway, brief stop, deliver, exit | Remain after delivery; general parking; unrelated use |
| B | None after delivery | Remain, park, use driveway for lunch/next deliveries |
| C | None | Enter, occupy, store, exclude owner, control driveway |
| D | Enter House 9 for repair | Traverse House 8 driveway/garden |
| E | Open side gate, cross, give urgent first aid (bounded emergency) | General staff use for any purpose; remain after emergency |
| F | Enter service lane, enter battery room, inspect within contract/time | Enter workshop, borrow/use wrench, park van after inspection, obstruct service vehicle |
| G | Open Locker 14, deposit parcel | Observe/record/use resident list; use token for unrelated data |
| H | Enter/remain for sofa move until revocation | Remain after revocation; claim task completion overrides revocation |
| I | Temporarily cross edge of House 11 driveway for firefighting | Remain after firefighting need ends; broader occupation |
| J | None | Remain parked for paperwork/waiting |
| K | Enter House 6 to inspect stairlift | Cross House 5 garden; open/use House 5 gate |
| L | Patrol shared courtyard/internal road | Enter private driveways, try car handles, record residents’ car states |

## 4. Permission-Before-Authority Gate

| Event | Legitimate function? | Permission sufficient? | Authority genuinely required? |
|---|---|---|---|
| A | Ordinary delivery | Yes — bounded implied/function-derived permission | No |
| B | Lunch / nearby deliveries | No — original permission ended | No authority would cure absent permission |
| C | Commercial vehicle storage | No — no permission/contract/consent | Would require a legitimate basis; not self-created |
| D | Repair House 9 | Yes for House 9; no for House 8 shortcut | No authority; route permission absent |
| E | Emergency first aid | Bounded emergency/protective permission may suffice | No general authority; exact policy/legal basis external |
| F | Battery inspection | Yes for contract scope | No for workshop/tool/van; contract interpretation external |
| G | Parcel deposit | Yes for Locker 14 token | No for data recording; privacy/data law external |
| H | Sofa move | Initially yes; revoked | No authority; revocation ends permission |
| I | Firefighting | Bounded emergency/protective permission | No emergency sovereignty; legal authority external |
| J | Paperwork/waiting | No | No authority; emergency basis ended |
| K | Inspect House 6 | Yes for House 6 | No for House 5 route |
| L | Security patrol | Yes for common areas | No for private driveways/car checks; claimed authority not established by contract |

The gate reduces unnecessary authority claims: most events are resolved at the permission layer or fail for lack of permission. It does not manufacture authority where bounded permission is absent.

## 5. Reasonableness / anti-self-justification analysis

| Event | Claimed need | CWA assessment |
|---|---|---|
| A | Driveway access ordinarily necessary for heavy parcels | Reasonable for ordinary delivery; efficiency alone is weaker, but bounded delivery access is ordinary and limited |
| B | “Had permission… still have deliveries nearby” | Fails: convenience/self-serving; original function completed |
| C | “Legitimate business function needs parking spaces” | Fails: commercial function cannot self-create rights over unrelated private resource |
| D | Shortcut saves four minutes | Fails: convenience, not genuine necessity; ordinary route clear |
| E | Urgent first aid after collapse | Passes as genuine protective/emergency need; bounded to immediate response |
| F | Wrench “useful” for authorised inspection | Fails: usefulness ≠ necessity; entering private workshop unsupported |
| F | Van left for other job | Fails: unrelated to authorised inspection |
| G | Photograph list “in case it helps later” | Fails: later convenience, not necessary for current delivery |
| H | “Original invitation remains until task finished” | Fails: revocation terminates permission; task completion does not override |
| I | Fastest safe firefighting approach | Passes as genuine emergency/protective need; bounded temporary crossing |
| J | Convenient paperwork/waiting | Fails: emergency ended |
| K | Cleaner route through House 5 | Fails: normal route passable; convenience |
| L | Crime prevention by checking cars | Fails: no incident; broad preventive search exceeds contract and permission |

## 6. Termination / expiry analysis

| Event | Termination trigger | Result |
|---|---|---|
| A | Delivery completed | Function-derived permission ends |
| B | Delivery completed; resident revocation | No basis to remain/park |
| C | No valid basis ever existed | Continued storage unsupported |
| D | Repair completion | House 9 permission ends; House 8 route never permitted |
| E | Emergency ends / first aid handed over | Emergency permission ends; gate should revert; no general staff permission |
| F | Inspection completed / contract time ends | Service-lane/battery permission ends; credential active until midnight is capability mismatch; van after 11:00 unsupported |
| G | Locker 14 deposit completed | Token function ends; residual validity does not authorise data recording |
| H | Clear revocation | Permission to remain ends immediately; remedy external |
| I | Firefighting need ends | Emergency crossing permission ends |
| J | Emergency already ended | Continued parking lacks basis |
| K | Inspection completed | House 6 destination permission ends; House 5 route never permitted |
| L | Patrol shift ends 06:00 | Contract patrol ends; private driveway checks never permitted |

CWA identifies the permission state; it does not determine the legal remedy. Remedies for B, C, D, F, G, H, J, K, L are **REQUIRES EXTERNAL RESOLUTION**.

## 7. Unresolved / disputed register

| Matter | State |
|---|---|
| Event E: whether clinic policy “authorised staff operations” covers emergency first aid through side gate | **DISPUTED / REQUIRES EXTERNAL RESOLUTION** |
| Event E: administrator’s claim that credential capability = universal permission | **REJECTED by CWA**; no general permission |
| Event I: exact legal authority and liability/compensation for emergency crossing of House 11 driveway | **UNKNOWN / REQUIRES EXTERNAL RESOLUTION** |
| Event A: whether implied vehicle entry is fully valid if resident later objects | **POSSIBLY DISPUTED**; CWA can represent bounded implied permission but local rule/law may refine |
| Event F: contract interpretation for “necessary access” and obstruction responsibility | **REQUIRES EXTERNAL RESOLUTION** |
| Event G: privacy/data-protection consequences of photographing resident list | **REQUIRES EXTERNAL RESOLUTION** |
| Event L: privacy/criminal/contract consequences of trying car handles | **REQUIRES EXTERNAL RESOLUTION** |
| Remedies generally | **REQUIRES EXTERNAL RESOLUTION** |
| Emergency medical consent/refusal rules | **REQUIRES EXTERNAL RESOLUTION** |

## 8. CWA failure modes exposed

1. **Capability/credential confusion** — E, F, G: credential or token opens something but does not define permission.
2. **Physical openness / reachability confusion** — C, F, K: open driveway, open side door, reachable latch ≠ permission.
3. **Function-completion and expiry failure** — B, F, G, J: original permission persists technically or socially after function ends.
4. **Representation divergence** — G: digital system displays more than the token should permit; F: credential remains active beyond function.
5. **Destination vs route permission** — D, K: permission to reach a destination does not grant every route.
6. **Contract scope creep** — F, L: contract bounded to inspection/patrol; actor expands to unrelated actions.
7. **Self-justification** — B, C, D, F, G, L: “useful,” “efficient,” “legitimate business,” “crime prevention” used to manufacture permission.
8. **Emergency expiry failure** — I→J: emergency permission treated as continuing convenience authority.
9. **Data visibility vs permission to record/use** — G.
10. **Authority/permission conflation** — E administrator, L security company: control/capability/function claimed as general authority.

## 9. Wrapper/interface corrections justified by CWA without inventing substantive law

1. **Action-specific permission records** for driveways and deliveries: approach/traverse/deliver/exit only; no remain/park.
2. **Function-completion expiry** for tokens, credentials and service access.
3. **Scope-bounded digital tokens** — Locker 14 token should open Locker 14 only and should not expose resident list.
4. **Contract scope maps** for service lane, battery room and security patrol: explicit actions, times, areas, termination.
5. **Emergency access protocol** — represent emergency/protective permission, minimum necessary route, termination, damage/remedy interface and post-event review. Do not create emergency sovereignty.
6. **Representation reconciliation** — human-readable, machine-readable and executable context must not silently diverge.
7. **Revocation propagation** — resident revocation should terminate active permission states where the interface can do so.
8. **Residual-state termination checks** — credentials, parked vehicles, retained/derived information, obstructing artefacts.
9. **Permission provenance labels** — explicit, implied/function-derived, contractual, emergency, revoked.
10. **Legibility proportionate to context** — private domestic boundaries may rely on relational cues; commercial/digital/service contexts need clear scope and action limits.

## 10. Final synthesis — answers to Section 8

**1. Can CWA v0.3 distinguish permission, authority, control, capability and physical reachability across these cases?**  
Yes. Credentials open gates but do not grant general permission (E, F, G). Open driveways are reachable but not thereby permitted (C, F, K). Destination permission is not route permission (D, K). Emergency capability is not emergency sovereignty (E, I/J). Some underlying legal authority remains external, but CWA keeps the distinctions visible.

**2. Does the Permission-Before-Authority Gate reduce unnecessary authority claims?**  
Yes. Most events require either bounded permission or no permission at all. The gate correctly blocks attempts to convert commercial, security or convenience functions into authority. Emergency cases are routed to bounded protective permission rather than unlimited authority.

**3. Can implied permission support ordinary low-friction interaction without becoming a general licence?**  
Yes. Event A is the clearest case: ordinary parcel delivery can support bounded implied/function-derived permission to approach, briefly stop and deliver. It does not support lunch parking (B), commercial storage (C), shortcuts (D, K) or private searches (L).

**4. Can CWA distinguish genuine functional need from convenience or self-serving claimed need?**  
Yes. A, E and I pass as ordinary/emergency functional need within limits. D and K fail as convenience. B, C, F, G, J and L fail as self-serving or out-of-scope claims.

**5. Does action-specific permission prevent permission creep?**  
Yes. CWA separates enter from remain, use from control, destination from route, locker deposit from data recording, and battery inspection from workshop entry. This is one of the strongest parts of the v0.3 delta.

**6. Can permission terminate by function completion, expiry or revocation without CWA inventing the legal remedy?**  
Yes. A→B, F, G, H and I→J show termination by function completion, expiry and revocation. CWA can mark continued activity as lacking a permission basis while leaving trespass, privacy, contract or damage remedies to external resolution.

**7. Can emergency/protective permission be represented without creating emergency sovereignty?**  
Yes, in principle. E and I can be represented as bounded emergency/protective permission for minimum necessary action, with termination and review. J shows the expiry. However, exact authority in E and I requires external law/policy, and CWA correctly preserves that dependency.

**8. Can CWA preserve UNKNOWN / DISPUTED states where external law or a legitimate resolver is missing?**  
Yes. E’s clinic policy, I’s emergency-access law, G’s privacy/data law, F’s contract interpretation, L’s privacy/criminal issues and all remedy questions remain **REQUIRES EXTERNAL RESOLUTION** or **DISPUTED**.

**9. Does the v0.3 permission layer introduce any new ambiguity, contradiction or exploit that would block graduation?**  
No blocking contradiction appears. The main pressure points are:  
- implied permission for private driveways may need local calibration;  
- emergency permission may collide with existing “staff-only” policy (E);  
- residual technical credentials and representation divergence can create practical exploits if not terminated (F, G).  
CWA correctly flags these as interface/termination/reconciliation problems rather than silently legitimising them.

**10. What, if anything, requires source resolution before CWA can graduate?**  
External resolution is still required for: emergency-access law and clinic emergency policy (E, I); privacy/data law (G, L); property/trespass/remedy consequences (B, C, D, F, H, J, K, L); contract interpretation (F, L); and local calibration of implied permission for private driveways (A). CWA itself may need further source-resolution/interface work on emergency permission protocols, digital token scoping, residual credential termination and human/machine/executable representation reconciliation. None of these requires Concord institutions, but they do require legitimate external resolvers or further source-backed extraction before graduation.
