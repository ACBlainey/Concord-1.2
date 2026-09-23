# Architectural Unit Resolution — Portable Specification v0.1

**Status:** DEVELOPMENT / PORTABLE EXTRACTION CANDIDATE / NOT YET GRADUATED  
**Version:** 0.1  
**Date:** 23 September 2026  
**Development level:** Level B — Extractable Architecture

## 1. Purpose

Architectural Unit Resolution (AUR) is a diagnostic method for determining **what architectural unit should actually be evaluated before a local omission is classified as a structural gap**.

Its core safeguards are:

> **Document ≠ necessarily System**

> **Missing locally ≠ missing architecturally**

> **Named neighbour ≠ adequate interface**

AUR reduces both false structural-gap declarations and false claims of external satisfaction.

## 2. Scope

AUR is a **pre-gap diagnostic architecture**. It asks:

1. What unit is being audited?
2. What is that unit legitimately intended to contain?
3. Is the tested relation/function local, delegated, distributed, inapplicable or unresolved?
4. Which connected architectural neighbours legitimately belong to the relevant system family?
5. Is an external/delegated function actually connected through an adequate interface?
6. What can be concluded after bounded family closure?

AUR does not redesign the architecture, choose development priority, grant authority, determine substantive law/ethics, guarantee complete source recovery, or perform the entire CRADP cycle.

## 3. Core problem

Given an observation that local unit D does not contain relation/function R, the unsafe inference is:

**MissingRelation(D,R) → StructuralGap**

D may instead be a subsystem, interface, portable module, companion, development note, core constraint, method, provenance source, or unresolved object.

AUR inserts:

**Observed Local Omission → Resolve Architectural Unit → Resolve Legitimate Scope → Resolve Relevant Family → Test Interface / Distributed Satisfaction → Classify**

## 4. Default unit types

- **CIA — Canonical Integrated Architecture:** intended to contain/represent the integrated architecture for a system/domain.
- **SUB — Subsystem:** bounded component intentionally contained within a larger architecture.
- **INT — Interface / Bridge:** primarily defines relations, translation or handoff between systems.
- **PM — Portable Module:** reusable architecture intended to operate across domains/hosts.
- **CDC — Companion / Developed Concept:** develops one aspect while explicitly relying on wider architecture.
- **DN — Development Note:** intentionally incomplete work under development.
- **CORE — Constitutional / Core Source:** establishes governing constraints/invariants rather than complete implementation.
- **MET — Method / Epistemic Tool:** reasoning, measurement, evaluation, research or development procedure.
- **REF — Reference / Provenance Source:** preserves history, evidence, derivation, decisions or prior state.
- **UNK — Unresolved Unit:** architectural role cannot yet be established.

Typing is functional, not hierarchical. A unit may have more than one applicable type. Local deployments may use equivalent labels.

## 5. Architectural-unit resolution

For target D record declared name, purpose, status, intended function, apparent scope, version/state, upstream/downstream interfaces, referenced fuller architectures, dependencies, dependents, provenance and uncertainty.

Then ask:

> **Is D intended to own the tested relation R?**

Allowed states: **YES / NO / PARTIALLY / UNKNOWN / DISPUTED**.

Do not infer ownership merely because R would be useful locally.

## 6. Tested relation abstraction

Describe the apparent omission as a function/relation rather than only missing wording:

**Target D → Candidate Relation/Function R → Why R appears applicable → Evidence present → Evidence absent**

This prevents literal phrase matching from becoming architectural reasoning.

## 7. Relevant system family

Define:

> **Family(D,R) = D + source-grounded architectural neighbours relevant to determining whether R is legitimately supplied for D's declared function.**

Family membership requires evidence such as explicit interface, declared dependency/ownership, fuller-system relationship, explicit delegation/composition, or strong source-grounded functional dependency.

> **Similar Topic ≠ Same Architectural Family**

## 8. Family-expansion procedure

Starting from D:

1. inspect declared purpose/status;
2. identify explicit interfaces/dependencies;
3. identify fuller/canonical architecture if declared;
4. identify legitimate owner candidates for R;
5. follow only source-grounded relations material to R;
6. record each family-membership justification;
7. stop when closure conditions are met.

Do not perform unrestricted corpus expansion merely because related material exists.

## 9. Family closure

Closure occurs when one is established:

- **FC-1 Local resolution:** R adequately supplied by D.
- **FC-2 External/delegated resolution:** R adequately supplied by a legitimate connected neighbour with sufficient interface.
- **FC-3 Distributed resolution:** R adequately supplied across multiple connected units with sufficient composition/interfaces.
- **FC-4 Inapplicable:** R does not legitimately apply to D/relevant family in context.
- **FC-5 Genuine family-level deficit:** relevant family sufficiently resolved to establish R is required but inadequately supplied.
- **FC-6 Unresolved:** evidence insufficient to establish family membership, ownership, applicability or satisfaction.

**UNRESOLVED is a valid stopping state.**

## 10. Interface adequacy

Where R is claimed externally supplied, test whether enough of this chain exists:

**Source Unit → Trigger / Handoff → Responsible Unit → Required Function → Return / Consequence Propagation → Provenance**

Also ask whether the responsible unit is identifiable, actually possesses the capability, has an operable handoff, preserves responsibility, represents failure/degradation, propagates correction/review where material, remains current, and is evidenced rather than inferred.

> **External Capability ≠ Interface Satisfaction**

> **Delegation Mentioned ≠ Delegation Operational**

## 11. Anti-false-positive rule

**MissingRelation(D,R) + ExplicitRelevantInterface(D,C) + RelationAdequatelyPresent(C,R) → DoNotInferStructuralGapFromD**

The result may instead be local representation gap, intentional scoping, externally satisfied function, distributed function, interface gap, family-level gap, inapplicable relation, or unresolved.

## 12. Anti-false-negative rule

> **NeighbourExists(C) NOT→ RelationSatisfied(D,R)**

> **RelationPresentSomewhere(R) NOT→ AdequateFor(D,R)**

A claimed external resolution must survive interface-adequacy testing.

## 13. Classification states

- **AUR-C1 LOCAL FUNCTION PRESENT** — R adequately present in D.
- **AUR-C2 INTENTIONAL LOCAL SCOPING** — R absent locally because D is not intended to own it; local omission itself establishes no defect.
- **AUR-C3 EXTERNALLY SATISFIED** — legitimate neighbour supplies R through adequate interface.
- **AUR-C4 DISTRIBUTED SATISFACTION** — R supplied across multiple units with adequate composition/interfaces.
- **AUR-C5 LOCAL REPRESENTATION GAP** — underlying function exists but current representation fails to expose the relationship sufficiently.
- **AUR-C6 INTERFACE GAP** — capability exists elsewhere but handoff/composition is inadequate.
- **AUR-C7 FAMILY-LEVEL STRUCTURAL GAP** — R is applicable/required at resolved family level but no adequate owner/capability is established within bounded search.
- **AUR-C8 INAPPLICABLE** — R does not legitimately apply in audited scope/context.
- **AUR-C9 UNRESOLVED** — evidence insufficient or conflicting.

## 14. ESCP safeguard

> **Not represented in the local object ≠ absent from the architecture**

> **No source found within the current search ≠ source does not exist**

AUR-C7 means no adequate satisfying mechanism was established within the resolved relevant family and recorded search scope. It does not mean no such mechanism exists anywhere.

Family boundaries are themselves hypotheses and remain revisable.

## 15. Search-scope record

Every run records sources inspected, interfaces followed, family members admitted, candidates rejected, inclusion/exclusion reasons, unavailable sources, unresolved references and stopping rationale.

## 16. Minimal AUR procedure

1. Record the observed omission.
2. Resolve D's unit type.
3. Test legitimate local scope.
4. Abstract R.
5. Build the relevant family from source-grounded relations.
6. Test external/distributed satisfaction.
7. Test interface adequacy.
8. Apply a closure rule.
9. Assign AUR-C1 through AUR-C9.
10. Record uncertainty and search scope.

## 17. Compact algorithm

**INPUT:** target D, candidate relation R, context c, accessible architecture C

1. ResolveUnit(D)
2. ResolveDeclaredScope(D,c)
3. AbstractRelation(R)
4. TestLocal(D,R,c)
5. If local adequate → AUR-C1
6. BuildRelevantFamily(D,R,C)
7. TestExternalOrDistributedSupply
8. TestInterfaceAdequacy
9. If intentional local scoping and no defect established → consider AUR-C2
10. Adequate external supply → AUR-C3
11. Adequate distributed supply → AUR-C4
12. Underlying relation exists but representation deficient → AUR-C5
13. Capability exists but interface deficient → AUR-C6
14. Relation demonstrably inapplicable → AUR-C8
15. Relevant family sufficiently resolved and required relation unsatisfied → AUR-C7
16. Otherwise → AUR-C9
17. Record provenance, uncertainty, family boundary and search scope.

