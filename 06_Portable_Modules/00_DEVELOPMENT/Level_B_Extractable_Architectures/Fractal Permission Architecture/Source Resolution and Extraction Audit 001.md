# Fractal Permission Architecture — Source Resolution and Extraction Audit 001

**Candidate:** Fractal Permission Architecture
**Development level:** Level B — Extractable Architecture
**Status:** SOURCE RESOLUTION COMPLETE / EXTRACTION AUTHORISED
**Date:** 23 September 2026

## 1. Resolution result

The current V1.2 branch contains only the portable-development placeholder, but Git-history resolution recovered the complete source paper from Concord V1.1.

Primary source:

**Fractal Permission Architecture — Context, Function and Minimum Necessary Access Across Public, Private and Safe Spaces**

Historical source metadata:
- Author: Alexander C. Blainey
- Project: The Concord V1.1
- Date: 13 September 2026
- Status: REVIEW COPY / FOUNDATIONAL ARCHITECTURAL FINDING / ACTIVE DEVELOPMENT / NOT CANONICAL
- Length: 58 substantive sections in the recovered source

> **No Source Found on Current Branch ≠ Source Does Not Exist**

The historical source is sufficiently complete for portable extraction.

## 2. Source purpose

The paper begins from the finding that spatial classification alone cannot determine legitimate access.

Its central observation is:

> **Spatial Classification ≠ Access Classification**

A physical or digital space may support different simultaneous permission relationships depending on participant, role, relationship, function, consent, rules, state and context.

## 3. Core source model

The source gives the preliminary expression:

**Effective Permission = f(Space, Participant, Role, Relationship, Function, Consent, Applicable Rules, Current State, Context)**

It explicitly states that this is conceptual and extensible rather than a final mathematical equation.

A compact permission claim is:

> **Participant P may perform Action A in Space S for Function F under Conditions C during Time T.**

The source later compresses this to:

> **WHO may do WHAT, WHERE, WHY, WHEN, under WHICH CONDITIONS, by WHICH LEGITIMATE BASIS, and until WHEN?**

## 4. Central mechanism

The strongest source mechanism is:

**Legitimate Function → Required Interaction → Required Spatial / Informational / Behavioural Access → Minimum Necessary Permission → Function-Bounded Activity → Function Completion → Permission Termination**

The source names this **Minimum Necessary Permission**.

Portable principle:

> **Where a legitimate function requires access to a space, resource, participant or capability, the resulting permission should normally extend only as far as reasonably necessary to perform that function, remain subject to higher-order rights and applicable rules, and terminate when the function or other legitimate basis for the permission ends.**

Short form:

> **Function → Need → Minimum Necessary Permission**

## 5. Permission is multidimensional

The source rejects binary “has access / has no access” models.

Candidate permission actions include:
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
- authorise.

> **Access ≠ Single Permission**

The portable module should represent permissions as scoped claims rather than one undifferentiated access flag.

## 6. Permission dimensions

The source establishes that permission may be:

- **space-specific**;
- **path-specific**;
- **purpose/function-specific**;
- **participant-specific**;
- **role-specific**;
- **relationship-specific**;
- **consent-specific**;
- **state-dependent**;
- **time-bounded**;
- **rule-source dependent**;
- **nested/contextual**;
- **emergency-modified**.

This produces a permission topology rather than a flat access list.

## 7. Rule provenance

The source distinguishes:
- legal requirement;
- owner/steward rule;
- contractual condition;
- relationship permission;
- cultural convention;
- contextual inference;
- emergency necessity.

> **Rule Content ≠ Rule Source**

Portable extraction should preserve provenance because identical-looking permission rules can have different legitimacy, scope, revocability and consequences depending on their basis.

## 8. Explicit and implied permission

The source recognises both explicit permission and bounded implied permission.

Candidate implied-permission principle:

> **Where a function is ordinary, legitimate, reasonably expected and requires limited access to perform, a bounded contextual permission may be implied unless explicitly restricted or conflicting rights and circumstances require otherwise.**

The source itself marks this as requiring substantial legal, cultural and empirical testing.

Therefore portable extraction must not convert culturally contingent implied permissions into universal defaults.

> **Universal Permission Grammar ≠ Universal Permission Outcome**

## 9. Nested permission

The source establishes:

> **Parent-Space Permission ≠ Automatic Child-Space Permission**

Permission may narrow as contextual privacy/risk increases. Deeper contextual access may require stronger or more specific justification.

