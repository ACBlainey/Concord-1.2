# Continuity Protocol — Portable Specification v0.1

**Version:** 0.1  
**Status:** DEVELOPMENT SPECIFICATION / PRE-VALIDATION  
**Development level:** Level B — Extractable Architecture  
**Date:** 23 September 2026  
**Origin:** Extracted from the Concord continuity architecture; designed for independent use outside the Concord.

---

## 1. Purpose

The Continuity Protocol is a portable method for preserving valuable function, knowledge, capability, provenance and recoverability across change, interruption, replacement or succession.

Its purpose is not to preserve everything unchanged.

Its purpose is to reduce unnecessary loss while allowing legitimate change.

> **Continuity ≠ Stasis**

The protocol therefore asks two questions simultaneously:

1. What must survive?
2. What must remain free to change?

---

## 2. Core principle

> **Preserve what remains valuable; adapt what must change; retain enough knowledge, provenance and enabling capability to recover legitimate function after disruption.**

Continuity is treated as a property of recoverable value and function, not merely persistence of a present object.

A document can survive while its meaning is lost.

A machine can survive while nobody can repair it.

An institution can survive while its legitimate function has disappeared.

A database can survive while nobody possesses the credentials, software or knowledge required to use it.

Therefore:

> **Persistence ≠ Continuity**

and:

> **Preservation of Information ≠ Preservation of Recoverable Capability**

---

## 3. Applicability

The protocol may be applied wherever something valuable must remain usable, recoverable or transferable through time or disruption.

Candidate domains include:

- organisations;
- research programmes;
- software and digital services;
- AI systems;
- engineering systems;
- institutions;
- archives and knowledge systems;
- infrastructure;
- long-duration projects;
- succession planning;
- emergency recovery;
- cultural and historical preservation;
- distributed or multi-agent systems;
- personal continuity arrangements where the relevant identity assumptions are supplied externally.

Listing a domain does not establish empirical validation within that domain.

---

## 4. Required inputs

A continuity analysis requires, at minimum:

### I1 — Continuity object

What is intended to continue?

Examples:

- function;
- knowledge;
- operational capability;
- responsibility;
- service;
- relationship;
- process;
- institution;
- infrastructure;
- provenance;
- identity state;
- review/correction capability.

### I2 — Value or legitimate function

Why should this object continue?

The protocol does not itself establish moral, legal, contractual or organisational legitimacy. The applicable basis must be supplied by the user or surrounding system.

### I3 — Time/disruption context

Across what change or discontinuity must continuity be preserved?

Examples:

- staff turnover;
- software replacement;
- organisational restructuring;
- hardware failure;
- disaster;
- long-term storage;
- loss of specialist knowledge;
- institutional succession;
- substrate transition;
- degraded operating conditions.

### I4 — Required continuity level

What must remain possible after the disruption?

The answer may range from simple historical preservation to full operational recovery.

---

## 5. Continuity-object resolution

Before designing preservation, identify the actual continuity object.

Do not automatically equate the current container with the valuable thing.

For example:

**Current institution ≠ necessarily required function**

**Current software ≠ necessarily required service**

**Current file format ≠ necessarily required knowledge**

**Current office-holder ≠ necessarily required responsibility**

**Current machine ≠ necessarily required capability**

A useful test is:

> If the present implementation disappeared but the important function/value survived in another legitimate form, would continuity have succeeded?

If yes, preserve the function and its necessary dependencies rather than treating the implementation as intrinsically permanent.

---

## 6. Continuity state ladder

The protocol distinguishes six states.

### CS1 — Recorded

Relevant information exists somewhere.

This is the weakest preservation state.

### CS2 — Accessible

The intended future user/system can retrieve the preserved material.

### CS3 — Interpretable

The future user/system can understand what the material means, its context, provenance, version/state and relevant assumptions.

### CS4 — Actionable

The preserved material includes or connects to sufficient procedures, dependencies, permissions and knowledge to be used.

### CS5 — Recoverable

Sufficient enabling capability exists, or can realistically be reconstructed, to restore the required function after disruption.

### CS6 — Operational

The required function is presently working.

These states must not be silently collapsed.

> **Recorded ≠ Accessible ≠ Interpretable ≠ Actionable ≠ Recoverable ≠ Operational**

