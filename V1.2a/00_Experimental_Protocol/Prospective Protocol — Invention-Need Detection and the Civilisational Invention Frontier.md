# Prospective Protocol — Invention-Need Detection and the Civilisational Invention Frontier

**Status:** V1.2a PROSPECTIVE EXPERIMENTAL PROTOCOL / FROZEN BEFORE CASE SEARCH  
**Date:** September 2026  
**Canonical effect:** NONE  
**Related frozen work:** Need–Invention Gap; Relational Grammar v1.0 H-G; Developmental Maturity Mapping; Solution Abstraction and Cross-Domain Reuse; Temporal Propagation Gaps; Architectural Unit Resolution v0.1

# 1. Research Question

Can a machine-readable civilisational topology identify, before failure occurs, not only a missing or vulnerable function but a position at which **new invention is required because no verified existing mechanism satisfies the derived functional specification**?

The strongest form of the claim is:

> A sufficiently developed civilisational model may be able to predict some future failure modes and identify the functional shape of inventions required to prevent them before those failures occur.

This protocol does not assume that the model can invent the solution itself.

It tests whether the model can identify an **invention target**.

# 2. Core Distinctions

The experiment must distinguish:

## State I — Existing Solution, Local Representation Missing

The apparent gap disappears when the relevant architecture is found.

## State II — Existing Distributed Solution, Interface Missing

Required capability exists but the affected system is not adequately connected to it.

## State III — Known Partial Solution

Existing mechanisms satisfy some but not all required constraints.

## State IV — Unresolved Functional Need

The topology derives a required function, but no verified current mechanism has yet been found that satisfies the specification.

## State V — Historical Invention Position

An earlier source records a need or failure condition before a later Concord invention appears that substantially satisfies it.

## State VI — Prospective Invention Frontier Candidate

A required capability is derived now, no satisfying existing mechanism is found after bounded adversarial search, and the missing capability can be specified sufficiently to guide invention/search.

Only State VI is a prospective invention-frontier candidate.

# 3. No-Invention Claim Rule

Failure to find a mechanism does not prove that none exists.

Therefore the model must not state:

“Invention is required.”

unless the evidential standard is explicitly bounded.

The safe formal status is:

**NO VERIFIED SATISFYING MECHANISM FOUND — INVENTION/EXTERNAL DISCOVERY CANDIDATE.**

Only after broad source closure and external-knowledge checks, where appropriate, may confidence increase.

ESCP remains active.

# 4. From Failure Prediction to Functional Requirement

For a candidate future failure mode F:

Reality/Trajectory
→ Dependency
→ Failure Condition
→ Consequence
→ Required Preserved Function.

Let the required function be Q.

Then derive:

Spec(Q) = {
  purpose,
  trigger,
  inputs,
  outputs,
  constraints,
  interfaces,
  affected participants,
  authority limits,
  failure tolerances,
  review,
  correction,
  continuity,
  provenance
}.

The topology should predict the **properties the solution must have**, not prematurely invent a mechanism.

# 5. Existing-Solution Test

For each candidate mechanism M_i:

Test:

M_i ⊨ Spec(Q)?

Classify each required property as:

- SATISFIED;
- PARTIAL;
- UNSATISFIED;
- UNKNOWN;
- NOT APPLICABLE.

If at least one existing architecture satisfies the required specification to the defined threshold:

→ not an invention gap.

If several mechanisms jointly satisfy it with adequate interfaces:

→ distributed solution.

If no known mechanism satisfies it:

→ candidate invention position.

# 6. The Invention Frontier

Define the current civilisational capability set:

C(t) = {verified available functions and mechanisms at time t}.

Define derived required capabilities:

Q(t+) = {functions predicted as necessary under identified future conditions or unresolved architecture}.

Then the provisional invention frontier is:

IF(t) = {q ∈ Q(t+) | no verified M ∈ C(t) satisfies Spec(q)}.

This does not mean every element requires a wholly unprecedented physical invention.

Possible resolutions include:

- new technical invention;
- new institutional architecture;
- new protocol;
- new mathematical method;
- new abstraction;
- new interface;
- new combination of existing capabilities;
- external discovery;
- environmental adaptation;
- removal of the dependency that created the need.

Therefore “invention” means **generation of a presently unavailable satisfying solution**, not necessarily patentable technology.

# 7. Predictive Failure Chain

A high-value invention-frontier candidate should expose a chain:

Current Architecture
→ Dependency / Constraint
→ Future or Conditional Failure Mode
→ Lost Required Function
→ Civilisational Consequence
→ Missing Capability
→ Functional Specification
→ Candidate Search / Invention Programme.

This allows research to begin before the failure occurs.

# 8. Prospective Predictions

If the model is valid:

### IN-1
Some documented Concord failure modes will map to already existing solutions and be rejected as invention gaps.

### IN-2
Some will map to later inventions or architectures that appeared after the need was first recorded.

### IN-3
For historical State-V cases, the topology should be able to reconstruct the required functional specification using only information available before the later invention is opened.

