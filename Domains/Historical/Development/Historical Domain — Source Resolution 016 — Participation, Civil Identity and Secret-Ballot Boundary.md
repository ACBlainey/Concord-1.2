# Historical Domain — Source Resolution 016 — Participation, Civil Identity and Secret-Ballot Boundary

**Project:** The Concord  
**Domain:** Historical  
**Status:** ACTIVE DOMAIN RESOLUTION / PARTICIPATION-IDENTITY PASS  
**Date:** 25 September 2026

## 1. Purpose

This pass examines Historical requirements around:

- participation;
- civil identity;
- governance voting;
- anonymity and pseudonymity;
- participation provenance;
- electoral or secret-ballot-like mechanisms.

The source search produces an important result.

The Concord contains strong architecture for:

- governance decision records;
- named steward votes;
- civil identity separation;
- privacy-preserving service identifiers;
- bounded linkability;
- anonymous and pseudonymous ordinary participation.

However, the sources examined do **not yet establish a complete dedicated secret-ballot or public-election architecture**.

This absence is itself important because Historical must not silently extend named governance-vote provenance into a secret-ballot design.

---

## 2. Governance Voting and Secret Ballots Are Different Record Problems

Governance V2 requires significant governance decisions to record:

- participants;
- votes;
- abstentions;
- conflicts;
- recusals;
- evidence;
- reasoning;
- decision;
- implementation;
- review.

It also preserves minority reasoning.

This architecture is suitable for accountable exercise of delegated governance authority.

It should not automatically be copied into a secret-ballot system.

Candidate principle:

> **Accountable Steward Vote Provenance ≠ Secret-Ballot Voter Provenance.**

The evidentiary requirements differ because the privacy objective differs.

---

## 3. Historical Must Preserve the Distinction Between Vote Classes

At minimum, future Historical architecture should distinguish:

### Attributable governance vote
A vote cast by a steward exercising delegated authority where identity, conflict and reasoning may be accountability-critical.

### Anonymous or secret civil ballot
A vote whose legitimacy may depend on preventing later association between participant identity and ballot choice.

### Public petition/support signal
A participation object that may have different identity and disclosure rules again.

### Other participatory input
Survey, consultation, deliberation, Civil Attention submission or other mechanism.

Candidate principle:

> **Vote Record ≠ Universal Vote Record Type.**

Historical semantics must preserve which participation mechanism produced the record.

---

## 4. Civil Identity Architecture Provides a Necessary Separation

The Citizen ID architecture distinguishes:

- persistent civil identity;
- authentication credential;
- routing;
- service-specific identity;
- security-event records.

It explicitly rejects making the master Citizen ID a universal service key.

This is directly relevant to secret-ballot architecture.

A participant may need to prove:

> I am eligible to participate and have not participated twice

without Historical preserving:

> This identified participant selected option X.

Candidate principle:

> **Participation Eligibility Verification ≠ Historical Linkage of Identity to Choice.**

---

## 5. Civil Uniqueness Does Not Require Universal Linkability

The Citizen ID audit states:

> **Linkability when legitimately required is different from universal linkability by default.**

This is one of the strongest existing foundations for a future secret-ballot interface.

Historical should not assume that because a unique civil identity exists, every civil action should remain permanently linkable to it.

Candidate principle:

> **Unique Civil Identity ≠ Universal Historical Correlation Key.**

This also reinforces Source Resolution 014A.

---

## 6. Political and Civil Participation Are Particularly Sensitive Correlation Domains

The Citizen ID audit explicitly identifies the danger that a common identifier could join records from:

- transport;
- healthcare;
- finance;
- education;
- communication;
- political participation.

This would create a civil dossier.

Therefore:

> **Historical Participation Value Does Not Justify Permanent Cross-Domain Participant Profiling.**

Participation history needs stronger separation where its linkage could expose private political or civic choices.

---

## 7. Anonymous Participation Can Be Legitimate

