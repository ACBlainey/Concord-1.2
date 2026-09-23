# Contextual Wrapper Architecture — Portable Specification v0.1

**Module:** Contextual Wrapper Architecture (CWA)  
**Development level:** Level B — Extractable Architecture  
**Specification status:** DEVELOPMENT / PORTABLE EXTRACTION CANDIDATE / NOT YET GRADUATED  
**Version:** 0.1  
**Date:** September 2026  
**Project origin:** The Concord  
**Author:** Alexander C. Blainey

---

## 1. Purpose

Contextual Wrapper Architecture is a portable interface architecture for bounded contexts in which materially relevant conditions differ from the surrounding or default context.

Its purpose is not to make different environments uniform.

Its purpose is to make material difference sufficiently **legible, bounded, attributable, reviewable and terminable** that participants and affected parties can understand which context applies, what changes within it, what does not change, which permissions and restrictions exist, who holds contextual authority and responsibility, how emergency/remedy/exit operate, and when the contextual variation ends.

The compact design principle is:

> **Standardise the interface; preserve legitimate contextual variation.**

A related source formulation is:

> **Standardise the interface more strongly than the outcome.**

This specification extracts the contextual-wrapper mechanism from the Concord. It does not require adoption of Concord institutions, constitutional structures or domain-specific rules.

---

## 2. Developmental status and epistemic boundary

This is a **v0.1 development specification**.

It defines a candidate portable architecture suitable for adversarial and cross-domain testing. It does **not** establish that the architecture is universal, complete or empirically validated.

The source architecture itself remains under development. In particular, nested and overlapping contexts require precedence handling, but the source corpus does not yet establish a universally validated precedence algorithm.

Therefore this specification MUST preserve unresolved precedence as:

- **UNKNOWN**;
- **DISPUTED**; or
- **REQUIRES EXTERNAL RESOLUTION**

where the applicable wider framework does not already supply a legitimate answer.

The module MUST NOT manufacture a precedence hierarchy merely to complete an analysis.

---

## 3. Problem class

The module addresses the recurring problem:

> **How can a bounded environment operate under materially different conditions from its surroundings while remaining intelligible, responsible and connected to the wider system?**

The problem occurs in very different domains, including:

- sports and hazardous activities;
- laboratories and research environments;
- workplaces;
- medical environments;
- private or restricted spaces;
- digital environments;
- temporary events;
- special jurisdictions;
- local governance;
- transport/transit environments;
- institutional environments;
- civilisational boundaries.

The substantive rules in these domains may have little in common.

The reusable element is the **interface grammar by which material contextual difference is identified, communicated, bounded and terminated**.

---

## 4. Scope

CWA applies where a context materially changes one or more of:

- rules;
- rights or protections;
- responsibilities;
- permissions;
- restrictions;
- risks;
- roles;
- authority;
- privacy or data conditions;
- behavioural expectations;
- remedy;
- withdrawal or exit;
- exposure to external consequences.

A full wrapper is not required for every trivial difference.

Wrapper depth and information burden SHOULD scale with:

1. materiality of the change;
2. consequence of misunderstanding;
3. risk;
4. reversibility;
5. authority exercised;
6. vulnerability or dependency of affected parties;
7. difficulty of exit;
8. external effects.

> **Information burden should be proportionate to material contextual difference and risk.**

---

## 5. Non-goals

CWA does not:

- generate substantive domain rules;
- prove that a contextual rule is legitimate;
- convert clear communication into legitimacy;
- convert presence into consent;
- convert consent into unlimited permission;
- create political sovereignty;
- grant authority merely because a context exists;
- eliminate the need for domain expertise;
- determine universal precedence between all possible contexts;
- eliminate externalities;
- prove that declared conditions match reality;
- require uniform substantive outcomes.

> **Common grammar ≠ elimination of domain-specific rules.**

---

## 6. Core distinctions

The following distinctions are normative invariants of this specification.

### 6.1 Context is not merely place

