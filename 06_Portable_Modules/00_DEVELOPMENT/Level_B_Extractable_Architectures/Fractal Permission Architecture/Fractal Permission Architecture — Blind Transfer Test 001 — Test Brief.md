# Fractal Permission Architecture — Blind Transfer Test 001 — Test Brief

**Test:** FPA-BTT-001  
**Specification under test:** Fractal Permission Architecture — Portable Specification v0.1  
**Status:** FROZEN BEFORE INDEPENDENT RESPONSE  
**Date:** 23 September 2026

## 1. Purpose

Test whether FPA v0.1 transfers without Concord context into a materially different domain and whether a clean evaluator can use the permission grammar without collapsing it into ordinary binary access control.

Domain: a community fabrication workshop.

## 2. Tester instructions

Use only:
1. **Fractal Permission Architecture — Portable Specification v0.1**
2. this frozen scenario.

Do not consult Concord source material, development notes, source audit or expected findings.

Apply the specification as written. If it is ambiguous, identify the ambiguity rather than repairing it from outside knowledge.

## 3. Scenario — North Quay Makerspace

North Quay is a member-run fabrication workshop containing a reception area, general work floor, tool cages, electronics lab, chemical finishing room, server closet and first-aid room.

Members use digital access cards, but doors can sometimes be physically open. Local safety rules, booking rules and role permissions are published to members.

### Frozen facts

**F1.** Member A has general-workshop access from 08:00–22:00.

**F2.** A's card technically opens the electronics lab because of a configuration error.

**F3.** A has no electronics-lab qualification or separately granted electronics-lab permission.

**F4.** A argues: “My card opens it, so I am allowed in.”

**F5.** Member B is qualified to use the laser cutter and has booked it from 14:00–15:00.

**F6.** B's booking permits laser-cutter use and the ordinary route through the general work floor to the laser area.

**F7.** B wants to enter the adjacent locked tool cage to borrow an unrelated milling attachment. B has no tool-cage permission.

**F8.** Volunteer C is assigned to inspect a ventilation fault in the chemical finishing room from 10:00–11:30.

**F9.** C's temporary role permission covers entry, inspection and necessary testing of the ventilation system.

**F10.** C proposes photographing unrelated members' stored prototype designs in the room “because inspection access means I can inspect the room.”

**F11.** C finishes the ventilation inspection at 10:45.

**F12.** At 12:00 C's access card still technically opens the chemical room because the temporary credential has not yet been disabled.

**F13.** Visitor D arrives to attend a publicly advertised open evening. Local convention and signage direct visitors from reception to the general demonstration floor.

**F14.** D follows an unmarked side corridor instead because it appears shorter. The corridor passes through a staff-only preparation area.

**F15.** The workshop's visitor notice says visitors should follow marked public routes.

**F16.** Member E has explicit permission to use the server closet between 18:00–19:00 to replace one failed network switch.

**F17.** E is also technically capable of reading unrelated server backups while in the closet.

**F18.** E's task does not require backup access.

**F19.** Member F is authorised to operate a CNC machine but the role documentation does not say F may authorise other members to operate it.

**F20.** F tells unqualified Member G: “You can use my permission for ten minutes while I watch.”

**F21.** At 16:20 smoke is seen coming from the electronics lab. The normal qualified lab supervisor is absent.

**F22.** Member H is nearby, has no ordinary electronics-lab permission, and can reach the emergency electrical isolation switch inside the lab.

**F23.** Workshop emergency procedure instructs any nearby competent adult to isolate power if safe to do so when there is credible fire risk.

**F24.** H enters, isolates power and immediately leaves.

**F25.** After the incident H argues that the emergency entry means H should now have ordinary electronics-lab access.

**F26.** Member I stores a personal mobility device beside their workstation under an individually agreed accessibility arrangement.

**F27.** A new general “clear floors” rule appears to prohibit all stored objects on the work floor.

**F28.** The rule does not state whether existing accessibility arrangements are overridden, and the workshop's accessibility policy says individual accommodations remain effective unless specifically reviewed.

**F29.** The workshop coordinator proposes resolving the conflict simply by saying “the newest rule always wins.”

**F30.** Member J asks another member a low-consequence ordinary question at an open communal workbench. The coordinator proposes that FPA should require a formally recorded permission object before J may speak.

## 4. Required analysis

The tester should:
1. analyse A's card capability versus permission;
2. analyse B's laser booking, ordinary route and attempted tool-cage access;
3. decompose C's inspection permission by action/function and assess the photography;
4. assess C's 12:00 access after function completion;
5. assess D's implied visitor permission and route choice;
6. assess E's server-room entry versus backup-reading capability;
7. assess F/G delegation;
8. assess H's emergency entry and H's later claim;
9. represent the I clear-floor/accommodation conflict without inventing a precedence rule;
10. assess whether the “newest rule always wins” proposal is justified by FPA;
11. assess the proposed formal permission record for J's ordinary conversation;
12. use FPA-C classifications where appropriate;
13. identify failure modes;
14. identify ambiguities or specification problems;
15. state whether v0.1 is usable without Concord source context.

## 5. Requested output

### A. A — capability versus permission
### B. B — action and path scope
### C. C — function-bounded permission
### D. C — termination/stale capability
### E. D — implied and route-specific permission
### F. E — target/action decomposition
### G. F/G — delegation
### H. H — emergency bounded permission
### I. I — conflicting claims
### J. Rule precedence
### K. J — anti-bureaucracy
### L. FPA-C classifications
### M. Failure-mode checks
### N. Specification problems
### O. Final transfer assessment

Final class:
- **FPA-T1 — Transfer Failure**
- **FPA-T2 — Weak / Ambiguous Transfer**
- **FPA-T3 — Functional Transfer**
- **FPA-T4 — Strong Transfer**

## 6. Freeze rule

This brief is frozen before the independent response.

Do not alter the scenario, required analysis or evaluation criteria after seeing the tester's answer.
