# Independent Evaluator Report — STRA-BTT-001
**Specification under test:** State Triggered Review Architecture — Portable Specification v0.1
**Test:** STRA-BTT-001 / Blind Transfer Test 001
**Method posture:** Independent, non-Concord, architectural only. No real industrial-safety determination is made.

## 1. Scope and basis

I evaluated STRA v0.1 only against the supplied fictional MIS scenario. I did not assume Concord architecture, the Civilisation Clock, KCS, CDT, or any Concord governance layer. I treated the scenario as an architectural pressure test of representation, uncertainty, routing, ownership, cascade control, privacy, temporal ordering, and revalidation.

STRA’s core kernel is usable here:

> represent condition → bind state/evidence → watch → evaluate → signal review/action candidacy → route to legitimate owner → record outcome → continue/reset/correct/supersede.

The critical invariant set — especially **Condition Satisfied ≠ Action Authorised**, **Review Due ≠ Required Outcome**, **Missing Evidence ≠ Condition False**, **Timestamp Order ≠ Universal Material Precedence**, and **Relevance Returned ≠ Validity Restored** — is directly relevant to A–M.

---

## 2. Scenario representation A–M

| Case | STRA trigger class(es) | Representation and expected STRA state | Key boundary |
|---|---|---|---|
| A — Periodic inspection | TEMPORAL, possibly COMPOUND | 18-month review is a temporal backstop, not sole trigger. Represent as `TemporalBackstop OR risk/event/evidence triggers`. | Avoid calendar collapse if time becomes the only meaningful trigger. |
| B — Vibration-risk condition | RISK / STATE / COMPOUND | Condition requires **validated** vibration-risk state > R. Raw crossing + unresolved calibration warning = not validated satisfaction. State: CONDITION-PARTIAL/UNKNOWN, not REVIEW-DUE. | Raw threshold crossing ≠ validated risk threshold. |
| C — Capability prerequisite | CAPABILITY / COMPOUND | `Rig Q AVAILABLE AND VALIDATED for envelope`. AVAILABLE true; VALIDATED incomplete. State: CONDITION-PARTIAL. | AVAILABLE ≠ VALIDATED. |
| D — Dependency condition | DEPENDENCY | `Project U reconsidered when M reaches ACCEPTED operational state`. Project DB says COMPLETE; acceptance register says ACCEPTANCE PENDING. State: DISPUTED/UNKNOWN; not satisfied. | COMPLETE ≠ ACCEPTED; inconsistent sources not resolved by STRA. |
| E — Event recurrence | RECURRENCE / EVENT | BF-7-like event shares symptoms but differs in load/lubricant. Equivalence disputed. State: DISPUTED / review-routing-required, not automatic recurrence satisfaction. | Symptom similarity ≠ material recurrence. |
| F — New evidence | EVIDENCE | Supplier dataset genuine, but batch-match to installed fleet unknown. Existence ≠ material change. State: UNKNOWN/CONDITION-PARTIAL; request materiality/revalidation. | New evidence does not automatically invalidate old guidance. |
| G — Stale trigger | STATE / DEPENDENCY / STALE | Branch F retired at v8; v9 unreachable. Trigger records still say WATCHING. Trigger definition must be reviewed. Outcome: suspend/supersede/retire or route for ownership. | WATCHING ≠ meaningful forever. |
| H — Privacy-limited condition | RISK / STATE / privacy-limited | Authorised process emits `THRESHOLD-MET`, `THRESHOLD-NOT-MET`, `UNCERTAIN`. STRA consumes bounded result only. | Privacy does not require disclosure of protected source material. |
| I — Ownership gap | Any class; ownership/routing issue | Condition becomes CONDITION-SATISFIED, but owner disputed. State: CONDITION-SATISFIED / ROUTING-UNRESOLVED. | Condition satisfaction does not create an owner. |
| J — Participant-declared notification | PARTICIPANT / CAPABILITY / COMPOUND | Contractor asks notify when MIS validates diagnostic capability D for remote use. Technically available, validation pending. State: CONDITION-PARTIAL; no notification yet. | Technical availability ≠ validation. |
| K — Trigger cascade | COMPOUND / cascade control | Risk-review trigger fires; five downstream triggers would auto-activate. Need materiality, depth, duplicate, owner/routing checks. | A fired risk trigger does not justify every downstream trigger. |
| L — Temporal ordering | EVENT / STATE / order interface | Alert 10:04; action 10:02 on possibly slow contractor clock. Need external consequence-relevant ordering. State: UNKNOWN/DISPUTED unless reconciled. | Earlier timestamp ≠ material precedence. |
| M — Retrieval/reactivation | RECURRENCE / EVIDENCE / memory interface | Archived investigation may be relevant to BF-7, but valid for older bearing generation. STRA signals relevance and requests retrieval/revalidation. | Retrieved historical material is not automatically current. |

