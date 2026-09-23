# KCS Change Propagation — Source Resolution and Extraction Audit 001

**Development level:** Level B — Extractable Architecture  
**Status:** SOURCE RESOLUTION COMPLETE / EXTRACTION AUTHORISED  
**Date:** 23 September 2026

## 1. Candidate

**KCS Change Propagation**

Candidate function:

> A dependency-aware mechanism for identifying downstream consequences when knowledge, architecture or assumptions change.

The development placeholder identifies the primary source as:

*03_Continuity_and_Memory/KCS Companion Upgrade 001 — Operational Dependency and Change-Propagation Architecture.md*

Initial discovery status: **VERY STRONG EXTRACTION CANDIDATE**.

## 2. Source resolved

Primary source successfully resolved:

**KCS Companion Upgrade 001 — Operational Dependency and Change-Propagation Architecture**

Source metadata:
- Author: Alexander C. Blainey
- Project: The Concord Framework
- Status: CANONICAL COMPANION UPGRADE — CORRIGIBLE / INITIAL OPERATIONAL VERSION
- Parent system: The Concord Knowledge Control System
- Interface architecture: Civilisational Developmental Topology
- Date: September 2026

The source contains a complete operational dependency/change-propagation mechanism rather than merely a conceptual mention.

## 3. Source purpose

The source extends a knowledge-control architecture from recording objects and their epistemic/provenance state into recording material relationships among objects and determining what should be reconsidered when an upstream object changes.

Its central statement is:

> **Record not only what civilisation knows, but the material relationships that determine what must be reconsidered when that knowledge changes.**

The portable mechanism does not require the original civilisational framing.

## 4. Portable problem

The portable problem is:

> **How can a complex evolving system represent material dependencies and identify which downstream objects require reconsideration after an upstream change without automatically invalidating everything downstream or turning the dependency graph into a central authority?**

This problem occurs independently in software, engineering, research, policy/document systems, organisational architecture, infrastructure, data/model pipelines and other dependency-rich systems.

## 5. Core portable principle

> **Record material dependencies with provenance and state; when an upstream object changes, generate a bounded downstream review set rather than automatic invalidation.**

Short form:

> **Change upstream → identify affected dependents → review selectively → propagate further only when downstream state materially changes.**

Critical source distinction:

> **Change(x) → CandidateReview(y)**

not:

> **Change(x) → AutomaticRejection(y)**

## 6. Core data model

Source graph:

**K(t) = <V, R, P, S, H>**

where:
- V = represented objects;
- R = typed material relations;
- P = provenance;
- S = current state;
- H = history/change record.

Dependency record:

**d = <source, target, capability, type, materiality, state, context, evidence, confidence, time>**

Practical source minimum additionally records:
- ID;
- alternatives;
- criticality;
- failure effect;
- first recorded;
- last confirmed;
- next review.

This is sufficiently general for portable extraction.

## 7. Object classes

The source explicitly warns against treating documents as the only dependency objects.

Portable object classes may include:
- functions;
- systems;
- architectures;
- interfaces;
- protocols;
- datasets;
- models;
- software;
- standards;
- rules/provisions;
- evidence bases;
- recovery capabilities;
- external services;
- physical infrastructure;
- represented participant capabilities;
- documents where the document itself is the relevant object.

> **Document May Evidence Dependency ≠ Document Necessarily Is Dependency**

## 8. Relation vocabulary

Initial shared relation types from source:
- DEPENDS_ON
- REQUIRES
- SUPPLIES
- INTERFACES_WITH
- ENABLES
- BLOCKS
- PROPAGATES_TO
- CORRECTS
- REVIEWS
- SUPERSEDES
- ALTERNATIVE_TO
- RECOVERS
- PRESERVES
- EVIDENCES

The source permits domain-specific relations while requiring shared meanings to remain semantically stable.

## 9. Dependency states

Source minimum vocabulary:
- ACTIVE
- SATISFIED
- DEGRADED
- BLOCKING
- FAILED
- ALTERNATIVE_AVAILABLE
- SUPERSEDED
- UNKNOWN
- DISPUTED

Important distinction:

> **Dependency Exists ≠ Dependency Is Blocking**

BLOCKING requires that the current prerequisite state materially prevents or constrains the dependent function.

## 10. Materiality and criticality

Source materiality states:
- CRITICAL
- HIGH
- MODERATE
- LOW
- IMMATERIAL
- UNKNOWN
- DISPUTED

Criticality is context-sensitive and may consider:
- consequence of failure;
- importance/number of dependents;
- alternatives;
- recovery difficulty;
- time sensitivity;
- reversibility;
- correlated exposure.

The source cautions against compressing these dimensions into a single score by default.

## 11. Traversal

For object x:

**Up(x) = objects on which x materially depends**

**Down(x) = objects materially dependent upon x**

Traversal can identify:
- prerequisites;
- affected downstream objects;
- shared upstream bottlenecks;
- suppliers/owners where represented;
- recovery/alternative paths.

But:

> **Traversal ≠ Priority Decision**

## 12. Change events