### IN-4
The later invention should satisfy a substantial fraction of that frozen specification without the specification being rewritten after inspection.

### IN-5
Some current needs will remain without a verified satisfying mechanism and therefore become prospective invention-frontier candidates.

### IN-6
Multiple apparently different local needs may collapse into one higher-order invention target.

### IN-7
Some apparent invention gaps will disappear when architectural-unit resolution or external solution search is performed.

### IN-8
The topology may predict classes of solution properties more reliably than specific inventions.

# 9. Historical Validation Test

For a candidate historical case:

1. choose an early source containing an unresolved need/failure;
2. hide later solution documents from the derivation step;
3. derive and freeze Spec(Q);
4. identify the later architecture/invention only after freezing;
5. test it against Spec(Q);
6. measure satisfied/partial/unsatisfied properties;
7. preserve mismatches;
8. compare chronology/provenance.

A successful historical case requires:

Need_t1
→ FrozenSpec_t1
→ LaterSolution_t2
→ HighSpecFit

with t2 > t1 in developmental provenance.

This tests prediction rather than retrospective storytelling.

# 10. Prospective Validation Test

For a current frontier candidate:

1. derive the failure chain;
2. freeze Spec(Q);
3. perform bounded Concord-wide search;
4. perform relevant external-state-of-the-art search where the claim concerns available real-world technology;
5. classify existing mechanisms;
6. if unresolved, register the invention target;
7. generate multiple candidate solution families without selecting a preferred implementation;
8. test candidates against the frozen specification;
9. preserve negative results;
10. revisit when new inventions appear.

# 11. Invention-Target Record

Each frontier entry should contain:

- Frontier ID;
- originating system(s);
- failure mode;
- trigger condition;
- time horizon if known;
- required preserved function;
- frozen functional specification;
- existing partial mechanisms;
- unsatisfied properties;
- dependencies;
- consequence if unresolved;
- candidate solution families;
- experiments/research routes;
- status;
- provenance;
- last re-test;
- confidence / ESCP note.

# 12. Priority Without Sovereignty

The invention frontier may expose urgency but must not become an autonomous authority for allocating civilisation's resources.

It may report dimensions such as:

- consequence magnitude;
- reversibility;
- dependency breadth;
- time sensitivity;
- number of systems affected;
- availability of fallback;
- uncertainty.

Human/constitutional decision processes remain responsible for prioritisation.

Visibility ≠ Sovereignty.

# 13. Relationship to Developmental Levelling

The invention frontier becomes especially important after an abstraction layer is levelled.

At L_n*:

known lower-level relations have been dispositioned.

Then abstraction may expose R_(n+1).

If:

R_(n+1)
→ RequiredCapability(Q)

and:

∀M ∈ C(t), M ⊭ Spec(Q),

then Q becomes a frontier candidate.

Thus:

L_n*
→ Abstract
→ New Relation
→ Predicted Failure / Need
→ Required Capability
→ Existing-Solution Test
→ Invention Frontier.

This is the proposed route by which a civilisation model could predict a need for invention before the corresponding failure is experienced.

# 14. Relationship to Generative Closure

The invention frontier also gives generative closure a detectable form.

Instead of merely asking:

“Can the civilisation invent?”

the topology can ask:

“Which required capability positions currently have no satisfying candidate?”

A civilisation may therefore know **where its search space is empty** even when it does not yet know how to fill it.

That converts an invisible generative limitation into a research object.

# 15. Critical Boundary

The topology does not prove that every predicted failure will occur.

It derives conditional statements:

If condition E occurs,
and dependency D remains,
and function Q is still required,
then current mechanisms do not yet demonstrate preservation of Q.

This is conditional structural prediction, not prophecy.

# 16. First Planned Historical Test

The first candidate historical validation case is:

**Civil Contact Point monopolisation / civil reachability**
versus later:
**Citizen ID + privacy-preserving logical routing + future communications architecture.**

The later solution material must not be used to modify the frozen required specification.

The test should ask whether the later communications architecture independently satisfies properties derivable from the earlier Contact Point problem.

# 17. Falsification / Weakening

The invention-frontier hypothesis is weakened if:

- functional specifications become obvious only after seeing later inventions;
- specifications are too generic to discriminate successful from unsuccessful mechanisms;
- nearly any invention can be made to “fit” retrospectively;
- most frontier candidates disappear under ordinary source search;
- the topology cannot distinguish missing integration from missing capability;
- predicted needs do not correspond to later solutions in historical tests;
- or the method generates so many candidates that it lacks useful selectivity.

# 18. Current Experimental Claim

The claim frozen here is deliberately limited:

> **A relational civilisational topology may be able to identify some conditional failure modes, derive the properties of the capabilities required to prevent or survive them, and distinguish cases where no verified existing mechanism currently satisfies those properties.**

If supported, this would create a civilisational **Invention Frontier**: a structured map not merely of unanswered questions, but of positions where the architecture predicts that new solution-generation effort is required.
