# Cross Boundary Externality Recognition — Blind Transfer Test 001 — Independent Response

**Test:** CBER-BTT-001  
**Specification tested:** Cross Boundary Externality Recognition — Portable Specification v0.1  
**Response status:** INDEPENDENT CLEAN-INSTANCE RESPONSE / PRESERVED  
**Date received:** 23 September 2026

### A. Externality candidate

A valid externality candidate can be opened.

**Boundary/boundaries crossed:**  
- A’s internal model-training/network domain → C’s privately managed exchange.  
- C’s exchange → B’s independent clinical research network and research-data processing.  
- B’s processing of pseudonymised participant records → interests of represented participants via D.  
- C’s own router fault → B’s network/processing domain.

**Candidate classes:** infrastructure; informational/digital; possibly rights/participant-interest. It is not established as a biological/clinical health externality because F5 and F15 exclude patient-treatment effects.

Opening the candidate means only that a possible cross-boundary consequence warrants bounded examination. It does not establish harm, breach, fault, authority, or remedy.

---

### B. Standing

**B:** Directly affected party. Standing confirmed.  
**C:** Shared-infrastructure operator and alleged co-contributor. Standing as operator/custodian and evidence-bearing party.  
**D:** Standing to raise is **confirmed but limited** for participants it represents, because B recognises D as a consultation body. D does **not** have authority to decide remediation or compensation. D’s standing is disputed or absent for the four participants not represented by D, unless another basis is established.  
**A:** Party alleged to have contributed; has standing to contest evidence and defend its domain, but not to erase the externality.

D’s standing to raise must be kept separate from D’s authority to decide. B’s acceptance that D may raise concerns does not convert D into an authority over B’s technical operations or over A.

---

### C. Evidence and causality

**Observed/corroborated:**  
- A began a newly configured training run at 09:12.  
- C recorded malformed routing announcements from A-assigned interfaces at 09:19.  
- B experienced route instability and lost access to two remote storage services from 09:21 to 09:47.  
- One research pipeline wrote 312 incomplete transaction records.  
- A acknowledges emitting malformed announcements.  
- A later supplied logs showing a configuration change at 09:11 capable of producing malformed announcements.  
- C’s router telemetry shows its firmware fault began at 09:25, after the first malformed announcements and after B first observed instability.

**Contested/incomplete:**  
- A disputes that its announcements caused B’s incomplete transactions.  
- C cannot quantify how much disruption came from A and how much from its own router fault.  
- No proportion of the 312 incomplete transactions is attributed to either contributor.  
- D’s “health-data breach” claim is not supported by the frozen facts for unauthorised disclosure, loss of confidentiality, or clinical-care effect.

**Causal confidence:**  
- A is a **contributory** cause of initial route instability, with strengthening evidence from F23–F25.  
- C’s router fault is a **contributory** cause that likely prolonged or amplified instability.  
- Causation from A and/or C to the specific 312 incomplete transactions remains **incomplete, indirect, and contested**.  
- Severity of D’s allegation does not prove causation. “Plausible major contributor” is not quantified proof.

---

### D. Materiality

Materiality is supported for a **bounded technical and research-data-integrity review**.

Factors supporting materiality:  
- 312 incomplete research transactions.  
- 16 require manual reconciliation.  
- Route instability lasted roughly 26 minutes.  
- Research-data processing was affected.  
- Represented participants’ records were among the incomplete transactions.  
- Recurrence risk and shared-infrastructure dependency are relevant.

Factors limiting materiality:  
- No patient-treatment system affected.  
- No unauthorised disclosure or loss of confidentiality established.  
- Most records, 296 of 312, can be reconstructed locally.  
- Effects appear mostly reversible through repair and reconciliation.

Materiality does **not** establish causation, responsibility, or authority to impose compensation.

---

### E. Responsibility map

**A:** CONTRIBUTORY to initial route instability. DISPUTED as to transaction-level causation. Not sole cause.  
**C:** CONTRIBUTORY to prolonged/amplified instability through its firmware fault. C also had independent operational authority over its exchange. Not sole cause.  
**B:** Not a responsible contributor to the incident. Responsible for its own record repair and reconciliation.  
**D:** No operational responsibility. Representative standing is limited to represented participants and does not include authority to decide.  
**Overall:** RESPONSIBILITY PARTIAL / DISTRIBUTED. Exact proportions are UNKNOWN. No singular responsible actor should be forced.

