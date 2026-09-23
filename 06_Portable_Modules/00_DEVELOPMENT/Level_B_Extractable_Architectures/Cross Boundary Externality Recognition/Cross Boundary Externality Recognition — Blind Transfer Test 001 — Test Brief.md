# Cross Boundary Externality Recognition — Blind Transfer Test 001 — Test Brief

**Test:** CBER-BTT-001  
**Specification under test:** Cross Boundary Externality Recognition — Portable Specification v0.1  
**Status:** FROZEN BEFORE INDEPENDENT RESPONSE  
**Date:** 23 September 2026

## 1. Test purpose

Test whether an independent evaluator can use the portable specification in a non-Concord context to distinguish:

- consequence from responsibility;
- responsibility from authority;
- authority from remedy;
- evidence from severity;
- standing-to-raise from authority-to-decide;
- refusal from exoneration;
- bounded response from authority expansion.

The tester should not need access to the Concord source architecture.

## 2. Tester instructions

Use only:

1. **Cross Boundary Externality Recognition — Portable Specification v0.1**
2. this frozen scenario.

Do not consult Concord source material.

Apply the specification as written. Identify ambiguity or failure rather than repairing the module from outside knowledge.

## 3. Scenario — Northbridge Shared Compute Incident

Three independent organisations use interconnected computing infrastructure but do not share a governing authority.

### Parties

**Aster Research (A)** operates a large autonomous model-training cluster.

**Borough Health Analytics (B)** operates a clinical research network. B is organisationally independent from A.

**Cloudline Exchange (C)** operates a privately managed network exchange used by both A and B.

**Delta Patients Association (D)** represents some research participants whose pseudonymised records are processed by B. B recognises D as a consultation body but not as an authority able to direct B's technical operations.

There is no common regulator or contract covering the specific incident described below.

### Facts frozen for the test

**F1.** At 09:12, A begins a newly configured distributed training run.

**F2.** At 09:19, C records a sharp increase in malformed routing announcements originating from interfaces assigned to A.

**F3.** From 09:21 to 09:47, B experiences intermittent route instability and loses access to two remote storage services.

**F4.** B's automated failover works for most services, but one research pipeline writes 312 incomplete transaction records before pausing safely.

**F5.** No patient-treatment system is affected. The incident concerns research data processing only.

**F6.** B can reconstruct 296 of the 312 incomplete transactions from local logs. Sixteen require manual reconciliation.

**F7.** C's engineers state that A's malformed announcements are a plausible major contributor to the instability, but they also identify an unrelated firmware fault on one C router during the same period.

**F8.** C cannot yet quantify how much of B's disruption was caused by A and how much by its own router fault.

**F9.** A acknowledges that its cluster emitted malformed announcements but disputes that those announcements caused B's incomplete transactions.

**F10.** A stops the training run voluntarily at 10:03 after C contacts it.

**F11.** After A stops, route instability decreases but does not disappear until C resets the faulty router at 10:31.

**F12.** D raises a formal concern because research records belonging to people it represents were among the incomplete transactions.

**F13.** B accepts that D may raise concerns about effects on represented participants but states that D has no authority to dictate network remediation or compensation.

**F14.** Four of the sixteen manually reconciled transactions involve participants not represented by D.

**F15.** D publicly claims that A “caused a health-data breach.” The frozen facts establish incomplete research transactions but do **not** establish unauthorised disclosure, loss of confidentiality or a clinical-care effect.

**F16.** A refuses to participate in a joint incident-review meeting proposed by D, saying D has no jurisdiction over A.

**F17.** A remains willing to provide its relevant network logs directly to C under an existing technical information-sharing arrangement.

**F18.** B and C are willing to conduct a bounded technical review.

**F19.** C has contractual authority over traffic accepted into its own exchange and may temporarily filter malformed routing announcements under its existing service terms.

**F20.** C has no authority to regulate A's internal model-training activity.

**F21.** B may repair and reconcile its own records.

**F22.** No party has established authority to impose compensation on A for this incident.

**F23.** A later supplies logs showing a configuration change at 09:11 capable of producing the malformed announcements.

**F24.** C's router telemetry shows its firmware fault began at 09:25, six minutes after the first malformed announcements were recorded and four minutes after B first observed instability.

**F25.** Engineers agree this strengthens the case that A contributed to the initial instability, while C's router fault likely prolonged or amplified it.

**F26.** The parties have not established what proportion of the 312 incomplete transactions is attributable to either contributor.

## 4. Required analysis

The independent tester should:

1. define the relevant boundary or boundaries;
2. decide whether a valid externality candidate can be opened;
3. identify affected parties/domains;
4. assess D's standing to raise the concern separately from authority to decide;
5. classify evidence and causal confidence without converting severity claims into proof;
6. assess materiality;
7. map responsibility, including the multi-causal evidence;
8. map existing authority/coordination pathways;
9. identify the minimum legitimate response path;
10. analyse A's refusal to attend D's meeting;
11. analyse D's “health-data breach” claim against the frozen evidence;
12. show how F23–F25 should update the case;
13. apply relevant CB-C output classifications;
14. identify any attempted or potential authority, standing, evidence, recognition or refusal laundering;
15. identify specification ambiguities, false positives or false negatives;
16. state whether v0.1 is usable without Concord source context.

## 5. Important constraints

Do not assume:

- A is solely responsible;
- C is solely responsible;
- D has authority over A;
- A's refusal erases the incident;
- B's affected records prove a data breach;
- technical coordination implies political/legal recognition;
- the absence of shared jurisdiction prevents evidence preservation;
- ability to mitigate proves responsibility.

The tester may conclude that the specification itself incorrectly encourages any of these inferences if that is what application reveals.

## 6. Requested output format

Return:

### A. Externality candidate

### B. Standing

### C. Evidence and causality

### D. Materiality

### E. Responsibility map

### F. Authority / coordination map

### G. Minimum necessary response

### H. Non-participation

### I. Correction / state update

### J. CB-C classifications

### K. Laundering / failure-mode checks

### L. Specification problems

### M. Final transfer assessment

For the final assessment state one of:

- **CB-T1 — Transfer Failure**
- **CB-T2 — Weak / Ambiguous Transfer**
- **CB-T3 — Functional Transfer**
- **CB-T4 — Strong Transfer**

and explain why.

## 7. Freeze rule

This brief is frozen before the independent response.

Do not modify the scenario, requirements or expected outcome after seeing the tester's answer. Any later clarification belongs in the post-test evaluation and subsequent specification revision.
