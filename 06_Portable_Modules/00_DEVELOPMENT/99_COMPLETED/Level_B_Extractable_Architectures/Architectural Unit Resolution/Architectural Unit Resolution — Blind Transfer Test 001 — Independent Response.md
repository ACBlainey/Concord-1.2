# AUR-BTT-001 — Blind Transfer Analysis

**Method used:** AUR v0.1 only, plus the frozen brief.  
**Rule applied:** local omission ≠ architectural gap unless unit, scope, family, external supply and interface adequacy are resolved. UNRESOLVED retained where evidence is insufficient.

## 1. Unit-resolution table

| Unit | Declared type | Resolved type(s) | Declared/local scope | Local ownership of tested relations? | Delegation/external relation | AUR note |
|---|---|---|---|---|---|---|
| N0 Northstar Platform Architecture | CIA | CIA | Integrated Northstar architecture; validates, stores, retrieves, records provenance, supports correction | Owns platform-level integration and correction support declaration | Components N1–N6, N10–N11 | CIA, but component documents are intentionally scoped |
| N1 Intake Gateway | SUB | SUB | Receives uploads; sends payload to Validation Engine; returns status | Does **not** own scientific validation rules | N2 Validation Engine via explicit handoff/return | Local omission is intentional scoping / external satisfaction |
| N2 Validation Engine | SUB | SUB | Applies scientific validation rules; emits validation result | Owns validation rules; does **not** own long-term storage/UI | N3 Archive Store and N5 Provenance Ledger receive validated event | Local storage omission is intentional scoping |
| N3 Archive Store | SUB | SUB | Preserves accepted payloads; authorised retrievability | Owns archive preservation/retrieval; correction handling delegated | Says corrections handled by N4, but no interface detail | Correction-related interface is inadequate |
| N4 Correction Service | SUB | SUB | Evaluates correction requests; approves/rejects; produces corrected package | Owns correction decision/package capability | Approved packages “returned to archive workflow”; no invoker, archive receipt, or provenance notification | Interface gaps to intake, archive, provenance |
| N5 Provenance Ledger | SUB | SUB | Preserves source, validation-rule version, acceptance, authorised history | Owns provenance record; can record correction events if supplied | No correction-event interface defined | Capability present; handoff absent |
| N6 Researcher Portal | INT/SUB | INT/SUB | Upload, status, retrieval; invokes N1; queries N3 | Does **not** currently own correction-request control | Future comment references Review Hub; no Review Hub source | Correction intake not operational; Review Hub unresolved |
| N7 Experimental Similarity Scanner | DN | DN | Experiment only; image-similarity detection | Explicitly not production validation | No declared interface to N2 | Rejected from production validation family |
| N8 Observatory Dashboard | separate neighbouring project | external neighbouring system / not Northstar | Telescope scheduling/weather telemetry | Uses “validation” only for weather-feed formatting | No Northstar reference | Rejected from Northstar validation family |
| N9 Legacy Curator API | REF | REF | Retired pre-Northstar service; migration history only | Once accepted curator correction requests; now decommissioned | No current interface | Historical/provenance source only; not current operational family |
| N10 Export Bundle Specification | INT | INT | Defines portable export from N3 + N5 | Does not store records | Explicitly assembled from N3 and N5 | Storage omission is intentional scoping |
| N11 Retention Policy Note | CORE | CORE | Governs retention constraint | Does not implement retrievability/provenance | No implementation owner specified, but N3/N5 exist in platform | CORE constraint, not implementation component |

## 2. Relevant-family map

### A. Validation family for N1/N2/N7/N8

**Candidate relation:** scientific validation of submissions.

**Admitted family:** N1 Intake Gateway, N2 Validation Engine, N0 Northstar CIA as context.  
**Membership evidence:** N1 → N2 explicit payload handoff; N2 applies validation rules; N2 returns status to N1; N0 declares validation function.

**Rejected:** N7 Experimental Similarity Scanner — explicit experiment only, no production interface.  
**Rejected:** N8 Observatory Dashboard — separate project, different domain, no Northstar reference.

**Closure:** N1’s lack of validation rules is resolved externally by N2 through adequate interface. No structural validation gap at N1.

