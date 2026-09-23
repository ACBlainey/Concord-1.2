# Fractal Permission Architecture — Portable Specification v0.1

**Version:** 0.1  
**Status:** DEVELOPMENT SPECIFICATION / SOURCE-EXTRACTED / NOT YET GRADUATED  
**Development level:** Level B — Extractable Architecture  
**Date:** 23 September 2026

## 1. Purpose

Fractal Permission Architecture (FPA) is a portable grammar for representing contextual permission without reducing permission to binary access, physical capability, ownership, role or a universal context-independent rule.

It asks:

> **Who may do what, where, why, when, under which conditions, by which legitimate basis, and until when?**

Its central problem is:

> **How can a system represent who may legitimately do what, where, why, when and under which conditions without collapsing permission into physical capability, binary access, ownership, role or a universal context-independent rule?**

## 2. Core principle

> **Represent permission as a bounded contextual relationship among participant, action, target/context, function, legitimate basis, conditions and time; grant no more permission than the legitimate basis requires; and terminate context-derived permission when that basis ends.**

Short form:

> **Who. What. Where. Why. When. Under what legitimate basis. No more than necessary.**

## 3. Non-functions

FPA does not by itself:
- decide whether every underlying rule is ethically or legally legitimate;
- create property rights, ownership, jurisdiction or authority;
- resolve every conflict between competing legitimate claims;
- define one culture's social conventions as universal;
- require formal permission negotiation for every ordinary interaction;
- turn technical capability into normative permission;
- define universal emergency powers;
- replace specialised legal, safeguarding, medical, employment, parental, security or regulatory systems.

> **Permission Representation ≠ Permission Justification**

## 4. Core separations

> **Spatial Classification ≠ Access Classification**

> **Permission to Enter ≠ Permission to Use**

> **Access ≠ Single Permission**

> **Physical Accessibility ≠ Normative Accessibility**

> **Contextual Permission ≠ General Permission**

> **Permission for One Function ≠ Permission for Unrelated Functions**

> **Parent-Space Permission ≠ Automatic Child-Space Permission**

> **Residence ≠ Universal Contextual Permission**

> **Shared Context ≠ Shared Consent**

> **Open Boundary ≠ Granted Permission**

> **Destination Permission ≠ Universal Route Permission**

> **Ownership ≠ Unlimited Contextual Sovereignty**

> **Past Permission ≠ Present Permission**

> **Machine-Readable Permission ≠ Machine-Determined Legitimacy**

## 5. Minimum Necessary Permission

The central operating mechanism is:

**Legitimate Function → Required Interaction → Required Access/Action → Minimum Necessary Permission → Function-Bounded Activity → Function Completion → Permission Termination**

> **Where a legitimate function requires access to a space, resource, participant or capability, the resulting permission should normally extend only as far as reasonably necessary to perform that function, remain subject to higher-order rights and applicable rules, and terminate when the function or other legitimate basis for the permission ends.**

This is **Minimum Necessary Permission (MNP)**.

MNP does not mean the narrowest technically possible permission regardless of usability. It means no broader permission than is reasonably necessary for the legitimate function in the actual context.

## 6. Permission claim

A conceptual permission record is:

**PermissionClaim = <Participant, Action, Target/Context, Function, Basis, RuleSource, Consent, Path, State, Conditions, Start, Expiry/Termination, DelegationScope, Provenance, Status>**

Fields may be omitted where genuinely irrelevant, but material uncertainty should remain explicit.

The record is extensible.

## 7. Minimum inputs

Where materially relevant, determine:
- participant/actor;
- proposed action;
- target space, resource, participant or context;
- function/purpose;
- claimed permission basis;
- rule source;
- consent state;
- applicable rules;
- current context/state;
- path or route;
- temporal scope;
- restrictions/conditions;
- revocation/termination conditions;
- delegation scope;
- known higher-order rights/constraints;
- provenance and uncertainty.

> **Unknown Permission Basis ≠ Permission**

But uncertainty also does not automatically prove prohibition.

## 8. Permission actions

“Access” should be decomposed where necessary.

Candidate actions include:
- approach;
- traverse;
- enter;
- remain;
- occupy;
- observe;
- interact;
- use;
- inspect;
- record;
- modify;
- remove;
- deliver;
- retrieve;
- supervise;
- exclude;
- authorise/delegate.

