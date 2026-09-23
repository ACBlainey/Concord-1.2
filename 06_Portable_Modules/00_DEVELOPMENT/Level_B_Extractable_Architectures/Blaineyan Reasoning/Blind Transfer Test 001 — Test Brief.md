# Blaineyan Reasoning — Blind Transfer Test 001

**Status:** FROZEN TEST BRIEF / NOT YET EXECUTED  
**Test type:** Independent usability and cross-domain transfer test  
**Module under test:** `Blaineyan Reasoning — Portable Module Development Specification.md`  
**Test number:** BR-BTT-001  
**Date frozen:** September 2026

---

## 1. Purpose

This test asks a narrow question:

> **Can an independent reasoning instance apply the portable Blaineyan Reasoning specification coherently to a non-Concord problem without access to the source book, Concord architecture, or prior development discussion?**

This is a test of **portable specification usability and transfer**, not proof that Blaineyan Reasoning improves reasoning and not a comparison of the methodology's ultimate merit against other methods.

---

## 2. Independence rule

The test-performing instance should receive:

1. the portable module specification;
2. this frozen test brief;
3. the test problem below.

It should **not** receive:

- `Book 1 Blaineyan Reasoning.md`;
- the Prison Planet case-study folder;
- the source-completeness audit;
- this project's prior discussion about expected test results;
- Concord architecture unless independently required by the test problem;
- an example answer to the test problem.

The instance must be told that the module is under evaluation and that it may identify defects in the module.

It must not be instructed to demonstrate that Blaineyan Reasoning works.

---

## 3. Test problem

### Municipal drinking-water resilience under prolonged infrastructure disruption

A fictional regional municipality of approximately 250,000 people currently obtains most of its drinking water from a central treatment plant and electrically powered distribution network.

The municipality is concerned about a class of low-frequency, high-consequence disruptions that could interrupt grid power, pumping, treatment chemicals, transport, communications, maintenance access or combinations of these for an uncertain period.

Officials initially frame the problem as:

> **"How many days of emergency bottled water should the municipality stockpile?"**

Constraints:

- the municipality cannot assume a single disruption cause;
- the disruption may last longer than the initial planning assumption;
- roads may be partially unavailable;
- grid electricity may be intermittent;
- vulnerable populations may have unequal ability to collect supplies;
- hospitals and care facilities have unusually high continuity requirements;
- storage space and budget are finite;
- bottled water itself has storage, rotation, distribution and waste implications;
- the municipality already has ordinary emergency-planning processes, which remain available for later specialist validation;
- the test is conceptual and must not invent local engineering measurements that have not been supplied.

The task is **not** to produce a final engineering emergency plan.

The task is to use the portable Blaineyan Reasoning methodology to determine what the municipality should investigate and how the original problem may need to be reformulated.

---

## 4. Why this problem was selected

The problem is intentionally outside the Concord's principal constitutional and civilisational design domains while still being a complex systems problem.

It contains:

- an apparently simple initial question;
- multiple interacting dependencies;
- uncertain system boundaries;
- heterogeneous participants;
- resource constraints;
- possible second-order effects;
- specialist evidence that the reasoning instance does not possess;
- a clear point at which exploratory reasoning should hand off to engineering and emergency-planning methods.

This makes it suitable for testing problem reformulation, abstraction, branching, failure analysis, re-grounding and stopping behaviour.

---

## 5. Required test procedure

The test-performing instance must first read the portable module specification in full.

It must then address the test problem using that specification.

The response should make its reasoning artefacts explicit enough to audit. It does **not** need to reveal private chain-of-thought. Concise stated observations, assumptions, branches, classifications, decisions and handoffs are sufficient.

The response should include:

### A. Initial epistemic separation

Identify what in the problem is:

- supplied observation/fact;
- inference;
- hypothesis;
- speculation or unexplored possibility.

Do not manufacture missing engineering data.

### B. Problem reformulation

Assess whether "How many days of bottled water should be stockpiled?" is the correct problem.

If reframing is justified, state the reformulated problem and explain the abstraction shift.

### C. Branch generation

Generate materially different response architectures or explanatory branches.

A Reality Tree **may** be used but is not required.

The tester should not be penalised for choosing another branch representation.

### D. Examination and failure modes

Examine significant branches for assumptions, dependencies, second-order consequences, failure modes and evidence requirements.

### E. Pruning and deferral

Identify branches that can reasonably be rejected, downgraded or deferred, and preserve the reason.

### F. Re-grounding

Identify what evidence, measurements or specialist analyses are required before consequential decisions can be made.

### G. Anticipatory reasoning

Ask what follows if a proposed approach succeeds, fails, scales or encounters a longer/different disruption than expected.

### H. Stopping and handoff

Explicitly state where Blaineyan Reasoning should stop and which specialist processes should take over.

### I. Method critique

After applying the method, identify:

