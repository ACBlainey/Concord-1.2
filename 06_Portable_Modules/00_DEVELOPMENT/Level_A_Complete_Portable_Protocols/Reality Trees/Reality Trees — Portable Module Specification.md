# Reality Trees — Portable Module Specification

**Author:** Alexander C. Blainey  
**Project of origin:** The Concord Framework  
**Module status:** PORTABLE SPECIFICATION CANDIDATE / BLIND TRANSFER TEST REQUIRED  
**Development level:** Level A — Complete Portable Protocol  
**Version:** 0.1  
**Date:** September 2026

---

## 1. Purpose

Reality Trees are a portable method for representing and examining multiple possible explanations, consequences or pathways arising from a present state without prematurely collapsing uncertainty into a single answer.

The method is intended to help a person, AI system or team:

- make meaningful alternatives visible;
- separate possibility from conclusion;
- expose assumptions and causal claims;
- represent uncertainty;
- examine consequences and failure modes;
- identify useful tests or next investigations;
- preserve unsuccessful branches as information;
- and revise the represented possibility space when evidence changes.

A Reality Tree does not determine truth by visualisation.

> **Reality remains the final arbiter.**

---

## 2. Core epistemic boundaries

A branch is a represented possibility, not automatically a conclusion.

> **Representation ≠ endorsement.**

> **Possibility ≠ truth.**

A branch may be strongly believed, weakly believed, uncertain, plausible but unsupported, disbelieved, actively dismissed, or deliberately retained as a devil's-advocate branch.

A branch can therefore be examined by asking:

> **If this were true, what would follow?**

without claiming that it is true.

---

## 3. Present state and root

Begin with a present state, observation, question or uncertainty.

The root should describe what is presently known or being examined without embedding an unsupported answer where practical.

Examples of root forms include:

- “Observed condition X has occurred; what might explain it?”
- “We need outcome Y; what materially different pathways could produce it?”
- “Condition Z may develop; what materially different consequences or responses should be considered?”

The root need not contain every relevant fact. It should be clear enough that branches can be related back to the same question or state.

---

## 4. The basic method

1. **Identify the present state.**
2. **Generate possible explanations, consequences, or pathways.**
3. **Branch where meaningful alternatives exist.**
4. **Examine the assumptions and causal relationships behind each branch.**
5. **Assess evidence, uncertainty, benefits, harms, and possible failure modes.**
6. **Test promising branches where practical.**
7. **Retain the results, including unsuccessful branches.**
8. **Refine the model as new evidence becomes available.**

The purpose is not exhaustive generation of every imaginable branch. Branches should be materially different enough to improve examination of the immediate uncertainty.

---

## 5. Branch representation

No mandatory visual notation is required.

A Reality Tree may be represented visually, as nested text, as a graph, or in a table, provided the relationship between the root and branches remains understandable.

A useful generic branch record is:

| Branch | Possibility / pathway | Current confidence or status | Key assumptions | Evidence / uncertainty | Consequences / failure modes | Test or next examination | Current disposition |
|---|---|---|---|---|---|---|---|

This table is an interface, not a requirement that every application fill every cell.

Sub-branches may be created where a branch contains materially different explanations, consequences or pathways that need separate examination.

---

## 6. Confidence and uncertainty

Branches may optionally receive confidence weightings.

A confidence weighting expresses the present degree of belief, support or plausibility assigned to a branch.

> **Confidence weighting ≠ objective probability.**

A numerical value such as 70% / 30% must not be presented as a statistically derived probability unless an appropriate probabilistic method actually supports that claim.

Qualitative states may be preferable where numerical precision would be misleading, for example:

- strongly supported;
- provisionally supported;
- uncertain;
- plausible but unsupported;
- weakly supported;
- currently contradicted;
- unresolved.

Confidence or status should be revisable when evidence changes.

---

## 7. Assumptions and causal relationships

For each important branch, identify assumptions that must hold for the branch to remain viable.

Where a branch asserts or depends upon a causal relationship, distinguish that causal claim from the observation that motivated the branch.

Questions may include:

- What must be true for this branch to work?
- What evidence currently supports it?
- What evidence challenges it?
- What remains unknown?
- What would follow if it were true?
- What would falsify, weaken or materially revise it?
- Does the branch depend on another branch?

Reality Trees make assumptions visible; they do not by themselves validate causal claims.

---

## 8. Consequences, benefits, harms and failure modes

Where relevant, examine what follows from each branch.

This can include:

- intended consequences;
- unintended consequences;
- benefits;
- harms;
- second-order effects;
- failure modes;
- dependencies;
- reversibility;
- information that would be gained even if the branch fails.

Not every cognitive tree requires a full risk analysis. Examination should be proportional to the question and consequence of action.

---

## 9. Testing and evidence

Promising branches should be tested where practical.

The source method recognises a possible progression:

> **Speculation → Simulation → Limited Pilot → Real-World Branch → Knowledge Integration**

This is a hierarchy of increasing engagement with reality, not a mandatory sequence for every tree.

