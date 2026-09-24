# Knowledge Control System — Source Resolution and Extraction Audit 001

**Candidate:** Knowledge Control System (KCS)  
**Development level:** Level B — Extractable Architecture  
**Method:** PMEDG v1.0  
**Status:** SOURCE RESOLUTION COMPLETE / PORTABLE EXTRACTION AUTHORISED  
**Date:** September 2026

## 1. Audit purpose

This audit determines whether the Concord Knowledge Control System contains a coherent reusable architecture that can be extracted as a standalone portable module, what source material legitimately belongs to that extraction, and which later KCS developments should remain separate modules or external interfaces.

This is the first candidate developed explicitly under **Portable Module Extraction, Development and Graduation Method — PMEDG v1.0**.

## 2. Primary source

Primary source:

**03_Continuity_and_Memory/KCS KNOWLEDGE CONTROL SYSTEM.md**

The source defines KCS as an architecture for externalised shared memory rather than a larger undifferentiated database.

Its central problem is:

> How can accumulated intelligence be preserved, shared and reused without requiring every participant to retain the entire accumulated state?

Its central closing principle is:

> **A civilisation should not require every intelligence to remember everything. It should make civilisation itself capable of remembering.**

Although written in civilisational terms, the underlying problem is not intrinsically Concord-specific.

## 3. Source-family resolution

Repository history and later V1.2a operationalisation show that KCS subsequently acquired additional machinery, particularly:

- KCS Companion Upgrade 001 — operational dependency and change-propagation architecture;
- KCS Material Dependency Index (KMDI);
- operational dependency datasets;
- interfaces into the Civil State Map and Civilisation Clock.

These later materials confirm that KCS became operational infrastructure inside Concord.

However, they do **not** all belong inside the portable KCS extraction.

The dependency/change-propagation mechanism has already been independently extracted and graduated as:

**KCS Change Propagation — Portable Module v1.0**

Therefore:

> **KCS Source Family ≠ One Portable Module**

and:

> **Presence inside KCS ≠ Ownership by the general KCS portable package**

The general KCS extraction must preserve an interface to dependency/change management where needed without duplicating the already-graduated KCS Change Propagation module.

## 4. Source architecture

The primary KCS paper contains several interacting architectural functions.

### 4.1 Externalised memory

The system preserves accumulated knowledge outside the active context of individual participants.

This separates:

**Shared persistent memory**

from:

**Individual active context**

The architecture therefore does not require every participant to carry everything continuously.

### 4.2 Knowledge-state representation

Recorded material can occupy distinguishable states including:

- ACTIVE;
- AVAILABLE;
- ARCHIVED;
- PROVISIONAL;
- DISPUTED;
- SUPERSEDED;
- REJECTED;
- INTEGRITY-COMPROMISED.

The state concerns the current treatment of the represented material, not metaphysical truth.

### 4.3 Provenance

Significant contributions preserve information about origin, inputs, tools, modifications, validation, derivative works and current status.

### 4.4 Historical preservation

Superseded or rejected material is not silently transformed into “never existed.”

The system preserves the path by which understanding changed.

### 4.5 Reasoning-path preservation

Where proportionate, the architecture retains assumptions, alternatives, evidence, calculations, experiments, failed approaches, revisions, conclusions and criticism rather than only final answers.

### 4.6 Honest negative knowledge

A falsified hypothesis or failed investigation can remain useful when it narrows possibility space or exposes a boundary, failure mode or incorrect assumption.

### 4.7 Integrity distinction

Incorrect good-faith work is distinguished from deliberate falsification, concealed uncertainty or corrupted provenance.

### 4.8 Reusable capability

Software, algorithms, models, datasets, procedures and specialised tools can be preserved for later retrieval rather than remaining tied to the originating participant.

### 4.9 Active/dormant/archive distinction

Useful capability need not remain continuously active.

The architecture separates active capability from dormant retrievable capability and historical/exceptional archival capability.

### 4.10 Retrieval rather than total retention

Consumers retrieve what is relevant to the current task rather than ingesting the complete repository.

### 4.11 Stewardship and compression

