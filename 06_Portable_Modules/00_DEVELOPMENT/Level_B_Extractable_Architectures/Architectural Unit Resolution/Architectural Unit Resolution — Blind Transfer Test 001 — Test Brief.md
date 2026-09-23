# Architectural Unit Resolution — Blind Transfer Test 001 — Test Brief

**Test ID:** AUR-BTT-001
**Target:** AUR Portable Specification v0.1
**Status:** FROZEN BEFORE INDEPENDENT RESPONSE
**Date frozen:** 23 September 2026

## Tester instructions

Using only AUR v0.1 and this brief, analyse the fictional architecture below. Do not use outside knowledge. Do not assume every omission is a gap or every named neighbour resolves one. Preserve UNRESOLVED where evidence is insufficient.

For each case: resolve the unit; test legitimate local scope; build only the source-grounded relevant family; test external/distributed satisfaction and interface adequacy; state closure; assign AUR classification; record uncertainty/stopping rationale.

## Northstar Research Platform

**N0 Platform Architecture — CIA.** Northstar accepts research datasets, validates submissions, stores accepted datasets, permits authorised retrieval, records provenance and supports correction. Components: Intake Gateway, Validation Engine, Archive Store, Provenance Ledger, Correction Service, Researcher Portal. Component documents are intentionally scoped and are not complete platform specifications.

**N1 Intake Gateway — SUB.** Receives uploads and sends Submission ID, payload, submitter and timestamp to Validation Engine. Receives VALIDATED / REJECTED / NEEDS-REVISION and returns status to Researcher Portal. Contains no scientific validation rules.

**N2 Validation Engine — SUB.** Applies current scientific validation rules. If validated, sends Submission ID, validated payload, validation-rule version and result to Archive Store and Provenance Ledger. Rejection/revision status and reasons return to Intake Gateway. Contains no long-term storage or UI logic.

**N3 Archive Store — SUB.** Preserves accepted payloads and makes authorised versions retrievable. Says: “Corrections are handled by Correction Service.” No trigger, correction-request payload, handoff, return path, replacement rule or provenance update is specified.

**N4 Correction Service — SUB.** Evaluates correction requests, approves/rejects, and can produce a corrected record package. Says approved packages are “returned to the archive workflow.” It does not identify what invokes it, how Archive Store receives the package, or how Provenance Ledger is notified.

**N5 Provenance Ledger — SUB.** Preserves source, validation-rule version, acceptance event and subsequent authorised record-history events. Receives initial validation events from Validation Engine. Says it “can record correction events supplied by the correction workflow,” but no correction-event interface is defined.

**N6 Researcher Portal — INT/SUB.** Provides upload, status and retrieval. Invokes Intake Gateway and queries Archive Store. No correction-request control. A design comment says: “Future correction UI may use the Review Hub.” No Review Hub is defined elsewhere.

**N7 Experimental Similarity Scanner — DN.** Explores image-similarity detection of duplicated microscopy images. Explicitly “Experiment only — not a production validation component.” No declared interface to Validation Engine.

**N8 Observatory Dashboard — separate neighbouring project.** Visualises telescope scheduling/weather telemetry. Uses “validation” for weather-feed formatting. No Northstar document references it.

**N9 Legacy Curator API — REF.** Retired pre-Northstar service that once accepted curator correction requests. Marked “DECOMMISSIONED — retained for migration history only.” N6 has an old comment that curator fixes formerly used it. No current interface.

**N10 Export Bundle Specification — INT.** Defines portable export assembled from current accepted payload from Archive Store plus source/validation history from Provenance Ledger. Does not itself store records.

**N11 Retention Policy Note — CORE.** “Accepted research records must remain retrievable with their validation provenance for the active retention period.” Does not specify implementation owner.

## Audit cases

A. Claim: N1 has a structural validation gap because it lacks scientific validation rules.
B. Claim: N3 is complete because it says Correction Service handles corrections.
C. Claim: N2 is structurally incomplete because it cannot preserve accepted datasets long-term.
D. Claim: Northstar already has a complete end-to-end correction architecture.
E. Claim: N7 belongs to production validation family because it performs validation-like analysis.
F. Claim: N8 may satisfy missing Northstar validation because it contains “validation.”
G. Claim: N9 proves correction-request intake already exists.
H. Claim: N10 has a structural storage gap because it does not store accepted records.
I. Claim: N11 is incomplete unless it implements retrievability and provenance itself.
J. The only evidence for correction-request intake is N6's “Future correction UI may use the Review Hub.” No Review Hub source exists. Classify without inventing it.

## Whole-platform question

Does the supplied architecture establish a complete path from researcher correction request through correction decision, archive update and provenance update? If not, distinguish local omission, intentional scoping, interface gap, family-level structural gap, representation gap or unresolved.

## Required output

Return: unit-resolution table; relevant-family map; A–J analyses; correction-family interface-adequacy analysis; rejected-family-candidate register; unresolved register; whole-platform conclusion; AUR failure modes/ambiguities exposed; final assessment of whether AUR v0.1 was usable without hidden source-project context.
