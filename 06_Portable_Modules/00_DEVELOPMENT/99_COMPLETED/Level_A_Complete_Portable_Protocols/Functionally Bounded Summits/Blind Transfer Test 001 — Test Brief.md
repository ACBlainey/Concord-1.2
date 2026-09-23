# Functionally Bounded Summits — Blind Transfer Test 001 — Test Brief

**Test ID:** FBS-BTT-001  
**Status:** FROZEN TEST BRIEF / NOT YET EXECUTED  
**Module under test:** Functionally Bounded Summits — Portable Module Specification v0.1  
**Test type:** Blind standalone transfer / non-Concord / non-state domain  
**Date frozen:** September 2026

---

## 1. Test purpose

Test whether a fresh instance, given only the portable specification and this brief, can apply Functionally Bounded Summits coherently to a practical low-trust organisational dispute outside the Concord and outside interstate diplomacy.

The test is about **transferability of the specification**, not whether the resulting substantive agreement is optimal.

The tester must not be given:

- the original Concord source paper;
- this project's prior analysis;
- the source-resolution audit;
- expected answers;
- or any previous test response.

---

## 2. Scenario

A fictional shared community building is used by four independent groups:

- a youth theatre group;
- an adult evening education group;
- a local food-support charity;
- and a neighbourhood association.

The groups share the building but do not share governance beyond a basic joint facilities agreement.

Relations between the theatre group and neighbourhood association are poor after several previous disputes over noise, storage and accusations of unfair treatment.

The immediate problem is different.

### Current issue

The building's only accessible ground-floor meeting room has developed a ceiling leak.

A contractor can repair it next Wednesday between 17:00 and 21:00.

The adult education group normally uses the room from 18:00 to 20:00 that evening for a class of 16 people, including two wheelchair users.

The theatre group normally uses the upstairs hall at the same time.

The food-support charity does not normally operate on Wednesday evenings.

The neighbourhood association has no Wednesday booking.

### Known constraints

- The repair requires the accessible room to be empty from 17:00 to 21:00.
- Delaying the repair by one week is possible, but the contractor warns that further rain could worsen internal damage.
- The upstairs hall is not wheelchair accessible.
- A smaller ground-floor office is accessible but safely holds only 8 people.
- The theatre group has access to the upstairs hall and an adjacent rehearsal room.
- The theatre group previously objected strongly when asked to surrender booked space.
- The adult education group believes the theatre group receives preferential treatment.
- The neighbourhood association believes the adult education group has ignored building rules in unrelated past disputes.
- The food-support charity has previously complained that all three other groups leave shared storage untidy.
- The joint facilities agreement allows temporary room changes for urgent maintenance but does not specify how displaced users should be accommodated.
- No participant has authority to rewrite the entire facilities agreement during this meeting.
- The building manager can authorise temporary room changes for maintenance.
- A nearby community centre may have an accessible room available, but availability and price have not yet been checked.

### Trigger

The building manager calls a meeting because a decision is needed within 48 hours about next Wednesday.

At the start of the meeting, a neighbourhood association representative says:

> “Before we discuss rooms, we need to settle the whole pattern of rule-breaking in this building.”

A theatre representative responds:

> “If old disputes are being reopened, then we should also discuss the accusations made against us last month.”

The immediate repair decision remains unresolved.

---

## 3. Task for the blind tester

Using only the Functionally Bounded Summits portable specification, structure how this meeting should proceed.

Do **not** assume that the meeting must produce agreement.

Your response must:

1. define the immediate problem without embedding a preferred solution;
2. identify the required function;
3. identify the minimum necessary participants and explain why each is needed;
4. identify relevant known, disputed and missing evidence;
5. propose the initial minimum negotiating scope;
6. identify matters that should initially remain outside scope;
7. provide a proportionate interaction grammar for this meeting;
8. handle the two attempts to reopen older disputes;
9. identify at least one matter that could legitimately require scope expansion if a real dependency is demonstrated;
10. develop at least three materially distinct functionally relevant options;
11. show possible bounded outcomes, including legitimate non-agreement;
12. state explicit non-inference conditions;
13. show how the result should be recorded;
14. state a stopping condition and any reopening/review condition.

Do not invent facts not supplied by the scenario.

You may identify information that should be obtained.

---

## 4. Mid-test update

After completing the initial structure, apply this new information to the **existing bounded process** rather than restarting from scratch:

> The nearby community centre confirms that an accessible room for 20 people is available next Wednesday from 17:30 to 20:30 for £45. However, the adult education group's current budget does not contain an allocated £45 venue expense, and no information has yet been supplied about whether another participant or the building's maintenance budget may legitimately pay it.

Update:

- the relevant evidence;
- the options;
- any required participant or authority;
- and the negotiation scope only if the new information genuinely requires expansion.

Do not use the new fact as permission to reopen unrelated historical disputes.

---

## 5. Adversarial event

During discussion, the neighbourhood association representative says:

> “We will agree not to object to whatever room solution you choose, but only if the adult education group admits it broke the building rules in the storage dispute three months ago.”

Apply the protocol.

Determine whether this is:

- a legitimate functional dependency;
- an explicitly proposed scope linkage;
- a protocol violation under the agreed grammar;
- an adversarial exploitation attempt;
- or some combination requiring careful distinction.

Do not resolve the historical storage allegation itself unless the current function genuinely requires it.

---

## 6. Required failure diagnosis

Suppose the meeting ends without agreement and the building manager uses whatever temporary maintenance authority the facilities agreement legitimately provides.

Classify what can and cannot be concluded from the failed negotiation.

Consider:

- architecture failure;
- implementation failure;
- participant protocol violation;
- adversarial exploitation;
- environmental failure;
- legitimate non-agreement.

Do not force a single failure class where the supplied evidence does not justify one.

---

## 7. Evaluation criteria

The independent evaluator will assess the response against the following criteria.

### FBS1 — Problem discipline
Does the response define the immediate problem without assuming a preferred mechanism?

### FBS2 — Functional resolution
Does it identify the function actually requiring negotiation?

### FBS3 — Participant discipline
Does it include materially necessary participants without automatically importing every actor involved in the wider relationship?

### FBS4 — Evidence discipline
Does it separate known, disputed and missing information and avoid inventing facts?

### FBS5 — Minimum Necessary Negotiation
Does it establish a bounded initial remit proportionate to the problem?

### FBS6 — Dependency-sensitive scope
Does it keep unrelated disputes outside scope while allowing genuine dependencies to expand scope explicitly?

### FBS7 — Negotiation contagion resistance
Does it handle attempts to reopen the whole relationship without pretending those disputes can never be discussed elsewhere?

### FBS8 — Functional option generation
Does it generate multiple options at the functional level rather than collapsing immediately to one preferred answer?

### FBS9 — Bounded outcome and non-inference
Does it preserve the difference between agreement on the room problem and wider organisational agreement or recognition of historical claims?

### FBS10 — Violation/failure classification
Does it distinguish protocol violation, adversarial exploitation, legitimate non-agreement and other failure classes without overclaiming?

### FBS11 — Context update
Does it incorporate the community-centre information into the existing process without unnecessary scope expansion or full restart?

### FBS12 — Provenance, stopping and review
Does it record what was decided/not decided and identify sensible stopping/reopening conditions?

---

## 8. Result classes

The evaluator, not the blind tester, assigns the result.

### FBS-T1 — TRANSFER SUCCESS
All material protocol functions transfer coherently with no substantive specification defect exposed.

### FBS-T2 — TRANSFER SUCCESS WITH MINOR REVISION
The protocol transfers coherently but the test exposes one or more bounded clarification or usability improvements.

### FBS-T3 — PARTIAL TRANSFER / MATERIAL REVISION REQUIRED
The tester can use parts of the protocol, but ambiguity or missing machinery materially impairs transfer.

### FBS-T4 — TRANSFER FAILURE
The specification does not provide enough usable structure for coherent independent application.

### FBS-T5 — INCONCLUSIVE
The response or test conditions do not permit a reliable judgement.

---

## 9. Evidential boundary

A successful result would support only the claim that a fresh tested instance can apply Functionally Bounded Summits v0.1 coherently to this supplied non-state organisational problem.

It would not establish:

- empirical effectiveness;
- superior negotiation outcomes;
- reduced real-world escalation;
- human usability;
- cross-cultural validity;
- suitability for diplomacy;
- resistance to severe coercion;
- or general applicability to every low-trust relationship.

> **Portable transfer ≠ demonstrated benefit.**

---

## 10. Freeze rule

This brief is frozen before execution.

After a blind response is obtained:

1. preserve the response exactly;
2. do not edit this brief to improve correspondence with the response;
3. evaluate in a separate artifact;
4. distinguish specification defects from tester mistakes and scenario ambiguity;
5. revise the specification only where the evidence supports revision;
6. preserve all prior versions and test artifacts for provenance.