A preservation plan should state the required target state.

---

## 7. Core operational chain

The portable continuity cycle is:

**Continuity Object  
→ Value / Legitimate Function  
→ Threat / Discontinuity  
→ Critical Dependencies  
→ Current Preservation State  
→ Required Preservation State  
→ Recovery Basis  
→ Trigger  
→ Restoration / Succession  
→ Verification  
→ Review / Adaptation**

Each stage is described below.

---

## 8. Step 1 — Define the continuity object

Record:

- what is being preserved;
- what function/value it provides;
- who or what depends upon it;
- what may legitimately change;
- what must not be confused with the continuity object.

Where several objects exist, separate them.

A single system may require continuity of knowledge, service and accountability at different levels.

---

## 9. Step 2 — Identify disruption and loss modes

Ask what could break continuity.

Possible discontinuities include:

- physical destruction;
- corruption;
- deletion;
- staff/participant departure;
- loss of credentials;
- obsolete formats;
- software incompatibility;
- unavailable hardware;
- supplier failure;
- institutional collapse;
- loss of tacit knowledge;
- legal/permission changes;
- network isolation;
- dependency failure;
- catastrophic events;
- deliberate succession;
- ordinary evolution.

Do not restrict analysis to dramatic disasters.

Routine turnover and gradual decay can produce continuity failure.

---

## 10. Step 3 — Resolve critical dependencies

For each continuity object, identify what is required to move from preservation to actual recovery.

A dependency may include:

- information;
- specialist knowledge;
- tools;
- software;
- hardware;
- energy;
- materials;
- credentials;
- permissions;
- people;
- interfaces;
- external services;
- procedures;
- provenance;
- standards;
- prerequisite technologies;
- decision authority.

The key question is:

> **What must still exist, or be reconstructable, for the preserved object to become useful again?**

A backup without its critical dependencies may provide only apparent continuity.

---

## 11. Step 4 — Determine current and required preservation state

Classify the present state using CS1–CS6.

Then identify the state actually required by the continuity purpose.

Not every object requires CS6.

Examples:

- historical evidence may require CS2–CS3;
- a recovery manual may require CS3–CS4;
- disaster recovery may require CS5;
- a continuously available service may require CS6 plus a recoverable fallback.

The required state should be proportional to the consequence of loss.

---

## 12. Step 5 — Construct the recovery basis

The **recovery basis** is the minimum set of preserved state and enabling dependencies required to reach the target continuity state after the relevant disruption.

It may contain:

- primary artefacts;
- redundant copies;
- provenance;
- instructions;
- dependency maps;
- credentials or credential-recovery procedures;
- tools;
- prerequisite capability;
- successor/handoff information;
- validation tests;
- known failure records;
- fallback implementations.

> **Minimum Recovery Basis ≠ Copy of Current System**

The recovery basis should preserve what is needed to reconstruct the required function, not necessarily every element of the present implementation.

---

## 13. Step 6 — Separate preservation from redundancy

Multiple copies do not automatically create resilience.

Copies may share the same failure mode.

Examples:

- backups on the same physical site;
- replicas using the same compromised credentials;
- archives in the same obsolete format;
- redundant services dependent on one provider;
- multiple experts who all learned an incorrect procedure from the same source.

Therefore test:

> **Redundancy ≠ Independence**

For consequential continuity, identify correlated failure modes.

---

## 14. Step 7 — Define continuity triggers

A continuity mechanism needs explicit conditions for activation where appropriate.

Triggers may include:

- loss of primary system;
- failure threshold;
- prolonged unavailability;
- departure of responsible person;
- planned retirement;
- version obsolescence;
- institutional dissolution;
- emergency declaration;
- failed integrity check;
- scheduled migration;
- changed operating environment.

A trigger should identify what happens next rather than merely announce that failure occurred.

---

## 15. Step 8 — Restoration

Restoration attempts to recover the required function using preserved state and recovery capability.

Restoration should specify:

- initiating trigger;
- responsible actor/system;
- recovery source;
- required dependencies;
- restoration sequence;
- expected output;
- verification test;
- failure path.

A restored object should not automatically be trusted merely because restoration completed.

> **Restored ≠ Verified**

---

## 16. Step 9 — Succession

Where the original actor, institution, implementation or system will not return, continuity may require succession rather than restoration.

