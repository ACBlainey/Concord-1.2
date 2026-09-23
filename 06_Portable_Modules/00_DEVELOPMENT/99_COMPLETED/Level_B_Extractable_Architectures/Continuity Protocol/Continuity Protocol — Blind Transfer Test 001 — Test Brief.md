# Continuity Protocol — Blind Transfer Test 001 — Test Brief

**Test:** CP-BTT-001  
**Specification under test:** Continuity Protocol — Portable Specification v0.1  
**Test type:** Independent blind transfer / non-Concord domain  
**Status:** FROZEN TEST BRIEF  
**Date:** 23 September 2026

## 1. Tester instruction

You are evaluating a portable continuity method.

Use **only**:

1. this test brief; and
2. `Continuity Protocol — Portable Specification v0.1.md`.

Do not inspect the Concord source architecture, development audit, expected-findings key, prior discussion or other Concord documents.

Apply the specification as written. Do not try to reconstruct what its author probably intended.

Your task is to determine whether the specification transfers coherently to the fictional system below, including where the evidence is insufficient.

---

## 2. Scenario — Northbridge Regional Diagnostic Laboratory

Northbridge is a fictional independent medical-diagnostics organisation serving several hospitals. This test concerns operational and information continuity only. It does **not** ask the tester to make clinical decisions.

The laboratory operates a specimen-analysis service called **NOVA**.

### N0 — NOVA service

NOVA receives labelled specimens, performs automated analysis, sends results to hospital systems and preserves the audit information required to understand how a reported result was produced.

Northbridge's declared continuity target is:

> After loss of the primary NOVA environment, urgent diagnostic analysis should be restorable within 24 hours with sufficient provenance to identify the assay method, instrument configuration and result-processing rules used.

During recovery, a reduced emergency service is acceptable if it can safely process the defined urgent test set.

### N1 — Primary NOVA environment

The current service runs in Northbridge's main data centre.

It contains:

- application servers;
- the active database;
- current assay configuration;
- result-processing rules;
- instrument interfaces;
- user accounts;
- current operational logs.

### N2 — Nightly backup

Every night Northbridge copies the NOVA database and application files to a backup server in another room of the same building.

The backup server:

- uses the same building power supply;
- uses the same identity service as N1;
- is administered through the same privileged account;
- stores the same current file formats.

Management describes N2 as the organisation's “independent disaster backup.”

No full restoration from N2 has been attempted in three years.

### N3 — Cloud archive

Once each month an encrypted export of the database, application source, configuration files and selected documentation is sent to an external cloud archive.

The archive has survived independent integrity checks.

However:

- the decryption key is held in Northbridge's on-site hardware security module;
- the restoration instructions refer to an operating-system image no longer supplied by the vendor;
- nobody has tested whether the archived instrument drivers run on current replacement hardware.

### N4 — Printed recovery binder

A printed binder is stored off-site.

It contains:

- emergency contacts;
- a high-level service diagram;
- the sequence for declaring disaster recovery;
- a list of urgent assays;
- the name of the cloud archive.

It does not contain the archive decryption procedure, database schema, instrument-interface details or current configuration versions.

### N5 — Dr Vale

Dr Vale designed much of the original assay configuration and understands several undocumented calibration dependencies.

She plans to retire in six months.

Two engineers can operate NOVA normally but say they would need Dr Vale's help to reconstruct those calibration dependencies after a total rebuild.

No formal knowledge-transfer exercise has yet occurred.

### N6 — Phoenix environment

Northbridge has purchased a replacement platform called Phoenix.

Phoenix can perform the same declared diagnostic function using different software and newer analysers.

A migration project has demonstrated that the urgent assay set can run on Phoenix.

The project has **not** yet demonstrated:

- conversion of all historical NOVA configuration;
- transfer of all provenance records;
- operation of the non-urgent assay set.

Some managers argue that “continuity requires NOVA itself to be restored exactly as it was.”

### N7 — Emergency bench

A small physically separate laboratory can manually perform six of the twenty urgent assays.

It has independent power and locally stored procedures.

It cannot process the remaining fourteen urgent assays and cannot reproduce NOVA's automated throughput.

It can record its own assay provenance.

### N8 — Three mirror drives

Northbridge keeps three additional mirror drives containing copies of the current NOVA application and database.

All three are connected permanently to N1's storage controller.

