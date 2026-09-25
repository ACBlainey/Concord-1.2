# Civil Attention, Reporting, Petition and Resolution Module
## Graduation-Candidate Specification

**Author:** Alexander C. Blainey
**Project:** The Concord Framework
**Method:** PMEDG v1.2
**Date:** 25 September 2026
**Status:** PMEDG STAGE 12 — GRADUATION CANDIDATE / NOT YET RELEASED

## 1. Purpose

This module provides a portable, domain-neutral method by which a participant can cause a legitimate system to notice, preserve, classify, route, examine and respond to a suggestion, problem report, petition or related attention input.

The participant need not understand the host system's internal topology.

The method creates legitimate attention and accountable processing. It does not give the participant unilateral authority over truth, priority, remedy, resources or outcome.

## 2. Core Architecture

**Participant Trigger → Common Intake → Receipt → Original Preservation → Provisional Classification → Existing-Issue Match → Information-Sufficiency Assessment → Issue Creation / Attachment / Split / Merge → Evidence and Epistemic State → Functional Routing → Domain Action Object(s) → Domain Examination / Action → Mandatory Return → Central Resolution Record → Participant Feedback → Challenge / Escalation / Reopening where legitimate**

## 3. Core Invariants

1. **Right to Trigger Attention ≠ Right to Dictate Outcome**
2. **Submission ≠ Evidence ≠ Verification ≠ Finding ≠ Authority to Act**
3. **Received ≠ Verified ≠ Accepted ≠ Authorised**
4. **Popularity ≠ Truth**
5. **Unverified ≠ False**
6. **Reported ≠ True**
7. **Central Visibility ≠ Central Control**
8. **Domain Completion ≠ Issue Resolution**
9. **Routing Creates Responsibility; It Must Not Break Traceability**
10. **Participant Knowledge of the Problem ≠ Participant Knowledge of the Host System**
11. **Auditable Status ≠ Universal Data Access**
12. **Failure to Identify an Owner Must Not Become Failure to Recognise an Issue**
13. **Responsibility Resolution ≠ Substantive Case Resolution**
14. **Participants Can Trigger Attention; They Cannot Manufacture Priority**
15. **Institutions Can Assess Priority; They Cannot Manufacture Finality**
16. **Reviewability Is the Counterweight to Pressure Resistance**
17. **Repeated Confirmation of a Known State ≠ Increased Problem Weight**
18. **New Information About the State → Reassessment of Problem Weight**
19. **Group for Processing; Preserve Individually for Evidence and Provenance**
20. **No Actionable Issue Should Become Inert Merely Because It Is Waiting**
21. **Triggering Review ≠ Authority Over Outcome**
22. **Individual Resolution ≠ Systemic Resolution**
23. **Urgent Enough to Examine or Protect Against ≠ Proven True**

## 4. Input Classes

### Suggestion
A proposed improvement, solution or opportunity. Merit does not depend on popularity.

### Problem Report
A report of a possible defect, harm, failure or undesirable condition.

> **Problem Report ≠ Established Problem**

### Petition
A collective expression of concern, preference or requested action.

> **Petition Support ≠ Problem Weight**

Support is an attention signal, not proof of truth, severity or entitlement to resources.

## 5. Object Model

**Submission Object ≠ Issue Object ≠ Investigation/Examination Object ≠ Finding/Decision Object ≠ Implementation/Remedy Object**

The Submission Object preserves what was actually received.

An Issue Object represents a concern requiring processing.

One submission may create several Issues. Several submissions may attach to one Issue.

Later processing must not rewrite original provenance.

## 6. Classification and Information Sufficiency

Submitter classification is advisory context.

System classification is a provisional, reviewable routing decision.

> **Classification ≠ Information Sufficiency**

Insufficient information is not a finding of falsity.

Anonymity does not itself make a submission non-actionable, and identity does not establish evidentiary sufficiency.

## 7. Split, Merge and Information Delta

Issue Objects are created when needed rather than automatically for every submission.

> **Common Topic ≠ Common Issue**

> **Merge for Processing ≠ Erase Individual Provenance**

