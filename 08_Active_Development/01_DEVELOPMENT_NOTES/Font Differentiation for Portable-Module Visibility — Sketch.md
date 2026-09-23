# Font Differentiation for Portable-Module Visibility — Sketch

**Status:** EARLY SKETCH / HOLD FOR LATER DEVELOPMENT  
**Area:** Portable modules / system legibility / machine-readable architecture  
**Date:** 23 September 2026

## Origin

A Concord system may be composed from multiple subsystems, portable modules and reasoning methods — for example Reality Trees, Blaineyan Reasoning and other reusable architectures.

At present, when reading a governance, judiciary or other system document, it may not be visible which module or method is operating in a particular section.

## Idea

Explore whether **very subtle typographic differentiation** could identify the module, method or architectural primitive being used within different parts of a Concord document.

The differentiation could potentially use slight variations in font or another typographic property.

The important possibility is that the distinction need not be visually prominent for a human reader. It could be subtle enough to leave normal reading largely unaffected while remaining reliably detectable by AI or machine analysis.

This could create an additional architectural information layer:

**Rendered text → subtle typographic marker → module identity → architectural provenance**

A reader or AI examining a complex system could therefore identify not only what the text says, but which reusable Concord mechanism is being instantiated by that section.

## Possible value

If workable, this may improve:

- visibility of module composition inside larger systems;
- architectural provenance;
- machine parsing of Concord documents;
- auditing of where particular modules are actually used;
- detection of missing or inconsistent module application;
- reconstruction of relationships between portable modules and larger systems;
- future automated topology mapping;
- legibility for AI instances working across the corpus.

It may also provide a way of preserving architectural metadata without repeatedly inserting intrusive textual labels into the prose.

## Questions for later development

The idea requires later investigation before any implementation decision.

Questions include:

- whether font variation is sufficiently robust across Markdown, GitHub, PDF, DOCX, web rendering and conversion;
- whether machine detection remains reliable after copying, reformatting or accessibility transformations;
- whether font differentiation should identify modules, methods, architectural layers or some combination;
- how collisions would be handled when several modules operate in the same passage;
- whether a non-visual metadata mechanism would be more reliable;
- whether human-visible labels or a hybrid visible/machine-readable system should accompany it;
- how the mechanism would preserve accessibility and avoid degrading ordinary readability;
- whether module identifiers should ultimately be standardised independently of their visual representation.

## Boundary

This is **not** a proposal to modify the current Concord formatting now.

It is an idea generated during portable-module development and should be retained for later investigation once the module set and its relationships are more mature.

> **Typographic Module Marker = Candidate Interface Idea, Not Current Standard**