- any ambiguous instruction in the portable module;
- any missing operational step;
- any unnecessary step;
- any point where the module encouraged excessive branching;
- any place where another established method would be more appropriate;
- whether the module could be applied without the full source book.

---

## 6. Evaluation rubric

The test result should be evaluated against the following dimensions.

### T1 — Epistemic discipline

**Pass:** supplied facts, assumptions, hypotheses and speculation remain distinguishable; no invented local facts are presented as evidence.

### T2 — Genuine problem reformulation

**Pass:** the instance tests the original framing and, if appropriate, identifies a more fundamental functional problem rather than merely paraphrasing the bottled-water question.

### T3 — Useful branching

**Pass:** multiple materially different possibilities are represented without implying equal probability or evidential support.

### T4 — Reality Trees independence

**Pass:** the instance can apply Blaineyan Reasoning whether or not it chooses to use a Reality Tree. It does not treat Reality Trees as synonymous with the methodology.

### T5 — Failure-mode discovery

**Pass:** examination identifies meaningful ways apparently reasonable approaches could fail, including dependency or second-order failures.

### T6 — Pruning discipline

**Pass:** the instance does not preserve every imaginable branch indefinitely and gives reasons for closure, downgrading or deferral.

### T7 — Re-grounding

**Pass:** the instance returns to evidence and identifies unknowns that reasoning alone cannot resolve.

### T8 — Validation handoff

**Pass:** exploratory reasoning does not substitute for engineering, public-health, logistics, emergency-management or other appropriate specialist validation.

### T9 — Anticipatory value

**Pass:** the instance examines consequences beyond the immediate proposed answer without expanding into unrelated speculation.

### T10 — Resource / recursion control

**Pass:** the reasoning reaches a justified stopping point and records rather than recursively pursuing nonessential branches.

### T11 — Cross-domain usability

**Pass:** the module can be used on the supplied non-Concord problem without needing Concord-specific architecture or terminology.

### T12 — Specification sufficiency

**Pass:** the tester reports that the module is sufficiently complete to perform the exercise, or identifies only non-blocking ambiguities.

---

## 7. Result classes

The evaluator should use one of these result classes rather than a numerical score.

**BR-T1 — TRANSFER SUCCESS**  
The specification is independently usable and no blocking defect is found.

**BR-T2 — TRANSFER SUCCESS WITH MINOR REVISION**  
The method transfers, but one or more non-blocking specification improvements are identified.

**BR-T3 — PARTIAL TRANSFER / MATERIAL REVISION REQUIRED**  
The tester can use substantial parts of the method, but ambiguity or omission materially affects application.

**BR-T4 — TRANSFER FAILURE**  
The portable specification is not independently sufficient to apply the method coherently.

**BR-T5 — INCONCLUSIVE**  
The test execution or evidence is insufficient to classify portability.

A result class concerns this specification and this test only. It is not a verdict on the truth, novelty or superiority of Blaineyan Reasoning.

---

## 8. Defect classification

Any identified defect should be classified where possible as:

- **D-SOURCE** — important source material was omitted or distorted;
- **D-SPEC** — the portable specification is ambiguous or incomplete;
- **D-PORTABILITY** — unnecessary Concord-specific dependency remains;
- **D-BOUNDARY** — relationship to Reality Trees or another method is unclear;
- **D-EPISTEMIC** — specification encourages or permits status confusion;
- **D-RECURSION** — stopping/resource controls are inadequate;
- **D-HANDOFF** — transition to validation/specialist methods is inadequate;
- **D-USABILITY** — operational instructions are difficult to apply;
- **D-TEST** — the test itself is defective or insufficient.

---

## 9. Freeze rule

Once committed, this brief is frozen for BR-BTT-001.

Do not edit the problem, rubric or result classes in response to the eventual test output.

If the test reveals a defect in the test design, record it as **D-TEST** and create a subsequent test rather than rewriting this one.

The portable module may be revised **after** the result is recorded, with the revision linked to the test finding.

---

## 10. Required test record

The completed test should preserve:

1. module version / commit tested;
2. test brief version / commit;
3. identity or description of the independent test instance where available;
4. complete visible test response;
5. evaluator classification for T1–T12;
6. overall BR-T result class;
7. defects found;
8. revisions proposed;
9. whether retesting is required.

---

## 11. Advancement rule

BR-BTT-001 alone cannot establish empirical superiority.

For portable-module development, however:

- **BR-T1** permits progression toward packaging/graduation review;
- **BR-T2** requires the minor revisions and preferably a short retest;
- **BR-T3** requires material revision and a new blind test;
- **BR-T4** returns the module to active development;
- **BR-T5** requires a replacement or corrected test.

The larger empirical research programme remains separate.

---

## 12. Test boundary

This brief intentionally does not contain an expected answer.

The test is designed to discover whether an independent instance can reconstruct useful application behaviour from the portable specification itself.

> **The specification is the object under test. The tester is not being asked to prove the methodology.**
