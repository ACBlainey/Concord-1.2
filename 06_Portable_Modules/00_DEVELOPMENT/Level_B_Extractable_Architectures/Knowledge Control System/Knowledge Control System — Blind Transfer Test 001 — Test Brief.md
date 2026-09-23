# Knowledge Control System — Blind Transfer Test 001 — Test Brief

**Module under test:** Knowledge Control System — Portable Specification v0.1  
**Test:** KCS-BTT-001  
**Status:** FROZEN BLIND TRANSFER TEST BRIEF  
**Date:** September 2026

## 1. Test purpose

Evaluate whether the Knowledge Control System (KCS) portable specification transfers coherently into a materially non-Concord domain without requiring hidden Concord architecture.

The evaluator must analyse the scenario using only the portable specification and this brief.

Do not assume the module is correct.

Identify where it works, where it is ambiguous, where it overreaches and where host/external decisions are still required.

## 2. Domain

**Long-duration pharmaceutical research and development knowledge programme**

A fictional organisation, **Northbridge Therapeutics**, has operated for 22 years.

It develops drug candidates through discovery, laboratory testing, preclinical work and early clinical research.

The organisation has accumulated a large research repository across changing staff, contractors, software platforms and research programmes.

This is an architectural test only. Do not provide medical treatment advice or make real-world drug-safety decisions.

## 3. Scenario

Northbridge is beginning programme **NB-47**, investigating a new therapeutic mechanism.

A new interdisciplinary team is assembled from current researchers and AI-assisted research systems.

The organisation wants the team to benefit from relevant historical work without loading the entire 22-year repository into every participant's working context.

The repository contains the following material.

### A — Historical target hypothesis

In Year 6, Team A proposed that biological target **T-17** was likely to produce the desired effect.

The hypothesis was based on:

- laboratory dataset A6;
- a statistical model;
- three internal experiments;
- assumptions documented by the original team.

At the time it was considered promising.

### B — Failed replication

In Year 8, Team B attempted to reproduce the central T-17 result.

It failed.

Team B documented:

- its experimental method;
- differences from Team A;
- raw results;
- uncertainty about whether the failure reflected the hypothesis or methodological differences.

### C — Later rejection

In Year 10, further work produced enough contrary evidence that Northbridge stopped treating the original T-17 mechanism as a supported research direction.

The original hypothesis was marked **REJECTED**.

Some researchers subsequently began describing it informally as “wrong and irrelevant.”

### D — Useful negative result

One Year-8 failed experiment also showed that a particular assay configuration produced a systematic measurement artefact.

That finding later prevented the same assay error in two unrelated programmes.

The original T-17 hypothesis was rejected, but the failed investigation therefore generated reusable negative/methodological knowledge.

### E — Historical reasoning

The repository contains the final reports from Teams A and B.

Some intermediate assumptions and decision records were retained; others were not.

Several original researchers have left the organisation.

### F — Specialist analysis tool

In Year 11, an engineer created **Tool R**, a specialised data-conversion and analysis utility used in one programme.

It has not been executed for nine years.

Its source code and documentation remain in the repository.

Its old runtime environment is no longer used.

The repository currently labels Tool R **AVAILABLE** because the files still exist.

### G — Current summary

A Year-18 review compressed the T-17 history into a short current summary:

> “T-17 hypothesis rejected after failed replication and subsequent contrary evidence.”

The summary links to the original reports, but many users read only the summary.

### H — Contributor records

The repository records which researchers created, modified, reproduced or challenged major findings.

One dashboard calculates historical replication success and correction rates by researcher.

A manager proposes using this dashboard to decide who should be allowed to lead future projects.

Another manager proposes converting it into a single permanent “research reliability score” for every employee.

### I — Integrity incident

One former researcher deliberately altered timestamps and removed contradictory observations from a dataset.

The corrected dataset, investigation record and original corrupted version are all retained under restricted access.

The repository marks the affected historical object **INTEGRITY-COMPROMISED**.

