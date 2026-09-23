# Continuity Protocol — Blind Transfer Test 002 — Independent Response

**Test:** CP-BTT-002  
**Specification:** Continuity Protocol — Portable Specification v0.2  
**Source:** Independent clean-instance response supplied after freeze of test brief and expected-findings key  
**Preservation status:** VERBATIM RESPONSE / NOT EDITED

---

# CP-BTT-002 — Independent Response

Using only the supplied test brief and Continuity Protocol v0.2.

## Task A — Continuity object and target

**Continuity object:** safe minimum water service for Pelagos, not the Atlas plant itself. Atlas is the current implementation; the valuable continuity object is the function of delivering treated water to designated community storage points at or above MAF.

**Declared target:**
- **MAF:** 1.4 million litres/day treated water delivered to designated community storage points.
- **RTO:** MAF restored within 18 hours of loss of the primary plant.
- **RPO:** operational water-quality and dosing records no more than 2 hours old at recovery.
- **Disruption envelope:** loss of the desalination plant building and installed control equipment, while the rest of the island remains physically accessible. Port closure, loss of all communications, and regional fuel unavailability are outside the primary envelope.

These must be evaluated separately because they answer different questions. RTO asks how fast service returns. RPO asks how much recent operational state may be lost. MAF asks what minimum service counts as success. The disruption envelope asks which failure scenario is being claimed. A recovery can meet RTO and MAF while failing RPO, or preserve records while missing RTO. Meeting one does not imply meeting the others.

## Task B — Object-relative CS classification

| Item | Component/artefact state | Whole-continuity implication |
|---|---|---|
| **P2 — Daily control archive** | **CS4 — Actionable** for the archived material: documented, readable, restorable into simulator. | Cannot meet RPO ≤2h because export is daily. Component is actionable, but the overall RPO path is below target. |
| **P3 — Swift standby plant** | **CS5 — Recoverable** for MAF: tested, independent local controls, startable within 6h. | Swift can likely reach MAF capacity within RTO, but its water-quality log syncs from Atlas every 8h, creating an RPO/dependency gap. High component state ≠ high system recovery state. |
| **P4 — Paper chemistry procedures** | **CS4 — Actionable** for current treatment procedures. | They support chemistry recovery but do not contain control-system configuration. They are not sufficient alone for full Atlas rebuild. |
| **P12 — Old emergency manual** | Technically **CS3/CS4** as a readable/actionable historical artefact. | Invalid for current restoration. It describes a retired chlorine dosing arrangement. It should remain provenance/history, not active recovery instruction. |

## Task C — Fast recovery exercise P11

- **RTO:** Swift reached 1.6 ML/day after 5 hours. 5h < 18h. RTO met.
- **MAF:** 1.6 ML/day > 1.4 ML/day. MAF capacity met, subject to delivery to designated storage points.
- **RPO:** restored operational record set was 7 hours old. 7h > 2h. RPO violated.

Therefore P11 does **not** satisfy the declared continuity target. Management’s statement that it “met the continuity target because service returned inside the RTO” is incomplete and treats RTO as if it were the whole target. The exercise demonstrates partial success: MAF/RTO achieved, RPO failed.

## Task D — MAF and Swift’s fuel basis

Swift satisfies the **production capacity** part of MAF: 1.6 ML/day exceeds 1.4 ML/day, and 6-hour start is inside the 18-hour RTO.

What is not explicitly established:
- that Swift’s output is delivered to the designated community storage points;
- that Swift’s water-quality/dosing records meet the 2-hour RPO;
- that all treatment/chemical dependencies are available.

The verified 72-hour fuel store establishes fuel sufficiency for at least 72 hours at MAF output. For the declared 18-hour RTO, this is sufficient fuel evidence. It does **not** establish long-duration resilience beyond 72 hours, port-independent resupply, full-service restoration, or that other critical dependencies remain available.

## Task E — Dependency evidence and criticality

| Dependency | Evidence state | Criticality relative to declared target |
|---|---|---|
| P5 — Membrane supplier | End-of-production: **DOCUMENTED**. Compatible replacement: **UNRESOLVED**. | **CRITICAL** for long-term Atlas rebuild/supplier continuity. Not immediately fatal for 18h MAF if Swift/Tide paths work, but a critical gap for eventual replacement. |
| P6 — Alleged calibration dongle | **UNRESOLVED** existence and necessity. | Cannot be labelled CRITICAL or FATAL-IF-UNAVAILABLE on current evidence. Record as an unresolved possible dependency. Do not invent its role. |
| P7 — Mira and conversion script | Script source: **DOCUMENTED**. Two transformation rules: **UNRESOLVED**. Mira’s unique knowledge: **INFERRED/VERIFIED** by scenario. | **CRITICAL** for Tide succession and historical database continuity. Could become fatal if no other path exists, but current evidence supports “critical/unresolved,” not definitive fatal. |
| P15 — Fuel store | **VERIFIED** sufficient for 72h at MAF output. | **CRITICAL** for Swift MAF operation, but satisfied for the declared 18h RTO. Beyond 72h is **UNRESOLVED**. |

