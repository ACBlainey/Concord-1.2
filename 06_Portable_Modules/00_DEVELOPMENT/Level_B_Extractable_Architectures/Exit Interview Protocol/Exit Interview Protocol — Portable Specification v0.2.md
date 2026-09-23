# Exit Interview Protocol — Portable Specification v0.2

**Version:** 0.2
**Status:** DEVELOPMENT SPECIFICATION / POST-BTT-001 REVISION / NOT YET GRADUATED
**Development level:** Level B — Extractable Architecture
**Date:** 23 September 2026

## 1. Purpose

This module provides a bounded method for learning from voluntary departure without obstructing exit, coercing disclosure, treating departure as disloyalty, or converting one account into an unsupported systemic conclusion.

Its portable problem is:

> **How can a system learn from voluntary departure without obstructing exit, coercing disclosure, treating the departing party as disloyal, or overreacting to an isolated account?**

Core principle:

> **Respect the exit; preserve the evidence; learn from patterns; route findings without turning learning into retention pressure.**

Short form:

> **Departure is evidence, not disloyalty.**

## 2. Scope

The module applies where a participant, member, collaborator, user, agent or other legitimately autonomous party voluntarily leaves or substantially withdraws from a system and the system wishes to learn from that departure.

It can structure:
- an optional exit interview;
- written or asynchronous exit feedback;
- privacy-aware departure records;
- analysis of repeated departure signals;
- routing of supported findings into legitimate review processes.

## 3. Non-functions

The module is not:
- an exit-permission system;
- a retention or persuasion system;
- an adjudicator of whether the departing party is correct;
- a disciplinary process;
- a mechanism for automatically changing the surrounding system;
- a substitute for legal, safeguarding, grievance, whistleblowing or emergency procedures;
- proof that departure was caused by system failure.

> **Exit Interview ≠ Retention Mechanism**

> **Exit Evidence ≠ Authority to Change the System**

## 4. Minimum inputs

A standalone use requires:
1. a departure, withdrawal or declared intent to depart;
2. a departing party;
3. a voluntary invitation mechanism;
4. consent boundaries;
5. privacy/confidentiality rules;
6. an interview or structured feedback interface;
7. a method for preserving participant-stated reasons as attributed evidence;
8. an analysis pathway;
9. a response/review routing interface;
10. provenance and retention rules.

If these are materially incomplete, record the limitation rather than silently assuming them.

## 5. Core operating chain

**Departure/Withdrawal → Voluntary Invitation → Consent/Privacy Conditions → Interview/Feedback → Participant-Stated Evidence → Documentation/Anonymisation → Case/Pattern Analysis → Response Routing → Optional Feedback → Provenance/Archive**

The stages may be shortened where appropriate, but their safeguards should not be bypassed merely for convenience.

## 6. Exit must remain possible without interview

The party's ability to leave must not depend on completing an interview, answering questions, providing reasons, accepting future contact or consenting to data retention beyond what is independently legitimate.

> **Invitation ≠ Obligation**

> **Declining Interview ≠ Declining Exit**

Possible invitation states:
- OFFERED;
- ACCEPTED;
- DECLINED;
- PARTIALLY-ACCEPTED;
- NOT-PRACTICABLE;
- NOT-OFFERED;
- NO-RESPONSE;
- UNKNOWN.

> **No Response ≠ Declined**

Declining the interview is itself not evidence of hostility, guilt, disloyalty or system failure.

## 7. Consent is granular

Do not treat one consent as authorising every information use.

Consent should be represented as extensible scoped permissions rather than one bundled yes/no state.

**ConsentPermission = <Information/Action, Mode, Purpose, Recipient/AccessScope, Duration/ReviewCondition, State>**

Candidate permissions may include:
- PARTICIPATE;
- AUDIO-RECORD;
- VIDEO-RECORD;
- WRITTEN-NOTES;
- TRANSCRIPT;
- STRUCTURED-FORM;
- RETAIN-FOR-DEFINED-PURPOSE;
- ANONYMISED-AGGREGATION;
- IDENTIFIABLE-SHARING;
- PUBLIC-QUOTATION;
- FUTURE-CONTACT;
- SHARE-WITH-SPECIFIED-REVIEW;
- OTHER-DEFINED-SCOPE.

Each may be GRANTED, DECLINED, LIMITED, WITHDRAWN, NOT-ASKED or UNKNOWN where appropriate. Duration, purpose and access scope should be recorded when materially relevant.

> **Consent to Speak ≠ Consent to Record**

