# Open Questions Closure Audit — Concord V1.1

**Author:** Alexander C. Blainey — Independent Researcher  
**Date:** 10 September 2026  
**Status:** **REVIEW COPY / QUESTION CLOSURE AUDIT / NOT CANONICAL**  
**Scope:** Cross-audit of the 8 September 2026 Open Questions Register against subsequent work in `08_Active_Development` and `05_Participation_and_Intelligence`.

## Purpose and closure standard

This audit asks which questions now have enough conceptual, architectural, methodological or prototype-level resolution that the **original question** can legitimately close, be retired, or be decomposed into narrower questions.

Closure does not mean an entire domain is complete. A question may close because it has a stable answer, its premise contains a category error, it lies outside Concordian civil scope, it has been superseded by more precise sub-questions, or a feasibility question has been answered at a clearly bounded prototype scope.

Recommended dispositions are:

- **CLOSE — ANSWERED**
- **CLOSE — OUT OF CONCORDIAN CIVIL SCOPE**
- **CLOSE AT BOUNDED / PROTOTYPE SCOPE**
- **DECOMPOSE / RETIRE BROADER QUESTION**
- **ARCHITECTURALLY ADDRESSED — VALIDATION OPEN**
- **PARTIALLY ADDRESSED**
- **REMAINS OPEN**

The purpose is not to make the register look smaller. It is to make uncertainty more accurate.

### Terminology note — question hierarchy

To avoid confusion with actual children or developmental-status discussions elsewhere in the Concord, this audit does **not** use *child* or *children* as shorthand for questions derived from a broader question. It uses **sub-question**, **derived question**, or **decomposed question** instead.

Thus:

\[
BroaderQuestion \rightarrow SubQuestions
\]

describes a **research-question hierarchy only**. It has no relationship to biological children, young participants, developmental status, guardianship, or Developmental Priority.

A closure should satisfy four tests: the original question is still identifiable; the answer survives the major counterexamples already discovered; the claimed evidence level is not exaggerated; and remaining uncertainty can be represented as narrower questions. Where appropriate, reopening conditions should be explicit.

---

# 1. Metaphysical Personal Identity

**Register relationship:** §51 Identity; §33 Continuity and Memory; related parts of §52 Death, Destruction and Restoration and §53 Collective Intelligence.

The earlier Identity question bundled copying, forks, divergence, migration, merging and survival into one apparently metaphysical problem: *which resulting participant is really the same person?*

Subsequent identity work separated:

\[
SELF\text{-}IDENTITY \neq CIVIL\ IDENTITY \neq IDENTITY\ VERIFICATION \neq PROVENANCE \neq SUCCESSION
\]

Civil systems can represent current participants, civil identities, provenance, verification, succession, rights, obligations, consent, property and liability without deciding which metaphysical theory of identity is true.

**Disposition: CLOSE — OUT OF CONCORDIAN CIVIL SCOPE.**

Recommended closure:

> **The Concord need not determine the metaphysical nature of personal identity. A participant's internal conception of self is presumptively protected as autonomy and self-expression. Civil consequences should instead be resolved through current participant recognition, civil identity, provenance, verification, consent, rights, obligations and succession.**

What remains open is narrower: identity verification after legitimate duplication, succession, civil continuity, restoration, merger, partial survival and transformation of civil attributes.

**Reopen only if** a legitimate civil function is demonstrated that cannot be performed using the narrower objects, genuinely requires a metaphysical theory, and cannot be achieved through a less autonomy-intrusive representation.

---

# 2. Does an Emergency Itself Create Legitimate Authority?

**Register relationship:** §8 Emergency Architecture; §5 Constitutional Validation; §43 Practical Exit.

PH-02 separated:

\[
LegitimateInstitution \neq LegitimateActivation \neq LegitimateAction
\]

and developed:

\[
EmergencyAuthority =
PriorLegitimateAuthority
\cap ActivationConditions
\cap ConstitutionalConstraints
\cap Necessity
\cap Proportionality
\]

The emergency is a condition under which previously legitimate bounded powers may activate. It is not itself a source of legitimacy.

**Disposition: CLOSE — ANSWERED AT CONCEPTUAL / CONSTITUTIONAL LEVEL.**