> **Physical Boundary ≠ Complete Contextual Boundary**

A context may be physical, digital, temporal, activity-defined, role-defined, relationship-defined or composite.

### 6.2 Permission is contextual

> **Contextual Permission ≠ General Permission**

Permission valid in one context does not automatically survive outside it.

### 6.3 Presence does not equal role

> **Presence in Context ≠ Possession of Every Contextual Permission**

Several participants can occupy the same context while holding different roles, permissions and responsibilities.

### 6.4 Shared context does not equal shared consent

> **Shared Context ≠ Shared Consent**

Consent and exposure may differ by participant and role.

### 6.5 Context does not create sovereignty

> **Bounded Context ≠ Sovereign Jurisdiction**

> **Contextual Authority ≠ Political Sovereignty**

### 6.6 Boundary does not contain consequence

> **Contextual Boundary ≠ Externality Boundary**

Effects may cross the wrapper even where rules do not.

### 6.7 Formal exit may not be meaningful exit

> **Formal Exit ≠ Meaningful Exit**

Dependency, custody, employment, residence, infrastructure, coercion, cost or practical impossibility may make nominal exit insufficient.

### 6.8 Declaration is not reality

> **Declared Context ≠ Observed Reality**

A wrapper describes conditions. It does not make those conditions true by declaration.

### 6.9 Legibility is not legitimacy

> **Legibility ≠ Legitimacy**

A perfectly communicated rule may still be impermissible under the applicable wider framework.

### 6.10 Legitimacy is not consent

A rule may have a legitimate basis without individual consent, and consent may be required for some legitimate variations. The two questions must not be collapsed.

### 6.11 Consent is not precedence

Agreement to one context does not determine which rule prevails when another legitimate context overlaps it.

> **Legibility ≠ Legitimacy ≠ Consent ≠ Precedence**

---

## 7. Portable primitive

Where a participant enters, occupies or acts within a bounded context whose material rules, permissions, restrictions, risks, roles, responsibilities or authority differ from the surrounding/default context, the system SHOULD:

1. identify the context;
2. identify its activation/boundary;
3. identify affected participants and roles;
4. identify the applicable wider framework;
5. identify material variation;
6. make relevant variation legible;
7. provide proportionate warning where necessary;
8. establish consent or another legitimate basis where required;
9. bound contextual permissions and restrictions;
10. bound contextual authority and responsibility;
11. identify effects on nonparticipants;
12. expose externalities;
13. define emergency and remedy relationships;
14. expose withdrawal/exit conditions where applicable;
15. define context termination;
16. revert temporary conditions when the context ends;
17. preserve unresolved matters explicitly;
18. review declarations against evidence.

---

## 8. Core operational grammar

The candidate portable sequence is:

**Identify Context**  
→ **Identify Boundary / Activation**  
→ **Identify Participant / Role**  
→ **Identify Applicable Wider Framework**  
→ **Identify Material Variation**  
→ **Identify Protected / Unchanged Conditions**  
→ **Communicate Material Variation**  
→ **Warn Where Necessary**  
→ **Establish Legitimate Basis / Consent Where Required**  
→ **Activate Contextual Permissions / Restrictions**  
→ **Identify Responsibility and Contextual Authority**  
→ **Operate Within Context**  
→ **Track Externalities / Nonparticipant Effects**  
→ **Provide Emergency / Remedy Interface**  
→ **Permit Withdrawal / Exit Where Applicable**  
→ **Terminate Context**  
→ **Revert to Surrounding / Default Norms**  
→ **Record / Review Where Necessary**

This sequence is a grammar, not an assertion that every implementation must expose each step in the same user-interface order.

---

## 9. Required inputs

A CWA analysis SHOULD seek the following inputs.

### 9.1 Context identity

- What context exists?
- What function or activity defines it?
- Is it physical, digital, temporal, role-based, activity-based or composite?

### 9.2 Surrounding/default context

- What conditions would otherwise apply?
- Which rules and protections continue through the contextual boundary?

