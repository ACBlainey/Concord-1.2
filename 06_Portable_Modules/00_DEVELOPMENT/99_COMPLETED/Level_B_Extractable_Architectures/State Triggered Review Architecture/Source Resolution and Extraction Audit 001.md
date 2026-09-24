# State Triggered Review Architecture — Source Resolution and Extraction Audit 001

**Candidate:** State Triggered Review Architecture (STRA)
**Development level:** Level B — Extractable Architecture
**Method:** PMEDG v1.1
**Status:** SOURCE RESOLUTION SUBSTANTIALLY COMPLETE / PORTABLE EXTRACTION AUTHORISED
**Date:** September 2026

## 1. Audit purpose

Determine whether the Civilisation Clock source family contains a coherent portable review-trigger mechanism that can operate outside the Concord without importing the whole Civilisation Clock, Civil State Map, KCS, CDT or Concord governance.

The candidate is deliberately narrower than the full Civilisation Clock.

## 2. Primary source family

The strongest portable source is:

**02_Epistemic_and_Research/Civilisational_Developmental_Topology/Civilisation Clock Companion Extension 001 — State, Functional and Compound Trigger Architecture.md**

Supporting operational evidence includes:

- Civilisation Clock Dependency Test 001 — Upstream Bottleneck and Development-Order Evidence;
- Civilisation Clock Extension 001 — Consequence-Relevant State Transition Layer;
- Civilisation Clock Queue Test 001 — First Dependency-Informed Development Order;
- Civilisation Clock Queue Test 002 — First Substantive Development Selection;
- Civilisation Clock Queue Test 004 — Validation Terminus;
- associated Civil State Map/KCS dependency work where it supplies state inputs rather than trigger ownership.

The source family shows both conceptual architecture and repeated internal use.

## 3. Source epistemic status

The Companion Extension is canonical but corrigible. It explicitly states that the general trigger mechanism is not operationally tested across all domains.

Clock queue tests provide internal prospective/operational consistency evidence, not independent external validation.

Therefore the portable candidate may inherit a coherent architecture, but it must not inherit a stronger validation claim than the sources support.

## 4. Source problem

The source rejects the interpretation of the Clock as merely chronological scheduling.

Its deeper problem is:

> When should a system reopen review, reconsider a decision, reactivate dormant work or become eligible for action when meaningful change may be driven by state, capability, dependency, evidence, risk or events rather than elapsed time alone?

The source distinction is:

> **Civilisation Clock ≠ Calendar**

and:

> **Civilisation Clock = State-Transition Scheduler + Review-Trigger Architecture**

The portable extraction should retain the review-trigger architecture without retaining the civilisational framing.

## 5. Candidate portable problem

> **How can a system represent when review or reconsideration becomes due using bounded conditions over time, state, capability, dependencies, events, risk, recurrence, evidence and participant-declared conditions, while keeping trigger detection separate from authority over the resulting action?**

This problem exists in research, engineering, software, safety review, archival systems, maintenance, governance processes, long-duration projects and agent systems.

## 6. Candidate portable kernel

The minimum reusable kernel is:

> **Represent condition → watch relevant state/evidence → detect material satisfaction → open review/action candidacy → route to legitimate owner → record outcome/state → continue, complete or supersede trigger.**

Central boundary:

> **Triggering Review ≠ Authority Over Outcome**

The trigger mechanism says that a condition has become reviewable/actionable. It does not decide the substantive result.

## 7. Trigger classes

The source supplies:

- TEMPORAL;
- STATE;
- CAPABILITY;
- DEPENDENCY;
- EVENT;
- RISK;
- RECURRENCE;
- EVIDENCE;
- PARTICIPANT;
- COMPOUND.

The portable architecture should preserve these as an extensible trigger vocabulary rather than a mandatory exhaustive ontology.

## 8. Compound conditions

Conditions may include:

- A;
- A AND B;
- A OR B;
- A AND NOT C;
- dependency D reaches state S;
- periodic backstop OR earlier material change.

This allows calendar time to act as a backstop without becoming the only scheduler.

## 9. Candidate trigger object

The source proposes:

**T = <type, subject, condition, evidence, owner, review-path, consequence, state>**

A fuller portable record may include:

- Trigger ID;
- subject;
- trigger class;
- condition expression;
- evidence/source interface;
- dependency references;
- earliest temporal boundary if any;
- temporal backstop if any;
- consequence class;
- legitimate action owner;
- review owner;
- notification/retrieval target;
- current trigger state;
- provenance;
- correction/supersession history.

