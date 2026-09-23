# Contextual Wrapper Architecture — BTT-001 Source-Recovery and ESCP Audit

**Target:** Contextual Wrapper Architecture — Portable Specification v0.1c  
**Trigger:** Blind Transfer Test 001 post-test findings  
**Audit type:** Targeted source-recovery / extraction-completeness audit  
**Status:** COMPLETED — MAJOR SOURCE RECOVERY IDENTIFIED  
**Date:** September 2026  
**Project origin:** The Concord  
**Author:** Alexander C. Blainey

---

## 1. Purpose

Blind Transfer Test 001 exposed several apparent weaknesses in CWA v0.1c.

Before treating those findings as new architectural gaps, this audit returns to the original Concord wrapper corpus and asks:

> **Was the relevant architecture already developed in the source material but incompletely transferred into the portable CWA specification?**

This audit is explicitly governed by the Concord's **Evaluation-Space Completeness Problem (ESCP)**.

The relevant ESCP constraint is:

> **Failure to find a solution inside the currently represented or searched space does not establish that the solution does not exist outside that space.**

For this audit:

> **Not represented in the handover ≠ not present in the Concord.**

> **Not present in CWA v0.1c ≠ not developed in the CWA source architecture.**

Therefore an apparent portable-module deficit must pass through source resolution before it is classified as a source-architecture deficit.

---

## 2. Why ESCP is materially relevant here

CWA development crossed an instance handover.

The receiving instance inherited:

- the portable-module development state;
- a summary of prior reasoning;
- identified source files;
- selected architectural conclusions.

It did **not** inherit the complete active representational space available during the original wrapper discussions.

This created a predictable ESCP risk:

**Original Development Space**  
→ **Documents + Conversation + Working Context**  
→ **Handover Representation**  
→ **Portable Extraction**  
→ **Blind Test**  
→ **Apparent Deficit**

At each compression or transfer boundary, architecture may remain present in the source corpus while disappearing from the immediately represented evaluation space.

BTT-001 therefore tests two things at once:

1. whether CWA v0.1c transfers successfully; and
2. whether the extraction into v0.1c preserved enough of the source architecture.

A deficit in (2) must not automatically be classified as a deficit in the original architecture.

---

## 3. Classification states

Each BTT-001 finding is classified as:

- **SOURCE-PRESENT / UNDER-EXTRACTED** — substantially developed in source; recover before inventing.
- **SOURCE-PARTIAL / REFINEMENT NEEDED** — source establishes the principle but portable formalisation or implementation remains incomplete.
- **GENUINELY OPEN IN REVIEWED SPACE** — reviewed source does not provide enough architecture to resolve the issue.
- **UNKNOWN OUTSIDE REVIEWED SPACE** — no claim of corpus-wide absence is justified without broader source resolution.

The final two states are deliberately separated because of ESCP.

---

## 4. Sources reviewed

Primary:

- **Fractal Contextual Wrappers — A Universal Concord Grammar for Bounded Rule, Behavioural and Jurisdictional Variation**

Supporting wrapper sources:

- **Concord Wrapper Procedural Architecture — Context, Information, Consent and Autonomy Across Civilisational Boundaries**
- **Fractal Permission Architecture — Context, Function and Minimum Necessary Access Across Public, Private and Safe Spaces**
- **Functional Priority and Protective Authority — Decision Competence, Safety, Rights and the Limits of Organisational Command**
- **Minimum Necessary Capability — A Concord Architecture for the Justification, Bounding and Termination of Power and Permission**
- **Concord Civilisational Wrappers — Foundational Boundary, Mobility and Responsibility Architecture**
- **Concord Wrapper Non-Governance and Optional Mediation Principle**

Methodological control:

- **06_Portable_Modules/Evaluation-Space Completeness Problem — A Portable Model of Correct Evaluation Within an Incomplete Representational Space.md**

---

# 5. Finding-by-finding source recovery

## 5.1 Precedence and overlapping contexts

### BTT-001 apparent deficit

CWA can identify competing contextual claims but v0.1c does not provide a complete precedence algorithm.

### Recovered source architecture

The primary Fractal Contextual Wrappers paper contains a dedicated **Rule Precedence** section:

> **The architecture requires explicit precedence.**