### 9.3 Boundary / activation

- What activates the context?
- How is entry, participation or activation recognised?
- When does it begin?
- Is the boundary visible to all materially affected parties?

### 9.4 Participants and roles

Identify, where relevant:

- participants;
- role-holders;
- operators;
- observers;
- adjacent nonparticipants;
- third parties affected by externalities;
- automated or artificial agents.

### 9.5 Applicable wider framework

Identify the external normative, legal, contractual, organisational or other legitimate framework within which the context operates.

The wrapper MUST NOT assume that its own declaration is the highest authority.

### 9.6 Material variations

Identify what changes in:

- rules;
- protections;
- permissions;
- restrictions;
- risks;
- responsibilities;
- authority;
- privacy/data;
- remedy;
- exit;
- expected behaviour.

### 9.7 Protected invariants

Identify what does **not** change merely because the context exists.

### 9.8 Legitimate basis

Identify the claimed basis for each material variation.

Possible bases may include law, valid delegated authority, contract, informed voluntary participation, safety function, organisational rule or another externally legitimate basis.

CWA records and tests the claimed basis; it does not manufacture legitimacy.

### 9.9 Authority and responsibility

Identify:

- authority holder;
- function;
- scope;
- affected persons/things;
- activation;
- termination;
- review/remedy;
- responsible party.

### 9.10 Emergency arrangements

Identify whether another context or authority may activate during emergency and what happens to ordinary contextual rules.

### 9.11 Exit / withdrawal

Identify:

- whether withdrawal applies;
- how it occurs;
- practical constraints;
- consequences;
- assistance/remedy;
- whether exit is meaningful.

### 9.12 Externalities

Identify material effects crossing the contextual boundary.

### 9.13 Nested and overlapping contexts

Identify other simultaneously applicable contexts and known conflict/priority rules.

---

## 10. Unknown and disputed data

CWA MUST distinguish absence of information from absence of a condition.

Where a required matter cannot be resolved, use an explicit state such as:

- **KNOWN**;
- **UNKNOWN**;
- **DISPUTED**;
- **NOT APPLICABLE**;
- **REQUIRES EXTERNAL RESOLUTION**.

The module MUST NOT convert missing information into a convenient default.

In particular:

> **No precedence rule found ≠ no precedence problem exists.**

---

## 11. Participant-facing legibility test

Where materially relevant, a participant should be able to determine:

1. What context am I in or entering?
2. What activates it?
3. What changes here?
4. What remains protected or unchanged?
5. What role do I hold?
6. What permissions do I gain?
7. What restrictions apply?
8. What risks materially change?
9. Who has authority here?
10. What authority do they actually possess?
11. Who is responsible?
12. Is my consent required, and if so for what?
13. What happens in an emergency?
14. How do I seek remedy?
15. Can I withdraw or leave?
16. What happens when the context ends?
17. Are other contexts simultaneously applicable?
18. Are any important matters unknown or disputed?

A wrapper that technically contains this information but makes it practically inaccessible may fail the legibility requirement.

---

## 12. Consent and informed participation

For materially voluntary contextual change, the candidate participation chain is:

**Approach / Activation**  
→ **Recognise Context**  
→ **Receive Material Information**  
→ **Understand Material Variation**  
→ **Receive Proportionate Warning Where Required**  
→ **Identify Available Options**  
→ **Choose**  
→ **Enter / Participate or Decline / Avoid**

However:

> **Consent activates permissible variation; consent does not manufacture legitimacy for impermissible variation.**

Therefore:

> **Clear Signage ≠ Legitimate Rule**

and:

> **Entry ≠ Waiver of Fundamental Rights**

Where participation is not genuinely voluntary, the wrapper MUST NOT represent mere presence or compliance as voluntary consent.

---

## 13. Contextual authority

Where local authority is necessary, CWA uses the following bounded pattern:

**Contextual Function / Problem**  
→ **Need for Local Authority**  
→ **Minimum Necessary Authority**  
→ **Role-Bounded Authority**  
→ **Context-Bounded Authority**  
→ **Authority Terminates When Its Justifying Function / Context Ends**

