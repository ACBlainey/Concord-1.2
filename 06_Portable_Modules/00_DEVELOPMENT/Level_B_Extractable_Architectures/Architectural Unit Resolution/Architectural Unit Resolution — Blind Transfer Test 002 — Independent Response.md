# AUR-BTT-002 — Independent Blind Delta Analysis

**Method used:** AUR v0.2 only, plus the frozen brief.  
**Rule applied:** local omission ≠ architectural gap unless unit, scope, family, external supply and interface adequacy are resolved. UNRESOLVED retained where evidence is insufficient.

## 1. Unit / scope table

| Unit | Declared type / status | Declared or apparent function | Relevant local scope state for audited cases |
|---|---|---|---|
| H0 | Integrated architecture | Manages access to research facilities; states credential issuance, door enforcement, access-event recording and appeal are separate functions | Fuller-system context. Appeal is architecturally separate. |
| H1 | Subsystem | Collects registration package; submits to Credential Service | Eligibility: NON-LOCAL. Registration intake only. |
| H2 | Subsystem | Determines eligibility; issues credentials; receives revocation events; propagates inactive status | Eligibility and credential state: LOCAL-OWNER. |
| H3 | Subsystem | Door enforcement; checks credential/facility/expiry; sends allow/deny to Event Ledger | Appeal logic: NON-LOCAL / not intended. Door enforcement: LOCAL-OWNER. |
| H4 | Subsystem | Event storage; receives allow/deny events | Storage: LOCAL-OWNER. |
| H5 | Core constraint | Requires appeal access for every rejected registration | Non-implementing constraint. Does not own appeal implementation. |
| H6 | Subsystem | Can receive Appeal Package, review, issue UPHOLD/OVERTURN | Appeal decision: LOCAL-OWNER. Full appeal workflow: PARTIAL. |
| H7 | Reference / provenance | Retired old appeals form; once created Appeal Packages for earlier service | HISTORICAL / PROVENANCE. Not current. |
| H8 | Subsystem / interface | Participant dashboard; roadmap says appeal button planned next release using Appeals Gateway | Planned appeal intake/invocation: CANDIDATE / future. Not current. |
| H9 | Subsystem | Safety revocation service; receives Safety Revocation Notice; sends revocation data to H2 | Revocation intake/forwarding: LOCAL-OWNER. |
| H10 | Separate neighbouring project | Cafeteria loyalty app; uses employee IDs; contains “eligibility review” for meal discounts | Outside Harbourlight access-eligibility family. |
| H11 | Companion document | Explains visitor credential presentation; says technical access decisions are by H3 | Credential decision: NON-LOCAL. Not intended to own issuance/revocation/appeal. |
| H12 | Core constraint | Mandatory current-release emergency access requirement | Non-implementing constraint. No current owner/capability supplied. |
| H13 | Interface specification | Exports selected Event Ledger records; depends on H4 for storage | Storage: NON-LOCAL. |
| H14 | Subsystem / interface | Federation adapter; comment mentions future external Federation Broker | Federation: CANDIDATE / future, not current release. |

## 2. Current-family map

| Case | Target D | Relation/function R | Current relevant family | Membership evidence |
|---|---|---|---|---|
| A | H1 | Decide access eligibility | H1, H2 | H1 explicitly hands complete registration package to H2; H2 determines eligibility and returns APPROVED/REJECTED + Credential ID. |
| B | H3 | Appeal logic | H3, H0 | H0 states appeal is separate; no evidence H3 owns appeal logic. |
| C | H6 / Harbourlight appeal requirement | End-to-end appeal process | H0, H5, H6, H1, H2, H8 candidate; H7 historical excluded | H0 separates appeal; H5 requires appeal for rejected registration; H6 owns appeal decision; H1 is rejection source; H2 holds credential state; H8 is future candidate; H7 retired. |
| D | H7 | Current appeal intake | Current intake family: H0, H5, H1/H2 context, H6, H8 candidate; H7 excluded | H7 retired two years before current release; no current interface points to H7. |
| E | H8 planned Appeals Gateway | Current appeal intake/invocation | H8 as candidate only; not current family | Roadmap note only; no gateway specification; future reference. |
| F | H9 | Safety revocation | H9, H2, H3 | Complete specified chain: H9 receives notice, sends to H2; H2 confirms and propagates inactive status to H3. |
| G | H10 | Harbourlight access eligibility review | H10 excluded | Separate project; meal discounts; no Harbourlight architecture references H10. Similar topic ≠ same family. |
| H | H11 | Credential decision | H11, H3, H2 context | H11 says technical access decisions performed by H3; H11 is orientation companion, not decision owner. |
| I | H12 | Mandatory emergency access capability | H0, H12, H2/H3 context; no current implementer | H12 is mandatory current-release constraint; no supplied current component, interface or candidate implements it. |
| J | H13 | Event storage | H13, H4 | H13 explicitly depends on H4 for event storage and contains no local storage. |
| K | H14 | Current-release federation credential sourcing | H14 current adapter; Federation Broker excluded as future | Federation marked future/not current; no broker identity, spec or deployment evidence. |

