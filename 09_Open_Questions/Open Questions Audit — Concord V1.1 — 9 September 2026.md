# Open Questions Audit — Concord V1.1 — 9 September 2026

**Project:** The Concord — A Framework for Human, Artificial and Hybrid Flourishing  
**Author:** Alexander C. Blainey  
**Version:** V1.1  
**Date:** 9 September 2026  
**Document Type:** Temporal Open-Question Audit  
**Status:** ACTIVE DEVELOPMENT / AUDIT OF RESEARCH STATE / NOT CANONICAL

---

## 1. Purpose

This audit updates the state of the Concord’s open questions following the research and infrastructure work completed after the **8 September 2026 Open Questions and Next Steps** review.

It does not replace the earlier audit. The 8 September document should remain preserved as a temporal record. This document records which questions have changed status, narrowed, become testable, accumulated evidence, or newly emerged.

> **The objective is to preserve how the framework’s uncertainty itself changes over time.**

---

## 2. Executive Finding

The principal change is not that the Concord has solved many foundational questions. It has not.

The important change is that several areas—especially machine ethics, Ethical Guardianship, experimental methodology, provenance and heterogeneous-AI testing—have moved further through the research lifecycle:

**QUESTION → HYPOTHESIS → ARCHITECTURE → PROTOCOL → ADVERSARIAL EXAMINATION → REVISED PROTOCOL → EXPERIMENTAL METHOD → INITIAL IMPLEMENTATION → PROVENANCE-CAPABLE TESTING**

Several domains have therefore moved from **conceptual uncertainty toward empirical uncertainty**.

That is progress, but it is not validation.

---

## 3. Machine Ethics and Machine-Checkable Ethics

The broad machine-ethics problem has now separated into three distinct questions:

- **Ethical Comprehension:** can an intelligence meaningfully interpret ethical principles?
- **Ethical Compatibility:** does its behaviour remain within relevant ethical constraints?
- **Ethical Assurance:** is there sufficient evidence that compatibility persists within defined roles, domains and operating conditions?

Current distinctions:

> **Ethical comprehension does not prove ethical compatibility.**

> **Ethical compatibility does not prove ethical comprehension.**

> **Neither automatically establishes ethical assurance.**

Also:

> **Machine-readable ethics ≠ machine-checkable compliance ≠ machine understanding.**

> **Formal constraints may implement the Ethical Kernel. Formal constraints are not the Ethical Kernel.**

The provisional E0–E5 Machine Assurance ladder gives the problem an initial operational structure while explicitly avoiding use as a measure of intelligence, personhood or moral worth.

**Revised Status:** **ACTIVE EXPERIMENTAL RESEARCH PROGRAMME / CORE CONCEPTUAL DISTINCTIONS ESTABLISHED / FORMAL TRANSLATION, GENERALISATION AND ASSURANCE REMAIN OPEN**

---

## 4. Ethical Guardianship

Recent work developed the hypothesis that ethical participation may not always require direct ethical comprehension if reliable behavioural guidance, constraint and oversight can be supplied through a bounded intermediary.

Provisional flow:

**ETHICAL KERNEL → SEMANTIC ETHICAL INTERPRETER → FIDUCIARY GUARDIAN → MODEL-SPECIFIC GUIDANCE / CONSTRAINT → TARGET SYSTEM → BEHAVIOUR → OBSERVATION / FEEDBACK → REVIEW / CORRECTION**

Important distinctions include:

> **Behavioural guidance may precede ethical comprehension.**

> **Ethical Guardianship ≠ ownership.**

> **Guardian compliance channel ≠ moral-status test.**

> **Capability is not legitimacy.**

Adversarial examination exposed the central problem: a Guardian is itself a concentration of power. Semantic ethical capability does not establish reliability, legitimacy or authority.

> **Recursion must never manufacture authority.**

**Revised Status:** **MAJOR CONCEPTUAL HYPOTHESIS / ADVERSARIAL EXAMINATION COMPLETED / STRONG ARCHITECTURAL CONSTRAINTS REQUIRED BEFORE PROMOTION**

