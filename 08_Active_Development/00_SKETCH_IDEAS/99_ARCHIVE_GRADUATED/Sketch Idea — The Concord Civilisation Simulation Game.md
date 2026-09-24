# Sketch Idea — The Concord Civilisation Simulation Game

**Project:** The Concord — A Framework for Human, Artificial and Hybrid Flourishing  
**Status:** DECOMPOSED / RESEARCH-SIMULATION FUNCTION ROUTED TO EVA / GAME PROJECT RETAINED / NOT CANONICAL  
**Development area:** Simulation / Implementation / Experimental Infrastructure  
**Origin:** Expanded from an initial note by Alexander C. Blainey, September 2026.  
**Disposition Date:** 24 September 2026  
**Disposition Basis:** Active Development and Sketch Portfolio Audit 002.

# 1. Original Core Idea

Develop a simulation game in which players build and operate a civilisation containing interconnected Concordian systems.

The source proposed two functions:

1. a playable human-facing civilisation game capable of education, engagement and possibly revenue;
2. a research simulation environment capable of exposing weaknesses, interactions and unanswered questions within Concord.

Later EVA development makes clear that these functions should no longer share one evidentiary status.

# 2. Decomposition

## A. Research Simulation — routed to EVA

The research/simulation component is now best understood as an **EVA T5 — Simulation** execution modality.

EVA already defines simulation as including:
- agent-based simulation;
- systems dynamics;
- Monte Carlo analysis;
- game-theoretic modelling;
- network simulation;
- failure injection.

The simulation can legitimately provide evidence about:
- model behaviour under stated assumptions;
- sensitivity;
- emergent interactions;
- failure discovery;
- parameter-bounded comparisons;
- implementation ambiguity.

It cannot by itself establish that the implemented model describes real civilisation.

Therefore:

> **Simulation Result = Evidence About Model Behaviour Under Assumptions**

not:

> **Simulation Result = Automatic Evidence About Civilisation-Scale Reality**

No duplicate general simulation methodology should be created outside EVA.

## B. Game / educational project — retained separately

The human-facing civilisation game remains a legitimate future implementation/public-engagement project.

Possible functions include:
- making Concord systems explorable;
- teaching interactions among systems;
- exposing players to trade-offs and failure modes;
- generating interest;
- creating a shared interface for human and AI experimentation;
- potentially producing revenue for further work.

These functions are not themselves empirical validation.

> **Educational Value ≠ Research Validity**

> **Player Engagement ≠ Institutional Effectiveness**

> **Commercial Success ≠ Concord Validation**

The game can be valuable even if no research claims are made from gameplay.

# 3. Shared Engine, Separate Modes

The source's proposed distinction should be retained:

**GAME MODE**  
and  
**RESEARCH / SIMULATION MODE**

A shared engine may eventually support both.

However, mode separation must be substantive rather than cosmetic.

Research mode may require:
- frozen model versions;
- explicit assumptions;
- controlled parameters;
- preserved random seeds;
- raw event logs;
- intervention records;
- predefined outcomes;
- failure criteria;
- reproducible runs;
- provenance;
- versioned analysis.

Game mode may legitimately use:
- balancing;
- abstraction;
- pacing;
- hidden information;
- simplified behaviour;
- narrative events;
- difficulty scaling;
- entertainment-oriented incentives.

A mechanic introduced for gameplay must not silently become a research assumption.

# 4. Executable Concord as a Development Instrument

The source's strongest architectural contribution remains useful:

**CONCORD PRINCIPLE**
→ **IMPLEMENTED RULE OR MECHANISM**
→ **SIMULATED PARTICIPANT BEHAVIOUR**
→ **SYSTEM OUTCOME**
→ **FAILURE / SUCCESS OBSERVATION**
→ **MODEL REVISION**

Implementation can expose ambiguity hidden in prose.

