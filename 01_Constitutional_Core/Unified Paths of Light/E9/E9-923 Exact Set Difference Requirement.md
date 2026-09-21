## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-923 — Exact Set-Difference Requirement

To close E9-RX-2.0 without circularity, the audit now requires two machine-readable keyed sets:

**A — authoritative relation set:** all 820 admitted `(R-ID, C-ID)` edges reconstructed from the overlap ledgers plus reconciliations.

**B — Pass-001 parser set:** the 805 `(R-ID, C-ID)` edges actually recovered from the local witness.

Compute `A − B`. It must contain exactly 15 edges. Then collision-test those fifteen C-IDs against the unique IDs represented by B and one another.

Only this keyed comparison can establish the final unique cardinality directly.