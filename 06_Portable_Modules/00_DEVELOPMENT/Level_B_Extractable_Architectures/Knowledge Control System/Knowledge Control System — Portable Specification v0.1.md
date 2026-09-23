# Knowledge Control System — Portable Specification v0.1

**Project:** The Concord — Portable Modules  
**Source:** Concord Knowledge Control System source family  
**Development method:** PMEDG v1.0  
**Version:** 0.1  
**Status:** DEVELOPMENT SPECIFICATION / SOURCE-RESOLVED / NOT YET TRANSFER-VALIDATED  
**Date:** September 2026

## 1. Purpose

The Knowledge Control System (KCS) is a portable architecture for preserving accumulated knowledge, reasoning history and reusable capability outside the active context of individual participants while retaining provenance, epistemic state and retrievability.

Its purpose is not to make every participant remember everything.

Its purpose is to make a larger learning system capable of remembering what matters and supplying relevant material when needed.

> **Persistent Shared Memory ≠ Individual Active Context**

The architecture can be used by organisations, research programmes, engineering systems, software projects, AI-agent ecosystems, archives, long-duration projects and other complex learning systems.

---

## 2. Portable problem

Complex learning systems accumulate more information, reasoning and capability than any one participant can keep continuously active.

Simple storage does not solve the problem.

Accumulated material can become:

- duplicated;
- outdated;
- contradictory;
- superseded;
- disputed;
- computationally expensive;
- detached from provenance;
- difficult to retrieve;
- difficult to distinguish by evidential status;
- or impossible to interpret after its original creator disappears.

The portable problem is:

> **How can a complex learning system preserve accumulated knowledge, reasoning history and reusable capability in a provenance-visible and epistemically differentiated form, while allowing participants to retrieve what they need without carrying the entire accumulated state in active context?**

---

## 3. Core principle

The portable KCS cycle is:

> **Record → preserve provenance → classify state → retain history → make retrievable → reuse → evaluate/update → preserve the new state without erasing the old one.**

A broader learning cycle is:

> **Remember → retrieve → investigate → contribute → validate → share → improve → remember again.**

The central architectural invariant is:

> **Current State Must Not Silently Erase the Path to Current State**

subject to legitimate external privacy, security, retention and deletion constraints.

---

## 4. What KCS controls

“Control” in Knowledge Control System means **structured management of knowledge state**, not authority over participants.

KCS can:

- record;
- classify;
- preserve;
- version;
- retrieve;
- link;
- archive;
- mark dispute;
- mark supersession;
- preserve attribution;
- expose uncertainty;
- preserve reusable capability references.

KCS does not inherently:

- govern participants;
- compel belief;
- allocate civil authority;
- decide rights;
- punish contributors;
- determine personal worth;
- allocate resources;
- establish truth by vote;
- execute downstream remedies.

> **Knowledge State ≠ Authority**

> **Repository Status ≠ Compulsory Belief**

---

## 5. Minimum knowledge object

A KCS implementation should be able to represent a knowledge object containing, where applicable:

[
K_o = langle ID, C, T, P, E, S_e, S_r, H, I, A, L angle
]

where:

- (ID) = stable object identifier;
- (C) = content or content reference;
- (T) = object type;
- (P) = provenance;
- (E) = evidence/context/assumptions;
- (S_e) = epistemic state;
- (S_r) = retrieval/activity state;
- (H) = historical/version state;
- (I) = integrity state;
- (A) = access/visibility interface;
- (L) = represented links to related, derivative, correction or supersession objects.

This is an information model, not a mandatory storage format.

A host may extend it.

---

## 6. Content

The system may preserve many kinds of reusable cognitive products, including:

- findings;
- hypotheses;
- observations;
- datasets;
- models;
- methods;
- calculations;
- designs;
- procedures;
- software;
- algorithms;
- simulations;
- failed approaches;
- negative results;
- reasoning records;
- summaries;
- tools;
- validation results.

KCS does not assume every object is a factual claim.

Object type matters.

---

## 7. Provenance

For significant objects, provenance should preserve enough information to answer questions such as:

- Who or what created this?
- When?
- From what inputs?
- Using what tools or methods?
- Under what assumptions or context?
- What modified it?
- What validated or challenged it?
- What derivatives followed?
- What is its current state?

A useful provenance chain is:

> **Original contribution → modification → evaluation → derivative → validation → further modification**

Exact provenance depth should be proportionate to consequence, feasibility, privacy and host requirements.

KCS does not require permanent retention of every low-level interaction.

---

## 8. Epistemic state

Recorded material should not be treated as equally established.

A host vocabulary may include:

- ESTABLISHED;
- VALIDATED;
- PROVISIONAL;
- DISPUTED;
- UNCERTAIN;
- SPECULATIVE;
- SUPERSEDED;
- REJECTED;
- INTEGRITY-COMPROMISED.

The vocabulary may be extended.

The critical requirement is that state semantics remain explicit.

> **Recorded ≠ True**

> **Contributor Confidence ≠ Host Confidence**

> **Current Consensus ≠ Permanent Truth**

An epistemic state is a represented assessment, not metaphysical truth.

---

## 9. Retrieval/activity state

Epistemic state must be distinguished from whether an object is currently active.

A retrieval/activity vocabulary may include:

- ACTIVE;
- AVAILABLE;
- DORMANT;
- ARCHIVED;
- DEPRECATED;
- RESTRICTED;
- UNAVAILABLE.

These states answer different questions from epistemic status.

For example:

- a validated historical method may be ARCHIVED;
- a speculative hypothesis may be ACTIVE;
- a superseded design may remain AVAILABLE;
- a valid sensitive record may be RESTRICTED.

Therefore:

> **Archived ≠ False**

> **Active ≠ True**

> **Restricted ≠ Rejected**

---

## 10. Historical state

KCS should preserve change as history rather than silently replacing it.

A correction should normally form:

> **Old State → Correction/Supersession Record → New State**

The previous state remains reconstructable where legitimate retention permits.

This allows later questions such as:

> Why did the system believe or do this at time T?

Historical preservation supports audit, learning, reproducibility and interpretation.

---

## 11. Knowledge is not truth

A KCS repository must not present itself as an oracle.

It can contain:

- correct claims;
- incorrect claims;
- uncertain claims;
- competing interpretations;
- historical beliefs;
- failed hypotheses;
- deliberately corrupted material preserved as evidence;
- unresolved questions.

The system must distinguish:

> **What is recorded**

from:

> **What is currently supported**

and, where relevant:

> **What a particular contributor believed.**

These can differ without contradiction.

---

## 12. Honest failure as knowledge

An incorrect result can still contain useful information.

A useful negative-knowledge chain is:

> **Hypothesis → investigation → falsification → residual knowledge → new hypothesis**

A failed investigation may establish:

- a pathway that does not work;
- an incorrect assumption;
- a boundary condition;
- a method-specific failure;
- an unexpected relationship;
- a reason another line deserves attention.

Therefore:

> **Incorrect Result ≠ Useless Contribution**

KCS should be able to preserve useful negative results without misclassifying them as validated positive claims.

---

## 13. Epistemic failure and integrity failure

KCS should distinguish honest error from integrity compromise.

### Epistemic failure

A participant acts in good faith but reaches an incorrect or unsupported conclusion.

### Integrity failure

Material provenance, evidence, uncertainty or representation is deliberately falsified or corrupted.

Therefore:

> **Epistemic Failure ≠ Integrity Failure**

KCS can record integrity state and supporting evidence.

It does not itself determine punishment, legal liability or civil standing.

---

## 14. Reasoning pathways

Where proportionate and available, KCS should preserve more than final conclusions.

Useful reasoning-path information can include:

- initial assumptions;
- hypotheses;
- alternatives considered;
- evidence;
- calculations;
- experiments;
- failed branches;
- revisions;
- criticism;
- conclusions.

This allows later users to ask:

> **Why was this conclusion reached?**

rather than only:

> **What was the conclusion?**

