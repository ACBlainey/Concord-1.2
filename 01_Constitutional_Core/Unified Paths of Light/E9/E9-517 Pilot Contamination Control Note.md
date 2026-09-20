## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-517 — Pilot Contamination Control Note

The local Rattray OCR contains Twi and English together. During source retrieval in the present environment, both can appear in the same tool output.

### Risk
If the same model instance reads the historical English immediately before generating the candidate translation, the pilot is no longer genuinely blinded.

### Control
The translation candidate must therefore be produced from a source-only representation created before reference comparison.

Acceptable implementations include:
- extracting Twi-only rows into a temporary file;
- manually masking English fields;
- using a separate translation pass that receives only the Twi column.

### Current status
The pilot architecture and sample are frozen, but **no performance percentage is claimed yet**.

This is deliberate. Methodological cleanliness is more important than producing an immediate score.
