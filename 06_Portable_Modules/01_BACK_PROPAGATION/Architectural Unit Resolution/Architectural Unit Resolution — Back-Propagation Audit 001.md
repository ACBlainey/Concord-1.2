# Architectural Unit Resolution — Back-Propagation Audit 001

**Portable module:** Architectural Unit Resolution — Portable Module v1.0
**Status:** SOURCE UPDATE CANDIDATE
**Primary source:** V1.2a/06_Topology_and_Formalisation/Architectural Unit Resolution v0.1 — Pre-Gap Node and System-Family Classification
**Source family:** Civilisational Developmental Topology / CRADP / abstraction-level formalisation
**Date:** 24 September 2026

## Purpose

This audit compares graduated AUR v1.0 with the experimental Concord source from which it was extracted.

The source was frozen before CH005 and explicitly had **Canonical effect: NONE**. Portable development subsequently completed two blind transfer tests and refined several classification boundaries.

The question is therefore not whether the source kernel should be replaced. It is whether validated post-extraction refinements should now return to the Concord methodology.

## Source kernel retained

The source already contains the central AUR architecture:

- Document ≠ necessarily System;
- functional unit typing;
- pre-gap resolution procedure;
- bounded system-family closure;
- anti-false-positive rule;
- document maturity versus family maturity;
- interface-adequacy chain;
- ESCP discipline;
- prediction that AUR should reduce false positives without hiding genuine interface gaps.

Portable development strongly confirmed this kernel.

## AUR-BP-01 — Local ownership versus architectural satisfaction

BTT-001 exposed ambiguity between intentional local scoping and external satisfaction.

Portable AUR now treats these as separate dimensions:

1. does the local unit legitimately own the function?
2. if not, is the function adequately supplied for the architecture?

Where a function is intentionally non-local and adequately supplied externally, external satisfaction is the primary architectural result while intentional non-ownership remains local-scope rationale.

**Class:** General clarification / classification correction.

**Decision:** INCORPORATE.

## AUR-BP-02 — C6 interface gap versus C7 family-level structural gap

Portable development sharpened the distinction:

- required capability exists but invocation/handoff/return/provenance is inadequate → **INTERFACE GAP**;
- required capability/owner is not established in the resolved family → **FAMILY-LEVEL STRUCTURAL GAP**.

A larger workflow may contain both at different sub-functions.

**Class:** General improvement / false-gap safeguard.

**Decision:** INCORPORATE.

## AUR-BP-03 — Smallest meaningful functional resolution

BTT-002 confirmed that mixed workflows must be decomposed before classifying the missing function.

> **Do Not Classify the Workflow Before Decomposing the Missing Function**

This prevents an integration failure from being mislabeled as absence of the entire capability.

**Class:** General improvement / diagnostic safeguard.

**Decision:** INCORPORATE.

## AUR-BP-04 — Current, historical and candidate dependencies

Portable development distinguishes:

- current architectural dependencies;
- historical/decommissioned relations retained for provenance;
- future/speculative candidate dependencies.

> **Future Reference ≠ Current Architectural Dependency**

> **Named but Unresolved Candidate ≠ Family Member**

Historical or planned neighbours cannot satisfy a current function merely because they are named.

**Class:** General improvement / epistemic safeguard.

**Decision:** INCORPORATE.

## AUR-BP-05 — Diagnostic closure versus functional satisfaction

The source says family search stops after relevant closure but does not explicitly separate successful function from sufficient diagnostic closure.

Portable AUR establishes:

> **Diagnostic Closure ≠ Functional Satisfaction**

A family may be sufficiently resolved to diagnose an interface gap, structural gap, inapplicability or unresolved state while the function remains unsatisfied.

**Class:** General improvement.

**Decision:** INCORPORATE.

## AUR-BP-06 — C2 versus C8 applicability boundary

BTT-002 sharpened the residual distinction:

- **intentional scoping/non-ownership:** the relation belongs to the wider architectural setting but not this unit;
- **inapplicable:** the relation does not apply to this unit/family in the audited context.

This is especially important for obsolete/historical units and false topical neighbours.

**Class:** Clarification.

**Decision:** INCORPORATE.

## AUR-BP-07 — Distributed satisfaction

Portable testing demonstrated that a function can be architecturally satisfied across multiple legitimate units without one unit containing the complete workflow.

This should remain distinguishable from both local satisfaction and interface failure.

**Class:** Clarification / interface improvement.

**Decision:** INCORPORATE.

## AUR-BP-08 — Explicit family-membership evidence

The source requires source-grounded family relations. Portable AUR makes the output obligation clearer: record the relevant family and the evidence supporting membership.

Topical similarity remains insufficient.

**Class:** Clarification / provenance improvement.

**Decision:** INCORPORATE.

## AUR-BP-09 — Search-scope provenance and bounded structural-gap claim

Portable AUR makes explicit that a C7/family-level gap means no adequate mechanism is established **within the resolved family/search scope**, not proof that none exists anywhere.

This operationalises the source ESCP safeguard in the output.

**Class:** Clarification / epistemic safeguard.

**Decision:** INCORPORATE.

## AUR-BP-10 — Functional unit typing remains non-hierarchical and non-authoritative

Blind transfer confirmed that CORE, interface, subsystem, method, companion and other unit types describe architectural role rather than authority.

This source rule survived testing and should become an explicit retained invariant if AUR is promoted from experimental method.

**Class:** Confirmed source safeguard.

**Decision:** RETAIN / FORMALISE.

## Audit result

The audit identifies **10 source-relevant post-extraction outcomes**:

- 5 materially sharpen diagnostic/classification behaviour;
- 4 clarify provenance, scope or interface semantics;
- 1 confirms and formalises a source safeguard;
- 0 require replacement of the AUR kernel;
- 0 create civil/governance authority.

Unlike the previous three audits, the primary source is explicitly an **experimental non-canonical method**. The back-propagation consequence is therefore more significant than a companion patch alone: successful portable development provides evidence to promote the method itself into the current Concord methodological architecture, while retaining corrigibility.

## Evidence basis

AUR development completed:

- BTT-001: **15/15 frozen predictions materially confirmed**; strong transfer; no fundamental failure;
- BTT-002: **17/17 frozen predictions materially confirmed**; strong transfer/delta validated; no blocking failure;
- demonstrated false-gap prevention and genuine-gap detection;
- preserved bounded-search/ESCP discipline;
- separated current, historical and candidate dependencies;
- validated diagnostic closure distinct from functional satisfaction.

These counts are evidence summaries, not universal statistical proof.

## Integration recommendation

Create a current source-side method:

**Architectural Unit Resolution — Concord Method v1.0**

in the Civilisational Developmental Topology/formalisation area.

It should preserve the original v0.1 provenance while incorporating the ten returned outcomes above.

The original frozen V1.2a experimental file should remain untouched as historical provenance.

Required regression should check at minimum:

- Civil State Map/SMM gap classification;
- CRADP/source-resolution workflow;
- KCS dependency/family evidence;
- Active Development gap/candidate generation;
- ESCP boundaries.

## Status decision

> **AUR BACK-PROPAGATION: SOURCE UPDATE CANDIDATE — METHOD PROMOTION JUSTIFIED**

This is not a claim of universal validation. It is a claim that the Concord's own experimental AUR method has now completed enough independent portable development to justify return as a current corrigible methodology.