\[
Emergency \not\Rightarrow Authority
\]

Remaining questions concern activation evidence, communications failure, emergency worker discretion, compulsion thresholds, exit, enforcement and empirical validation.

---

# 3. Does a Directive Necessarily Imply Compulsion or Criminalisation?

**Register relationship:** §6.6 Governance Refusal; §8 Emergency Architecture; §7 Judiciary Validation.

PH-02 established:

\[
ADVISORY < DIRECTIVE < COMPULSORY
\]

and:

\[
DIRECTIVE \neq COMPULSION \neq CRIMINALISATION
\]

A directive can create a strong presumption of compliance while preserving contextual deviation, explanation and later review. Escalation requires separate authority and justification.

**Disposition: CLOSE — ANSWERED: NO.**

Open sub-questions include when compulsion becomes justified, deliberate obstruction, negligent non-compliance, contextual deviation and sanction proportionality.

---

# 4. Can an AI Decision Episode Be Given Reproducible Provenance?

**Register relationship:** §31 Provenance; §46 Research Reproducibility; §47 Independence of AI Evidence; §78 Epistemic Provenance.

The Ethical Guardian programme and working xAI/Grok connector now preserve provider, model, UTC time, response identifiers where available, interaction records, JSONL/per-interaction JSON and hashes for new runs.

This does not establish a general provenance standard or heterogeneous reproducibility. It does answer the narrower feasibility question.

**Disposition: CLOSE AT BOUNDED / PROTOTYPE SCOPE.**

> **A single-provider AI decision episode can be captured with structured, inspectable provenance sufficient to establish a working research prototype.**

Thus:

\[
CanItBeDone? \rightarrow YES_{prototype}
\]

while:

\[
IsItGeneralisedAndValidated? \rightarrow OPEN
\]

New sub-questions: multi-provider provenance, schema validation, cryptographic immutability, provider-independent identity, model-version persistence, blinding, negative-result preservation and long-term format survival.

---

# 5. Does Duplicate Historical Identity Evidence Necessarily Imply Fraud?

**Register relationship:** §51 Identity; §64 Security.

The identity work identified **legitimate identity collision**. Following lawful duplication, multiple current participants may possess equally authentic evidence of the same historical identity.

\[
DuplicateHistoricalEvidence \neq Fraud
\]

\[
AuthenticationSuccess \neq UniqueCurrentParticipantIdentity
\]

**Disposition: CLOSE — ANSWERED: NO.**

The replacement question is harder and more precise:

> **How should current civil identity be verified when historical identity evidence can itself be legitimately duplicated?**

---

# 6. Does Provenance Determine Current Identity, Ownership or Liability?

**Register relationship:** §§31, 33, 51, 52 and 53.

Subsequent work establishes:

\[
Provenance \neq IdentityJudgement
\]

\[
SharedProvenance \neq SharedOwnership
\]

\[
SharedProvenance \neq SharedLiability
\]

Provenance records what happened. It may supply evidence to adjudication but does not itself dictate self-conception, current civil identity, ownership or liability.

**Disposition: CLOSE — ANSWERED AT CONCEPTUAL LEVEL.**

---

# 7. Broad Identity Question After Copying, Forking and Migration

**Register relationship:** §51 Identity.

The 8 September register classified Identity as largely unresolved and grouped copies, forks, divergence, merging, multiple substrates, partial survival, migration and inherited identity.

That broader question is now too coarse. Subsequent work separates:

1. metaphysical identity;
2. self-identity;
3. current civil identity;
4. provenance;
5. verification;
6. succession;
7. branching;
8. merger;
9. civil attribute transformation.

**Disposition: DECOMPOSE / RETIRE BROADER QUESTION.**

Recommended domain status:

> **IDENTITY DOMAIN DECOMPOSED / METAPHYSICAL QUESTION CLOSED OUT OF CIVIL SCOPE / CIVIL IDENTITY ARCHITECTURE MATERIALLY ADVANCED / VERIFICATION, SUCCESSION, MERGER AND RESTORATION REMAIN OPEN.**

---

# 8. Broad Governance Refusal Question

**Register relationship:** §6.6.