## 18. Required output record

A minimal result contains:

1. Audit ID.
2. Target D.
3. Context c.
4. Candidate relation/function R.
5. Resolved unit type(s).
6. Declared/local scope.
7. Family members.
8. Family-membership evidence.
9. Sources searched.
10. Local relation state.
11. External/distributed relation state.
12. Interface-adequacy result.
13. Closure state.
14. AUR classification.
15. Confidence/uncertainty.
16. Unresolved references.
17. Stopping rationale.

## 19. Worked abstract examples

### A — subsystem with legitimate external owner

A subsystem lacks appeal handling. Its specification explicitly delegates appeals to a review service. The service contains the capability and the interface specifies trigger, case transfer, decision return and correction propagation.

**Result: AUR-C3 — EXTERNALLY SATISFIED.**

### B — neighbour named, handoff absent

A policy says disputes are “handled by Review” but defines no trigger, payload, responsibility, return or correction path. Review possesses dispute capability.

**Result: AUR-C6 — INTERFACE GAP.**

### C — intentionally narrow research note

A development note explores one algorithm and explicitly points to a production architecture for production concerns.

**Result: AUR-C2 — INTENTIONAL LOCAL SCOPING**, subject to inspection of any material claimed dependency.

### D — unresolved family

A component depends on a service referred to by an obsolete name. Multiple possible successors exist and provenance is incomplete.

**Result: AUR-C9 — UNRESOLVED.**

Do not choose the most plausible successor merely to close the audit.

## 20. Failure modes

- Document-equals-system error.
- Topic-family inflation.
- Infinite family search.
- Named-neighbour false satisfaction.
- Capability-without-handoff false satisfaction.
- Local ownership inflation.
- Representation/structure confusion.
- Unknown-to-absence conversion.
- Canonical-status hierarchy.
- Stale-family error.

## 21. Relationship to wider methods

AUR can be used independently. In a wider development protocol it should normally occur before structural-gap declaration and invention:

**Observed Deficit → AUR → Gap Classification → Ownership Resolution → Dependency Analysis → Response Selection → Development / Integration → Retest**

AUR owns only the unit/family-resolution portion.

## 22. Non-authority boundary

> **Architectural Classification ≠ Authority**

> **Family Membership ≠ Ownership**

> **Dependency ≠ Permission**

> **Diagnostic Confidence ≠ Legitimacy**

## 23. Validation requirements before graduation

AUR should be blind-tested against cases containing:

- deliberately narrow subsystem;
- complete integrated architecture;
- named but inadequate external interface;
- genuinely adequate external interface;
- distributed function;
- false topical neighbour;
- stale/obsolete interface evidence;
- ambiguous family membership;
- genuine family-level deficit;
- correct UNKNOWN result;
- harmless local omission with material interface failure.

The test should be able to falsify AUR if it systematically hides genuine gaps, expands family boundaries arbitrarily, cannot distinguish scoping from absence, accepts named neighbours without handoff, cannot stop bounded search, or collapses UNKNOWN into confidence.

A test brief and expected-findings key must be frozen before obtaining the independent response.

## 24. Current finding

AUR v0.1 is sufficiently extracted for adversarial transfer testing.

The strongest portable claim presently supported is:

> **Before inferring a structural gap from a local omission, resolve the architectural unit, close the relevant source-grounded system family, and test interface adequacy.**

This specification does not yet establish reliable improvement outside its source architecture.

## 25. Provenance

Primary source:

- *Architectural Unit Resolution v0.1 — Pre-Gap Node and System-Family Classification*

Supporting source family:

- *Concord Recursive Architectural Development Protocol — CRADP v0.1*
- *Civilisational Developmental Topology — Foundations, Boundaries and Operating Architecture*
- *Developmental Topology Demonstration 001 — From Local Gap to Upstream Development and Recursive Closure*
- *Evaluation-Space Completeness Problem — A Portable Model of Correct Evaluation Within an Incomplete Representational Space*
- *Architectural Unit Resolution — Source Resolution and Extraction Audit 001*

Revisions must preserve the distinction between source architecture, extracted portable claims and later test-driven additions.
