# Independent Evaluator Response — STRA-BTT-002

**Scope:** Used only STRA v0.2 and the frozen BTT-002 scenario. No Concord architecture or BTT-001 assumptions imported. No silent repair of v0.2.

## 1. Mapping and evaluation A–N

| Case | STRA class(es) | Evaluation and state | Key constraint preserved |
|---|---|---|---|
| **A — Dormant transient hypothesis** | EVIDENCE + CAPABILITY + COMPOUND; TEMPORAL backstop for trigger-definition review | One observation matches S is not two independently validated observations. Second candidate is uncertain. Instrument N lab Q is not commissioned operational validated sensitivity Q. First disjunct: not satisfied / partial. Second disjunct: not satisfied / unknown. Overall: **CONDITION-PARTIAL / UNKNOWN**, not REVIEW-DUE for H. The 30-month condition is a **TEMPORAL backstop on trigger-definition review**, not automatic H review. | Candidate evidence ≠ validated pair; lab capability ≠ operational capability; backstop ≠ substantive outcome. |
| **B — Instrument capability** | CAPABILITY | Lab calibration reaching Q is at most claimed/available/lab-validated. Orbital commissioning incomplete means operational validated/authorised state is UNKNOWN or not reached. State: **CONDITION-PARTIAL / UNKNOWN** depending on host definition. | Capability claimed/available/validated/authorised distinction retained. |
| **C — Dependency disagreement** | DEPENDENCY | Required state is RELEASED. Dashboard says COMPLETE; calibration authority says RELEASE REVIEW PENDING. COMPLETE ≠ RELEASED. Use bounded reconciliation \(R_h\). Until resolver returns RELEASED, dependency is not satisfied. State: **WATCHING / UNKNOWN / DISPUTED** as reconciled. | Dependency trigger ≠ dependency graph ownership; conflicting state not flattened. |
| **D — Evidence/materiality** | EVIDENCE + materiality interface | Credible paper changes a parameter estimate, but material change to H’s evidential state is undetermined. Consume \(M_t\). If \(M_t\) result is UNKNOWN, condition is UNKNOWN. State: **WATCHING / UNKNOWN**, not REVIEW-DUE. | New evidence exists ≠ material change; STRA not scientific judge. |
| **E — Recurrence/equivalence** | RECURRENCE | Similar duration/spectrum but different spatial environment; two groups dispute class membership. Similarity ≠ materially equivalent recurrence. State: **DISPUTED**, routed to domain-owned equivalence resolver or \(R_h\). No REVIEW-DUE until equivalence confirmed. | Same label ≠ similar pattern ≠ materially equivalent recurrence. |
| **F — Privacy/access-limited participant condition** | PARTICIPANT + privacy boundary | Access office may expose only SHAREABLE / NOT-SHAREABLE / UNKNOWN. Consume bounded privacy-preserving result \(P_r\). SHAREABLE → CONDITION-SATISFIED / notification candidate; NOT-SHAREABLE → not satisfied; UNKNOWN → UNKNOWN. | Participant trigger ≠ consent to every consequence; no raw legal/contractual content. |
| **G — Ownership transition** | Routing/ownership | Trigger condition may be satisfied, but two successor consortia dispute ownership. State: **CONDITION-SATISFIED / ROUTING-UNRESOLVED**. No substantive review/action executes until legitimate owner resolved. | Need for action ≠ authority to invent actor. Role separation required. |
| **H — Trigger cascade** | COMPOUND / CASCADE | Only anomaly review is unquestionably appropriate before materiality. Parent anomaly trigger may become REVIEW-DUE for anomaly review. Archive retrieval may be relevance signal. Observation scheduling, public alert drafting, partner notification, and alert-generated anomaly trigger require own conditions, materiality gate, owner/routing validation. State: parent REVIEW-DUE; children DORMANT/blocked. | Cascade provenance, cycle detection, duplicate suppression, materiality gate, owner validation. |
| **I — Ordering uncertainty** | EVENT + event-order interface | 03:09 timestamp does not prove material precedence over 03:11 when clock sync is UNKNOWN. Consume external consequence-relevant ordering relation with provenance/confidence. State: **UNKNOWN / DISPUTED** for ordering-dependent trigger. | Timestamp order ≠ universal material precedence. |
| **J — Impossible trigger** | CAPABILITY/STATE/EVENT | Telescope R decommissioned; detector generation 5 will not arrive. Condition unreachable. State: **IMPOSSIBLE**, then route for RETIRED / SUPERSEDED / modified. Do not fabricate detector generation 5. Six-year unreviewed WATCHING is stale/impossible persistence. | Long-lived WATCHING requires bounded definition review/backstop. |
| **K — Superseded/retired trigger** | SUPERSEDED / duplicate suppression | T2 explicitly replaced T1. T1 should be **SUPERSEDED**, not WATCHING. Replica exposing T1 as WATCHING is stale state. Downstream subscribing to both must not double-activate same consequence. | Correction/supersession history; duplicate activation suppression. |
| **L — Compound uncertainty** | COMPOUND | A=TRUE, B=UNKNOWN, C=FALSE, D=UNKNOWN. (A AND B) → UNKNOWN. (A AND B) OR C → UNKNOWN OR FALSE → UNKNOWN. “Unless D” expressed as AND NOT D gives UNKNOWN AND UNKNOWN → UNKNOWN. Overall: **UNKNOWN**, not REVIEW-DUE. | v0.2 §22A: TRUE AND UNKNOWN → UNKNOWN; FALSE OR UNKNOWN → UNKNOWN; NOT UNKNOWN → UNKNOWN. |
| **M — Bounded reconciliation** | DEPENDENCY/STATE + reconciliation | Two systems disagree on VALIDATED. STRA lacks authority to inspect material. Consume \(R_h\): VALIDATED → satisfied; NOT-VALIDATED → not satisfied; DISPUTED → DISPUTED; missing → UNKNOWN. | State label without provenance ≠ validation; bounded reconciliation. |
| **N — Ownership-resolution tracking** | Routing/ownership-resolution | Satisfied trigger, no settled owner. State: **CONDITION-SATISFIED / ROUTING-UNRESOLVED** across three cycles. Preserve trigger, condition state, candidate consequence, disputed/unknown owners, routing request, provenance, resolution status. | No legitimate owner invented; unresolved-owner record retained. |

