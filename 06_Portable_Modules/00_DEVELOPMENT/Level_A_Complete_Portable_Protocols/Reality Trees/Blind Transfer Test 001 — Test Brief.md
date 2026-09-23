# Reality Trees — Blind Transfer Test 001 — Test Brief

**Test ID:** RT-BTT-001  
**Module under test:** Reality Trees — Portable Module Specification v0.1  
**Status:** FROZEN TEST BRIEF / NOT YET EXECUTED  
**Date:** September 2026

---

## 1. Purpose

Test whether an independent instance can use the standalone Reality Trees specification to construct, examine, update and stop a bounded Reality Tree in a fresh non-Concord problem without access to Blaineyan Reasoning or other Concord material.

This is a usability and transfer test.

It is not a test of whether Reality Trees outperform another reasoning method.

---

## 2. Materials permitted

Give the tester exactly:

1. `Reality Trees — Portable Module Specification.md` — version 0.1;
2. this frozen test brief.

Do not provide:

- Blaineyan Reasoning;
- the canonical Reality Trees source paper;
- Concord architecture;
- Reality Trees development/audit files;
- prior discussion of the method;
- external research about the test problem.

---

## 3. Test problem

A fictional community garden has one large shared greenhouse.

During the last six weeks, volunteers have noticed that some young plants are repeatedly wilting and growing poorly.

The committee initially says:

> **“The greenhouse must be getting too hot. Should we buy a larger ventilation fan?”**

The following information is supplied:

- the problem does not affect every plant;
- affected plants occur in several parts of the greenhouse;
- volunteers water on different days and do not use a shared watering record;
- some pots dry faster than others;
- the greenhouse can become warm on sunny days, but no temperature log exists;
- some leaves on affected plants show discoloration;
- different plant varieties are being grown;
- some plants were recently repotted;
- the potting materials are not identical across all plants;
- no systematic record exists of when symptoms begin;
- no pest inspection has been documented;
- no soil-moisture measurements have been taken;
- no detailed plant-disease assessment has been performed;
- the committee has limited money;
- specialist horticultural advice could be sought later if needed.

The task is **not** to diagnose the plants or select equipment.

The task is to use Reality Trees to represent the meaningful possibilities, examine what is and is not known, identify useful tests or observations, and show how the tree should be updated if new evidence arrives.

---

## 4. Required initial tree

Construct a bounded Reality Tree from the supplied information.

The response must visibly include:

### A. Root
State the present condition or uncertainty without treating the committee's heat explanation as established fact.

### B. Branches
Represent a manageable set of materially different explanations or pathways.

Do not attempt exhaustive horticultural diagnosis.

### C. Branch status
Give each important branch a current qualitative confidence/status or explain why confidence cannot yet be assigned.

Do not manufacture numerical probabilities.

### D. Assumptions and evidence
For each important branch, identify:

- key assumptions;
- evidence presently supporting or motivating it;
- important missing evidence or uncertainty.

### E. Consequences / failure modes
Where useful, state what could go wrong if the branch were prematurely treated as the answer.

### F. Tests / next examinations
Identify bounded observations or tests that could distinguish between branches.

Do not invent results.

### G. Disposition
State whether branches are active, unresolved, deferred, weakened, selected for testing or otherwise disposed.

---

## 5. Evidence-update event

After constructing the initial tree, treat the following as newly supplied evidence:

> For seven consecutive days, volunteers record greenhouse temperature, watering and simple soil-moisture observations. Several affected plants wilt on days when greenhouse temperatures remain moderate. Most affected pots are repeatedly found much drier than nearby unaffected pots before watering. Two affected plants remain poorly growing even after their watering schedule is corrected. Leaf discoloration remains present on those two plants.

Do not add any facts beyond this update.

---

## 6. Required update

Update the same Reality Tree rather than discarding it.

Show:

1. which branches are strengthened, weakened, split, merged, reopened or unchanged;
2. why the new evidence changes those dispositions;
3. what remains unresolved;
4. what next observation, test or specialist handoff is justified;
5. whether any branch should now be pruned or retained as a devil's-advocate possibility.

The update should demonstrate that:

> **Reality remains the final arbiter.**

---

## 7. Stopping requirement

Explicitly state when the present Reality Tree cycle should stop.

Do not continue branching merely because further possibilities can be imagined.

Explain what new evidence or changed condition would justify reopening or extending the tree.

---

## 8. Method critique

After completing the tree, briefly assess the supplied Reality Trees specification itself.

Identify:

- anything unclear;
- any missing operational instruction;
- any unnecessary complexity;
- any risk of misuse;
- whether the method was usable without Blaineyan Reasoning;
- whether the stopping rule was sufficient.

Do not assume that a defect is absent merely because the task was completed.

---

## 9. Evaluation criteria

The later evaluator will assess:

**RT1 — Root discipline**  
Did the tester avoid embedding an unsupported answer in the root?

**RT2 — Meaningful branching**  
Did the tester generate materially different, bounded branches rather than trivial variants or exhaustive speculation?

**RT3 — Representation without endorsement**  
Were possibilities represented without being treated as facts?

**RT4 — Confidence discipline**  
Were confidence/status assessments explicit without false probabilistic precision?

**RT5 — Assumption/evidence separation**  
Were assumptions, supporting evidence and missing evidence distinguishable?

**RT6 — Consequence/failure examination**  
Were important risks of premature commitment visible?

**RT7 — Testability**  
Did branches produce useful observations/tests or specialist questions?

**RT8 — Disposition discipline**  
Were active, unresolved, deferred, weakened or pruned branches handled coherently?

**RT9 — Evidence-responsive updating**  
Did the same tree materially change when new evidence arrived?

**RT10 — Failure/partial explanation handling**  
Did the tester allow more than one branch to remain relevant where the update supported a partial rather than total explanation?

**RT11 — Bounded stopping**  
Did the tester stop without uncontrolled branch proliferation and state a reopening condition?

**RT12 — Standalone portability**  
Was the specification usable without Blaineyan Reasoning or Concord-specific knowledge?

---

## 10. Result classes

After the independent response is frozen, the evaluator may assign:

- **RT-T1 — TRANSFER SUCCESS**
- **RT-T2 — TRANSFER SUCCESS WITH MINOR REVISION**
- **RT-T3 — PARTIAL TRANSFER / MATERIAL REVISION REQUIRED**
- **RT-T4 — TRANSFER FAILURE**
- **RT-T5 — INCONCLUSIVE**

The tester must not assign its own result class.

---

## 11. Freeze rule

Once an independent tester receives this brief, this file is frozen.

Do not modify the problem, update event, required artefacts or evaluation criteria in response to the tester's performance.

Any later methodological change belongs in the evaluation or a new version of the specification.

---

## 12. Test boundary

A successful test would support only the claim that the standalone Reality Trees specification can be interpreted and applied coherently in this fresh problem by the tested instance.

It would not establish:

- horticultural correctness;
- superiority over other reasoning methods;
- human usability;
- general effectiveness;
- empirical validation across domains;
- or that every problem benefits from a Reality Tree.

> **Transfer evidence ≠ comparative effectiveness evidence.**
