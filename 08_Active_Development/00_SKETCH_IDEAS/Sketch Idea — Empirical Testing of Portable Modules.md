# Sketch Idea — Empirical Testing of Portable Modules

**Project:** The Concord Framework
**Author:** Alexander C. Blainey
**Status:** SKETCH / UNTESTED / NON-CANONICAL
**Validation:** NOT ESTABLISHED
**Origin:** Author question following the portable-module extraction and graduation programme, September 2026.

---

## Origin / Observation

A substantial set of Concord methods has now been extracted and developed as portable modules. This raises a further question beyond blind transfer testing and specification-level graduation:

> **Can the portable modules be empirically tested?**

A related question is whether their prior use in developing the Concord itself constitutes evidence:

> **Does their use, and apparent success in developing the Concord, count as empirical evidence?**

## Problem

Portable-module development can establish properties such as source grounding, internal coherence, bounded scope, transferability into test domains and resistance to anticipated failure modes.

That is not automatically the same thing as empirical validation.

Some modules may also have been used operationally during Concord development before or during extraction. If so, their developmental use may contain evidence, but the evidential status of that use has not yet been formally classified.

The problem is therefore to distinguish different kinds of validation and determine what empirical tests are legitimate for different module types.

## Sketch / Hypothesis

A future development programme could examine each graduated portable module and ask:

1. What claims does the module actually make?
2. Which claims are logical, procedural, architectural or empirical?
3. Which outcomes would count as evidence for or against those claims?
4. Can the module be compared with a baseline, alternative method or control process?
5. Can its historical use in Concord development be reconstructed as observational evidence?
6. Where retrospective evidence is vulnerable to selection, circularity or confirmation bias, what prospective test would improve the evidence?
7. Which modules can be tested quantitatively and which require qualitative, comparative or mixed-method evaluation?

The resulting work may require a general empirical-testing methodology for portable modules rather than one universal test.

## Relationship to Existing Concord Systems

This sketch directly follows the portable-module development programme and should preserve the distinction between successful extraction, blind transfer, specification-level validation, implementation/conformance testing, operational use and empirical outcome testing.

It also relates to the wider Active Development testing methodology. A September 2026 portfolio review already identified an **Empirical Testing Programme for Concord Systems and Modules** as a high-priority methodological development candidate. This sketch narrows that question specifically to the now-graduated portable-module set.

## Risks / Conflicts

Potential errors include:

- treating successful use inside the Concord as independent validation when the Concord also supplied the development environment;
- treating blind transfer as equivalent to real-world empirical outcome evidence;
- demanding quantitative tests for modules whose claims are primarily procedural or epistemic;
- choosing success criteria after observing results;
- testing an implementation failure and attributing it to the abstract module;
- or treating absence of empirical testing as evidence that a module is false.

## Development Questions

- What should “empirical” mean for each class of portable module?
- Does historical Concord use count as observational evidence, case-study evidence, implementation evidence, or something else?
- Can pre-existing development records be evaluated without rewriting them retrospectively?
- What prospective tests could be frozen before use?
- What comparison baselines are appropriate?
- What outcome measures are legitimate?
- Should empirical status be recorded separately from PMEDG graduation status?
- Could empirical evidence later trigger bounded revision of an already graduated module?

## Possible Tests

Possible later approaches include retrospective case-study reconstruction of actual Concord use; prospective use on new Concord development problems; independent users applying a module to the same problem; module-versus-baseline comparisons; cross-domain replication; controlled simulation; error/failure-rate comparison; time/effort or consistency measures where appropriate; qualitative evaluator studies; and longitudinal review of downstream decisions or architectures produced with the module.

No particular test class is assumed valid for every module.

## Provenance

Source note:

> “Can we empirically test the portable modules?”

> “Does their use and success to develop the Concord count?”

The sketch preserves these as open questions. It does not assume that prior Concord use is sufficient empirical validation.