This is the “fractal” aspect: contexts can contain nested contexts with different permission relationships without each becoming a separate jurisdiction.

## 10. State and time

Permission may change when state changes:
- occupied/unoccupied;
- open/closed;
- active/inactive;
- event active/concluded;
- ordinary/emergency;
- hazardous/safe;
- confidential session active/inactive;
- temporary restriction.

> **Same Physical Space + Different Current State → Different Permission Structure**

Permission may also have explicit temporal scope.

> **Past Permission ≠ Present Permission**

## 11. Permission termination

The source repeatedly guards against stale or creeping permission:

> **Function Completion Should Normally Terminate Function-Derived Permission**

> **Context Termination Should Terminate Context-Derived Permissions Unless Another Legitimate Basis Persists**

Portable extraction should therefore treat termination/expiry as part of the permission object, not an optional afterthought.

## 12. Emergency override

The source permits bounded emergency override where necessary and proportionate to a legitimate emergency function.

**Privacy Context + Credible Emergency Context → Minimum Necessary Emergency Access**

But:

> **Emergency Need ≠ Unlimited Emergency Authority**

Emergency access must remain function-bounded and should terminate when the emergency basis ends.

## 13. Permission versus capability

The source strongly separates physical/technical possibility from normative legitimacy:

> **Capability to Enter ≠ Permission to Enter**

> **Physical Accessibility ≠ Normative Accessibility**

> **Physical Capability ≠ Normative Permission ≠ Actual Behaviour**

An unlocked door, technically available API or visible resource does not itself establish legitimate permission.

## 14. Permission conflict

Multiple legitimate claims may conflict. The source examples include privacy versus maintenance responsibility, child privacy versus safeguarding responsibility, and patient privacy versus emergency medical need.

The permission grammar does not itself resolve every such conflict.

> **Representation of Permission Conflict ≠ Resolution of Permission Conflict**

Resolution may require external ethical, legal, contractual or domain-specific architecture.

## 15. Relationship to Minimum Necessary Capability

Fractal Permission Architecture and Minimum Necessary Capability are related but not identical.

MNC asks how much capability is justified by a required function.

FPA asks which participant may perform which action in which context, for which function, under which legitimate basis and conditions.

A system may possess technical capability while permission remains absent or narrower.

> **Capability ≠ Permission**

Portable FPA may use a minimum-necessary logic without collapsing into the existing MNC module.

## 16. Relationship to Contextual Wrapper Architecture

The source explicitly distinguishes:

**Fractal Contextual Wrappers:** What changes when a participant enters or operates within a bounded context?

**Fractal Permission Architecture:** Given that context, who may do what, where, why, when and under what legitimate basis?

The portable Contextual Wrapper Architecture therefore provides a related interface but is not a hidden prerequisite.

> **Context Description ≠ Permission Relationship**

## 17. Concord-specific dependencies to externalise

The source references:
- Safe Spaces;
- Public/Private Space Architecture;
- Fractal Contextual Wrappers;
- Concord Interoperability Wrappers;
- Ethical Kernel;
- Authority Justification Chain;
- Peaceful/Respectful Distance;
- GTP;
- Layer 0 / Layer −0;
- Ratchet;
- Developmental Priority.

These should become generic interfaces where necessary. The portable module must not require adoption of Concord ontology.

## 18. Candidate portable problem

> **How can a system represent who may legitimately do what, where, why, when and under which conditions without collapsing permission into physical capability, binary access, ownership, role or a universal context-independent rule?**

## 19. Candidate portable principle

> **Represent permission as a bounded contextual relationship among participant, action, resource/context, function, legitimate basis, conditions and time; grant no more permission than the legitimate basis requires; and terminate context-derived permission when that basis ends.**

Short form:

> **Who. What. Where. Why. When. Under what legitimate basis. No more than necessary.**

## 20. Minimum standalone inputs

A portable mechanism requires, where materially relevant:
- participant/actor;
- proposed action;
- target space/resource/context;
- function/purpose;
- permission basis/source;
- consent state;
- applicable rules;
- current context/state;
- temporal scope;
- relevant path or sub-context;
- restrictions/conditions;
- revocation/termination conditions;
- known higher-order rights or constraints.

Unknown inputs should remain UNKNOWN rather than be inferred merely from capability or convenience.

## 21. Minimum standalone outputs

