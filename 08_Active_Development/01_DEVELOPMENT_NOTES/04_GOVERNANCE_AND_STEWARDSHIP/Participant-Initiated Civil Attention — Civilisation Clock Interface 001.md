# Participant-Initiated Civil Attention — Civilisation Clock Interface 001

**Author:** Alexander C. Blainey
**Project:** The Concord Framework
**Date:** 25 September 2026
**Status:** ACTIVE DEVELOPMENT / SOURCE-RESOLVED INTERFACE / NON-CANONICAL

## Purpose

Civil Attention requires a way to keep unresolved Issue Objects and Domain Action Objects from becoming inert while waiting for reviews, dependencies or inter-domain information.

Source resolution shows that this function already belongs to the Civilisation Clock source family. The Clock is defined as a **State-Transition Scheduler + Review-Trigger Architecture**, with temporal, state, dependency, event, risk, recurrence, evidence, participant and compound triggers. STRA also supplies routing-unresolved, uncertainty, stale-trigger review and bounded backstops.

The interface therefore reuses the existing Clock rather than inventing another scheduler.

## Core interface

**Issue / Domain Action State → Clock Trigger → Condition or Backstop Reached → Review Candidate / Prompt → Legitimate Domain or Resolution Owner → Action / State Update**

> **Triggering Review ≠ Authority Over Outcome**

The Clock can trigger review or communication. It does not decide the substantive case.

## Represented waiting

A queue item should not merely say WAITING. Where possible it should represent:

**Waiting For + Dependency Owner + Required State/Information + Review Condition + Backstop + Next Responsible Function**

Example:

**DAO-B waits for DAO-A finding F → Clock watches DAO-A → F becomes available → DAO-B becomes review-due → its legitimate owner is prompted.**

> **Waiting Without a Represented Condition Is a Staleness Risk.**

## Queue vitality and difficult work

Clock triggers may support next-review conditions, dependency completion, inter-domain communication prompts, Response-State reassessment, responsibility review, evidence or Problem-State change, and temporal backstops.

A domain queue can become distorted if easy work is repeatedly selected while difficult legitimate problems remain indefinitely deferred. The Clock should not assign substantive priority, but it can make deferral visible and require a reason and review condition.

> **Deferral Requires a State, Reason and Review Condition.**

A difficult case may legitimately remain unresolved because evidence, capability, authority or resources are missing. In that case the dependency should be represented.

**Issue H blocked by Capability C → watch C → C becomes available, validated or authorised → review H.**

A temporal backstop can still check whether the dependency model itself has become stale. This prevents both futile constant reconsideration and permanent forgetting.

> **No Actionable Issue Should Become Inert Merely Because It Is Waiting.**

## Timing boundary

Different domains legitimately operate at different speeds.

> **Age of Queue Item ≠ Problem Weight**

> **Elapsed Time Alone ≠ Process Failure**

but:

> **Missed Legitimate Review Condition → Response-State Reassessment**

Time can therefore reveal a response-state problem without manufacturing substantive problem priority.

## Inter-domain communication

Where one Domain Action Object depends on another, the Clock may prompt the relevant coordination owners when a legitimate review or backstop condition is reached.

The prompt may request a status or dependency update and cause the Central Resolution Record to be refreshed.

> **Prompting Communication ≠ Authority to Demand a Particular Substantive Result.**

## Oversight interface

Resolution Oversight may consume Clock state to detect:
- review due or overdue;
- unresolved dependency;
- routing unresolved;
- trigger unknown or disputed;
- action pending;
- repeated deferral;
- stale trigger definition;
- missing owner;
- completed domain work awaiting parent reconciliation.

Oversight may initiate the legitimate review route without substituting its judgment for the domain owner.

## Queue accountability

For unresolved actionable work, a domain should expose bounded status sufficient to identify current state, responsible function, reason for waiting or deferral, dependency, next review condition, Clock trigger or backstop where applicable, and last material action.

A queue containing old or difficult work is not automatically defective. A queue containing unresolved work with **no represented reason, owner or review path** is a stronger warning.

## Submission boundary

Participants should not be able to accelerate Clock escalation by repeatedly resubmitting unchanged information. Clock conditions attach primarily to the Issue Object, Domain Action Objects, dependencies and legitimate review states.

> **Repeated Submission ≠ Repeated Clock Escalation**

Material information delta may legitimately change the trigger state.