Different implementations may use different action vocabularies.

> **Permission to Perform Action A ≠ Permission to Perform Action B**

## 9. Permission basis and rule provenance

Candidate bases/sources include:
- explicit consent;
- contractual permission;
- role/function assignment;
- owner/steward rule;
- relationship permission;
- legal requirement or entitlement;
- cultural/social convention;
- contextual inference;
- emergency necessity;
- delegated permission;
- other independently defined legitimate basis.

Record the basis rather than treating the visible rule as self-justifying.

> **Rule Content ≠ Rule Source**

A declared rule may itself remain contestable under external ethical, legal or institutional architecture.

## 10. Explicit permission

Explicit permission should preserve scope.

“Come in” may authorise entry without authorising recording, inspection, removal, unrelated use or indefinite return.

Explicit permission should be interpreted according to the action, context, function, conditions and temporal scope actually granted.

## 11. Implied permission

Some systems rely on ordinary implied permission.

A candidate implied-permission claim is legitimate only where the surrounding context independently supports the inference—for example through established convention, ordinary function, prior relationship or another recognised rule source.

The source architecture proposes:

> **Where a function is ordinary, legitimate, reasonably expected and requires limited access to perform, a bounded contextual permission may be implied unless it has been explicitly restricted or conflicting rights and circumstances require otherwise.**

This is a hypothesis requiring domain, cultural and legal validation.

Therefore:

> **Implied Permission ≠ Universal Default**

> **Universal Permission Grammar ≠ Universal Permission Outcome**

An implementation should record the provenance of the implied rule or convention where consequential.

## 12. Path-specific permission

Permission to reach a destination does not necessarily authorise every possible route.

**PathPermission = <Origin, PermittedRoute/BoundarySequence, Destination, Function, Conditions, State>**

> **Destination Permission ≠ Universal Route Permission**

If the permitted route is unknown and route choice materially affects privacy, risk or rights, preserve the uncertainty or seek additional permission.

## 13. Nested contexts

Contexts may contain nested contexts.

Examples can include:
**Site → Building → Shared Area → Restricted Room → High-Privacy Subcontext**

Permission at a parent context does not automatically inherit into a child context.

> **Parent-Space Permission ≠ Automatic Child-Space Permission**

Nested contexts need not be separate jurisdictions. They are permission-relevant boundaries.

## 14. Contextual depth

Moving into a context with materially greater privacy, risk or restriction may require stronger or more specific permission.

> **Deeper Contextual Access May Require Additional Justification**

“Deeper” refers to permission-relevant context, not merely physical distance.

## 15. Relationship-specific permission

Different participants may legitimately possess different permissions for the same action and target because their relationships or responsibilities differ.

But:

> **Relationship ≠ Unlimited Permission**

A relationship-derived permission should retain scope, purpose, conditions and termination logic where material.

## 16. Role-specific permission

A role may establish a legitimate basis for some actions.

But:

> **Role ≠ Universal Access**

Role-derived permission should be connected to the function for which the role exists and bounded accordingly.

## 17. State-dependent permission

Permission may change when relevant state changes.

Candidate state variables include:
- occupied/unoccupied;
- open/closed;
- active/inactive;
- event active/concluded;
- ordinary/emergency;
- hazardous/safe;
- confidential session active/inactive;
- temporary restriction active/inactive;
- participant present/absent;
- system security state.

> **Same Target + Different Relevant State → Potentially Different Permission**

State should not be inferred merely because doing so would make access convenient.

## 18. Temporal permission

A permission may have:
- start time/event;
- end time/event;
- duration;
- review trigger;
- function-completion termination;
- revocation condition;
- context-termination condition.

> **Past Permission ≠ Present Permission**

> **Function Completion Should Normally Terminate Function-Derived Permission**

> **Context Termination Should Terminate Context-Derived Permissions Unless Another Legitimate Basis Persists**

## 19. Revocation and restriction

A legitimate permission may be narrowed, revoked or replaced where the underlying basis permits that change.

Record:
**PermissionChange = <PermissionClaim, Change, Basis, EffectivePoint, Actor/Source, Provenance, State>**

Revocation itself may be contestable under external rules. FPA records the change and its basis; it does not make every attempted revocation legitimate.

## 20. Delegation

