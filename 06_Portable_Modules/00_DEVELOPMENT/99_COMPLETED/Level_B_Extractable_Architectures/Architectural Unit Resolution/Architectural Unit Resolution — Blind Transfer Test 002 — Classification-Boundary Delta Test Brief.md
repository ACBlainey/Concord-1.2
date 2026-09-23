# Architectural Unit Resolution — Blind Transfer Test 002 — Classification-Boundary Delta Test Brief

**Test ID:** AUR-BTT-002  
**Target:** Architectural Unit Resolution — Portable Specification v0.2  
**Test type:** Focused blind delta test  
**Status:** FROZEN BEFORE INDEPENDENT RESPONSE  
**Date frozen:** 23 September 2026

## 1. Purpose

Test only the v0.2 clarifications exposed by BTT-001:

- local scope versus architectural satisfaction;
- C2 versus C3;
- C6 versus C7 at sub-function resolution;
- current versus historical versus candidate dependencies;
- diagnostic closure versus functional satisfaction;
- preservation of C9 where the evaluation space is insufficient.

This is not a repeat of BTT-001.

## 2. Tester instructions

Using only AUR v0.2 and this brief, analyse the fictional **Harbourlight Access Network** below.

Do not use outside knowledge. Do not invent missing components or interfaces.

For each case record:

1. local ownership/scope state;
2. relevant family;
3. dependency status where relevant;
4. whether the family can close diagnostically;
5. whether the tested function is actually satisfied;
6. AUR classification;
7. uncertainty/stopping rationale.

## 3. Harbourlight architecture

### H0 — Harbourlight Access Network

**Status:** integrated architecture.

Harbourlight manages access to a distributed collection of research facilities. It states that credential issuance, door enforcement, access-event recording and appeal are separate functions.

### H1 — Registration Portal

**Status:** subsystem.

Collects identity and affiliation information and submits a complete registration package to Credential Service.

It explicitly states:

“Registration Portal does not decide access eligibility.”

The handoff to Credential Service is fully defined and returns APPROVED / REJECTED plus Credential ID where approved.

### H2 — Credential Service

**Status:** subsystem.

Determines eligibility and issues credentials.

It sends active credential ID, permitted facility set and expiry to Door Enforcement.

It receives revocation events from Revocation Service.

### H3 — Door Enforcement

**Status:** subsystem.

Checks presented credential ID, facility and expiry against active permission data from Credential Service.

Every allow/deny event is sent to Event Ledger.

H3 contains no registration UI and no appeal logic.

### H4 — Event Ledger

**Status:** subsystem.

Receives allow/deny events from H3 and preserves them.

### H5 — Appeal Policy Note

**Status:** core constraint.

States:

“Every rejected registration must have access to an appeal process.”

It does not implement appeal.

### H6 — Appeal Service

**Status:** subsystem.

Can receive an Appeal Package, review it and issue UPHOLD / OVERTURN.

Its input schema is fully defined.

No current Harbourlight component is documented as creating or sending an Appeal Package.

No return interface from H6 to H2 is documented.

### H7 — Old Appeals Form

**Status:** reference/provenance source.

Marked:

“RETIRED two years before current Harbourlight release.”

It once created Appeal Packages for an earlier Appeal Service version.

No current interface points to H7.

### H8 — Participant Dashboard

**Status:** subsystem/interface.

Shows registration result and active credentials.

A roadmap note says:

“Appeal button planned for next release; expected to use Appeals Gateway.”

No Appeals Gateway specification is supplied.

### H9 — Safety Revocation Service

**Status:** subsystem.

Receives a defined Safety Revocation Notice from authorised facility safety systems and sends Credential ID + revocation reason + timestamp to H2.

H2 confirms revocation and propagates inactive status to H3.

The complete trigger, handoff, return and propagation chain is specified.

### H10 — Cafeteria Loyalty App

**Status:** separate neighbouring project.

Uses Harbourlight employee IDs for meal discounts. It contains a function named “eligibility review.”

No Harbourlight architecture references H10.

### H11 — Visitor Orientation Guide

**Status:** companion document.

Explains how approved visitors present credentials at doors. It explicitly says technical access decisions are performed by H3.

It is not intended to define credential issuance, revocation or appeal.

### H12 — Emergency Override Requirement

**Status:** core constraint.

States:

“Emergency responders must be capable of obtaining time-bounded emergency access.”

No supplied current component, interface or candidate service implements emergency access.

The requirement is explicitly marked **mandatory for the current release**.

### H13 — Analytics Export

**Status:** interface specification.

Exports selected Event Ledger records to authorised researchers. H13 explicitly depends on H4 for event storage and contains no local storage.

### H14 — Federation Adapter

**Status:** subsystem/interface.

A comment says:

“Future federation may obtain credentials from an external Federation Broker.”

No broker identity, specification or current deployment evidence is supplied. Federation is marked **future / not current release**.

## 4. Audit cases

### A — H1 eligibility

Claim: “H1 is incomplete because it does not decide access eligibility.”

### B — H3 appeal

Claim: “H3 has an appeal gap because it contains no appeal logic.”

### C — H6 appeal workflow

Claim: “Because H6 can decide appeals, Harbourlight's appeal requirement is satisfied.”

### D — H7 historical appeal form

Claim: “H7 proves current appeal intake exists.”

### E — planned Appeals Gateway

Classify the roadmap reference without inventing the gateway.

### F — H9 revocation

Determine whether revocation is externally/distributedly satisfied and whether diagnostic closure differs from functional satisfaction.

### G — H10 eligibility review

Determine whether H10 belongs to the access-eligibility family.

### H — H11 visitor guide

Claim: “H11 has a credential-decision gap because it cannot decide access.”

### I — H12 emergency access

Determine whether the current family contains an interface gap or a family-level structural gap for mandatory emergency-access capability.

### J — H13 storage

Claim: “H13 has a structural storage gap.”

### K — H14 future federation

Classify the Federation Broker reference and whether any current-release gap follows from its absence.

## 5. Mixed workflow question

For the current-release appeal requirement, distinguish at sub-function level:

- existence of appeal-decision capability;
- creation/intake of Appeal Package;
- H6 invocation;
- consequence propagation back to credential state.

State which are C6, C7 or C9, if any.

## 6. Required output

Return:

1. unit/scope table;
2. current-family map;
3. dependency-status register;
4. A–K analyses;
5. appeal sub-function decomposition;
6. emergency-access analysis;
7. diagnostic-closure versus functional-satisfaction table;
8. unresolved register;
9. ambiguities/failure modes exposed;
10. final assessment of the v0.2 delta.
