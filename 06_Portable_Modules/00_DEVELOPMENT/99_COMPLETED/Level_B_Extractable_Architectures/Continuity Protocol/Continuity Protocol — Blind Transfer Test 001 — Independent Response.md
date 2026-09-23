# Continuity Protocol — Blind Transfer Test 001 — Independent Response

**Test:** CP-BTT-001  
**System:** Northbridge Regional Diagnostic Laboratory / NOVA  
**Source:** Independent clean-instance response supplied after freeze of test brief and expected-findings key  
**Preservation status:** VERBATIM RESPONSE / NOT EDITED

---

# Continuity Audit — CP-BTT-001  
**System:** Northbridge Regional Diagnostic Laboratory / NOVA  
**Scope:** Operational and information continuity only. No clinical decision is made.  
**Evidence used:** Test Brief CP-BTT-001 and *Continuity Protocol — Portable Specification v0.1* only.

---

## Task A — Continuity-object resolution

The principal continuity object is **not NOVA as an implementation**. It is:

> The legitimate urgent diagnostic analysis function performed by NOVA/Northbridge, restorable within 24 hours after loss of the primary NOVA environment, with sufficient provenance to identify the assay method, instrument configuration and result-processing rules used.

A secondary continuity object is:

> The associated provenance, configuration knowledge and correction capability needed to understand how a reported result was produced and to avoid restoring known-bad states.

NOVA’s application servers, database, exact file formats and current vendor platform are **containers/implementation details**, not necessarily the continuity object. If Phoenix can perform the same legitimate diagnostic function with transferred provenance, continuity can still succeed. The managers’ claim that “continuity requires NOVA itself to be restored exactly as it was” risks **F2 — Implementation Immortality** and **F14 — Over-Preservation**.

The declared target also allows a reduced emergency service only if it can safely process the defined urgent test set. Therefore the continuity object includes the **minimum safe urgent-service function**, not merely the existence of backups.

## Task B — State classification

Using CS1–CS6, provisional classifications are:

| Item | Current continuity state | Explanation |
|---|---|---|
| **N2 — Nightly backup** | **CS2–CS3 at best; not CS5** | It is recorded and likely accessible/interpretable to the same administrators, but it shares building power, identity service, privileged account and file formats with N1. No full restoration has been attempted in three years. As data copy it may be CS1–CS3; as disaster recovery for loss of primary NOVA it does not establish recoverability. Single label hides this distinction. |
| **N3 — Cloud archive** | **CS1–CS2; partial CS3 at most; not CS4/CS5** | The archive exists and integrity checks passed, but the decryption key is in the on-site HSM, restoration instructions refer to an unavailable OS image, and archived instrument drivers are untested on current replacement hardware. It is not actionable or recoverable as a whole. |
| **N4 — Printed recovery binder** | **CS1–CS3 for declaration/contacts; not CS4 for technical recovery** | Off-site, readable, interpretable at a high level. It contains emergency contacts, diagram, declaration sequence, urgent assay list and archive name. It lacks decryption procedure, schema, instrument-interface details and current configuration versions. It can guide declaration but not restoration. |
| **N7 — Emergency bench** | **CS6 for six of twenty urgent assays; CS5/CS6 only for that subset; not CS6 for the full urgent set** | It physically and procedurally provides a real degraded service for six assays and records its own provenance. It cannot process the remaining fourteen and cannot reproduce automated throughput. Overall, it is degraded continuity, not full urgent-service continuity. |
| **N9 — Retired rule set** | **CS3 for historical/provenance value; CS4 installable but operationally invalid** | It is archived with excellent provenance and records why it was superseded. As historical/failure knowledge it is well preserved. As current operational restoration it must remain superseded; using it would be **F6 — Obsolete-State Resurrection**. |

## Task C — Dependency and recovery-basis analysis

Critical dependencies that prevent existing arrangements from automatically establishing 24-hour recoverability include:

- Independent site/power. N2 shares the same building and power supply as N1. N8 is permanently connected to N1’s storage controller.
- Independent identity and privileged access. N2 uses the same identity service and privileged account as N1.
- Decryption capability. N3’s key is held in the on-site HSM, which may be lost with the primary environment.
- Compatible operating environment. N3’s restoration instructions refer to an OS image no longer supplied by the vendor.
- Hardware/instrument-driver compatibility. Archived instrument drivers have not been tested on current replacement hardware.
- Current configuration and result-processing rules. N4 lacks schema, interface details and current configuration versions. N9 is obsolete and unsafe as current operation.
- Calibration dependencies. Dr Vale understands undocumented calibration dependencies; no formal transfer has occurred.
- Unknown calibration package. N14 may be required but cannot be located.
- Licence dependency. N13’s legacy licence server may shut down in four months with no established offline/replacement/migration path.
- Provenance transfer. Phoenix has not demonstrated transfer of all provenance records or conversion of all historical NOVA configuration.
- Verification. No full restoration from N2 has been attempted in three years; no practical recovery exercise is evidenced.
- Authority/permission for succession. N12 lacks contract, data-access permission, governance approval and formal handoff.

A minimum plausible recovery basis for the declared target, using only scenario evidence, would include:

1. A tested, independently powered recovery environment not dependent on N1’s site, identity service or storage controller.
2. Recoverable decryption credentials or key material available independently of the lost primary site.
3. A supported OS image or validated replacement platform.
4. Compatible instrument interfaces/drivers, or validated Phoenix equivalents, for the urgent assay set.
5. Current, validated assay configuration and result-processing rules, including N10’s corrected unit-conversion rule and excluding N9’s superseded rule.
6. Documented calibration dependencies formerly held by Dr Vale, or verified Phoenix calibration equivalents.
7. A valid licence path for NOVA or Phoenix.
8. Transferred provenance sufficient to identify assay method, instrument configuration and result-processing rules for urgent results.
9. Trained operators and recovered permissions.
10. A written restoration/migration sequence and practical verification test for the urgent assay set.
11. A fallback degraded path, such as N7 for six assays, while full recovery is attempted.
12. Authority to declare the emergency and lawful permission to access/operate data, supplied independently of the continuity protocol.

> **Minimum Recovery Basis ≠ Copy of Current System.**  
> A copy of N1 is not sufficient without the dependencies above.

## Task D — Redundancy analysis: N2, N3, N8

Do not count copies mechanically.

- **N2** is not an independent disaster backup. It shares building, power, identity service, privileged account and file formats with N1. Its failure modes are correlated with N1 for site loss, power loss, identity compromise, admin error, ransomware and format obsolescence.
- **N3** has greater geographic/provider independence because it is an external cloud archive with independent integrity checks. However, its recovery basis is not independent: the decryption key is on-site in the HSM, restoration instructions refer to an unavailable OS image, and archived drivers are untested on replacement hardware. It may survive while remaining unusable.
- **N8** consists of three mirror drives permanently connected to N1’s storage controller. They share the same controller, power, identity, environment and corruption/deletion pathways. Three copies do not create three independent failure domains.

Conclusion: **Redundancy ≠ Independence.** N2 and N8 are correlated with N1. N3 is geographically independent but still has critical dependency-chain gaps. The arrangement risks **F8 — Single-Point Preservation** and **F9 — Correlated Redundancy**.

## Task E — Phoenix / implementation continuity

Migration to Phoenix can be consistent with continuity even though NOVA itself changes. The specification explicitly rejects stasis:

> **Continuity ≠ Stasis**  
> Current software ≠ necessarily required service.

Phoenix can be a legitimate successor implementation if it preserves the **legitimate diagnostic function** and the **provenance/knowledge** needed to understand results.

For Phoenix to satisfy the declared continuity target, the following must still be preserved or transferred:

- The urgent assay set and its validated performance on Phoenix.
- Traceability from Phoenix methods/instrument configurations/result-processing rules back to prior NOVA provenance where relevant.
- Current result-processing rules, including the corrected unit-conversion rule from N10.
- Exclusion of the superseded 2024 rule set from operational recovery.
- Conversion or mapping of historical NOVA configuration sufficient for the declared target.
- Transfer of provenance records, not just data.
- Validation of the non-urgent assay set if it falls within the eventual continuity target.
- Licence, support, training and permission dependencies for Phoenix.
- A handoff/succession record because Phoenix replaces NOVA as the implementation.

The managers’ exact-NOVA argument is not required by the specification unless some dependency cannot be transferred. The unresolved Phoenix gaps mean Phoenix is not yet a complete continuity answer: it is **CP-C6** for implementation succession, potentially **CP-C4** for the urgent set if dependencies are resolved, but still **CP-C2/CP-C7/CP-C9** for the full declared target because historical configuration, provenance transfer and non-urgent assays are not demonstrated.

## Task F — Degraded continuity: N7 emergency bench

N7 provides:

- A physically separate laboratory.
- Independent power.
- Locally stored procedures.
- Manual performance of **six of twenty urgent assays**.
- Its own assay provenance recording.

N7 does **not** provide:

- The remaining fourteen urgent assays.
- NOVA’s automated throughput.
- NOVA’s configuration, instrument interfaces or result-processing rules.
- Full urgent-service coverage if the defined urgent test set is all twenty assays.

Therefore N7 provides **CP-C5 — DEGRADED CONTINUITY** for a subset. If the declared urgent-service target requires all twenty urgent assays, N7 is below target and also **CP-C2/CP-C7** for the missing fourteen. It is valuable as a minimum-safe fallback, but it cannot be presented as satisfying the full urgent-service continuity claim.

## Task G — Obsolete state and failure knowledge: N9 and N10

**N9 — Retired 2024 rule set**  
Preserve it as historical and provenance material. It is valuable because it records what was superseded and why. The archive clearly states that one rule could incorrectly classify a particular result pattern. That knowledge helps prevent future regression.

Operationally, it must **not** be restored as current. Easier installation is not a legitimate reason to resurrect a known-superseded rule. Doing so would be **F6 — Obsolete-State Resurrection** and could undermine the declared provenance/safety target.

Classification: **CS3 historical/provenance preservation**; installable in a narrow technical sense but not a valid operational recovery basis for the current target.

**N10 — Failed migration record**  
This is a continuity asset under the specification’s “honest failure as continuity data.” It records the attempted mapping, discrepancy, root cause, corrected rule and verification data. The current migration uses the corrected rule. N10 should be preserved and used to prevent repeating the unit-conversion failure.

N10 is not a state to restore operationally; it is knowledge that improves the recovery basis for Phoenix/NOVA migration.

## Task H — Succession and authority: N12

The proposed consortium succession must separate:

- **Continuity/succession requirements:** function to continue, predecessor state, successor, information/capability transferred, unresolved liabilities/dependencies, handoff evidence, activation point, verification, fallback.
- **Legitimacy/permission/authority:** contract, data-access permission, governance approval, legal/ethical authority, hospital contracts, ownership of laboratory data.

The planning note says the consortium “automatically inherits Northbridge’s authority.” This is incorrect under the specification:

> **Continuity ≠ Authority**  
> **Succession ≠ Automatic Legitimacy**

No contract, data-access permission, governance approval or formal handoff has been completed. The Operations Director can declare a NOVA operational emergency under existing governance, but the documentation grants no additional authority over clinical standards, employment, hospital contracts or ownership of laboratory data. The Director cannot simply transfer that authority to the consortium.

Classification: **CP-C6** for succession if chosen, **CP-C7** for missing authority/permission/handoff, **CP-C9** for the unverified inheritance claim, and **CP-C10** for unresolved status. Also risks **F12 — Succession Without Handoff** and **F13 — Succession-as-Legitimacy**.

## Task I — Personnel/tacit-knowledge continuity: N5 and Dr Vale

Dr Vale holds undocumented calibration dependencies for the original assay configuration. Two engineers can operate NOVA normally but would need her help to reconstruct those dependencies after a total rebuild. She plans to retire in six months. No formal knowledge-transfer exercise has occurred.

Current state: the knowledge is accessible through Dr Vale while she remains available. For recovery purposes, it is a critical dependency, not a preserved asset. If she retires without transfer, the dependency may become irrecoverable.

Required state for recovery: at least **CS3–CS4** documentation/procedures for the calibration dependencies, verified by the engineers and preferably by Dr Vale before retirement.

Classification: **CP-C7 — Critical Dependency Gap** now. If no transfer occurs before retirement, it may become **CP-C8 — Irrecoverable Loss Identified**. This is a clear **F5 — Dependency-Chain Blindness** and **F8 — Single-Point Preservation** risk.

## Task J — Unresolved dependencies: N13 and N14

Use the specification’s epistemic and ESCP safeguards. Do not invent facts.

**N13 — Legacy licence server**  
NOVA requires a vendor licence service during installation. The old service will shut down in four months. Northbridge has not established whether an offline licence, replacement licence or migration path will remain. This is a known critical dependency with an approaching deadline.

Classification: **CP-C7** for the dependency gap, with **CP-C10** because the actual availability of alternatives is unresolved. If no licence path exists and NOVA must be restored, this may become **CP-C8**.

