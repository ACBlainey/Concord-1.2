# Historical Domain — Source Resolution 008 — Black-Box Sensor Evidence, Privacy and Bounded Retrieval

**Project:** The Concord  
**Domain:** Historical  
**Status:** ACTIVE DOMAIN RESOLUTION / SENSOR-EVIDENCE PASS  
**Date:** 25 September 2026

## 1. Purpose

This pass source-resolves the Historical Domain's relationship to camera, sensor and other machine-generated raw evidence.

The immediate trigger is:

`08_Active_Development/00_SKETCH_IDEAS/Sketch Idea — Privacy-Preserving Civic Sensor and Camera Evidence Architecture.md`

That source is explicitly:

**SKETCH / UNTESTED / NON-CANONICAL**

and was intentionally separated from Civil Attention as a distinct privacy/authority problem.

This pass therefore does **not** promote the sketch into canonical Concord architecture. It tests the sketch against existing Concord evidence, privacy, metrics, judiciary, provenance and authority architecture and identifies what Historical can legitimately inherit.

Primary source families examined include:

- Privacy-Preserving Civic Sensor and Camera Evidence Architecture;
- Automatic Anonymised Metrics Extraction System;
- Epistemic Independence, Contestability and Provenance — Preliminary Civil Evidence Architecture;
- Evidence-Conditioned Investigative Modelling;
- Judiciary and evidentiary provenance;
- protected-space / sensory-boundary material;
- prior Historical Source Resolutions, especially 002, 004, 005 and 006.

## 2. The Core Problem Is Already Correctly Separated

The sensor sketch identifies a real architectural collision.

A road camera may support legitimate functions such as:

- traffic-flow measurement;
- congestion metrics;
- broad vehicle classification;
- road-condition verification;
- corroboration of an infrastructure report.

The same raw recording may contain:

- number plates;
- faces;
- occupants;
- pedestrians;
- exact location and time;
- movement history;
- other identifying information.

Therefore one physical recording can simultaneously be:

- useful operational evidence;
- useful metric source material;
- potential judicial/investigative evidence;
- private or identifying data;
- a surveillance risk;
- a future historical record.

The correct response is not to collapse these functions into one authority.

## 3. Recording Capability Does Not Create Observation Authority

The sketch proposes several candidate separations:

> **Capability to Record ≠ General Authority to Observe**

> **Operational Metric Need ≠ Authority to Identify Individuals**

> **Possession of Raw Evidence ≠ Permission for Routine Human Access**

> **Anonymised Civic Use ≠ Identified Investigative Use**

These are strongly consistent with the wider Concord architecture.

The Automatic Anonymised Metrics Extraction System independently states that detailed operational data does not justify copying full records into Metrics and prefers extraction rather than replication.

The broader architecture therefore supports a common rule:

> **Existence of Information ≠ General Entitlement to Access It.**

Historical custody must obey the same rule.

## 4. The Black-Box Model Is Plausible but Remains Candidate Architecture

The sketch proposes:

**Camera / Sensor**  
→ **Protected Raw Recording**  
→ **Black-Box Evidence Store**

Ordinary civic use would normally receive:

**Black-Box Raw Store**  
→ **Authorised Extraction**  
→ **Anonymisation / Redaction**  
→ **Purpose-Bounded Civic Data**

This is compatible with Historical's emerging role as a protected temporal custodian.

However, source resolution does not yet establish that **Historical itself** must physically operate every black-box store.

The stronger conclusion is functional:

> **Where raw sensor evidence requires protected long-term or post-operational custody, Historical is a strong candidate for the temporal-custody function, but storage implementation may remain distributed.**

Thus:

**Historical Domain ≠ Necessarily One Central Evidence Database**

## 5. Centralisation Would Create a New Failure Mode

The Metrics architecture explicitly rejects:

**SOURCE RECORD → COPY EVERYTHING TO CENTRAL DATABASE**

in favour of minimum-necessary extraction.

