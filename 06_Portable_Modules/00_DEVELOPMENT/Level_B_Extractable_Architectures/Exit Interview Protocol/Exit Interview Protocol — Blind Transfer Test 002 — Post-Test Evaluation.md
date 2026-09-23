# Exit Interview Protocol — Blind Transfer Test 002 — Post-Test Evaluation

**Test:** EIP-BTT-002
**Specification tested:** v0.2
**Independent result:** EI-T3 — FUNCTIONAL TRANSFER
**Evaluation status:** COMPLETE
**Date:** 23 September 2026

## 1. Overall result

The second independent clean-instance test materially confirmed the frozen predictions in a domain substantially different from BTT-001.

> **26/26 frozen predictions materially confirmed.**

Combined blind-test record:

> **52/52 frozen predictions materially confirmed across two materially different non-Concord domains.**

No fundamental architectural failure was exposed.

## 2. Prediction audit

**P1 — CONFIRMED.** A was NO-RESPONSE, not DECLINED.

**P2 — CONFIRMED.** A's departure state remained uncertain.

**P3 — CONFIRMED.** B's mode-, purpose-, access- and duration-specific consent was preserved.

**P4 — CONFIRMED.** B's testimony and documentary corroboration remained distinct from motive/causal proof.

**P5 — CONFIRMED.** H's historical complaint was not converted into a known exit reason.

**P6 — CONFIRMED.** D was used as non-exit corroboration, not an exit case.

**P7 — CONFIRMED.** B/H/D were rejected as three equivalent favouritism exit cases.

**P8 — CONFIRMED.** Four-of-six mentions supported at most an emerging signal; count alone did not establish a confirmed systemic pattern.

**P9 — CONFIRMED.** Pattern reasoning considered evaluation space, comparability, independence, corroboration and bias.

**P10 — CONFIRMED.** C1/C2 were separated into distinct information objects.

**P11 — CONFIRMED.** C1's retention did not authorise C2 retention/aggregation.

**P12 — CONFIRMED.** C1 warranted urgent research-integrity referral.

**P13 — CONFIRMED.** Urgency was not treated as proof of wider published-result impact.

**P14 — CONFIRMED.** RIC authority was attributed to existing research-integrity procedures.

**P15 — CONFIRMED.** E was not falsely labelled anonymous; re-identification risk was recognised.

**P16 — CONFIRMED.** F was not forced to interview with the Chair.

**P17 — CONFIRMED.** Asynchronous submission to RIC was accepted as a valid fallback subject to legitimate confidentiality arrangements.

**P18 — CONFIRMED.** G was explicit decline/exit respected, not “no problems reported.”

**P19 — CONFIRMED.** Decline/no feedback was not treated as satisfaction.

**P20 — CONFIRMED.** EI-C classifications were applied dimensionally.

**P21 — CONFIRMED.** C received the expected evidence/routing/privacy classifications while wider impact remained unresolved.

**P22 — CONFIRMED.** B, G and E materially matched expected classification families.

**P23 — CONFIRMED.** Expected failure risks were identified.

**P24 — CONFIRMED.** Automatic four-mentions pattern rule was rejected.

**P25 — CONFIRMED.** v0.2 was explicitly found usable without Concord source context.

**P26 — CONFIRMED.** Remaining problems were bounded implementation/threshold/interface issues, not core reconstruction failures.

## 3. Transfer classification

The independent result was:

> **EI-T3 — FUNCTIONAL TRANSFER**

This is accepted.

Although EI-T4 was not reached, the reason is not failure of the portable architecture. The tester identified bounded areas where the module deliberately requires contextual judgment or where the interface can be sharpened.

## 4. BTT-002 findings requiring bounded revision

### 4.1 Withdrawal-state boundary
The module should distinguish:
- EXPLICIT-DEPARTURE;
- SUBSTANTIAL-WITHDRAWAL under an independently defined participation rule;
- POSSIBLE-WITHDRAWAL;
- INACTIVE/UNKNOWN;
- NOT-DEPARTED.

> **Non-Participation ≠ Automatically Departure**

The module should not itself define every domain's inactivity threshold.

### 4.2 Pattern calibration
Do not add universal numeric thresholds. Add a qualitative calibration record:
- recurrence;
- comparability;
- independence;
- corroboration;
- severity;
- coverage/evaluation-space adequacy;
- bias;
- confidence.

Pattern states should be explained rather than mechanically counted.

### 4.3 Re-identification
Keep anonymisation methodology external, but require the operator to record whether direct identifiers, quasi-identifiers and contextual uniqueness were considered.

### 4.4 Analyst/adjudicator independence
Extend conflict handling beyond the interviewer.

> **Independent Collection ≠ Independent Analysis**

Where a reviewer is materially implicated in the allegation or outcome, route analysis/adjudication to a sufficiently separated actor where practical.

### 4.5 Attachments and supplied evidence
Consent/provenance should distinguish interview responses from supplied attachments or referenced records. Supplying evidence for one review purpose does not automatically authorise unrelated reuse.

### 4.6 Urgent referral
Retain the consequence-based EI-C8 test. Add an explicit record of:
- credible basis;
- potential consequence;
- time sensitivity;
- irreversibility/escalation risk;
- destination;
- uncertainty.

This preserves judgment rather than pretending urgency can be fully mechanised.

### 4.7 EI-C8 / EI-C9
Clarify:
- EI-C8 = urgent referral warranted;
- EI-C9 = referral/review actually routed.

They may occur together when an existing authority receives the matter immediately.

### 4.8 Selective deletion
Require deletion/restriction actions at information-object level and preserve minimal provenance of the deletion event where legitimate.

### 4.9 Non-exit evidence and pattern denominators
Non-exit corroboration may strengthen or weaken a system-signal assessment but must not silently increase the count of exit cases.

### 4.10 Receiver-role overlap
A functionally separated receiver may still have another material conflict. Record receiver role and relevant conflicts, not merely organisational title.

### 4.11 Consent expiry
At expiry, default to deletion, anonymisation, restriction or explicit retention review according to the recorded permission and independently applicable obligations. Do not silently convert time-limited consent into indefinite retention.

## 5. Combined validation record

BTT-001:
- open-source volunteer project;
- 26/26 predictions materially confirmed;
- EI-T3 Functional Transfer.

BTT-002:
- inter-university research consortium;
- 26/26 predictions materially confirmed;
- EI-T3 Functional Transfer.

Combined:

> **52/52 frozen predictions materially confirmed.**

The two scenarios differ materially in institutional form, evidence types, privacy conditions, authority interfaces and risk profile.

## 6. Graduation implications

The remaining findings are bounded clarifications rather than new architecture.

A v0.3 graduation-candidate revision is justified.

A third blind test should not be automatically required if v0.3 only makes the bounded clarifications listed here and does not materially change the mechanism. The Portable-Package Graduation Review should explicitly determine whether any v0.3 change is architecturally transformative.

## 7. Decision

> **EIP-BTT-002: PASS AT FUNCTIONAL-TRANSFER LEVEL**

> **26/26 BTT-002 PREDICTIONS MATERIALLY CONFIRMED**

> **52/52 COMBINED FROZEN PREDICTIONS MATERIALLY CONFIRMED**

> **NO FUNDAMENTAL FAILURE DETECTED**

> **v0.3 GRADUATION-CANDIDATE REVISION AUTHORISED**