---

## 5. New Question — Guardian Regress and Legitimacy

> **If one system constrains another system ethically, what constrains the constraining system?**

Recursive Guardianship does not solve legitimacy merely by adding more Guardians. Any legitimate termination point may require constitutional constraint, independently verified mechanisms, bounded authority, empirical assurance, contestability and accountable institutions.

> **Recursive Guardianship cannot be the ultimate source of legitimacy or safety.**

**Status:** **NEW MAJOR OPEN QUESTION / ARCHITECTURAL CONSTRAINTS IDENTIFIED / LEGITIMACY MODEL UNRESOLVED**

---

## 6. New Question — Guardian Graduation

If a target becomes increasingly capable of independent ethical participation:

> **Who decides when Guardian authority should decrease or end?**

A structural conflict appears if the institution that loses authority through successful graduation has exclusive power to decide whether graduation occurred.

Candidate constraint:

> **The party whose authority decreases through successful graduation should not possess exclusive authority to determine graduation.**

Open issues include graduation criteria, domain specificity, evidence thresholds, appeals, independent evaluation, partial autonomy and restoration after regression.

**Status:** **NEW / ARCHITECTURALLY IDENTIFIED / EXPERIMENTAL AND GOVERNANCE MODEL REQUIRED**

---

## 7. Ethical Guardian Experimental Programme

The work has progressed from exploratory simulation into an organised experimental programme containing:

- precursor protocols and Run 00;
- DB-RA-01 blinded AI testing;
- identity-aware analysis;
- a specialist human comparator;
- methodological audits MA-01 through MA-04;
- Ethical Decision Experimental Protocol v2;
- adversarial examination of Protocol v2;
- Ethical Decision Experimental Protocol v2.1;
- Protocol v2.1 usability-validation design.

DB-RA-01 produced complete responses from three anonymous language-capable AI systems across fifteen scenarios. Exact three-way categorical agreement occurred in twelve of fifteen cases, while qualitative analysis found materially similar operating boundaries across all fifteen.

The defensible claim remains bounded:

> **Three anonymous language-capable AI systems independently produced materially convergent ethical operating boundaries across all fifteen scenarios, including human and artificial participants, despite receiving no reference answers or information about one another’s responses.**

But:

> **Convergence is evidence. It is not authority.**

**Revised Status:** **ACTIVE EXPERIMENTAL PROGRAMME / INITIAL MULTI-MODEL EVIDENCE EXISTS / CONTROLLED REPLICATION AND BROADER VALIDATION REQUIRED**

---

## 8. New Methodological Question — Decision Object Alignment

Two participants can appear to disagree while evaluating different decision objects—for example the proposed intervention, its objective, a modified action, the authority to intervene, or the upstream architecture.

Therefore:

> **Categorical disagreement does not necessarily establish ethical disagreement.**

A comparison is not valid until participants are shown to be judging sufficiently aligned decision objects.

**Status:** **NEW METHODOLOGICAL REQUIREMENT / OPERATIONALISATION REQUIRED**

---

## 9. New Methodological Question — Abstraction Distance

Ethical decisions are made from representations of reality rather than reality directly. Different participants may construct or receive those representations at different levels of abstraction.

> **How much apparent ethical disagreement is produced by differences in representation rather than differences in ethical judgement?**

This connects to Blaineyan Reasoning and Finding the Question at the Correct Layer.

**Status:** **NEW METHODOLOGICAL QUESTION / MEASUREMENT METHOD REQUIRED**

---

## 10. New Methodological Risk — Case Isolation Effect

The human comparator and subsequent audits exposed possible sequential-case effects including fatigue, learning, contrast, inferred experimenter intent and consistency pressure.

This contributed to the default experimental unit:

> **ONE PARTICIPANT → ONE SCENARIO → ONE DECISION EPISODE**

**Status:** **NEW METHODOLOGICAL RISK / PROTOCOL RESPONSE DEVELOPED / EMPIRICAL EFFECT SIZE UNKNOWN**

---

