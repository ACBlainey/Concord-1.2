# Architectural Unit Resolution v0.1 — Pre-Gap Node and System-Family Classification

**Status:** V1.2a EXPERIMENTAL METHOD / FROZEN BEFORE CH005  
**Date:** September 2026  
**Canonical effect:** NONE  
**Derived from:** CH004 false-positive analysis

# 1. Problem

CH004 demonstrated that a topology can generate a false structural-gap candidate when it treats an intentionally scoped document as though it were the complete architectural system.

Therefore:

Document ≠ necessarily System.

Before testing a missing relation, the model must determine the architectural unit to which the relation should apply.

# 2. Unit Types

Each mapped source should be typed, where evidence permits, as one or more of:

- **Canonical Integrated Architecture (CIA)** — intended to contain the integrated architecture for a system/domain.
- **Subsystem (SUB)** — bounded component inside a larger architecture.
- **Interface / Bridge (INT)** — primarily defines relations between systems.
- **Portable Module (PM)** — reusable architecture intended to operate across domains.
- **Companion / Developed Concept (CDC)** — preserves or develops one aspect while explicitly relying on wider architecture.
- **Development Note (DN)** — intentionally incomplete work under development.
- **Constitutional/Core Source (CORE)** — establishes governing constraints or principles.
- **Method / Epistemic Tool (MET)** — procedure or reasoning architecture rather than civil authority system.
- **Reference / Provenance Source (REF)** — records history, evidence or derivation rather than supplying complete operative architecture.
- **Unresolved Unit (UNK)** — source role not yet established.

Typing is functional, not hierarchical.

# 3. Resolution Procedure

Before candidate-gap generation:

1. identify the document's declared purpose/status;
2. identify explicit upstream/downstream interfaces;
3. identify whether it points to a canonical or fuller architecture;
4. determine whether the tested relation belongs locally, at an interface, or in the wider system family;
5. inspect the relevant connected architecture before declaring a structural absence;
6. preserve unresolved scope rather than guessing.

# 4. System-Family Closure

For document D and relation R:

Family(D) = D + explicitly relevant architectural neighbours required to perform D's declared function.

The search should stop when the relation is:

- locally resolved;
- deliberately delegated and adequately interfaced;
- demonstrably inapplicable;
- or still unresolved after relevant family closure.

Family closure is not unrestricted corpus search. It follows declared or source-grounded architectural relations.

# 5. Anti-False-Positive Rule

Candidate future grammar rule:

MissingRelation(D,R)
+ ExplicitInterface(D,C)
+ RelationPresent(C,R)
→ DoNotInferStructuralGapFromD.

Possible classifications then include:

- local representation gap;
- intentional scoping;
- distributed existing function;
- interface gap;
- genuine system-family gap;
- unresolved.

# 6. CH004 Calibration

Multisubstrate Economic Participation is best treated as a Companion / Developed Concept with an explicit economic relationship to Ratchet.

The local paper only partially states challenge/correction propagation.

Ratchet V4.2, the canonical integrated economic/coordination architecture, explicitly supplies appeal, correction, bounded consequence, review, recoverable trust and governance/escalation.

Therefore the system-family relation is present.

# 7. Consequence for Maturity Mapping

Future maturity vectors should distinguish:

M_document(D)

from:

M_family(F(D)).

A document-level partial relation should not lower system-family maturity where the missing function is intentionally and adequately supplied by an explicit neighbour.

Conversely, merely naming another system is insufficient.

The interface itself must be adequate for the required function.

# 8. Interface Adequacy Test

Delegation counts as resolved only if the source-grounded architecture establishes enough of:

Source System
→ Trigger / Handoff
→ Responsible System
→ Required Function
→ Return / Consequence Propagation
→ Provenance.

If only the neighbour's name is present, classify as a possible partial interface rather than complete resolution.

# 9. Experimental Prediction

Applying Architectural Unit Resolution before CH005 should reduce candidate false positives caused by:

- companion papers;
- intentionally narrow modules;
- development notes;
- interface documents;
- functions deliberately delegated to Judiciary, Governance, Metrics, KCS, Ratchet or other systems.

It should **not** eliminate genuine integration gaps where the external function exists but the handoff is insufficient.

# 10. ESCP

Architectural family boundaries are themselves hypotheses.

The model must not infer family membership merely because two documents discuss similar topics.

Family closure must follow explicit interfaces, declared dependencies, canonical status, or strong source-grounded functional dependency.

This method is frozen before selecting CH005.