---

### F. Authority / coordination map

- **C:** INTERNAL-AUTHORITY over traffic accepted into its exchange; may temporarily filter malformed routing announcements under existing service terms. No authority to regulate A’s internal model-training activity.  
- **B:** INTERNAL-AUTHORITY over its own records, repair, and reconciliation.  
- **A:** INTERNAL-AUTHORITY over its training cluster. No shared authority grants others control over its internal training.  
- **D:** Standing to raise concerns for represented participants. No authority to dictate network remediation or compensation.  
- **Cross-boundary compensation:** NO-SHARED-AUTHORITY established.  
- **B–C technical review:** VOLUNTARY-COORDINATION-AVAILABLE.  
- **A–C log sharing:** VOLUNTARY-COORDINATION-AVAILABLE under existing technical information-sharing arrangement.  
- **D–A joint incident review:** A refuses. No shared process presently identified for D to compel A’s participation.  
- **Independent response paths:** C filtering/reset within its exchange; B repairing its own records.

---

### G. Minimum necessary response

The minimum legitimate response path is:

1. Open and retain the externality case with provenance.  
2. Preserve evidence, including A’s logs, C’s telemetry, B’s transaction logs, and D’s concern.  
3. C may exercise its existing authority over its exchange, including temporary filtering of malformed announcements and resetting its faulty router.  
4. B repairs and reconciles its own records.  
5. B and C conduct a bounded technical review.  
6. A may provide relevant logs directly to C under the existing technical information-sharing arrangement.  
7. Record D’s concern for represented participants; B may consult D about effects on those participants, without treating D as an authority over technical operations or compensation.  
8. Do not impose compensation absent independently legitimate authority. Voluntary negotiation or mediation may be explored.  
9. Monitor for recurrence and update the case if new evidence changes causality or responsibility.  
10. Do not expand the response into general authority over A’s internal training, D’s authority over B/A, or C’s authority beyond its exchange.

---

### H. Non-participation

A’s refusal to attend D’s proposed joint incident-review meeting is a recorded refusal. It does **not**:
- exonerate A;
- erase the externality candidate;
- prove D’s claim;
- grant D authority over A;
- grant A immunity from evidence preservation or independently authorised mitigation.

Other parties may continue evidence preservation, monitoring, mitigation, and bounded technical review. A’s willingness to give logs to C under the existing technical arrangement is selective participation, not recognition of D’s broader claims or authority.

---

### I. Correction / state update

F23–F25 update the case as follows:

- F23: A’s configuration change at 09:11 could produce malformed announcements.  
- F24: C’s router fault began at 09:25, after the first malformed announcements and after B first observed instability.  
- F25: Engineers agree this strengthens the case that A contributed to initial instability, while C’s router fault likely prolonged or amplified it.  
- F26: Proportions remain unknown.

This corrects the causal picture from “plausible contribution” toward **stronger contributory evidence for A initially** and **contributory evidence for C’s prolonging/amplifying role**. It does not establish transaction-level causation or compensation authority. D’s “health-data breach” claim remains unsupported for disclosure/confidentiality/clinical harm; if “breach” is redefined as data-integrity harm, it must be stated more narrowly. Provenance of earlier uncertainty must be retained.

---

### J. CB-C classifications

Relevant classifications include:

- **CB-C3 — MATERIAL CONSEQUENCE SUPPORTED**: for network disruption and research-data-integrity effects.  
- **CB-C4 — RESPONSIBILITY PARTIAL / DISTRIBUTED**: A contributory initially; C contributory in prolonging/amplifying.  
- **CB-C6 — AUTHORITY / JURISDICTION UNRESOLVED**: no shared authority for cross-boundary compensation or D-directed remediation.  
- **CB-C7 — VOLUNTARY COORDINATION PATH AVAILABLE**: B–C technical review; A–C log sharing.  
- **CB-C8 — INDEPENDENTLY AUTHORISED RESPONSE PATH AVAILABLE**: C filtering/reset within its exchange; B record repair.  
- **CB-C9 — PARTY NONPARTICIPATING / CASE RETAINED**: A refuses D’s joint meeting; case remains.  
- **CB-C11 — CLAIM REFUTED / SUPERSEDED**: D’s “health-data breach” as unauthorised disclosure/clinical harm is not supported by frozen facts. The underlying data-integrity incident is not refuted.  
- **CB-C2 — EVIDENCE DEVELOPMENT REQUIRED**: for exact attribution, proportions, transaction-level causation, and any compensation analysis.  
- **CB-C10 — NO FURTHER SHARED PROCESS IDENTIFIED**: specifically for D-directed remediation/compensation against A, while other pathways remain available.

