## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-865 — Spaced-Numeric Identifier Collision Audit

OCR spacing can split a valid C-ID, producing false duplicate candidates if fragments are searched independently. Two demonstrated cases are:

- R252 `(l 770)` → C1770, not C770;
- R629 `(1 359)` → C1359, not C359.

After normalisation, neither repair adds a new repeated C-ID. Similar spacing repairs must always be compared using the reconciled whole identifier rather than a visible suffix.