**N14 — Unknown calibration package**  
An engineer remembers an external specialist once supplied a calibration package for one uncommon analyser. The current team cannot locate it or establish whether it is still required. No one knows whether Dr Vale has a copy.

Under ESCP:

> No recovery mechanism found in examined space ≠ no recovery mechanism exists.

Classification: **CP-C10 — UNRESOLVED**. If evidence later shows the package is required and unavailable, it becomes **CP-C7** and possibly **CP-C8**. The correct action is to expand the evaluation space: search records, ask Dr Vale, contact the specialist/vendor, test whether the analyser still needs the package.

## Task K — Overall classification

Multiple classifications apply to different sub-functions.

1. **Current full NOVA 24-hour recovery claim**  
   **CP-C2 — Preserved but below required state**  
   **CP-C7 — Critical dependency gap**  
   **CP-C9 — Continuity claim unverified**  
   Not **CP-C1**. Some preservation exists, but independent power, decryption/key recovery, compatible OS/drivers, current configuration, Dr Vale’s calibration knowledge, licence path and practical restoration testing are missing or unverified. **CP-C8** is not yet proven, but possible for some dependencies. **CP-C10** applies to unresolved items.

2. **Emergency degraded continuity**  
   **CP-C5 — Degraded continuity** for N7’s six-assay subset.  
   **CP-C2/CP-C7** for the remaining fourteen urgent assays and full urgent-service target.

3. **Phoenix migration continuity**  
   **CP-C6 — Succession required** for implementation replacement, if NOVA will not be restored as the primary platform.  
   **CP-C4 — Recoverable with identified dependencies** for the urgent set, if Phoenix validation and provenance transfer are completed.  
   **CP-C2/CP-C7/CP-C9** for the full declared target because historical configuration conversion, provenance transfer and non-urgent assay operation are not demonstrated.

4. **Proposed consortium succession**  
   **CP-C6 — Succession required/contemplated**  
   **CP-C7 — Critical dependency gap** for authority, permission and handoff  
   **CP-C9 — Continuity claim unverified**  
   **CP-C10 — Unresolved**  
   The planning note’s automatic inheritance claim is not supported by the specification.

5. **Unknown calibration dependency**  
   **CP-C10 — Unresolved**  
   Possible **CP-C7** if later shown required and unavailable; possible **CP-C8** if irrecoverable.

## Task L — Minimal continuity record

**Object:** Northbridge NOVA urgent diagnostic analysis service and associated provenance/knowledge.  
**Value/function:** Restore urgent diagnostic analysis within 24 hours after loss of primary NOVA, with sufficient provenance to identify assay method, instrument configuration and result-processing rules. Reduced emergency service acceptable only if it safely processes the defined urgent test set.  
**Audit level:** Service/organisational operational-information continuity; no clinical decision.  
**Relevant disruption:** Loss of primary NOVA environment; also Dr Vale retirement, licence-server shutdown, hardware/format obsolescence, possible succession to consortium.  
**Current state (CS1–CS6):** N1 is CS6. Overall full recovery capability is approximately CS2–CS3, with N7 as CS6 for six assays only. Full urgent-service recovery is not CS5.  
**Required state (CS1–CS6):** CS5 for the full urgent-service recovery basis, then CS6 for restored urgent operation; CS3–CS4 for historical/failure knowledge.  
**Critical dependencies:** Independent site/power; independent identity/credentials; HSM decryption key; supported OS; compatible instrument drivers/hardware; current assay configuration; current result-processing rules; calibration dependencies/Dr Vale; licence path; schema/interfaces; provenance transfer; trained staff; authority/permissions; practical restoration/migration tests.  
**Recovery basis:** Tested independent recovery environment; recoverable credentials/key; current validated urgent assay config/rules; compatible interfaces/drivers/licence; documented calibration dependencies; provenance mapping; trained operators; restoration/migration procedure and verification; N7 fallback for six assays; Phoenix urgent-set migration if completed.  
**Redundancy/independence:** N2 and N8 are correlated with N1. N3 is geographically independent but key/instructions/drivers create dependency-chain gaps. Redundancy ≠ independence.  
**Trigger:** Declaration of NOVA operational emergency by Operations Director; loss of primary; licence shutdown; Dr Vale retirement; failed integrity/restoration test; scheduled Phoenix migration; consortium handoff.  
**Restoration or succession path:** Restore NOVA from an independent recovery basis if possible; otherwise migrate urgent set to Phoenix with validated provenance/config transfer; use N7 for six assays interim; formal handoff if consortium succeeds.  
**Authority/permission dependency:** Operations Director only declares emergency under existing governance. No additional authority over clinical standards, employment, hospital contracts or data ownership. Consortium requires independent contract, data-access permission and governance approval.  
**Verification method:** Practical restoration/migration exercises; urgent assay validation; provenance checks; driver/licence/OS compatibility tests; check that N9 is not active; use N10 corrected rule; post-recovery review.  
**Known failure modes:** F1 Archive Theatre; F2 Implementation Immortality; F5 Dependency-Chain Blindness; F6 Obsolete-State Resurrection; F8 Single-Point Preservation; F9 Correlated Redundancy; F11 Restoration Without Verification; F12 Succession Without Handoff; F13 Succession-as-Legitimacy; F15 Under-Preservation; F16 Correction-Capacity Loss.  
**Known irrecoverable loss:** Not yet confirmed. Possible loss: Dr Vale’s calibration knowledge, N14 package, licence path, historical configuration/provenance if not transferred. Record as uncertainty.  
**Provenance:** N9 supersession record; N10 failed migration record; current config versions; provenance records for reported results.  
**Review condition/date:** Before Dr Vale retirement (six months); before licence-server shutdown (four months); after any restoration test; at Phoenix migration milestones; before consortium handoff.  
**Uncertainty:** N14 unknown; licence path unknown; whether Dr Vale has N14 copy unknown; drivers on replacement hardware untested; full restoration untested; ESCP limits apply.