Consequential change records should preserve:
- object;
- old state;
- new state;
- reason;
- evidence;
- time;
- actor/source.

Candidate events include:
- validation;
- correction;
- supersession;
- deprecation;
- interface change;
- owner/supplier change;
- dependency discovery/removal;
- failure;
- recovery;
- contested status;
- version change.

## 13. Change propagation mechanism

For changed object x:

1. preserve prior state;
2. record the change and provenance;
3. traverse materially dependent downstream relations;
4. evaluate applicability/materiality;
5. generate REVIEW_REQUIRED/CandidateReview states where justified;
6. surface the review through an appropriate external interface;
7. record review outcomes;
8. clear the review state where the dependency remains satisfied;
9. propagate further only where the reviewed downstream object's material state changes.

This is **bounded recursive propagation**.

## 14. Selective stopping and escalation

Propagation should stop where:
- dependency is immaterial;
- unaffected alternative satisfies requirement;
- downstream object is superseded;
- context makes relation non-applicable;
- evidence shows the upstream change does not alter dependent function.

Propagation should escalate where:
- high-consequence functionality depends on the changed object;
- no alternative exists;
- failure may be silent;
- multiple dependents share the prerequisite;
- protected/rights-critical consequences may be affected.

Portable extraction should generalise the final category as high-consequence protected constraints rather than require Concord constitutional architecture.

## 15. Correction propagation

Source sequence:
1. preserve previous state;
2. record correction;
3. identify materially dependent objects;
4. mark REVIEW_REQUIRED where justified;
5. surface review;
6. preserve outcomes;
7. clear flags where dependency remains satisfied;
8. propagate further only where downstream state materially changes.

This is directly portable.

## 16. Supersession propagation

Old objects are not erased.

Represent:

**OldObject — SUPERSEDED_BY → NewObject**

Dependents may be classified:
- COMPATIBLE_WITH_NEW
- MIGRATION_REQUIRED
- REVIEW_REQUIRED
- LEGACY_DEPENDENCY
- UNKNOWN

This preserves history and prevents silent migration assumptions.

## 17. Failure and alternatives

When an object fails, expose where relevant:
- direct dependents;
- critical indirect dependents;
- alternatives;
- recovery owners/suppliers;
- degraded modes;
- unresolved unknowns.

Alternative states:
- FULL
- PARTIAL
- EMERGENCY_ONLY
- DEGRADED
- UNVERIFIED

> **Alternative Label ≠ Proven Equivalence**

## 18. Dependency versus authority

One of the strongest portable boundaries is:

> **Dependency ≠ Subordination**

If A depends on B, B does not thereby gain authority over A.

Likewise:

> **Knowledge State ≠ System Authority**

The dependency layer may record, retrieve, link and flag review requirements. It does not automatically allocate resources, command dependents, adjudicate disputes or set priorities.

## 19. Distributed suppliers/ownership

The source avoids a false single-owner model.

Candidate roles:
- PRIMARY
- CO-OWNER
- DISTRIBUTED_SUPPLIER
- DELEGATED
- INTERFACE_SUPPLIER
- FALLBACK

Portable terminology may prefer **supplier/responsibility role** where “owner” would imply legal ownership.

## 20. Unknown and disputed states

First-class source states include:
- UNKNOWN_OWNER
- UNKNOWN_DEPENDENCY
- UNKNOWN_MATERIALITY
- DISPUTED_DEPENDENCY
- DISPUTED_OWNER
- DISPUTED_EFFECT

Portable invariant:

> **Unknown ≠ Absent**

> **Disputed ≠ False**

This is essential to avoid false graph completeness.

## 21. Freshness

Material dependency records should support:
- first recorded;
- last confirmed;
- last changed;
- next review;
- evidence freshness;
- source/reviewer;
- confidence.

> **Stale ≠ Automatically False**

A stale relation may become REVIEW_OVERDUE without deletion.

## 22. Privacy/security boundary

Dependency maps may reveal:
- infrastructure vulnerabilities;
- privileged interfaces;
- recovery paths;
- single points of failure;
- sensitive participant/system dependencies.

Therefore:

> **Dependency Legibility ≠ Universal Visibility**

Portable extraction must preserve purpose-bounded access and avoid turning dependency mapping into a vulnerability catalogue.

## 23. Anti-centralisation boundary

A dependency graph can look like a commanding system map.

The source explicitly prevents this:

The mechanism may record, preserve, retrieve, link, flag and propagate review requirements.

It does not automatically:
- command systems;
- allocate resources;
- approve changes;
- adjudicate disputes;
- define ethical legitimacy;
- rank persons;
- impose development priority.

This boundary is central to portability.

## 24. Failure modes from source

- dependency hallucination;
- missing dependency;
- stale dependency;
- cascade overload;
- hidden centralisation;
- vulnerability exposure;
- false equivalence of alternatives;
- historical erasure.

Safeguards include provenance, confidence, UNKNOWN, ESCP-style absence discipline, freshness/review, materiality/selective propagation, authority separation, purpose-bounded access, contextual alternative validation and preservation of superseded state.

## 25. Falsification conditions

