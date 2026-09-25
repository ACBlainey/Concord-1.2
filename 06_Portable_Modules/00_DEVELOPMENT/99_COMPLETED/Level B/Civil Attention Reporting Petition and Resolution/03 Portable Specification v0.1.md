# Civil Attention, Reporting, Petition and Resolution Module
## Portable Specification v0.1

**Author:** Alexander C. Blainey
**Project:** The Concord Framework
**Method:** PMEDG v1.2
**Date:** 25 September 2026
**Status:** PMEDG STAGE 4 / PORTABLE SPECIFICATION v0.1 / NOT GRADUATED

## 1. Purpose

This module provides a domain-neutral method by which a participant can cause a legitimate system to notice, preserve, classify, route, examine and respond to a suggestion, problem report, petition or related attention input.

It is designed so that the participant need not understand the host system's internal topology.

It does not give the participant unilateral authority over truth, priority, remedy, resource allocation or outcome.

## 2. Core Invariants

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

## 3. Core Object Separation

The module distinguishes:

**Submission Object ≠ Issue Object ≠ Investigation/Examination Object ≠ Finding/Decision Object ≠ Implementation/Remedy Object**

A Submission Object preserves what was actually received.

An Issue Object represents a problem/question/concern that requires processing.

Downstream objects represent later work without rewriting the original submission.

One submission may produce several Issue Objects.

Several submissions may attach to one Issue Object.

## 4. Input Classes

### Suggestion
A proposed improvement, solution or opportunity.

Its value does not depend on popularity. A low-support suggestion may be important if it plausibly addresses a significant known need.

### Problem Report
A report of a possible defect, harm, failure or undesirable condition.

> **Problem Report ≠ Established Problem**

Severity, evidence and verification matter more than popularity.

### Petition
A collective expression of concern, preference or requested action.

Support is a legitimate collective-attention signal.

> **Petition Support ≠ Problem Weight**

Petition volume does not itself establish factual truth, severity or entitlement to resources.

## 5. Common Processing Path

**Participant Trigger → Common Intake → Receipt → Original Preservation → Provisional Classification → Existing-Issue Match → Information-Sufficiency Assessment → Issue Creation / Attachment / Split / Merge → Evidence and Epistemic State → Functional Routing → Domain Action Object(s) → Domain Examination / Action → Mandatory Return → Central Resolution Record → Participant Feedback → Challenge / Escalation / Reopening where legitimate**

The exact host implementation may vary while preserving these functions and invariants.

## 6. Classification

The participant may suggest a classification, but this is advisory.

> **Submitter Classification = Advisory Context**

> **System Classification = Provisional Routing Decision**

Classification must be reviewable.

A useful classification record may include type, reason, confidence/uncertainty where justified, time, classifier and reviewability.

Multi-domain classification is permitted.

## 7. Information Sufficiency

Classification and information sufficiency are separate questions.

> **Classification ≠ Information Sufficiency**

The system asks whether enough information exists to take the next legitimate step.

Insufficient information must not silently become a finding that the report is false.

> **Insufficient Information ≠ False Report**

> **Currently Non-Actionable ≠ Permanently Closed**

> **Anonymity ≠ Non-Actionability**

> **Identity ≠ Evidentiary Sufficiency**

## 8. Issue Matching, Split and Merge

Issue Objects are created when needed, not automatically for every submission.

A new submission may:
- create a new Issue Object;
- attach to an existing Issue Object;
- cause an existing Issue to split;
- reveal several distinct Issues;
- supply new information to an existing Issue.

Similarity is not equivalence.

> **Common Topic ≠ Common Issue**

When submissions are grouped, their original provenance remains recoverable.

> **Merge for Processing ≠ Erase Individual Provenance**

## 9. Aggregation and Information Delta

The module separates:
- number of submissions/support expressions;
- distinguishable sources where legitimately knowable;
- source-independence assessment;
- materially distinct information;
- corroborating evidence;
- contradictory evidence.

> **Raw Count ≠ Independent Participants**

> **Independent Participants ≠ Independent Evidence**

> **Duplicate Processing ≠ Duplicate Information**

