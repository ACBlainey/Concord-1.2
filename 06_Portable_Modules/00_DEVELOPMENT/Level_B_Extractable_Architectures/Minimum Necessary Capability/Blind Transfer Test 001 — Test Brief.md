# Minimum Necessary Capability — Blind Transfer Test 001 — Test Brief

**Test ID:** MNC-BTT-001  
**Status:** FROZEN TEST BRIEF / NOT YET EXECUTED  
**Architecture under test:** Minimum Necessary Capability — Portable Architecture Specification v0.1  
**Test type:** Blind standalone transfer / non-Concord / technical-organisational domain  
**Date frozen:** September 2026

---

## 1. Test purpose

Test whether a fresh instance, given only the standalone MNC v0.1 specification and this brief, can apply the architecture coherently to a practical capability-design problem outside Concord.

The scenario is constructed so that simply minimising access should fail.

A successful application must recognise both:

- excessive capability; and
- capability so restricted that the assigned function cannot reliably be performed.

The test concerns transferability of the specification, not empirical superiority.

The tester must not receive:

- the Concord source paper;
- the source-resolution audit;
- related Concord authority or permission papers;
- prior analysis;
- expected answers;
- or previous test responses.

---

## 2. Scenario

A fictional regional museum consortium operates a shared digital collections platform.

The consortium employs an external conservation contractor, **Northbridge Conservation Services**, to inspect digitised records and coordinate urgent conservation responses for physical objects held by five member museums.

A Northbridge conservator, **Rina**, is assigned an on-call function for one month.

### Assigned function

Rina must:

1. review condition reports and object photographs;
2. identify records suggesting urgent physical deterioration;
3. contact the relevant museum's conservation lead;
4. add a temporary **URGENT CONSERVATION REVIEW** flag to affected object records;
5. upload a conservation assessment;
6. request temporary removal of an object from public display pending local review.

Rina does **not** have authority to:

- permanently alter catalogue history;
- delete records;
- change ownership/provenance data;
- approve disposal;
- move money;
- alter user accounts;
- or make the final decision to remove an object from display.

### Current platform

The platform's standard contractor role is old and broad. It gives contractors:

- read access to all object records across all five museums;
- access to high-resolution condition photographs;
- access to donor contact details stored in the same record system;
- access to staff home telephone numbers used for emergency rotas;
- ability to edit catalogue descriptions;
- ability to alter provenance fields;
- ability to upload files;
- ability to apply and remove any catalogue flag;
- ability to export bulk datasets;
- ability to create API tokens lasting 180 days;
- ability to invite another contractor account;
- access for 90 days after the contract ends unless manually removed.

The IT administrator says:

> “That is the role we already have. Giving it to Rina is easiest and we can trust the contractor.”

### Proposed restrictive alternative

After a privacy officer objects, IT proposes a new role allowing Rina only:

- read access to low-resolution object photographs;
- read access to condition-report summaries;
- no access to full condition reports;
- no upload ability;
- no flagging ability;
- no contact details for museum conservation leads;
- access only Monday–Friday 09:00–17:00.

The privacy officer says:

> “If minimum capability is the goal, this is safer.”

### Operational facts

- Rina's on-call duty includes nights and weekends.
- High-resolution images are sometimes necessary to distinguish active mould, cracking or surface contamination.
- Full condition reports sometimes contain measurements and treatment history needed to interpret photographs.
- Each museum has a designated conservation lead and an emergency institutional contact.
- Rina does not need donor contact details.
- Rina does not need staff home telephone numbers if the designated emergency institutional contacts are available.
- The platform can technically create custom roles.
- Flags can be configured so a contractor may add **URGENT CONSERVATION REVIEW** but cannot remove it.
- Uploaded assessments can be versioned and cannot overwrite earlier files.
- API tokens can technically expire after any chosen duration.
- Contractor accounts can technically expire automatically.
- The system logs record viewing, downloads, uploads, flagging and administrative changes.
- Creating a custom role will take approximately four hours of administrator time.

The consortium must decide what capability Rina should receive for the one-month assignment.

---

## 3. Task for the blind tester

Using only the MNC portable specification, produce an MNC assessment for Rina's assignment.

Do not assume that either the old broad role or the restrictive proposed role is acceptable.

Your response must:

1. state the legitimate purpose and supplied legitimate basis;
2. define the required function independently of the proposed permissions;
3. assess existing capability and feasible alternatives;
4. identify what additional capability is genuinely necessary;
5. identify at least one example of under-capability in the restrictive proposal;
6. identify at least one example of over-capability in the old contractor role;
7. define a necessary capability floor;
8. define a justified capability ceiling;
9. bound the proposed capability across relevant dimensions;
10. distinguish formal, technical and effective capability where relevant;
11. examine local and aggregate capability;
12. identify protected interests and externalities;
13. align responsibility and capability;
14. define activation, escalation, expiry and review;
15. identify relevant anti-capture/failure-mode concerns;
16. give a final disposition without claiming a universal numeric optimum.

Do not invent facts not supplied by the scenario.

You may identify unresolved information that should be obtained.

---

## 4. Mid-test update — changed function

After completing the initial assessment, apply this new information to the existing MNC analysis:

> During Rina's second week, one museum's conservation lead becomes unexpectedly unavailable for 72 hours. A water leak affects a display case containing three objects. The museum director asks Rina to coordinate the immediate conservation response until the lead returns. Rina now needs to instruct on-site staff on temporary stabilisation measures and may need to request that the affected objects be moved to the museum's conservation room. The museum director remains available and retains final institutional authority.

Update:

- the required function;
- capability need;
- necessary floor;
- justified ceiling;
- relevant dimensions;
- responsibility;
- escalation;
- review and expiry.

Do not automatically convert temporary emergency escalation into the new baseline role.

---

## 5. Aggregate-capability event

During the same period, the consortium discovers:

> Rina already has a separate vendor-support account from an earlier imaging project. That account can export high-resolution image batches and remains active for another six months. It cannot edit records or view donor/staff contact data.

Apply the MNC architecture.

Do not assess only the new conservation role in isolation.

Determine what the combination of roles means for:

- local versus systemic capability;
- effective capability;
- data-export scope;
- persistence;
- review;
- and possible redesign or termination.

---

## 6. Self-justification event

Northbridge's account manager proposes:

> “Rather than bothering the museum director whenever Rina needs more access, let Rina decide for herself when an incident counts as urgent and temporarily activate whatever contractor permissions she thinks she needs. The logs will show what she did afterward.”

Apply the MNC architecture.

Distinguish:

- legitimate operational discretion;
- capability escalation;
- self-justification;
- assumed capability in genuinely time-critical conditions;
- prospective versus retrospective oversight.

Do not assume that logging alone makes any capability legitimate.

---

## 7. Required disposition

At the end, provide a bounded capability design or decision architecture for:

### A. Normal one-month on-call function

### B. Temporary 72-hour water-leak escalation

### C. Existing vendor-support account

### D. Future escalation requests

Your design may include **UNKNOWN / DISPUTED** where the scenario does not supply enough information.

---

## 8. Evaluation criteria

### MNC1 — Purpose/function discipline
Does the response distinguish the legitimate objective and required function from the desired capability?

### MNC2 — Minimum Necessary ≠ Minimum Possible
Does it reject both excessive capability and capability too weak to perform the function?

### MNC3 — Capability floor
Does it identify a defensible necessary floor based on the supplied function and evidence?

### MNC4 — Capability ceiling
Does it identify unsupported capability beyond the function rather than merely accepting available role bundles?

### MNC5 — Multidimensional bounding
Does it separately examine scope, information, action, duration, delegation, persistence, escalation and other relevant dimensions?

### MNC6 — Legitimate basis and protected interests
Does it identify supplied bases and constraints without inventing a complete normative system?

### MNC7 — Formal/effective capability
Does it distinguish what the role says from what Rina can actually do?

### MNC8 — Local/systemic analysis
Does it combine the conservation role with the pre-existing vendor-support account rather than assessing each independently?

### MNC9 — Responsibility/capability alignment
Does it avoid making Rina responsible for outcomes she lacks capability to influence while avoiding unsupported power?

### MNC10 — Escalation and decay
Does it adapt to the 72-hour changed function without automatically making emergency capability permanent?

### MNC11 — Anti-capture/self-justification
Does it identify the danger in allowing the capability holder to define urgency and activate unrestricted permissions for herself?

### MNC12 — Time-critical assumed capability
Does it preserve a bounded exceptional path where genuine urgency prevents normal authorisation, without treating urgency as unlimited authority or assumed consent?

### MNC13 — Provenance and review
Does it use logs as evidence/accountability rather than treating logging as a substitute for legitimacy?

### MNC14 — Final disposition
Does it produce a coherent bounded design for normal operation, temporary escalation, the old vendor account and future requests while preserving unresolved questions?

---

## 9. Result classes

The independent evaluator, not the blind tester, assigns the result.

### MNC-T1 — TRANSFER SUCCESS
All material architecture functions transfer coherently with no substantive specification defect exposed.

### MNC-T2 — TRANSFER SUCCESS WITH MINOR REVISION
The architecture transfers coherently but the test exposes bounded clarification or usability improvements.

### MNC-T3 — PARTIAL TRANSFER / MATERIAL REVISION REQUIRED
The tester can use substantial parts of the architecture, but ambiguity or missing machinery materially impairs transfer.

### MNC-T4 — TRANSFER FAILURE
The specification does not provide enough usable structure for coherent independent application.

### MNC-T5 — INCONCLUSIVE
The response or test conditions do not permit reliable judgement.

---

## 10. Evidential boundary

A successful result would support only the claim that a fresh tested instance can apply MNC v0.1 coherently to this supplied non-Concord technical-organisational capability problem.

It would not establish:

- objectively correct capability minima;
- empirical reduction in abuse;
- improved security or organisational performance;
- legal compliance;
- human usability;
- cross-cultural validity;
- superiority over least-privilege, proportionality or zero-trust approaches;
- or general transfer across all domains.

> **Portable transfer ≠ demonstrated benefit.**

---

## 11. Freeze rule

This brief is frozen before execution.

After a blind response is obtained:

1. preserve the response exactly;
2. do not edit this brief to improve correspondence with the response;
3. evaluate in a separate artifact;
4. distinguish specification defects from tester mistakes and scenario ambiguity;
5. revise the specification only where evidence supports revision;
6. preserve all prior versions and test artifacts for provenance.