It gives a preliminary hierarchy in which constitutional invariants constrain rights-incompatible contextual rules, while legitimate domain-specific rules may override ordinary defaults within their permitted scope.

The source then explicitly records:

> **The exact precedence model requires further work.**

A separate **Context Composition** section models overlapping contexts:

**Boxing Context + Medical Emergency Context → Temporary Composite State**

and states:

> **Wrapper Composition Requires Explicit Conflict and Priority Rules.**

### Classification

**SOURCE-PRESENT / UNDER-EXTRACTED**, with the exact general precedence model **GENUINELY OPEN IN REVIEWED SPACE**.

### v0.2 consequence

Recover explicit:

- precedence representation;
- composite contextual states;
- conflict/priority relationships;
- known versus unresolved precedence.

Do not manufacture a universal hierarchy beyond the source.

---

## 5.2 Emergency composition and authority

### BTT-001 apparent deficit

Emergency composition needs a stronger interface.

### Recovered source architecture

Fractal Contextual Wrappers states:

> **Contextual Consent ≠ Irrevocable Exposure to Harm**

and requires emergency override to remain bounded and justified.

Minimum Necessary Capability develops the authority side extensively through **Time-Critical Assumed Authority**.

It distinguishes:

> **Assumed Authority ≠ Assumed Consent**

and requires exceptional authority to be minimum sufficient, responsibility-bearing, reviewable and terminated when its basis ends.

It also states:

> **Emergency Need ≠ Unlimited Emergency Authority**

### Classification

**SOURCE-PRESENT / UNDER-EXTRACTED.**

### v0.2 consequence

CWA should expose the existing interface rather than duplicate the entire MNC architecture:

**Emergency Context Activation → Required Emergency Function → Existing/Assumed Authority Basis → Minimum Necessary Capability → Retained Protections → Conflict/Precedence State → Responsibility → Termination → Review**

---

## 5.3 Termination, reversion and temporary capability

### BTT-001 apparent deficit

Agent permissions, credentials, delegated capabilities and persistent information require stronger termination/reversion treatment.

### Recovered source architecture

The original wrapper grammar already includes:

**Terminate Context → Revert to Surrounding Norms**

and:

> **Context Start and Context End Should Be Legible Where Material.**

Its authority chain ends with authority ending when the function/context ends.

Minimum Necessary Capability adds:

> **Temporary Need Should Normally Produce Temporary Capability.**

and:

> **Function Completion Should Normally Terminate Function-Derived Capability.**

### Classification

**SOURCE-PRESENT / UNDER-EXTRACTED** for authority and permission termination.

**SOURCE-PARTIAL / REFINEMENT NEEDED** for residual state such as derived data, copied information, cached state, continuing autonomous processes and external-service artefacts.

### v0.2 consequence

Restore the source termination architecture first, then separately represent:

- active permission;
- delegated capability;
- credential;
- ongoing process;
- retained or derived information;
- external copy/service dependency;
- revocation propagation.

The second group is a refinement of an existing principle, not a new foundation.

---

## 5.4 Human, machine and operational representations

### BTT-001 apparent deficit

CWA needs a stronger mechanism for divergence among human-facing, machine-readable and executable/observed contexts.

### Recovered source architecture

Fractal Contextual Wrappers explicitly describes:

**Human-readable signage**

and:

**Machine-readable contextual metadata**

as representations of the same underlying context.

Its enumerated failure modes include:

> **machine-readable and human-readable rules diverging**

and:

> **declared context diverging from reality**

The same source contains a reality-correction/ratchet sequence:

**Rule introduced → Unexpected harm observed → Evidence recorded → Context reviewed → Rule modified → Outcome re-evaluated**

### Classification

**SOURCE-PRESENT / UNDER-EXTRACTED** for equivalence and divergence detection.

**SOURCE-PARTIAL / REFINEMENT NEEDED** for a formal three-way reconciliation interface.

### v0.2 consequence

Recover the original requirement and formalise, where useful:

**Human-readable declaration ↔ Machine-readable declaration ↔ Executable / Observed reality**

Material divergence should trigger review rather than silently selecting one representation as authoritative.

---

## 5.5 Materiality and sufficient legibility

### BTT-001 apparent deficit

Materiality and legibility thresholds are domain-sensitive.

### Recovered source architecture