Repeated unchanged information need not restart processing.

Material information delta can change the Issue state.

> **Case State(t+1) = Case State(t) + Evaluated Information Delta**

Aggregate actionability does not establish every individual report as substantiated.

## 10. Attention, Truth, Priority and Resources

The module maintains a firewall between:

1. **Intake Layer** — what was submitted;
2. **Attention / Epistemic Layer** — what deserves examination and what evidence supports;
3. **Problem / Resource Layer** — actual problem state, priority and legitimate resource response.

> **Intake Pressure May Trigger Re-Evaluation; It Must Not Directly Command Problem Priority or Resource Allocation.**

> **Cost of Processing Attention ≠ Weight of the Problem**

Volume thresholds, where a host uses them, trigger additional evaluation rather than automatic substantive priority.

## 11. Domain Routing

A common intake may route one Issue to one or several legitimate functional owners.

Each route creates or binds a **Domain Action Object (DAO)**.

A DAO should preserve at least:
- parent Issue reference;
- routing reason;
- responsible function;
- acceptance/transfer state;
- processing state;
- last material action;
- dependencies;
- disposition;
- next review condition where applicable;
- bounded return information;
- provenance.

> **One Front Door; Many Legitimate Functional Owners.**

## 12. Mandatory Return Path

Every outbound route requires a return path.

A domain should return bounded information sufficient for the parent Issue to know its processing state without requiring universal access to domain data.

Possible states include received, accepted, transferred, awaiting information, under examination, action authorised, action in progress, no action justified, outside authority, deferred with reason, blocked by dependency, resolved, escalated and closed subject to reopening.

> **Every Outbound Route Requires a Return Path.**

## 13. Problem State and Response State

The module separates:

### Problem State
The current best-supported representation of the underlying issue.

### Response State
What legitimate functions have done, are doing, failed to do or are waiting upon.

> **Problem-State Stability ≠ Response-State Adequacy**

A problem may remain unchanged while institutional response becomes inadequate.

## 14. Responsibility Resolution

If ordinary routing cannot establish legitimate ownership, the Issue remains recognised.

A **Responsibility Resolution Object (RRO)** may preserve:
- parent Issue;
- domains considered;
- routing reasons;
- acceptance/refusal/transfer history;
- disputed responsibility;
- unresolved functional need;
- current resolver;
- escalation route;
- ownership disposition.

The RRO determines who must process a function. It does not determine the substantive outcome.

## 15. Dependencies

DAOs may be independent, sequential, mutually dependent, conditionally dependent, blocked by another domain or jointly required.

Dependency representation must support coordination without transferring substantive authority.

A waiting state should identify where possible:

**Waiting For + Dependency Owner + Required State/Information + Review Condition + Backstop + Next Responsible Function**

> **Waiting Without a Represented Condition Is a Staleness Risk.**

## 16. Queue Vitality and Deferral

The module may bind to a legitimate scheduler/review-trigger mechanism.

It must preserve:

> **Deferral Requires a State, Reason and Review Condition.**

Significant deferral events should remain visible.

**Deferral Event = <time/state, reason, owner, blocking basis, review condition, outcome>**

> **Replacing a Review Date Must Not Erase the History of Deferral.**

A BLOCKED state should identify its blocking basis where possible.

> **Blocked Is a Claim About State, Not an Exemption From Accountability.**

A triggered review should produce a meaningful outcome where one is required.

> **Review Performed ≠ Review Resolved**

> **Timestamp Refresh ≠ Meaningful State Update**

## 17. Urgency

A high-consequence claim may justify rapid examination or protective routing without being treated as proven.

Urgency may change routing speed and protective action through legitimate host authority.

Civil Attention does not itself acquire emergency powers.

## 18. Protected Information

The central/common layer receives only information necessary for routing, status, coordination, review and participant feedback.

Protected substantive evidence may remain with its legitimate domain.

A domain may return bounded status or condition results without exposing underlying protected material.

## 19. Individual and Systemic Issues

A participant's immediate problem may reveal a broader systemic defect.

The two may be linked but independently processed.

