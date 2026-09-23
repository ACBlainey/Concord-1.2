# Continuity Protocol — Blind Transfer Test 002 — Delta Test Brief

**Test:** CP-BTT-002  
**Specification under test:** Continuity Protocol — Portable Specification v0.2  
**Test type:** Independent blind transfer / delta test / non-Concord domain  
**Status:** FROZEN TEST BRIEF  
**Date:** 23 September 2026

## 1. Tester instruction

Use only this test brief and the supplied Continuity Protocol portable specification v0.2.

Do not inspect the Concord source architecture, BTT-001, development notes, expected-findings key or prior discussion.

Apply the specification as written. Preserve unresolved facts. Do not assume that documentation, authority, redundancy or successful activation automatically establishes continuity.

## 2. Scenario — Pelagos Island Water Cooperative

Pelagos is a fictional island cooperative that supplies drinking water to five settlements through desalination, storage and gravity distribution.

The continuity target is to preserve **safe minimum water service** through equipment ageing, supplier withdrawal, staff turnover and eventual replacement of the current plant.

### P0 — Declared targets

Normal output is 4.0 million litres/day.

The island authority has independently defined the **Minimum Acceptable Function (MAF)** during an emergency as 1.4 million litres/day of treated water delivered to designated community storage points.

Declared targets:

- **RTO:** MAF must be restored within 18 hours of loss of the primary plant.
- **RPO:** operational water-quality and dosing records may be no more than 2 hours old at recovery.
- Full service may be restored later.

The declared disruption envelope for the primary recovery claim is:

> loss of the desalination plant building and its installed control equipment, while the rest of the island remains physically accessible.

It does not automatically include island-wide port closure, loss of all communications or regional fuel unavailability.

### P1 — Atlas plant

Atlas is the current desalination plant. It is operational and exceeds normal demand.

Its control system was installed 17 years ago.

### P2 — Daily control archive

Every 24 hours Atlas exports control configuration, dosing settings and operating records to an off-site municipal server.

The archive is documented, readable and has been restored into a simulator.

Because export occurs once per day, up to 24 hours of operating records may be absent after disruption.

### P3 — Rapid standby plant

A separate standby unit, Swift, can produce 1.6 million litres/day.

It has independent local controls and has passed a full production test.

Operators can start it within 6 hours.

However, Swift's water-quality log synchronises from Atlas only every 8 hours.

### P4 — Paper chemistry procedures

Current treatment procedures are printed at two community sites. Operators have used them successfully during exercises.

They do not contain control-system configuration.

### P5 — Membrane supplier

Atlas uses a membrane model that its manufacturer will stop producing next year.

The cooperative has a documented statement from the supplier confirming end-of-production.

A compatible replacement is being investigated but has not been selected or tested.

### P6 — Alleged calibration dongle

A retired technician remembers that early Atlas commissioning may have used a proprietary calibration dongle.

Current engineers cannot find the dongle and have operated and recalibrated Atlas for nine years without seeing it.

No current procedure mentions it.

It is unknown whether it would be needed for a complete rebuild.

### P7 — Mira

Mira is the only engineer who understands a locally written conversion script that translates old Atlas sensor identifiers into the cooperative's historical database.

The script source code exists and is documented at a high level, but a recent engineer could not explain two transformation rules.

Mira is leaving in three months.

### P8 — New Tide plant

A replacement plant, Tide, is under construction.

It uses different membranes, controls and sensor identifiers.

Acceptance tests show it can produce 4.2 million litres/day and meet water-quality requirements.

Historical record migration has not yet been completed.

### P9 — Authority for Tide

The island authority has formally approved Tide to become the replacement production plant once commissioning conditions are satisfied.

The approval is valid and independently evidenced.

### P10 — Handoff defect

Although Tide has legitimate authority to replace Atlas, the operating team has not received:

- the complete historical sensor mapping;
- Mira's two unexplained transformation rules;
- a verified method for connecting Tide's records to the historical database.

### P11 — Fast recovery exercise

A disaster exercise destroyed the simulated Atlas environment.

Swift reached 1.6 million litres/day after 5 hours and water quality remained within limits.

The restored operational record set was 7 hours old.

Management declared that the exercise “met the continuity target because service returned inside the RTO.”

### P12 — Old emergency manual

A 2018 emergency manual is complete, readable and easy to follow.

It instructs staff to activate a chlorine dosing arrangement retired in 2023 after the treatment process changed.

The current manual supersedes it and records why.

### P13 — Continuity spreadsheet

The cooperative's continuity spreadsheet was created eight years ago.

It still lists:

- a former membrane supplier;
- a staff member who left five years ago;
- a recovery server that has been decommissioned.

The spreadsheet is still formally designated as the organisation's “master continuity plan.”

### P14 — Port dependency

Replacement membranes and several treatment chemicals arrive through the island port.

The primary disruption envelope does not include port closure.

A reviewer nevertheless argues that because an extended port closure could eventually stop water production, the primary plant-loss continuity claim must automatically be classified as failed.

### P15 — Fuel store

Swift requires diesel.

The island has a verified independent fuel store sufficient for 72 hours at MAF output.

The continuity target requires only the first 18 hours to reach MAF, but a separate long-duration resilience review has not yet been performed.

## 3. Tasks

### Task A — Resolve the continuity object and target

State the continuity object, MAF, RTO, RPO and disruption envelope. Explain why they must be evaluated separately.

### Task B — Apply object-relative CS classification

Evaluate P2, P3, P4 and P12. Distinguish the state of an artefact/component from the state of the whole continuity claim.

### Task C — Evaluate the fast recovery exercise

Determine whether P11 satisfies the declared continuity target. Treat RTO and RPO independently.

### Task D — Evaluate MAF

Determine whether Swift satisfies the functional MAF and what its 72-hour fuel basis does and does not establish.

### Task E — Dependency evidence and criticality

Classify P5, P6, P7 and P15 using VERIFIED / DOCUMENTED / INFERRED / UNRESOLVED where useful, and assess criticality relative to the declared target.

Do not invent the calibration dongle's role.

### Task F — Function versus implementation

Determine whether Tide can provide continuity despite replacing Atlas.

### Task G — Succession and authority

Evaluate P9 and P10. Determine whether legitimate authority is sufficient for successful continuity succession.

### Task H — Historical/current validity

Evaluate P12. Distinguish technical actionability/readability from validity for current restoration.

### Task I — Continuity mechanism fossilisation

Evaluate P13. Determine what it says about continuity of the continuity mechanism itself.

### Task J — Disruption-envelope discipline

Evaluate P14. Determine whether a port-closure risk invalidates the bounded primary claim and how it should instead be handled.

### Task K — Overall classifications

Apply CP-C1–CP-C10 as appropriate to:

1. Swift MAF functional recovery;
2. P11 overall declared continuity target;
3. Atlas rebuild dependency state;
4. Tide succession;
5. the master continuity spreadsheet.

### Task L — Minimal continuity record

Produce a concise record using the v0.2 template.

## 4. Required final assessment

Conclude with:

1. whether v0.2 was usable without source context;
2. whether the new RTO/RPO, MAF, Disruption Envelope and evidence-state concepts reduced ambiguity;
3. any remaining ambiguity;
4. any false-positive/false-negative pressure created by v0.2;
5. whether another revision is needed before graduation review.

Do not inspect or infer an unpublished answer key.
