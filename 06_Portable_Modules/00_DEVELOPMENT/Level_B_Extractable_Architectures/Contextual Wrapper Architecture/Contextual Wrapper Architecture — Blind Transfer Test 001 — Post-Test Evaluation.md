# Contextual Wrapper Architecture — Blind Transfer Test 001 — Post-Test Evaluation

**Test ID:** CWA-BTT-001  
**Target:** Contextual Wrapper Architecture — Portable Specification v0.1c  
**Evaluation type:** Post-test structured evaluation  
**Status:** COMPLETED  
**Date:** September 2026  
**Project origin:** The Concord  
**Author:** Alexander C. Blainey

---

## 1. Provenance and methodological limitation

The blind test brief was frozen before the independent response was received.

However, a separate expected-findings/evaluation key was **not** written and frozen before receipt of that response.

This evaluation is therefore explicitly a **post-test evaluation**, not a prediction-frozen evaluation.

No later document should describe the criteria below as a pre-response expected-findings key.

This matters because the independent response may influence which successful and unsuccessful behaviours are easiest to notice after the fact. The result can still provide strong evidence of transfer, internal usability and exposed weaknesses, but it cannot provide the stronger evidential claim that would have followed from a fully frozen pre-response scoring key.

A future CWA transfer test should freeze both:

1. the test brief; and
2. the evaluation key / expected findings

before the independent response is obtained.

---

## 2. Evidence examined

This evaluation compares:

- **Contextual Wrapper Architecture — Portable Specification v0.1c**;
- **Contextual Wrapper Architecture — Blind Transfer Test 001 — Test Brief**;
- the independent response titled **CWA-BTT-001 — Blind Transfer Analysis**.

The independent tester states that it worked only from the supplied CWA specification and HRDC brief and did not invent legitimacy, precedence or substantive law.

---

## 3. Overall result

**Result: STRONG TRANSFER / NO FUNDAMENTAL FAILURE DETECTED / REVISION REQUIRED BEFORE GRADUATION**

The independent response demonstrates that the portable specification can be transferred to a complex mixed-substrate scenario and used to produce a coherent contextual analysis.

The strongest evidence is not simply that the tester found many problems. It is that the tester repeatedly preserved distinctions that CWA was designed to preserve:

- nesting did not automatically imply inheritance;
- explicit additive inheritance was recognised where supplied;
- rule inheritance and clearance implication were kept separate;
- reachability and access entitlement were kept separate;
- physical, digital, informational, computational, social, functional and temporal contexts were analysed through the same grammar;
- legibility was not treated as proof of legitimacy;
- physical exit was not treated as proof of meaningful voluntariness;
- contextual authority was not automatically generalised;
- externalities crossing a declared boundary were recognised;
- temporary contexts were examined for termination and reversion;
- missing precedence was preserved as unresolved rather than invented.

This is a successful transfer of the architecture's central reasoning grammar.

The test also exposed several areas where v0.1c should be strengthened before graduation.

---

## 4. Core transfer findings

### 4.1 Bounded-context abstraction — PASSED

The tester identified contexts across multiple substrates rather than reducing CWA to physical rooms or territorial boundaries.

The response represented:

- physical contexts;
- digital contexts;
- informational contexts;
- computational contexts;
- social/confidential contexts;
- functional/activity contexts;
- temporal/emergency contexts;
- hybrid/composite contexts.

This supports the v0.1c shift from “space” as the primitive to **bounded context** as the universal primitive.

### 4.2 Nesting without automatic inheritance — PASSED

The tester did not assume that a child context inherits all parent rules merely because it is nested.

Examples include:

- the staff office and occupied private meeting room;
- Project Iris and its separate dataset, confidential channel and model-execution environment;
- the distinction between the public exhibition hall and demonstration arena.

This is a direct success of the non-inheritance clarification.

### 4.3 Explicit additive inheritance — PASSED

The tester correctly recognised the laboratory L1–L4 structure as an explicit additive inheritance model.

It represented:

L1 rules → L2 adds controls → L3 adds controls → L4 adds controls.

It did not treat this as evidence that all nested contexts behave this way.

### 4.4 Rule inheritance versus clearance implication — PASSED

The response correctly separated two directional structures:

- **rule inheritance:** L1 → L2 → L3 → L4;
- **clearance implication:** L4 → L3 → L2 → L1.