This is an information model, not a prescribed implementation.

## 10. Candidate trigger states

Source candidate states:

- DORMANT;
- WATCHING;
- CONDITION-PARTIAL;
- CONDITION-SATISFIED;
- REVIEW-DUE;
- ACTION-PENDING;
- COMPLETED;
- SUPERSEDED;
- UNKNOWN;
- DISPUTED.

Portable extraction should preserve the distinction between condition satisfaction and completed substantive action.

## 11. Trigger satisfaction is not substantive decision

This is the strongest portability invariant.

A satisfied condition may produce:

- review due;
- notification;
- retrieval request;
- eligibility for reconsideration;
- action candidate;
- escalation to legitimate owner.

It does not inherently produce:

- permission;
- authority;
- truth;
- compulsory execution;
- rights override;
- automatic deployment.

> **Condition Satisfied ≠ Action Authorised**

## 12. State-input boundary

The source architecture depends on represented state.

Inside Concord the chain is:

KCS state → Civil State Map → Clock trigger evaluation → legitimate domain review/action → state update.

Portable extraction generalises this to:

> **Host state/evidence sources → Trigger evaluation → Legitimate host review/action → Host state update**

STRA therefore does not own the truth, completeness or legitimacy of every input state.

## 13. Dependency boundary

A DEPENDENCY trigger can reopen work when a prerequisite reaches a required state.

But STRA should not absorb full dependency discovery/change propagation.

It consumes represented dependency state or references supplied by the host or another dependency mechanism.

> **Dependency Trigger ≠ Dependency Graph Ownership**

## 14. Review/action ownership

Each consequential trigger should identify or interface with a legitimate review/action owner.

The trigger mechanism may route a candidate but must not manufacture an owner merely because the condition fired.

If ownership is unresolved, the correct state may be HOLD/UNKNOWN/REVIEW-ROUTING-REQUIRED rather than automatic action.

## 15. Evidence and uncertainty

Trigger evaluation must preserve uncertainty where the condition depends on uncertain evidence.

A trigger should not silently convert:

- incomplete evidence into certainty;
- missing evidence into false;
- disputed state into settled state;
- stale evidence into current evidence.

Where condition satisfaction is materially uncertain, the architecture must be able to represent partial, disputed or unknown satisfaction.

## 16. Temporal backstops

A temporal review can coexist with functional triggers:

> review every N months OR earlier if risk/evidence/capability changes materially.

This protects against trigger models that fail to notice unforeseen changes while avoiding pointless calendar-only review.

## 17. Recurrence

A recurrence trigger can reopen previously closed/dormant work when a materially similar pattern returns.

It must not assume superficial similarity is sufficient.

Host/domain interpretation determines whether recurrence is material.

## 18. Participant-declared conditions

The source includes participant-defined conditions such as voluntary wake-me-when cases.

Portable STRA may represent participant-declared triggers, but consent/identity/continuity rules remain external.

> **Participant Condition Satisfied ≠ Forced Action**

## 19. Cold-memory/retrieval interface

The source shows a useful interface:

Trigger → relevance signal → legitimate retrieval → revalidation → use or return to dormant storage.

STRA owns the trigger/relevance signal.

KCS or another memory system owns retrieval/provenance.

The domain owner owns substantive use.

## 20. Consequence-relevant transition interface

The Civilisation Clock later developed CRSTL to represent material precedence, legitimate concurrency, branch ancestry and uncertain ordering.

This is adjacent to STRA but should not automatically be absorbed into it.

STRA needs only enough transition/state information to evaluate its declared condition.

Complex event ordering or reconciliation remains an external interface unless a particular trigger condition explicitly requires it.

## 21. Candidate inputs

- trigger definition;
- subject;
- condition expression;
- represented state/evidence;
- dependency/capability/event references where required;
- temporal bounds/backstops where required;
- provenance;
- legitimate owner/routing information;
- host access/privacy constraints.

## 22. Candidate outputs

- current trigger state;
- condition satisfaction/partial/unknown/disputed result;
- evidence/provenance for the result;
- review/action candidate;
- notification/retrieval request where configured;
- routing target;
- next evaluation condition/backstop;
- correction/supersession record.

Outputs are review/control signals, not substantive domain decisions.

## 23. Minimum operating cycle