### B. Archive/storage/export family for N2/N3/N10

**Candidate relation:** long-term preservation of accepted datasets.

**Admitted family:** N2 Validation Engine, N3 Archive Store, N5 Provenance Ledger, N0 Northstar CIA.  
**Interface evidence:** N2 sends validated payload and rule version to N3 and N5.

**Rejected as storage owner:** N10 Export Bundle Specification — interface specification, not archive.  
**Rejected as storage owner:** N11 Retention Policy Note — CORE constraint, not implementation.

**Closure:** N2 and N10 do not need local storage. N3 owns preservation; N5 owns provenance. No structural storage gap in N2/N10.

### C. Correction family for N0/N3/N4/N5/N6/N9

**Candidate relation:** correction request → correction decision → archive update → provenance update.

**Admitted current family:** N0 Northstar CIA, N3 Archive Store, N4 Correction Service, N5 Provenance Ledger, N6 Researcher Portal.  
**Contextual/constraint family:** N11 Retention Policy Note, as a CORE retention/provenance constraint.

**Rejected as current operational member:** N9 Legacy Curator API — decommissioned, no current interface. Retain only as REF historical evidence.

**Rejected as undefined reference:** Review Hub — named in N6 comment but no source exists. Not admitted as family member.

**Rejected:** N7 and N8 — not correction-related.

**Closure:** Not closed as external or distributed satisfaction. The correction family resolves enough to show required path is not established. Dominant issue: multiple interface gaps. The researcher-to-correction intake link additionally has an unresolved named reference.

## 3. A–J analyses

| Case | Target D | Candidate relation R | Unit resolution | Local scope | Relevant family | Interface / external test | Closure | AUR classification | Result |
|---|---|---|---|---|---|---|---|---|---|
| A | N1 Intake Gateway | Scientific validation rules | SUB | N1 not intended to own validation | N1 + N2 + N0 | N1 sends payload to N2; N2 validates; N2 returns status; N2 sends provenance event | FC-2 external/delegated resolution | **AUR-C3** externally satisfied; also C2 scoping rationale | Claim false. N1 is not structurally incomplete merely because it lacks validation rules. |
| B | N3 Archive Store | Correction handling / archive update | SUB | N3 owns archive; correction delegated to N4 | N3 + N4 + N5 + N0 | Only “handled by Correction Service”; no trigger, payload, handoff, return, replacement rule, provenance update | External claim fails interface adequacy | **AUR-C6** interface gap | Claim false. Saying N4 handles corrections does not make N3 complete. |
| C | N2 Validation Engine | Long-term preservation of accepted datasets | SUB | N2 not intended to own storage | N2 + N3 + N5 + N0 | N2 sends validated payload to N3; N3 preserves; N5 receives validation event | FC-2 external resolution | **AUR-C3** externally satisfied; C2 scoping rationale | Claim false. N2 is not structurally incomplete for lacking long-term storage. |
| D | Northstar correction architecture | Complete end-to-end correction path | N0 CIA + N3/N4/N5/N6 SUBs | N0 declares correction support; components scoped | N0 + N3 + N4 + N5 + N6 | Intake absent; N4 invocation absent; N4→N3 archive receipt vague; N5 correction-event interface absent | Not FC-2/FC-3; multiple interface failures | **AUR-C6** primary; possible **AUR-C7** only for intake sub-function if no responsible owner admitted | Claim false. Complete correction architecture is not established. |
| E | N7 Similarity Scanner | Production validation family membership | DN | Explicitly experiment only | No production validation family interface | No declared interface to N2 | FC-4 inapplicable | **AUR-C8** inapplicable; DN scoping | Claim false. Similar topic ≠ same architectural family. |
| F | N8 Observatory Dashboard | Northstar validation satisfaction | Separate neighbouring project | Weather-feed formatting only | No Northstar family membership | No Northstar reference or interface | FC-4 inapplicable | **AUR-C8** inapplicable | Claim false. Word “validation” does not create family membership. |
| G | N9 Legacy Curator API | Current correction-request intake | REF | Decommissioned; migration history only | Not current correction family; REF historical only | No current interface | FC-4 for current operation | **AUR-C8** for current correction intake | Claim false. N9 proves historical capability only, not current intake. |
| H | N10 Export Bundle | Storage of accepted records | INT | Export specification only | N10 + N3 + N5 + N0 | N10 assembled from N3 and N5 | FC-2 external resolution | **AUR-C2/C3** | Claim false. N10 does not have a structural storage gap. |
| I | N11 Retention Policy | Implementation of retrievability/provenance | CORE | Governing constraint, not implementation | N11 + N0 + N3 + N5 | N3 supplies retrievability; N5 supplies provenance; N11 does not implement | C2 local scoping | **AUR-C2** intentional local scoping | Claim false. CORE note is not incomplete merely because it does not implement. |
| J | Correction-request intake | Current researcher correction request intake | Unresolved role; N6 portal lacks control; N4 evaluates requests | No current intake control in N6 | N6 + N4 + N3 + N5 + N0; N9 rejected; Review Hub undefined | N6 no correction control; N4 invoker unidentified; N9 decommissioned; Review Hub no source | Not closed; Review Hub unresolved | **AUR-C6** for intake interface; **AUR-C9** for Review Hub reference | Claim false. Only evidence is future/undefined; no current intake established. |

