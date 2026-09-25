# Historical Domain — Source Resolution 019 — Privacy, Permission, Protected Spaces and Historical Access

**Project:** The Concord  
**Domain:** Historical  
**Status:** ACTIVE DOMAIN RESOLUTION / PRIVACY-ACCESS PASS  
**Date:** 25 September 2026

## 1. Purpose

This pass examines the Historical Domain against Concord privacy, personal-data, safe-space and permission architecture.

Primary V1.2 sources include:

- `03_Continuity_and_Memory/Personal Data and Metrics/Citizen Data Ownership, Access and Contestable Civilisational Metrics.md`;
- `06_Portable_Modules/Fractal Permission Architecture — Portable Module.md`;
- `08_Active_Development/.../Basic Civil Space Classification — Public Space, Private Space, Safe Space and Substrate-Neutral Access.md`;
- `08_Active_Development/.../8. Intermediary Personal-Data Boundary.md`;
- `08_Active_Development/.../9. Automatic Anonymised Metrics Extraction System.md`;
- `00_Front_Door/4 Need, Consent and Legitimate Authority.md`;
- prior Historical Source Resolutions 005, 008, 014A, 016 and 018.

The central question is:

> **If Historical is allowed to preserve information for long periods, what prevents preservation from becoming permanent permission to inspect, correlate, disclose or reuse it?**

The source architecture strongly indicates that **custody, discoverability, accessibility, disclosure, publication and reuse are separate functions**.

---

## 2. Preservation Does Not Carry Permission Forward Automatically

FPA states:

> **Past Permission ≠ Present Permission.**

and:

> **Permission for One Function ≠ Permission for Unrelated Functions.**

This applies directly to Historical.

Information may have been legitimately visible to an operational system at time T1.

That does not imply that every future Historical user at T2 inherits the original permission.

Candidate principle:

> **Historical Preservation of Information ≠ Preservation of Every Permission Once Associated With That Information.**

---

## 3. Historical Custody Is Not Historical Access

A Historical system may legitimately hold a protected record while almost nobody is permitted to inspect it.

Therefore:

> **Historical Custody ≠ Historical Access.**

This strengthens the earlier distinction:

> **Discoverability ≠ Accessibility.**

The existence of a record may be knowable while its content remains protected.

---

## 4. Historical Access Is Action-Specific

FPA decomposes “access” into distinct actions.

Historical therefore should distinguish at least:

- know that a record exists;
- search metadata;
- inspect content;
- extract a field;
- derive an aggregate;
- correlate with another record;
- copy;
- disclose;
- publish;
- alter metadata;
- annotate;
- challenge;
- delete;
- restore;
- execute/reactivate where applicable.

Candidate principle:

> **Permission to Perform One Historical Action ≠ Permission to Perform Another.**

“Has archive access” is therefore too coarse for consequential records.

---

## 5. Historical Access Must Be Function-Bounded

The source architecture asks:

> **What information does this actor require for this legitimate purpose?**

Historical access should therefore follow:

`Legitimate Function → Required Historical Information → Minimum Necessary Access → Bounded Use → Function Completion → Access Termination`.

Candidate principle:

> **Historical Access Should Be Bounded to the Minimum Information and Action Set Required by the Legitimate Function.**

---

## 6. Storage Does Not Transfer Ownership

The personal-data architecture explicitly states:

- collection does not automatically transfer ownership;
- storage does not transfer ownership;
- analysis does not transfer ownership;
- predictive usefulness does not transfer ownership.

Therefore:

> **Historical Storage of Personal Data ≠ Historical Ownership of the Person's Data.**

Historical may possess custody responsibilities without acquiring general ownership.

---

## 7. Participant Data Rights Survive Archival Transfer Where Applicable

The current personal-data architecture gives participants a strong presumptive relationship to identifiable data derived from them, including:

- access;
- context;
- contestability;
- correction.

Archival transfer should not silently extinguish these rights.

Candidate principle:

> **Archival Transfer ≠ Automatic Termination of Participant Data Rights.**

Exceptions may exist for legitimate judicial, security, third-party privacy or other bounded reasons, but those require their own justification.

