# Civil Attention, Reporting, Petition and Resolution — Source Resolution and Extraction Audit

**Method:** PMEDG v1.2
**Status:** PMEDG STAGE 3 — EXTRACTION AUDIT

## Audit Question

Can a coherent domain-neutral method be extracted from the Concord Civil Attention development programme without importing Concord-specific substantive authority or silently omitting required source-owned functions?

## Finding

**YES — EXTRACTION JUSTIFIED.**

The tested architecture contains a stable common method that survived internal historical regressions, aggregation/pressure tests, institutional failure tests, cross-domain routing tests, Clock queue-vitality tests and materially different operational-domain tests.

The common architecture remained stable while domain-specific substantive processing varied.

## Portable Core Boundary

The extracted module should own:
1. participant-triggered common intake semantics;
2. input-class semantics;
3. original-submission preservation;
4. provisional/reviewable classification;
5. issue matching and Issue Objects;
6. split/merge/provenance rules;
7. information/evidence state separation;
8. aggregation and information-delta rules;
9. domain routing and Domain Action Objects;
10. responsibility resolution when ownership fails;
11. dependency representation;
12. mandatory return/status path;
13. Problem State and Response State;
14. central resolution visibility;
15. feedback;
16. challenge/review/reopening interfaces;
17. queue-vitality interface to an external scheduler/Clock;
18. deferral accountability;
19. protected-information minimum-return principle;
20. individual/systemic resolution separation.

## Required Host Interfaces

A host system must provide or bind legitimate implementations for:
- receipt/persistence;
- identity/standing where required;
- substantive domain owners;
- domain authority;
- evidence/verification processes;
- privacy/protected information;
- review/escalation authority;
- scheduler/review triggers where queue vitality is required;
- resource allocation;
- emergency routing where applicable.

The portable module specifies interface requirements; it does not invent these authorities.

## Core/Companion Invariant

A domain implementation must be composed as:

**Core Method Version N + Companion for Domain D + Bound Host Authorities/Services**

The companion may narrow, add or specify domain procedure where the core deliberately delegates to the host.

It may not contradict or locally rewrite a core invariant.

If a domain requirement appears incompatible with the core:
1. preserve the core unchanged;
2. record the conflict;
3. determine whether the issue is domain-specific or general;
4. if general, submit it to controlled core revision/back-propagation;
5. version and regression-test any accepted core revision.

> **Domain-Specific Need Is Evidence for Review, Not Permission for Drift.**

## Extraction Risks

Primary risks for the portable specification are:
- accidentally embedding Concord-specific names as universal authorities;
- turning participant attention into participant command;
- turning aggregation into truth/priority;
- centralising domain judgment;
- allowing companions to override core invariants;
- treating scheduler/Clock prompts as authority;
- over-specifying implementation details not established by evidence;
- declaring internal tests equivalent to independent validation.

These risks can be controlled in the portable specification and BTT tests.

## PMEDG Decision

**STAGE 3 PASSED.**

Proceed to **Stage 4 — Portable Specification v0.1**.

The specification should be written in domain-neutral language and explicitly define the companion-method extension contract before blind testing.
