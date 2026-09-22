# KMDI-001A — Frozen Requirements for the KCS Material Dependency Index

**Status:** V1.2a SECOND BOTTLENECK / PRE-DEVELOPMENT FREEZE  
**Date:** September 2026  
**External knowledge state:** INTERNAL ONLY  
**Canonical effect:** NONE  
**Parent:** KCS Dependency Capability Source Test 001

# 1. Purpose

Freeze the requirements for the minimum KCS extension before designing it.

The proposed capability is not a new knowledge system. It is an integration layer inside the existing Knowledge Control System that makes material dependencies reusable across civil systems.

# 2. Core Requirement

> The KCS should be able to record, retrieve and update provenance-aware material dependency relations among knowledge objects, capabilities and architectures so that legitimate downstream systems can identify relevant prerequisites and review consequences when upstream state changes.

# 3. Frozen Requirements

K1 — **Material Relation**
Represent that object/capability/architecture A materially depends upon B for a specified function or scope.

K2 — **Typed Dependency**
Distinguish dependency types where materially relevant rather than reducing every edge to one generic relation.

K3 — **Scope**
A dependency must identify the function/context in which it applies. Dependency in one function must not silently become dependency in all functions.

K4 — **Provenance**
Every consequential dependency edge must retain sufficient provenance to explain why the relation was recorded.

K5 — **Epistemic Status**
Edges must permit confirmed, provisional, disputed, superseded and unknown/incomplete states.

K6 — **Version Applicability**
A dependency may apply only to particular versions/states of either endpoint.

K7 — **Owner Separation**
The KCS may record the relation without acquiring decision authority over the systems represented.

K8 — **Downstream Discovery**
Given a materially changed object B, the system should be able to identify recorded downstream objects potentially requiring review.

K9 — **No Automatic Consequence**
A dependency edge may trigger review; it must not automatically determine the downstream decision.

K10 — **Correction Propagation**
Legitimate correction/supersession of B should be capable of generating bounded review triggers for material dependents.

K11 — **Historical Preservation**
Correction of an edge or endpoint must not erase prior dependency state or provenance.

K12 — **Missing-Edge Humility**
Absence of a recorded edge must never be treated as proof that no dependency exists.

K13 — **Contestability**
Consequential dependency claims must be challengeable and correctable.

K14 — **Current-State Retrieval**
A consumer should be able to retrieve the dependency state relevant to its current task without loading the entire civil knowledge graph.

K15 — **Bounded Disclosure**
Dependency retrieval should expose only the information necessary for the legitimate downstream function.

K16 — **Circularity Visibility**
The index should permit detection/representation of cycles without automatically classifying every cycle as pathological.

K17 — **Criticality Without Sovereignty**
Material criticality may be recorded where legitimately established, but centrality/criticality must not create authority.

K18 — **Temporal Compatibility**
Dependency state should interface with the Civilisation Clock so that changes and review triggers can be related to developmental/civil state transitions.

K19 — **Continuity Compatibility**
Dependency information should support identification of minimum functional restoration prerequisites without defining personal or constitutional continuity by itself.

K20 — **Domain Extensibility**
The relation model must be usable across governance, continuity, emergency, resource, epistemic and participation domains without erasing domain-specific meaning.

K21 — **Machine/Human Accessibility**
The representation should support machine-readable traversal while retaining human-auditable explanations.

K22 — **Recursive Self-Application**
The KMDI's own dependencies, assumptions, versions and corrections must themselves be representable/reviewable.

# 4. Frozen Downstream Predictions

The extension should improve, without absorbing:

P1 Civilisation Clock prerequisite/development ordering.
P2 Bounded correction propagation.
P3 State Map explanatory dependency state.
P4 Dependency-relevant induction.
P5 Continuity restoration dependency sets.
P6 Emergency dependency querying.
P7 Resource-model assumption/dependency review.
P8 Developmental-topology reuse and reduced rediscovery.

# 5. Failure Conditions

The candidate fails if it:

- becomes a universal truth/authority graph;
- treats missing edges as absence;
- silently converts correlation into dependency;
- forces domain-specific relations into misleading uniformity;
- creates automatic downstream decisions;
- requires indiscriminate centralisation of sensitive information;
- cannot preserve uncertainty or contested edges;
- duplicates an already sufficient existing system;
- adds maintenance burden without improving downstream reasoning.

# 6. Freeze

K1–K22 and P1–P8 are frozen before candidate design.

The next operation may design only the minimum architecture necessary to satisfy these requirements.
