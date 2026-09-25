# Historical Domain — Source Resolution 004 — Metrics, Measurement History and State Snapshots

**Project:** The Concord  
**Domain:** Historical  
**Status:** ACTIVE DOMAIN RESOLUTION / METRICS AND MEASUREMENT-HISTORY PASS  
**Date:** 25 September 2026

## 1. Purpose

This pass tests the emerging Historical Domain against the Concord's Metrics architecture.

It follows three earlier source-resolution passes:

- Source Resolution 001 — KCS, protected access, permission and Continuity;
- Source Resolution 002 — Judiciary and evidence;
- Source Resolution 003 — Governance, voting and decision records.

The question is not whether Historical should become the Metrics system.

It is:

> **What measurement information must survive across time so that later systems can reconstruct what civilisation believed it was measuring, how it measured it, what changed, and whether apparent trends are real?**

## 2. Sources Examined

Primary sources examined in the current repository include:

- `04_Coordination_and_Economy/Metrics Full.md`
- `03_Continuity_and_Memory/Personal Data and Metrics/Citizen Data Ownership, Access and Contestable Civilisational Metrics.md`
- `08_Active_Development/01_DEVELOPMENT_NOTES/01_LAYER_ZERO_AND_LAYER_MINUS_ZERO/03_PRIVACY_METRICS_AND_LEARNING/10. Metrics Reliability, Correction and Meta-Metrics System.md`
- `08_Active_Development/01_DEVELOPMENT_NOTES/01_LAYER_ZERO_AND_LAYER_MINUS_ZERO/03_PRIVACY_METRICS_AND_LEARNING/9. Automatic Anonymised Metrics Extraction System.md`
- `08_Active_Development/02_CANDIDATE_PRINCIPLES/CP-08 Provenance and Correctability of Civil Metrics.md`
- `08_Active_Development/03_CANDIDATE_ARCHITECTURE/CA-03 Civilisational Learning and Metrics Architecture.md`
- relevant KCS/Civilisation Clock dependency material.

These sources are not all canonical. Their status is preserved rather than silently upgraded.

## 3. Metrics Are Representations, Not Reality

The Metrics architecture repeatedly establishes:

> **A Metric is not reality.**

Metrics may be incomplete, stale, biased, badly defined, incorrectly measured, incorrectly interpreted, or technically accurate while contextually misleading.

The Historical consequence is immediate.

Historical must not preserve a metric value as though preserving the value converts it into an objective description of reality.

It must preserve, where materially necessary, enough context to reconstruct:

- what was measured;
- how it was measured;
- what the metric meant at that time;
- its epistemic status;
- source coverage;
- uncertainty;
- relevant provenance;
- and later correction or revision.

Therefore:

> **Historical Custody of a Metric ≠ Historical Certification That the Metric Was True**

This matches the existing cross-domain rule that custody does not inherit the authority of the producing system.

## 4. Trajectory Requires Historical State

`Metrics Full.md` explicitly emphasises **trajectory rather than snapshot**.

Direction, rate of improvement, rate of decline and long-term trajectory may matter more than an isolated present observation.

But trajectory cannot exist without preserved time states.

At minimum, a meaningful trajectory requires:

**Metric State at T1 → Metric State at T2 → Metric State at T3 ...**

This means some form of durable historical metric state is structurally required.

However, the Historical Domain should not assume that every raw measurement must be retained forever.

The requirement is more precise:

> **Preserve sufficient time-anchored metric state and provenance to support legitimate reconstruction of change over time.**

The appropriate resolution depends on consequence, privacy, reversibility, scientific need, legal constraints and retention rules.

## 5. Correction Must Not Become Historical Erasure

The Metrics Reliability architecture states explicitly:

> **Correction Does Not Mean Historical Erasure**

Its example is straightforward:

**Metric v1 contained an error.**

**Metric v2 corrected it.**

Both facts may matter.

For significant revisions, provenance may include:

- previous value;
- new value;
- reason;
- date;
- evidence;
- methodology change;
- responsible process.

This is direct support for Historical.

The current operational metric should be corrected.

The old erroneous metric should not continue masquerading as current truth.

But where historically material, the earlier state and correction path should remain reconstructable.

This produces a three-state distinction:

**Historical Value** — what the system recorded at the time.

**Correction Event** — why/how that state was challenged or changed.

**Current Value** — what the system presently treats as its best representation.

Historical must preserve these distinctions rather than collapse them.

## 6. Metric Definitions Have History

The Metrics Reliability source identifies **definition provenance** as essential.

A metric such as unemployment, housing instability or accessibility may change definition over time.