---

## 8. Contestability Is Part of Historical Integrity

Historical 004 already established correction without historical erasure.

The personal-data architecture adds that a participant may contest:

- a datum;
- its context;
- an inference;
- a consequential model.

Historical should preserve:

`Original Record → Participant Challenge/Context → Review → Correction/Confirmation/Dispute → Current Representation`.

Candidate principle:

> **Historical Integrity Includes the History of Legitimate Contestation.**

---

## 9. Correction Must Not Become Silent Retrospective Editing

A participant's right to correction does not require Historical to pretend the original error never existed where the original state is materially relevant.

Therefore:

> **Correction of Personal Data ≠ Falsification of the Historical Record of the Error.**

But preservation of the erroneous state must not justify continued operational use of an error already corrected.

> **Historical Survival of an Error ≠ Permission to Continue Treating the Error as Current Truth.**

---

## 10. Context Can Be Privacy-Sensitive

The personal-data architecture recognises the right to add context.

But context can itself reveal:

- relationships;
- health;
- location;
- private circumstances;
- third-party information.

Therefore:

> **Historical Context Preservation ≠ Automatic Public Disclosure of Context.**

Context needs its own access classification.

---

## 11. Third-Party Rights Complicate Participant Access

A record about Participant A may also contain protected information about B.

A cannot necessarily receive the complete raw record merely because it concerns them.

Candidate principle:

> **Right of Access to One's Historical Data ≠ Right to Unrestricted Third-Party Historical Data.**

Historical may need bounded views, redaction or mediated access.

---

## 12. Personal Data and Civilisational Data Must Remain Distinct

The source architecture explicitly separates identifiable personal data from civilisational data.

Historical should preserve the same distinction.

Where long-run pattern analysis does not require identity:

`Identifiable Operational Data → Privacy Transformation → Aggregate/Anonymised Historical Pattern Data`.

Candidate principle:

> **Civilisational Historical Value Does Not Automatically Justify Retention of Identifiable Resolution.**

This directly supports Historical 014A.

---

## 13. Pattern Value Does Not Require Universal Identity Retention

Historical 014A found that useful information can reside in patterns such as consumer behaviour, food demand, infrastructure use and later health correlations.

The privacy architecture provides the missing constraint:

> **Where a civil objective can be achieved through aggregate system-level learning, unnecessary individual observation should be avoided.**

Therefore:

> **Historical Pattern Preservation Should Prefer the Minimum Resolution That Preserves the Legitimate Pattern Value.**

---

## 14. Anonymisation Is a Transformation, Not Magic

The Metrics architecture recognises:

- small-population risk;
- deanonymisation;
- technical fingerprints;
- anonymisation failure.

Historical should not classify data as permanently safe merely because an anonymisation operation once occurred.

Candidate principle:

> **Historical Anonymisation Status Must Remain Sensitive to Re-Identification Risk Over Time.**

A dataset safe at T1 may become identifiable at T2 through new auxiliary data or techniques.

---

## 15. Privacy State Can Change Through Time

This produces a new temporal Historical problem.

A record may transition:

`Identifiable → Anonymised-at-T1 → Re-identification-risk-increases → Restricted/Reprocessed`.

Therefore:

> **Privacy Classification Is Itself Historically Versioned State.**

Historical must preserve the fact that an older disclosure may have been considered safe under the knowledge available at the time while protecting against current risk.

---

## 16. Historical Correlation Is a Distinct Permission

The user's earlier pattern-value observation exposes an important boundary.

Two privacy-safe datasets may become privacy-sensitive when correlated.

For example:

- consumer trends;
- location patterns;
- rare health outcomes;
- small populations.

Candidate principle:

> **Permission to Hold Dataset A + Permission to Hold Dataset B ≠ Automatic Permission to Correlate A and B.**

Correlation can create information that neither source contains independently.

---

## 17. Derived Information Can Be More Sensitive Than Its Inputs

A historical system may infer:

- disease clusters;
- identity;
- relationships;
- beliefs;
- vulnerabilities;
- behavioural profiles.