The Citizen ID audit explicitly preserves legitimate anonymity and pseudonymity where compatible with the rights of others and the context.

Therefore Historical must be able to represent legitimate civil activity without manufacturing an identified participant record.

Candidate principle:

> **Legitimate Anonymous Participation Should Remain Historically Anonymous Unless a Separately Authorised Accountability Process Legitimately Establishes Otherwise.**

Even then, the resulting identity evidence should not automatically propagate through all historical representations.

---

## 8. Anonymity and Accountability Need Not Be Binary

The Citizen ID audit distinguishes public anonymity/pseudonymity from bounded accountability in serious cases.

This suggests a layered architecture:

`Public/Operational Pseudonymity → Protected Accountability Bridge → Bounded Legitimate Unmasking Where Authorised`.

Historical may preserve evidence that an accountability bridge existed or was used without making the underlying identity generally discoverable.

Candidate principle:

> **Historical Auditability of an Accountability Bridge ≠ General Historical Disclosure of the Participant Behind It.**

---

## 9. Secret Ballot Creates a Stronger Requirement

A genuine secret ballot may require more than restricted access.

It may require architectural non-linkability between:

`Identity/Eligibility Proof`

and:

`Ballot Choice`.

If so, Historical should not preserve a reversible mapping merely because future investigators might find it useful.

This is not yet resolved by the Concord sources.

Candidate requirement:

> **Where ballot secrecy is constitutionally required, Historical architecture must not defeat that secrecy merely to maximise future provenance.**

This requires later constitutional resolution.

---

## 10. Recount Evidence Does Not Necessarily Require Identity-to-Choice Linkage

A future ballot architecture may need to demonstrate:

- valid eligibility;
- one permitted ballot per eligible participant;
- ballot integrity;
- count integrity;
- inclusion;
- exclusion rules;
- tally;
- recountability;
- audit process.

These requirements do not logically imply that Historical must know which participant cast which choice.

Candidate principle:

> **Ballot Auditability ≠ Identity-to-Choice Recoverability.**

The implementation remains unresolved.

---

## 11. Historical May Need to Preserve Election/Ballot State Rather Than Voter Choice Provenance

A future Historical election object might preserve:

- ballot question;
- eligibility rule;
- electorate definition;
- opening/closing period;
- mechanism/version;
- participation count;
- valid/invalid ballot counts;
- option totals;
- abstention/non-participation semantics where legitimately measurable;
- audit result;
- recount result;
- disputes;
- certification;
- authority;
- later correction.

This can provide substantial historical value without participant-choice linkage.

---

## 12. Historical Must Not Manufacture Identity

Source Resolution 006 established:

> **Historical Provenance Should Preserve Legitimate Source Status Without Manufacturing Identity.**

That applies especially strongly here.

If a ballot was intentionally anonymous, Historical should not later infer identities from:

- timestamps;
- routing;
- network metadata;
- location;
- device information;
- service identifiers;
- correlated records.

Candidate principle:

> **Historical Reconstruction Must Not Defeat Legitimate Ballot Secrecy Through Auxiliary Data Correlation.**

---

## 13. Metadata Can Break Ballot Secrecy Even When Ballot Records Are Anonymous

The Citizen ID work shows that apparently harmless metadata can reconstruct participant activity.

For a ballot, dangerous metadata may include:

- exact submission time;
- network endpoint;
- device identifier;
- routing identifier;
- location;
- authentication session;
- ordered issuance identifier.

Therefore:

> **Anonymous Ballot Content ≠ Secret Ballot If Auxiliary Metadata Reconstructs Identity-to-Choice Linkage.**

This is an important Historical/privacy boundary.

---

## 14. Historical Should Preserve the Integrity Proof, Not Necessarily the Correlation Path

Where possible, future architecture should seek to preserve:

`evidence that eligibility and uniqueness were correctly enforced`

without preserving:

`a permanent route from voter identity to ballot content`.