The method separates submission volume, source independence where legitimately knowable, materially distinct information, corroborating evidence and contradictory evidence.

> **Raw Count ≠ Independent Participants**

> **Independent Participants ≠ Independent Evidence**

> **Duplicate Processing ≠ Duplicate Information**

> **Case State(t+1) = Case State(t) + Evaluated Information Delta**

## 8. Attention / Truth / Priority Firewall

The module separates:
1. Intake — what was submitted;
2. Attention/Epistemic Assessment — what requires examination and what evidence supports;
3. Problem/Priority/Resource Assessment — the supported state and legitimate response.

> **Intake Pressure May Trigger Re-Evaluation; It Must Not Directly Command Problem Priority or Resource Allocation.**

## 9. Domain Routing and Domain Action Objects

One Issue may route to one or several legitimate functional owners.

Each route creates or binds a **Domain Action Object (DAO)** linking the parent Issue to domain processing.

A DAO should preserve parent reference, routing reason, responsible function, processing state, significant action, dependencies, disposition, review condition where applicable, bounded return information and provenance.

> **One Front Door; Many Legitimate Functional Owners.**

## 10. Mandatory Return

Every outbound route requires a return path.

The parent/common layer must receive enough bounded information to know whether work was received, accepted, transferred, awaiting information, under examination, authorised, in progress, blocked, deferred, resolved, escalated or otherwise legitimately disposed.

> **Every Outbound Route Requires a Return Path.**

Protected evidence need not be returned centrally.

## 11. Problem State and Response State

**Problem State** represents the current best-supported understanding of the underlying Issue.

**Response State** represents what legitimate functions have done, are doing, failed to do or are waiting upon.

> **Problem-State Stability ≠ Response-State Adequacy**

## 12. Responsibility Resolution

When ordinary routing cannot establish legitimate ownership, the Issue remains recognised.

A **Responsibility Resolution Object (RRO)** may record candidate owners, routing reasons, acceptance/refusal/transfer history, disputed responsibility, unresolved functional need, current resolver, escalation and disposition.

> **Responsibility Resolution ≠ Substantive Case Resolution**

The core does not manufacture an authority merely because one is missing.

## 13. Dependencies and External Dependencies

Dependencies may be independent, sequential, mutually dependent, conditionally dependent, blocked or jointly required.

A useful waiting representation is:

**Waiting For + Dependency Owner + Required State/Information + Review Condition + Backstop + Next Responsible Function**

> **Waiting Without a Represented Condition Is a Staleness Risk.**

BTT-002 confirmed that an external/upstream dependency does not require a new core object.

Existing Issue, DAO/RRO, dependency, mandatory-return and review structures are sufficient.

> **External Dependency ≠ Transfer of Local Responsibility**

## 14. Queue Vitality and Deferral

A host may bind the module to a scheduler or state-trigger architecture.

> **Deferral Requires a State, Reason and Review Condition.**

Significant deferrals should remain auditable.

> **Replacing a Review Date Must Not Erase the History of Deferral.**

> **Blocked Is a Claim About State, Not an Exemption From Accountability.**

> **Review Performed ≠ Review Resolved**

> **Timestamp Refresh ≠ Meaningful State Update**

## 15. Urgency

Urgency can justify rapid examination, protective routing or host-authorised protective action.

Urgency does not establish truth.

The Civil Attention core does not acquire emergency authority.

## 16. Protected Information

Protected evidence may remain within the legitimate domain that owns it.

The common layer receives only information necessary for routing, coordination, status, review and feedback.

> **Auditable Status ≠ Universal Data Access**

## 17. Individual and Systemic Resolution

An individual case may reveal a systemic defect.

The two may be linked but processed independently.

> **Systemic Investigation ≠ Reason to Delay an Available Individual Remedy**

An individual workaround or remedy does not automatically resolve the systemic Issue.

## 18. Challenge, Review and Reopening

Legitimate grounds may include classification error, missed evidence, material information delta, stale processing, conflict of interest, implementation failure, changed conditions or overlooked rights/safety implications.

> **Right to Challenge Processing ≠ Right to Dictate Outcome**