Therefore:

> **Privacy Risk Must Be Evaluated at the Level of Derived Information, Not Only Source Records.**

This is a major consequence of treating patterns as information.

---

## 18. Pattern Discovery Can Create New Historical Objects

If later analysis discovers a relationship between old consumer data and a health outcome, Historical should preserve:

- source datasets;
- privacy state;
- analysis method;
- discovered correlation;
- uncertainty;
- later validation;
- access restrictions.

Candidate principle:

> **Later Pattern Discovery Adds Historical Knowledge; It Does Not Mean the Pattern Was Known at the Time the Source Data Were Created.**

This extends Historical 009 and 014A.

---

## 19. Correlation Is Not Causation

The Metrics architecture explicitly identifies the failure mode of treating correlation as causation.

Historical must preserve:

`Observed Pattern ≠ Causal Finding`.

Candidate principle:

> **Historical Correlation ≠ Historical Causation.**

This is particularly important when retrospective health, consumer or behavioural correlations could stigmatise groups.

---

## 20. Safe Spaces Create Information Boundaries

Concord safe-space architecture is not merely physical.

Protected spaces can be:

- physical;
- digital;
- informational;
- relational;
- functional.

Historical records originating in a safe/private/protected context should preserve that context.

Candidate principle:

> **Historical Transfer Does Not Automatically Flatten the Protection Level of the Context From Which a Record Came.**

---

## 21. Parent-Space Access Does Not Propagate Downward

FPA states:

> **Parent-Space Permission ≠ Automatic Child-Space Permission.**

Historical therefore cannot infer that access to a broad archive grants access to nested protected collections.

Example:

`Historical Domain → Medical History Collection → Protected Participant Record → Highly Restricted Subrecord`.

Candidate principle:

> **Archive-Level Access ≠ Collection-Level Access ≠ Record-Level Access ≠ Field-Level Access.**

---

## 22. Deeper Historical Context Can Require Stronger Permission

FPA states that deeper contextual access may require additional justification.

Historical research may begin with public aggregates and later require protected records.

The permission must be reassessed at the boundary.

Candidate principle:

> **Analytical Convenience Does Not Authorise Descent Into More Protected Historical Resolution.**

---

## 23. Technical Capability Is Not Historical Permission

FPA states:

> **Physical/Technical Capability ≠ Normative Permission.**

Therefore an archivist, administrator, AI model or database operator being technically capable of reading a protected record does not establish legitimate access.

Candidate principle:

> **Historical System Capability ≠ Historical Access Authority.**

This is essential if Historical is implemented using powerful search or AI systems.

---

## 24. Machine Search Creates a New Exposure Surface

An AI may not display a raw record but may still:

- search it;
- classify it;
- correlate it;
- summarise it;
- answer questions from it.

Those are information uses.

Candidate principle:

> **Machine Processing of Protected History Is Access-Relevant Even When No Human Reads the Raw Record.**

Historical permission architecture must therefore govern machine as well as human use.

---

## 25. Searchability Is Not Neutral

A record hidden in cold storage and a record instantly searchable across civilisation have radically different privacy consequences even if the bytes are identical.

Therefore:

> **Retention State ≠ Searchability State.**

and:

> **Increasing Discoverability Can Increase Privacy Exposure Without Changing Stored Content.**

This links Historical 005's cold storage to FPA.

---

## 26. Indexes Can Leak Protected Information

Even metadata such as:

- record existence;
- category;
- date;
- participant link;
- location;

can reveal sensitive facts.

Candidate principle:

> **Historical Metadata Can Itself Be Protected Information.**

Therefore “discoverability without accessibility” is not always harmless; even discoverability may require tiering.

---

## 27. Existence Disclosure Is a Permission Action

A query such as “Does Historical hold a psychiatric record for X?” can expose sensitive information even if content is never returned.

Candidate principle:

> **Permission to Reveal Record Existence ≠ Permission to Reveal Record Content, and Neither Should Be Assumed From the Other.**

---

## 28. Purpose Limitation Survives Time

The personal-data architecture states:

> **Possession of information for one legitimate purpose does not automatically authorise its use for another.**

Historical retention creates a temptation to reuse old data because it is available.

Candidate principle:

> **Age of a Record Does Not Dissolve Purpose Limitation.**

A new use requires a new legitimate basis where required.

---

## 29. Historical Importance Is Not Unlimited Reuse Authority

A record can be historically valuable while remaining protected.

Therefore:

> **Historical Value ≠ Universal Research Permission.**

This strengthens the distinction established in Historical 017 between preservation and public access.

---

## 30. Research Access May Require Privacy Transformation

Where researchers need patterns rather than identities, Historical can provide:

- aggregates;
- redacted records;
- anonymised extracts;
- bounded query interfaces;
- controlled environments.

Candidate principle:

> **Historical Research Access Should Prefer the Least Identity-Revealing Representation That Can Answer the Legitimate Question.**

---

## 31. Query Interfaces May Be Safer Than Data Release

For some protected historical datasets, the safest architecture may be:

`Research Question → Authorised Query → Protected Computation → Bounded Result`

rather than:

`Protected Dataset → Copy to Researcher`.

Candidate principle:

> **Ability to Ask a Legitimate Question Need Not Imply Possession of the Underlying Historical Dataset.**

This is strongly compatible with the black-box architecture in Historical 008.

---

## 32. Exceptional Access Must Remain Exceptional

The source architecture permits separately justified identifiable access for judicial, emergency or other legitimate functions.

Historical should preserve:

- basis;
- scope;
- actor;
- records accessed;
- actions performed;
- outputs;
- time;
- termination;
- review.

Candidate principle:

> **Exceptional Historical Access Should Produce Its Own Accountability Provenance.**

---

## 33. Emergency Access Must Expire

FPA states:

> **Emergency Need ≠ Unlimited Emergency Authority.**

Historical access opened for an emergency must not silently become permanent.

Candidate principle:

> **Emergency Historical Access Must Terminate or Be Reauthorised When the Emergency Basis Ends.**

---

## 34. Historical Access Decisions Can Be Contested

If access is consequential, participants may need mechanisms to challenge:

- improper access;
- excessive scope;
- incorrect identity linkage;
- misuse;
- improper disclosure;
- retained permission after purpose ended.

Candidate principle:

> **Historical Access Governance Must Be Contestable Where Consequential.**

The precise forum remains domain-dependent.

---

## 35. Historical Access History Is Itself Sensitive

An access log can reveal:

- investigations;
- health concerns;
- disputes;
- security interests;
- personal relationships.

Therefore:

> **Historical Access Provenance ≠ Automatically Public Provenance.**

Auditability and publicity are different.

---

## 36. Auditability Can Be Layered

A useful candidate structure is:

- participant-visible access history where appropriate;
- restricted institutional audit;
- protected security/judicial audit;
- anonymised systemic access-abuse metrics;
- public aggregate accountability.

Candidate principle:

> **Historical Auditability Does Not Require Universal Visibility of Every Access Event.**

---

## 37. Permission Changes Need Historical Provenance

FPA models permission change with basis, effective point, actor/source, provenance and state.

Historical should preserve consequential:

- grant;
- narrowing;
- revocation;
- expiry;
- delegation;
- emergency override;
- restoration.

Candidate principle:

> **Historical Access State Is a Versioned Relationship, Not a Permanent Property of a User or Record.**

---

## 38. Delegated Access Must Preserve Scope

FPA states:

> **Permission to Act ≠ Permission to Delegate.**

A researcher or official authorised to inspect a record cannot automatically forward it to another person, institution or AI.

Candidate principle:

> **Historical Access Permission ≠ Historical Disclosure Permission.**

---

## 39. Credentials Are Not Authority

Possession of a password, key, administrator account or copied credential does not establish permission.

Candidate principle:

> **Historical Credential Possession ≠ Historical Access Legitimacy.**

Historical security logs should preserve the distinction between successful access and authorised access.

---

## 40. Historical Disclosure Is a New Use Event

When a protected record is disclosed, the disclosure changes the information environment.

