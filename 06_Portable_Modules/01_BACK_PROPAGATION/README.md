# Portable Modules — Back-Propagation

**Project:** The Concord Framework
**Status:** OPERATIONAL RECORD / CORRIGIBLE
**Scope:** Post-graduation review of portable modules and reintegration of justified improvements into the Concord main corpus.

## Purpose

Portable-module graduation is not necessarily the end of development flow. PMEDG can expose failure modes, interface requirements, semantic distinctions and other improvements after a method has been extracted from its original Concord architecture. A graduated module can therefore become more developed in some respects than the source system from which it was derived.

This section records the return path:

**Concord Source → Portable Extraction → PMEDG Development → Graduated Module → Back-Propagation Audit → Source-Relevance Decision → Bounded Reintegration → Interface Retest → Integrated Concord Capability**

Its purpose is to ensure useful post-extraction improvements are not stranded in portable modules and to preserve a visible audit trail showing exactly what has, and has not, been integrated back into the Concord main corpus.

## Core rule

> **Portable Difference ≠ Source-System Improvement**

> **Validated Portable Refinement ≠ Automatic Canonical Amendment**

Every graduated module may be reviewed, but no change is copied back merely because it exists in the portable version.

## Post-graduation audit

A back-propagation audit should determine the Concord source system; what materially changed during portable development; the evidence origin for each change; whether each change is portability-only, clarification, general improvement, failure-mode correction, interface improvement or source-specific; whether it applies to the current source architecture; the legitimate reintegration path; required interface/regression testing; and final integration state.

## Integration states

- **NOT YET AUDITED**
- **AUDIT ACTIVE**
- **NO SOURCE CHANGE REQUIRED**
- **SOURCE UPDATE CANDIDATE**
- **AWAITING INTEGRATION / RETEST**
- **INTEGRATED / ARCHITECTURAL INTERFACE RETEST PASSED**
- **HOLD / FURTHER EVIDENCE REQUIRED**

These states describe back-propagation only. They do not alter portable-module graduation status.

## Records

The portfolio-level index is **Back-Propagation Register.md**.

Each audited module should receive its own subfolder containing, where applicable, its audit summary, source/delta register, source integration references, interface/regression result, final integration record and unresolved follow-ups.

The authoritative integrated architecture remains in the relevant Concord corpus location. This folder records the portable-module-side audit trail and points to that integration.

## First completed pilot

**State and Maturity Mapping (SMM)** is the first completed back-propagation pilot. Its PMEDG development produced twelve evidence-supported refinements relevant to the original Civil State Map. All twelve passed source-interface regression. The resulting Civil State Map companion is now integrated at the architectural-interface level.

## Relationship to PMEDG

PMEDG governs extraction, development, transfer testing and graduation.

Back-propagation begins **after graduation**.

This separation is deliberate. Graduation asks whether the module is a stable portable artifact. Back-propagation asks whether development performed during that process produced improvements that should return to the Concord source architecture.

Future methodology work may decide whether a back-propagation audit should become an automatic post-graduation trigger. Until then, this section provides the operational record without changing PMEDG retroactively.