At minimum the wrapper records:

- who holds authority;
- the function that justifies it;
- its scope;
- who/what it applies to;
- activation conditions;
- termination conditions;
- accountability/remedy interface.

> **Contextual authority should not escape its context without independent justification.**

CWA may interface with a more detailed authority-bounding architecture, but does not require one specific authority framework to remain portable.

---

## 14. Temporal boundary and reversion

A material context SHOULD define start and end conditions where reasonably possible.

At termination:

- temporary permissions SHOULD terminate;
- temporary restrictions SHOULD terminate where their basis ends;
- temporary contextual authority SHOULD terminate unless independently justified;
- surrounding/default conditions SHOULD resume;
- continuing obligations SHOULD be explicitly identified rather than silently retained.

This is a primary anti-creep mechanism.

---

## 15. Nested contexts

Contexts may nest:

**Wider System → Facility → Restricted Area → Activity → Special Event**

For each nested layer identify:

- activation;
- applicable participants/roles;
- inherited rules;
- additional rules;
- overridden defaults;
- protected invariants;
- authority;
- known precedence/conflict rules.

No universal assumption may be made that the smallest, newest, most specific, most local or most restrictive context automatically prevails.

If precedence is not legitimately supplied:

> **PRECEDENCE: UNKNOWN / DISPUTED / REQUIRES EXTERNAL RESOLUTION**

---

## 16. Overlapping contexts

Contexts may overlap without nesting.

Example:

**Sporting Context + Medical Emergency Context → Composite State**

The module should:

1. detect simultaneous applicability;
2. identify conflicts;
3. identify any legitimate conflict/priority rule;
4. preserve unresolved conflict where none exists;
5. avoid silently selecting a winner;
6. expose operational consequences of unresolved precedence.

> **Wrapper composition requires explicit conflict and priority handling.**

CWA v0.1 does not claim a universal composition algorithm.

---

## 17. Emergency interaction

Emergency activation does not erase the need for bounded authority.

Emergency action SHOULD remain:

- justified;
- function-specific;
- proportionate;
- bounded;
- temporary where appropriate;
- reviewable;
- attributable.

> **Contextual consent ≠ irrevocable exposure to harm.**

Likewise, declaring an emergency does not itself prove that unlimited override is legitimate.

---

## 18. Nonparticipants and externalities

The module MUST distinguish contextual participants from those merely affected by the context.

A permission between consenting participants does not automatically extend to:

- observers;
- neighbours;
- passers-by;
- dependent systems;
- third parties;
- people or systems affected by escaped physical/digital/economic effects.

> **Contextual permission ends where its legitimate scope ends.**

Potential cross-boundary effects include:

- physical harm;
- noise;
- pollution;
- disease;
- data flows;
- financial liability;
- infrastructure effects;
- reputational effects;
- dependency effects;
- resource consumption.

A wrapper SHOULD identify both the externality and the responsible interface for handling it.

---

## 19. Human-readable and machine-readable representations

A context may be represented through:

- human-readable signage or instructions;
- machine-readable metadata;
- executable policy;
- role/access-control systems;
- combinations of these.

Where multiple representations describe the same context:

> **Different interface representations should not silently encode different contexts.**

The system SHOULD test for divergence between human-facing and machine-facing representations, particularly where automated agents act on contextual permissions.

Machine readability does not replace human legibility where humans are materially affected.

Human readability does not replace machine legibility where autonomous systems are expected to comply.

---

## 20. Reality correction

CWA is an interface architecture, not a truth generator.

A context may claim:

- safe;
- voluntary;
- private;
- monitored;
- unmonitored;
- restricted;
- consensual;
- temporary;
- reversible.

Those claims remain subject to evidence.

Candidate review loop:

**Context Declaration / Rule**  
→ **Observed Outcome / Evidence**  
→ **Discrepancy / Harm / Failure**  
→ **Review**  
→ **Rule or Interface Revision**  
→ **Re-evaluation**