> **Systemic Investigation ≠ Reason to Delay an Available Individual Remedy**

Resolving an individual's case does not automatically close the systemic Issue.

## 20. Challenge, Review and Reopening

A participant may legitimately challenge classification, missed evidence, stale information, conflict of interest, implementation failure, materially changed circumstances or overlooked rights/safety implications.

> **Right to Challenge Processing ≠ Right to Dictate Outcome**

Unchanged repetition may be attached/preserved without full re-examination.

Material information delta or a legitimate review ground may trigger re-evaluation.

Closure does not erase provenance.

## 21. Feedback

Participant feedback should, where legitimately possible, answer:

**Current State + Reason + Responsible Function(s) + Last Material Action + Next Review Condition**

Protected information may limit detail but must not be used to conceal absence of processing.

## 22. Host Interface Requirements

The host must provide or bind legitimate mechanisms for functions it requires, including:
- durable receipt/persistence;
- identity/standing where required;
- substantive domain authority;
- evidence/verification;
- privacy/protected information;
- escalation/review authority;
- scheduler/review triggers;
- resource allocation;
- emergency authority where applicable.

The module does not manufacture missing authority.

## 23. Core and Companion Contract

The portable core is versioned independently from domain companions.

**Core Method Version N + Domain Companion + Bound Host Services → Domain Implementation**

A companion may specify:
- domain terminology;
- local evidence requirements;
- authority/jurisdiction boundaries;
- confidentiality rules;
- domain processing states;
- escalation routes;
- scheduler/Clock conditions;
- permitted dispositions;
- domain-specific feedback constraints;
- interfaces to specialist systems.

A companion may not:
- redefine a core invariant;
- convert participant attention into command authority;
- remove provenance requirements;
- remove the mandatory return path;
- turn popularity into truth/priority;
- make central visibility into central substantive control;
- erase reviewability solely for local convenience;
- silently modify the core version.

> **Domain Requirement ≠ Core Method Amendment**

> **Companion Extension ≠ Core Override**

> **Local Adaptation Must Preserve Core Invariants**

## 24. Core Revision Rule

If a domain discovers a requirement that appears to conflict with or improve the core:

1. preserve the current core unchanged;
2. record the domain finding;
3. determine whether it is local or general;
4. submit general candidates to controlled core review;
5. revise/version the core only if justified;
6. regression-test affected companions against the revised core.

> **Domain-Specific Need Is Evidence for Review, Not Permission for Drift.**

## 25. Minimum Auditability

A host implementation should preserve enough provenance to reconstruct:
- what was submitted;
- what Issue(s) it became associated with;
- classification/routing changes;
- responsible owners;
- significant evidence/information changes;
- dispositions;
- significant deferrals;
- challenge/review outcomes;
- overall resolution;
- feedback state.

## 26. Non-Goals

This module does not prescribe:
- a universal database schema;
- a universal user interface;
- a universal priority algorithm;
- universal numerical thresholds;
- a universal identity system;
- substantive domain law/policy;
- domain-specific evidence standards;
- resource allocation formulas;
- emergency powers;
- surveillance authority.

## 27. v0.1 Testable Claims

A portable implementation should be able to demonstrate that:
1. a participant can submit without knowing internal topology;
2. original provenance survives processing;
3. multiple submissions can converge on one Issue without evidence collapse;
4. one submission can produce several Issues;
5. one Issue can route to several domains;
6. domains retain substantive authority;
7. every route has a return path;
8. unresolved ownership does not erase the Issue;
9. waiting dependencies can reactivate;
10. difficult work cannot become silently inert;
11. participant volume cannot directly manufacture truth/priority/resources;
12. protected data need not be centralised;
13. individual and systemic resolution remain distinct;
14. challenge/reopening is possible without participant command authority;
15. a domain companion can add legitimate nuance without modifying the core.

## PMEDG Status

**STAGE 4 COMPLETE — PORTABLE SPECIFICATION v0.1**

**NEXT: STAGE 5 — FREEZE BTT-001 TEST BRIEF AND HIDDEN EXPECTED-FINDINGS / EVALUATION KEY**
