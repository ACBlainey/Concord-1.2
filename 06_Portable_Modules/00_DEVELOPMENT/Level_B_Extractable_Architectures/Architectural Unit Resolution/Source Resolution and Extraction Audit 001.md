# Architectural Unit Resolution — Source Resolution and Extraction Audit 001

**Development level:** Level B — Extractable Architecture  
**Status:** SOURCE RESOLUTION COMPLETE / EXTRACTION AUTHORISED  
**Date:** 23 September 2026  
**Primary source:** `V1.2a/06_Topology_and_Formalisation/Architectural Unit Resolution v0.1 — Pre-Gap Node and System-Family Classification.md`  
**Source family:** Civilisational Developmental Topology / CRADP / abstraction-level formalisation

---

## 1. Audit question

Does Architectural Unit Resolution (AUR) contain a coherent portable mechanism that can be extracted from the Concord without requiring adoption of the wider civilisational architecture?

**Finding: YES.**

The source already contains a compact pre-gap method whose function is to prevent false structural-gap declarations caused by auditing an intentionally partial document as though it were the complete architecture.

---

## 2. Origin and problem

AUR was created after CH004 exposed a false-positive failure mode:

> **Document ≠ necessarily System.**

A local document may be a subsystem, interface, companion, method, development note or provenance record. A relation absent locally may already be supplied by a legitimate neighbouring architecture.

The portable problem is therefore broader than Concord:

> **Before declaring that an architecture lacks a required function, determine the correct architectural unit and close the relevant system family.**

---

## 3. Primary portable mechanism

The source procedure is:

1. identify the source/document's declared purpose and status;
2. identify explicit upstream/downstream interfaces;
3. identify whether it points to a canonical or fuller architecture;
4. determine whether the tested relation belongs locally, at an interface, or in the wider system family;
5. inspect the relevant connected architecture before declaring structural absence;
6. preserve unresolved scope rather than guessing.

This is sufficiently self-contained to extract.

---

## 4. Unit classification

The source supplies functional unit types:

- Canonical Integrated Architecture;
- Subsystem;
- Interface / Bridge;
- Portable Module;
- Companion / Developed Concept;
- Development Note;
- Constitutional/Core Source;
- Method / Epistemic Tool;
- Reference / Provenance Source;
- Unresolved Unit.

The classification is explicitly functional rather than hierarchical.

For portability these labels can remain as a default vocabulary while allowing equivalent local labels.

---

## 5. System-family closure

The central abstraction is:

> **Family(D) = D + explicitly relevant architectural neighbours required to perform D's declared function.**

Family closure stops when the tested relation is:

- locally resolved;
- deliberately delegated and adequately interfaced;
- demonstrably inapplicable;
- or unresolved after the relevant family has been inspected.

Critically, family closure is **not unrestricted corpus search**. Membership follows declared interfaces, dependencies, canonical status or strong source-grounded functional dependency.

This gives AUR a bounded search rule rather than an invitation to search indefinitely.

---

## 6. Anti-false-positive rule

The source formalises:

**MissingRelation(D,R)**  
+ **ExplicitInterface(D,C)**  
+ **RelationPresent(C,R)**  
→ **DoNotInferStructuralGapFromD**

Candidate outcomes then include:

- local representation gap;
- intentional scoping;
- distributed existing function;
- interface gap;
- genuine system-family gap;
- unresolved.

This is the strongest portable core.

---

## 7. Interface adequacy

AUR does not allow a mere reference to another system to erase a gap.

Delegation counts as resolved only where enough of the following chain exists:

**Source System**  
→ **Trigger / Handoff**  
→ **Responsible System**  
→ **Required Function**  
→ **Return / Consequence Propagation**  
→ **Provenance**

Therefore:

> **Named Neighbour ≠ Adequate Interface**

This prevents AUR from replacing one false positive with a false negative.

---

## 8. Relationship to CRADP

CRADP contains a wider diagnostic/development cycle including source resolution, ownership resolution, dependency tracing, gap classification, response selection, prediction freezing, development and retest.