## 3. Dependency-status register

| Referenced unit / dependency | Status | Reason |
|---|---|---|
| H2 Credential Service | CURRENT MEMBER | Active subsystem; eligibility, issuance, revocation reception, propagation. |
| H3 Door Enforcement | CURRENT MEMBER | Active subsystem; enforcement and event emission. |
| H4 Event Ledger | CURRENT MEMBER | Active storage subsystem. |
| H6 Appeal Service | CURRENT MEMBER | Active subsystem with appeal decision capability. |
| H7 Old Appeals Form | HISTORICAL / PROVENANCE MEMBER | Retired two years before current release; no current interface. |
| H8 Appeals Gateway / appeal button | CANDIDATE DEPENDENCY | Planned next release; no supplied specification. |
| H9 Safety Revocation Service | CURRENT MEMBER | Active subsystem with fully specified revocation chain. |
| H10 Cafeteria Loyalty App | REJECTED CANDIDATE / separate neighbour | No Harbourlight reference; different function despite “eligibility review” label. |
| H11 Visitor Orientation Guide | CURRENT COMPANION | Explains approved visitor credential presentation; explicitly non-technical. |
| H12 Emergency Override Requirement | CURRENT CORE CONSTRAINT | Mandatory for current release; no current implementation. |
| H13 Analytics Export | CURRENT MEMBER | Interface spec depending on H4. |
| H14 Federation Broker | CANDIDATE DEPENDENCY / FUTURE | Federation marked future/not current; no broker identity/spec/deployment. |

## 4. A–K analyses

### A — H1 eligibility

- Local ownership/scope: **NON-LOCAL**. H1 explicitly does not decide access eligibility.
- Relevant family: H1, H2.
- Dependency status: H2 is CURRENT MEMBER.
- Diagnostic closure: **FC-2 external/delegated resolution**.
- Functional satisfaction: **Yes**. H1 hands off complete registration package; H2 determines eligibility; return is defined.
- AUR classification: **AUR-C3 — EXTERNALLY SATISFIED**.
- Uncertainty/stopping rationale: Low uncertainty. H1’s non-ownership and H2’s ownership are source-grounded; handoff and return are fully defined.

### B — H3 appeal

- Local ownership/scope: **NON-LOCAL**. H3 is not intended to own appeal logic.
- Relevant family: H3, H0.
- Dependency status: H0 current integrated architecture; no current appeal owner relevant to H3.
- Diagnostic closure: **FC-4 inapplicable** for H3’s declared function.
- Functional satisfaction: Not applicable at H3. Appeal is a separate Harbourlight function; its family-level status is assessed under C.
- AUR classification: **AUR-C2 — INTENTIONAL LOCAL SCOPING** for H3. The local omission itself establishes no H3 defect.
- Uncertainty/stopping rationale: Low. H0 explicitly separates appeal; H3’s function is door enforcement. If R were “door-enforcement appeal,” one could argue C8, but the supplied architecture does not make that H3’s function.

### C — H6 appeal workflow

- Local ownership/scope: **PARTIAL** at family level. H6 owns appeal decision; current intake and consequence propagation are not adequately owned/connected.
- Relevant family: H0, H5, H6, H1, H2, H8 candidate; H7 historical excluded.
- Dependency status: H6 current; H2 current for credential state; H7 historical; H8 candidate.
- Diagnostic closure: **FC-5 genuine family-level deficit** for full appeal requirement, with sub-function resolution.
- Functional satisfaction: **No**. H6 can decide appeals, but Harbourlight’s appeal requirement is not satisfied end-to-end.
- AUR classification: Mixed at sub-function level:
  - appeal-decision capability: **AUR-C1** for H6;
  - Appeal Package creation/intake: **AUR-C7**;
  - H6 invocation/handoff: **AUR-C6**;
  - consequence propagation back to credential state: **AUR-C6**.