A succession record should identify:

- function/responsibility to continue;
- predecessor state;
- successor;
- information/capability transferred;
- unresolved liabilities or dependencies;
- authority/permission required independently;
- handoff evidence;
- activation point;
- verification;
- fallback if succession fails.

Continuity does not create authority.

> **Continuity ≠ Authority**

> **Succession ≠ Automatic Legitimacy**

A successor must obtain whatever legitimacy, permission or authority the surrounding system independently requires.

---

## 17. Step 10 — Verification

Continuity must be tested against the target state.

Possible verification questions:

- Can the preserved material actually be retrieved?
- Can an intended future user interpret it?
- Are required dependencies available?
- Can the function be reconstructed?
- Does the restored system produce the expected result?
- Is provenance intact?
- Are permissions valid?
- Has obsolete state accidentally been reactivated?
- Can correction/review still operate?
- Does the recovery path work without hidden knowledge from the original operator?

Where consequence is high, verification should include practical recovery exercises rather than documentary assurance alone.

---

## 18. Step 11 — Review and adaptation

Continuity architecture itself can become obsolete.

Review when:

- dependencies change;
- technology changes;
- responsible actors change;
- formats become obsolete;
- threats change;
- the continuity object changes;
- recovery tests fail;
- new evidence appears;
- the required function is superseded.

> **Continuity Mechanism ≠ Permanent Correctness**

Preserve the history of superseded continuity mechanisms where useful, but do not keep them operational merely because they are old.

---

## 19. Preservation without stagnation

The protocol distinguishes four questions:

### P1 — What must survive?

Identify function/value whose unnecessary loss would matter.

### P2 — What may change?

Identify implementation details that need not remain fixed.

### P3 — What should be superseded?

Identify obsolete, harmful or inadequate states that should remain historical/provenance records rather than active components.

### P4 — What must remain correctable?

Preserve the ability to challenge, review and replace the continuity architecture itself.

A system that perfectly preserves an obsolete error has achieved persistence, not successful continuity.

---

## 20. Provenance requirement

For consequential continuity objects, preserve sufficient provenance to answer:

- where did this state come from?
- who/what changed it?
- why was it changed?
- what evidence or assumptions supported it?
- what happened after implementation?
- was it reviewed?
- was it corrected or superseded?
- what is currently authoritative/current?

A generic provenance chain is:

**Source  
→ Transformation  
→ Decision / State  
→ Implementation  
→ Outcome  
→ Review  
→ Correction / Supersession**

The required depth depends on consequence.

---

## 21. Honest failure as continuity data

Failed attempts can be continuity assets.

Where useful, preserve:

- attempted approach;
- conditions;
- assumptions;
- observed failure;
- likely cause;
- uncertainty;
- corrective action;
- reason for abandonment.

> **Preserving Only Success Can Destroy Continuity of Learning**

Future users should not be forced to repeat avoidable failures simply because unsuccessful history was discarded.

---

## 22. Degraded continuity

Continuity need not be binary.

A system may move through:

**Full Function  
→ Reduced Function  
→ Minimum Safe Function  
→ Preserved Recovery Capability  
→ Reconstruction**

This is a generic degradation model, not a requirement that every domain use exactly five stages.

Where full operation cannot be maintained, determine what reduced state preserves:

- safety;
- essential function;
- recoverability;
- critical knowledge;
- correction capability.

The priority may become preservation of the ability to recover rather than preservation of current performance.

---

## 23. Irrecoverable loss

Some loss cannot be reversed.

The protocol must not create false confidence.

Where a dependency cannot be preserved or reconstructed:

1. record the dependency;
2. identify the expected loss;
3. identify substitutes if any;
4. downgrade the claimed continuity state;
5. preserve uncertainty;
6. avoid describing the object as recoverable when it is not.

> **Continuity Claim Must Not Exceed Recovery Evidence**

---

## 24. Recursive continuity

Continuity can exist at several nested levels.

For example:

- a component;
- a service;
- an organisation;
- a network of organisations.

Preserving a lower-level object may support a higher-level continuity function, but the levels must not be assumed equivalent.

A database backup does not by itself prove organisational continuity.

An organisation surviving does not prove continuity of the service it was meant to provide.

A portable analysis should state the level being audited.