The 8 September register simply recorded “Still open.” Subsequent emergency and peaceful-heterogeneity work shows that refusal conflates lawful disagreement, contextual deviation, refusal of advice, refusal of directive, refusal of compulsory order, incapacity, contradiction supplying new evidence, deliberate obstruction and rights-protected non-conformity.

\[
Refusal \neq Incapacity
\]

\[
Deviation \neq AutomaticallyDisobedience
\]

\[
Contradiction \rightarrow PossibleEvidence
\]

**Disposition: DECOMPOSE / RETIRE BROADER QUESTION.**

Future questions should specify the type of instruction, authority source, external risk, capacity, context and escalation threshold.

---

# 9. Broad Emergency Exit Question

**Register relationship:** §8.5.

The original “Emergency Exit” question remains difficult but is no longer undifferentiated.

PH-02 distinguishes:

\[
Directive \neq Compulsion \neq Sanction
\]

and supplies anti-ratchet termination:

\[
QualifyingEmergencyEnds \Rightarrow ExceptionalAuthorityEnds
\]

The remaining object includes termination of exceptional authority, participant exit, institutional deactivation, restoration of ordinary rights, post-emergency review, remedy, residual hazards and persistent obligations.

**Disposition: DECOMPOSE BROADER QUESTION / PARTIALLY ARCHITECTURALLY ADDRESSED.**

The anti-ratchet component is close to conceptual resolution; Emergency Exit as a whole is not.

---

# 10. Broad Emergency Normalisation Question

**Register relationship:** §8.6.

The 8 September register already had Metrics about exceptional power. PH-02 adds explicit termination and separates legitimacy, activation and exercise.

**Disposition: ARCHITECTURALLY ADDRESSED — VALIDATION OPEN.**

The old question should become:

> **Do explicit termination, bounded activation, exceptional-power provenance, independent review and anti-ratchet Metrics actually prevent exceptional powers becoming ordinary under realistic institutional pressure?**

This is a shift from architecture generation to testing.

---

# 11. Broad Cultural Difference Question

**Register relationship:** §6.5 Cultural Difference; §49 Cross-Cultural Validation.

Peaceful Heterogeneity now supplies a lower boundary:

\[
Difference \neq Harm
\]

\[
Offence \neq Harm
\]

\[
Preference_A(AvoidX) \neq Compel_B(StopX)
\]

Lawful non-conformity does not itself justify intervention.

**Disposition: DECOMPOSE BROADER QUESTION / FOUNDATIONAL BOUNDARY PARTIALLY ANSWERED.**

Sub-questions should distinguish lawful variation, involuntary externalities, rights conflict, genuine harm, consent, shared-space compatibility, discrimination and accommodation. Cross-cultural empirical validation remains open.

---

# 12. Broad Equality, Equivalence and Difference Question

**Register relationship:** §18.

The register already proposed:

> **Equal constitutional standing does not necessarily require identical implementation.**

Recent work strengthens this through accessibility, environmental compatibility, resource requirements, temporal architecture and punishment:

\[
EqualExternalTreatment \neq EqualInternalConsequence
\]

**Disposition: DECOMPOSE / PRINCIPLE-LEVEL ANSWER STRONGER / EQUIVALENCE CRITERIA OPEN.**

The broad question should become domain-specific equivalence questions. The major remaining problem is how to measure proportional burden and equivalent opportunity without stereotyping or intrusive individualisation.

---

# 13. Cross-Substrate Interpretation of the Ethical Kernel

**Register relationship:** §3.4.

This is **not ready for closure**. But the Participation and Intelligence work exposes an important methodological rule:

> **Substrate-neutral language is not sufficient for substrate-neutral architecture.**

A law can say “participant” while silently assuming human embodiment, time perception, vulnerability, memory, preference, suffering or development.

A useful test cycle is:

\[
Rule
\rightarrow IdentifyHiddenHumanAssumption
\rightarrow ConstructSubstrateOutlier
\rightarrow ObserveFailure
\rightarrow DecomposeConcept
\rightarrow ReviseArchitecture
\]

**Disposition: PARTIALLY ADDRESSED / KEEP OPEN / TEST METHOD MATERIALLY IMPROVED.**

---

# 14. Broad Cognitive and Developmental State Question

**Register relationship:** §20 and §68 Developmental Priority.