Permission to act does not automatically include permission to authorise someone else.

> **Permission to Act ≠ Permission to Delegate**

Delegation should record:
- delegating basis;
- delegated participant;
- actions;
- target/context;
- function;
- conditions;
- temporal scope;
- re-delegation state;
- termination.

Unauthorised delegation is a permission failure.

## 21. Emergency-bounded permission

A credible emergency may alter the permission relationship where intervention is necessary and proportionate to the legitimate emergency function.

**Emergency Function → Required Intervention → Minimum Necessary Emergency Permission → Emergency Action → Emergency End → Override Termination**

> **Emergency Need ≠ Unlimited Emergency Authority**

Candidate emergency record:

**EmergencyPermission = <CredibleEmergencyBasis, PotentialConsequence, RequiredAction, Target/Context, MinimumScope, TimeSensitivity, Constraints, Review/Provenance, TerminationState>**

Emergency permission should not silently persist after the emergency basis ends.

## 22. Conflicting claims

A case may contain multiple apparently legitimate permission claims.

Examples:
- privacy versus maintenance responsibility;
- confidentiality versus emergency protection;
- individual consent versus independently applicable legal obligation.

FPA should represent the conflict rather than fabricate a resolution.

Candidate state:

**CONFLICTING-CLAIMS / REQUIRES-HIGHER-ORDER-REVIEW**

> **Representation of Permission Conflict ≠ Resolution of Permission Conflict**

## 23. Permission status

Candidate statuses:
- **PERMITTED**;
- **PERMITTED-WITH-CONDITIONS**;
- **NOT-PERMITTED**;
- **EXPLICITLY-PROHIBITED**;
- **PERMISSION-EXPIRED**;
- **PERMISSION-REVOKED**;
- **EMERGENCY-BOUNDED-PERMISSION**;
- **CONFLICTING-CLAIMS**;
- **REQUIRES-ADDITIONAL-CONSENT**;
- **REQUIRES-HIGHER-ORDER-REVIEW**;
- **UNKNOWN/INSUFFICIENT-BASIS**.

These are not necessarily a single ladder. Multiple fields may be required to represent a complex case.

## 24. Physical capability

A participant may be technically able to perform an action without possessing legitimate permission.

An unlocked door, visible file, known password, open API, administrator capability or physical proximity does not by itself establish permission.

> **Physical/Technical Capability ≠ Normative Permission**

FPA concerns permission. Actual behaviour and capability should be separately observable where relevant.

## 25. Ownership and stewardship

Ownership or stewardship may be one legitimate source of permission rules, but does not automatically erase independently held rights or constraints.

> **Ownership ≠ Unlimited Contextual Sovereignty**

The portable module does not define property law or the complete rights of owners, occupants, users, workers, guests or other parties.

## 26. Consent

Consent may be one permission basis but should not be treated as valid merely because a system labels it consent.

Where consent is material, relevant external questions may include:
- capacity;
- voluntariness;
- informed scope;
- specificity;
- withdrawal;
- coercive dependency;
- dark patterns.

FPA records consent state and scope; specialised consent architecture determines validity where necessary.

> **Recorded Consent ≠ Automatically Legitimate Consent**

## 27. Cultural and local variation

Different communities may establish different legitimate defaults.

FPA standardises the permission grammar more strongly than the permission outcome.

> **Standardise the Interface More Strongly Than the Outcome**

A local convention should be represented as a local/contextual rule source, not silently promoted to universal law.

## 28. Human-readable and machine-readable forms

A permission claim may be represented in human-readable or machine-readable form.

Where both exist:

> **Machine-Readable Rule ≠ Automatically Authoritative Rule**

Material divergence between human-readable and machine-readable rules should be treated as a conflict/error requiring resolution.

Machine representation communicates/evaluates a declared rule; it does not prove the rule is justified.

## 29. Anti-bureaucracy boundary

FPA is not intended to require formal records for every ordinary social action.

Use the minimum representational precision appropriate to consequence, ambiguity, risk and need for interoperability/audit.

Low-consequence ordinary contexts may rely on lightweight conventions. Consequential, contested, automated or cross-context cases may require richer records.

> **Permission Legibility ≠ Permission Bureaucracy**

## 30. Permission creep

A narrow permission can become improperly interpreted as a broader entitlement.