1. DEFINE — represent trigger and condition.
2. BIND — identify state/evidence sources and legitimate routing owner.
3. WATCH — observe relevant represented inputs.
4. EVALUATE — test condition without manufacturing certainty.
5. SIGNAL — mark partial/satisfied/review-due/unknown/disputed.
6. ROUTE — send review/action candidate to legitimate owner.
7. RECORD — preserve provenance and outcome.
8. UPDATE — complete, reset, continue watching, correct or supersede.
9. BACKSTOP — re-evaluate on temporal or other bounded fallback where defined.

## 24. Failure modes

STRA-F1 Calendar collapse — treating elapsed time as the only meaningful trigger.
STRA-F2 Trigger-authority collapse — condition satisfaction becomes automatic substantive authority.
STRA-F3 False satisfaction — weak/incomplete evidence treated as fulfilled condition.
STRA-F4 False non-satisfaction — missing/unobserved evidence treated as proof condition is false.
STRA-F5 Stale trigger — old condition remains active after assumptions materially change.
STRA-F6 Impossible trigger persistence — unreachable condition watches forever without review/backstop.
STRA-F7 Event overmatching — superficial event similarity fires a recurrence/event trigger.
STRA-F8 Cascade amplification — one trigger creates uncontrolled trigger chains.
STRA-F9 Dependency absorption — trigger architecture attempts to own the whole dependency graph.
STRA-F10 Domain absorption — trigger mechanism decides the substantive domain outcome.
STRA-F11 Consent bypass — participant-declared trigger becomes forced action.
STRA-F12 Privacy leakage — trigger evaluation/retrieval exposes more protected information than necessary.
STRA-F13 Stale reactivation — retrieved/dormant material is treated as current without revalidation.
STRA-F14 Ownership vacuum — trigger fires but no legitimate review/action owner exists.
STRA-F15 Total-order assumption — timestamp order is mistaken for all material precedence.
STRA-F16 Completeness illusion — unobserved relevant state is assumed not to exist.

## 25. Falsification/revision conditions

Question the portable mechanism if transfer testing shows that:

- useful non-temporal review cannot be represented without the full Concord Clock;
- condition satisfaction cannot remain separate from action authority;
- compound triggers cannot preserve UNKNOWN/DISPUTED states;
- temporal backstops cannot coexist with state/event triggers;
- dependency triggers require STRA to own the full dependency architecture;
- participant-defined conditions inherently require forced action;
- retrieval triggers cannot preserve revalidation/privacy boundaries;
- legitimate routing cannot be externalised;
- trigger correction/supersession necessarily erases history;
- a clean evaluator cannot apply the architecture outside civilisational development.

## 26. Concord-specific dependencies to externalise

- Civil State Map → generic host state/evidence interface.
- KCS → generic memory/provenance/retrieval interface.
- CDT → generic dependency/state semantics where required.
- constitutional/domain authority → legitimate host review/action owner.
- Continuity/participant autonomy → host consent/identity/continuity interface.
- CRSTL/CDRP → event-order/reconciliation interface where materially required.
- Threat Think Tank → ordinary domain-specific review owner.

## 27. Internal operational evidence

The source family has already used the broader Clock mechanism internally:

- CLOCK-001 selected retests and exposure investigations rather than premature development;
- CLOCK-002 selected substantive development once evidence justified it;
- CLOCK-004 reached a predeclared terminus without requiring further self-development.

This is useful internal operational evidence that the trigger/review grammar can guide differentiated action.

It is not independent external transfer evidence for STRA.

## 28. Extraction decision

A coherent portable mechanism is present and is narrower than the full Civilisation Clock.

> **SOURCE RESOLUTION SUBSTANTIALLY COMPLETE**

> **STATE-TRIGGERED REVIEW ARCHITECTURE IS A DISTINCT PORTABLE OWNER**

> **FULL CIVILISATION CLOCK EXTRACTION IS NOT REQUIRED**

> **PORTABLE SPECIFICATION v0.1 AUTHORISED**

The portable owner is:

> **condition representation + state/evidence watching + bounded trigger evaluation + review/action candidacy + legitimate routing + provenance/history**

while substantive authority, state truth, dependency ownership, memory retrieval, continuity and complex reconciliation remain external interfaces.

## 29. Next PMEDG stage

Create:

**State Triggered Review Architecture — Portable Specification v0.1**

Then freeze a blind transfer test in a materially non-Concord domain.