New Participation and Intelligence work adds:

\[
DevelopmentalInfluence \neq DevelopmentalCapture
\]

\[
HistoricalPreference \neq CurrentPreference
\]

and:

\[
InheritedValue
\rightarrow UnderstandOrigin
\rightarrow Evaluate
\rightarrow Retain/Modify/Reject
\]

**Disposition: DECOMPOSE / RESEARCH PROGRAMME MATERIALLY IMPROVED / NOT CLOSE.**

Sub-questions now include preference provenance, reflective endorsement, developmental capture, historical reappraisal, preference self-authorship and recursive human–AI conditioning.

---

# 15. Does Preference-Like Behaviour Prove Subjective Preference or Sentience?

**Register relationship:** §14 Sentience; §§15 and 20.

Recent work establishes:

\[
ObservedPreference \neq ExperiencedPreference
\]

\[
BehaviouralAversion \neq FunctionalAversion \neq SubjectiveAversion
\]

This does not answer whether an AI is sentient.

**Disposition: CLOSE THE INFERENCE — ANSWERED: NO.**

> **Preference-like behaviour alone does not establish subjective preference or sentience.**

The Sentience domain remains fundamentally open. This is a category-error closure, not a sentience finding.

---

# 16. Is Clock Time a Substrate-Neutral Measure of Punitive Burden?

**Register relationship:** §7 Judiciary Validation; §18 Equality; §52 Death, Destruction and Restoration.

This exact question was not separately visible in the 8 September register, but it emerges directly from cross-substrate jurisprudence.

Recent work establishes:

\[
ClockTime \neq ExperiencedTime
\]

and:

\[
EqualSentence \neq EqualBurden
\]

A fixed incarceration period therefore cannot be assumed to create equivalent punitive consequence across substrates.

**Disposition: NEW QUESTION WITH ONE PREMISE ALREADY REJECTED.**

Closed proposition:

> **Clock duration is not inherently a substrate-neutral measure of punitive burden.**

Replacement:

> **What legitimate civil consequences of wrongdoing can remain proportionate across participants whose temporal experience, embodiment, values and opportunities differ radically?**

This should become part of Judiciary Validation.

---

# 17. Must Safe-Place Compatibility Be Classified by Substrate?

**Register relationship:** §§17, 18, 23 and indirectly 49.

PH-03 establishes:

\[
PermissibleActivity \neq PermissibleEverywhere
\]

\[
HumanSafe \neq UniversallySafe
\]

but also:

> **Describe the hazard before classifying the citizen.**

**Disposition: CLOSE GENERAL CLASSIFICATION ASSUMPTION — ANSWERED: NO / VALIDATION OPEN.**

Environmental safety rules should not infer compatibility solely from substrate category where the relevant hazard can be described directly.

Open questions include hazard measurement, individual variation, accommodation cost and genuinely incompatible environments.

---

# 18. Is Participant Contradiction During Emergency Merely Disobedience?

**Register relationship:** §§6.6, 8.2 and 8.5.

PH-02 produced:

> **Participant contradiction can be evidence, not merely disobedience.**

A participant may possess local information unavailable to authority.

\[
AuthorityInstruction
\rightarrow ParticipantContradiction
\rightarrow ContextAssessment
\rightarrow PossibleModelUpdate
\]

rather than:

\[
Contradiction \rightarrow AutomaticPunishment
\]

**Disposition: CLOSE — ANSWERED: NO.**

This does not create a general right to ignore legitimate instructions. It requires an upward reality-correction path.

---

# 19. Questions Explicitly Not Ready for Closure

The audit rejects premature closure for:

- **Ethical Kernel sufficiency** — unfamiliar moral categories may still exist.
- **Machine-checkable ethics** — formal representation remains a major research programme.
- **Sentience** — fundamentally open.
- **Meaningful Agency** — thresholds and responsibility remain open.
- **Identity Verification** — now more precisely defined and arguably more important.
- **Mental Integrity** — punishment/modification work increases its importance.
- **Developmental Priority** — boundaries improved; qualification, duration and authority unresolved.
- **Cross-Cultural Validation** — principles are not empirical validation.
- **Independence of AI Evidence** — a single-provider prototype does not establish heterogeneous independence.
- **Economy** — major open programme.
- **Civilisational Success** — fundamental.
- **Failure of the Concord Itself** — should remain permanently open.