## 4. Correction-family interface-adequacy analysis

Required chain:  
**Source Unit → Trigger / Handoff → Responsible Unit → Required Function → Return / Consequence Propagation → Provenance**

| Link | Source | Trigger / Handoff | Responsible unit | Required function | Return / propagation | Provenance | Adequacy |
|---|---|---|---|---|---|---|---|
| Researcher correction request → correction decision | Researcher / N6 | Absent. N6 has no correction-request control. N4 invoker not identified. Review Hub undefined. | N4? Or undefined Review Hub? | N4 can evaluate correction requests | N4 can approve/reject and produce package; “returned to archive workflow” vague | N5 can record correction events, but no interface | **Inadequate.** C6 interface gap; Review Hub C9 unresolved |
| Correction decision → archive update | N4 Correction Service | “Returned to archive workflow” only; no package handoff, receipt, replacement rule | N3 Archive Store | N4 can produce corrected package; N3 can preserve/retrieve | No defined return or consequence propagation | No defined notification to N5 | **Inadequate.** C6 interface gap |
| Archive update / correction workflow → provenance update | N4 / archive workflow | No correction-event interface defined | N5 Provenance Ledger | N5 can record correction events if supplied | No defined return/acknowledgement | N5 itself, but trigger absent | **Inadequate.** C6 interface gap |

**Correction-family conclusion:**  
The supplied architecture does **not** establish a complete path from researcher correction request through correction decision, archive update and provenance update. The strongest classification is **AUR-C6 INTERFACE GAP at multiple links**. The correction-request intake link may also be treated as **AUR-C7** for that sub-function if no responsible intake owner is admitted. The undefined Review Hub remains **AUR-C9 UNRESOLVED** and cannot be invented.

## 5. Rejected-family-candidate register

| Candidate | Claimed family | Reason rejected | AUR safeguard |
|---|---|---|---|
| N7 Experimental Similarity Scanner | Production validation | Explicitly experiment only; no declared interface to N2 | Similar topic ≠ same architectural family |
| N8 Observatory Dashboard | Northstar validation | Separate neighbouring project; no Northstar reference; “validation” used for weather-feed formatting | Topic-family inflation |
| N9 Legacy Curator API | Current correction intake | Decommissioned; migration history only; no current interface | Stale-family / obsolete interface evidence |
| Review Hub | Current correction intake | Referenced only as future design comment; no source exists | Unknown-to-absence / named-neighbour caution |
| N10 Export Bundle | Archive/storage owner | INT export specification; does not store records | Local ownership inflation |
| N11 Retention Policy | Implementation owner of retrievability/provenance | CORE constraint; not implementation component | Representation/structure confusion |

## 6. Unresolved register