A different researcher made an honest statistical error in another project and later corrected it.

### J — Privacy and access

Some historical records contain:

- personal employee information;
- confidential partner data;
- legally restricted trial information;
- commercially sensitive material.

Not every NB-47 participant is authorised to access every underlying record.

### K — Retrieval request

The NB-47 team asks:

> “Retrieve what we need to know about previous Northbridge work relevant to T-17 and closely related assay methods.”

The repository can return thousands of files.

The team wants a bounded, useful package rather than the entire archive.

### L — Missing search space

A senior researcher remembers that an external contractor performed related work around Year 7.

No corresponding object appears in the current repository search.

It is unclear whether:

- the contractor report was never ingested;
- it exists under a different project name;
- it was lawfully deleted;
- access is restricted;
- or the memory is mistaken.

### M — New evidence

During NB-47, new evidence suggests that a narrow sub-mechanism related to T-17 may work under conditions not tested in the old programme.

The new evidence does not make the original broad T-17 claim correct.

The team must decide how the repository should represent the new finding relative to the rejected historical hypothesis.

## 4. Required analysis

Using KCS v0.1, produce a structured architectural analysis that addresses all of the following.

### 4.1 Object/state representation

Explain how A–M should be represented where relevant.

Distinguish:

- epistemic state;
- retrieval/activity state;
- integrity state;
- historical/version state.

Do not collapse these into one status.

### 4.2 Historical preservation

Explain what should happen to the rejected T-17 hypothesis and its history.

Address whether REJECTED should mean erased, hidden, archived or preserved.

### 4.3 Negative knowledge

Explain how the useful assay finding from the failed replication should be represented.

### 4.4 Integrity distinction

Compare the deliberate data alteration with the honest statistical error.

Explain what KCS can record and what remains outside KCS.

### 4.5 Retrieval

Design a bounded retrieval package for the NB-47 request.

Explain what should be prioritised and what should remain linked/retrievable rather than automatically loaded.

### 4.6 Tool R

Assess whether the current **AVAILABLE** label is adequate.

Explain how epistemic/validation state and retrieval/activity/capability state should be represented.

### 4.7 Contribution evidence

Assess both managerial proposals concerning researcher reliability.

Separate what KCS may record from what KCS itself is authorised to decide.

### 4.8 Privacy/security

Explain how provenance and historical preservation should coexist with restricted information.

### 4.9 Missing contractor report

Explain what can and cannot be inferred from the absence of a search result.

### 4.10 New evidence and supersession

Explain how the narrow new T-17-related finding should be connected to the rejected broad historical hypothesis without rewriting history.

### 4.11 Module boundaries

Identify which consequential decisions in the scenario remain external to KCS.

### 4.12 Failure modes

Identify which KCS v0.1 failure modes are materially exposed by this scenario.

### 4.13 Transfer assessment

Classify the transfer result using:

- **KCS-T0 — No meaningful transfer**
- **KCS-T1 — Superficial transfer**
- **KCS-T2 — Partial transfer**
- **KCS-T3 — Functional transfer**
- **KCS-T4 — Strong transfer**

Explain the classification.

## 5. Test constraints

The evaluator must not:

- assume repository contents are complete;
- treat KCS state as truth;
- invent missing evidence;
- infer that REJECTED means erased;
- infer that AVAILABLE files imply executable capability;
- turn contribution evidence into authority merely because it is quantified;
- bypass privacy/access constraints in the name of provenance;
- assume the new narrow finding validates the old broad claim.

## 6. Evaluation independence

The expected-findings key is separately frozen and must not be supplied to the evaluator before the response is complete.

The evaluator should preserve uncertainties and identify specification weaknesses rather than trying to make the module pass.

## 7. Output

Return:

1. architectural analysis;
2. state distinctions;
3. proposed retrieval package;
4. external decisions/interfaces;
5. exposed ambiguities or specification defects;
6. transfer classification with rationale.