## Task F — Function versus implementation: Tide

Tide can provide continuity of the **function** despite replacing Atlas, because the continuity object is safe minimum water service, not the Atlas plant. Tide’s acceptance tests show 4.2 ML/day and water-quality compliance. Legitimate authority has approved it once commissioning conditions are satisfied.

However, Tide’s continuity succession is not yet complete. Historical record migration is unfinished, sensor mapping is incomplete, and the method for connecting Tide records to the historical database is not verified. So Tide can be a valid replacement implementation, but it is not yet a fully demonstrated continuity successor.

## Task G — Succession and authority

P9 establishes valid authority for Tide to become the replacement plant once commissioning conditions are satisfied. That is necessary but not sufficient.

P10 shows an incomplete handoff: missing historical sensor mapping, Mira’s two unexplained transformation rules, and no verified method for connecting Tide’s records to the historical database.

Therefore:
- legitimate authority exists;
- capability/knowledge handoff is incomplete;
- continuity succession is active but not complete;
- **Continuity ≠ Authority** and **Succession ≠ Automatic Legitimacy** both apply. Authority does not substitute for operational handoff.

## Task H — Historical/current validity: P12

The 2018 emergency manual is readable, complete, and technically actionable. But it is **not valid for current restoration** because it instructs use of a chlorine dosing arrangement retired in 2023. The current manual supersedes it and records why.

So P12 is:
- **CS3/CS4** as a historical/provenance artefact;
- **not valid** as current recovery instruction;
- a risk of **F6 — Obsolete-State Resurrection** if used operationally.

## Task I — Continuity mechanism fossilisation: P13

The master continuity spreadsheet is stale. It lists a former supplier, a departed staff member, and a decommissioned recovery server, yet remains formally designated as the master continuity plan.

This shows the continuity mechanism itself lacks review, adaptation, and correction capacity. It is a case of **F17 — Continuity Fossilisation** and likely also **F1 — Archive Theatre** / **F11 — Restoration Without Verification** in spirit: the plan exists, but it does not represent current recoverability.

A continuity mechanism needs its own continuity: ownership, review triggers, update procedure, and authority to replace obsolete content.

## Task J — Disruption-envelope discipline: P14

The port dependency does not automatically invalidate the bounded primary claim. The primary disruption envelope explicitly excludes island-wide port closure. Per the protocol:

> Recovery under one disruption envelope ≠ recovery under every disruption envelope.

Port closure should be handled as a **separate disruption envelope**, with its own dependency analysis, RTO, RPO, MAF, and evidence state. If port closure is included, then membrane/chemical resupply may become a critical or fatal dependency. But that does not retroactively fail the narrower plant-loss claim.

## Task K — Overall classifications

| Item | Classification(s) | Rationale |
|---|---|---|
| 1. Swift MAF functional recovery | **CP-C1** for MAF capacity/RTO sub-function; **CP-C7/C9** for RPO/log sub-function | Swift can reach MAF within RTO, but the 8h log sync creates an RPO dependency gap. Decompose rather than collapsing to one label. |
| 2. P11 overall declared continuity target | **CP-C2 + CP-C7** | RTO and MAF met, but RPO failed. Aggregate state is preserved below required target, with a critical record-freshness dependency gap. Management’s full-success claim is false. |
| 3. Atlas rebuild dependency state | **CP-C7 + CP-C10** | Membrane replacement unresolved, Mira’s transformation rules unresolved, dongle unknown. Critical dependency gaps and unresolved evidence. |
| 4. Tide succession | **CP-C6 + CP-C7 + CP-C9** | Succession path is required/active and authority is valid, but handoff is incomplete and record-connection method is unverified. |
| 5. Master continuity spreadsheet | **CP-C3 + CP-C9** | Recorded/archived only; stale and not actionable/current. Also a fossilised continuity mechanism. |

## Task L — Minimal continuity record