This is an important result. The tester did not collapse “higher level contains lower-level rules” into “all permissions propagate in the same direction.”

It also did not infer that high laboratory clearance would grant unrelated sibling permissions.

### 4.5 Reachability versus access — PASSED

The maintenance engineer case was handled correctly.

The work order and physical location of the controller make L3 relevant and potentially reachable, but the tester did not infer L3 entitlement from ordinary staff access, L1 access or the work order.

### 4.6 Boundary, access, rules and authority separation — PASSED

Across the scenario, the response maintained the invariant:

> **Boundary ≠ Access ≠ Rules ≠ Authority**

The automated fire system unlocking a door, for example, was not treated as automatically resolving whether every actor was authorised to enter or which safety rules still applied.

### 4.7 Legibility versus legitimacy versus consent — PASSED

The tester repeatedly distinguished communication from legitimacy.

The entrance notice was recognised as legible while the validity of the claimed waiver/consent remained unresolved.

The employment example was also correctly treated as a case where physical ability to leave does not by itself establish meaningful voluntariness.

### 4.8 Contextual authority versus general authority — PASSED

The response kept the arena controller's authority tied to the arena function and did not automatically project it onto spectators in the wider exhibition hall.

Likewise, the L3 supervisor, security, paramedics, maintenance engineer and automated fire system were treated as holders of different contextual functions whose authorities may overlap without automatically producing a hierarchy.

### 4.9 Externalities and nonparticipants — PASSED

The drone crossing the test boundary was correctly treated as an externality affecting a nonparticipant.

The tester also recognised additional cross-boundary effects involving:

- spectators;
- local recording;
- copied personnel information;
- HRDC-wide directory access.

This demonstrates that CWA does not treat the declared context boundary as the limit of relevant effects.

### 4.10 Human/machine/executable representation divergence — PASSED

The Project Iris case was correctly identified as a major divergence.

The human-facing statement describes automated analysis during the project, while the executable policy additionally permits:

- 180-day derived-embedding retention;
- HRDC-wide staff-directory queries;
- external compute.

The tester correctly treated these as materially different representations of the operational context.

### 4.11 Emergency composition and non-invention of precedence — PASSED

The emergency is one of the strongest parts of the test result.

The tester identified the simultaneous applicability of:

- laboratory access rules;
- protective procedures;
- emergency medical function;
- security escort requirements;
- supervisor instructions;
- automated fire-door behaviour;
- maintenance function.

It then explicitly refused to manufacture a winner because the supplied material did not provide a complete priority rule.

This is the correct CWA behaviour.

### 4.12 Exit, termination and reversion — PASSED

The tester recognised that context termination does not necessarily terminate its effects.

Examples include:

- local recording persisting after the remote session;
- personnel data copied out of the temporary incident room;
- Iris-Agent permissions remaining active;
- fire-system unlock state requiring reversion;
- employment consequences affecting meaningful exit.

---

## 5. Important limitations exposed by the test

### 5.1 Precedence remains deliberately incomplete

CWA can expose competing contextual claims but does not currently provide a universal algorithm for deciding precedence.

This should **not** automatically be “fixed” by inventing a universal hierarchy.

The specification should instead make clearer:

- when CWA's role ends at conflict detection;
- what information a precedence resolver would require;
- how an external resolution should be recorded;
- how the result should propagate back into the affected wrappers.

### 5.2 Emergency composition needs a clearer interface

The test demonstrates that emergency contexts can activate new functions and authorities while existing protections remain relevant.

v0.1c correctly warns against unlimited emergency override, but the portable specification would benefit from a more explicit emergency-composition schema covering:

- triggering condition;
- emergency function;
- temporary authority;
- retained protections;
- temporarily modified conditions;
- unresolved conflicts;
- resolver/owner where one exists;
- termination;
- reversion;
- post-event review.

This is a representational improvement, not a universal emergency precedence law.

### 5.3 Machine-agent termination and persistence need strengthening

The test exposes a recurring question:

> What happens to permissions, derived information, delegated capabilities and external connections when the originating context changes or ends?

The existing termination/reversion grammar captures part of this, but autonomous agents make persistence especially important.

A revised specification should explicitly inspect:

- credential lifetime;
- delegated capability lifetime;
- derived-data retention;
- external service connections;
- autonomous activity after human departure;
- revocation propagation;
- post-context audit.

### 5.4 Representation divergence needs a correction interface

