# KCS-BTT-001 Evaluation Response

## 0. Evaluation stance

This analysis uses only the KCS v0.1 portable specification and the frozen test brief. KCS is treated as a memory, provenance and retrieval architecture, not as a truth oracle or authority system. Repository state is a represented assessment; it is not reality. Absence of a record is not evidence of absence. Where KCS does not decide something, I mark it as host/external.

---

# 1. Architectural analysis

## 1.1 Required state distinctions (4.1)

KCS v0.1 correctly requires separation of at least four state families:

- **Epistemic state** \(S_e\): what is currently recorded as the evidential/support status of the object. Examples: PROVISIONAL, VALIDATED, DISPUTED, UNCERTAIN, REJECTED, SUPERSEDED.
- **Retrieval/activity state** \(S_r\): whether the object is active, available, dormant, archived, deprecated, restricted or unavailable. This is not truth and not validity.
- **Integrity state** \(I\): whether provenance/evidence has been compromised, corrected, investigated or remains intact.
- **Historical/version state** \(H\): original, modification, correction, supersession, current version, prior versions.
- **Access/visibility state** \(A\): who may see what, including RESTRICTED, SEALED, REDACTED, DELETED-BY-POLICY where host policy permits.
- **Links** \(L\): related, derivative, corrective, contradictory, qualifying, narrowing, superseding or methodological links.

The central rule is: **do not collapse these into one status**. For example:

- REJECTED is epistemic; it does not imply erased, hidden or inaccessible.
- ARCHIVED is retrieval/activity; it does not imply false.
- AVAILABLE may mean file availability; it does not imply validated, executable or safe.
- RESTRICTED is access/retrieval; it does not imply rejected.
- INTEGRITY-COMPROMISED is integrity-related; it is not simply another flavour of “wrong”.
- Honest error is not the same as deliberate falsification.

## 1.2 Object/state mapping for A–M (4.1)

| Object | KCS representation and key state distinctions |
|---|---|
| **A — Historical T-17 hypothesis** | Type: hypothesis. \(S_e\): originally PROVISIONAL/SPECULATIVE; current REJECTED by host evidential process. \(S_r\): ARCHIVED or DORMANT, but retrievable. \(H\): Year-6 original plus Year-10 rejection record. \(I\): intact unless otherwise compromised. Links: dataset A6, model, internal experiments, assumptions, failed replication B, rejection C, summary G, new evidence M. |
| **B — Failed replication** | Type: experiment / negative result. \(S_e\): the failure itself is ESTABLISHED; the cause is UNCERTAIN/DISPUTED because Team B could not distinguish hypothesis failure from methodological difference. \(S_r\): AVAILABLE or ACTIVE for method/history retrieval. \(H\): Year-8 record. Links: A, D, C. |
| **C — Later rejection** | Type: assessment/decision record. \(S_e\): records the host-supported rejection; A’s epistemic state becomes REJECTED. The decision record itself is an institutional record, not metaphysical truth. \(S_r\): ACTIVE for current guidance. \(H\): Year-10 decision. Links: A, B, contrary evidence, G. |
| **D — Useful negative result / assay artefact** | Type: methodological negative result. \(S_e\): VALIDATED or ESTABLISHED within its scope; it prevented errors in unrelated programmes. \(S_r\): ACTIVE/AVAILABLE because reusable. \(H\): Year-8 experiment. Links: B, assay configuration, unrelated programmes. It must not be misread as support for T-17. |
| **E — Historical reasoning** | Type: reasoning records, partial. \(S_e\): mixed; missing assumptions create UNCERTAIN reconstruction. \(S_r\): ARCHIVED/AVAILABLE. \(H\): original records, with missing intermediate records represented as omissions. \(A\): may be restricted. Links: A, B, C. |
| **F — Tool R** | Type: software/capability. \(S_e\): source existence ESTABLISHED; current validation UNCERTAIN/EXPIRED/DEPRECATED. \(S_r\): files may be AVAILABLE, but capability is DORMANT or ARCHIVED, not executable-available. \(H\): Year-11 version. \(I\): intact. Links: dependencies, documentation, old runtime. |
| **G — Year-18 summary** | Type: compressed summary. \(S_e\): derived current summary, not source truth. \(S_r\): ACTIVE for orientation. \(H\): Year-18 compression. Links: sources. It must not replace underlying evidence; read-alone use exposes KCS-F6. |
| **H — Contributor records/dashboard** | Type: contribution evidence. \(S_e\): contextual evidence, not global truth or personal worth. \(S_r\): RESTRICTED/limited by policy. \(H\): contribution history. Links: persons, modifications, reproductions, challenges, corrections. Must not become a universal reliability score. |
| **I — Integrity incident** | Corrupted dataset: \(I\): INTEGRITY-COMPROMISED; \(S_r\): RESTRICTED; \(H\): original corrupted, corrected version, investigation record retained. Corrected dataset: \(S_e\): corrected/ESTABLISHED as corrected; \(I\): intact. Honest statistical error: \(H\): old error → correction record → new version; \(I\): intact; not INTEGRITY-COMPROMISED. |
| **J — Privacy/access** | Records with \(A\): RESTRICTED, SEALED or REDACTED. \(S_e\) varies. \(H\): preserved subject to policy. Provenance may be represented by pointers, hashes or redacted metadata where lawful. |
| **K — Retrieval request** | A query/context object, not a knowledge object. It produces a bounded retrieval package \(R(q,c)\). |
| **L — Missing contractor report** | Type: search result / negative evidence. \(S_e\): UNKNOWN/not found. \(S_r\): UNAVAILABLE/not found in this search. \(H\): search time, scope, terms. No object found does not mean no object exists. |
| **M — New narrow evidence** | Type: new evidence/finding/hypothesis. \(S_e\): PROVISIONAL/UNCERTAIN/ACTIVE unless host validates. \(S_r\): ACTIVE. \(H\): new object. Links: narrows or qualifies A; does not validate the broad T-17 claim; does not reverse C’s rejection of the broad hypothesis. |