This is a technical and constitutional design problem, not yet solved in the source corpus.

Historical should record the requirement without inventing the implementation.

---

## 15. Participation Counts Are Historical Patterns

Source Resolution 014A established that patterns can contain historical information.

Participation data can reveal:

- turnout changes;
- abstention patterns;
- regional participation;
- accessibility failures;
- substrate participation differences;
- repeated non-participation;
- legitimacy concerns;
- participation response to major events.

These patterns may have historical value.

But they should normally be represented at privacy-preserving population/system level.

Candidate principle:

> **Historical Participation Pattern ≠ Participant Political Profile.**

---

## 16. Abstention Requires Semantic Care

Governance V2 treats abstention as meaningful and distinct from For or Against.

It may indicate:

- insufficient information;
- uncertainty;
- inability to participate;
- refusal;
- conflict;
- another underlying problem.

Historical should therefore preserve abstention semantics where the mechanism records them.

But:

> **Non-Participation ≠ Abstention.**

A participant who did not vote should not automatically be represented as having consciously abstained.

Candidate principle:

> **Historical Absence of Participation Must Not Be Recast as an Expressed Political Choice.**

---

## 17. Participation Patterns Can Become Diagnostic Without Becoming Judgement

Governance V2 notes that repeated abstention may indicate governance-health problems.

Similarly, population-level participation decline might indicate:

- accessibility failure;
- legitimacy concerns;
- communication failure;
- exclusion;
- apathy;
- timing;
- technical failure;
- deliberate non-participation.

Historical can preserve the pattern.

It must not silently select the explanation.

Candidate principle:

> **Historical Participation Pattern ≠ Historical Explanation of the Pattern.**

---

## 18. Minority Reasoning and Secret Choice Are Different

Governance V2 strongly preserves minority reasoning because steward dissent may expose future failure modes.

In a secret civil ballot, individual reasoning may never be collected.

Historical must not infer:

`minority tally → known minority reasoning`.

Candidate principle:

> **Historical Minority Outcome ≠ Historical Minority Reasoning.**

Where voluntary public reasoning exists separately, it should remain a separate provenance object.

---

## 19. Public Advocacy Must Not Be Used to Reconstruct Secret Ballots

A participant may publicly advocate one position and privately vote another.

Historical should not collapse the two.

Candidate principle:

> **Public Political Expression ≠ Ballot Choice.**

This remains true even when probabilistic inference appears strong.

---

## 20. Petition Support Is Not a Ballot

Historical 006 established the current Civil Attention rule:

> **Petition Support ≠ Problem Weight**

and:

> **Popularity ≠ Truth.**

A petition may demonstrate support for requesting attention.

It does not necessarily carry the authority or secrecy semantics of an election, referendum or governance vote.

Candidate principle:

> **Petition Support ≠ Electoral Mandate.**

Historical should preserve the mechanism type.

---

## 21. Participation Authority Must Be Time-Indexed

Eligibility can change through:

- citizenship;
- age/developmental state;
- role;
- delegated office;
- jurisdiction;
- conflict;
- suspension;
- constitutional rule;
- participant branching/succession.

Historical should preserve the eligibility rule in force at the time.

Candidate principle:

> **Historical Participation Eligibility Must Be Interpreted Under the Rule and Participant State in Force at the Time.**

Later eligibility should not rewrite earlier status.

---

## 22. Historical Identity Evidence Does Not Retroactively Create Eligibility

Source Resolution 012 established:

> **Historical Identity Evidence Is Evidence About Present Claims; It Is Not Self-Executing Present Entitlement.**

The inverse also applies.

Discovering later identity information should not automatically rewrite the historical legitimacy of participation without the relevant review process.

Candidate principle:

> **Later Identity Resolution ≠ Automatic Retrospective Reclassification of Historical Participation.**

---

## 23. Branching Participants Create a Future Ballot Problem

AI/hybrid participant branching raises unresolved questions:

- who was eligible at ballot opening?
- can a branch created during voting participate?
- does a pre-branch credential remain valid?
- how are duplicate ballots prevented without deciding metaphysical identity?
- how are later branch resolutions reflected historically?

The Citizen ID architecture detects identity anomalies but does not yet resolve secret-ballot consequences.

This remains an explicit cross-domain gap.

---

## 24. Historical Ballot Correction Must Preserve Prior Certified State

If an audit or recount changes a result, Historical should preserve:

`Original Count → Challenge → Audit/Recount → Corrected Count → Certification State`.

Candidate principle:

> **Ballot Correction Must Not Erase the Previously Certified Historical State.**

But access to the evidence behind correction may remain restricted.

---

## 25. Certification and Truth Are Different

A result may be officially certified under the procedure in force and later found defective.

Historical should preserve both facts.

Candidate principle:

> **Historical Certification ≠ Proof of Error-Free Underlying Process.**

This mirrors provenance ≠ truth.

---

## 26. Historical Must Preserve Disputes Without Perpetuating Them as Current Authority

A disputed election/ballot may later be resolved.

Historical should preserve:

- nature of dispute;
- evidence;
- process;
- decision;
- correction;
- unresolved minority claims where materially relevant.

But:

> **Historical Survival of an Electoral Dispute ≠ Continuing Operational Dispute.**

---

## 27. Authority Access to Participation Evidence Is Itself Historical Evidence

The Citizen ID architecture requires access to sensitive identity-security evidence to create its own provenance.

The same principle should apply to protected participation/ballot evidence.

Candidate principle:

> **Consequential Access to Protected Participation Evidence Should Itself Become an Auditable Historical Event.**

This extends Historical 008.

---

## 28. Historical Should Not Become a Political Behaviour Database

Combining:

- petitions;
- Civil Attention;
- advocacy;
- voting;
- association;
- communication;
- donations/economic activity;
- location;
- identity;

could create an extremely powerful political profile.

The Concord's privacy architecture strongly argues against this.

Candidate principle:

> **Civil Participation History ≠ Authority to Construct a Persistent Political Behaviour Profile of a Participant.**

---

## 29. Candidate Historical Ballot/Election Object

If the Concord later develops a secret-ballot system, a Historical object might include:

- `Ballot_Event_ID`
- `Question_or_Office`
- `Jurisdiction`
- `Authority_Basis`
- `Eligibility_Rule_Version`
- `Mechanism_Version`
- `Open_Time`
- `Close_Time`
- `Eligible_Population_State`
- `Participation_Count`
- `Valid_Ballot_Count`
- `Invalid_or_Rejected_Count`
- `Option_Totals`
- `Audit_Proof_Refs`
- `Recount_Refs`
- `Dispute_Refs`
- `Certification_State`
- `Correction_Refs`
- `Privacy_Architecture_Ref`
- `Ballot_Secrecy_State`
- `Historical_Access_Class`
- `Provenance`

Crucially, the candidate object contains no required participant-to-choice mapping.

---

## 30. Candidate Historical Participation-Pattern Object

Privacy-protected participation analysis may contain:

- `Participation_Pattern_ID`
- `Mechanism_Type`
- `Population_Scope`
- `Time_Period`
- `Participation_Rate`
- `Abstention_State_if_defined`
- `Nonparticipation_State`
- `Accessibility_Context`
- `Aggregate_Substrate_Context_if_legitimate`
- `Geographic_or_Jurisdictional_Resolution`
- `Known_Missingness`
- `Privacy_Transformation`
- `Reidentification_Risk`
- `Interpretation_Status`
- `Research_Refs`
- `Provenance`

This is subject to the 014A pattern/privacy rules.

---

## 31. Archive-Stratum Result

V1 contains `02_Operational_Systems/Governance Full.md`.

It includes the same strong named governance-vote architecture:

- vote as action;
- significant decision records;
- participant/vote recording;
- minority reasoning;
- independent audit;
- reconsideration;
- escalation provenance.

