# State Map 001A — Frozen Minimum Schema and Boundary Requirements

**Status:** V1.2a PRE-DEVELOPMENT FREEZE  
**Date:** September 2026  
**External knowledge state:** INTERNAL ONLY  
**Canonical effect:** NONE  
**Parent:** State Map Source Resolution 001

# 1. Purpose

Freeze the minimum requirements for a Concord State Map before candidate design.

The State Map is a synthesis representation, not a new authority.

# 2. Frozen Functional Requirements

SM1 — identify the architectural unit/object being represented.

SM2 — identify the unit's legitimate owner/domain where known.

SM3 — represent current developmental/maturity state multidimensionally where applicable.

SM4 — represent capabilities currently established.

SM5 — represent unresolved/open capabilities or questions.

SM6 — represent upstream blockers/dependencies.

SM7 — represent known downstream dependents.

SM8 — represent interface state separately from internal maturity.

SM9 — represent validation/evidence status.

SM10 — preserve provenance for consequential state claims.

SM11 — represent uncertainty, disputed state and unknown state explicitly.

SM12 — identify last material review/update.

SM13 — interface with Clock/CRSTL transition state.

SM14 — interface with KCS/KMDI dependency/knowledge state.

SM15 — permit comparison with prior State Map state without erasing history.

SM16 — expose stale state rather than silently presenting it as current.

SM17 — permit bounded retrieval by system, capability, dependency, maturity dimension or unresolved question.

SM18 — distinguish missing data from negative findings.

SM19 — permit healthy recursive/circular dependencies without automatically labelling them defects.

SM20 — support human-readable and machine-readable representations.

SM21 — permit domain-owned corrections and contestation.

SM22 — support partial maps; completeness must never be implied merely because a map exists.

# 3. Frozen Boundary Requirements

B1 — State description != governance authority.

B2 — State Map maturity != participant worth or political status.

B3 — Dependency centrality != authority.

B4 — Priority is not decided by the State Map.

B5 — A map entry is not truth merely because it is recorded.

B6 — No recorded gap != no gap.

B7 — No recorded dependency != no dependency.

B8 — Domain systems retain authority for domain-specific conclusions.

B9 — Sensitive dependency/state information must support bounded disclosure.

B10 — The State Map must itself be mapped, versioned, reviewable and correctable.

# 4. Frozen Core State Record

A candidate record must be capable of representing at least:

- Unit ID;
- unit type;
- owner/domain;
- purpose/function;
- maturity vector/status;
- established capabilities;
- unresolved capabilities/questions;
- upstream dependencies/blockers;
- downstream dependents;
- interface status;
- validation/evidence status;
- provenance;
- uncertainty/dispute;
- last review;
- Clock/transition reference;
- supersession/correction history.

# 5. Frozen Predictions

P-SM1 Clock state assessment.
P-SM2 Priority/dependency selection.
P-SM3 Induction current-state navigation.
P-SM4 Developmental topology analysis.
P-SM5 Temporal review comparison.
P-SM6 Resource steering enhancement.

# 6. Failure Conditions

The State Map fails if it becomes:

- a central command mechanism;
- a false claim of complete civil knowledge;
- a single maturity score;
- a replacement for KCS, Clock or domain systems;
- a mechanism for automatic authority;
- a stale dashboard presented as current reality;
- an indiscriminate disclosure surface;
- an unchallengeable classification registry.

# 7. Freeze

SM1–SM22, B1–B10, the core record and P-SM1–P-SM6 are frozen before candidate architecture generation.