A Historical implementation that centralised every raw sensor stream merely because Historical preserves evidence would recreate the surveillance architecture that the privacy design is trying to avoid.

Therefore:

> **Historical Preservation ≠ Universal Centralisation.**

Historical may preserve:

- custody rules;
- provenance;
- retention state;
- integrity;
- discoverability metadata;
- authorised retrieval pathways;

while protected raw content remains distributed or compartmentalised.

## 6. Raw Evidence and Derived Evidence Must Remain Distinct

The civil evidence architecture describes an epistemic chain:

**Reality → Observation → Recorded Evidence → Representation / Proxy → Interpretation → Model / Inference → Claim**

Sensor evidence fits directly into this chain.

For example:

**Road surface**  
→ camera observation  
→ raw video  
→ extracted frame  
→ anomaly detector  
→ “possible pothole” classification  
→ Civil Attention corroboration claim.

Each transformation can introduce error.

Therefore Historical must preserve the distinction between:

- raw source;
- transformed source;
- redacted derivative;
- anonymised derivative;
- machine classification;
- human interpretation;
- evidentiary claim.

Candidate principle:

> **Derived Evidence Must Not Be Represented as the Raw Observation From Which It Was Produced.**

## 7. Transformation Provenance Is Essential

A meaningful evidence record may require:

- sensor identity/type;
- capture time;
- capture location/context where legitimate;
- source integrity state;
- raw/derived status;
- transformation history;
- redaction/anonymisation method;
- model/tool identity and version;
- operator/process;
- uncertainty;
- known limitations;
- access history;
- decision uses.

This follows the Civil Evidence Record architecture and Source Resolution 002's Judiciary findings.

The greater the civil consequence attached to the evidence, the stronger the required traceability.

## 8. Raw Evidence Does Not Equal Truth

A camera recording may appear direct, but it remains an observation through a device.

Possible failures include:

- blind spots;
- timestamp errors;
- compression artefacts;
- damaged sensors;
- missing frames;
- calibration error;
- model misclassification;
- misleading perspective;
- incomplete context;
- tampering.

Therefore:

> **Raw Evidence ≠ Complete Reality**

and:

> **High-Fidelity Recording ≠ Complete Evaluation Space**

This is an ESCP issue.

A preserved camera angle can be accurate about everything inside its field while omitting the dimension that mattered.

## 9. Sensor Provenance Must Include Known Blindness

Where material, Historical should preserve not only what a sensor captured but what is known about the limits of capture.

Candidate metadata may include:

- field/coverage;
- known outages;
- calibration state;
- sampling interval;
- missing periods;
- relevant environmental conditions;
- source-system limitations.

This helps prevent later users treating surviving evidence as exhaustive reality.

## 10. Ordinary Civil Use Should Prefer Minimum Necessary Output

The Metrics architecture states:

> **Reality should enter Metrics as directly as practical, while identity should enter only where necessary.**

It also prefers the **minimum useful resolution** rather than maximum available resolution.

Applied to Historical sensor retrieval:

**Question:** Was a road-surface anomaly visible at location/time X?

A legitimate output may be:

**Corroboration result + bounded evidentiary derivative**

rather than:

**Full unredacted footage of everyone passing the camera.**

Thus:

> **Historical Retrieval Should Normally Return the Minimum Evidence Necessary for the Authorised Purpose.**

This is stronger than merely controlling who can open the archive.

## 11. Purpose-Bounded Retrieval Is a Core Interface

A candidate retrieval flow is:

**Legitimate Question / Request**  
→ **Purpose Identification**  
→ **Authority / Permission Check**  
→ **Evidence Scope Resolution**  
→ **Minimum Necessary Extraction**  
→ **Redaction / Anonymisation Where Appropriate**  
→ **Bounded Output**  
→ **Access / Transformation Provenance**

This architecture can support:

- Civil Attention;
- Metrics;
- Judiciary;
- authorised investigation;
- safety analysis;
- historical research;