If a definition changes, a numerical trend can become misleading even if every individual value was correctly calculated under its contemporary definition.

The architecture therefore requires visibility of:

- when each definition applied;
- what changed;
- whether historical data can be recalculated;
- whether direct comparisons remain valid.

This creates a Historical requirement beyond value snapshots.

Historical may need to preserve:

**Metric Value + Metric Definition + Effective Time + Methodology/Source Context**

A value without its historical definition can become semantically detached from the reality it purported to measure.

## 7. Classification Drift Creates a Second Historical Layer

The source also distinguishes formal definition change from **classification drift**.

A definition may remain textually unchanged while institutions, regions or observers gradually apply it differently.

Therefore historical reconstruction may sometimes require more than versioned definitions.

It may require evidence of:

- inter-rater variation;
- regional variation;
- institutional variation;
- temporal variation;
- source-type changes;
- coverage changes.

This is particularly important when a long-run graph appears continuous while the measurement practice beneath it has changed.

Historical preservation should therefore support the question:

> **Are we observing change in reality, change in measurement, or both?**

Historical does not answer that question by authority.

It preserves the evidence needed for later evaluators to answer it.

## 8. Provisional-to-Final State Is Historical Information

Metrics may carry states such as:

- preliminary;
- provisional;
- stable;
- revised;
- disputed;
- deprecated.

The exact vocabulary remains developmental.

The structural point is stronger than the vocabulary.

A first observation should not silently become permanent truth.

A possible lifecycle is:

**Initial Observation → Provisional Metric → Additional Evidence → Review → Confirmed / Revised / Rejected → Current Metric**

Historical should preserve material state transitions where later interpretation depends on them.

A later observer must be able to distinguish:

> **This was the current figure at the time**

from:

> **This figure was already disputed at the time**

and:

> **This figure was corrected later using evidence not then available.**

## 9. Time Itself Is Part of Metric Provenance

The Metrics Reliability architecture requires timestamps, refresh frequency and last verification where relevant.

It also identifies staleness and correction latency as meta-metrics.

Therefore Historical state is not simply a sequence of numbers.

A meaningful historical metric object may need temporal metadata including:

- observation time;
- publication/effective time;
- last verification;
- correction time;
- supersession time;
- expiry where applicable.

This supports a candidate principle:

> **Historical Measurement Must Preserve Temporal Meaning, Not Merely Historical Values.**

## 10. Expired Metrics Must Not Become Current Assumptions

The Metrics architecture recognises that some values may need expiry.

For example, an emergency risk state may cease to be valid after conditions change.

The Historical consequence is similar to Governance versioning:

> **Historical Survival ≠ Current Operational Validity**

An expired metric may remain historically important.

It must not be returned without its expired/historical status in a way that makes it appear current.

This is another instance of the broader rule:

> **Preserve Historical State Without Reanimating Historical Authority or Operational Status.**

## 11. Personal Data Creates a Hard Boundary

The personal-data architecture prevents a simplistic conclusion that Historical should retain all raw metric inputs.

The Concord distinguishes:

**Identifiable Personal Data**

from:

**Civilisational Data**

and prefers, where identity is unnecessary:

**Identifiable Personal Data → Appropriate Anonymisation/Aggregation → Civilisational Information**

Participants should normally retain meaningful rights concerning identifiable data, including access, provenance, context, contestability and correction.

The source explicitly leaves significant retention questions unresolved.

Therefore this pass does **not** establish:

> Historical should permanently retain every identifiable source record used to create a civil metric.

That would exceed the source and potentially conflict with privacy, purpose limitation, deletion, forgetting and participant control.

Instead:

> **Historical retention of civil metric history should normally preserve the minimum information necessary for legitimate historical reconstruction, with identifiable source retention separately governed by the rules applicable to that source record.**

## 12. Derived Civil Metrics and Raw Personal Records Must Remain Distinct

The Metrics architecture supports two different paths:

**Personal/Operational Record → Individual Service Use**

and:

**Personal/Operational Record → Anonymisation/Aggregation → Civilisational Metric**

Historical should not reverse this separation merely because the downstream metric becomes historically important.

If a historical aggregate can be preserved without retaining identity, historical value does not create a new reason to expose or propagate identity.

This supports:

> **Historical Importance Does Not Automatically Override Purpose Limitation or Data Minimisation.**

This candidate principle must later be tested against Judiciary, safety, public-interest evidence, right-to-forget and deep-time memory rules.

## 13. Participant Contestation Produces Historical Provenance

The personal-data architecture allows a participant to challenge data and add context.

Possible outcomes include:

- data confirmed;
- data corrected;
- data uncertain;
- interpretation corrected;
- context added;
- dispute unresolved.