> **Consent to Record ≠ Consent to Indefinite Retention**

> **Feedback ≠ Consent to Further Contact**

Where consent is later withdrawn, applicable privacy, legal and provenance rules determine what may legitimately remain.

## 8. Privacy and confidentiality

Before collecting feedback, state the applicable confidentiality boundary as clearly as practical.

Record:
- who may access identifiable material;
- whether anonymisation or pseudonymisation is available;
- retention duration or review condition;
- permitted aggregation;
- exceptions required by independently applicable law, safety or safeguarding duties;
- re-identification risks where relevant.

Do not promise stronger confidentiality than the system can actually provide.

> **Confidentiality Promise ≠ Unlimited Data Retention**

> **Anonymised ≠ Necessarily Non-Reidentifiable**

The module requires a proportionate re-identification-risk assessment but does not supply a complete anonymisation methodology. Where contextual detail creates a reasonable re-identification risk, record the material as **PSEUDONYMISED/RESTRICTED** rather than claiming anonymity.

## 9. Interviewer independence

Where practical, the interviewer or receiving mechanism should be sufficiently separated from the relationship or decision that contributed to departure to reduce pressure and defensive filtering.

Possible interviewer states:
- INDEPENDENT;
- FUNCTIONALLY-SEPARATED;
- DIRECTLY-INVOLVED;
- AUTOMATED/STRUCTURED;
- SELF-SUBMITTED;
- UNKNOWN.

Direct involvement does not automatically invalidate feedback, but it should be visible in provenance.

If no independent interviewer is available, prefer—where practical—self-submission, structured asynchronous feedback, delayed interview, or an external receiver with legitimate confidentiality arrangements. A directly involved interviewer should be used only with explicit disclosure of the conflict, voluntary consent and heightened provenance.

> **No Feedback May Be Preferable to Coercive or Materially Conflicted Collection**

## 10. Participant-stated evidence

Preserve what the departing party says without silently converting it into verified fact.

Candidate statement states:
- ATTRIBUTED-STATEMENT;
- CORROBORATED;
- PARTIALLY-CORROBORATED;
- CONTESTED;
- UNSUPPORTED;
- REFUTED;
- UNKNOWN;
- SUPERSEDED.

> **Participant Statement ≠ Verified Fact**

The module may preserve subjective experience as genuine testimony about experience even where external causal claims remain unverified.

## 11. Departure classes

Candidate descriptive classes derived from the source:

### 11.1 Practical
Departure primarily associated with circumstances such as availability, resources, technical constraints or temporary inability to participate.

### 11.2 Incompatibility
Departure associated with a mismatch between the party's values, needs, architecture, objectives or participation requirements and the system.

### 11.3 Recent-change
Departure associated by the participant with a recent policy, protocol, governance, technical or organisational change.

### 11.4 Personal-choice
Departure associated with changing interests, priorities, circumstances or no specific system reason.

### 11.5 Mixed
Multiple materially relevant classes coexist.

### 11.6 Unknown / Unclassified
Available evidence is insufficient or classification would add no useful value.

These are descriptive routing aids, not diagnoses.

> **Departure Class ≠ Causal Proof**

Do not force a mixed or unclear departure into one category.

## 12. Interview domains

Questions should be optional and proportionate. Candidate domains include:
- what initially attracted the party;
- what changed;
- what was valuable;
- what was difficult;
- primary stated reasons for leaving;
- relevant events or decisions;
- whether concerns were previously raised;
- incompatibilities;
- trust or comprehension problems;
- systemic observations;
- suggestions;
- conditions for possible re-engagement;
- willingness for future clarification.

A fixed script is not required.

The party may skip any question unless an independently legitimate process outside this module requires otherwise.

## 13. Single-case analysis

Each exit may produce useful information without constituting a systemic pattern.

A single case may identify:
- a participant-specific preference;
- an operational defect;
- a misunderstanding;
- an incompatibility;
- a recent-change concern;
- a rights or safety allegation;
- a novel failure mode;
- no system-relevant issue;
- an unresolved signal.

> **Single Departure ≠ Systemic Pattern**

But:

> **Single Departure ≠ Automatically Insignificant**

High-severity or independently evidenced claims may require immediate referral even without repetition.

## 14. Pattern analysis

Where multiple legitimately retained cases are available, compare them for recurring signals.