Candidate outputs include:
- PERMITTED;
- PERMITTED-WITH-CONDITIONS;
- NOT-PERMITTED;
- EXPLICITLY-PROHIBITED;
- PERMISSION-EXPIRED;
- PERMISSION-REVOKED;
- EMERGENCY-BOUNDED-PERMISSION;
- CONFLICTING-CLAIMS;
- REQUIRES-ADDITIONAL-CONSENT;
- REQUIRES-HIGHER-ORDER-REVIEW;
- UNKNOWN/INSUFFICIENT-BASIS.

The specification should avoid pretending that all permission conflicts can be mechanically resolved.

## 22. Candidate permission record

A conceptual record may take the form:

**PermissionClaim = <Participant, Action, Target/Context, Function, Basis, RuleSource, Consent, Path, State, Conditions, Start, Expiry/Termination, DelegationScope, Provenance, Status>**

This should remain extensible.

## 23. Critical portable separations

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

> **Machine-Readable Permission ≠ Machine-Determined Legitimacy**

> **Permission Representation ≠ Permission Justification**

## 24. Candidate failure modes

The source explicitly identifies at least:
1. excessive permission bureaucracy;
2. ambiguous implied permission;
3. conflicting cultural assumptions;
4. deceptive consent;
5. unclear property boundaries;
6. unclear contextual boundaries;
7. permission creep;
8. emergency-authority creep;
9. ownership treated as sovereignty;
10. parental responsibility treated as unlimited authority;
11. child safeguarding failures;
12. hidden surveillance;
13. discrimination through selective access;
14. inaccessible signage;
15. digital dark patterns;
16. machine-readable rules diverging from human-readable rules;
17. overlapping context conflicts;
18. unclear precedence;
19. inability to withdraw;
20. coercive dependency;
21. excessive fragmentation;
22. context state incorrectly inferred;
23. unauthorised delegation;
24. stale permissions;
25. permissions surviving after legitimate function ends.

Portable extraction should preserve these and test for additional abstraction-specific failures such as provenance laundering and rule-source collapse.

## 25. Anti-bureaucracy boundary

The source explicitly rejects turning ordinary social life into continuous formal permission administration.

The portable goal is not:

> **Require explicit formal permission for every action.**

It is:

> **Provide a coherent grammar capable of representing explicit permission, implied permission, convention and contextual judgement when precision is necessary.**

A portable implementation must permit lightweight use.

## 26. Cultural boundary

The source warns against encoding one culture's ordinary expectations as universal.

The portable layer should standardise representation more strongly than outcomes.

> **Standardise the Interface More Strongly Than the Outcome**

The module may represent a local default without declaring that default universally legitimate.

## 27. Machine-readable boundary

The architecture is suitable for machine-readable representation, but the source explicitly rejects treating encoded rules as self-justifying.

> **Machine-Readable Permission ≠ Machine-Determined Legitimacy**

A machine can communicate/evaluate a declared permission claim while the legitimacy of the underlying rule may remain contestable.

## 28. Falsification conditions

The source says the architecture should be weakened or rejected if testing shows that:
- contextual permission requires impractical complexity;
- implied permission is too culturally variable for useful common grammar;
- ordinary people cannot understand the model;
- formalisation reduces autonomy;
- nested permissions create irresolvable ambiguity;
- minimum necessary permission produces unacceptable uncertainty;
- existing domain systems handle the problem better without this abstraction;
- the architecture encourages excessive control over ordinary social behaviour.

These are important portable-development criteria.

## 29. Source completeness conclusion

The recovered 58-section source contains a coherent candidate architecture, explicit mechanism, conceptual data structures, failure modes, falsification conditions, interfaces and boundaries.

It is substantially more developed than the portable-development placeholder indicated.

> **SOURCE RESOLUTION SUFFICIENT FOR PORTABLE EXTRACTION**

> **NO BLOCKING SOURCE OMISSION IDENTIFIED AT THIS STAGE**

The original source remains a review-copy / active-development finding, so extraction must not overstate its validation state.

## 30. Next step

Produce **Fractal Permission Architecture — Portable Specification v0.1**.

The first specification should preserve:
- contextual permission claims;
- multidimensional action scope;
- function-bounded minimum necessary permission;
- rule/basis provenance;
- nested and path-specific permission;
- state/time dependence;
- explicit/implied permission distinction;
- termination/revocation;
- emergency bounded override;
- permission conflict without false automatic resolution;
- anti-bureaucracy and cultural-variation boundaries;
- separation from MNC and CWA.
