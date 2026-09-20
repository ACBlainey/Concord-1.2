## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-782 — Translation Validation Source Package Consolidation B

Continuation of the operational source-only recovery package. This preserves the recovery/audit record through the freeze of E9-TVP-SOURCE-v1.0. It is **not a candidate translation**.



---

## SOURCE DOCUMENT: E9-536 Pilot Frozen Sample Gap Audit.md

## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-536 — Pilot Frozen Sample Gap Audit

The 50-item list frozen in E9-511 has been compared against the source-only recovery documents.

### Recovered from the frozen list
The current dataset now contains exact source-only rows for all frozen items except those that were not yet mechanically recovered in the earlier construction pass:

R24, R153-related neighbouring sample status already recovered where listed, plus R205 etc.

A direct list reconciliation reveals that the original 50-item sample contains several items not yet present in the source-only documents:
- R24
- R153 is present
- R225 is present
- R286 and R291 are present
- R305 is present
- later rows through R825 are present.

### Immediate implication
Dataset version 1.0 must not yet be declared frozen until R24 and any other list mismatch found by final one-to-one reconciliation are resolved.

This audit intentionally treats the sample list, not the intended count, as authoritative.


---

## SOURCE DOCUMENT: E9-537 Pilot Source Identifier Anomaly Register.md

## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-537 — Pilot Source Identifier Anomaly Register

### R585
The OCR displays the parenthetical identifier as **B14**.

This is anomalous because the surrounding corpus normally uses numeric Christaller identifiers.

### Treatment
- retain RAW value B14;
- do not infer a numeric C-ID;
- mark identifier debt;
- inspect page image or independent witness before any alignment claim.

### Broader rule
A validation item's translation can still be tested using its Rattray number and source text, but an unresolved C-ID must not later be used for Christaller deduplication.

This separates translation validation from identifier reconstruction.


---

## SOURCE DOCUMENT: E9-538 Pilot Dataset One to One Reconciliation Protocol.md

## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-538 — Pilot Dataset One-to-One Reconciliation Protocol

Before source-only dataset v1.0 is frozen:

1. take the exact E9-511 sample list as the authority;
2. create a 50-row checklist;
3. require exactly one source-only row for each R-ID;
4. reject duplicates;
5. reject substitutions not documented by amendment;
6. require visible C-ID or explicit identifier-debt flag;
7. require RAW Twi or explicit source-access failure;
8. count populated rows mechanically.

### Freeze criterion
Dataset v1.0 is frozen only when:
- all 50 sample R-IDs have exactly one row;
- no undeclared replacement exists;
- all unresolved fields are explicitly marked.

The purpose is to avoid a nominal “50/50” result produced by accidental substitutions or omissions.


---

## SOURCE DOCUMENT: E9-539 Pilot Dataset Execution Status 002.md

## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-539 — Pilot Dataset Execution Status 002

### Progress this batch
Twenty-five additional exact source-only rows have been recovered in E9-531–535, including the previously unresolved R705.

### Important audit result
The source-only set is very close to completion, but final one-to-one reconciliation against E9-511 is still required before freezing version 1.0.

R24 is a known outstanding frozen-sample row from the present reconciliation.

R585 also carries an unresolved OCR identifier anomaly (“B14”).

### Translation status
Candidate translation has not begun.

This remains correct: source dataset completeness and identity are being proven before the blinded run starts.


---

## SOURCE DOCUMENT: E9-540 Christaller Expansion Checkpoint 057 Pilot Source Recovery Near Complete.md

## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-540 — Christaller Expansion Checkpoint 057: Pilot Source Recovery Near Complete

The second major source-only recovery pass is complete.

### Achievements
- 25 additional frozen-sample rows recovered;
- R705 gap resolved directly from source;
- late-corpus sample through R825 recovered;
- R585 identifier anomaly preserved rather than guessed;
- one-to-one reconciliation protocol frozen.

### Remaining gate
R24 is known to remain unrecovered in the source-only dataset, and a final exact checklist must confirm whether any additional mismatch exists.

### Next
Recover R24, perform the 50-row one-to-one audit, resolve or formally debt-flag the R585 identifier, and freeze source-only dataset v1.0.

Only after that may the candidate translation run begin.

No Christaller-only ethical classification has begun.

The E9 internal firewall remains closed.