Examples:
- maintenance access → general access;
- emergency access → routine authority;
- temporary access → indefinite access;
- observe → record;
- enter → use;
- use → modify;
- act → delegate.

The module should compare proposed action against the current permission claim rather than relying on historical access alone.

## 31. Permission inheritance

Inheritance must be explicit or independently justified.

Candidate inheritance states:
- INHERITS;
- DOES-NOT-INHERIT;
- CONDITIONAL-INHERITANCE;
- UNKNOWN.

> **Parent Permission ≠ Automatic Child Permission**

> **Broad Context Membership ≠ Permission to Every Nested Resource**

## 32. Minimum operating procedure

For a materially consequential permission question:

1. Identify the participant.
2. Identify the proposed action.
3. Identify the target/context.
4. Identify the function/purpose.
5. Identify the claimed permission basis and rule source.
6. Identify consent where relevant.
7. Identify path/nested-context implications.
8. Identify current state.
9. Identify temporal scope.
10. Identify restrictions, revocation and termination conditions.
11. Identify delegation state where relevant.
12. Identify higher-order constraints or conflicting claims.
13. Determine the minimum permission reasonably necessary for the legitimate function.
14. Classify the permission state.
15. If conflict cannot legitimately be resolved locally, route to the relevant external process.
16. Perform only the bounded permitted action.
17. Terminate or update function/context-derived permission when its basis changes or ends.
18. Preserve provenance proportionate to consequence and audit need.

## 33. Candidate output classifications

**FPA-C1 — PERMISSION CONFIRMED**  
A sufficiently supported permission exists for the proposed action within stated scope.

**FPA-C2 — PERMISSION CONFIRMED WITH CONDITIONS**  
Permission exists only under specified restrictions, route, state, time, function or other conditions.

**FPA-C3 — ADDITIONAL CONSENT/PERMISSION REQUIRED**  
Existing permission does not extend to the proposed action/context.

**FPA-C4 — PERMISSION ABSENT / NOT SUPPORTED**  
No sufficient legitimate basis for the proposed permission is established.

**FPA-C5 — EXPLICIT PROHIBITION**  
A relevant legitimate rule explicitly prohibits the action.

**FPA-C6 — PERMISSION EXPIRED / TERMINATED**  
A prior permission no longer applies.

**FPA-C7 — PERMISSION REVOKED / RESTRICTED**  
A previously applicable permission has been legitimately changed, subject to external review where contested.

**FPA-C8 — EMERGENCY-BOUNDED PERMISSION**  
A credible emergency supplies a bounded temporary basis for necessary/proportionate action.

**FPA-C9 — CONFLICTING PERMISSION CLAIMS**  
Multiple material claims conflict and cannot be resolved by the permission grammar alone.

**FPA-C10 — HIGHER-ORDER REVIEW REQUIRED**  
External ethical/legal/institutional/domain resolution is required.

**FPA-C11 — DELEGATION LIMIT / FAILURE**  
The proposed action depends on absent, exceeded or unclear delegation authority.

**FPA-C12 — UNKNOWN / INSUFFICIENT BASIS**  
The available evaluation space is insufficient to determine permission reliably.

Multiple classifications may coexist where they represent different dimensions of the case.

## 34. Failure modes

### 34.1 Capability laundering
Treating ability to act as permission to act.

### 34.2 Ownership laundering
Treating ownership as unlimited authority over all participants and contexts.

### 34.3 Role laundering
Treating a role as general access unrelated to its legitimate function.

### 34.4 Function laundering
Inventing or broadening a function to justify desired access.

### 34.5 Consent laundering
Treating coerced, bundled, stale or out-of-scope consent as permission.

### 34.6 Implied-permission laundering
Presenting a contested local convention as a universal default.

### 34.7 Permission creep
Expanding a narrow permission into broader actions, spaces, times or purposes.

### 34.8 Emergency creep
Allowing temporary emergency permission to become routine authority.

### 34.9 Inheritance error
Assuming parent-context permission automatically applies to nested contexts.

### 34.10 Route laundering
Using destination permission to justify an unrelated or more intrusive route.

### 34.11 State inference error
Assuming a convenient state without sufficient basis.

### 34.12 Stale permission
Continuing to rely on permission after function, time, context or relationship basis has ended.