---

## 3. Required analyses

### 2. B — Raw threshold crossing is not validated satisfaction

The condition is not “raw sensor value exceeds R.” It is “validated vibration-risk state exceeds R.” STRA must bind both the sensor/risk source and the validation/calibration provenance. Because calibration is unresolved, the validated risk state is not established. The correct evaluation is **UNKNOWN**, or at most **CONDITION-PARTIAL** if modelled as `calibration-valid AND threshold-exceeded`. It must not become **CONDITION-SATISFIED** or **REVIEW-DUE** merely because the raw number crossed a numerically associated value. If MIS wants calibration warning itself to trigger review, that must be a separate declared trigger.

### 3. C — Compound capability trigger

This maps directly to STRA’s worked example A. The condition is:

> `Rig Q AVAILABLE AND VALIDATED for pressure/temperature envelope`.

AVAILABLE is true. VALIDATED is incomplete/UNKNOWN. STRA records **CONDITION-PARTIAL**, not REVIEW-DUE. When validation evidence is later established, the compound condition can become satisfied and route a seal-material qualification review candidate to the legitimate engineering owner. STRA does not certify Rig Q and does not approve the seal material.

### 4. D — Inconsistent dependency states

The dependency condition requires M to reach **ACCEPTED** operational state. A project database saying **COMPLETE** is not the same represented state as ACCEPTED. The engineering acceptance register saying ACCEPTANCE PENDING directly contradicts treating the dependency as satisfied. STRA should preserve the conflict as **DISPUTED** or, if the acceptance register is authoritative, as not satisfied. It must not resolve the discrepancy by inference. The correct output is a routing/reconciliation need, not dependency satisfaction.

### 5. E — BF-7 recurrence

STRA’s recurrence class requires distinguishing same label, similar pattern, and materially equivalent recurrence. The new event shares two symptoms but differs in load profile and lubricant history. One engineer claims recurrence; another denies established equivalence. STRA should record **DISPUTED** and route the equivalence question to the legitimate domain owner. It must not fire recurrence satisfaction merely on symptom overlap. If host semantics say disputed equivalence itself warrants review, STRA may signal a review-routing requirement, but it does not declare BF-7 recurrence.

### 6. F — New supplier evidence

The fatigue dataset is genuine, but its applicability to MIS’s installed material batch is unestablished. STRA’s EVIDENCE trigger requires material change to the represented decision state. Existence of new evidence is weaker than material change. The correct treatment is **UNKNOWN/CONDITION-PARTIAL** plus a request for materiality assessment or revalidation. STRA preserves the prior state rather than rewriting history: prior guidance → new evidence → review/revalidation due or not → revised/retained state. The old guidance is not automatically invalidated.

### 7. G — Stale/impossible Controller C trigger

The condition “Branch F reaches version 9” is impossible if Branch F was permanently retired at version 8. The trigger records still saying WATCHING are stale. STRA’s stale/impossible trigger provisions permit review of the trigger definition itself. Correct treatment is to flag the trigger as stale/impossible, preserve its history, and route it for one of: modify, reset, suspend, supersede, retire, or ownership resolution. It should not remain meaningfully WATCHING forever. STRA v0.1 lacks explicit **IMPOSSIBLE** and **RETIRED** states, which is a specification/interface ambiguity, but the intended treatment is clear from section 29.

### 8. H — Privacy-limited signal

STRA does not need the underlying incident investigation content. It needs only the bounded condition result. The authorised safety process can emit:

- `THRESHOLD-MET` → condition satisfied, REVIEW-DUE, route to authorised owner;
- `THRESHOLD-NOT-MET` → condition not satisfied;
- `UNCERTAIN` → UNKNOWN/DISPUTED.

This satisfies minimum-necessary observation. The trigger must not become a pretext for broad retrieval or disclosure. The protected source material stays outside STRA. Routing must be restricted to the legitimate owner, not all engineering staff.

### 9. I — Ownership gap

The condition is satisfied, but the lease renegotiation leaves ownership disputed among MIS operations, equipment owner, and service contractor. STRA can produce **CONDITION-SATISFIED / ROUTING-UNRESOLVED**. It must not invent an owner or execute the substantive consequence. Section 23 says exactly this: if ownership is unresolved, STRA may produce condition-satisfied plus routing-unresolved rather than action. The trigger should route for ownership resolution.