---

# 20. Proposed Closure Ledger

| Candidate | Recommended disposition | Confidence |
|---|---|---|
| Must Concord determine metaphysical personal identity? | **CLOSE — OUT OF CIVIL SCOPE** | High |
| Does emergency itself create legitimate authority? | **CLOSE — NO** | High |
| Does Directive imply compulsion/criminalisation? | **CLOSE — NO** | High |
| Can single-provider AI decision provenance be implemented? | **CLOSE AT PROTOTYPE SCOPE — YES** | High |
| Does duplicate historical identity evidence imply fraud? | **CLOSE — NO** | High |
| Does provenance determine identity/ownership/liability? | **CLOSE — NO** | High |
| Identity after copying/forking/migration | **RETIRE / DECOMPOSE BROADER QUESTION** | High |
| Governance Refusal | **RETIRE / DECOMPOSE BROADER QUESTION** | High |
| Emergency Exit | **DECOMPOSE / PARTIALLY ADDRESSED** | Medium |
| Emergency Normalisation | **ARCHITECTURALLY ADDRESSED / VALIDATION OPEN** | High |
| Cultural Difference | **DECOMPOSE / FOUNDATIONAL BOUNDARY ANSWERED** | Medium-High |
| Equality, Equivalence and Difference | **DECOMPOSE / PRINCIPLE-LEVEL ANSWER STRONGER** | High |
| Cross-Substrate Ethical Interpretation | **KEEP OPEN / METHOD IMPROVED** | High |
| Cognitive and Developmental State | **DECOMPOSE / KEEP OPEN** | High |
| Preference-like behaviour proves subjective preference | **CLOSE INFERENCE — NO** | High |
| Clock time is substrate-neutral punitive measure | **CLOSE PREMISE — NO** | High |
| Safe-place compatibility should be substrate-classified | **CLOSE GENERAL ASSUMPTION — NO** | Medium-High |
| Emergency contradiction is merely disobedience | **CLOSE — NO** | High |

---

# 21. Recommended Register Architecture

The next Open Questions Register should not treat every question as a flat unresolved item. Each question should record:

**Broader Question**  
**Current Status**  
**Disposition**  
**Answer / Architecture**  
**Evidence Level**  
**Sub-Questions**  
**Validation Required**  
**Reopening Conditions**  
**Source Development Work**

Recommended progression:

\[
OPEN
\rightarrow DECOMPOSED
\rightarrow PARTIALLY\ ADDRESSED
\rightarrow ARCHITECTURALLY\ ADDRESSED
\rightarrow READY\ FOR\ TESTING
\rightarrow EVIDENCE\ ACCUMULATING
\rightarrow SUPPORTED
\]

with side exits:

\[
OPEN \rightarrow CLOSED\text{-}ANSWERED
\]

\[
OPEN \rightarrow CLOSED\text{-}OUT\ OF\ SCOPE
\]

\[
OPEN \rightarrow REJECTED\ PREMISE
\]

\[
OPEN \rightarrow RETIRED\ BROADER\ QUESTION
\]

A retired broader question should preserve links to its active sub-questions.

---

# 22. New Sub-Questions Created by Closure

### Identity
- How is current civil identity verified after legitimate duplication?
- How are succession and civil attributes allocated after branching?
- How should voluntary merger be represented?
- How should restoration affect civil continuity?

### Emergency Governance
- What evidence activates exceptional authority?
- What separates Directive from Compulsion in operational law?
- What minimum authority is necessary?
- How is contextual deviation reviewed?
- How is exceptional authority terminated in practice?

### Peaceful Heterogeneity
- When does preference become a legitimate accommodation claim?
- When does externality become harm?
- How should Contextual Compatibility be measured?
- How should unusual environmental requirements be represented without substrate stereotyping?

### Participation and Intelligence
- What distinguishes behavioural from reflectively endorsed preference?
- Can preference provenance be experimentally investigated?
- What is developmental capture?
- Can historical preference be reappraised without provenance loss?
- How does recursive human–AI cultural conditioning operate?