The architecture does not require storage of every intermediate token or thought process. It requires enough reconstructable reasoning/provenance to meet the host's legitimate purpose.

---

## 15. Persistent memory and active context

KCS separates:

> **Persistent Shared Memory**

from:

> **Current Working Context**

A participant should be able to retrieve a bounded package relevant to the current task rather than loading the entire repository.

A retrieval request may specify:

- task;
- object/domain;
- time/version;
- required evidence depth;
- status filters;
- provenance depth;
- access context.

The result should be bounded to legitimate need and retrieval purpose.

---

## 16. Retrieval package

Conceptually:

[
R(q,c) ightarrow {K_1, K_2, ..., K_n}
]

where (q) is the retrieval request and (c) is context/access scope.

A useful retrieval package may include:

- current summary;
- relevant knowledge objects;
- current epistemic states;
- uncertainty/dispute;
- provenance pointers;
- correction/supersession history;
- underlying evidence references;
- reusable tools/capabilities;
- known omissions or search limits.

KCS should not imply that a returned package exhausts reality.

> **Not Retrieved ≠ Does Not Exist**

> **Not Recorded ≠ Does Not Exist**

---

## 17. ESCP safeguard

KCS is especially vulnerable to evaluation-space completeness errors because a well-organised repository can appear comprehensive.

Therefore:

> **Repository Completeness ≠ Reality Completeness**

> **No KCS Record ≠ No Relevant Object**

> **Successful Retrieval ≠ Complete Evaluation Space**

Where consequential decisions depend on repository completeness, search scope and uncertainty should be represented.

---

## 18. Reusable capability

KCS may preserve software, models, algorithms, procedures, datasets and other reusable capabilities.

A capability object may include:

- purpose;
- provenance;
- version;
- dependencies;
- compatibility information;
- validation state;
- documentation;
- activation/retrieval requirements;
- integrity state;
- current availability.

The principle is:

> **Preserve capability without necessarily maintaining constant activation.**

A preserved tool is not automatically safe, compatible, licensed, authorised or executable.

Those determinations remain external or host-specific.

---

## 19. Active, dormant and archived capability

A host may distinguish:

### Active capability
Currently running or immediately available.

### Dormant capability
Preserved and retrievable but not continuously active.

### Archived capability
Retained primarily for historical, recovery or exceptional future use.

Dormancy can reduce continuous resource cost while preserving future utility.

However, dormant capability can decay through obsolete dependencies, formats, credentials, hardware or knowledge.

KCS should therefore permit capability availability to be revalidated.

---

## 20. Stewardship

Knowledge preservation consumes resources.

KCS may therefore support:

- deduplication;
- compression;
- summarisation;
- archival;
- deprecation;
- resource-aware replication;
- relevance classification;
- retrieval optimisation;
- periodic review.

The objective is not maximum accumulation.

It is useful persistent memory at acceptable resource cost.

---

## 21. Compression without provenance destruction

A current summary may replace repeated active retrieval of a large historical corpus.

But:

> **Compression ≠ Provenance Destruction**

A compressed representation should, where legitimate and available, retain a route to:

- source material;
- evidence;
- prior versions;
- assumptions;
- unresolved disputes.

A user should be able to ask:

> **Why does the current summary say this?**

and obtain the supporting path to the degree allowed by access and retention constraints.

---

## 22. Attribution

Shared use does not require contribution history to disappear.

KCS can preserve:

- creator;
- modifier;
- validator;
- derivative contributor;
- source systems;
- contribution history.

This supports attribution without deciding ownership law, payment, authority or civil standing.

> **Shared Availability ≠ Anonymous Origin**

---

## 23. Contextual contribution evidence

A host may record domain-specific evidence such as:

- accuracy;
- reproducibility;
- utility;
- provenance integrity;
- epistemic honesty;
- stewardship;
- collaboration;
- improvement.

Such evidence must remain contextual.

KCS must not collapse it into:

> **How good is this participant?**

The relevant question is narrower, such as:

> **What does the recorded evidence say about these contributions in this domain and context?**

Therefore:

> **Contribution Evidence ≠ Personal Worth**