The architecture recognises storage, indexing, retrieval, replication and processing costs.

It therefore permits deduplication, compression, summarisation, archival, deprecation and review while retaining links to underlying provenance.

### 4.12 Attribution

Shared availability does not require erasure of the contributor or contribution history.

### 4.13 Contextual contribution evidence

The source discusses contextual, multidimensional evidence about contribution reliability and utility while explicitly rejecting a universal measure of personal worth.

This is present in the source architecture but requires careful portability treatment because contribution recognition, resource access and participant induction depend on external institutional legitimacy.

## 5. Portable problem

The portable problem can be stated as:

> **How can a complex learning system preserve accumulated knowledge, reasoning history and reusable capability in a provenance-visible and epistemically differentiated form, while allowing participants to retrieve what they need without carrying the entire accumulated state in active context?**

This applies beyond civilisation-scale systems.

Potential hosts include:

- research organisations;
- engineering programmes;
- software organisations;
- long-duration projects;
- institutional knowledge systems;
- AI-agent ecosystems;
- distributed technical communities;
- archives with active knowledge-state management;
- other complex learning systems.

## 6. Candidate portable kernel

The portable kernel is:

> **Record → preserve provenance → classify epistemic/operational state → retain history → make retrievable → reuse → evaluate/update → preserve the new state without erasing the old one.**

A compact memory cycle is:

> **Remember → retrieve → investigate → contribute → validate → share → improve → remember again.**

The kernel requires a distinction between:

1. content;
2. provenance;
3. epistemic/operational status;
4. history;
5. retrieval state;
6. reusable capability where applicable.

## 7. Minimum knowledge object

A portable KCS object should minimally be able to represent:

- object ID;
- content or content reference;
- object type;
- creator/source;
- creation time/version;
- provenance;
- assumptions/context where material;
- evidence references;
- current epistemic status;
- confidence/uncertainty where applicable;
- modification history;
- validation/review history;
- supersession/correction links;
- retrieval/activity state;
- integrity state;
- access/visibility interface;
- derivative/related objects where represented.

The exact schema is implementation-specific.

## 8. State families

The source mixes epistemic status and storage/activity state. Portability should preserve both while avoiding false equivalence.

### 8.1 Epistemic status

Examples:

- ESTABLISHED / VALIDATED;
- PROVISIONAL;
- DISPUTED;
- UNCERTAIN;
- SUPERSEDED;
- REJECTED;
- SPECULATIVE;
- INTEGRITY-COMPROMISED.

### 8.2 Retrieval/activity status

Examples:

- ACTIVE;
- AVAILABLE;
- DORMANT;
- ARCHIVED;
- DEPRECATED.

These dimensions may coexist.

> **Archived ≠ False**

> **Active ≠ True**

> **Rejected ≠ Erased**

> **Superseded ≠ Never Existed**

## 9. Knowledge is not truth

The portable architecture must preserve the source distinction between:

> **what has been recorded**

and:

> **what is currently believed to be true.**

A repository is not an oracle.

A high-confidence contributor statement does not automatically become high-confidence host knowledge.

Likewise, current consensus must remain revisable.

## 10. Provenance and history invariant

The strongest portable invariant is:

> **Current State Must Not Erase the Path to Current State**

Corrections and supersessions should normally be additive/versioned.

Where storage or privacy requirements justify deletion or restricted retention, the decision belongs to an external legitimate retention/access process rather than being silently inferred from epistemic status.

## 11. Honest failure

The source supports a reusable distinction:

> **Incorrect Result ≠ Useless Contribution**

and:

> **Epistemic Failure ≠ Integrity Failure**

A failed hypothesis may still preserve useful negative knowledge.

Deliberate falsification, provenance corruption or concealed uncertainty is a different class of problem.

KCS records this distinction; it does not itself adjudicate misconduct or punishment.

## 12. Active context and persistent memory

A key portable separation is:

> **Persistent Shared Memory ≠ Active Working Context**

A consumer should be able to retrieve bounded material relevant to a current task.

The architecture therefore supports externalised memory without requiring universal active retention.

## 13. Capability preservation

Reusable code, models, procedures and tools can be treated as knowledge/capability objects.