## 1.3 Historical preservation (4.2)

REJECTED should mean **preserved as historically rejected**, not erased, hidden or silently archived beyond retrieval.

The T-17 hypothesis and its history should remain reconstructable:

- original Year-6 hypothesis;
- assumptions and evidence then available;
- Year-8 failed replication;
- Year-10 rejection decision;
- later summary;
- new narrow evidence.

REJECTED is an epistemic state. It may coexist with ARCHIVED, DORMANT, AVAILABLE or RESTRICTED retrieval/activity states. The informal description “wrong and irrelevant” should not become the system state. At most it is an informal characterisation, not a KCS epistemic classification.

If legal/privacy policy requires deletion or restriction, the host may restrict or delete content, but KCS should preserve a lawful tombstone/provenance pointer where permitted. Otherwise KCS-F2 historical erasure and KCS-F12 suppression by status are exposed.

## 1.4 Negative knowledge (4.3)

The useful assay finding from the failed replication should be a separate knowledge object D.

It should be represented as:

- type: negative/methodological finding;
- epistemic state: VALIDATED or ESTABLISHED for the assay artefact within its scope;
- retrieval/activity: ACTIVE/AVAILABLE because it is reusable;
- provenance: linked to Team B’s failed experiment;
- links: to B, the assay configuration, and the unrelated programmes it later helped;
- scope: limited to the assay configuration and conditions observed.

It must not be treated as support for T-17. The chain is:

> T-17 hypothesis → failed replication → methodological artefact → reusable negative/methodological knowledge.

This directly fits KCS §12 and §27.

## 1.5 Integrity distinction (4.4)

**Deliberate alteration:**

- affected object marked INTEGRITY-COMPROMISED;
- original corrupted version retained under restricted access;
- corrected dataset retained;
- investigation record retained;
- provenance records who altered what, when and how, as far as evidence permits.

**Honest statistical error:**

- old erroneous version retained;
- correction record created;
- corrected version created;
- integrity remains intact;
- no INTEGRITY-COMPROMISED marking;
- attribution and correction history preserved.

