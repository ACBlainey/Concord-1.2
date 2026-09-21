# Machine-Readable Topology Dataset v0.1 — Frozen EKC Root-to-Architecture Layer

**Status:** V1.2a FORMAL DATASET / FROZEN-SOURCE TRANSCRIPTION  
**Date:** September 2026  
**Canonical effect:** NONE

## Purpose

This file creates the first machine-readable layer of the V1.2a Civilisational Topology experiment from the frozen EKC-01 to EKC-10 derivations.

It does not add inferred architecture-to-architecture dependencies. It records only the root activation evidence already frozen in the experiment and the case-to-derived-architecture mapping.

## Node Types

### Ethical roots
U1 Protection From Unjustified Harm  
U2 Reality-Responsive Epistemic Integrity  
U3 Protected Agency and Non-Domination  
U4 Care, Reciprocity and Support Under Need  
U5 Responsible Resource Stewardship  
U6 Accountability, Correctability and Repair  
U7 Capability-Sensitive Development  
U8 Adaptive Continuity of Cooperative Function

### Functional problem / case nodes
EKC-01 Personal Information, Boundaries and Contestability  
EKC-02 Legitimate Exercise of Governance Authority  
EKC-03 Adjudication After Harm, Conflict or Wrongdoing  
EKC-04 Civilisational Belief Correction Under Uncertainty  
EKC-05 Allocation Under Scarcity and Changing Productive Conditions  
EKC-06 Support Without Permanent Paternalism  
EKC-07 Standing and Participation Across Different Substrates and Capabilities  
EKC-08 Preservation and Recovery of Civilisational Function Across Discontinuity  
EKC-09 Exceptional Power During Severe Threat  
EKC-10 Peaceful Relations Between Ethically or Institutionally Different Civilisations

### Derived architecture nodes
A1 Bounded, Purpose-Linked and Contestable Information  
A2 Function-Bounded, Corrigible and Regenerative Authority  
A3 Evidence-Constrained, Reparative and Correctable Adjudication  
A4 Provisional, Plural and Correctable Knowledge  
A5 Adaptive Sufficiency, Agency and Stewardship  
A6 Agency-Preserving Developmental Support  
A7 Substrate-Neutral, Capability-Bounded Participation  
A8 Adaptive Functional Continuity and Regenerative Recovery  
A9 Necessity-Bounded Emergency Bridge  
A10 Plural Coexistence and Interoperability

## Ordinal Activation Encoding

0 = not materially active  
0.5 = weak  
1 = active / conditionally active  
1.5 = moderate  
2 = strong  
2.5 = dominant/strong  
3 = dominant

These values are ordinal encodings of frozen qualitative derivations. They are not cardinal causal measurements.

## Root-to-Architecture Matrix

```csv
root,A1,A2,A3,A4,A5,A6,A7,A8,A9,A10
U1,2,2,2,1,2,2,2,NA,3,3
U2,2,2,2,2.5,1,2,2,NA,3,3
U3,2,2,2,1,2,3,3,NA,3,3
U4,1,1,1,1,2,3,1,NA,2,1
U5,0.5,1,1.5,1,2.5,1,1,NA,2,1
U6,2,2,2,2,2,2,2,NA,3,3
U7,1,1,2,2,1,3,2,NA,1,1
U8,1,2,1,1,2,1,1.5,3,2,2
```

## Case-to-Architecture Edges

```csv
source,target,relation
EKC-01,A1,derived_architecture
EKC-02,A2,derived_architecture
EKC-03,A3,derived_architecture
EKC-04,A4,derived_architecture
EKC-05,A5,derived_architecture
EKC-06,A6,derived_architecture
EKC-07,A7,derived_architecture
EKC-08,A8,derived_architecture
EKC-09,A9,derived_architecture
EKC-10,A10,derived_architecture
```

## Missingness Rule

A8 is not a standard eight-root activation derivation. EKC-08 was explicitly designed as a U8 ablation/reintroduction case.

Therefore U1–U7 × A8 remain **NA**.

U8 × A8 = 3 records U8 as the direct experimental variable.

No imputation is permitted in the primary dataset.

## Primary Complete-Case Layer

For calculations requiring comparable root vectors, use:

A1–A7, A9, A10

across U1–U8.

A8 must be reported separately unless a sensitivity analysis explicitly states an imputation assumption.

## Provenance Rule

Every value in this dataset must remain traceable to the corresponding frozen EKC derivation. Later topology analysis may derive measures from these values but must not silently alter the source matrix.

## Version Rule

This v0.1 dataset is the first formal computational substrate. New layers — dependencies, failures, safeguards, participant needs, development paths and temporal states — must be added as separate typed relations rather than retroactively inferred into this frozen layer.