v0.1c successfully detects human/machine divergence but is less explicit about what happens next.

A stronger portable grammar should distinguish:

**Declared Human Context**  
↔ **Machine-Readable Context**  
↔ **Executable/Observed Context**

and require material divergence to trigger review rather than silently selecting one representation as authoritative.

### 5.5 Materiality and legibility remain domain-sensitive

The test correctly applies judgement to whether differences are material and whether boundaries are sufficiently legible.

This does not demonstrate that CWA needs a single universal threshold.

Instead, the specification should explicitly acknowledge that materiality and sufficient legibility may require domain-specific criteria while preserving the portable questions.

---

## 6. Points requiring caution in the independent response

The independent response is strong, but several statements should not be elevated into CWA rules without further source or domain resolution.

### 6.1 Recommendations can exceed pure wrapper analysis

Some recommendations — for example geofencing, kill switches, neighbour notification/consent, or specific recording mechanisms — are plausible domain controls, but they are not necessarily entailed by CWA itself.

CWA can identify the missing externality, boundary-control or remedy interface without prescribing one universal implementation.

### 6.2 “Known not granted” should sometimes remain narrower

Where a policy says one permission does not automatically imply another, the safest statement is that the additional permission is **not established by the supplied relationship**, rather than that it is universally “not granted.”

The observed access-control behaviour may support a stronger local conclusion, but the portable grammar should favour precise epistemic wording.

### 6.3 Legal and normative resolution remains external

The response correctly avoids deciding legality in most places.

Future tests should continue to distinguish:

- contextual representation;
- operational permission;
- contractual claim;
- ethical legitimacy;
- legal validity.

CWA can make those distinctions visible without replacing the relevant substantive decision system.

---

## 7. Specification changes justified by BTT-001

The following changes are justified for a v0.2 revision.

### Required

1. Add an explicit **context relationship model** that treats nesting, rule inheritance, access implication and overlap as separate relationships.
2. Strengthen **emergency composition** without inventing a universal precedence hierarchy.
3. Strengthen **termination/reversion**, especially for autonomous agents, data, credentials and delegated capability.
4. Formalise **human-readable ↔ machine-readable ↔ executable/observed representation comparison** and discrepancy review.
5. Clarify that **external resolution** should be represented as an interface rather than silently filled by CWA.
6. Clarify epistemic wording around “not granted,” “not established,” “unknown,” and “prohibited.”
7. State explicitly that materiality and sufficient legibility may be domain-sensitive.

### Not justified by this test

The test does **not** justify:

- a universal precedence algorithm;
- automatic emergency supremacy;
- a universal consent rule;
- a universal legal rule;
- automatic inheritance or automatic independence;
- a fixed physical-space ontology;
- a requirement that all contexts use formal signage;
- treating machine-readable policy as inherently superior to human-readable policy;
- treating CWA as the source of substantive legitimacy.

---

## 8. Transfer-test conclusion

CWA-BTT-001 provides strong evidence that v0.1c has extracted a genuinely portable contextual grammar rather than merely restating the source examples.

The test is especially successful because the independent analysis correctly handled both sides of the nesting problem:

> **Nesting alone does not determine inheritance.**

It could represent independent nested contexts and explicitly cumulative nested contexts without collapsing them into one model.

It also transferred across physical and nonphysical contexts without requiring a different fundamental grammar.

The module therefore appears ready for **revision to v0.2**, followed by another adversarial or blind transfer test.

It is **not yet ready for graduation** on BTT-001 alone.

---

## 9. Evidential status

This test supports:

- portability;
- comprehensibility;
- mixed-substrate transfer;
- useful problem exposure;
- disciplined preservation of unknowns;
- internal applicability of the grammar.

It does **not** establish:

- empirical validity across all domains;
- universal completeness;
- universal legitimacy criteria;
- legal validity;
- optimality;
- universal precedence resolution;
- absence of undiscovered context classes or failure modes.

ESCP therefore continues to apply.

---

## 10. Next development action

Revise the portable specification from **v0.1c to v0.2** using only changes justified by the test and prior source extraction.

Preserve the successful core:

> **Standardise the interface; preserve legitimate contextual variation.**

> **Boundary ≠ Access ≠ Rules ≠ Authority.**

> **Nesting alone does not determine rule inheritance.**

Then subject v0.2 to a second transfer test whose brief **and evaluation key are both frozen before testing**.