The portable principle is:

> **Preserve capability without necessarily maintaining constant activation.**

Whether a preserved tool is safe, licensed, executable, compatible or authorised for use remains an external determination.

## 14. Stewardship

The portable architecture may support:

- deduplication;
- compression;
- summarisation;
- archival;
- deprecation;
- retrieval optimisation;
- resource-aware replication;
- periodic review.

However:

> **Compression ≠ Provenance Destruction**

A compressed current representation should retain sufficient links to underlying evidence/history where legitimate and available.

## 15. Contribution and recognition boundary

The source includes contribution recognition and possible reciprocal access.

The portable kernel can preserve:

- attribution;
- domain-specific contribution evidence;
- reliability history;
- utility evidence;
- reproducibility evidence;
- provenance integrity.

But the following are external:

- personal worth;
- civil standing;
- rights;
- punishment;
- general social credit;
- entitlement to authority;
- entitlement to resources;
- access decisions not already justified by a host process.

Therefore:

> **Contribution Evidence ≠ Personal Worth**

> **Reliability Evidence ≠ Authority**

> **Attribution ≠ Ownership of Shared Truth**

> **Recorded Utility ≠ Entitlement**

Any host using contribution evidence for consequential access or allocation requires its own legitimate decision architecture.

## 16. Concord-specific dependencies to externalise

The primary paper links KCS to Concord-specific systems.

For portability these become generic interfaces.

### Concord constitutional/ethical system
Portable interface: host legitimacy, rights, privacy, consent and protected constraints.

### Concord Induction Protocol
Portable interface: onboarding/access process.

### Civilisation Clock
Portable interface: scheduling, prioritisation and review timing.

### Civil State Map
Portable interface: external state/maturity synthesis.

### Concord contribution/resource systems
Portable interface: recognition, access or allocation process.

### KCS Change Propagation/KMDI
Portable interface: dependency-aware change review.

The KCS portable module should not recreate these systems.

## 17. Boundary with KCS Change Propagation

KCS may store:

- dependency records;
- correction links;
- supersession links;
- review state.

But the already-graduated **KCS Change Propagation** module owns the reusable mechanism for:

> **When one represented object changes, what materially depends on it and how far should review propagate?**

General KCS instead owns:

> **What should be preserved, in what state, with what provenance/history, and how should it remain retrievable and reusable?**

This separation prevents duplicate ownership.

## 18. Boundary with Continuity Protocol

KCS preserves knowledge and reusable capability.

The **Continuity Protocol** addresses whether enough function, knowledge and enabling dependencies survive disruption for legitimate recovery.

Therefore:

> **Preserved Knowledge ≠ Recoverable Function**

KCS can supply continuity inputs without replacing continuity architecture.

## 19. Boundary with ESCP

KCS can preserve uncertainty, provenance and known search scope.

It cannot prove that its repository contains every decision-relevant object.

Therefore:

> **Not Found in KCS ≠ Does Not Exist**

> **Recorded Knowledge ≠ Complete Evaluation Space**

ESCP remains a governing evaluation safeguard.

## 20. Boundary with authority and governance

KCS records, preserves, retrieves, classifies and links knowledge.

It does not inherently:

- govern participants;
- allocate civil authority;
- decide rights;
- determine punishment;
- define personal worth;
- compel belief;
- establish truth by consensus;
- suppress unpopular claims merely because they are unpopular.

> **Knowledge State ≠ Authority**

> **Repository Status ≠ Compulsory Belief**

## 21. Security, privacy and forgetting

The source strongly emphasises preservation but also warns against surveillance and suppression.

Later Concord development identifies deep-time forgetting/privacy as a separate underdeveloped area.

Therefore the portable KCS must not infer:

> **Preserve Provenance → Preserve Everything Forever and Expose It to Everyone**

Instead:

> **Preservation Requirement Is Bounded by Legitimate Retention, Privacy, Security and Access Constraints**

KCS should represent restricted, expired, deleted-by-legitimate-policy or unavailable states where host architecture requires them, without pretending inaccessible information never existed when a lawful metadata trace may legitimately remain.