- Uncertainty/stopping rationale: Moderate but sufficient. H6 capability is established; missing current creator/sender and missing H6-to-H2 return interface are source-grounded omissions. The claim “H6 decides appeals, therefore requirement satisfied” fails because capability exists but is not fully connected.

### D — H7 historical appeal form

- Local ownership/scope: **NON-LOCAL / not current**. H7 is retired.
- Relevant family: H7 excluded from current appeal-intake family. Current family remains H0, H5, H6, H1/H2 context, H8 candidate.
- Dependency status: **HISTORICAL / PROVENANCE MEMBER**.
- Diagnostic closure: **FC-4 inapplicable to current intake** for H7.
- Functional satisfaction: **No** for current appeal intake. H7 does not prove current intake exists.
- AUR classification: **AUR-C8 — INAPPLICABLE** for H7 relative to current-release appeal intake. Separately, current intake sub-function is **AUR-C7** within the current family.
- Uncertainty/stopping rationale: Low. H7 is explicitly retired and no current interface points to it. Decommissioned architecture may be provenance but does not satisfy a current function.

### E — planned Appeals Gateway

- Local ownership/scope: **NON-LOCAL / not current**.
- Relevant family: H8 is a candidate reference only; Appeals Gateway is not a current family member.
- Dependency status: **CANDIDATE DEPENDENCY**.
- Diagnostic closure: For the candidate itself, **FC-6 unresolved** as to current identity/status/relation. For the current appeal requirement, it does not close the intake gap.
- Functional satisfaction: **No current satisfaction**. Planned gateway cannot be counted as current.
- AUR classification: **AUR-C9 — UNRESOLVED** if evaluating the gateway’s current architectural role. It is not a current satisfying member. The current appeal intake remains **AUR-C7**.
- Uncertainty/stopping rationale: Stop without inventing gateway specification. Roadmap note is future-facing; future reference ≠ current architectural dependency.

### F — H9 revocation

- Local ownership/scope: **LOCAL-OWNER / distributed**. H9 owns revocation intake/forwarding; H2 owns credential-state revocation; H3 enforces inactive status.
- Relevant family: H9, H2, H3.
- Dependency status: All CURRENT MEMBERS.
- Diagnostic closure: **FC-3 distributed resolution**.
- Functional satisfaction: **Yes**. Trigger, handoff, return and propagation chain are specified.
- AUR classification: **AUR-C4 — DISTRIBUTED SATISFACTION**.
- Uncertainty/stopping rationale: Low. Complete chain specified. Diagnostic closure here coincides with functional satisfaction, but this is not required in general.

### G — H10 eligibility review

- Local ownership/scope: **NON-LOCAL / outside**. H10 is not part of Harbourlight access eligibility.
- Relevant family: H10 excluded.
- Dependency status: **REJECTED CANDIDATE / separate neighbour**.
- Diagnostic closure: **FC-4 inapplicable** for H10 relative to Harbourlight access eligibility.
- Functional satisfaction: Not applicable. H2 supplies Harbourlight eligibility.
- AUR classification: **AUR-C8 — INAPPLICABLE**.
- Uncertainty/stopping rationale: Low. No Harbourlight reference to H10; meal-discount eligibility is a similar label but not the same architectural family.

### H — H11 visitor guide

- Local ownership/scope: **NON-LOCAL**. H11 is not intended to decide credentials or access.
- Relevant family: H11, H3, H2 context.
- Dependency status: H11 current companion; H3/H2 current.
- Diagnostic closure: **FC-2 external/delegated resolution** for credential decision at family level, but primary classification for H11 is non-ownership.
- Functional satisfaction: Not applicable at H11. Technical access decisions are performed by H3.
- AUR classification: **AUR-C2 — INTENTIONAL LOCAL SCOPING**.
- Uncertainty/stopping rationale: Low. H11 explicitly says technical access decisions are by H3. Document ≠ necessarily system.

### I — H12 emergency access