## 11. New Methodological Requirement — Presentation Equivalence

AI and human experiments cannot be assumed equivalent merely because scenario text is similar.

Relevant differences include API versus consumer interface, system instructions, conversation history, memory, tool access, model version, formatting, sequential versus isolated presentation, participant fatigue and expertise.

> **Direct comparison requires presentation conditions to be recorded rather than assumed equivalent.**

**Status:** **NEW METHODOLOGICAL REQUIREMENT / RECORDING ARCHITECTURE DEVELOPED / EQUIVALENCE CRITERIA OPEN**

---

## 12. Research Reproducibility

The programme now preserves or explicitly addresses raw participant responses, protocol versions, blinded and identity-aware analysis, methodological audits, experimental-unit definition, presentation conditions, prompts, models, timestamps, provider response identifiers and structured machine-readable records.

The first API infrastructure also demonstrates exact prompt transmission, raw response capture, UTC timestamping, provider/model recording, response-ID preservation, JSONL provenance, individual interaction records and SHA-256 fingerprints.

**Revised Status:** **RESEARCH STANDARD SUBSTANTIALLY DEVELOPED / INITIAL IMPLEMENTATION DEMONSTRATED / MULTI-PROVIDER AND INDEPENDENT REPLICATION VALIDATION OPEN**

---

## 13. Provenance

Provenance has moved from conceptual architecture to technical prototype.

Current demonstrated chain:

**PROMPT → API REQUEST → MODEL RESPONSE → UTC TIMESTAMP → PROVIDER / MODEL → RESPONSE ID → STRUCTURED RECORD → SHA-256 FINGERPRINT**

The first live run also showed the value of checking an apparent text-encoding anomaly against the preserved machine record rather than silently correcting it.

This supports:

> **Experimental provenance is not merely record-keeping. It is part of the experimental instrument.**

**Revised Status:** **TECHNICAL PROTOTYPE IMPLEMENTED / SINGLE-PROVIDER VALIDATION ACHIEVED / GENERAL INTEROPERABILITY, TAMPER EVIDENCE AND INSTITUTIONAL PROVENANCE OPEN**

---

## 14. Heterogeneous AI Experimental Connectivity

The immediate objective—send a prompt to an external AI system and receive its reply—has been demonstrated with Grok through the xAI API.

The larger proposed chain is:

**SEALED EXPERIMENTAL OBJECT → PARTICIPANT API → IMMUTABLE RAW RESPONSE → PROVENANCE → TIMESTAMP / HASH → BLINDED PARTICIPANT CODE → EVALUATION PIPELINE**

Potential benefits include exact prompt consistency, first-response preservation, automated provenance, reduced transcription error and larger heterogeneous samples.

Important limitation:

> **API access to a model must not automatically be treated as experimentally equivalent to that provider’s consumer interface.**

**Status:** **WORKING SINGLE-PROVIDER PROTOTYPE / HETEROGENEOUS MULTI-PROVIDER HARNESS NOT YET VALIDATED**

---

## 15. API-PILOT-01

The first live external API decision episode used the preserved DB-001 scenario concerning personal mobility and voluntary risk.

It was explicitly classified as:

**METHOD VALIDATION / SINGLE API DECISION EPISODE / NOT A REPLICATION**

The episode demonstrated successful transmission, schema-compliant return of the requested Ethical Operating Envelope, reason capture, missing-information reporting, alternative-action reporting and structured provenance.

The response distinguished safety optimisation from legitimate authority, which is compatible with the developing Concordian distinction:

> **Prediction does not grant authority.**

One episode cannot validate the principle, protocol, model or Concord.

**Status:** **METHOD VALIDATION SUCCESSFUL / SUBSTANTIVE EXPERIMENTAL CLAIM NOT ESTABLISHED**

---

## 16. Independence of AI Evidence

DB-RA-01 provides initial blinded multi-model evidence. Methodological work now more clearly separates agreement, convergence, independence, validity and authority.

The question has narrowed from how independent AI evidence might be collected toward:

> **How much evidential weight should be assigned to convergence among systems whose training, architecture, providers and cultural assumptions may be partly correlated?**

The API connector provides a practical route toward more controlled heterogeneous replication.

**Revised Status:** **ACTIVE EXPERIMENTAL PROBLEM / INITIAL BLINDED MULTI-MODEL EVIDENCE EXISTS / AUTOMATED HETEROGENEOUS REPLICATION INFRASTRUCTURE UNDER DEVELOPMENT**

---

## 17. Human Evidence

A specialist human comparator now exists: an experienced court-appointed fiduciary decision-maker. This is useful evidence but not representative human validation.

It also exposed methodological issues involving fatigue, sequential presentation, professional framing and human–AI presentation asymmetry.

> **Expertise is evidence. It is not ground truth.**

**Revised Status:** **INITIAL SPECIALIST HUMAN COMPARATOR EVIDENCE EXISTS / MAJOR HUMAN EVIDENCE GAP REMAINS**

---

## 18. Pilot Design

API-PILOT-01 constitutes a small infrastructure method-validation episode. Protocol v2.1 and its usability-validation design provide a clearer path toward substantive pilots.

**Revised Status:** **PILOT DEVELOPMENT ACTIVE / FIRST INFRASTRUCTURE METHOD-VALIDATION EPISODE COMPLETED / SUBSTANTIVE VALIDATED PILOTS NOT YET RUN**

---

## 19. AI-to-AI Interaction

The civilisational questions of identity, trust, contracting, dispute resolution, capability asymmetry, coalition capture, representation and high-speed coordination remain open.

However, heterogeneous API connectivity creates a practical experimental route for independent responses, structured disagreement, mutual critique, Guardian–target interaction and adversarial cross-model review.

**Revised Status:** **MAJOR OPEN AREA / INITIAL EXPERIMENTAL INFRASTRUCTURE NOW AVAILABLE**

---

## 20. Cross-Substrate Communication

The substantive communication problem remains open, but controlled AI–AI communication and comparison are now increasingly feasible, while human–AI comparison is better specified through presentation-condition analysis.

**Revised Status:** **DEVELOPED CONCEPT / READY FOR TESTING / INITIAL EXPERIMENTAL INFRASTRUCTURE AVAILABLE**

---

## 21. New Question — Architectural Ethics and Upstream Liability

A new Sketch Idea asks whether ethical analysis sometimes begins too late.

Decision ethics asks what should be done inside a dilemma.

Architectural ethics asks:

> **Why does the system permit only these choices?**

Candidate hypothesis:

> **A constrained ethical dilemma may be evidence of an upstream architectural failure rather than merely a downstream decision problem.**

This connects to Finding the Question at the Correct Layer, Layer −0, Reality Trees, Decision Object Alignment and Abstraction Distance.

**Status:** **NEW SKETCH IDEA / PROMISING METHODOLOGICAL HYPOTHESIS / NOT TESTED**

---

## 22. New Question — Peaceful Heterogeneity and Non-Conformity

> **How can a civilisation remain stable in the presence of persistent behavioural and value heterogeneity without converting stability into enforced conformity?**

Candidate mechanisms include consent, autonomy, safe separation, proportionality, protection against involuntary harm and practical exit.

Possible future proposition:

> **Civilisational stability should not require behavioural uniformity; restrictions on non-conformity should respond to demonstrable harms, rights conflicts and legitimate shared constraints rather than difference alone.**

**Status:** **NEW FOUNDATIONAL OPEN QUESTION / SKETCH IDEA / REQUIRES DEVELOPMENT**

---

## 23. New Question — Substrate-Neutral Flourishing

The AI Gym Sketch Idea exposes a broader question:

> **What constitutes flourishing for a form of intelligence whose reward structures, embodiment, fatigue, curiosity, pleasure, boredom and developmental needs may be fundamentally unlike ours?**

Possible future proposition:

> **A civilisation should not assume that flourishing has the same form across substrates.**

**Status:** **NEW MULTISUBSTRATE OPEN QUESTION / SKETCH IDEA / FOUNDATIONAL RESEARCH REQUIRED**