The exact retention/deletion rules are external.

## 22. Dependency/change operationalisation evidence

Later Concord work operationalised KCS dependency records and demonstrated that explicit records could support bounded downstream review and State Map integration.

This is useful evidence that the wider KCS concept can support machine/human operational records.

However, because that mechanism has been extracted separately as KCS Change Propagation, those operational datasets are **supporting source-family evidence**, not part of the general KCS portable kernel.

## 23. Candidate inputs

A portable implementation requires:

- objects/content or references;
- provenance information;
- host-defined object types;
- epistemic/status evidence;
- update/correction events;
- retention/access constraints;
- retrieval requests;
- validation/review outcomes where available.

Optional inputs include contribution evidence, dependency records and capability metadata.

## 24. Candidate outputs

Potential outputs include:

- current knowledge object;
- provenance chain;
- historical versions;
- epistemic state;
- uncertainty/status;
- retrieval package;
- supersession/correction chain;
- reusable capability reference;
- integrity warning;
- attribution record;
- unresolved/disputed state.

KCS outputs information.

It does not automatically convert outputs into governance decisions.

## 25. Candidate failure modes

The portable specification should explicitly address at least:

1. **Oracle failure** — repository status treated as truth.
2. **Historical erasure** — rejected/superseded material silently removed from intellectual history.
3. **Provenance loss** — content survives while origin/assumptions/modification history disappears.
4. **Context overload** — external memory is defeated by indiscriminate retrieval.
5. **Runaway accumulation** — everything remains active or equally prominent.
6. **Compression loss** — summaries sever the route to underlying evidence/history.
7. **False certainty** — uncertainty/dispute collapsed into a single authoritative state.
8. **Integrity conflation** — honest error treated like deception, or deception treated like ordinary error.
9. **Contribution-to-worth collapse** — contextual contribution evidence becomes a universal rating of persons.
10. **Authority laundering** — reliability/utility evidence becomes power.
11. **Surveillance creep** — provenance becomes justification for indefinite monitoring.
12. **Suppression by status** — unpopular or rejected material becomes inaccessible merely because current consensus rejects it.
13. **Dormant-capability decay** — preserved tools become unusable while still represented as available.
14. **Access leakage** — sensitive provenance/content exposed beyond legitimate need.
15. **Completeness illusion** — repository absence treated as reality absence.
16. **Module duplication** — KCS absorbs change propagation, continuity, governance or other neighbouring functions instead of interfacing with them.

## 26. Candidate falsification conditions

The portable architecture requires revision if, in transfer testing:

- users cannot distinguish recorded state from truth;
- provenance cannot survive correction/supersession;
- rejected/superseded material must be erased for the mechanism to function;
- retrieval requires loading the whole repository;
- active/archive status becomes inseparable from epistemic status;
- honest negative results cannot be represented without treating them as worthless;
- contribution evidence necessarily becomes a universal personal score;
- the module requires Concord-specific governance to perform basic memory/provenance functions;
- dependency propagation must be reimplemented internally rather than interfaced;
- legitimate privacy/security/retention constraints cannot coexist with provenance/history;
- a clean evaluator cannot apply the architecture outside a civilisation-scale setting.

## 27. Extraction decision

The source architecture contains a coherent portable core.

The source family is sufficiently resolved to distinguish the general memory/provenance architecture from later specialised KCS mechanisms.

No blocking source omission has been identified for the present extraction stage.

> **SOURCE RESOLUTION SUFFICIENT FOR PORTABLE EXTRACTION**

> **GENERAL KCS AND KCS CHANGE PROPAGATION ARE DISTINCT PORTABLE OWNERS**

> **NO BLOCKING SOURCE OMISSION IDENTIFIED AT THIS STAGE**

> **PORTABLE SPECIFICATION v0.1 AUTHORISED**

## 28. Next step

Create:

**Knowledge Control System — Portable Specification v0.1**

The specification should focus on:

> **externalised memory + epistemic state + provenance + history + bounded retrieval + reusable capability + stewardship**

while keeping dependency propagation, continuity, authority, retention legitimacy and consequential access/allocation as explicit external interfaces.