# **CHECKPOINT 057 — SOURCE-ONLY PILOT DATASET NEAR COMPLETE; FINAL RECONCILIATION NEXT**


---

## SOURCE DOCUMENT: E9-541 Pilot Source Only Dataset R24 Recovery.md

## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-541 — Pilot Source-Only Dataset R24 Recovery

The outstanding R24 row has now been recovered.

### Local primary witness
The local OCR preserves the proverb text and C-ID but drops the printed Rattray number in this damaged section:

**Obosomfo ka ne nkonim, na ghka ne nkogtc. (624)**

### Independent reconciliation
Independent scans/OCR of the same Rattray edition explicitly identify this entry as:

**24. Obosomfo ka ne nkonim, na onka ne nkogu. (624)**

The surrounding numbered sequence also visibly gives R23/C621 and R25/C3285 in the independent witness.

### Source-only row

| R | C | RAW source-only Twi |
|---|---:|---|
| 24 | 624 | Obosomfo ka ne nkonim, na ghka ne nkogtc. |

### Status
R24 is recovered by source reconciliation, not bare sequential inference.


---

## SOURCE DOCUMENT: E9-542 R585 Identifier Reconciliation.md

## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-542 — R585 Identifier Reconciliation

The R585 identifier anomaly has been resolved.

### Local witness
The working OCR displays:

**R585 ... (B14)**

### Independent witnesses
Independent OCR representations of the same Rattray page identify the parenthetical number as:

**(814)**

and preserve the same proverb and Rattray number.

### Reconciled identifier
**R585 = C814**

### Dataset treatment
- RAW local identifier remains recorded as B14;
- reconciled C-ID = 814;
- repair basis = independent same-edition witness;
- confidence = high.

This satisfies the frozen rule permitting source-reconciled OCR repairs supported by independent evidence.


---

## SOURCE DOCUMENT: E9-543 Pilot Fifty Row Reconciliation Audit.md

## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-543 — Pilot Fifty-Row Reconciliation Audit

The E9-511 frozen sample has now been reconciled one-to-one against the source-only recovery set.

### Frozen sample
50 Rattray IDs.

### Result
- exact R-IDs represented: 50/50;
- duplicate R-ID substitutions: 0;
- undeclared replacements: 0;
- unresolved missing source rows: 0;
- R24 OCR numbering omission: reconciled;
- R585 identifier OCR anomaly: reconciled to C814.

### Authority
The sample list remains exactly:

R1, R14, R24, R27, R31,
R35, R41, R46, R54, R66,
R74, R95, R120, R153, R155,
R156, R160, R205, R225, R245,
R265, R286, R291, R305, R325,
R345, R365, R385, R405, R411,
R425, R445, R465, R485, R505,
R525, R545, R565, R585, R604,
R625, R645, R665, R685, R705,
R725, R745, R765, R785, R825.

### Gate
The source-only completeness gate is passed.


---

## SOURCE DOCUMENT: E9-544 Pilot Source Only Dataset Version 1 Freeze.md

## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-544 — Pilot Source-Only Dataset Version 1 Freeze

**Dataset version: E9-TVP-SOURCE-v1.0**

The 50-item source-only validation dataset is now frozen.

### Contents
Each item has:
- frozen R-ID;
- Christaller identifier;
- RAW Twi/source string;
- explicit source-reconciliation record where required.

### Repairs
- R24 identity restored through independent same-edition verification;
- R585 C-ID restored from local OCR B14 to C814 through independent same-edition verification.

### Immutability
The source strings used for a candidate translation run must not be silently changed.

Any later improved transcription creates a new source version and, if material, a new validation run.

### Status
**SOURCE-ONLY DATASET v1.0: FROZEN**


---

## SOURCE DOCUMENT: E9-545 Blinding Feasibility Audit.md

## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-545 — Blinding Feasibility Audit

A further methodological constraint is now explicit.

The current AI instance has retrieved sections of the primary witness in which Twi and Rattray English appear together.

Therefore this same conversational context cannot honestly serve as a fully blinded candidate translator for E9-TVP-SOURCE-v1.0.

### Consequence
Generating translations here and calling them “blinded” would overstate experimental independence.

### Valid execution routes
The candidate translation must be performed in a context that receives:
- E9-TVP-SOURCE-v1.0 only;
- no Rattray English;
- no previous E9 semantic classifications;
- no answer key.