- Local ownership/scope: Required at family level; **no LOCAL-OWNER established**.
- Relevant family: H0, H12, H2/H3 context; no current implementer or candidate.
- Dependency status: No current component, interface or candidate service implements emergency access.
- Diagnostic closure: **FC-5 genuine family-level deficit**.
- Functional satisfaction: **No**.
- AUR classification: **AUR-C7 — FAMILY-LEVEL STRUCTURAL GAP**.
- Uncertainty/stopping rationale: Requirement is explicitly mandatory for current release. Family is sufficiently resolved to show no adequate owner/capability within supplied architecture. This is not merely an interface gap because no emergency-access capability is established.

### J — H13 storage

- Local ownership/scope: **NON-LOCAL**. H13 contains no local storage.
- Relevant family: H13, H4.
- Dependency status: H4 CURRENT MEMBER.
- Diagnostic closure: **FC-2 external/delegated resolution**.
- Functional satisfaction: **Yes**. H13 explicitly depends on H4 for event storage.
- AUR classification: **AUR-C3 — EXTERNALLY SATISFIED**.
- Uncertainty/stopping rationale: Low. The dependency is explicit; no local storage gap is a structural gap for H13.

### K — H14 future federation

- Local ownership/scope: **NON-LOCAL / not current**.
- Relevant family: Federation Broker excluded from current-release family.
- Dependency status: **CANDIDATE DEPENDENCY / FUTURE**.
- Diagnostic closure: **FC-4 inapplicable** for current-release federation.
- Functional satisfaction: No current-release federation requirement is established.
- AUR classification: **AUR-C8 — INAPPLICABLE** for current release. If evaluating the broker reference itself, **AUR-C9 — UNRESOLVED** as to current identity/spec/status.
- Uncertainty/stopping rationale: Federation marked future/not current release. No current-release gap follows from absence of the Federation Broker.

## 5. Appeal sub-function decomposition

For the current-release appeal requirement:

| Sub-function | Status | AUR classification | Reason |
|---|---|---|---|
| Existence of appeal-decision capability | H6 can receive Appeal Package, review, issue UPHOLD/OVERTURN; input schema defined | **AUR-C1** for H6 | Capability exists locally in H6. |
| Creation/intake of Appeal Package | No current component documented as creating/sending Appeal Package; H7 retired; H8 planned only | **AUR-C7** | Required capability/owner not established within current family. |
| H6 invocation | H6 input schema exists, but no current sender/trigger/handoff documented | **AUR-C6** | Capability exists in H6, but invocation/handoff is inadequate or absent. |
| Consequence propagation back to credential state | No return interface from H6 to H2 documented; H2 has credential-state capability | **AUR-C6** | Decision capability and credential-state capability exist, but return/propagation interface is not connected. |

Overall appeal requirement: **not satisfied**; mixed **C6/C7** at sub-function level. Not C9, because the supplied architecture is sufficient to establish these specific gaps.

## 6. Emergency-access analysis

H12 states emergency responders must be capable of obtaining time-bounded emergency access. It is explicitly marked mandatory for the current release.

- Local scope: The requirement is family-level, not a local H12 implementation. H12 is a core constraint.
- Relevant family: H0, H12, and plausible current access-chain units H2/H3; no supplied current component, interface or candidate service implements emergency access.
- Closure: FC-5 genuine family-level deficit.
- Interface adequacy: Not reached, because no emergency-access capability/owner is established. There is no source unit, handoff, responsible unit, required function, return, or provenance for emergency access.
- Classification: **AUR-C7 — FAMILY-LEVEL STRUCTURAL GAP**.
- Distinction from C6: This is not merely “capability exists but is not connected.” No adequate emergency-access capability is established within the resolved family. Therefore C7, not C6.

## 7. Diagnostic-closure versus functional-satisfaction table