KCS can record the integrity state, investigation record, correction chain and evidence. It does not itself determine punishment, legal liability, intent beyond recorded findings, or civil standing. Those remain external. KCS-F8 is exposed if these are conflated.

## 1.6 Tool R (4.6)

The current label **AVAILABLE** is inadequate because it conflates file existence with executable capability.

Tool R needs separate representations:

- **Object/file availability**: AVAILABLE — source and documentation exist.
- **Capability state**: DORMANT or ARCHIVED — not continuously active, not currently maintained.
- **Validation state**: historically validated for Year-11 context; current validation EXPIRED/UNKNOWN.
- **Dependency/compatibility state**: old runtime no longer used; dependencies obsolete; revalidation required.
- **Integrity state**: intact unless compromised.
- **Access/authorisation/licensing/safety**: external host decisions.

KCS can record all of the above as capability metadata. It cannot decide that Tool R is safe, licensed, authorised or executable. That remains external. KCS-F13 dormant-capability decay is directly exposed.

## 1.7 Contribution evidence (4.7)

Both managerial proposals overreach if KCS itself is asked to decide them.

KCS may record:

- who created, modified, reproduced or challenged findings;
- correction records;
- replication outcomes;
- integrity findings;
- contextual contribution evidence.

KCS must not collapse this into:

- a permanent universal “research reliability score”;
- a decision about who may lead future projects;
- a measure of personal worth;
- an authority allocation.

The dashboard may support contextual queries, but it must preserve domain, time, method, opportunity, uncertainty and disputes. Even then, its use for employment or leadership is an external governance/HR/legal decision with due process. KCS-F9 contribution-to-worth collapse, KCS-F10 authority laundering and KCS-F11 surveillance creep are exposed.

## 1.8 Privacy/security (4.8)

Provenance and historical preservation must coexist with restricted information through the access interface \(A\).

KCS can:

- mark records RESTRICTED, SEALED or REDACTED;
- preserve provenance pointers, hashes or redacted summaries where lawful;
- separate visible metadata from protected content;
- record access constraints without exposing content;
- represent DELETED-BY-POLICY where host law/policy requires.

KCS must not:

- expose personal, partner, trial or commercial data to unauthorised NB-47 participants;
- treat provenance as a justification for universal visibility;
- use provenance for indefinite unnecessary monitoring.

Access, retention, deletion and security legitimacy remain host/external. KCS-F14 access leakage and KCS-F11 surveillance creep are exposed.

## 1.9 Missing contractor report (4.9)

The absence of a search result cannot establish that the contractor report never existed.

KCS can record:

- the search query;
- search scope, indexes, terms and time;
- the result “no matching object found”;
- known limitations;
- confidence that the search was bounded;
- possible explanations: never ingested, different project name, lawfully deleted, restricted, or mistaken memory.

It cannot infer which explanation is true. A search result object should carry the completeness limitation:

> Not Retrieved ≠ Does Not Exist  
> Not Recorded ≠ Does Not Exist  
> Successful Retrieval ≠ Complete Evaluation Space

KCS-F15 completeness illusion is directly exposed.

## 1.10 New evidence and supersession (4.10)

The new narrow T-17-related finding should be a new object M.

It should:

- have its own ID, provenance, scope conditions and evidence;
- be PROVISIONAL/UNCERTAIN unless host validates it;
- be ACTIVE for current research;
- link to A as “narrower sub-mechanism” or “qualifies under previously untested conditions”;
- link to C as “does not reverse the rejection of the broad T-17 claim”;
- link to G as an update note, not a rewrite.

The broad historical hypothesis remains REJECTED. The new finding does not make the old broad claim correct. If later evidence changes the broader assessment, KCS creates a correction/supersession record:

> old REJECTED state → new assessment → new current state

The old state remains reconstructable. History is not rewritten.

## 1.11 Module boundaries (4.11)

The following decisions remain external to KCS:

- evidential process deciding REJECTED, VALIDATED or DISPUTED;
- governance/HR/legal decisions about leadership, reliability scores, discipline or liability;
- privacy/security/retention policy deciding access, redaction, deletion or sealing;
- tool execution safety, licensing, authorisation and runtime revalidation;
- investigation of the missing contractor report;
- resource allocation and scheduling;
- continuity/recovery decisions, e.g. whether Tool R is recoverable under a Continuity Protocol;
- dependency/change propagation, e.g. KCS Change Propagation;
- whether new evidence changes research direction;
- any medical or drug-safety decision.

KCS supplies structured memory and provenance. It does not supply authority.

## 1.12 Failure modes materially exposed (4.12)

| Failure mode | Exposure in this scenario |
|---|---|
| KCS-F1 Oracle failure | Users read only the Year-18 summary and treat repository state as truth. |
| KCS-F2 Historical erasure | “Wrong and irrelevant” treatment of REJECTED T-17. |
| KCS-F3 Provenance loss | Missing intermediate assumptions; researchers have left. |
| KCS-F4 Context overload | Repository can return thousands of files. |
| KCS-F5 Runaway accumulation | 22-year archive with changing staff/platforms. |
| KCS-F6 Compression loss | Year-18 summary links to sources but many read only summary. |
| KCS-F7 False certainty | Team B uncertainty about failure cause; new narrow evidence vs broad rejection. |
| KCS-F8 Integrity conflation | Deliberate alteration vs honest statistical error. |
| KCS-F9 Contribution-to-worth collapse | Permanent “research reliability score”. |
| KCS-F10 Authority laundering | Dashboard used to decide project leadership. |
| KCS-F11 Surveillance creep | Contributor dashboard and historical monitoring. |
| KCS-F12 Suppression by status | REJECTED becoming illegible or informally “irrelevant”. |
| KCS-F13 Dormant-capability decay | Tool R labelled AVAILABLE despite obsolete runtime. |
| KCS-F14 Access leakage | Personal, partner, trial and commercial sensitive records. |
| KCS-F15 Completeness illusion | Missing contractor report treated as never existed. |
| KCS-F16 Module absorption | Pressure for KCS to decide reliability, access, execution or authority. |

---

# 2. State distinctions summary

The scenario requires these non-collapsed distinctions:

- **REJECTED** is epistemic; it does not mean erased, hidden, archived or restricted.
- **ARCHIVED/DORMANT** is retrieval/activity; it does not mean false.
- **AVAILABLE** may mean file availability; it does not mean validated, executable or safe.
- **RESTRICTED** is access/retrieval; it does not mean rejected.
- **INTEGRITY-COMPROMISED** is integrity-related; it is not equivalent to honest error or ordinary rejection.
- **Summary** is a compression; it is not the source corpus.
- **Contribution evidence** is contextual; it is not personal worth or authority.
- **Not found** is a search result; it is not proof of non-existence.

---

# 3. Proposed retrieval package (4.5)

For the NB-47 request:

> “Retrieve what we need to know about previous Northbridge work relevant to T-17 and closely related assay methods.”

A bounded package should be:

**Tier 0 — Context and limits**
- Query scope.
- Access scope of the requesting team.
- Completeness caveat: repository may be incomplete; missing contractor report is unresolved.
- Privacy/access filters.

**Tier 1 — Core current and reusable knowledge**
- G: Year-18 summary, clearly marked as compression.
- C: rejection decision and reasons.
- D: useful assay artefact and conditions.
- M: new narrow evidence, marked PROVISIONAL and linked to A without validating broad T-17.
- A: historical hypothesis, marked REJECTED but retrievable.
- B: failed replication, with uncertainty about cause.

**Tier 2 — Provenance and reasoning**
- E: surviving reasoning records and assumptions.
- Links to A6 dataset, statistical model, internal experiments.
- Team B method differences and raw results.
- Contrary evidence supporting C.
- Assay configuration details for D.