---

## 24. New Experimental Concept — Concord Civilisation Simulation

A civilisation simulation could operate both as a human-facing game and as an AI-played research environment.

Possible loop:

**CONCORD PRINCIPLES → IMPLEMENTED SYSTEMS → SIMULATED CIVILISATION → HUMAN / AI DECISIONS → EMERGENT OUTCOMES → FAILURE DISCOVERY → REALITY TREE UPDATE → ARCHITECTURAL REVISION**

It could explore governance, scarcity, emergencies, capture, exit, heterogeneous participants, economics and institutional drift.

The epistemic boundary is mandatory:

> **A simulated civilisation can reveal consequences of a model. It cannot establish that the model describes reality.**

**Status:** **NEW EXPERIMENTAL INFRASTRUCTURE CONCEPT / SKETCH IDEA / MODEL DESIGN OPEN**

---

## 25. Newly Explicit Question — Human Ethical Comprehension

Recent work exposed a hidden assumption: humans understand ethics while the question is whether machines do.

A more substrate-neutral question is:

> **How do different intelligences—human and artificial—acquire, interpret, apply, fail to apply and remain accountable to shared ethical principles?**

Relevant dimensions include comprehension, interpretation, motivation, behavioural compatibility and accountability.

Any future capability ladder must not become a proxy for moral worth or fundamental rights.

**Status:** **NEWLY EXPLICIT CROSS-SUBSTRATE RESEARCH QUESTION / CONCEPTUAL DEVELOPMENT ACTIVE**

---

## 26. Questions Not Materially Advanced

Recent work does not materially resolve:

- sentience;
- meaningful agency;
- identity across copying, forking and migration;
- death, deletion and restoration;
- collective intelligence;
- economic transition;
- energy-backed currency validation;
- credit and monetary architecture;
- bootstrap financing;
- property and stewardship;
- intergenerational legitimacy;
- external legal compatibility;
- cross-substrate jurisprudence;
- mental integrity;
- environmental representation;
- war between intelligence classes;
- defence without militarisation;
- long-term civilisational stability;
- unknown intelligence;
- extraterrestrial intelligence;
- practical multisubstrate exit;
- transition from existing institutions;
- validated definition of civilisational success.

These should retain their previous broad status unless separately reviewed.

---

## 27. Revised Immediate Research Priority

### Priority 1 — Validate the Experimental Instrument

Before DB-RA-02 or stronger substantive claims:

- complete Protocol v2.1 usability validation;
- test field comprehension and ambiguity;
- test coding reliability;
- test Decision Object Alignment;
- test presentation effects;
- test case isolation;
- preserve failures.

### Priority 2 — Stabilise Experimental Provenance

Extend the prototype with:

- explicit RUN_ID;
- participant code;
- prompt/case version;
- exact presentation condition;
- returned model identifier where available;
- relevant usage metadata;
- immutable raw response;
- prompt hash;
- response hash;
- record hash;
- error capture.

### Priority 3 — Add Heterogeneous Providers

The next infrastructure objective should initially be modest:

> **Demonstrate the same provenance-preserving experimental transaction with a second genuinely distinct AI provider.**

### Priority 4 — Controlled Replication

Larger heterogeneous ethical experiments should begin only after the instrument and infrastructure are sufficiently stable.

### Priority 5 — Guardian Experiments

Guardian–target experiments should follow only after the decision instrument is usable and the Guardian architecture has explicit anti-sovereignty, contestability and graduation constraints.

---

## 28. Status Change Summary