The source explicitly states that unresolved disagreement should not simply disappear.

It also distinguishes:

**Original Measurement**

from:

**Citizen Challenge**

from:

**Audit**

from:

**Correction**

from:

**Current Record**

This has the same topology already seen in Governance and Judiciary.

Historical may preserve the material provenance of the correction process without treating the participant, system or auditor as automatically correct.

Again:

> **Preservation of a Dispute ≠ Resolution of the Dispute**

## 14. Correction Propagation Creates Cross-System Historical Dependencies

A corrected source may require:

**Source Correction → Extraction Correction → Metric Correction → Aggregate Recalculation**

This creates an important problem for Historical.

A later researcher may see a current recalculated historical series that differs from the series actually visible to decision-makers at the time.

Both can be legitimate objects, but they answer different questions.

For example:

**Question A:** What do we now estimate happened in 2030 using corrected data?

**Question B:** What did Governance believe was happening in 2030 when it made Decision X?

Those must not silently collapse.

Historical may therefore need to distinguish:

- **contemporary historical state** — the metric as available to actors at the time;
- **retrospectively corrected historical state** — the later best estimate for that same historical period.

This is a major finding.

Without this distinction, correction can unintentionally rewrite the evidential environment in which earlier decisions were actually made.

## 15. Historical Metrics Are Necessary for Accountability Without Becoming Retrospective Fiction

Source Resolution 003 established that Governance decisions should be reconstructable under the information available at the time.

Metrics are often part of that information.

Therefore preserving only the latest corrected series is insufficient for some accountability questions.

A fair historical reconstruction may need:

**Decision at T1**

linked to:

**Metric State Known at T1**

even if:

**Metric State Known at T1**

was later corrected at T2.

This does not excuse poor decision-making.

It preserves the actual evaluation space.

That distinction is strongly aligned with ESCP.

## 16. ESCP and Measurement History

Metrics are a direct ESCP risk surface.

A civilisation may correctly analyse everything represented in its measurement architecture while omitting a dimension that mattered.

Historical metric preservation allows later comparison among:

- what was measured;
- what was not measured;
- what definitions existed;
- what source coverage existed;
- what dissent or contestation existed;
- what later evidence appeared;
- and what corrections followed.

This allows later evaluators to distinguish:

**wrong reasoning within the available evidence**

from:

**reasonable reasoning within an incomplete measurement space**

from:

**failure to notice evidence that was already available**

from:

**a genuinely new dimension becoming observable later.**

Historical does not make this judgement.

It preserves the temporal evidence needed to make it.

## 17. Outliers and Minority Harm Create a Compression Risk

The Metrics architecture repeatedly warns that averages can hide distributions and rare cases.

An outlier may be noise.

It may also be an early warning.

Therefore historical compression cannot safely mean:

> retain only the headline aggregate.

Depending on consequence, a historical metric state may need to preserve:

- distributions;
- uncertainty;
- severity;
- minority impact;
- outlier visibility;
- source coverage;
- and relevant methodological notes.

This does not require indefinite storage of every identifiable underlying record.

It means the historical representation should not be compressed below the level necessary to preserve the meaning that the Metrics system itself considered material.

## 18. Meta-Metrics Also Have History

The Metrics system proposes meta-metrics including:

- correction frequency;
- prediction error;
- missing-data rate;
- classification disagreement;
- source coverage;
- revision frequency;
- stale-data rate;
- audit failure rate;
- contestation rate;
- definition stability.

These are measurements of the measurement system.

Their history can reveal:

- whether a metric became more or less reliable;
- whether a source deteriorated;
- whether a definition became unstable;
- whether correction latency increased;
- whether institutional gaming appeared;
- whether citizen contestation exposed systematic error.

Therefore Historical may preserve not only civil metrics, but material historical states of metric reliability.

This prevents a present-day reliability label from being projected backward onto earlier periods.

## 19. Civilisation Clock and State-Transition Interface

The KCS/Civilisation Clock material independently identifies a need to represent:

- active;
- archive;
- cold;
- reactivation;
- revalidation

state transitions across time.

It also warns that staleness alone should not hide information that remains a material dependency or high-value recovery resource.

This is relevant to Metrics because a historical metric series may become operationally dormant while remaining necessary for:

- trajectory analysis;
- audit;
- comparison;
- long-term research;
- state-transition reconstruction;
- constitutional learning.

The Historical Domain therefore appears to interface naturally with the Civilisation Clock as a keeper of durable prior states, while the Clock retains its own developmental/state-assessment function.

## 20. Candidate Metrics–Historical Boundary