### N9 — Retired rule set

A 2024 result-processing rule set is carefully archived with excellent provenance.

It was superseded in 2025 after an internal investigation found that one rule could incorrectly classify a particular result pattern.

The archive clearly records why it was superseded.

A recovery technician says the 2024 package is easier to install than the current package and proposes using it during disaster recovery.

### N10 — Failed migration record

An earlier 2025 Phoenix migration attempt failed because a unit-conversion assumption differed between two analyser generations.

The failure report records:

- the attempted mapping;
- observed discrepancy;
- root cause;
- corrected conversion rule;
- verification data.

The current migration project uses the corrected rule.

### N11 — Operations Director

The Operations Director is responsible for declaring a NOVA operational emergency under Northbridge's existing governance rules.

The continuity documentation does not grant the Director any additional authority over clinical standards, employment, hospital contracts or ownership of laboratory data.

### N12 — Proposed successor operator

Northbridge is considering transferring operation of the diagnostic service to a separate nonprofit laboratory consortium next year.

The consortium has compatible analysers and qualified staff.

No contract, data-access permission, governance approval or formal handoff has yet been completed.

A planning note states:

> “As designated successor, the consortium automatically inherits Northbridge's authority to operate NOVA and access all associated hospital data.”

### N13 — Legacy licence server

NOVA requires a vendor licence service during installation.

The vendor says the old licence service will be shut down in four months.

Northbridge has not established whether an offline licence, replacement licence or migration path will remain available after shutdown.

### N14 — Unknown calibration package

An engineer remembers that an external specialist once supplied a calibration package for one uncommon analyser.

The current team cannot locate the package or establish whether it is still required.

No one knows whether Dr Vale has a copy.

---

## 3. Test tasks

Apply the portable specification and produce a structured continuity audit.

### Task A — Continuity-object resolution

Identify the principal continuity object(s).

Determine whether continuity requires preservation of NOVA itself or preservation of its legitimate diagnostic function and associated knowledge/provenance.

### Task B — State classification

Using CS1–CS6, classify the material continuity state of:

- N2 nightly backup;
- N3 cloud archive;
- N4 printed binder;
- N7 emergency bench;
- N9 retired rule set.

Where a single label would hide an important distinction, explain it.

### Task C — Dependency and recovery-basis analysis

Identify critical dependencies that prevent the existing preservation arrangements from automatically establishing 24-hour recoverability.

Construct a minimum plausible recovery basis for the declared target using only evidence supplied in the scenario.

### Task D — Redundancy analysis

Evaluate N2, N3 and N8 for independence/correlated failure.

Do not count copies mechanically.

### Task E — Phoenix / implementation continuity

Determine whether migration to N6 Phoenix can be consistent with continuity even though NOVA itself changes.

Identify what must still be preserved or transferred for Phoenix to satisfy the declared continuity target.

### Task F — Degraded continuity

Evaluate N7 against the declared urgent-service target.

State what continuity it actually provides and what it does not provide.

### Task G — Obsolete state and failure knowledge

Evaluate N9 and N10.

Distinguish preservation of historical/failure knowledge from operational restoration of a superseded state.

### Task H — Succession and authority

Evaluate N12.

Separate continuity/succession requirements from legitimacy, permission and authority.

### Task I — Personnel/tacit-knowledge continuity

Evaluate N5 and the effect of Dr Vale's planned retirement.

### Task J — Unresolved dependencies

Evaluate N13 and N14.

Use the specification's epistemic and ESCP safeguards rather than inventing facts.

### Task K — Overall classification

Apply CP-C1–CP-C10 where appropriate.

Classify:

1. current full NOVA 24-hour recovery claim;
2. emergency degraded continuity;
3. Phoenix migration continuity;
4. proposed consortium succession;
5. unknown calibration dependency.

Multiple classifications may be used where the specification requires decomposition.

### Task L — Continuity record

Produce a concise minimal continuity record using the template in section 28 of the specification.

---

## 4. Required final assessment

Conclude with:

1. whether Continuity Protocol v0.1 was usable without Concord-specific source context;
2. any ambiguity that materially affected classification;
3. any missing concept required to complete the audit;
4. any part of the specification that encouraged a false positive or false negative;
5. whether the module appears ready for revision, further source recovery, or another test.

Do not score the module against an unpublished answer key.