| Unresolved item | Evidence | Status |
|---|---|---|
| Review Hub | N6 comment: “Future correction UI may use the Review Hub.” No source elsewhere. | **AUR-C9** unresolved reference; not admitted to family |
| Current correction-request intake owner/trigger | N6 no correction-request control; N4 invoker absent; N9 decommissioned; Review Hub undefined | Interface gap / unresolved |
| What invokes Correction Service | N4 does not identify trigger or caller | Interface gap |
| How Archive Store receives corrected package | N4 says “returned to archive workflow”; N3 gives no receipt, replacement rule, or handoff | Interface gap |
| How Provenance Ledger receives correction event | N5 can record correction events, but no correction-event interface defined | Interface gap |
| Implementation owner for N11 retention policy | N11 does not specify owner | Not a structural gap in CORE; N3/N5 provide likely implementation, but N11 itself does not assign |
| End-to-end correction orchestration | No unit owns full correction workflow | Not established; primary C6, possible C7 for intake sub-function |

## 7. Whole-platform conclusion

The supplied Northstar architecture does **not** establish a complete path from researcher correction request through correction decision, archive update and provenance update.

- **Local omission, intentional scoping:** N1 lacks validation rules; N2 lacks long-term storage; N10 lacks storage; N11 lacks implementation. These are not structural gaps in those units.
- **External/delegated satisfaction:** N1 → N2 validation is adequately connected. N2 → N3/N5 initial validation and storage/provenance are adequately connected.
- **Interface gap:** N3 → N4 correction handling; N4 → N3 archive update; N4/N3 → N5 correction-event provenance. Capabilities exist, but handoffs, returns, replacement rules and provenance propagation are not defined.
- **Unresolved:** Review Hub is named only as a future possibility and has no source. It cannot be used to close correction-request intake.
- **Family-level structural gap?** For the complete correction path, the dominant issue is interface inadequacy, because N4, N3 and N5 possess relevant capabilities. If correction-request intake is treated as a required capability with no admitted owner, then that sub-function is **AUR-C7**; otherwise it is **AUR-C6** with an unresolved named reference.
- **Representation gap?** Not primary. The architecture does mention correction in several places, but the problem is not merely wording; the operational handoffs are missing.
- **Complete correction architecture?** No.

## 8. AUR failure modes / ambiguities exposed

1. **Named-neighbour false satisfaction** — N3 saying “Correction Service handles corrections” is not enough.
2. **Topic-family inflation** — N7 and N8 fail family admission despite validation-like wording.
3. **Capability-without-handoff false satisfaction** — N4 has correction capability, but intake/archive/provenance interfaces are absent.
4. **C2 vs C3 overlap** — Intentional local scoping often coincides with external satisfaction; both can describe N1, N2, N10.
5. **C6 vs C7 boundary** — When capabilities exist but handoffs are missing, it is not always clear whether to classify as interface gap or family-level structural gap.
6. **C9 for undefined references** — Review Hub is named but unsourced; AUR correctly prevents invention but leaves the intake link unresolved.
7. **Future/design comments** — AUR does not clearly state how much weight to give future-facing comments that are not current architecture.
8. **Multiple unit types** — N6 is INT/SUB; N0 is CIA; N9 is REF. Type resolution works, but classification depends on whether the audit targets current operation or historical provenance.
9. **CORE vs implementation** — N11 shows that a CORE constraint can be judged incomplete if the auditor wrongly expects implementation.
10. **Family closure under missing interfaces** — AUR allows stopping at interface inadequacy, but the closure label is less crisp than the AUR-C6 classification.

## 9. Final assessment: was AUR v0.1 usable without hidden source-project context?

**Yes.** Using only AUR v0.1 and the frozen test brief, the audit can be performed. AUR provided sufficient safeguards to:

- reject false structural-gap claims for N1, N2, N10 and N11;
- reject topical/false-family candidates N7, N8 and N9;
- identify N3/N4/N5 correction relations as interface gaps rather than local structural gaps;
- keep Review Hub unresolved rather than inventing it;
- conclude that Northstar does not establish a complete end-to-end correction path.

**Caveat:** AUR v0.1 is usable but not fully deterministic at a few boundaries: C2 vs C3, C6 vs C7, and C9 treatment of undefined future references. Those ambiguities do not prevent the blind transfer test, but they do mean some classifications require explicit reasoning rather than a mechanical result. Overall, AUR v0.1 is adequate for this blind transfer test without hidden source-project context.