AUR is narrower.

Its portable function is the **pre-gap unit-resolution gate**:

**Candidate Local Deficit**  
→ **What Unit Is Being Audited?**  
→ **What Is Its Legitimate Scope?**  
→ **What Family/Interfaces Supply Its Function?**  
→ **Is the Relation Local, Delegated, Distributed, Inapplicable or Actually Missing?**  
→ **Only Then Classify the Gap**

AUR should therefore remain a standalone diagnostic primitive rather than absorbing CRADP.

---

## 9. Relationship to ESCP

AUR operationalises an important ESCP safeguard at architectural-unit scale.

> **Not represented in the local document ≠ absent from the architecture.**

But the converse is equally important:

> **Possible external ownership ≠ demonstrated external satisfaction.**

AUR therefore requires evidence-based family membership and interface adequacy.

---

## 10. Concord-specific dependencies

The portable mechanism does **not** require:

- Concord constitutional institutions;
- the Civilisation Clock;
- CCSSL;
- KCS;
- the Concord abstraction-layer ladder;
- the full Civilisational Developmental Topology;
- Concord governance;
- Concord-specific folder structure.

Those systems provide source context and applications.

A portable user needs only:

1. an audit object;
2. a candidate required relation/function;
3. evidence about the object's declared scope/status;
4. identifiable architectural neighbours/interfaces;
5. enough source access to inspect the relevant family;
6. an explicit uncertainty state.

---

## 11. Minimum inputs

A standalone AUR assessment should receive:

- target source/unit;
- declared purpose;
- declared status/type if available;
- candidate missing relation/function;
- known interfaces/dependencies;
- relevant neighbouring sources;
- provenance/evidence;
- search scope.

Where type, family membership or interface adequacy cannot be established, preserve **UNKNOWN**.

---

## 12. Outputs

AUR should produce:

- resolved audit unit;
- unit type(s);
- declared/local scope;
- relevant system family;
- family-membership evidence;
- tested relation/function;
- local state;
- external/delegated state;
- interface adequacy;
- closure state;
- classification;
- uncertainty;
- provenance/search scope.

---

## 13. Failure modes

The source and neighbouring methodology expose several important failure modes:

- Document = System error;
- unrestricted family expansion;
- family membership inferred from topical similarity;
- neighbour named but interface not demonstrated;
- local omission promoted directly to structural absence;
- external capability used to hide an inadequate interface;
- unresolved scope converted into certainty;
- canonical labels treated as hierarchy;
- current representation treated as complete evaluation space.

---

## 14. Source-family support

The primary AUR paper is unusually compact and already close to portable form.

Neighbouring source architecture strengthens rather than replaces it:

- **CRADP** supplies the larger source-resolution and gap-classification context;
- **Civilisational Developmental Topology** supplies ownership, dependency and minimum-intervention logic;
- **Developmental Topology Demonstration 001** shows why owner/interface resolution can prevent unnecessary architectural proliferation;
- **ESCP** supplies the epistemic boundary against converting incomplete representation into absence.

No blocking dependency was found that prevents AUR being specified independently.

---

## 15. Extraction decision

> **SOURCE RESOLUTION SUFFICIENT FOR STANDALONE SPECIFICATION.**

> **NO BLOCKING SOURCE OMISSION IDENTIFIED AT THIS STAGE.**

AUR is a strong Level B extraction candidate because its source mechanism is explicit, bounded and separable from Concord-specific institutions.

The next development step is to create a standalone portable specification preserving:

**Resolve Unit → Close Relevant Family → Test Interface Adequacy → Classify Local Omission Correctly → Preserve Unknowns**

without expanding AUR into the full CRADP development protocol.

---

## 16. Epistemic boundary

This audit establishes extractability, not validation.

It does not establish that AUR:

- always identifies the correct system family;
- eliminates false positives;
- eliminates false negatives;
- guarantees complete source recovery;
- works equally well across software, institutions, research corpora and other architectures;
- or outperforms alternative dependency/modularity analysis methods.

Those claims require transfer and empirical testing.
