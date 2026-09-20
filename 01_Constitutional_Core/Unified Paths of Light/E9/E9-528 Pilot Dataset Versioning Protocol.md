## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-528 — Pilot Dataset Versioning Protocol

The validation dataset is now treated as a versioned research object.

### Version fields
- sample version;
- source-recovery version;
- raw transcription version;
- normalisation version;
- candidate-translation version;
- reference-join version;
- scoring version.

### Freeze discipline
Once candidate translation begins, the source-only version used for that run is immutable.

Later source repairs may create a new run but must not silently alter the old one.

### Reason
This makes it possible to distinguish:
- translation error;
- OCR error;
- later source correction;
- scoring disagreement.

It also preserves reproducibility if E9 is independently audited.