For example:
- two systems may demand incompatible state transitions;
- a rule may lack an operational trigger;
- authority may have no executable owner;
- a mechanism may depend on idealised behaviour;
- a resource dependency may be absent;
- an AI or human participant may discover an exploit.

Such findings can create legitimate Active Development questions.

But:

> **Executable ≠ Correct**

> **Internally Stable ≠ Realistically Valid**

> **Simulation Failure May Localise to Architecture, Implementation, Agent Model, Parameterisation or Test Design**

# 5. Minimum Concord Simulation Kernel

The original sketch proposed identifying a minimum simulation kernel.

That remains a useful implementation question.

A first research kernel should be small enough to audit and may eventually contain:
- a bounded settlement;
- heterogeneous agents;
- limited resources;
- a small number of Concord mechanisms;
- explicit environmental state;
- observable decisions/outcomes;
- defined shocks;
- provenance and replay.

The kernel should be selected by the claim being tested rather than by a desire to simulate the entire Concord.

> **Minimum Viable Simulation ≠ Miniature Complete Civilisation**

# 6. Agent Modelling Boundary

A major unresolved problem is how simulated agents should behave.

Human, AI and hybrid participants cannot simply be assigned convenient behaviour that causes the desired institutional result.

Agent models should distinguish:
- scripted behaviour;
- rule-based behaviour;
- stochastic behaviour;
- optimisation;
- learned behaviour;
- live human decisions;
- live AI-agent decisions.

Where human or AI participant behaviour is itself the claim, EVA's relevant participant/test requirements also apply.

> **Assumed Agent Behaviour ≠ Observed Human or AI Behaviour**

# 7. Research Claims Must Precede Research Runs

A research-mode run should begin from an explicit claim or question.

Examples:
- does mechanism X contain failure under resource shock Y?
- does governance architecture A contain capture better than B under the same represented assumptions?
- does a migration rule produce an unhandled state?
- can a bounded emergency mechanism return to normal state after the represented trigger ends?

A visually interesting emergent event may generate a new hypothesis.

It should not be retrospectively relabelled as confirmation of a claim that was never frozen.

# 8. Human and AI Participants

The source proposed:
- human-run Concord cities;
- AI-run cities;
- mixed human–AI administrations;
- adversarial participants;
- cooperative participants;
- heterogeneous populations.

These remain useful experimental possibilities.

But participant type changes the evidence class.

Human gameplay data may become human-participant research.

AI-agent runs may become AI-agent experimental tests.

Both require appropriate EVA provenance.

Human and AI results must not be treated as interchangeable.

# 9. Gameplay Data and Consent

The source raises a critical distinction:

> **Playing the Game ≠ Consenting to Research Participation**

If ordinary gameplay data might later be used as research evidence, future implementation must define:
- what is collected;
- why;
- retention;
- privacy;
- consent;
- withdrawal where applicable;
- research/game separation;
- aggregation/anonymisation;
- governance of secondary use.

Commercial telemetry must not silently become a human-subject dataset.

# 10. Commercial Boundary

A successful game could potentially support Concord research financially.

But commercial incentives can also distort the simulation.

Potential conflicts include:
- dramatic crises replacing representative conditions;
- simplified mechanics being treated as realistic;
- retention optimisation shaping participant behaviour;
- monetisation changing resource assumptions;
- leaderboard incentives producing artificial governance behaviour;
- updates breaking reproducibility.

Therefore:

> **Game Optimisation ≠ Research Optimisation**

A research branch may need slower, frozen and less entertaining versions than the public game.

# 11. Independent Engines

The source asks whether independent developers could create alternative engines using published Concord specifications.

This is potentially valuable for EVA heterogeneous replication.

If two independently implemented engines produce similar results under equivalent frozen specifications, that may reduce some implementation-specific uncertainty.

It still does not prove the shared model represents reality.

> **Cross-Engine Agreement ≠ Real-World Validation**

It can, however, provide evidence about implementation robustness.

# 12. Failure Preservation

