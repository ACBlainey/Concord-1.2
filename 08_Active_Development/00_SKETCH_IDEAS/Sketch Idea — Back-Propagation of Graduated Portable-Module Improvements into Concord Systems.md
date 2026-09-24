# Sketch Idea — Back-Propagation of Graduated Portable-Module Improvements into Concord Systems

**Project:** The Concord Framework
**Author:** Alexander C. Blainey
**Status:** SKETCH / UNTESTED / NON-CANONICAL
**Validation:** NOT ESTABLISHED
**Origin:** Author observation following the portable-module extraction and graduation programme, September 2026.

---

## Origin / Observation

Many portable modules underwent additional development after extraction from their original Concord systems.

That development included clarification of boundaries, failure modes, transfer behaviour, safeguards and other revisions needed to make the modules portable.

The source Concord systems from which those modules were derived may therefore still contain earlier forms of the methods and may not include improvements discovered during portable-module development.

## Problem

Portable-module extraction was not necessarily a one-way copying process.

Where development after extraction produced a genuine improvement to a method, the graduated module may now contain knowledge that its original Concord implementation lacks.

This creates a possible divergence:

> **Original Concord Method → Portable Extraction → Testing / Revision → Improved Graduated Module**

without a corresponding:

> **Improved Graduated Module → Source-System Review → Appropriate Back-Propagation**

If left unresolved, Concord could continue using an older internal form of a method while simultaneously publishing a better portable form.

## Sketch / Hypothesis

Existing Concord systems should be systematically checked against the graduated portable modules derived from them.

For each graduated module:

1. identify its source Concord system or systems;
2. compare the graduated module with the current canonical/internal implementation;
3. identify changes introduced during portable-module development;
4. classify each change as portability-only, clarification-only, general improvement, failure-mode correction, interface improvement, or potentially source-specific;
5. determine whether the change is relevant to the original Concord system;
6. where relevant, route it through the appropriate Concord development/integration process rather than silently editing canonical architecture;
7. record changes that should not be back-propagated and why.

The objective is not to replace Concord systems with portable modules. It is to prevent useful knowledge discovered during extraction and testing from being stranded outside the systems that originally generated it.

## Relationship to Existing Concord Systems

This sketch concerns the interface between the graduated portable modules, their retained PMEDG development records, the canonical or active Concord systems from which they were extracted, and the ordinary Active Development/integration process.

It should preserve the rule that a portable module has a bounded owner and may deliberately omit Concord-specific machinery. Therefore not every portable-module difference is an improvement that belongs back in the source architecture.

## Risks / Conflicts

Potential errors include:

- automatically replacing richer Concord-specific architecture with a deliberately narrower portable abstraction;
- assuming every PMEDG revision is relevant to the source system;
- silently modifying canonical systems without source resolution and review;
- losing provenance between original method, portable extraction and later reintegration;
- creating circular references in which the source system and portable module are treated as independent evidence for one another;
- or failing to incorporate a genuine failure-mode correction because it was discovered outside the original development path.

## Development Questions

- Which graduated modules contain substantive post-extraction improvements?
- Which changes are portability adaptations only?
- Which changes correct a weakness that also exists in the original Concord implementation?
- What is the correct authority path for reintegration?
- Should a standard post-graduation back-propagation audit become part of PMEDG or remain a separate Concord integration method?
- How should version/provenance links be recorded after a source system incorporates a portable-module improvement?
- Should future module development automatically create a source-system review trigger at graduation?

## Possible Tests

A bounded first test could select one graduated module with well-documented post-extraction revisions, reconstruct its source-system form, enumerate changes introduced during PMEDG, independently classify which changes are portable-only versus generally applicable, inspect the current Concord source system for each generally applicable change, identify genuine reintegration gaps, and test whether the proposed audit method produces useful corrections without collapsing the portable/source boundary.

If successful, the method could be applied across the graduated portable-module portfolio.

## Provenance

Source observation:

> “Many of the portable modules had additional development work done to address failure modes etc.”

> “The existing methods they were derived from in the Concord systems do not have those new updates.”

> “Existing Concord systems need to be checked against graduated portable modules to ensure all new developments are incorporated.”

This sketch preserves that concern as a development task. It does not assume that every portable-module revision should automatically be incorporated.