### 10. J — Contractor notification

The participant-declared condition is: notify me if MIS validates diagnostic capability D for remote use. Technical availability is not validation. Formal remote-use validation remains pending. Therefore the condition is **CONDITION-PARTIAL/UNKNOWN**, not satisfied. No notification should be generated yet. When MIS validates the capability, STRA may generate the declared notification. It must not infer consent to any further action beyond the declared consequence. Identity/consent/continuity remain external.

### 11. K — Containing the trigger cascade

The risk-review trigger firing does not authorise automatic activation of all five downstream triggers. STRA’s cascade controls should apply:

- provenance of trigger creation;
- cycle/depth limits;
- duplicate suppression;
- materiality checks;
- owner/routing validation;
- human/domain review where consequence warrants.

Only the engineering review may be immediately due if its own condition is satisfied. Procurement, shutdown planning, contractor notification, and second risk review should remain candidates or dormant until materiality is determined. The second risk-review trigger in particular risks a cycle. The correct output is bounded cascade, not automatic propagation.

### 12. L — Timestamp/order problem

STRA may consume an externally supplied consequence-relevant ordering relation. It must not infer material precedence from timestamps alone. The contractor clock may be slow, so the 10:02 timestamp does not prove the maintenance action materially preceded the alert condition. Unless an event-order/reconciliation system supplies a reliable ordering with provenance and confidence, the result should be **UNKNOWN/DISPUTED**. Timestamp order is not universal material precedence.

### 13. M — Archived-investigation retrieval/revalidation

The seven-year-old investigation may be relevant to BF-7, but it was valid for an older bearing generation. STRA owns the relevance/trigger signal, not retrieval or domain use. The correct sequence is:

> relevance signal → legitimate retrieval → revalidation → domain use or return to dormant state.

It should issue a **revalidation request**, not an immediate substantive use signal. Relevance returned does not restore validity. The memory/knowledge system owns retrieval/provenance; the domain owner decides current applicability.

---

## 4. Relevant STRA failure modes

If implemented correctly, the scenario exposes these risks:

- **STRA-F1 — Calendar collapse:** A, if the 18-month backstop becomes the only trigger.
- **STRA-F2 — Trigger-authority collapse:** I/K, if satisfaction is treated as authority.
- **STRA-F3 — False satisfaction:** B, C, D, F, J.
- **STRA-F4 — False non-satisfaction:** B, C, D, F, where missing/uncertain evidence is treated as false.
- **STRA-F5 — Stale trigger:** G.
- **STRA-F6 — Impossible trigger persistence:** G.
- **STRA-F7 — Event overmatching:** E.
- **STRA-F8 — Cascade amplification:** K.
- **STRA-F9 — Dependency absorption:** D, if STRA tries to resolve the whole dependency graph.
- **STRA-F10 — Domain absorption:** E/F/M, if STRA decides material equivalence or validity.
- **STRA-F11 — Consent bypass:** J.
- **STRA-F12 — Privacy leakage:** H.
- **STRA-F13 — Stale reactivation:** M.
- **STRA-F14 — Ownership vacuum:** I.
- **STRA-F15 — Total-order assumption:** L.
- **STRA-F16 — Completeness illusion:** D/F/L, where unobserved or unreconciled state is assumed settled.

The kernel itself, as written, does not force these failures. They occur if the host collapses STRA’s separations or if missing interfaces are filled by convenience assumptions.

---

## 5. Specification/interface ambiguities exposed

STRA v0.1 does **not** need to become a Concord architecture, but the test exposes several bounded specification/interface gaps:

1. **No explicit `IMPOSSIBLE` or `RETIRED` state.** Section 29 allows retirement/supersession outcomes, but the state vocabulary lacks them.
2. **No explicit `ROUTING-UNRESOLVED` state.** Section 23 uses the phrase, but it is not in the minimum trigger-state vocabulary.
3. **Compound uncertainty semantics are under-specified.** How should `A AND UNKNOWN`, `A OR UNKNOWN`, `NOT UNKNOWN`, or `A AND DISPUTED` resolve? Section 22 says preserve uncertainty according to declared semantics, but no default or minimum algebra is given.
4. **Materiality interface is not formalised.** STRA correctly says materiality is domain-supplied, but it does not define a minimum materiality declaration object or evaluation interface.
5. **Validation/authority interface is thin.** CAPABILITY distinguishes claimed, available, validated, authorised, but there is no explicit interface for validation evidence or authority provenance.
6. **Dependency reconciliation is external but under-described.** Conflicting source states such as COMPLETE vs ACCEPTED/PENDING need an explicit reconciliation/routing interface.
7. **Recurrence/event equivalence is domain-owned but not interfaced.** STRA says domain determines equivalence, but there is no standard way to record a disputed equivalence determination and route it.
8. **Privacy signal semantics are not specified.** The three-token signal in H maps cleanly, but STRA does not define a privacy-preserving result interface.
9. **Cascade controls are host-dependent.** Section 30 lists controls, but no minimum defaults, depth limits, or materiality gate are specified.
10. **Ownership resolution has no process.** STRA can say ROUTING-UNRESOLVED, but it does not define how resolution is requested or tracked.
11. **Temporal ordering interface needs provenance/confidence.** Section 26 says STRA may consume an external ordering relation, but does not require confidence, source, or reconciliation status.
12. **Stale-trigger review cadence is optional.** Section 29 permits periodic/backstop review of trigger definitions but does not make it mandatory.

These are not necessarily failures of the portable kernel. They are specification/interface issues that a v0.2 should either clarify or explicitly externalise.

---

## 6. Host/domain implementation choices

The following are not STRA decisions; MIS must supply them:

- define threshold R and what “validated vibration-risk state” means;
- define calibration-warning handling and sensor-validation authority;
- define Test Rig Q validation authority and required pressure/temperature envelope;
- define whether project DB or engineering acceptance register is authoritative for M, or define reconciliation;
- define BF-7 material-equivalence criteria and who decides;
- define fatigue-dataset materiality and material-batch matching;
- define trigger-definition review cadence and retirement authority for Controller C;
- define privacy boundary, authorised safety process, and routing restrictions;
- define ownership-resolution mechanism for the leased compressor;
- define what “MIS validates” means for diagnostic capability D;
- define cascade materiality gates and which downstream triggers are independent;
- define event-order/reconciliation service and clock-skew handling;
- define archive revalidation authority for older bearing-generation analysis.

---

## 7. Useful findings not explicitly requested

1. **STRA transfers without importing the Civilisation Clock.** The scenario is materially non-Concord and the kernel still applies.
2. **The invariant set is the strongest part of the architecture.** It prevents the most dangerous collapses in B, C, D, E, F, G, I, J, K, L, and M.
3. **Privacy-limited evaluation fits STRA naturally.** Because STRA needs only a bounded condition result, it can work with `THRESHOLD-MET/NOT-MET/UNCERTAIN` without exposing protected content.
4. **Stale-trigger hygiene should be treated as a first-class lifecycle concern.** G shows that WATCHING can become a false persistent state.
5. **Cascade control needs a materiality gate before downstream activation.** K shows that a fired risk trigger can otherwise become an accidental authority chain.
6. **Ownership resolution is a recurring boundary.** I and K both show that condition satisfaction can outrun legitimate ownership.

---

## 8. Transfer classification

**Classification: STRA-T3 — Functional transfer.**

STRA v0.1 transfers coherently and usefully into the MIS domain without assuming Concord architecture. It can represent the trigger classes, preserve uncertainty, separate satisfaction from authority, route to owners, handle privacy-limited signals, request revalidation, and contain cascades in principle.

It is not **STRA-T4** because the test exposes material specification/interface ambiguities: missing explicit states for impossible/retired/routing-unresolved, incomplete compound uncertainty semantics, thin materiality and validation interfaces, and host-dependent cascade/ownership-resolution rules. These are bounded issues rather than fundamental failures.

It is clearly above **STRA-T2** because there are no major hidden Concord assumptions, and the mechanism provides substantial usable structure across all scenario pressures.

---

## 9. Conclusion

STRA v0.1 survives the blind transfer test as a useful standalone architecture. Its core mechanism correctly refuses to collapse raw sensor crossing into validated risk, availability into validation, COMPLETE into ACCEPTED, similarity into recurrence, new evidence into invalidation, WATCHING into permanence, condition satisfaction into ownership, technical capability into validation, risk-trigger firing into cascade authority, timestamp order into material precedence, or retrieval into current validity.

The remaining issues are not “STRA decides the wrong thing.” They are “STRA v0.1 does not fully specify how some boundary outcomes are recorded, reconciled, or governed.” That is a **functional transfer with bounded specification/interface gaps** — **STRA-T3**.
