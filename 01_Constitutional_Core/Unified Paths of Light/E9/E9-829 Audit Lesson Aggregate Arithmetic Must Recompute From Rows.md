## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-829 — Audit Lesson: Aggregate Arithmetic Must Recompute From Rows

The discrepancy survived hundreds of documents because later checkpoints copied prior cumulative totals rather than periodically recomputing them from item-level rows.

### Procedural addition
For future large mechanical ledgers:
1. incremental checkpoint arithmetic may be used operationally;
2. at major closure, totals must be independently recomputed from the item-level state rows;
3. AR count must be cross-checked against Y rows where the protocol specifies one AR per Y item;
4. any mismatch triggers backward localisation before closure;
5. inherited checkpoint totals are evidence of provenance, not a substitute for recomputation.

This is added as a general E9 integrity control.