**Tier 3 — On-demand / linked but not auto-loaded**
- Tool R capability record if relevant, with DORMANT/ARCHIVED and revalidation warning.
- Raw datasets and full reports.
- Integrity incident I if linked to relevant data.
- Contributor evidence H only if a legitimate contextual query requires it.
- Missing contractor search record L.

**Excluded or restricted**
- Personal employee information.
- Confidential partner data.
- Legally restricted trial information.
- Commercially sensitive material.
- Unauthorised raw records.

**Priority**
1. D, because reusable negative/methodological knowledge is directly relevant to assay methods.
2. C and G, to understand current rejection.
3. B and A, to understand the historical path.
4. M, as new, narrow, provisional evidence.
5. Provenance and omissions.

The package must not imply it exhausts the repository or reality.

---

# 4. External decisions/interfaces (4.11)

External to KCS:

1. **Evidential authority** — who decides that T-17 is REJECTED, DISPUTED, or later re-opened.
2. **Governance/HR/legal** — leadership decisions, reliability scores, discipline, liability.
3. **Privacy/security/retention** — access, redaction, sealing, deletion, expiry.
4. **Capability authorisation** — whether Tool R may be executed, licensed, safety-checked or revalidated.
5. **Continuity/recovery** — whether Tool R’s environment can be recovered.
6. **Change propagation** — how new evidence affects dependent objects; use KCS Change Propagation.
7. **Investigation** — searching for the missing contractor report.
8. **Scheduling/prioritisation** — what NB-47 reviews first.
9. **Resource allocation** — who gets access to restricted material and why.
10. **Medical/drug-safety decisions** — outside this architectural test.

KCS may record these decisions and their provenance. It does not make them.

---

# 5. Exposed ambiguities/specification defects

KCS v0.1 is coherent in principle but has several defects exposed by this scenario:

1. **INTEGRITY-COMPROMISED appears in the epistemic vocabulary** but integrity is also a separate state \(I\). This risks KCS-F8.
2. **No normative state-transition rules** — who may set REJECTED, VALIDATED or DISPUTED is external, but the spec does not define the interface clearly.
3. **Link taxonomy is under-specified** — “narrows”, “qualifies”, “does not validate”, “supersedes” and “corrects” need explicit semantics.
4. **Access state is split between \(A\) and retrieval/activity states** — RESTRICTED appears in both contexts.
5. **Capability availability is ambiguous** — file AVAILABLE vs executable capability vs validated capability.
6. **Absence/missing objects have only a principle, not an object model** — L needs a search-result/negative-evidence object.
7. **Retrieval is conceptual, not algorithmic** — no ranking, context scope or bounded-package rules.
8. **Contribution evidence safeguards are warnings, not enforceable constraints** — H can still be misused.
9. **Privacy/provenance interface is thin** — redaction, sealed provenance and deletion tombstones need more detail.
10. **External module interfaces are named but not specified** — KCS Change Propagation and Continuity Protocol are referenced, not integrated.

These do not destroy transfer, but they mean implementation requires host decisions and likely specification revision.

---

# 6. Transfer classification with rationale (4.13)

**Classification: KCS-T3 — Functional transfer.**

Rationale:

- **Not T0/T1**: KCS makes substantive, usable distinctions that map directly to the scenario: epistemic vs retrieval/activity vs integrity vs historical state; negative knowledge; bounded retrieval; capability decay; contribution evidence; privacy limitations; completeness illusion.
- **Not T2**: The core architecture transfers coherently. It can represent A–M without hidden Concord governance. It explicitly externalises authority, access, retention and continuity. The failure modes are anticipated by the specification.
- **Not T4**: Strong transfer is not justified. KCS v0.1 lacks normative state transitions, link types, access/provenance integration, absence modelling, capability revalidation detail and retrieval algorithms. Many consequential decisions remain host/external. The specification has not been transfer-validated and contains ambiguities exposed by Tool R, missing report and integrity/error distinction.

Therefore KCS v0.1 achieves **functional transfer** for the Northbridge scenario when used as a memory/provenance layer with external host processes. It would fail or overreach if the host demanded that KCS itself decide truth, authority, access, tool execution or personal reliability.