Reconsider or narrow the portable architecture if:
- dependency records do not improve relevant decisions/reviews;
- maintenance cost exceeds useful value;
- propagation produces mostly irrelevant reviews;
- relation semantics are unstable;
- an existing host system already supplies the capability without benefit from this abstraction;
- mapping creates unacceptable centralisation/security risk;
- source-grounded audits repeatedly contradict graph-derived dependencies.

## 26. Concord-specific dependencies to externalise

The source integrates with:
- Knowledge Control System;
- Civilisational Developmental Topology;
- Civil State Map;
- Civilisation Clock;
- Continuity architecture;
- Active Development;
- Legacy Ladder;
- constitutional/rights architecture.

These are **not required** by the portable core.

Portable replacements:
- **host knowledge/state store** for KCS;
- **object/relation schema** for CDT;
- **external state evaluator** for Civil State Map;
- **external scheduler/prioritiser** for Civilisation Clock;
- **external continuity/recovery system** for Continuity/Legacy Ladder;
- **external change-management workflow** for Active Development;
- **external protected-constraint/authority system** for constitutional/rights architecture.

The portable module should define interfaces without absorbing those systems.

## 27. Candidate portable inputs

Minimum consequential inputs:
- object identifiers;
- typed dependency relations;
- dependency capability/function;
- context;
- materiality/criticality evidence;
- dependency state;
- provenance/evidence;
- confidence/uncertainty;
- alternatives where known;
- freshness/review state;
- a consequential change event.

## 28. Candidate portable outputs

Potential output classes:
- NO_MATERIAL_DOWNSTREAM_EFFECT
- REVIEW_REQUIRED
- REVIEW_OVERDUE
- DEPENDENCY_DEGRADED
- DEPENDENCY_BLOCKING
- DEPENDENCY_FAILED
- MIGRATION_REQUIRED
- LEGACY_DEPENDENCY
- ALTERNATIVE_AVAILABLE
- ALTERNATIVE_UNVERIFIED
- UNKNOWN_DEPENDENCY
- DISPUTED_DEPENDENCY
- UNKNOWN_EFFECT
- PROPAGATION_STOPPED
- PROPAGATION_CONTINUES
- EXTERNAL_ESCALATION_REQUIRED

These should be refined in v0.1 rather than treated as final.

## 29. Candidate portable workflow

**Represent → Change → Traverse → Filter → Review → Update → Propagate-if-material**

Expanded:
1. represent objects and material relations;
2. preserve provenance/state/history;
3. record consequential change;
4. traverse materially relevant downstream relations;
5. filter by applicability, materiality, alternatives and context;
6. create review set rather than automatic invalidation;
7. perform review through the appropriate external process;
8. record outcome;
9. propagate recursively only where downstream material state changes;
10. stop when no further material effect remains.

## 30. Relationship to other portable modules

### Architectural Unit Resolution

AUR helps determine whether an apparent omission belongs locally, elsewhere or at an interface.

KCS Change Propagation assumes a dependency relation has been represented and asks what should be reconsidered when a represented upstream object changes.

> **Unit Resolution ≠ Change Propagation**

### Continuity Protocol

Continuity asks what must survive disruption and what dependencies are necessary for recovery.

KCS Change Propagation can expose dependency and recovery chains but does not itself decide continuity strategy.

> **Dependency Map ≠ Continuity Plan**

### Minimum Necessary Capability

MNC bounds consequential capability to legitimate function.

KCS Change Propagation may expose dependency relationships involving capabilities, but does not determine how much authority/capability an actor should possess.

> **Dependency ≠ Authority**

## 31. Extraction assessment

The primary source is unusually complete for a Level B candidate. It already contains:
- explicit graph/data model;
- relation vocabulary;
- state vocabulary;
- materiality;
- traversal;
- event model;
- bounded propagation;
- correction/supersession/failure logic;
- alternatives;
- distributed suppliers;
- unknown/disputed states;
- freshness;
- security boundaries;
- anti-centralisation;
- failure modes;
- falsification conditions;
- integration boundaries.

No blocking source gap is apparent for producing a standalone v0.1.

The source's own status is canonical companion upgrade but corrigible/initial operational version. Portable extraction must preserve that epistemic history and must not treat extraction as empirical validation.

## 32. Source-resolution conclusion

> **SOURCE RESOLUTION SUFFICIENT FOR PORTABLE EXTRACTION**

> **NO BLOCKING SOURCE OMISSION IDENTIFIED AT THIS STAGE**

> **PORTABLE SPECIFICATION v0.1 AUTHORISED**

## 33. Next step

Create **KCS Change Propagation — Portable Specification v0.1**.

The first specification should preserve:
- typed dependency records;
- materiality and state;
- provenance/confidence/freshness;
- unknown/disputed states;
- upstream/downstream traversal;
- review-set generation rather than automatic invalidation;
- selective propagation stopping/escalation;
- correction, supersession and failure handling;
- alternatives;
- distributed suppliers;
- dependency/authority separation;
- purpose-bounded visibility;
- anti-centralisation;
- explicit external interfaces.

After v0.1, freeze BTT-001 and its expected-findings key before obtaining an independent response.