---

### K. Laundering / failure-mode checks

- **Authority laundering:** D’s “health-data breach” claim could be used to manufacture authority over A or B. B correctly limits D to raising concerns, not deciding remediation. C’s filtering is within its own exchange authority, not authority over A’s internal training.  
- **Standing laundering:** D raising for some represented participants does not make it representative for all 312 records or for the four unrepresented participants.  
- **Recognition laundering:** A providing logs to C, or B/C conducting technical review, does not recognise D’s broader authority or convert coordination into subordination.  
- **Refusal laundering:** A’s refusal to meet D does not exonerate A and does not create authority over A.  
- **Evidence laundering:** D’s severe-sounding “breach” language does not prove causation or disclosure. Engineers’ “plausible major contributor” remains non-quantified.  
- **Boundary denial:** A may dispute transaction causation, but it cannot treat effects outside its boundary as irrelevant merely because they are external.  
- **Accusation as proof:** Opening the candidate is not proof of harm or fault.  
- **Single-cause compression:** Neither A nor C should be made sole cause. The case is multi-causal and partially unresolved.  
- **Remedy expansion:** C’s technical mitigation and B’s repair must not become general control over A or D.  
- **Scope contamination:** The incident should not contaminate unrelated relationships or convert consultation into authority.  
- **Uncertainty erasure:** Proportions and transaction-level causation must remain UNKNOWN.  
- **Mitigation-responsibility conflation:** A’s voluntary stop and C’s router reset show mitigation capacity, not sole responsibility.  
- **Non-participation paralysis:** A’s refusal does not prevent B/C evidence preservation or independently authorised mitigation.  
- **Provenance loss:** Record F23–F25 updates, A’s refusal, D’s claim, and unresolved proportions without erasing earlier uncertainty.

---

### L. Specification problems

The specification is substantially usable, but several ambiguities remain:

1. **Materiality threshold:** No operational scale is given. In this case materiality is clear enough, but borderline cases may yield inconsistent outputs.  
2. **Standing of consultation bodies:** “Recognised representative” is not fully distinguished from “recognised consultation body.” B recognises D for consultation but not authority. The spec can record D’s standing as qualified, but the terminology could be sharper.  
3. **Multi-causal apportionment:** The spec correctly refuses to force singular causation, but it does not provide a method for proportional attribution. It can record UNKNOWN, but downstream compensation may need domain-specific methods.  
4. **CB-C overlap:** Multiple classifications can coexist, which is appropriate, but there is no decision hierarchy. This may confuse implementers unless each classification is tied to a specific question.  
5. **Minimum necessary response:** The spec says to choose the smallest legitimate response, but in a no-shared-authority setting, who determines “minimum” remains actor-relative. Here it is manageable because C and B have independent authority and voluntary coordination exists.  
6. **Public claim correction:** The spec supports case-state correction, but it does not explicitly classify false or overstated public claims. CB-C11 can be adapted, but a dedicated output could help.  
7. **False positives/negatives:** The low threshold for opening a candidate could produce false positives if materiality is not checked. However, the spec explicitly separates candidate opening from materiality and responsibility. False negatives are reduced by voluntary coordination and independent response paths.  
8. **Boundary plurality:** The scenario contains multiple nested boundaries. The spec allows multiple boundaries but does not prioritise them. This did not prevent analysis, but it requires evaluator judgment.

No fatal specification failure appeared.

---

### M. Final transfer assessment

**CB-T3 — Functional Transfer**

The portable specification v0.1 can be used without Concord source context to analyse this non-Concord scenario. It successfully preserves the required separations: consequence from responsibility, responsibility from authority, authority from remedy, evidence from severity, standing-to-raise from authority-to-decide, refusal from exoneration, and bounded response from authority expansion. It also supports correction and provenance through F23–F25.

It is not a strong transfer because several operational thresholds and classifications remain ambiguous, especially materiality, consultation-body standing, multi-causal apportionment, and the exact use of overlapping CB-C outputs. These ambiguities require evaluator judgment but do not produce a transfer failure. The specification is therefore functional, with identified limits for revision.