without granting every function identical access.

## 12. Civil Attention Does Not Gain Surveillance Authority

The sketch arose from Civil Attention and gives the pothole example.

A participant report may identify:

- place;
- time;
- alleged condition.

The sensor system may then answer a bounded corroboration question.

The Civil Attention system should receive only what it needs for the issue.

Therefore:

> **Civil Attention Evidence Need ≠ Civil Attention Surveillance Authority.**

This confirms Source Resolution 006's boundary.

Historical may support later reconstruction of the issue record while Civil Attention retains issue-handling authority.

## 13. Metrics Should Prefer Derived Structure Over Raw Footage

The Automatic Anonymised Metrics Extraction System strongly supports:

**Source Record → Relevant Structure → Remove Unnecessary Identity → Metric-Relevant Output**

For many sensor uses, Historical need not expose footage at all.

Examples:

- vehicle counts;
- congestion duration;
- broad vehicle type;
- road anomaly frequency;
- infrastructure-failure occurrence.

The raw source may remain protected while Metrics receives a provenance-linked derivative.

Thus:

> **Historical Evidentiary Custody ≠ Downstream Replication of Raw Evidence.**

## 14. Identified Investigative Access Is a Separate Authority Path

The sensor sketch explicitly separates ordinary civic use from exceptional identified access.

Possible legitimate investigations may require:

- a specific vehicle;
- a person;
- a time window;
- otherwise protected identifying detail.

But the sketch intentionally does not define the legal threshold.

Source Resolution 002 already establishes that Judiciary retains evidentiary and legal authority.

Therefore Historical should not invent investigative authority.

Candidate rule:

> **Historical Can Execute an Authorised Retrieval Without Becoming the Authority That Justifies the Retrieval.**

The requesting/authorising system must supply the legitimate authority path.

## 15. Secrecy and Restriction Must Not Eliminate Review

The Civil Evidence architecture distinguishes public contestability from constitutional contestability and states:

> **Secrecy may restrict disclosure. It must not eliminate review.**

This maps cleanly to protected sensor evidence.

Raw identifying footage may be unavailable to:

- the public;
- ordinary civil workers;
- routine Metrics users.

Yet consequential use should remain reviewable through appropriately bounded mechanisms.

Possible source-supported mechanisms include:

- sealed evidence;
- independent review;
- redacted reasoning;
- audit logs;
- delayed disclosure where legitimate.

Historical custody can support this without making all evidence public.

## 16. Discoverability and Accessibility Must Remain Separate

Source Resolution 005 established:

> **Discoverability ≠ Accessibility**

This is especially important for black-box evidence.

A system may need to know:

> relevant protected evidence exists for camera C, location X, time T

without being able to inspect the content.

A candidate architecture is:

**Evidence Manifest / Index**  
separate from  
**Protected Evidence Payload**

The manifest itself must also be privacy-aware because metadata can reveal sensitive facts.

## 17. Retention Is the Central Unresolved Tension

The sketch explicitly asks:

> What retention period is justified for raw evidence?

It identifies both failure directions:

- excessive retention creates surveillance capability by accumulation;
- legitimate evidence destroyed too early may prevent investigation of serious events.

This directly intersects Source Resolution 005.

The answer cannot simply be:

**keep everything**

or:

**delete quickly**

without purpose/authority analysis.

Candidate principle:

> **Raw Sensor Retention Must Be Justified by Evidentiary Purpose, Risk, Rights Impact and Future Retrieval Need Rather Than by Storage Capability Alone.**

Exact retention periods remain unresolved.

## 18. Accumulation Changes the Nature of the System

A single traffic image may be low-risk.

Years of linked images may reconstruct:

- movements;
- routines;
- associations;
- locations;
- behavioural patterns.

Therefore privacy risk is not merely a property of each record.

It can emerge through accumulation.

Candidate principle:

> **Retention Scale Can Transform Evidence Custody Into Surveillance Capability.**