Therefore Historical may need to record:

`Protected Record → Authorisation → Disclosure → Recipient → Purpose → Derived Outputs/Restrictions`.

Candidate principle:

> **Disclosure Does Not Merely Reveal History; It Can Create New History.**

This is particularly important for cross-civilisational disclosure identified in Historical 018.

---

## 41. Publication Is Stronger Than Access

Access to a protected record for a bounded function does not imply permission to publish it.

Candidate principle:

> **Historical Access ≠ Historical Publication Authority.**

Public historical narratives should use appropriately publishable representations, not simply whatever Historical can internally access.

---

## 42. Privacy and Public Memory Are Different Layers

Historical 017 established that the Library/public memory layer is distinct from Historical custody.

This pass strengthens that result:

`Protected Historical Record → Authorised Historical Interpretation → Privacy-Safe Public Representation`.

Candidate principle:

> **Public Historical Knowledge Need Not Expose the Maximum Resolution Preserved by Historical Custody.**

---

## 43. Right to Forget Remains a Real Conflict

Historical 005 identified unresolved conflict between forgetting and preservation.

This pass adds that the conflict is not only “keep vs delete.”

Possible state changes include:

- remove from ordinary search;
- remove identity linkage;
- restrict access;
- anonymise;
- aggregate;
- cold-store;
- seal;
- destroy content while retaining destruction provenance;
- legally retain under bounded access.

Candidate principle:

> **Privacy-Preserving Forgetting Can Operate Through Access, Linkage, Resolution and Discoverability Changes as Well as Destruction.**

This does not solve when destruction is required.

---

## 44. Forgetting Must Not Become Hidden Institutional Exoneration

A participant's legitimate privacy interest and an institution's desire to erase evidence of wrongdoing are not the same claim.

Candidate principle:

> **Right-to-Forget Architecture Must Distinguish Participant Privacy From Institutional Accountability Avoidance.**

This is a major anti-capture requirement.

---

## 45. Group Privacy Exists

Aggregate data can still expose:

- tiny communities;
- rare diseases;
- unusual substrates;
- distinctive cultural groups.

Therefore:

> **Removal of Individual Names ≠ Elimination of Group-Level Privacy Risk.**

Historical aggregation thresholds may need contextual review.

---

## 46. Privacy Can Conflict With Pattern Preservation

The earlier consumer/health example illustrates the conflict precisely.

High-resolution historical data can make later correlations discoverable.

The same resolution can also enable re-identification.

Therefore Historical cannot maximise both future analytical possibility and privacy simultaneously.

Candidate principle:

> **Historical Resolution Is a Stewardship Trade-Off, Not a Free Increase in Knowledge.**

This is a genuine architectural tension rather than a defect that can be eliminated by wording.

---

## 47. Minimum Resolution Must Consider Unknown Future Questions

Strictly minimising data to today's known use can destroy future pattern value.

Retaining maximum detail creates privacy risk.

The current Concord sources do not fully solve this.

A candidate compromise architecture is layered preservation:

- privacy-safe aggregates for broad retention;
- more detailed protected datasets under stronger custody;
- identifiable records only where independently justified;
- time-based review and transformation;
- controlled query rather than unrestricted release.

This is candidate synthesis, not yet canonical architecture.

---

## 48. Historical Privacy Is Relational

The same record can legitimately be:

- visible to the participant;
- partially visible to another affected participant;
- available to a court under authority;
- queryable in anonymised form by research;
- inaccessible to the public;
- discoverable only through protected metadata.

Candidate principle:

> **Historical Privacy Is Not a Binary Property of a Record; It Is a Relationship Among Record, Actor, Action, Purpose, Context and Time.**

This maps directly onto FPA.

---

## 49. Candidate Historical Permission Object

A future Historical permission object may include:

- `Actor`
- `Historical_Object`
- `Action`
- `Purpose/Function`
- `Authority_or_Consent_Basis`
- `Context`
- `Resolution_Level`
- `Identity_Exposure_Level`
- `Conditions`
- `Start`
- `Expiry/Termination`
- `Delegation_Scope`
- `Output_Restrictions`
- `Provenance`
- `Contestability_Path`
- `Status`