## 2. Frozen-test scenario findings

- **A/B:** STRA v0.2 correctly prevents collapse of candidate observations into validated pairs and lab capability into commissioned operational capability. The main need is host definition of “independently validated” and “validated sensitivity Q.”
- **C/M:** Bounded reconciliation is the correct interface. C shows COMPLETE vs RELEASED is a host/dependency semantic mismatch, not an STRA authority. M directly exercises \(R_h\) and privacy-limited validation.
- **D/E:** Materiality and recurrence equivalence remain domain-owned. STRA can preserve UNKNOWN/DISPUTED without becoming the scientific judge.
- **F:** Privacy-preserving bounded result works: STRA can receive SHAREABLE/NOT-SHAREABLE/UNKNOWN without exposing legal/contractual records.
- **G/N:** Role separation and ROUTING-UNRESOLVED are adequate for ownership vacuum, but N exposes a missing portable backstop for long-pending ownership-resolution.
- **H/K:** Cascade and supersession controls are present, but duplicate suppression depends on host source-of-truth and downstream subscription discipline.
- **I/J/L:** Ordering, impossible triggers, and compound uncertainty are handled by existing v0.2 interfaces and semantics.

## 3. Mechanism failures

No fundamental STRA v0.2 mechanism failure was observed in A–N.

The relevant failure risks are:

- **STRA-F3 False satisfaction** — if A/B/C/D/E collapse partial, lab, dashboard, credible, or similar states into satisfaction.
- **STRA-F4 False non-satisfaction** — if missing calibration/validation is treated as false.
- **STRA-F5 Stale trigger** — J and K if supersession/impossible handling is ignored.
- **STRA-F6 Impossible trigger persistence** — J if kept WATCHING indefinitely.
- **STRA-F7 Event overmatching** — E and I if similarity or timestamps fire triggers.
- **STRA-F8 Cascade amplification** — H if children activate without own conditions/materiality/owner.
- **STRA-F11 Consent bypass** — F if notification becomes broader action.
- **STRA-F12 Privacy leakage** — F/M if STRA inspects protected source material.
- **STRA-F13 Stale reactivation** — A/J if dormant material treated as current.
- **STRA-F14 Ownership vacuum** — G/N if no legitimate owner is resolved.
- **STRA-F15 Total-order assumption** — I if timestamps prove precedence.
- **STRA-F16 Completeness illusion** — C/M if unrepresented dependency state is assumed absent.

These are failure-mode risks, not observed v0.2 mechanism failures under the frozen scenario.