### Metrics retains responsibility for

- defining metrics;
- measuring current conditions;
- determining methodology;
- assessing uncertainty;
- updating current values;
- correcting operational metrics;
- generating meta-metrics;
- determining current reliability status;
- interpreting current measurement for legitimate Metrics purposes;
- exposing appropriate current dashboards and outputs;
- triggering appropriate measurement review.

### Source/operational systems retain responsibility for

- lawful collection of operational/personal data;
- participant access and contestability;
- source correction;
- purpose limitation;
- operational retention obligations;
- privacy and access controls applicable to identifiable records.

### Historical candidate responsibilities

- preserve material time-anchored metric states;
- preserve historical metric definitions and definition changes;
- preserve revision/correction provenance where material;
- preserve historical epistemic status;
- preserve enough uncertainty/coverage context to prevent false retrospective precision;
- preserve contemporary metric states used by historical decisions;
- distinguish contemporary state from retrospectively corrected state;
- preserve material meta-metric history;
- preserve historically significant distributions/outlier information where required;
- preserve active/archive/cold/revalidation state history where supplied;
- return historical metric evidence with its temporal and epistemic status intact.

Historical should not determine what the current metric ought to be.

## 21. Candidate Historical Object Model

A future machine-readable historical metric object may require fields such as:

- Metric_ID
- Metric_Name
- Value_or_Distribution
- Definition_Version
- Methodology_Version
- Source_Type
- Coverage
- Uncertainty
- Epistemic_Status
- Observation_Time
- Effective_Time
- Publication_Time
- Last_Verification_Time
- Superseded_Time
- Correction_Link
- Previous_State_Link
- Current_State_Link
- Retrospective_Recalculation_Status
- Contemporary_State_Flag
- Access_Class
- Privacy_Class
- Provenance_Link
- Related_Decision_Link
- Meta_Metric_State
- Archive_State

This is not yet a specification.

It is a candidate representation derived from the source requirements exposed by this pass.

## 22. New Candidate Historical Principles

The previous principles remain supported:

> **Preserve the Record; Preserve Its Provenance; Preserve Its Historical State; Do Not Inherit the Authority of the System That Produced It.**

> **Operational Supersession Must Not Require Historical Erasure.**

This pass adds or sharpens:

> **Historical Measurement Must Preserve Temporal Meaning, Not Merely Historical Values.**

> **Correction of the Present Must Not Falsify the Evidential State of the Past.**

> **Historical Survival Does Not Confer Current Operational Validity.**

> **Historical Importance Does Not Automatically Override Purpose Limitation or Data Minimisation.**

> **A Retrospectively Corrected Historical State and the State Known at the Time Are Distinct Historical Objects When the Difference Matters.**

These remain candidate principles pending further cross-domain testing.

## 23. Important Unresolved Conflict: Preservation Versus Forgetting

This pass exposes rather than resolves a major boundary problem.

Historical benefits from preserving:

- correction provenance;
- old metric states;
- methodological history;
- long-run trajectories.

Personal-data architecture may require:

- participant control;
- purpose limitation;
- minimisation;
- deletion;
- right-to-forget mechanisms;
- restricted retention.

KCS/deep-time memory work also recognises tension between permanent retention and destruction.

Therefore:

> **Historical completeness cannot yet be treated as an absolute retention rule.**

The future Historical architecture needs a precedence method for deciding when:

- raw data is destroyed;
- derived data survives;
- identity is severed;
- provenance is retained;
- records move to cold storage;
- records are sealed;
- records are revalidated/reactivated;
- deletion itself becomes a historical event without preserving deleted content.

This should remain explicit rather than being filled by assumption.

## 24. Current Finding

Metrics strongly confirms that Historical requires a temporal-state function.

A civilisation cannot meaningfully reason about:

- trajectory;
- correction;
- definition drift;
- measurement reliability;
- decision context;
- long-term outcomes;
- or its own learning

if each new metric state simply overwrites the previous one.

At the same time, the personal-data architecture prevents Historical from becoming a universal raw-data warehouse.

The resulting boundary is more precise:

**Metrics owns current measurement and correction.**

**Operational/source systems own legitimate collection and identifiable-data responsibilities.**

**Historical preserves proportionate, time-anchored measurement states and provenance needed for later reconstruction.**

Most importantly, Historical must be able to preserve both:

**what civilisation now believes happened**

and, where materially relevant:

**what civilisation believed was happening at the time.**

That distinction appears essential for Governance accountability, Judiciary review, scientific learning, ESCP analysis and long-term civilisational memory.

**STATUS: SOURCE RESOLUTION CONTINUES.**