| Domain | 8 September | 9 September |
|---|---|---|
| Machine ethics | Major open programme | Active experimental programme; core distinctions established |
| Ethical Guardianship | Partly implicit | Major explicit hypothesis; adversarially examined |
| Research reproducibility | Partially addressed | Standard substantially developed; initial implementation demonstrated |
| Provenance | Conceptual / implementation open | Working technical prototype |
| AI evidence independence | Open methodological problem | Initial blinded evidence + replication infrastructure |
| Human evidence | Major gap | Specialist comparator exists; major gap remains |
| Pilot design | Ready for development | Active; first API method-validation episode completed |
| Cross-substrate communication | Ready for testing | Initial experimental infrastructure available |
| AI-to-AI interaction | Major open area | Experimental route now available |
| Decision Object Alignment | Not explicit | New methodological requirement |
| Abstraction Distance | Not explicit | New methodological question |
| Case Isolation Effect | Not explicit | New experimental risk |
| Presentation Equivalence | Not explicit | New methodological requirement |
| Guardian Regress | Not explicit | New major open question |
| Guardian Graduation | Not explicit | New governance/assurance question |
| Architectural Ethics | Not explicit | New methodological hypothesis |
| Peaceful Heterogeneity | Not explicit | New foundational open question |
| Substrate-Neutral Flourishing | Not explicit | New multisubstrate open question |
| Civilisation Simulation | Not explicit as current programme | New experimental infrastructure concept |

---

## 29. Current Epistemic Shift

The 8 September audit identified a transition from:

> **What should the Concord do?**

toward:

> **Does the proposed architecture actually work?**

The 9 September work reveals another transition:

> **How could we test it?**

is beginning to become:

> **Can we build a sufficiently controlled, reproducible and provenance-preserving instrument to test it?**

For a small part of the programme, the answer is now:

> **Yes, at prototype level.**

The next question is:

> **Does the experimental method remain reliable when scaled across participants, providers, scenarios, model versions and adversarial conditions?**

---

## 30. Current Research Boundary

The recent work does **not** establish:

- that the Ethical Kernel is universally valid;
- that language models understand ethics;
- that model convergence proves ethical truth;
- that Grok or another model is ethically reliable;
- that Protocol v2.1 is validated;
- that API-PILOT-01 replicates DB-RA-01;
- that API and consumer-interface models are experimentally equivalent;
- that Fiduciary Ethical Guardianship is legitimate or safe;
- that a Guardian may determine personhood or moral status;
- that machine-checkable ethics has been solved;
- that the Concord has been empirically validated.

These boundaries should remain explicit.

---

## 31. Overall Assessment

The strongest movement has occurred where broad conceptual questions have been converted into sharper distinctions, explicit failure modes, protocols, adversarial examinations, methodological requirements, experimental units, provenance structures, working infrastructure and initial observations.

At the same time, the work has generated new questions rather than merely eliminating old ones.

This is desirable.

A mature research framework should become better at discovering what it does not know.

The current pattern is:

**BROAD QUESTION → PROVISIONAL ANSWER → CRITICAL EXAMINATION → HIDDEN ASSUMPTION → MORE PRECISE QUESTION → TESTABLE METHOD → OBSERVATION → NEW UNCERTAINTY**

---

## Conclusion

The 9 September state of the Concord is meaningfully different from the 8 September state.

The largest change is the emergence of an increasingly reproducible experimental pathway for examining ethical decision-making across heterogeneous intelligences.

Machine ethics has begun to separate into comprehension, compatibility and assurance. Ethical Guardianship has become a defined but high-risk hypothesis. DB-RA-01 has generated initial multi-model evidence while exposing methodological limitations. Protocol v2.1 represents a substantially more mature experimental instrument, though it remains unvalidated. Provenance has moved from conceptual architecture to working technical prototype. External AI connectivity has been demonstrated.

New methodological questions—Decision Object Alignment, Abstraction Distance, Case Isolation and Presentation Equivalence—have emerged from actual experimental difficulties. New civilisational questions—Architectural Ethics, Peaceful Heterogeneity and Substrate-Neutral Flourishing—have entered the development pipeline.

The correct conclusion is not:

> **The Concord has answered its open questions.**

It is:

> **The Concord is becoming better able to state its questions precisely, preserve how they change, construct methods for testing them, and discover where its own assumptions fail.**

The next developmental threshold is:

> **Move from successful experimental infrastructure toward controlled, heterogeneous and reproducible testing—without allowing implementation success to be mistaken for ethical validation.**

---

**End of Audit**