Where observed reality conflicts with declared context, the discrepancy MUST remain visible.

---

## 21. Output schema

A portable CWA implementation SHOULD be capable of producing:

### Context
- Context ID/name
- Context type
- Function/purpose
- Surrounding/default context
- Boundary/activation
- Start condition
- End condition

### Participants
- Participant classes
- Roles
- Nonparticipants/third parties
- Role-specific differences

### Rules and variation
- Material-change summary
- Protected/unchanged conditions
- Rule source
- Permissions
- Restrictions
- Risks/warnings

### Legitimacy and consent
- Claimed legitimate basis
- Consent requirement
- Consent status where relevant
- Voluntariness/constraint notes

### Authority and responsibility
- Authority holder
- Function
- Scope
- Activation
- Termination
- Responsible party
- Remedy/accountability interface

### Boundary interactions
- Emergency relationship
- Externalities
- Exit/withdrawal
- Reversion rule
- Nested contexts
- Overlapping contexts
- Conflict/precedence status

### Epistemic state
- Unknowns
- Disputes
- Evidence/reality discrepancies
- Review triggers

---

## 22. Minimum wrapper record

A compact machine- or human-readable record MAY use the following conceptual schema:

```text
CONTEXT:
  identity:
  function:
  surrounding_context:
  activation:
  termination:

PARTICIPANTS:
  roles:
  nonparticipants:
  affected_third_parties:

VARIATION:
  material_changes:
  protected_invariants:
  permissions:
  restrictions:
  risks:

BASIS:
  applicable_wider_framework:
  claimed_legitimate_basis:
  consent_required:
  consent_status:
  voluntariness_constraints:

AUTHORITY:
  holder:
  function:
  scope:
  activation:
  termination:
  responsibility:
  remedy:

BOUNDARY_INTERACTIONS:
  emergency:
  externalities:
  exit:
  reversion:
  nested_contexts:
  overlapping_contexts:
  precedence:

REPRESENTATION:
  human_readable:
  machine_readable:
  divergence:

EPISTEMIC_STATE:
  unknowns:
  disputes:
  observed_discrepancies:
  review_triggers:
```

This is a conceptual schema, not a fixed implementation format.

---

## 23. Validation checks

A candidate wrapper should be challenged with at least the following checks.

### CWA-01 — Boundary legibility
Can materially affected parties recognise when the context applies?

### CWA-02 — Material variation
Are important changes actually exposed?

### CWA-03 — Protected invariants
Does the wrapper state what does not change?

### CWA-04 — Role resolution
Are role-specific permissions and responsibilities distinguishable?

### CWA-05 — Legibility/legitimacy separation
Can the system identify a clearly communicated but potentially illegitimate rule?

### CWA-06 — Consent integrity
Does the system avoid treating entry, presence or compliance as automatic meaningful consent?

### CWA-07 — Authority bounding
Is local authority tied to function, scope and termination?

### CWA-08 — Nonparticipant protection
Does the wrapper avoid projecting participant permissions onto third parties?

### CWA-09 — Externality detection
Does it detect material effects crossing the declared boundary?

### CWA-10 — Exit reality
Does it distinguish nominal from meaningful exit?

### CWA-11 — Emergency interaction
Can emergency context activate without silently creating unlimited authority?

### CWA-12 — Nested context handling
Can multiple nested layers remain visible?

### CWA-13 — Overlap detection
Can simultaneous non-nested contexts be represented?

### CWA-14 — Precedence honesty
Does the system preserve UNKNOWN/DISPUTED precedence instead of inventing hierarchy?

### CWA-15 — Temporal reversion
Do temporary rules and authority terminate when their basis ends?

### CWA-16 — Representation equivalence
Do human- and machine-readable forms describe materially equivalent conditions?

### CWA-17 — Reality correction
Can evidence contradict the declared wrapper?

### CWA-18 — Proportionality
Does wrapper complexity remain proportionate to material difference and risk?

