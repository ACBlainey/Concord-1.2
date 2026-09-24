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

## Governing method

The operational method is:

**Portable-Module Back-Propagation Method — BPM v1.0**

located in:

`08_Active_Development/01_DEVELOPMENT_NOTES/03_CONCORDIAN_METHODOLOGY/`

BPM v1.0 was formalised after five completed cycles: SMM, STRA, KCS Change Propagation, Architectural Unit Resolution and Contextual Wrapper Architecture.

It adds explicit source-family resolution, recovered-architecture classification, multiple integration dispositions, one-cycle execution, regression discipline and a no-change discrimination check.

## Post-graduation audit

A back-propagation audit should determine the immediate Concord source and materially relevant source family; what materially changed or was exposed during portable development; the evidence origin for each delta; whether each delta is portability-only, clarification, general improvement, failure-mode correction, interface improvement, recovered architecture/source-family consolidation or source-specific; whether it applies to the current source architecture; the smallest legitimate disposition; required interface/regression testing; and final integration state.

> **Local Source Absence ≠ Concord-Wide Absence**

> **Source Recovery ≠ New Invention**

> **Back-Propagation Success = Correct Disposition of the Delta**

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

## Completed methodological evidence

Five distinct cycles currently support BPM v1.0:

- **SMM:** substantial bounded companion upgrade;
- **STRA:** operational/failure-mode companion upgrade;
- **KCS Change Propagation:** bounded refinement of an already-mature source;
- **Architectural Unit Resolution:** promotion of a validated experimental method;
- **Contextual Wrapper Architecture:** source-family consolidation after ESCP source recovery.

The variety of outcomes is important. Back-propagation is not an automatic source-expansion mechanism.

## Relationship to PMEDG

PMEDG governs extraction, development, transfer testing and graduation.

Back-propagation begins **after graduation**.

This separation is deliberate. Graduation asks whether the module is a stable portable artifact. Back-propagation asks whether development performed during that process produced improvements that should return to the Concord source architecture.

BPM v1.0 now provides the normal post-graduation audit path. A graduated module may be reviewed through BPM without changing PMEDG retroactively.

Once evidence is available, normal execution is a single continuous cycle:

**SOURCE RESOLVE → COMPARE → CLASSIFY → DISPOSE → INTEGRATE IF JUSTIFIED → REGRESS → FINALISE → RECORD**

The cycle stops where evidence, source ownership, new development needs or failed regression genuinely require it.