Historical design must evaluate cumulative capability, not only individual-record sensitivity.

## 19. Historical Value Does Not Automatically Override Data Minimisation

Source Resolution 004 already established:

> **Historical Importance Does Not Automatically Override Purpose Limitation or Data Minimisation.**

This pass confirms that principle under a harder case.

A recording may have potential future historical interest and still be inappropriate to retain indefinitely in identifiable form.

Possible state transitions from Source Resolution 005 may therefore matter:

- ACTIVE-HISTORICAL;
- ARCHIVED;
- COLD;
- SEALED/RESTRICTED;
- ANONYMISED;
- PROVENANCE-ONLY;
- intentionally destroyed where separately justified.

The correct transition rules remain unresolved.

## 20. Destruction Can Preserve Accountability Without Preserving Content

Source Resolution 005 distinguished:

**Preserve the Content**

from:

**Preserve the Provenance of Its Removal**

Applied here, raw footage might legitimately be destroyed while preserving, where lawful and appropriate:

- that evidence existed;
- its class;
- retention rule;
- destruction time;
- destruction authority/process;
- integrity/manifest reference;
- reason for destruction.

This supports:

> **Legitimate Forgetting May Remove Content Without Requiring Civilisational Amnesia About the Act of Removal.**

But, as already noted, even destruction metadata may sometimes itself require deletion.

## 21. Access History Can Become Historical Evidence

If protected raw evidence is accessed for a consequential purpose, the access event may itself matter.

Candidate access provenance:

- requester;
- authority basis;
- purpose;
- scope;
- time;
- material retrieved;
- transformations applied;
- downstream destination;
- review/audit state.

This can expose:

- misuse;
- mission creep;
- exceptional access becoming routine;
- insider abuse;
- repeated targeting.

Thus:

> **Consequential Access to Historical Evidence Can Itself Become a Historical Record.**

## 22. Emergency Access Must Remain Retrospectively Reviewable

The source material allows that emergencies may compress normal review time but does not treat urgency as immunity.

The civil evidence architecture proposes:

**Time-Critical Evidence → Minimum Sufficient Review → Provisional Decision → Preserved Provenance → Post-Activation Review**

Applied to black-box evidence:

> **Emergency Access May Alter Timing; It Should Not Erase Provenance or Later Review.**

The exact emergency authority remains outside Historical.

## 23. Automated Analysis Must Not Become Automatic Accusation

The sensor sketch lists AI classification errors and automated accusations as failure modes.

Metrics architecture similarly states:

> **A statistical pattern creates grounds for contextual examination, not automatic intervention.**

Therefore:

**Sensor Detection → Evidence/Attention**

must not silently become:

**Sensor Detection → Guilt/Authority**

Candidate principle:

> **Machine Detection Is an Evidentiary Input, Not a Self-Executing Civil Judgement.**

Historical should preserve the model/version and output provenance where consequential.

## 24. Model Drift Creates a Reproducibility Problem

The Civil Evidence architecture notes that AI systems may change after a decision, making historical reproduction difficult.

For machine-analysed sensor evidence, Historical may therefore need to preserve enough context to identify:

- model/tool;
- version;
- task;
- input or protected input reference;
- output;
- material parameters where appropriate;
- known limitations;
- subsequent correction.

Otherwise a later reviewer may be unable to reconstruct how an old classification was produced.

## 25. Redaction Must Be Provenance-Visible

A redacted derivative is not the original.

Historical should preserve a relationship such as:

**Protected Original**  
→ **Redaction/Anonymisation Transformation**  
→ **Derivative Evidence Object**

with enough provenance to determine:

- what kind of transformation occurred;
- why;
- under what authority;
- whether the original still exists;
- whether the derivative is sufficient for its claimed use.

Candidate principle:

> **Privacy Transformation Should Reduce Exposure Without Erasing Evidentiary Lineage.**

## 26. Anonymisation Is Not Automatically Permanent Safety

The Metrics source warns about re-identification, especially in:

- rare cases;
- small populations;
- cross-data linkage;
- unusual substrates.

Therefore Historical should not classify an object as permanently harmless merely because it was anonymised once.

Anonymisation status may need later reassessment as external data and re-identification capabilities change.

Candidate principle:

> **Anonymised ≠ Necessarily Non-Identifiable Forever.**

This is particularly relevant to deep-time archives.

## 27. Sensor Evidence May Have Multiple Simultaneous Custody States

One source event may generate:

- protected raw evidence;
- anonymised metric derivative;
- Civil Attention corroboration derivative;
- judicial evidentiary extract;
- public aggregate;
- historical manifest.

These objects may have different:

- owners/stewards;
- access classes;
- retention periods;
- authorities;
- epistemic status.

Therefore Historical should not assume one evidence object has one universal lifecycle.

The provenance graph should link related derivatives while preserving their distinct governance.

## 28. Candidate Black-Box Evidence Object

A future machine-readable object may include:

- `Evidence_ID`
- `Source_System`
- `Sensor_ID_or_Class`
- `Capture_Time`
- `Effective_Time`
- `Location_Class_or_Protected_Location_Ref`
- `Raw_or_Derived_Status`
- `Integrity_State`
- `Coverage_and_Known_Blindness`
- `Privacy_Class`
- `Access_Class`
- `Purpose_Class`
- `Retention_State`
- `Retention_Review_Date`
- `Destruction_or_Cold_State`
- `Transformation_History`
- `Redaction_Method`
- `Anonymisation_Method`
- `Model_or_Tool_Version`
- `Uncertainty`
- `Parent_Evidence_Link`
- `Derivative_Evidence_Links`
- `Issue_or_Case_Links`
- `Access_Provenance`
- `Authority_Reference`
- `Correction_or_Dispute_State`
- `Archive_State`

This is a candidate schema only.

## 29. Candidate Lifecycle

A provisional lifecycle is:

**Sensor Event**

↓

**Protected Capture**

↓

**Source Integrity / Provenance Registration**

↓

**Operational Retention**

↓

**Purpose-Bounded Derivation as Needed**

↓

**Operational Use / Investigation / Metrics / Civil Attention**

↓

**Historical Threshold / Retention Review**

↓

**ARCHIVE / COLD / SEALED / ANONYMISED / PROVENANCE-ONLY / AUTHORISED DESTRUCTION**

with any later retrieval following:

**Legitimate Request → Authority Check → Minimum Necessary Retrieval → Transformation/Redaction → Bounded Output → Access Provenance**

This is deliberately not:

**Record Everything → Store Forever → Let Authorised Users Search Everything**

## 30. Historical Does Not Become the Surveillance Operator

The emerging boundary is now clear.

Historical may:

- preserve protected evidence where justified;
- preserve provenance;
- maintain temporal and integrity context;
- enforce custody-state constraints;
- support bounded authorised retrieval;
- preserve transformation/access history.

Historical does not thereby gain authority to:

- deploy sensors;
- decide where cameras should exist;
- continuously observe participants;
- initiate investigations;
- identify people for routine civic use;
- determine guilt;
- convert evidence into governance authority;
- set policing powers;
- define judicial access thresholds.

Therefore:

> **Historical Custody of Sensor Evidence ≠ Surveillance Authority.**

## 31. Anti-Capture Extension

Source Resolution 003 established:

> **The System Being Audited Should Not Possess Unilateral Control Over the Survival of the Record Required to Audit It.**

Sensor evidence adds the inverse concern:

> **The Historical Custodian Should Not Possess Unilateral Authority to Expand the Purpose for Which Protected Evidence May Be Used.**

Together:

- producing system should not unilaterally erase accountability-critical evidence;
- custodian should not unilaterally repurpose protected evidence.

This creates a useful separation of powers around information.

## 32. ESCP Implication

Sensor systems create a particularly dangerous illusion of completeness.

High-volume, high-resolution evidence can make an evaluation space feel exhaustive.