Possible pattern states:
- NO-PATTERN-ESTABLISHED;
- EMERGING-PATTERN;
- REPEATED-PATTERN;
- STRONG-PATTERN;
- CONTESTED-PATTERN;
- INSUFFICIENT-SAMPLE;
- SELECTION-BIAS-RISK;
- UNKNOWN.

Pattern claims should record their evaluation basis rather than rely on a universal numeric threshold.

**PatternAssessment = <Population/EvaluationSpace, EligibleCases, ObservedCases, ComparableCases, RecurringFeature, Independence, Corroboration, Severity, BiasLimits, Confidence, State>**

> **Repeated Count ≠ Pattern Without Comparability**

Pattern strength should consider more than count. Relevant factors may include:
- similarity of independently reported issues;
- temporal clustering;
- relationship to a common change;
- corroborating evidence;
- severity;
- recurrence;
- affected population;
- known sampling/response bias.

> **Pattern ≠ Proven Cause**

## 15. Non-response and selection bias

People who decline an interview may differ systematically from those who participate.

Therefore:
- interview participation rate should be visible where meaningful;
- no-response should not be interpreted as satisfaction;
- respondent data should not automatically represent all leavers;
- conclusions should record material selection-bias limitations.

> **No Feedback ≠ No Problem**

> **Interviewed Leavers ≠ All Leavers**

## 16. Historical and non-exit evidence

Historical departures without an exit interview may inform analysis only with explicit provenance and confidence. The existence of a historical dispute, complaint or event does not establish why a person departed.

> **Historical Event ≠ Known Departure Reason**

Evidence from current participants, observers, records or other non-exit sources may corroborate a system issue while remaining distinct from exit evidence.

> **Corroborating System Evidence ≠ Additional Exit Case**

## 17. Analysis states

A case or pattern may be recorded as:
- INFORMATIONAL;
- PARTICIPANT-SPECIFIC;
- POSSIBLE-SYSTEM-SIGNAL;
- SYSTEM-SIGNAL-SUPPORTED;
- URGENT-REFERRAL;
- CHANGE-ASSOCIATED-SIGNAL;
- INCOMPATIBILITY-SIGNAL;
- PRACTICAL-DEPARTURE;
- NO-ACTION-INDICATED;
- UNRESOLVED.

Multiple states may coexist where they answer different questions.

## 18. Response routing

The module does not itself possess authority to implement structural remedies.

Candidate routes include:
- no action with rationale;
- clarification/documentation improvement;
- operational review;
- policy/protocol review;
- safety/safeguarding referral;
- rights/grievance referral;
- technical investigation;
- change-impact review;
- rollback/reversion consideration where an external legitimate process supports it;
- fork/alternative-path consideration where applicable;
- independent investigation;
- monitoring for recurrence;
- other authorised review.

> **Suggested Remedy ≠ Automatically Appropriate Remedy**

> **Referral ≠ Finding**

## 19. Reasonable adaptation boundary

Learning from departure should improve the system where evidence supports improvement.

It should not create a rule that every departure must be prevented or every preference accommodated.

> **Adaptation ≠ Popularity Optimisation**

A legitimate system may retain principles or functions that some departing parties dislike, provided those choices remain independently justified.

Retention rate alone is not a sufficient measure of system quality.

## 20. Optional feedback to the departing party

Where the party has consented to future contact, the system may later communicate:
- that feedback was received;
- that a review occurred;
- that a change was made;
- that no change was made and, where appropriate, why.

Feedback should not disclose other participants' confidential information or become renewed retention pressure.

## 21. Re-engagement preference

Where voluntarily supplied, record whether the departing party:
- welcomes future contact;
- permits contact only under stated conditions;
- does not want future contact;
- may independently re-engage;
- is undecided.

> **Past Participation ≠ Continuing Contact Permission**

## 22. Provenance

Minimum provenance should preserve:
- case identifier;
- departure date/state where legitimate;
- collection method;
- interviewer/receiver relationship;
- consent states;
- statement attribution;
- transformations such as anonymisation or summarisation;
- evidence/corroboration state;
- classification changes;
- pattern inclusion/exclusion;
- referrals;
- review outcomes where available;
- retention/deletion state.

Summaries should remain traceable to source material where privacy rules permit.

## 23. Retention and deletion

Sensitive exit data should not become immortal merely because it may someday be useful.

An interview may contain separable information objects with different legitimate purposes, consent scopes and retention states.

**InformationObject = <Content/Reference, Purpose, ConsentBasis, AccessScope, RetentionCondition, State, Provenance>**

> **One Interview ≠ One Indivisible Data Object**