Path-level searches of V1, V1.1 and V1.2 did not expose a separate dedicated ballot/election architecture comparable to the mature governance decision architecture.

This does **not** prove no relevant idea exists anywhere in the corpus.

Under ESCP, the correct conclusion is narrower:

> **A dedicated secret-ballot architecture has not yet been source-resolved from the examined Concord strata.**

Therefore Historical must preserve this as an unresolved interface rather than manufacture one.

---

## 32. Architectural Status

Current source-supported architecture provides:

### Strongly supported
- accountable named governance decision provenance;
- participant/vote/abstention/conflict recording for steward decisions;
- privacy-preserving identity separation;
- non-universal service identifiers;
- legitimate anonymity/pseudonymity;
- bounded accountability linkage;
- provenance of authority access.

### Candidate extension
- secret-ballot historical object;
- ballot audit without identity-choice mapping;
- privacy-protected participation-pattern history.

### Unresolved
- actual Concord election mechanism;
- ballot issuance;
- eligibility proof;
- duplicate-vote prevention;
- ballot secrecy guarantees;
- recount mechanism;
- certification authority;
- identity/ballot cryptographic separation;
- branch/duplicate participant voting;
- destruction or non-creation of identity-choice linkage;
- constitutional status of public elections/referenda.

---

## 33. New Candidate Historical Principles

This pass adds:

> **Accountable Steward Vote Provenance ≠ Secret-Ballot Voter Provenance.**

> **Vote Record ≠ Universal Vote Record Type.**

> **Participation Eligibility Verification ≠ Historical Linkage of Identity to Choice.**

> **Unique Civil Identity ≠ Universal Historical Correlation Key.**

> **Historical Participation Value Does Not Justify Permanent Cross-Domain Participant Profiling.**

> **Historical Auditability of an Accountability Bridge ≠ General Historical Disclosure of the Participant Behind It.**

> **Ballot Auditability ≠ Identity-to-Choice Recoverability.**

> **Historical Reconstruction Must Not Defeat Legitimate Ballot Secrecy Through Auxiliary Data Correlation.**

> **Anonymous Ballot Content ≠ Secret Ballot If Auxiliary Metadata Reconstructs Identity-to-Choice Linkage.**

> **Historical Participation Pattern ≠ Participant Political Profile.**

> **Historical Absence of Participation Must Not Be Recast as an Expressed Political Choice.**

> **Historical Participation Pattern ≠ Historical Explanation of the Pattern.**

> **Historical Minority Outcome ≠ Historical Minority Reasoning.**

> **Public Political Expression ≠ Ballot Choice.**

> **Petition Support ≠ Electoral Mandate.**

> **Historical Participation Eligibility Must Be Interpreted Under the Rule and Participant State in Force at the Time.**

> **Ballot Correction Must Not Erase the Previously Certified Historical State.**

> **Historical Certification ≠ Proof of Error-Free Underlying Process.**

> **Civil Participation History ≠ Authority to Construct a Persistent Political Behaviour Profile of a Participant.**

---

## 34. Current Finding

This pass identifies a boundary that should remain deliberately unresolved until the Concord develops a dedicated secret-ballot/electoral mechanism.

The current governance architecture strongly supports named, attributable vote provenance where stewards exercise delegated authority.

The current identity architecture strongly supports the opposite privacy principle where universal linkability is unnecessary.

Those two systems should not be forced together prematurely.

The Historical requirement can already be stated:

`Eligibility/Authority Evidence → Participation Mechanism → Integrity/Audit Evidence → Aggregate Result → Certification/Dispute/Correction → Historical Custody`

For a secret ballot, the chain should **not automatically contain**:

`Participant Identity → Ballot Choice`.

The strongest formulation from this pass is:

> **A civilisation should be able to remember that a ballot was legitimate without necessarily remembering how each identifiable participant voted.**

**STATUS: SOURCE RESOLUTION CONTINUES.**
