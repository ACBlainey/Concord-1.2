## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-773 — LoC Canvas-Enumeration Boundary

The LoC collection result establishes image ordinals 1–172, but an ordinal such as `sp=12` is a viewer locator, not automatically the IIIF image-service identifier.

### Frozen rule
Do not synthesize a tile.loc.gov identifier from `43019087`, `gdc.43019087`, `gdclccn.43019087`, or the image ordinal. Only an identifier directly emitted by LoC metadata/manifest may enter an image-service request.

This blocks a subtle form of source fabrication at the infrastructure layer.