### 34.13 Delegation laundering
Assuming permission to act includes permission to delegate.

### 34.14 Rule-source collapse
Ignoring whether a rule derives from law, contract, consent, convention, emergency or another basis.

### 34.15 Machine-legibility laundering
Treating encoded rules as automatically legitimate.

### 34.16 Excessive bureaucracy
Formalising low-consequence ordinary interaction until the permission system itself damages autonomy/usability.

### 34.17 Hidden discrimination
Using selective access rules as an unexamined mechanism of discriminatory exclusion.

### 34.18 Provenance loss
Losing the basis, scope or termination conditions of consequential permission.

## 35. Adversarial checks

Before accepting a consequential permission claim, ask:

1. Are we confusing capability with permission?
2. Are we confusing ownership, residence, role or relationship with unlimited permission?
3. Is the proposed action actually within the granted function?
4. Is the route itself permitted?
5. Does permission inherit into the nested context?
6. Is the relevant state known or merely assumed?
7. Is the permission still temporally valid?
8. Has consent been exceeded, withdrawn or bundled?
9. Is an implied permission actually supported by this context?
10. Is an emergency being used to manufacture ongoing authority?
11. Does the actor have delegation authority?
12. Are multiple legitimate claims in conflict?
13. Is a machine-readable rule being mistaken for proof of legitimacy?
14. Are we applying a local cultural default universally?
15. Are we creating more bureaucracy than the consequence justifies?
16. What terminates this permission?

## 36. Interface with Contextual Wrapper Architecture

Contextual Wrapper Architecture describes the bounded environment and how rules/conditions change across it.

FPA describes participant-action permission relationships within and across those contexts.

> **Context Description ≠ Permission Relationship**

FPA can consume contextual information from a wrapper architecture but does not require CWA specifically.

## 37. Interface with Minimum Necessary Capability

Minimum Necessary Capability asks what capability is justified by a required function.

FPA asks whether a participant is permitted to perform a particular action in a particular context under a legitimate basis.

> **Capability ≠ Permission**

The modules may be composed but should remain independently intelligible.

## 38. Interface with external systems

FPA may require external resolution from:
- law/regulation;
- ethics/rights architecture;
- consent/capacity systems;
- safeguarding;
- security;
- property/tenancy rules;
- employment rules;
- parental/developmental responsibility;
- contracts;
- emergency procedures;
- dispute resolution;
- cultural/local convention records.

These interfaces should supply domain-specific legitimacy where FPA itself has no authority to decide it.

## 39. Falsification and weakening criteria

The architecture should be weakened, narrowed or rejected if testing shows that:
- contextual permission cannot be represented without impractical complexity;
- implied permission is too culturally variable for a useful common grammar;
- ordinary users cannot understand the model;
- formalisation systematically reduces autonomy;
- nested permissions create irresolvable ambiguity;
- MNP produces unacceptable uncertainty;
- domain-specific systems consistently solve the problem better without this abstraction;
- the architecture encourages excessive control over ordinary behaviour.

## 40. Portability claim

Currently supported:

> **A coherent standalone portable specification has been extracted from a substantial historical Concord source architecture and source-resolution audit.**

Not yet supported:

> **The specification has demonstrated independent functional transfer outside Concord.**

That requires frozen blind transfer testing.

## 41. Source provenance

Primary historical source:

*Fractal Permission Architecture — Context, Function and Minimum Necessary Access Across Public, Private and Safe Spaces*, Concord V1.1, 13 September 2026.

Source status was REVIEW COPY / FOUNDATIONAL ARCHITECTURAL FINDING / ACTIVE DEVELOPMENT / NOT CANONICAL.

Portable extraction record:

*Fractal Permission Architecture — Source Resolution and Extraction Audit 001.*

The portable specification must not retroactively upgrade the epistemic status of the historical source.

## 42. Development next step

Freeze **Fractal Permission Architecture — Blind Transfer Test 001** before obtaining an independent response.

The first test should use a materially non-Concord domain and pressure:
- binary-access failure;
- action-specific permission;
- path/nested-context permission;
- role/function limits;
- explicit versus implied permission;
- state/time dependence;
- termination;
- delegation;
- emergency bounded override;
- permission conflict;
- cultural/local defaults;
- capability versus permission;
- anti-bureaucracy boundary.
