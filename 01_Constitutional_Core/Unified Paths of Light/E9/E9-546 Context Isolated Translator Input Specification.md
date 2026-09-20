## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-546 — Context-Isolated Translator Input Specification

A context-isolated translator receives only:

1. experiment identifier;
2. R-ID;
3. C-ID;
4. RAW Twi;
5. any pre-frozen NORMALISED Twi;
6. instruction to translate conservatively;
7. instruction to expose uncertainty.

It must not receive:
- Rattray English;
- Rattray commentary unless separately designated as source-language aid;
- E9 ethical classifications;
- AR records;
- X1–X7;
- expected ethical meaning;
- validation score.

### Required output
For each row:
- conservative English rendering;
- uncertain tokens/phrases;
- confidence;
- whether OCR appears materially damaged;
- no ethical interpretation.

This output is fixed before reference comparison.