Possible implementations include a fresh isolated AI context, an independent translator, or another reproducibly separated translation process.

### Rule
The present instance may prepare the experiment and later score fixed candidate outputs, but must not claim that its own post-exposure translations are blinded.


---

## SOURCE DOCUMENT: E9-546 Context Isolated Translator Input Specification.md

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


---

## SOURCE DOCUMENT: E9-547 Context Isolated Translator Prompt Freeze.md

## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-547 — Context-Isolated Translator Prompt Freeze

The translation instruction is frozen prospectively:

> Translate each Akan/Twi proverb into conservative English using only the source text supplied. Preserve who acts on whom, negation, modality, possession, authority, causality and evaluative force. Do not expand metaphors into moral lessons. If a token or construction is uncertain or appears corrupted, say so rather than guessing. Do not infer what ethical principle the proverb is intended to express. Return one translation and an uncertainty note for each item.

### Purpose
The prompt targets semantic preservation rather than literary fluency.

### Prohibition
The translator may not be told how Rattray translated the item or what E9 previously extracted from it.


---

## SOURCE DOCUMENT: E9-548 Translation Pilot Answer Key Isolation Protocol.md

## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-548 — Translation Pilot Answer-Key Isolation Protocol

The historical English layer now functions as the validation answer/reference set.

### Isolation
Before candidate output is fixed, the translating context must not receive:
- Rattray English;
- T1 English for the selected item;
- E9 paraphrases derived from those translations.

### After fixation
The scoring context may join:
- candidate translation;
- Rattray English;
- Rattray notes;
- T1/T3 where available.

### Important distinction
The reference is not treated as infallible ground truth.

It is an independent historical comparator whose disagreements are adjudicated under E9-516.

### Provenance
Candidate output must identify the isolated run/context used so that contamination can be audited.


---

## SOURCE DOCUMENT: E9-549 Translation Pilot Execution Gate 003.md

## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-549 — Translation Pilot Execution Gate 003

### Passed
- 50-item sample frozen;
- source-only recovery complete;
- one-to-one reconciliation complete;
- R24 repaired by independent witness;
- R585/C814 repaired by independent witness;
- dataset v1.0 frozen;
- translation prompt frozen;
- scoring rules frozen.

### Not passed inside this context
**Blinded translator independence.**

The present instance has already observed portions of the historical English answer layer.

### Decision
Do not manufacture a pilot score from a contaminated translation run.

The next valid experimental action is a context-isolated translation run using E9-TVP-SOURCE-v1.0 and the frozen E9-547 prompt.

Once those candidate outputs are fixed, this workflow can resume reference comparison and scoring.


---

## SOURCE DOCUMENT: E9-550 Christaller Expansion Checkpoint 058 Source Dataset Frozen Independent Translation Required.md

## Author, Copyright and Licence

© 2026 Alexander C. Blainey.

**Author:** Alexander C. Blainey — Independent Researcher
**Project:** The Concord Framework
**Licence:** Creative Commons Attribution 4.0 International (CC BY 4.0)

# Unified Paths of Light — E9

## E9-550 — Christaller Expansion Checkpoint 058: Source Dataset Frozen; Independent Translation Required

The 50-item pilot source dataset is complete and frozen as **E9-TVP-SOURCE-v1.0**.

### Closure of outstanding source issues
- R24 recovered as C624 through independent same-edition verification;
- R585 local OCR “B14” reconciled to **C814** through independent same-edition verification;
- 50/50 frozen R-IDs now represented exactly once.

### Experimental integrity finding
This AI context has already seen portions of Rattray's English during source retrieval.

It therefore cannot honestly generate a fully blinded candidate translation set.

### Next valid step
Run E9-TVP-SOURCE-v1.0 through a context-isolated translator using the frozen E9-547 instruction, fix the 50 candidate outputs, and return them for comparison against the historical reference layer.

### Experiment state
- source dataset: COMPLETE;
- candidate translations: NOT YET RUN IN AN INDEPENDENT CONTEXT;
- scoring: NOT STARTED;
- C-only extraction: NOT STARTED;
- X1–X7 firewall: CLOSED.

# **CHECKPOINT 058 — 50/50 SOURCE DATASET FROZEN; CONTEXT-ISOLATED TRANSLATION RUN REQUIRED**