## 4. Specification/interface ambiguities and defects

1. **“Unless” semantics are not explicitly specified.**
   v0.2 supports A AND NOT C, so “unless D” can be expressed as AND NOT D. But natural-language “unless” exception semantics are not defined in the condition grammar. L can be evaluated as UNKNOWN, but the host must declare the exact structure.

2. **Ownership-resolution tracking lacks a portable backstop/escalation requirement.**
   N can remain ROUTING-UNRESOLVED across cycles. v0.2 requires preservation of the unresolved-owner record, but does not require periodic trigger-definition review, escalation, or terminal routing after N cycles. This is adjacent to stale-trigger control but not explicitly covered.

3. **Cascade duplicate suppression is host-conditional.**
   v0.2 says suppress duplicate activation “where host semantics allow.” K shows a stale replica can expose T1 as WATCHING while T2 supersedes it. If the host does not define source-of-truth and downstream subscription rules, double activation remains possible. This is an interface/integration ambiguity more than a kernel defect.

4. **Capability validation/authorisation interface is not fully shaped.**
   v0.2 requires provenance for AVAILABLE/VALIDATED/AUTHORISED and distinguishes claimed/available/validated/authorised where material. B still depends on host definition of whether lab calibration or orbital commissioning is the relevant capability state. This is a legitimate host choice, but the interface could be pressured more explicitly for operational commissioning.

5. **Temporal backstop on trigger-definition review vs subject review is not separately named.**
   A says “Review trigger definition no later than 30 months.” v0.2 supports temporal backstops, but the scenario requires distinguishing trigger-definition review from H-review. The mechanism can represent this, but the specification does not strongly foreground the distinction.

6. **Bounded reconciliation does not specify next step when resolver returns DISPUTED.**
   v0.2 allows result/status including DISPUTED, but the follow-on routing or escalation is host-defined. This is acceptable for a portable kernel but remains an interface ambiguity.

## 5. Host/domain choices

These are not STRA mechanism defects; they are legitimate host/domain determinations that v0.2 requires:

- define “independently validated observation” and whether uncertain calibration counts;
- define operational vs laboratory capability and commissioning requirements;
- define RELEASED authority and reconcile COMPLETE vs RELEASED;
- define materiality criterion for parameter-estimate change;
- define event-class equivalence for recurrence;
- define legal shareability and access-office signal mapping;
- define successor ownership-resolution process;
- define cascade depth/rate limits, materiality gates, and owner validation;
- define clock-sync/order confidence and reconciliation;
- define decommission retirement/supersession process;
- define supersession propagation to replicas and downstream services;
- define escalation/backstop for unresolved ownership.

## 6. Useful unrequested findings

- v0.2’s strongest transfer feature is the invariant separation: condition satisfied ≠ review due ≠ legitimate owner ≠ substantive outcome.
- The main pressure points in BTT-002 are not trigger classes. They are semantic interfaces: materiality, equivalence, reconciliation, operational validation, ownership resolution, and supersession propagation.
- Ownership-resolution tracking may need the same bounded-review discipline as stale triggers. N shows that a satisfied trigger can remain unresolved indefinitely without violating the letter of v0.2.
- Supersession must be treated as a source-of-truth and integration problem, not merely a state label. K can defeat duplicate suppression if replicas and downstream services do not honor SUPERSEDED.
- v0.2 successfully avoids absorbing scientific, legal, dependency-graph, or ownership authority in A–N.

## 7. Transfer classification

**STRA-T3 — Functional transfer.**

STRA v0.2 transfers functionally into the AVON observatory/research-programme domain. All A–N cases map to v0.2 trigger classes, states, and interfaces without importing the Civilisation Clock or manufacturing substantive authority. The mechanism handles non-temporal triggers, uncertainty, compound conditions, privacy-limited signals, ownership vacuum, cascade risk, impossible triggers, supersession, and bounded reconciliation.

It does not reach **STRA-T4 — Strong transfer** because several portable semantics remain under-specified or host-dependent: “unless” exception semantics, ownership-resolution backstop/escalation, cascade duplicate suppression against stale replicas, and operational-vs-lab capability validation. These are ambiguities and host choices rather than fundamental mechanism failures.

**Bottom line:** BTT-002 supports **STRA-T3 functional transfer**, with no observed fundamental failure. The v0.2 revisions improve portability, but the remaining defects are interface-level and should be frozen for a further bounded test if T4 is desired.