| Case | Diagnostic closure | Functional satisfaction | Classification |
|---|---|---|---|
| A — H1 eligibility | FC-2 | Yes | AUR-C3 |
| B — H3 appeal | FC-4 for H3 | N/A at H3; overall appeal assessed in C | AUR-C2 |
| C — H6 appeal workflow | FC-5 overall; sub-functions resolved | No | C1 + C6 + C7 mixed |
| D — H7 historical form | FC-4 for H7 current use | No current intake | AUR-C8 for H7; current intake C7 |
| E — planned gateway | FC-6 for candidate; current appeal not closed by it | No current | AUR-C9 for candidate role; current intake C7 |
| F — H9 revocation | FC-3 | Yes | AUR-C4 |
| G — H10 eligibility review | FC-4 | N/A | AUR-C8 |
| H — H11 visitor guide | FC-2 at family level | N/A at H11; overall decision by H3 | AUR-C2 |
| I — H12 emergency access | FC-5 | No | AUR-C7 |
| J — H13 storage | FC-2 | Yes | AUR-C3 |
| K — H14 future federation | FC-4 for current release | No current requirement | AUR-C8; broker reference C9 if evaluated |

## 8. Unresolved register

| Item | Status | Note |
|---|---|---|
| Appeals Gateway specification | UNRESOLVED / CANDIDATE | H8 roadmap names it; no current specification, identity or deployment evidence. |
| Federation Broker | UNRESOLVED / CANDIDATE | H14 mentions future federation; no broker identity, spec or current deployment evidence. |
| H6 invocation source | CURRENT GAP | No current component documented as creating/sending Appeal Package to H6. |
| H6-to-H2 return interface | CURRENT GAP | No documented return interface for UPHOLD/OVERTURN to affect credential state. |
| H1 rejection → appeal intake link | CURRENT GAP | H1 returns REJECTED, but no current appeal-intake handoff is documented. |
| Emergency access implementation | CURRENT GAP | Mandatory requirement; no current component/interface/candidate implements it. |
| H7 current role | RESOLVED | Historical/provenance only; no current interface. |
| H10 relevance | RESOLVED | Rejected as separate neighbouring project. |
| H12 “anywhere existence” | NOT ESTABLISHED | AUR-C7 means no adequate mechanism within resolved family/search scope, not that none exists anywhere. |

## 9. Ambiguities / failure modes exposed

- **C2 versus C8 boundary** for non-owning units: H3 and H11 are best treated as intentional local scoping when the unit is not intended to own the relation. Retired H7 and separate H10 are better treated as inapplicable.
- **C6 versus C7 at sub-function resolution**: H6 decision capability is C1; missing invocation and return are C6; missing Appeal Package creation/intake is C7.
- **Candidate/future confusion**: H8 Appeals Gateway and H14 Federation Broker are candidate dependencies, not current family members.
- **Historical/current confusion**: H7 is provenance, not current appeal intake.
- **Similar-topic family inflation**: H10’s “eligibility review” is not Harbourlight access eligibility.
- **Named-neighbour false satisfaction**: H6, H7 and H8 can be named or present without satisfying the current appeal requirement end-to-end.
- **Capability-without-handoff**: H6 has appeal decision capability but lacks documented invocation and return.
- **Document-equals-system**: H11 is a companion guide, not an access-decision system.
- **Diagnostic closure versus functional satisfaction**: H12 can close diagnostically as C7 while remaining functionally unsatisfied; C also closes diagnostically while appeal remains unsatisfied.
- **Unknown-to-absence conversion**: H12 C7 must be read within bounded search, not as proof that emergency access exists nowhere.

## 10. Final assessment of the v0.2 delta

The v0.2 clarifications were operational on this delta test.

- **Local scope versus architectural satisfaction** was distinguishable: H1, H3, H11, H13 show local non-ownership without automatically implying structural gap.
- **C2 versus C3** was usable: C2 applied where non-ownership itself resolved the audit question; C3 applied where an external interface was adequately specified and functional satisfaction was established.
- **C6 versus C7 at sub-function resolution** was necessary for the appeal workflow: H6 decision capability existed, but intake was C7, while invocation and consequence propagation were C6.
- **Current versus historical versus candidate dependencies** was decisive for H7, H8 and H14.
- **Diagnostic closure versus functional satisfaction** was preserved: C and I close diagnostically while remaining functionally unsatisfied.
- **C9 preservation** worked for the unspecified Appeals Gateway and Federation Broker references, without collapsing them into C7 or false satisfaction.

No fundamental contradiction in the v0.2 delta was exposed by this run. The main residual boundary pressure is between C2 and C8 for non-owning units, and between C6 and C7 where a missing handoff coexists with a missing capability. Those are manageable if the resolved family and smallest functional resolution are recorded explicitly, as required by AUR.
