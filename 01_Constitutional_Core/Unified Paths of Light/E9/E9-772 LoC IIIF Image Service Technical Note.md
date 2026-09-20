## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-772 — LoC IIIF Image-Service Technical Note

Library of Congress documentation confirms its IIIF image service pattern:

`https://tile.loc.gov/image-services/iiif/{identifier}/info.json`

and image retrieval through the same identifier plus region/size/rotation/quality/format components.

### Consequence for E9
Once a Christaller canvas exposes its LoC image-service identifier, page bytes can be requested independently of the interactive viewer. The missing link is therefore the **canvas/image identifier**, not uncertainty about the IIIF service itself.

No identifier is guessed from the bibliographic LCCN.