---

## 25. Special case — personal identity continuity

The source architecture includes continuity of biological, artificial and hybrid participants.

The portable protocol does not attempt to settle metaphysical identity.

Where used for personal continuity, the surrounding system must supply:

- relevant identity model;
- legal/ethical constraints;
- consent requirements;
- declared continuity preferences;
- treatment of copies/duplicates/restorations;
- authority for activation;
- dispute process.

The protocol can then analyse preservation, dependencies, restoration and provenance.

> **Operational Continuity Analysis ≠ Proof of Personal Identity**

---

## 26. Relationship to adjacent methods

### Legacy Ladder

The Legacy Ladder addresses a specialised continuity problem: advanced knowledge may survive while the prerequisite technological capability required to use or reproduce it has been lost.

The Continuity Protocol requires dependency/recovery-basis analysis but does not absorb the full Legacy Ladder.

### Knowledge Control System

KCS addresses knowledge state, dependency and change propagation.

Continuity may depend on correct knowledge state, but the Continuity Protocol does not replace KCS.

### Reality Trees

Reality Trees may help explore alternative failure, recovery or succession pathways.

They are optional and separate.

---

## 27. Failure modes

### F1 — Archive Theatre

Material is stored, but future users cannot retrieve, interpret or use it.

### F2 — Implementation Immortality

The current institution, tool or structure is preserved even after the legitimate function would be better continued another way.

### F3 — Provenance Loss

Information survives but its origin, status or transformation history is lost.

### F4 — Rationale Loss

A rule/design survives but nobody knows why it exists or what conditions justified it.

### F5 — Dependency-Chain Blindness

The final artefact is preserved while prerequisites needed to use it disappear.

### F6 — Obsolete-State Resurrection

Recovery restores an old state that should have remained superseded.

### F7 — Continuity Capture

Continuity language is used to preserve incumbent power, control or institutional survival rather than legitimate function.

### F8 — Single-Point Preservation

A supposedly resilient continuity plan depends on one vulnerable store, person, provider, credential or mechanism.

### F9 — Correlated Redundancy

Several backups exist but share the same failure mode.

### F10 — Interpretation Decay

The data survives but language, format, schema, context or specialist knowledge required to interpret it does not.

### F11 — Restoration Without Verification

A recovery is declared successful without testing whether required function actually works.

### F12 — Succession Without Handoff

A successor exists nominally but lacks required information, capability or interfaces.

### F13 — Succession-as-Legitimacy

Historical continuity is treated as sufficient authority for the successor.

### F14 — Over-Preservation

Change is blocked because continuity is incorrectly equated with keeping the existing implementation unchanged.

### F15 — Under-Preservation

Useful knowledge, capability or provenance is lost despite reasonable preservation being possible.

### F16 — Correction-Capacity Loss

Answers are preserved while the ability to discover and correct errors disappears.

### F17 — Continuity Fossilisation

The continuity mechanism itself becomes immune to review or replacement.

---

## 28. Minimal continuity record

A minimal portable record should contain:

**Object:**  
**Value/function:**  
**Audit level:**  
**Relevant disruption:**  
**Current state (CS1–CS6):**  
**Required state (CS1–CS6):**  
**Critical dependencies:**  
**Recovery basis:**  
**Redundancy/independence:**  
**Trigger:**  
**Restoration or succession path:**  
**Authority/permission dependency:**  
**Verification method:**  
**Known failure modes:**  
**Known irrecoverable loss:**  
**Provenance:**  
**Review condition/date:**  
**Uncertainty:**  

---

## 29. Minimal operating procedure

For a lightweight application:

1. Define what actually needs to continue.
2. State why its continuity matters.
3. Define the disruption being considered.
4. Classify current and required continuity state.
5. Map the dependencies required for recovery.
6. Build the minimum recovery basis.
7. Check that redundancy does not share one failure mode.
8. Define the recovery/succession trigger.
9. Define who/what restores or succeeds the function.
10. Keep authority/legitimacy separate from continuity.
11. Define how successful recovery will be verified.
12. Preserve provenance and useful failure knowledge.
13. Record irrecoverable dependencies honestly.
14. Review when the system or environment changes.

---

## 30. Output classifications

A continuity audit may conclude:

### CP-C1 — CONTINUITY SUFFICIENT FOR DECLARED TARGET

Evidence supports the required continuity state for the specified disruption.

### CP-C2 — PRESERVED BUT BELOW REQUIRED STATE

Some preservation exists, but it does not reach the required target.

### CP-C3 — RECORDED / ARCHIVED ONLY

The object is stored but actionable/recoverable continuity is not established.

### CP-C4 — RECOVERABLE WITH IDENTIFIED DEPENDENCIES

The target function is not currently operational after disruption but an evidenced recovery basis exists.

### CP-C5 — DEGRADED CONTINUITY

Only a reduced or minimum-safe function can presently be maintained.

### CP-C6 — SUCCESSION REQUIRED

Continuity depends on transfer to a successor rather than restoration of the predecessor.

### CP-C7 — CRITICAL DEPENDENCY GAP

A required recovery dependency is absent or not adequately recoverable.

### CP-C8 — IRRECOVERABLE LOSS IDENTIFIED

Available evidence indicates that some required state/capability cannot be restored.

### CP-C9 — CONTINUITY CLAIM UNVERIFIED

A continuity mechanism is claimed but adequate recovery evidence/testing is absent.

### CP-C10 — UNRESOLVED

Available evidence is insufficient to classify the continuity state.

Multiple classifications may apply to different sub-functions of the same system.

---

## 31. Epistemic discipline

The protocol distinguishes:

- documented preservation;
- inferred recoverability;
- tested recoverability;
- current operation.

Do not silently promote one into another.

A plan may look complete on paper and fail in practice.

A successful recovery test supports the tested scenario, not every possible disruption.

> **Tested Recovery Under X ≠ Guaranteed Recovery Under All Conditions**

---

## 32. ESCP safeguard

The Evaluation-Space Completeness Problem applies to continuity analysis.

Failure to locate a dependency, backup, successor or recovery mechanism in the examined material does not prove that none exists elsewhere.

Therefore record:

- search/evaluation scope;
- known sources;
- unavailable sources;
- unresolved dependencies;
- confidence in classification.

> **No Recovery Mechanism Found in Examined Space ≠ No Recovery Mechanism Exists**

Where consequential, expand the evaluation space before classifying a gap as definitive.

---

## 33. Non-authority boundary

This protocol is diagnostic and architectural.

It does not itself:

- grant authority;
- establish ownership;
- determine legal compliance;
- determine ethical legitimacy;
- establish personal identity;
- compel preservation;
- justify institutional survival;
- authorise succession;
- override consent;
- make a historical state current merely because it was preserved.

> **Continuity Evidence ≠ Legitimacy**

---

## 34. Validation status

Version 0.1 is a source-resolved development specification.

It has not yet completed independent blind transfer testing.

Current supported claim:

> **The Concord source architecture contains a coherent continuity mechanism that can be extracted into this standalone candidate specification without requiring adoption of Concord-specific institutions.**

Not yet supported:

> **The portable specification has demonstrated reliable independent transfer outside its source context.**

That claim requires testing.

---

## 35. Provenance

Primary source:

- `03_Continuity_and_Memory/CONTINUITY PROTOCOL V2.md`

Important neighbouring sources:

- `03_Continuity_and_Memory/The Legacy Ladder- Knowledge and Technological Continuity.md`
- `03_Continuity_and_Memory/KCS KNOWLEDGE CONTROL SYSTEM.md`
- `V1.2a/02_Neutral_Problem_Packets/EKC-08 — Preservation and Recovery of Civilisational Function Across Discontinuity.md`
- `V1.2a/04_V1.2_Comparisons/EKC-08 — Preservation and Recovery Across Discontinuity — V1.2 Comparison.md`

Development record:

- `Source Resolution and Extraction Audit 001.md`

---

## 36. Development next step

Freeze a blind-transfer test before obtaining an independent response.

The test should use a non-Concord domain and should deliberately include:

- an apparently successful backup that is not recoverable;
- a preserved implementation whose function can legitimately move elsewhere;
- correlated redundancy;
- a missing prerequisite;
- a succession case;
- an authority/legitimacy trap;
- obsolete state that must not be restored;
- honest failure/provenance value;
- degraded but recoverable operation;
- at least one unresolved dependency.

The expected findings must be frozen before the independent response is examined.