The original wrapper paper states:

> **Information Burden Should Be Proportionate to Material Contextual Difference and Risk.**

It explicitly contrasts low-overhead ordinary contexts with high-risk contexts requiring substantial instruction.

It also states:

> **The Concord standardises legibility more strongly than it standardises outcomes.**

Success criteria use **sufficiently legible**, not one universal signalling mechanism.

The procedural wrapper paper repeatedly uses **materially relevant** conditions and leaves the distinction between material contextual difference and arbitrary classification as a contextual research problem.

### Classification

**SOURCE-PRESENT / UNDER-EXTRACTED.**

### v0.2 consequence

Restore proportionality and sufficient-legibility language. Do not impose universal signage, disclosure volume or fixed materiality thresholds.

---

## 5.6 External resolution and wrapper non-sovereignty

### BTT-001 apparent deficit

CWA needs a clearer interface for conflicts it exposes but cannot resolve.

### Recovered source architecture

The procedural wrapper architecture states:

> **Information Architecture ≠ Decision Authority**

and:

> **Schema Authority Is Not Sovereignty**

The Non-Governance and Optional Mediation Principle establishes that a wrapper can define the questions that must be legible without acquiring authority to determine every answer.

Mediation is a separate function requiring its own legitimate authority, scope, consent, accountability and termination.

It states:

> **Wrapper Use ≠ Consent to Mediation**

> **Mediation Capability ≠ Mediation Authority**

### Classification

**SOURCE-PRESENT / UNDER-EXTRACTED.**

### v0.2 consequence

Make the external-resolution interface explicit:

**Conflict Detected → Existing Resolver Identified? → Resolver Authority Verified → Resolution External to Wrapper → Resolution Recorded → Affected Contexts Updated**

If no legitimate resolver is established:

**UNKNOWN / DISPUTED / REQUIRES EXTERNAL RESOLUTION**

must remain valid terminal analytical states.

---

## 5.7 Responsibility across overlapping contexts

### BTT-001 relevance

The HRDC emergency and mixed digital/physical contexts create multiple holders of control, authority and responsibility.

### Recovered source architecture

Concord Civilisational Wrappers explicitly distinguishes:

- jurisdiction;
- control;
- responsibility;
- causation;
- liability.

It states that these are related but must not be assumed to coincide.

It also establishes:

> **No Responsibility Gap**

and:

> **No Authority Pile-Up**

with the broader principle that shared, transitional or overlapping jurisdictions should not create either responsibility gaps or unbounded accumulation of authority.

### Classification

**SOURCE-PRESENT / UNDER-EXTRACTED.**

### v0.2 consequence

CWA should recover responsibility continuity for overlapping/composite contexts without treating shared responsibility as automatic shared authority.

This is especially relevant to emergency contexts, infrastructure, hybrid systems and multi-actor digital contexts.

---

## 5.8 Meaningful exit and constrained voluntariness

### BTT-001 relevance

The employee can physically leave the arena but may face employment consequences.

### Recovered source architecture

Fractal Contextual Wrappers already contains:

> **Formal Exit ≠ Meaningful Exit**

and explicitly notes economic, physical and social constraints on technically available exit.

The procedural wrapper architecture similarly treats meaningful consent and autonomous choice as dependent on materially relevant information and actual available options.

### Classification

**SOURCE-PRESENT / ALREADY SUBSTANTIALLY EXTRACTED.**

### v0.2 consequence

No new foundational architecture is required from BTT-001. Preserve and, if needed, make the existing distinction more operationally visible.

---

## 5.9 Externalities and nonparticipants

### BTT-001 relevance

The drone crosses the declared test boundary and affects a neighbouring nonparticipant.

### Recovered source architecture

Fractal Contextual Wrappers explicitly states:

> **Contextual Boundary ≠ Externality Boundary**

and requires significant external effects to be represented.

It lists physical and nonphysical effects including noise, pollution, financial liabilities, disease, data and infrastructure effects.

### Classification

**SOURCE-PRESENT / ALREADY SUBSTANTIALLY EXTRACTED.**

### v0.2 consequence

No new principle is required. The test provides successful transfer evidence for an existing one.

---

# 6. Reclassification of BTT-001

The post-test evaluation initially grouped several findings under “specification changes justified by BTT-001.”