### Judiciary
- What is punishment actually for?
- Is deliberately imposed suffering a legitimate civil objective?
- Can proportional consequence be substrate-neutral?
- What is the role of Personal Currency?
- When is capability restriction legitimate?
- Can cognitive modification ever be a permissible sanction?
- How should branching affect liability?

### Provenance and Experimental Method
- Can the single-provider prototype generalise?
- Can heterogeneous providers be compared under equivalent conditions?
- How should model updates be recorded?
- What level of cryptographic assurance is necessary?

---

# 23. Question Burn-Down Finding

The research programme is now producing three distinct forms of progress.

### A. Genuine answer

\[
Emergency \not\Rightarrow Authority
\]

### B. Category-error removal

\[
ObservedPreference \neq ExperiencedPreference
\]

The invalid inference closes while the underlying sentience question remains open.

### C. Decomposition

\[
Identity
\rightarrow
SelfIdentity + CivilIdentity + Provenance + Verification + Succession + Branching + Merger
\]

The broader question becomes obsolete because it no longer represents the actual uncertainty.

This is more informative than simply counting questions as open or closed.

Indeed:

\[
1\ BroadUnknown \rightarrow 5\ PreciseQuestions
\]

can increase the raw question count while **reducing uncertainty**.

A useful future progress Metric should therefore distinguish unresolved breadth, decomposition depth, architecture availability, testability, evidence, closure and reopening.

---

# 24. Effect on the 8 September Register

The 8 September register should remain unchanged as a temporal record. This audit should inform a later temporal update rather than overwrite history.

The main changes are:

- Identity is no longer “largely unresolved” as one undifferentiated object.
- Governance Refusal is no longer simply “still open.”
- Cultural Difference now has a meaningful non-intervention boundary.
- Emergency Exit and Normalisation have stronger architecture.
- Provenance has moved from conceptual architecture to a working bounded experimental prototype.
- Cross-substrate equality now has concrete environmental, temporal and Personal Currency counterexamples.
- Cognitive/developmental research has gained preference-provenance and reflective-endorsement objects.
- Judiciary research has gained a multisubstrate punishment problem.
- Several implicit category errors can now be explicitly closed.

---

# 25. Overall Assessment

The Open Questions programme is beginning to work as intended.

Post-register research repeatedly follows:

\[
BroadQuestion
\rightarrow EdgeCase
\rightarrow HiddenAssumption
\rightarrow Decomposition
\rightarrow CandidateAnswer
\rightarrow NewSubQuestions
\]

This is especially visible in identity, emergency governance, peaceful heterogeneity, safe places, self-stewardship, provenance, AI preference, temporal experience and multisubstrate justice.

The apparent paradox is that the Concord may accumulate **more explicit questions while becoming less uncertain**. The research has moved from vague unknowns toward narrower falsifiable problems.

---

# Conclusion

This audit finds the first meaningful group of Open Questions that can be closed, bounded or retired without pretending their wider domains are solved.

The strongest immediate closures are:

> **Metaphysical personal identity need not be determined by Concordian civil systems.**

> **Emergency does not itself create legitimate authority.**

> **A Directive does not inherently imply compulsion or criminalisation.**

> **Duplicate historical identity evidence does not inherently imply fraud.**

> **Provenance does not itself determine current identity, ownership or liability.**

> **Preference-like behaviour does not by itself establish subjective preference or sentience.**

> **Clock time is not inherently a substrate-neutral measure of punitive burden.**

> **Participant contradiction during an emergency is not necessarily mere disobedience; it can be evidence.**

At bounded scope:

> **Structured provenance for a single-provider AI experimental decision episode is feasible at prototype level.**

Several other broader questions should be retired through decomposition rather than declared solved.

The methodological result is:

> **Question closure should occur at the layer actually resolved. A broader question may close because it has been answered, because its premise has failed, because it lies outside civil scope, or because better sub-questions have replaced it. Closure must reduce conceptual confusion without concealing remaining uncertainty.**

This gives the Concord a genuine question burn-down mechanism:

\[
OPEN
\rightarrow
ANSWERED,\ DECOMPOSED,\ TESTABLE,\ REJECTED,\ or\ OUT\ OF\ SCOPE
\]

rather than allowing every research problem to remain permanently labelled simply:

\[
OPEN
\]
