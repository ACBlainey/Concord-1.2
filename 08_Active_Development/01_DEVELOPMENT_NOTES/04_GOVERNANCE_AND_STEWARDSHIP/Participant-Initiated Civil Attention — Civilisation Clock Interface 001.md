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