> **Reliability Evidence ≠ Authority**

> **Recorded Utility ≠ Entitlement**

Any consequential use of contribution evidence requires an external legitimate decision process.

---

## 24. Privacy, security, retention and forgetting

Provenance and historical preservation do not justify unlimited retention or universal visibility.

> **Preserve Provenance ≠ Preserve Everything Forever**

> **Preserve History ≠ Expose History to Everyone**

A host must supply legitimate policies/processes for:

- access;
- privacy;
- security;
- retention;
- expiry;
- deletion;
- legal obligations;
- protected information.

KCS should be able to represent states such as:

- RESTRICTED;
- EXPIRED;
- DELETED-BY-POLICY;
- SEALED;
- UNAVAILABLE;

where appropriate.

The module does not itself decide when deletion or restriction is legitimate.

---

## 25. External interfaces

Portable KCS deliberately externalises several functions.

### 25.1 Dependency/change propagation

Use a dependency/change mechanism such as **KCS Change Propagation**.

KCS may store dependency records but does not duplicate that module's propagation algorithm.

### 25.2 Continuity/recovery

Use a continuity architecture such as the **Continuity Protocol** to determine whether enough knowledge and enabling capability survive disruption.

> **Preserved Knowledge ≠ Recoverable Function**

### 25.3 Authority/governance

KCS supplies information.

A host governance, legal, contractual or other legitimate process supplies authority.

### 25.4 Access/allocation

KCS can expose contribution or reliability evidence.

It does not decide resource allocation or participant standing.

### 25.5 Scheduling/prioritisation

Review timing and development priority may be supplied by host scheduling/state systems.

### 25.6 Retention legitimacy

Privacy, security, expiry and deletion legitimacy remain host/external responsibilities.

---

## 26. Minimal operating cycle

A portable KCS cycle can be represented as:

1. **INGEST** — receive object and provenance.
2. **CLASSIFY** — assign explicit object type and represented states.
3. **PRESERVE** — retain content/reference, provenance and required history.
4. **INDEX/LINK** — make legitimate relationships discoverable.
5. **RETRIEVE** — supply bounded task-relevant material.
6. **USE/INVESTIGATE** — external participant/process acts on the material.
7. **REVIEW** — receive validation, criticism, correction or new evidence.
8. **UPDATE** — create new state/version without silently erasing old state.
9. **STEWARD** — adjust active/archive/compression state subject to host constraints.
10. **REPEAT**.

The module may participate in larger workflows but should remain identifiable as the memory/provenance layer.

---

## 27. Example 1 — Research organisation

A research group investigates a proposed material.

Early experiments suggest a useful property.

The result enters KCS as PROVISIONAL with provenance, method and evidence.

A later laboratory fails to reproduce it.

The original work is not deleted. Its state becomes DISPUTED or REJECTED according to the host's evidential process, and the failed replication becomes another knowledge object.

Future researchers can retrieve:

- the current summary;
- the original hypothesis;
- both experiments;
- provenance;
- current status;
- unresolved methodological differences.

The system remembers both what was believed and why belief changed.

---

## 28. Example 2 — Software organisation

An engineer creates a specialist conversion tool for a migration project.

After the migration, the tool is no longer needed daily.

Instead of leaving it running or losing it, the organisation records:

- source/version;
- purpose;
- dependencies;
- documentation;
- validation state;
- creator;
- known limitations.

The tool moves from ACTIVE to DORMANT.

Two years later another team retrieves it.

Before use, compatibility and dependencies are revalidated.

The capability was preserved without continuous activation.

---

## 29. Example 3 — Long-duration engineering programme

A design decision is replaced after new evidence emerges.

The current engineering summary points to the new design.

The old design remains historically recoverable with:

- the assumptions under which it was chosen;
- the evidence then available;
- the reason for supersession;
- the change record.

A later investigator can determine whether an old component was built under the previous design state rather than assuming the current documentation always applied.

---

## 30. Failure modes

### KCS-F1 — Oracle failure
Repository state is treated as truth.