A branch may stop at conceptual examination. Consequential experiments require whatever specialist, safety, ethical, legal, governance or domain-specific controls legitimately apply.

> **A Reality Tree can identify a test. It does not itself authorise the test.**

Evidence produced by testing should update the branch rather than be forced to fit the original expectation.

---

## 10. Branch disposition

Branches may remain:

- active;
- unresolved;
- selected for testing;
- deferred;
- weakened;
- contradicted;
- pruned;
- rejected for the present question;
- or retained as a devil's-advocate branch.

Pruning does not require deletion.

Where practical, retain the branch and the reason for its disposition.

> **Branch failure ≠ tree failure.**

An unsuccessful branch may still reveal assumptions, constraints, failure mechanisms or useful negative evidence.

---

## 11. Updating the tree

A Reality Tree is revisable.

New evidence may:

- change branch confidence;
- weaken or strengthen assumptions;
- prune a branch;
- reopen a previously rejected branch;
- create a new branch;
- merge branches that prove equivalent;
- split a branch into materially different sub-branches;
- or reformulate the root question.

Updating the tree is not evidence that the earlier model was useless. Revision is part of the method.

---

## 12. Stopping

Reality Trees are not a mandate for unlimited branching.

A bounded cycle may stop when:

1. the meaningful alternatives needed for the immediate question have been represented sufficiently;
2. important assumptions and uncertainties are visible;
3. promising branches have identifiable next examinations or tests where appropriate;
4. unsupported, deferred or rejected branches have a recorded disposition where useful;
5. further branching would add little material value without new evidence.

The tree can be reopened when new evidence, changed conditions or a new decision context warrants it.

---

## 13. Failure and misuse modes

### Premature collapse
Selecting one branch as certain before alternatives have been adequately examined.

### False equivalence
Treating all visible branches as equally plausible merely because they are represented.

### Confidence-as-probability error
Presenting subjective or evidence-relative confidence as objective mathematical probability.

### Branch proliferation
Generating possibilities without proportional examination, prioritisation or testing.

### Exploration-as-endorsement
Treating a speculative, dismissed or devil's-advocate branch as the user's belief.

### Visualisation-as-proof
Treating the existence or structure of a tree as evidence that a branch is true.

### Failure erasure
Deleting unsuccessful branches and losing what was learned.

### Evidence resistance
Protecting a preferred branch from revision when evidence contradicts it.

### Unsafe escalation
Moving from speculation to consequential real-world experimentation without appropriate safeguards, authority or specialist methods.

---

## 14. Documentation and provenance

For simple personal use, lightweight notes may be sufficient.

Where branches develop into consequential research, organisational or real-world experiments, preserve where practical:

- provenance;
- assumptions and methodology;
- reasoning and experimental rationale;
- confidence assessments;
- measured outcomes;
- unintended consequences;
- successful discoveries;
- unsuccessful discoveries;
- lessons learned.

The purpose is to allow the tree to learn from reality rather than merely accumulate branches.

---

## 15. Relationship to Blaineyan Reasoning

Reality Trees originated within the broader Blaineyan Reasoning approach and can support its exploration of multiple possibilities.

The relationship is:

> **Blaineyan Reasoning → may use → Reality Trees**

Reality Trees are not the whole Blaineyan Reasoning methodology.

They do not require Blaineyan Reasoning in order to function, and Blaineyan Reasoning does not require Reality Trees in every application.

Reality Trees provide a structured branch representation where such representation is useful.

---

## 16. Civilisational and organisational use

Reality Trees can scale beyond individual cognition.

Branches may represent competing designs, experimental pathways, environmental adaptations or other materially different approaches.

Where branches become real-world experiments, appropriately isolated failures can produce local learning rather than requiring global commitment.

This does not grant permission to create harmful or unaccountable experiments. The relevant organisation, community or domain retains responsibility for legitimate authority, safeguards and consequences.

---

## 17. Minimum input

A Reality Tree minimally needs:

1. a present state, observation, question or uncertainty;
2. at least two materially distinct possibilities, explanations, consequences or pathways worth representing.

Evidence, assumptions, constraints and confidence assessments improve the tree but need not all be available at the beginning.

---

## 18. Minimum output

A bounded Reality Tree cycle should leave enough information to understand:

- the root question or present state;
- the branches considered;
- important branch relationships;
- assumptions and causal claims examined;
- evidence and uncertainty;
- optional confidence/status assessments;
- important consequences or failure modes where relevant;
- which branches require testing or further investigation;
- which branches were pruned, rejected, deferred or remain unresolved;
- what was learned from any tests performed;
- and how the tree changed when evidence changed.

---

## 19. Scope and evidential status

Reality Trees are presented as a portable cognitive and experimental exploration method.

They are not presented here as:

- a complete theory of reasoning;
- a replacement for scientific or specialist methods;
- a Bayesian probability system;
- a formal causal-inference framework;
- a forecasting guarantee;
- a decision-authority mechanism;
- or proof that exploring more branches always improves outcomes.

The module has been source-extracted from the Concord architecture but has not yet completed its independent blind transfer test.

> **Portable specification candidate ≠ empirically validated method.**