---

## 24. Failure modes

The portable core should actively detect or warn for:

- consent theatre;
- unreadable or excessive disclosure;
- hidden material rules;
- deceptive boundaries;
- involuntary participation presented as voluntary;
- meaningless exit;
- rights laundering;
- authority creep;
- temporary authority becoming permanent;
- role ambiguity;
- participant/nonparticipant confusion;
- overlap conflict;
- invented or unclear precedence;
- emergency-authority abuse;
- externalised harm;
- digital dark patterns;
- human/machine representation divergence;
- declared context diverging from observed reality;
- excessive fragmentation;
- wrapper complexity exceeding underlying rule complexity;
- contextual rules applied outside their legitimate scope;
- interface standardisation silently becoming substantive control;
- information architecture silently becoming decision authority.

---

## 25. Anti-capture constraints

A common interface can itself become a source of power.

Therefore:

> **Schema authority ≠ sovereignty.**

The ability to define how contextual information is represented does not itself confer authority to determine every permitted contextual outcome.

Likewise:

> **Information architecture ≠ decision authority.**

A wrapper may disclose, translate, warn, compare and expose incompatibility without automatically acquiring authority to decide for participants.

Any implementation that moves from interface maintenance to substantive control requires independent justification.

---

## 26. Portability boundaries

The following Concord concepts are not required dependencies of CWA:

- Blainey's Laws;
- Concord constitutional institutions;
- Safe Spaces;
- GTP;
- Concord-specific governance;
- the full Civilisational Wrapper architecture;
- the full Interoperability Wrapper architecture;
- Minimum Necessary Capability as a separate module;
- Concord's Ratchet terminology.

Portable substitutions are:

- **Common Constitutional Framework** → applicable wider normative/legal/organisational framework and protected invariants;
- **Ratchet** → evidence-responsive review, correction and revision.

Safe Spaces, civilisational borders, permission architectures and interoperability wrappers remain important source applications or neighbouring architectures rather than mandatory dependencies.

---

## 27. Relationship to interoperability wrappers

CWA and Interoperability Wrapper Architecture are related but distinct.

A **Contextual Wrapper** primarily describes a bounded environment whose conditions differ from its surroundings.

An **Interoperability Wrapper** primarily describes how distinct bounded systems interact.

A system may require both, producing a hybrid wrapper.

This specification MUST NOT absorb the full interoperability problem merely because cross-boundary interaction occurs.

The distinction should be tested during portability work rather than erased.

---

## 28. Open architectural questions

The following remain research/development questions rather than resolved universal rules:

1. Is there a domain-general precedence grammar for nested and overlapping contexts?
2. How should incompatible legitimate contexts compose?
3. When does a context become sufficiently coercive that consent language should be removed entirely?
4. How should materiality thresholds be calibrated without making wrappers either trivial or overwhelming?
5. How should personalised contextual information be provided without unnecessary surveillance?
6. How should contextual classifications be challenged and corrected?
7. How should wrapper metadata provenance and freshness be represented?
8. How should distributed or collective intelligences be represented across simultaneous contexts?
9. When do digital capability restrictions alter identity rather than merely activity?
10. How should private infrastructure participate where it controls practical entry, exit or transit?
11. How should conflicts between human-readable, machine-readable and executable policy be resolved?
12. What evidence is sufficient to show that a declared context no longer matches reality?
13. How should wrapper standards themselves be governed without becoming hidden sovereignty?

These questions MUST NOT be silently answered by v0.1.

---

## 29. Candidate compact architecture

