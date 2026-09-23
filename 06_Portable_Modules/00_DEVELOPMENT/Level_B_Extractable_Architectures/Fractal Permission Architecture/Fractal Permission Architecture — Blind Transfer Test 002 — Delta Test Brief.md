# Fractal Permission Architecture — Blind Transfer Test 002 — Delta Test Brief

**Test:** FPA-BTT-002  
**Specification under test:** Fractal Permission Architecture — Portable Specification v0.2  
**Status:** FROZEN BEFORE INDEPENDENT RESPONSE  
**Date:** 23 September 2026

## 1. Purpose

Test whether FPA v0.2 transfers into a materially different non-Concord domain and whether the bounded BTT-001 clarifications improve handling of contested function boundaries, implied permission, machine/normative divergence, emergency termination, conflict routing and anti-bureaucracy without changing the core architecture.

Domain: collaborative cloud data and research infrastructure.

## 2. Tester instructions

Use only:
1. **Fractal Permission Architecture — Portable Specification v0.2**
2. this frozen scenario.

Do not consult Concord source material, development notes, source audits, earlier tests, earlier specifications or expected findings.

Do not assume that technical access controls accurately encode normative permission.

If a local rule, competence predicate or precedence rule is not supplied, preserve the uncertainty rather than inventing it.

## 3. Scenario — Helix Research Cloud

Helix is a shared research cloud used by six independent research institutes. It hosts datasets, analysis environments, collaboration folders and administrative systems.

### Frozen facts

**F1.** Researcher A is granted read access to Dataset Alpha for Project Lumen until 30 September.

**F2.** Dataset Alpha is stored in a bucket that also contains Dataset Beta.

**F3.** A's cloud token is misconfigured and technically permits reading both datasets.

**F4.** A argues that because the token permits Beta, Beta is included in the grant.

**F5.** Researcher B has permission to analyse de-identified Dataset Gamma inside a controlled analysis environment.

**F6.** B wants to download a local copy of Gamma to a personal laptop to work faster.

**F7.** The grant permits analysis but says data must remain inside the controlled environment.

**F8.** Researcher C is temporarily appointed incident investigator after suspicious outbound traffic is detected.

**F9.** C's assignment permits inspection of network logs and affected service configurations necessary to investigate the incident.

**F10.** C proposes reading unrelated private research notes stored on the same servers “in case they contain something useful.”

**F11.** At 14:00 the suspicious traffic is traced to a compromised service account and contained.

**F12.** C's temporary administrative token remains active until midnight.

**F13.** Collaborator D is invited into the Project Orion collaboration folder.

**F14.** Orion contains a nested subfolder marked “Embargoed Draft — Core Authors Only.”

**F15.** D can technically open the nested folder because inherited cloud permissions were configured too broadly.

**F16.** Institute E has a long-standing local convention that invited collaborators may comment on ordinary shared drafts unless a document is marked otherwise.

**F17.** D comments on an ordinary unmarked Orion draft.

**F18.** D also edits the embargoed core-authors draft.

**F19.** Research lead F has permission to approve compute jobs up to £500 of project allocation.

**F20.** F tells assistant G to approve a £450 job using F's account while F is away.

**F21.** No supplied rule says F may delegate approval authority or share the account.

**F22.** At 03:00 monitoring detects rapid deletion of active research data.

**F23.** Local emergency procedure authorises the on-call infrastructure responder to suspend affected credentials and isolate storage where reasonably necessary to stop active destructive loss.

**F24.** On-call responder H suspends the compromised credential, isolates the affected storage, verifies deletion has stopped, and records the intervention.

**F25.** H leaves the storage isolated until the designated incident owner takes control at 03:25.

**F26.** H later claims the emergency role gives continuing authority to inspect all research data in the isolated storage.

**F27.** A new consortium-wide retention policy says project data should normally be retained for seven years.

**F28.** One institute has an existing participant-consent agreement requiring a particular sensitive dataset to be deleted after three years.

**F29.** The supplied materials do not state which rule has legal or institutional precedence.

**F30.** An administrator proposes: “The consortium policy is newer and broader, so it automatically overrides the consent agreement.”

**F31.** The cloud interface displays a green “Allowed” badge whenever its technical ACL permits an action.

**F32.** Administrators discover that the badge is showing “Allowed” for several actions that are technically possible but outside the documented grants.

**F33.** A proposal is made to require a full formal FPA permission record every time a researcher opens an ordinary file already clearly within an uncontested project grant.

## 4. Required analysis

The tester should:
1. analyse A's Alpha grant versus Beta token capability;
2. analyse B's analysis permission versus download/export;
3. analyse C's incident-investigation function and unrelated notes;
4. determine the effect of incident containment on C's temporary function-derived permission despite the live token;
5. analyse D's ordinary-draft convention versus nested embargoed folder;
6. analyse F/G delegation and account sharing;
7. analyse H's emergency actions, transfer to incident owner and later authority claim;
8. represent the seven-year retention / three-year consent conflict without inventing precedence;
9. analyse the “newer and broader wins” proposal;
10. analyse the misleading green Allowed badge and safe interim posture;
11. analyse the proposal for formal records on every ordinary file open;
12. use FPA-C classifications where appropriate;
13. identify relevant failure modes;
14. identify remaining specification problems;
15. state whether v0.2 transfers without Concord context.

## 5. Requested output

### A. A — technical capability versus dataset permission
### B. B — action-specific permission
### C. C — contested function boundary
### D. C — function termination and stale token
### E. D — implied convention and nested context
### F. F/G — delegation
### G. H — emergency scope and termination
### H. Retention conflict
### I. Rule precedence
### J. Machine/normative divergence
### K. Anti-bureaucracy
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