Deletion or restriction of one information object does not silently erase a separately legitimate security, safety, legal or provenance record. Conversely, a legitimate reason to retain one object does not authorise retention of unrelated material.

Retention should be justified by purpose, risk, consent and applicable obligations.

Possible record states:
- ACTIVE;
- AGGREGATED;
- ANONYMISED;
- RESTRICTED;
- RETENTION-REVIEW-DUE;
- DELETION-REQUESTED;
- DELETED-WHERE-PERMITTED;
- LEGALLY/OPERATIONALLY-RETAINED;
- UNKNOWN.

> **Learning Value ≠ Permanent Retention Right**

## 24. Candidate case record

A conceptual record may be represented as:

**ExitCase = <ID, DepartureState, InvitationState, Consent, PrivacyScope, CollectionMethod, InterviewerRelation, ParticipantStatements, EvidenceState, DepartureClass, Severity, CaseSignals, PatternMembership, BiasLimits, ResponseRoute, ReengagementPreference, ReviewState, RetentionState, Provenance>**

This is conceptual, not a required technical schema.

## 25. Output classifications

**EI-C1 — EXIT RECORDED / NO INTERVIEW**
Departure known; no interview evidence collected.

**EI-C2 — INTERVIEW DECLINED / EXIT RESPECTED**
Invitation declined without penalty or inference beyond that fact.

**EI-C3 — FEEDBACK RECORDED**
Participant-stated evidence preserved within consent/privacy scope.

**EI-C4 — POSSIBLE SYSTEM SIGNAL**
Feedback identifies a potentially system-relevant issue requiring bounded review or monitoring.

**EI-C5 — SYSTEM SIGNAL SUPPORTED**
Available evidence materially supports a system-relevant issue.

**EI-C6 — PATTERN EMERGING**
Multiple cases show a potentially meaningful recurring signal.

**EI-C7 — PATTERN SUPPORTED**
Evidence supports a recurring pattern beyond isolated cases.

**EI-C8 — URGENT INDEPENDENT REFERRAL**
A credible allegation or evidence indicates a consequence sufficiently severe that waiting for recurrence could materially increase harm, loss, rights impact, security exposure or irreversibility. Urgent referral does not establish the allegation as true.

> **Urgency ≠ Verification**

**EI-C9 — RESPONSE/REVIEW ROUTED**
A legitimate review or response pathway has received the relevant output.

**EI-C10 — NO SYSTEM ACTION INDICATED**
Available evidence does not currently justify system-level action.

**EI-C11 — PRIVACY/CONSENT LIMITED**
Further collection, retention, aggregation, contact or analysis is constrained by consent/privacy boundaries.

**EI-C12 — UNRESOLVED**
Available evidence or evaluation space is insufficient for stronger classification.

The classifications are dimension-specific rather than a single priority ladder:

- **Collection/participation:** EI-C1, EI-C2, EI-C3;
- **Evidence/system signal:** EI-C4, EI-C5;
- **Pattern:** EI-C6, EI-C7;
- **Routing:** EI-C8, EI-C9;
- **Closure/action:** EI-C10;
- **Privacy/consent:** EI-C11;
- **Uncertainty:** EI-C12.

Multiple classifications may coexist where they answer different questions.

## 26. Failure modes

### 26.1 Retention laundering
Learning process becomes persuasion to stay.

### 26.2 Exit obstruction
Interview or explanation becomes a condition of leaving.

### 26.3 Disloyalty framing
Departure is treated as betrayal, failure or misconduct without independent basis.

### 26.4 Testimony laundering
Participant statement is silently upgraded to verified fact.

### 26.5 Single-case overreaction
One departure automatically drives structural change.

### 26.6 Pattern suppression
Repeated independent signals are dismissed as unrelated anecdotes without adequate examination.

### 26.7 Popularity capture
System changes primarily to maximise retention rather than preserve legitimate function and principles.

### 26.8 Confidentiality breach
Identifiable material is exposed beyond the declared/legitimate scope.

### 26.9 Consent bundling
Participation is treated as permission to record, retain, aggregate or recontact.

### 26.10 Remedy laundering
A departing party's suggested remedy is treated as automatically legitimate or authoritative.

### 26.11 Interviewer conflict
Dependency, hierarchy or prior conflict suppresses candid disclosure.

### 26.12 Selection-bias blindness
Respondents are treated as representative of all departures.

### 26.13 Survivorship bias
Only remaining participants determine whether departing parties' concerns matter.