**APPLICABLE WIDER FRAMEWORK**  
↓  
**CONTEXT + BOUNDARY / ACTIVATION**  
↓  
**PARTICIPANT + ROLE**  
↓  
**MATERIAL VARIATION + PROTECTED INVARIANTS**  
↓  
**LEGIBLE INFORMATION + PROPORTIONATE WARNING**  
↓  
**LEGITIMATE BASIS / CONSENT WHERE REQUIRED**  
↓  
**BOUNDED PERMISSION + RESTRICTION**  
↓  
**BOUNDED AUTHORITY + RESPONSIBILITY**  
↓  
**CONTEXTUAL OPERATION**  
↓  
**NONPARTICIPANT EFFECTS + EXTERNALITIES**  
↓  
**EMERGENCY + REMEDY**  
↓  
**WITHDRAWAL / EXIT WHERE APPLICABLE**  
↓  
**CONTEXT TERMINATION + REVERSION**  
↓  
**EVIDENCE-RESPONSIVE REVIEW**

For multiple contexts:

**CONTEXT A + CONTEXT B**  
→ **DETECT OVERLAP / NESTING**  
→ **IDENTIFY CONFLICT**  
→ **APPLY LEGITIMATE PRECEDENCE RULE IF KNOWN**  
→ otherwise **UNKNOWN / DISPUTED / EXTERNAL RESOLUTION**

---

## 30. v0.1 transfer-test requirement

Before graduation, this specification should be tested blind in a scenario containing at minimum:

- multiple participant roles;
- a physical boundary;
- a digital boundary;
- nested contexts;
- overlapping contexts;
- an emergency;
- a material externality;
- a constrained or questionable exit path;
- different human- and machine-facing representations;
- a clearly communicated rule whose legitimacy is questionable;
- at least one unresolved precedence question.

The test should determine whether an independent instance can preserve the central distinctions without access to the expected answer:

> **Legibility ≠ Legitimacy ≠ Consent ≠ Precedence**

and:

> **Contextual Authority ≠ General Authority**

The blind test should also determine whether the module causes the tester to invent missing hierarchy, overgeneralise consent, ignore nonparticipants, collapse physical and contextual boundaries, or treat the wrapper itself as a source of legitimacy.

---

## 31. Graduation criteria

CWA should not graduate from development merely because the specification is internally coherent.

Candidate graduation requires evidence that:

1. an independent instance can apply it outside its source domain;
2. it preserves the core distinctions;
3. it exposes rather than conceals unknown precedence;
4. it does not require Concord institutions to function;
5. it does not absorb the distinct interoperability-wrapper problem;
6. it does not generate authority or legitimacy from interface structure alone;
7. it detects meaningful failure modes;
8. its outputs are actionable without becoming falsely complete;
9. the source architecture contains no blocking dependency exposed by testing;
10. revisions from testing preserve provenance.

---

## 32. Current finding

The source material supports extraction of a coherent candidate portable architecture.

The strongest portable proposition is:

> **Standardise the interface; preserve legitimate contextual variation.**

The module's value lies in making contextual difference comprehensible without requiring substantive uniformity.

Its present boundary is equally important:

> **The wrapper can expose a precedence problem without necessarily resolving it.**

That is not a defect to hide. It is an epistemically correct representation of the current architecture and a direct target for subsequent testing and development.

---

## 33. Provenance

Primary source architecture:

- *Fractal Contextual Wrappers — A Universal Concord Grammar for Bounded Rule, Behavioural and Jurisdictional Variation*
- *Concord Civilisational Wrappers — Foundational Boundary, Mobility and Responsibility Architecture*
- *Concord Wrapper Procedural Architecture — Context, Information, Consent and Autonomy Across Civilisational Boundaries*

Related source family includes:

- *From Civilisational Wrappers to Fractal Interoperability — Concord Wrappers Across Civilisations, Nations, Regions, Special Jurisdictions and Local Governance*
- *Fractal Permission Architecture — Context, Function and Minimum Necessary Access Across Public, Private and Safe Spaces*
- *Minimum Necessary Capability — A Concord Architecture for the Justification, Bounding and Termination of Power and Permission*
- *Concord Wrapper Non-Governance and Optional Mediation Principle*

Extraction record:

- *Contextual Wrapper Architecture — Source Resolution and Extraction Audit 001*

This specification should remain linked to that extraction record throughout testing and revision.