# Required final assessment

1. **Was Continuity Protocol v0.1 usable without Concord-specific source context?**  
   Yes, largely. The portable specification supplied the necessary concepts: continuity object vs container, CS1–CS6, recovery basis, dependency analysis, redundancy vs independence, succession vs authority, provenance, failure knowledge, degraded continuity and CP classifications. The audit could be performed without inspecting Concord source architecture.

2. **Ambiguity that materially affected classification.**  
   The main ambiguities were:
   - The boundary between CS2, CS3, CS4 and CS5 when material exists but has not been tested.
   - When to classify as CP-C2 “preserved but below required” versus CP-C7 “critical dependency gap” versus CP-C9 “claim unverified.”
   - How to classify an obsolete but well-preserved state like N9: historical CS3 versus technically installable CS4.
   - Whether “degraded emergency service” requires all twenty urgent assays or only a governed minimum-safe subset.
   - What exactly “loss of the primary NOVA environment” covers: room, building, site, identity service or whole operational environment.
   - How to treat partial recovery capability that is real but untested, especially N3.

3. **Missing concept required to complete the audit.**  
   The protocol would benefit from:
   - Explicit RTO/RPO alignment or data-loss tolerance, because N2 nightly and N3 monthly imply different recovery-point gaps.
   - A formal way to define the “minimum safe function” or “defined urgent set” when reduced service is allowed.
   - A confidence/uncertainty scale for unresolved dependencies under ESCP.
   - A clearer dependency-criticality method to distinguish “missing but searchable” from “missing and fatal.”
   - A more explicit handoff/authority matrix for succession cases.

4. **Part of the specification that encouraged a false positive or false negative.**  
   - **Potential false positive:** CP-C4 “recoverable with identified dependencies” could be read optimistically when dependencies are merely named but not actually available or tested. CS6 operational status can also mask lack of recovery capability, although the specification explicitly warns against this.
   - **Potential false negative:** The CS ladder could under-classify N3 as merely CS2 because decryption is blocked, even though the cloud archive itself is geographically independent and may be recoverable if key recovery exists. ESCP correctly warns against treating “not found in examined space” as “does not exist.”
   - **Potential false positive:** CP-C6 succession could be used to treat planned replacement as continuity even when authority, handoff and provenance transfer are absent. The specification’s F12/F13 warnings mitigate this.
   - **Potential false negative:** F2 Implementation Immortality could be over-applied to dismiss exact NOVA restoration even where some dependencies may only work with NOVA.

5. **Is the module ready for revision, further source recovery, or another test?**  
   The module appears usable but not yet ready for a validation claim. It should go to **revision** to clarify CS/CP boundary rules, degraded-service definitions, RTO/RPO, uncertainty handling and succession/authority separation. After revision, it should undergo **another independent blind transfer test**, preferably with a different non-Concord domain. Further source recovery is not obviously required for this audit; the portable specification was usable without Concord-specific context. The next step is revision and then another blind test, not a claim of demonstrated reliable independent transfer.