Unchanged repetition may attach without full re-examination.

Closure preserves provenance and remains subject to legitimate reopening.

## 19. Feedback

Where legitimately possible, participant-facing feedback should communicate:

**Current State + Reason + Responsible Function(s) + Last Material Action + Next Review Condition**

Protected information may limit detail but must not become a pretext for concealing absence of processing.

## 20. Core / Domain Companion Contract

The portable core is versioned independently.

A domain implementation is:

**Core Method Version N + Domain Companion + Bound Host Services → Domain Implementation**

A Domain Companion may specify:
- domain terminology;
- local evidence requirements;
- authority/jurisdiction boundaries;
- confidentiality rules;
- local processing states;
- escalation routes;
- scheduler/Clock conditions;
- permitted dispositions;
- specialist-system interfaces;
- domain-specific feedback constraints.

A Domain Companion may not:
- redefine a core invariant;
- convert participant attention into command authority;
- remove provenance;
- remove mandatory return;
- turn popularity into truth or substantive priority;
- convert central visibility into central substantive control;
- erase reviewability for convenience;
- silently modify the core version.

> **Domain Requirement ≠ Core Method Amendment**

> **Companion Extension ≠ Core Override**

> **Local Adaptation Must Preserve Core Invariants**

> **Domain Variation Belongs at the Companion Boundary Unless a General Core Defect Is Demonstrated.**

## 21. Core Revision Rule

If a domain discovers a requirement that appears to conflict with or improve the core:

**Domain Finding → Candidate Back-Propagation → Core Review → Bounded Core Revision if Justified → Core Version Change → Companion Regression Review**

Until that process completes, the domain must preserve the current core.

> **Domain-Specific Need Is Evidence for Review, Not Permission for Drift.**

## 22. Host Interface Requirements

The host supplies or binds legitimate mechanisms where needed for:
- durable receipt/persistence;
- identity/standing/anonymity;
- substantive domain authority;
- evidence/verification;
- privacy/protected information;
- escalation/review authority;
- scheduler/review triggers;
- resource allocation;
- emergency authority;
- external-system communication.

The module does not invent missing authority.

## 23. Minimum Auditability

A host implementation should preserve enough provenance to reconstruct:
- original submission;
- associated Issues;
- classification/routing changes;
- responsible owners;
- significant information/evidence changes;
- dispositions;
- significant deferrals;
- challenge/review outcomes;
- overall resolution;
- feedback state.

## 24. Non-Goals

The module does not prescribe:
- universal database schema;
- universal user interface;
- universal priority algorithm;
- universal numerical thresholds;
- universal identity system;
- substantive domain law/policy;
- domain-specific evidence standards;
- resource-allocation formula;
- emergency powers;
- surveillance authority.

## 25. Validation Record

### BTT-001 — Multi-Site Facilities
**16/16 cases handled without core amendment.**

Tested physical hazards, facilities ownership, accessibility, procurement, protected security evidence, contractor implementation, cross-domain defects, no-owner cases and queue staleness.

### BTT-002 — Distributed Open-Source Software Ecosystem
**16/16 cases handled without core amendment.**

Tested distributed repository authority, protected vulnerability evidence, upstream dependencies, release staleness, telemetry conflicts, copied campaigns, submitted patches, cross-repository ownership and systemic versus individual resolution.

### Cross-Test Convergence
**32/32 blind-transfer cases handled without core amendment.**

No core defect was identified.

No material core ambiguity required revision.

Domain variation was absorbed by Domain Companions and Host Interfaces.

## 26. Graduation-Candidate Status

The module has completed:
- candidate registration;
- source resolution;
- extraction audit;
- Portable Specification v0.1;
- BTT-001 freeze, independent response and evaluation;
- BTT-002 freeze, independent response and evaluation;
- cross-test convergence;
- Stage 11 determination that no third BTT is required.

**PMEDG STAGE 12 COMPLETE — GRADUATION-CANDIDATE SPECIFICATION PREPARED.**

**NEXT: STAGE 13 — PORTABLE-PACKAGE GRADUATION REVIEW.**