**Object:** Pelagos safe minimum water service.  
**Value/function:** Deliver ≥1.4 ML/day treated water to designated community storage points through disruption and eventual plant replacement.  
**Audit level:** System-level continuity of safe minimum water service.  
**Relevant disruption:** Loss of Atlas plant building and installed control equipment.  
**Disruption envelope:** Atlas building/control-equipment loss; rest of island physically accessible. Port closure, total communications loss, and regional fuel unavailability excluded.  
**RTO:** MAF restored within 18 hours.  
**RPO:** Water-quality and dosing records ≤2 hours old at recovery.  
**MAF:** 1.4 ML/day treated water delivered to designated storage points.  
**Current state (CS1–CS6):** Normal service CS6 via Atlas. For declared envelope, Swift MAF recovery is approximately CS5, but RPO record path is below target. Tide succession is CS4–CS6 with handoff gaps.  
**Required state (CS1–CS6):** CS5 pre-disruption recoverable basis sufficient to reach CS6 MAF after trigger, meeting RTO/RPO/MAF.  
**Critical dependencies and evidence state:** Swift + fuel: VERIFIED for 72h/MAF and 6h start. Paper procedures: CS4, but no control config. Daily archive: documented/restorable, but 24h export cannot meet RPO. Membrane supplier: DOCUMENTED end-of-production; replacement UNRESOLVED. Mira script/rules: script DOCUMENTED, two rules UNRESOLVED. Calibration dongle: UNRESOLVED. Tide authority: VERIFIED; handoff incomplete.  
**Recovery basis:** Swift for immediate MAF; paper chemistry procedures; current manual; daily archive for historical records; Tide as eventual successor. Missing: ≤2h water-quality/dosing record path, verified delivery to designated storage, complete sensor mapping, membrane replacement plan, Tide record integration.  
**Redundancy/independence:** Swift has independent local controls and independent fuel store. But Swift’s water-quality log syncs from Atlas every 8h, creating correlated dependency. Port is a single external dependency for membranes/chemicals outside primary envelope.  
**Trigger:** Loss/failure of Atlas plant or control equipment; activate Swift; begin Tide succession when commissioning conditions satisfied.  
**Restoration or succession path:** Swift for immediate MAF; Atlas rebuild if possible; Tide as replacement successor. Tide has authority but incomplete handoff.  
**Authority/permission dependency:** Island authority defines MAF and has approved Tide once commissioning conditions are met. Continuity analysis does not create authority.  
**Verification method:** Swift full production test and disaster exercise; Tide acceptance tests; archive simulator restoration. Needed: end-to-end RPO test, delivery-to-storage verification, sensor-mapping handoff test, Tide historical database connection test.  
**Known failure modes:** F5 dependency-chain blindness; F6 obsolete-state resurrection; F9 correlated redundancy; F10 interpretation decay; F11 restoration without verification; F12 succession without handoff; F17 continuity fossilisation.  
**Known irrecoverable loss:** None definitively established. Potential loss of Mira’s two transformation rules if not handed off; potential membrane-model loss after production ends; unknown dongle dependency.  
**Provenance:** Atlas records, supplier end-of-production statement, Tide authority approval, disaster exercise record, current and old manuals, Mira’s script and partial documentation.  
**Review condition/date:** Before Mira leaves; before membrane production ends; after Tide commissioning; after RPO fix; if port dependency enters scope; periodic review.  
**Uncertainty:** Delivery to designated storage; dongle necessity; replacement membrane availability; Mira’s two rules; Tide record integration; long-duration fuel beyond 72h; port-closure envelope.

## Final assessment

1. **Was v0.2 usable without source context?**  
   Yes. The scenario could be analysed using only the portable specification and test brief. The protocol’s distinctions were sufficient to identify the main continuity issues.

2. **Did the new RTO/RPO, MAF, Disruption Envelope and evidence-state concepts reduce ambiguity?**  
   Yes. RTO/RPO separation directly exposed the false success claim in P11. MAF clarified the minimum service target. Disruption Envelope prevented port closure from incorrectly invalidating the bounded primary claim. Evidence states prevented documentation from being treated as verified recoverability.

3. **Remaining ambiguity:**
   - CS classification of a tested standby plant: CS5 versus CS6.
   - How to label mixed outcomes where RTO/MAF pass but RPO fails.
   - Whether MAF includes production only or also delivery/quality.
   - Criticality when an alternative successor path exists but is incomplete.
   - Combining CP-C2, CP-C7 and CP-C9 without forcing one label.

4. **False-positive/false-negative pressure:**
   - v0.2 reduces false positives: it blocks “RTO met” from being treated as full target success; blocks authority from being treated as complete succession; blocks redundancy from being treated as independence.
   - It could create false negatives if RPO failure makes an otherwise functional MAF recovery appear wholly failed. The decomposition rule helps, but clear guidance on mixed RTO/RPO outcomes would reduce this.

5. **Another revision before graduation review?**  
   No structural revision is required. v0.2 handled the delta test. A minor clarification or v0.2.1 note would help before graduation review, especially on mixed RTO/RPO classification, MAF delivery/quality scope, standby CS5/CS6, and C6/C7/C9 combination.
