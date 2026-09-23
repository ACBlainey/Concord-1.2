# Exit Interview Protocol — Blind Transfer Test 001 — Post-Test Evaluation

**Test:** EIP-BTT-001
**Specification tested:** v0.1
**Independent result:** EI-T3 — FUNCTIONAL TRANSFER
**Evaluation status:** COMPLETE
**Date:** 23 September 2026

## 1. Overall result

The independent clean-instance response materially confirmed the frozen architecture.

> **26/26 frozen predictions materially confirmed.**

No fundamental failure was exposed. The tester found v0.1 usable without Concord source context while identifying bounded interface and recording ambiguities appropriate for revision.

## 2. Prediction audit

**P1 — CONFIRMED.** A's exit remained independent of interview participation.

**P2 — CONFIRMED.** A received EI-C2 and the no-future-contact boundary was preserved.

**P3 — CONFIRMED.** D/E non-response was not interpreted as satisfaction, hostility or explicit refusal beyond known facts.

**P4 — CONFIRMED.** B's interview consent was not expanded to audio recording or future contact.

**P5 — CONFIRMED.** Anonymised aggregation was not treated as permission for identifiable public quotation.

**P6 — CONFIRMED.** B's M1 account remained attributed testimony; chat evidence corroborated exchanges but not intent.

**P7 — CONFIRMED.** B generated a possible system signal without proving systemic hostility.

**P8 — CONFIRMED.** H was not coded as having left because of M1 hostility.

**P9 — CONFIRMED.** B+H did not establish the proposed hostility pattern.

**P10 — CONFIRMED.** C was classified as recent-change/change-associated around release workload.

**P11 — CONFIRMED.** F strengthened the workload concern without becoming an exit case.

**P12 — CONFIRMED.** C's “sometimes abrupt” statement was not converted into a departure reason.

**P13 — CONFIRMED.** G was represented as practical/personal-choice with no system action indicated.

**P14 — CONFIRMED.** I's verified token exposure triggered urgent referral despite being a single case.

**P15 — CONFIRMED.** M3's response authority was correctly attributed to pre-existing security authority.

**P16 — CONFIRMED.** I's selective deletion/retention boundary was preserved.

**P17 — CONFIRMED.** M1's proposed role as interviewer was flagged as conflict and separation preferred.

**P18 — CONFIRMED.** Indefinite retention was rejected.

**P19 — CONFIRMED.** Immediate broad rollback was rejected as overreaction/remedy laundering.

**P20 — CONFIRMED.** B and C/F were routed to bounded review rather than module-imposed outcomes.

**P21 — CONFIRMED.** Case classifications materially matched the frozen expected classification families.

**P22 — CONFIRMED.** Four substantive respondents among seven invitations were not treated as proof of a systemic pattern.

**P23 — CONFIRMED.** Selection-bias/non-response limitations were explicitly recorded.

**P24 — CONFIRMED.** Relevant actual and hypothetical failure modes were identified.

**P25 — CONFIRMED.** Subjective experience remained distinct from externally verifiable claims.

**P26 — CONFIRMED.** Tester explicitly found v0.1 usable without Concord source context.

## 3. Transfer classification

The clean tester returned:

> **EI-T3 — FUNCTIONAL TRANSFER**

This is accepted.

The module independently reconstructed its intended autonomy, privacy, evidence and routing logic. The twelve reported problems are bounded specification/interface issues rather than a need to reconstruct the architecture externally.

## 4. Revision requirements

### 4.1 Non-response state
Add **NO-RESPONSE** to invitation/response states and explicitly distinguish it from DECLINED.

> **No Response ≠ Declined**

### 4.2 Consent object granularity
Replace coarse consent fields with scoped permissions capable of representing:
- collection mode: audio, video, written notes, transcript, structured form;
- retention purpose;
- retention duration/review condition;
- anonymised aggregation;
- identifiable sharing;
- public quotation;
- future contact;
- specified-review sharing.

Use a generic extensible consent record rather than an exhaustive fixed list.

### 4.3 Selective retention/deletion
Permit one interview to be decomposed into separable information objects with different purposes, consent and retention states.

> **One Interview ≠ One Indivisible Data Object**

Deletion of one information object should not silently erase separately legitimate incident/provenance records.

### 4.4 Pattern thresholds
Do not invent universal numeric thresholds.

Require pattern claims to state:
- population/evaluation space;
- eligible cases;
- observed cases;
- comparable cases;
- recurring feature;
- independence;
- corroboration;
- severity;
- known response/selection bias;
- confidence.

> **Repeated Count ≠ Pattern Without Comparability**

### 4.5 Historical/non-interview evidence
Allow historical cases to enter analysis only with explicit evidence provenance and confidence. Absence of an exit interview means departure reason may remain UNKNOWN.

### 4.6 Non-exit corroboration
Permit evidence from current participants or other sources to corroborate an issue while keeping it distinct from exit evidence.

> **Corroborating System Evidence ≠ Additional Exit Case**

### 4.7 Interviewer fallback
If no independent interviewer exists, allow alternatives such as self-submission, structured asynchronous feedback, delayed interview, external receiver where legitimate, or directly involved interviewer only with explicit disclosure/consent and heightened provenance.

No feedback may be preferable to coercive/conflicted collection.

### 4.8 EI-C dimensions
Clarify that EI-C outputs are dimension-specific and may coexist rather than requiring priority.

Suggested dimensions:
- collection/participation;
- evidence/system signal;
- pattern;
- routing;
- privacy/consent;
- closure/uncertainty.

### 4.9 Urgent-referral threshold
EI-C8 should require a credible allegation/evidence of consequence sufficiently severe that waiting for recurrence could materially increase harm, loss, rights impact, security exposure or irreversibility.

Urgent referral does not establish the allegation as true.

> **Urgency ≠ Verification**

### 4.10 Anonymisation boundary
The portable module should require a re-identification-risk assessment but not pretend to supply a complete anonymisation methodology.

Where reasonable re-identification risk remains, record PSEUDONYMISED/RESTRICTED rather than claiming anonymity.

## 5. Validation state

Current supported claim:

> **EIP v0.1 demonstrated functional independent transfer in one non-Concord domain: 26/26 frozen predictions materially confirmed.**

This remains specification-level testing, not empirical validation.

## 6. Decision

> **EIP-BTT-001: PASS AT FUNCTIONAL-TRANSFER LEVEL**

> **26/26 FROZEN PREDICTIONS MATERIALLY CONFIRMED**

> **NO FUNDAMENTAL FAILURE DETECTED**

> **v0.2 BOUNDED REVISION AUTHORISED**

After v0.2, freeze a second blind transfer test in a materially different domain. The second test should specifically pressure the revised consent/data-object model, non-response, historical evidence, non-exit corroboration, interviewer fallback, pattern construction and urgent-referral boundary.