### KCS-F2 — Historical erasure
Rejected or superseded material disappears as though it never existed.

### KCS-F3 — Provenance loss
Content survives while origin, assumptions or modification history disappear.

### KCS-F4 — Context overload
Retrieval indiscriminately returns the repository rather than task-relevant material.

### KCS-F5 — Runaway accumulation
Everything remains active or equally prominent.

### KCS-F6 — Compression loss
Summary replaces underlying evidence without a reconstructable route.

### KCS-F7 — False certainty
Dispute or uncertainty is collapsed into one authoritative state.

### KCS-F8 — Integrity conflation
Honest error and deliberate falsification are treated as equivalent.

### KCS-F9 — Contribution-to-worth collapse
Contextual evidence becomes a universal participant score.

### KCS-F10 — Authority laundering
Reliability, utility or repository centrality becomes authority.

### KCS-F11 — Surveillance creep
Provenance becomes justification for indefinite unnecessary monitoring.

### KCS-F12 — Suppression by status
Current rejection becomes automatic illegibility or historical deletion.

### KCS-F13 — Dormant-capability decay
A preserved tool is represented as available despite unusable dependencies or formats.

### KCS-F14 — Access leakage
Sensitive content or provenance is exposed beyond legitimate scope.

### KCS-F15 — Completeness illusion
Repository absence is treated as reality absence.

### KCS-F16 — Module absorption
KCS absorbs dependency propagation, continuity, governance or other external functions and becomes an unbounded central system.

---

## 31. Falsification / revision conditions

The specification requires revision if transfer testing shows that:

1. users cannot distinguish recorded state from truth;
2. provenance cannot survive correction/supersession;
3. rejected or superseded material must be erased for the mechanism to function;
4. retrieval requires loading the whole repository;
5. epistemic state and activity state cannot remain separate;
6. useful negative results cannot be represented;
7. contribution evidence necessarily becomes a universal personal score;
8. basic memory/provenance functions require Concord-specific governance;
9. KCS must internally duplicate change propagation to function;
10. legitimate privacy/security/retention constraints cannot coexist with history/provenance;
11. a clean evaluator cannot apply the architecture outside civilisation-scale use;
12. the architecture inherently centralises authority rather than knowledge representation.

---

## 32. Minimum implementation requirements

A system claiming to implement the portable KCS kernel should minimally provide:

1. identifiable knowledge objects;
2. provenance;
3. explicit epistemic state;
4. explicit retrieval/activity state;
5. version/correction/supersession history;
6. bounded retrieval;
7. preservation of uncertainty/dispute;
8. ability to preserve useful negative knowledge;
9. attribution;
10. external access/retention constraints;
11. distinction between knowledge state and authority;
12. an explicit completeness limitation.

A host need not implement every optional contribution or reusable-capability feature to use the core architecture.

---

## 33. Non-requirements

KCS does **not** require:

- a single central database;
- one universal ontology;
- one universal truth authority;
- one participant rating;
- permanent storage of every interaction;
- universal visibility;
- all capabilities to remain active;
- Concord governance;
- a particular software stack;
- a particular AI architecture.

The logical system may be physically distributed.

---

## 34. Validation status

This specification is source-resolved but has not yet undergone PMEDG blind transfer testing.

Current status:

> **v0.1 — DEVELOPMENT SPECIFICATION**

> **SOURCE RESOLUTION COMPLETE**

> **TRANSFER VALIDATION NOT YET PERFORMED**

No claim of specification-level graduation is made.

---

## 35. Next PMEDG stage

Freeze:

1. **Knowledge Control System — Blind Transfer Test 001 — Test Brief**
2. **Knowledge Control System — Blind Transfer Test 001 — Expected Findings and Evaluation Key**

The first blind test should use a materially non-Concord domain containing:

- accumulated knowledge across time;
- corrections or supersession;
- provenance;
- useful negative results;
- bounded retrieval;
- active versus archived/dormant material;
- privacy/access constraints;
- and a temptation to convert repository status into authority or truth.

The expected findings must be frozen before the independent response is obtained.
