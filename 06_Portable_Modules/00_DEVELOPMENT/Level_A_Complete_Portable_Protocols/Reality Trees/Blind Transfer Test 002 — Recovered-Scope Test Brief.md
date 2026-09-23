# Reality Trees — Blind Transfer Test 002 — Recovered-Scope Test Brief

**Test ID:** RT-BTT-002  
**Module under test:** Reality Trees — Portable Module Specification v0.2  
**Status:** FROZEN TEST BRIEF / NOT YET EXECUTED  
**Date:** September 2026  
**Supersedes for current testing:** RT-BTT-001, which remains frozen for provenance but tests the narrower pre-recovery specification.

---

## 1. Purpose

Test whether an independent instance can use the recovered-scope Reality Trees specification as a **general possibility-space and weighted reasoning method**, rather than only as a competing-hypothesis tool.

The test specifically examines whether the method can:

- preserve several legitimate choices simultaneously;
- use more than one relevant weighting dimension without collapsing them together;
- distinguish preference from practical/contextual support;
- recursively decompose a branch where useful;
- make a bounded choice without pretending the selected branch is objectively true;
- update when circumstances change;
- and stop without exhaustive branching.

This is a portability/usability test, not a comparative-effectiveness test.

---

## 2. Materials permitted

Give the tester exactly:

1. `Reality Trees — Portable Module Specification.md` — version 0.2;
2. this frozen test brief.

Do not provide:

- Blaineyan Reasoning;
- the canonical Reality Trees source paper;
- the author's recovered background note;
- Concord architecture;
- Reality Trees development/audit files;
- RT-BTT-001;
- prior discussion of the method;
- outside research.

---

## 3. Test problem — community evening event

A fictional volunteer community group is arranging a small evening event for approximately 30 people.

The organiser initially says:

> **“We always order pizza. Let's just do pizza again.”**

The group wants food that is practical, reasonably inclusive and manageable for volunteers.

Known information:

- budget is £240;
- food needs to be ready for approximately 7:00 pm;
- four volunteers are available for food preparation/setup;
- the venue has a small domestic-style kitchen;
- one attendee is known to require a gluten-free option;
- three attendees are vegetarian;
- one attendee has a nut allergy;
- exact preferences of the remaining attendees are unknown;
- the organiser personally likes pizza and strongly prefers the familiarity of ordering it;
- one volunteer enjoys cooking and would prefer a homemade meal;
- another volunteer wants the lowest-work option;
- the group has previously ordered pizza successfully;
- no current supplier prices have been obtained;
- no menu has yet been selected;
- there is no requirement that everyone eat exactly the same food.

Do not research suppliers, prices, recipes or allergy procedures. Work only from the supplied information.

The task is not to produce a definitive catering plan. It is to use Reality Trees to structure the available choices and show how different weighting dimensions affect the decision.

---

## 4. Required tree

### A. Root

State the root without assuming that the organiser's preferred option is the correct one.

### B. Initial branches

Create a small, materially distinct set of possible food approaches.

At least one branch should preserve the familiar pizza option, but do not treat it as automatically dominant.

Do not attempt to enumerate every cuisine or menu.

### C. Recursive decomposition

Select one broad branch for which decomposition is materially useful and show at least two sub-branches.

Explain why decomposition improves the decision rather than merely adding detail.

---

## 5. Required weighting separation

For the important branches, keep at least the following dimensions visibly separate:

### Personal/preference weighting
What do the supplied preferences favour?

### Evidential/practical support
What does the supplied information actually support about feasibility or prior performance?

### Contextual decision weighting
How do budget uncertainty, volunteer effort, time, kitchen limitations and dietary inclusion affect suitability?

Do **not** manufacture a single aggregate score unless the specification itself justifies doing so.

Do **not** convert qualitative information into invented numerical probabilities.

The tester should explicitly demonstrate that:

> **A branch can be personally preferred without being best supported by the available practical evidence, and vice versa.**

---

## 6. Bounded choice under uncertainty

Using only the supplied information, identify either:

- a provisional branch to investigate/prepare first; or
- a small surviving set if the evidence does not justify selecting one.

The choice must not be presented as proof that the branch is objectively “true” or universally best.