This is candidate architecture derived from FPA rather than a replacement for FPA.

---

## 50. Candidate Historical Information-State Stack

The source resolution now supports separating:

1. **Custody** — does Historical preserve it?
2. **Existence visibility** — may an actor know it exists?
3. **Discoverability** — may an actor find it?
4. **Accessibility** — may an actor inspect it?
5. **Resolution** — what detail may be seen?
6. **Correlation** — may it be combined with other information?
7. **Derivation** — may new information be inferred?
8. **Extraction** — may information leave the protected environment?
9. **Disclosure** — may it be shared with a specified recipient?
10. **Publication** — may it become public?
11. **Reuse** — may it be used for another purpose?
12. **Retention** — how long may the relevant representation survive?
13. **Destruction/forgetting** — what may or must cease to exist?

Candidate principle:

> **Historical Information Governance Requires More Than an Access-Control Bit.**

---

## 51. Archive-Stratum Note

Privacy, safe-space, personal-data and permission concepts have earlier Concord ancestry, but the current mature FPA and detailed privacy-learning architecture are substantially developed in the V1.2 corpus.

Older material should therefore be treated as precursor evidence where source-resolved, not automatically as equivalent to the current permission grammar.

The current pass does not justify retroactively describing every older privacy mechanism as FPA.

---

## 52. New Candidate Historical Principles

This pass adds or strengthens:

> **Historical Preservation of Information ≠ Preservation of Every Permission Once Associated With That Information.**

> **Historical Custody ≠ Historical Access.**

> **Permission to Perform One Historical Action ≠ Permission to Perform Another.**

> **Historical Storage of Personal Data ≠ Historical Ownership of the Person's Data.**

> **Archival Transfer ≠ Automatic Termination of Participant Data Rights.**

> **Civilisational Historical Value Does Not Automatically Justify Retention of Identifiable Resolution.**

> **Historical Anonymisation Status Must Remain Sensitive to Re-Identification Risk Over Time.**

> **Permission to Hold Dataset A + Permission to Hold Dataset B ≠ Automatic Permission to Correlate A and B.**

> **Privacy Risk Must Be Evaluated at the Level of Derived Information, Not Only Source Records.**

> **Historical Correlation ≠ Historical Causation.**

> **Historical Transfer Does Not Automatically Flatten the Protection Level of the Context From Which a Record Came.**

> **Historical System Capability ≠ Historical Access Authority.**

> **Retention State ≠ Searchability State.**

> **Historical Metadata Can Itself Be Protected Information.**

> **Age of a Record Does Not Dissolve Purpose Limitation.**

> **Historical Value ≠ Universal Research Permission.**

> **Historical Access Permission ≠ Historical Disclosure Permission.**

> **Historical Access ≠ Historical Publication Authority.**

> **Privacy-Preserving Forgetting Can Operate Through Access, Linkage, Resolution and Discoverability Changes as Well as Destruction.**

> **Removal of Individual Names ≠ Elimination of Group-Level Privacy Risk.**

> **Historical Privacy Is Not a Binary Property of a Record; It Is a Relationship Among Record, Actor, Action, Purpose, Context and Time.**

---

## 53. Current Finding

This pass materially changes the emerging Historical model.

Historical is not merely a custody system with an access-control layer attached.

It is increasingly a **temporally persistent information environment in which preservation state and permission state must remain separate**.

A record can survive while:

- ordinary access expires;
- identity linkage is removed;
- discoverability is reduced;
- research remains possible through bounded queries;
- participant contestation remains possible;
- exceptional access remains separately justified;
- public publication remains prohibited.

The user's earlier observation that **patterns themselves hold useful information** makes this even more important. Correlation and derivation are not passive reading operations. They can create new knowledge and new privacy risks.

The strongest formulation from this pass is:

> **Historical should preserve what civilisation may need to remember without assuming that preservation grants civilisation permanent permission to know everything about everyone.**

**STATUS: SOURCE RESOLUTION CONTINUES.**