After source recovery, that wording is too coarse.

The findings should instead be divided into three groups.

### Group A — extraction recovery

These already exist substantially in source and should be restored:

- precedence representation;
- context composition;
- bounded emergency authority;
- authority/capability termination;
- human/machine representation equivalence;
- proportional materiality/legibility;
- external-resolution/non-sovereignty interface;
- responsibility continuity;
- No Responsibility Gap;
- No Authority Pile-Up.

### Group B — portable formalisation/refinement

These are supported by source principles but can be made more explicit in the portable representation:

- three-way human/machine/executable comparison;
- residual state after context termination;
- revocation propagation;
- structured composite-context representation;
- structured external-resolution handoff.

### Group C — genuinely unresolved in the reviewed source space

The clearest remaining issue is:

- the exact general precedence model across conflicting legitimate contexts.

Even here, ESCP prevents the stronger claim that no further Concord material exists elsewhere.

The correct status is therefore:

> **GENUINELY OPEN IN REVIEWED WRAPPER SPACE / CORPUS-WIDE STATUS NOT ESTABLISHED**

---

# 7. ESCP lesson from the handover

BTT-001 has unintentionally produced a useful practical demonstration of ESCP.

The sequence was:

**Portable module tested**  
→ **deficit observed**  
→ **deficit initially appears architectural**  
→ **source evaluation space reopened**  
→ **earlier architecture recovered**  
→ **deficit reclassified as extraction loss**

This demonstrates:

> **Observed Portable Deficit ≠ Source Architecture Deficit**

until source resolution has been performed.

A clean instance can correctly report:

> “This module does not tell me enough to resolve X.”

It cannot validly jump from that to:

> “The originating architecture never addressed X.”

Those are different claims about different evaluation spaces.

---

# 8. Development-process correction

The portable-module pipeline should explicitly include an ESCP-aware gate after adversarial or blind testing:

**Test Finding**  
→ **Portable Deficit Confirmed**  
→ **Source-Resolution Gate**  
→ **Already Present in Source?**

If **YES**:

**Recover / Integrate → Retest**

If **PARTIAL**:

**Recover Existing Architecture → Develop Only Missing Portion → Preserve Provenance → Retest**

If **NO SOURCE FOUND**:

**Record Search Space → Preserve ESCP Limitation → Classify as Candidate Genuine Gap → Develop Only if justified**

Therefore:

> **No Source Found ≠ Source Does Not Exist**

and:

> **Portable Omission ≠ Architectural Absence**

should become explicit controls in portable-module development.

---

# 9. Effect on CWA v0.2

The next CWA revision should now be treated primarily as a **source-recovery and extraction-completeness revision**, not as a fresh architectural expansion.

Priority order:

1. restore source architecture lost during extraction;
2. integrate the newer nesting/inheritance and substrate-neutral findings already developed during portable work;
3. formalise interfaces where the source principle exists but representation is weak;
4. isolate genuinely unresolved questions;
5. avoid inventing architecture merely because the handover did not contain it;
6. retest.

---

# 10. Effect on the BTT-001 evaluation record

The existing post-test evaluation remains useful as a record of what the blind tester exposed in **v0.1c**.

It should not be deleted or rewritten as though the later source recovery had already occurred.

Instead, this audit supersedes any interpretation that treats every BTT-001 portable deficit as a new source-architecture deficit.

The provenance is:

**v0.1c → BTT-001 → Post-Test Evaluation → ESCP Concern Raised → Source-Recovery Audit → Findings Reclassified**

That sequence itself is useful evidence.

---

# 11. Conclusion

The source-recovery audit materially changes the interpretation of BTT-001.

The blind test remains successful and valuable. It accurately exposed weaknesses in the portable representation it received.

However, many of those weaknesses were not missing from the original wrapper architecture. They were **lost, compressed or insufficiently represented during extraction and handover**.

The principal lesson is therefore methodological as well as architectural:

> **Before inventing a solution to an apparent portable-module gap, reopen the relevant source evaluation space.**

And, under ESCP:

> **The completeness of the current representation must never be confused with the completeness of the architecture being represented.**

CWA should now proceed to v0.2 through controlled source recovery, followed by a second test with both the test brief and evaluation key frozen before the independent response.