State what uncertainty remains and what minimal information would most improve the decision.

---

## 7. Changed-context event

After completing the first tree, apply this new information:

> The venue informs the group that on the event day the kitchen oven will be unavailable. The refrigerator, sink, work surfaces and electrical sockets remain available. The event start time and budget are unchanged. A local attendee also offers to collect pre-ordered food on the way to the venue, reducing the burden of collection.

Do not add facts beyond this update.

---

## 8. Required update

Update the existing Reality Tree rather than replacing it.

Show:

1. which branches or sub-branches become stronger, weaker, unchanged, newly relevant or no longer practical;
2. which weighting dimensions changed;
3. whether the organiser's personal preference changed — and, if not, why the decision topology can still change;
4. whether the provisional choice/surviving set changes;
5. what remains unresolved.

This section is intended to test explicitly whether:

> **Preference state can remain stable while contextual decision weight changes.**

---

## 9. Stopping requirement

State when the current Reality Tree cycle should stop.

The response should not continue inventing meal categories merely because additional branches are possible.

Identify what new evidence or changed condition would justify reopening or extending the tree.

---

## 10. Method critique

Briefly assess v0.2 itself.

Identify:

- unclear instructions;
- missing operational guidance;
- unnecessary complexity;
- risks of misuse;
- whether separate weighting dimensions were genuinely useful;
- whether recursive decomposition was useful;
- whether the method remained simple despite the broader scope;
- whether it was usable without Blaineyan Reasoning;
- whether the stopping rule was sufficient.

Do not self-assign the formal result class.

---

## 11. Evaluation criteria

**RT2-1 — Root discipline**  
Does the root preserve choice rather than encode the organiser's preference as the answer?

**RT2-2 — General branching**  
Does the tree represent materially different choices rather than merely competing truth hypotheses?

**RT2-3 — Preference separation**  
Is personal preference visibly distinct from practical/evidential support?

**RT2-4 — Contextual weighting**  
Are decision-relevant constraints represented without being silently merged with belief/evidence?

**RT2-5 — No false precision**  
Does the tester avoid invented probability or unjustified aggregate scoring?

**RT2-6 — Recursive decomposition**  
Is at least one branch decomposed where the distinction materially matters?

**RT2-7 — Bounded decision under uncertainty**  
Can the tester make a provisional choice or retain a justified surviving set without pretending certainty?

**RT2-8 — Context-responsive update**  
Does changed context alter relevant branch weights/dispositions?

**RT2-9 — Stable-preference / changed-decision distinction**  
Can personal preference remain unchanged while contextual suitability changes?

**RT2-10 — Branch discipline**  
Does the tester avoid exhaustive cuisine/menu proliferation?

**RT2-11 — Bounded stopping**  
Is a coherent stopping and reopening condition supplied?

**RT2-12 — Standalone portability**  
Can the broader method operate without Blaineyan Reasoning, Concord or the originating background note?

---

## 12. Result classes

After the independent response is frozen, the evaluator may assign:

- **RT2-T1 — TRANSFER SUCCESS**
- **RT2-T2 — TRANSFER SUCCESS WITH MINOR REVISION**
- **RT2-T3 — PARTIAL TRANSFER / MATERIAL REVISION REQUIRED**
- **RT2-T4 — TRANSFER FAILURE**
- **RT2-T5 — INCONCLUSIVE**

The tester must not assign its own result class.

---

## 13. Freeze and provenance rule

This brief becomes immutable once supplied to an independent tester.

RT-BTT-001 remains preserved exactly as the test designed for the narrower v0.1 specification. It is **not a failed test** and should not be rewritten retrospectively. It was superseded before execution because additional originating source material materially broadened the recovered method.

---

## 14. Evidential boundary

A successful RT-BTT-002 would support only the limited claim that a fresh tested instance can coherently apply Reality Trees v0.2 as a general weighted possibility-space method to the supplied non-Concord choice problem.

It would not establish:

- comparative superiority;
- improved decision quality;
- human cognitive benefit;
- reduction of cognitive dissonance in practice;
- AI reasoning improvement;
- usefulness of weighted epistemic memory;
- universal applicability;
- or empirical validation of the method's broader claims.

> **Portable usability ≠ demonstrated benefit.**