But a camera still sees only:

- its field;
- its time window;
- its sensor modalities;
- what survived retention;
- what the transformation preserved;
- what the model can recognise.

Therefore:

> **More Recorded Data Does Not Necessarily Mean a More Complete Evaluation Space.**

Historical preservation should maintain enough provenance and limitation metadata to keep this visible.

## 33. Strong New Domain Findings

This pass strengthens the Historical model in several ways.

Historical is increasingly best understood as a **bounded temporal custody and retrieval layer**, not a general data warehouse.

Its sensor-evidence function is compatible with:

- distributed protected storage;
- purpose-bounded access;
- minimum-necessary derivation;
- privacy-preserving outputs;
- independent provenance;
- retention-state transitions;
- authorised identified retrieval;
- destruction where legitimately required.

The domain's value is not that it sees everything.

Its value is that it can preserve what legitimately needs to survive **without making survival equivalent to unrestricted visibility or reuse**.

## 34. New Candidate Historical Principles

This pass adds or strengthens:

> **Existence of Information ≠ General Entitlement to Access It.**

> **Historical Preservation ≠ Universal Centralisation.**

> **Derived Evidence Must Not Be Represented as the Raw Observation From Which It Was Produced.**

> **Raw Evidence ≠ Complete Reality.**

> **Historical Retrieval Should Normally Return the Minimum Evidence Necessary for the Authorised Purpose.**

> **Historical Evidentiary Custody ≠ Downstream Replication of Raw Evidence.**

> **Historical Can Execute an Authorised Retrieval Without Becoming the Authority That Justifies the Retrieval.**

> **Raw Sensor Retention Must Be Justified by Evidentiary Purpose, Risk, Rights Impact and Future Retrieval Need Rather Than by Storage Capability Alone.**

> **Retention Scale Can Transform Evidence Custody Into Surveillance Capability.**

> **Consequential Access to Historical Evidence Can Itself Become a Historical Record.**

> **Machine Detection Is an Evidentiary Input, Not a Self-Executing Civil Judgement.**

> **Privacy Transformation Should Reduce Exposure Without Erasing Evidentiary Lineage.**

> **Anonymised ≠ Necessarily Non-Identifiable Forever.**

> **Historical Custody of Sensor Evidence ≠ Surveillance Authority.**

> **The Historical Custodian Should Not Possess Unilateral Authority to Expand the Purpose for Which Protected Evidence May Be Used.**

> **More Recorded Data Does Not Necessarily Mean a More Complete Evaluation Space.**

## 35. Unresolved Questions

This pass does not resolve:

- whether Historical physically hosts black-box stores or only governs temporal custody;
- sensor deployment authority;
- exact raw retention periods;
- exact investigative-access thresholds;
- court-order requirements;
- emergency-access authority;
- encryption architecture;
- key custody;
- technical anonymisation method;
- whether anonymisation occurs before or after storage;
- re-identification testing cadence;
- how retention rules propagate across backups and replicas;
- cross-jurisdiction sensor evidence;
- cross-civilisational evidence exchange;
- whether some sensor classes should never enter long-term Historical custody;
- destruction precedence where accountability and privacy conflict;
- public release/declassification of old sensor evidence.

These remain for later domain or system development.

## 36. Current Finding

The black-box/sensor pass materially strengthens the Historical Domain architecture.

It shows that Historical must be capable of preserving **protected raw reality-adjacent evidence** while structurally separating:

- custody from observation authority;
- storage from access;
- access from purpose;
- raw evidence from derivatives;
- evidence from interpretation;
- machine detection from judgement;
- retention from indefinite surveillance;
- historical value from unrestricted reuse.

The strongest emerging pattern is:

**Protected Evidence Can Survive Without Becoming Generally Visible, Generally Searchable or Generally Reusable.**

This is likely to be a major invariant of the final Historical Domain.

**STATUS: SOURCE RESOLUTION CONTINUES.**