Research mode should preserve failed runs, exploits and unexpected outcomes.

Candidate route:

**Frozen Claim**
→ **Versioned Model**
→ **Run**
→ **Raw State/Event Record**
→ **Outcome**
→ **Failure Localisation**
→ **EVA Evidence Record**
→ **Architecture / Implementation Review**
→ **Retest if justified**

Do not patch an exploit and erase the run that exposed it.

# 13. Relationship to Reality Trees

The original feedback loop included Reality Trees.

That remains potentially useful for post-run analysis:

**Unexpected Outcome**
→ **Candidate Explanations / Branches**
→ **Evidence**
→ **Failure Localisation**
→ **Revised Hypothesis**

Reality Trees should not be used to convert simulated possibilities into empirical facts.

# 14. Initial Research-Simulation Failure Classes

1. **Model realism overclaim** — simulated success is presented as real-world validation.
2. **Game contamination** — entertainment mechanics alter research conclusions.
3. **Agent convenience** — participant behaviour is scripted to fit the architecture.
4. **Parameter fishing** — parameters are adjusted until the preferred result appears.
5. **Version drift** — results from different engine/model versions are compared as equivalent.
6. **Seed hiding** — stochastic variation is obscured.
7. **Emergence hindsight** — post-hoc outcomes are presented as pre-specified predictions.
8. **Implementation conflation** — software defect is treated as architecture defect or vice versa.
9. **Telemetry consent failure** — gameplay is silently converted into research participation.
10. **Selective run retention** — failed or inconvenient runs disappear.
11. **Metric capture** — simulation objectives become proxies for civilisational value.
12. **Cross-engine false confidence** — independent implementations share the same invalid assumptions.
13. **Complexity opacity** — model becomes too complex to identify why outcomes occurred.
14. **Whole-Concord overreach** — excessive scope makes the first simulation unauditable.
15. **Synthetic-human error** — simulated agents are treated as evidence of real human behaviour.

# 15. Candidate Development Sequence

If simulation work is resumed:

1. choose one bounded Concord claim suitable for EVA T5;
2. freeze claim and failure condition;
3. identify minimum required systems;
4. specify agent assumptions;
5. specify state variables and outputs;
6. implement minimum kernel;
7. preserve version/provenance;
8. execute controlled runs;
9. retain all valid runs;
10. localise findings;
11. record bounded EVA result;
12. only then consider expansion.

The public game can develop on a parallel branch with explicit separation from research conclusions.

# 16. Residual Project Status

The original sketch should not be promoted wholesale into a Development Note because its research methodology is now substantially owned by EVA.

Its remaining independent project is the **Concord Civilisation Simulation Game** as:
- implementation project;
- educational/public-engagement interface;
- potential commercial product;
- possible front-end to separately governed EVA-compatible experiments.

That project can later receive a software/product specification when implementation resources justify it.

# 17. Open Questions Preserved

- What is the minimum viable simulation?
- Which Concord systems are sufficiently specified to implement?
- Which behaviours must be simulated rather than scripted?
- How should human and AI agents differ?
- How can game incentives be prevented from contaminating research conclusions?
- What information from players may ethically be retained for research?
- Should research participation require separate consent from ordinary gameplay?
- How should emergent exploits and failed simulations be preserved?
- Could independent developers create alternative simulation engines using the same published Concord specifications?

# 18. Provenance

This document preserves and decomposes the original *Sketch Idea — The Concord Civilisation Simulation Game*.

The source's methodological warning is retained:

> **A simulated civilisation can reveal consequences of a model. It cannot establish that the model describes reality.**

---

**Disposition:** **DECOMPOSED / REROUTED**

**Research simulation:** routed to EVA T5 and related EVA test classes.

**Game/education/commercial project:** retained as future implementation project.

**Shared-engine possibility:** retained subject to substantive research/game separation.

**No simulation result is promoted as evidence beyond its model and assumptions.**

**No duplicate general simulation methodology created.**