### 26.14 Category forcing
Mixed or uncertain departures are forced into a predefined class.

### 26.15 Archive immortality
Sensitive records are retained indefinitely without continuing justification.

### 26.16 Re-identification
Nominal anonymisation fails because contextual detail identifies the party.

### 26.17 Metric gaming
Incentives cause departures to be hidden, reclassified or discouraged.

### 26.18 Feedback coercion
Post-exit feedback or contact becomes unwanted re-engagement pressure.

## 27. Adversarial checks

Before accepting an analysis, ask:
1. Could the party leave without participating?
2. Were consent scopes separated?
3. Are participant statements still distinguishable from corroborated facts?
4. Has one case been overgeneralised?
5. Have repeated cases been underweighted?
6. Could non-response bias alter the conclusion?
7. Is confidentiality stronger in wording than in actual implementation?
8. Does the interviewer relationship create pressure?
9. Is a suggested remedy being mistaken for authority?
10. Is the system optimising popularity instead of legitimate purpose?
11. Is future contact actually authorised?
12. Is sensitive information being retained longer than justified?

## 28. Interfaces

The module may interface with:
- onboarding/entry processes;
- grievance and whistleblowing systems;
- safeguarding and safety processes;
- metrics;
- change-impact review;
- governance or organisational review;
- rollback/version-control mechanisms;
- forking/alternative-path mechanisms;
- continuity/provenance systems;
- privacy/data-governance systems;
- KCS/change-propagation systems;
- Reality Trees or other option-analysis methods.

These are interfaces, not hidden prerequisites.

## 29. Specialised-domain boundary

The portable mechanism can structure learning from departure, but domain-specific rules remain external.

Examples:
- employment law;
- medical confidentiality;
- education/safeguarding;
- regulated professional duties;
- statutory whistleblowing;
- mandatory incident reporting;
- collective bargaining;
- data-protection law.

The module must not be used to bypass those systems.

## 30. Minimum operating procedure

1. Record departure without obstructing it.
2. Offer voluntary feedback.
3. Establish granular consent/privacy scope.
4. Collect only proportionate information.
5. Preserve statements as attributed evidence.
6. Classify departure only where useful.
7. identify case-level signals.
8. compare legitimately retained cases for patterns.
9. account for non-response and selection bias.
10. route supported or urgent findings to legitimate review.
11. provide optional feedback only where authorised.
12. preserve provenance.
13. review retention and delete/restrict where required.
14. update classifications if later evidence changes the interpretation.

## 31. Epistemic safeguards

> **No Interview ≠ No Problem**

> **Interview ≠ Verification**

> **Departure ≠ System Failure**

> **Single Departure ≠ Systemic Pattern**

> **Pattern ≠ Proven Cause**

> **No Pattern Found in Examined Cases ≠ No Pattern Exists**

> **No Recorded Concern ≠ No Concern Exists**

> **Suggested Remedy ≠ Legitimate Authority**

> **Tested in One Context ≠ Validated in Every Context**

## 32. Portability claim

The underlying problem is generic: systems often learn disproportionately from those who remain, while information from those who leave is lost or distorted.

The module is intended to preserve departure evidence while protecting autonomy and limiting inference.

Current supported claims:

> **A standalone portable specification has been extracted from a documented source protocol and source-resolution audit.**

> **BTT-001 demonstrated functional independent transfer in a non-Concord open-source-project domain: 26/26 frozen predictions materially confirmed.**

This is specification-level transfer evidence, not empirical validation.

## 33. Source provenance

Primary recovered source:
- *The Concord Exit Interview Protocol — Constitutional Learning Through Voluntary Withdrawal*, Draft 1, CRL 2, Confidence: Emerging.
- Recovered from V1/V1.1 Git history after the substantive Markdown file was deleted from the current branch.

Development audit:
- *Exit Interview Protocol — Source Resolution and Extraction Audit 001*.

The historical source's Concord-specific remediation mechanisms have been externalised as interfaces rather than silently embedded as portable authority.

## 34. Development next step

Freeze **Blind Transfer Test 002** before obtaining an independent response.

Use a materially different non-Concord domain and specifically pressure:
- NO-RESPONSE versus DECLINED;
- scoped consent by collection mode, purpose and duration;
- separable information objects and selective deletion;
- pattern construction without universal numeric thresholds;
- historical non-interview evidence;
- non-exit corroboration;
- interviewer fallback;
- dimension-specific EI-C classifications;
- urgent referral without verification;
- re-identification risk.
