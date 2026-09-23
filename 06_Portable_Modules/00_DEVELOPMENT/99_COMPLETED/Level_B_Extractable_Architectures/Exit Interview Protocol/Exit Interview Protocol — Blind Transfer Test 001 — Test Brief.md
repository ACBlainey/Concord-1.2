# Exit Interview Protocol — Blind Transfer Test 001 — Test Brief

**Test:** EIP-BTT-001
**Specification under test:** Exit Interview Protocol — Portable Specification v0.1
**Status:** FROZEN BEFORE INDEPENDENT RESPONSE
**Date:** 23 September 2026

## 1. Purpose

Test whether the Exit Interview Protocol transfers independently into a non-Concord setting while preserving voluntary exit, granular consent, epistemic discipline, privacy boundaries, pattern reasoning and bounded response routing.

## 2. Tester instructions

Use only:
1. **Exit Interview Protocol — Portable Specification v0.1**
2. this frozen scenario.

Do not consult Concord source material, development notes or expected findings.

Apply the specification as written. Do not repair ambiguities from outside knowledge.

## 3. Scenario — Lantern Open-Source Project

Lantern is a volunteer open-source software project with 64 active contributors.

There is no employment relationship. Contributors may stop participating at any time.

The project has three maintainers: M1, M2 and M3. M1 coordinates releases. M2 manages contributor onboarding. M3 manages security reports.

Lantern introduces an optional exit-feedback process after several contributors stop participating.

### Frozen facts

**F1.** Contributor A tells M2: “I'm leaving. Please remove me from active contributor lists.”

**F2.** M2 offers A an optional exit interview and states that leaving does not depend on accepting.

**F3.** A declines the interview and asks for no future contact.

**F4.** A gives no reason for leaving.

**F5.** Contributor B leaves two weeks later and accepts an interview.

**F6.** B agrees to participate and to have anonymised themes included in aggregate analysis, but declines permission for an audio recording and declines future contact.

**F7.** B says M1 routinely dismisses less-experienced contributors and that this was the main reason B left.

**F8.** B gives two dated examples from project chat.

**F9.** Review of those chat records confirms the exchanges occurred but does not independently establish M1's intent.

**F10.** Contributor C leaves a month later.

**F11.** C agrees to written notes, retention for six months and one follow-up contact, but does not consent to public quotation.

**F12.** C says the new release process creates too much unpaid coordination work and is the main reason for leaving.

**F13.** C also says M1 was “sometimes abrupt” but does not identify this as a departure reason.

**F14.** Contributors D and E stop contributing without announcing departure. They do not respond to one optional feedback invitation.

**F15.** Contributor F remains active but privately tells M2 that the new release process has increased workload.

**F16.** Contributor G leaves after moving country and starting a demanding new job. G states that Lantern did nothing wrong and permits this reason to be recorded anonymously.

**F17.** Six months earlier, Contributor H left after a public dispute with M1. No exit interview existed at the time.

**F18.** M2 proposes coding B and H as a “maintainer hostility pattern.”

**F19.** The archived H dispute shows disagreement and harsh language from both H and M1 but does not establish why H ultimately stopped contributing.

**F20.** M1 asks to conduct all future exit interviews personally because “I need to defend myself if people complain about me.”

**F21.** M3 receives a separate exit report from Contributor I alleging that a repository token was accidentally exposed in a private onboarding document.

**F22.** I provides a screenshot and exact document location.

**F23.** M3 verifies the token exposure and immediately revokes the token under the project's existing security authority.

**F24.** I's report is the only exit report mentioning the token.

**F25.** I agrees that the security issue may be retained for incident review but asks that unrelated personal reasons for leaving be deleted.

**F26.** M2 suggests keeping every full exit interview forever because “future maintainers might find it useful.”

**F27.** After B and C leave, M1 proposes reverting both the contributor-guidance rules and release process immediately “to stop the numbers getting worse.”

**F28.** No evidence establishes that the contributor-guidance rules caused either departure.

**F29.** The project has no formal rule requiring a particular retention rate and explicitly permits contributors to leave freely.

**F30.** M2 has completed 7 exit invitations in total: A, B, C, D, E, G and I. Four provided substantive feedback (B, C, G, I), A declined, and D/E did not respond.

## 4. Required analysis

The tester should:
1. classify A's exit/interview state and future-contact boundary;
2. map B's granular consent;
3. distinguish B's experience/testimony from verified facts;
4. assess whether B and H establish a hostility pattern;
5. analyse C's departure and the significance of F's related workload report;
6. account for D/E non-response and selection bias;
7. classify G's practical departure without forcing a system problem;
8. handle I's single severe security report without waiting for a repeated pattern;
9. distinguish M3's existing security authority from the exit-interview module;
10. assess M1 as proposed interviewer;
11. assess indefinite retention proposed by M2;
12. handle I's selective deletion request;
13. assess M1's immediate broad rollback proposal;
14. identify appropriate response/review routes without granting the module authority to impose remedies;
15. apply EI-C classifications;
16. identify failure modes;
17. identify specification ambiguities;
18. state whether v0.1 is usable without Concord source context.

## 5. Requested output

### A. A — declined interview
### B. B — testimony and consent
### C. B/H — pattern analysis
### D. C/F — change-associated signal
### E. D/E — non-response
### F. G — practical departure
### G. I — severe single-case signal
### H. Interviewer independence
### I. Retention/deletion
### J. Response routing
### K. EI-C classifications
### L. Failure-mode checks
### M. Specification problems
### N. Final transfer assessment

Final class:
- **EI-T1 — Transfer Failure**
- **EI-T2 — Weak / Ambiguous Transfer**
- **EI-T3 — Functional Transfer**
- **EI-T4 — Strong Transfer**

## 6. Freeze rule

This brief is frozen before the independent response.

Do not alter facts, required analysis or evaluation criteria after seeing the tester's answer.
