# Historical Domain — Formal Schema Set 001 — Core Objects and Interfaces

**Project:** The Concord
**Domain:** Historical
**Status:** DEVELOPMENT SCHEMA / NOT CANONICAL
**Date:** 25 September 2026
**Basis:** Historical Formal Domain Specification v0.3

## 1. Purpose

This document extracts the principal v0.3 objects and interfaces into implementation-neutral schemas. It does not prescribe a database, language, storage engine or API.

All schemas inherit the Historical invariants. Identifiers are references, not claims of central ownership. Schemas may be distributed provided required relationships remain reconstructable.

## 2. HSO-1 — Historical State Object

Fields:

- HistoricalObjectID
- SourceDomain
- SourceObjectRef
- InformationClass
- EventTime
- StateEffectiveTime
- RecordCreationTime
- HistoricalCustodyTime
- VersionOrStateID
- EpistemicStatus
- AuthorityStatus
- PrivacyState
- ClassificationState
- RetentionState
- AccessState
- ProvenanceRefs
- RelationshipRefs
- TransformationRefs
- CorrectionRefs
- KnownUncertainty
- KnownDisputes
- EvaluationContextRef
- SearchBoundaryRef
- CompletenessScope
- SupersessionRefs
- CurrentOperationalRef
- CustodyMode
- ReviewCondition

Event time, creation time, effective time and custody time must remain distinguishable.

## 3. HEC-1 — Historical Evaluation Context

Fields:

- EvaluationContextID
- SubjectRef
- EffectiveTime
- PotentialEvidenceKnown
- AccessibleEvidence
- InaccessibleEvidenceKnown
- ObservedEvidence
- RepresentedVariablesOrCategories
- MethodOrModelRefs
- InterfaceOrSensorLimits
- SearchOrSamplingBoundaryRef
- KnownUnknowns
- KnownMissingDimensions
- ContemporaryUncertainty
- ContemporaryScopeClaim
- DecisionContextRef
- LaterDiscoveredDimensions
- RetrospectiveInterpretationRefs

Unknown-state typing must support KNOWN_UNKNOWN, KNOWN_MISSING_DIMENSION and LATER_RECOGNISED_UNREPRESENTED_DIMENSION.

## 4. HPR-1 — Provenance Relationship

Fields:

- RelationshipID
- FromRef / ToRef
- RelationshipType
- EffectiveStart / EffectiveEnd
- AssertionTime
- SourceRef
- EpistemicType
- PrivacyState
- AccessState
- IdentityExposureState
- DisputedState
- SupersessionRef

Relationship types may include DERIVED_FROM, SUPERSEDES, CORRECTS, CHALLENGES, INVALIDATES, DEPENDS_ON, CONTRIBUTED_TO, TEMPORALLY_FOLLOWS, ALTERNATIVE_TO, DISPUTES, SHARES_PROVENANCE_WITH, AUTHORIZED_BY, DELEGATED_BY, DECIDED_BY, REVIEWED_BY, REVOKED_BY, EXPIRED_BY and IMPLEMENTED_BY.

**Shared Provenance ≠ Shared Identity.**

## 5. HAE-1 — Authority Activation and Exercise Record

Fields:

- AuthorityEventID
- PreExerciseContextRef
- ActorOrInstitutionRef
- StandingEligibilityRef
- AuthoritySourceRef
- LegitimateFunction
- FunctionalNeed
- ActivationConditions
- ConditionsSatisfiedEvidence
- PermittedAction
- ObjectOrTargetRef
- JurisdictionOrSpace
- Scope
- AffectedRights
- ActivationTime
- ExerciseTime
- TerminationTime / TerminationCondition
- ExerciseDescription
- ConsequenceRefs
- PostExerciseContextRef
- ClaimedAuthorityState
- ContemporaneousRecognitionState
- ContestState
- LaterAdjudicationRefs
- CurrentInterpretationRef
- ProvenanceRefs
- EvaluationContextRef

Authority states may include CLAIMED, ACTIVATED, EXERCISED, CONTESTED, CONTEMPORANEOUSLY_RECOGNISED, EXPIRED, REVOKED, SUPERSEDED, INVALIDATED, HISTORICAL_ONLY, STATUS_UNKNOWN and STATUS_DISPUTED.

For discrete exercises:

C0 → justification → A1 activation → bounded exercise → A1 terminates/is consumed → C1.

The schema must not represent authority as an unbounded reusable property of an actor.

## 6. HIST-1 — Information-State Transition Record

Fields:

- TransitionID
- AffectedObjectOrClassRef
- PreviousInformationState
- NewInformationState
- TransitionType
- AuthorisingProcessRef
- AuthorityEventRef
- LegitimatePurpose
- EffectiveTime
- Scope
- AffectedRelationshipClasses
- KnownDerivativeRefs
- KnownReplicaRefs
- ExecutionStatus
- ReconciliationStatus
- ReviewOrAppealState
- MinimumResidueRef
- ProvenanceRefs
- CompletenessScope

Transition types may include REDUCE_DISCOVERABILITY, RESTRICT_ACCESS, RESTRICT_CORRELATION, PSEUDONYMISE, ANONYMISE, AGGREGATE, SEAL, CRYPTOGRAPHICALLY_DISABLE, RECLASSIFY, PARTIALLY_DISCLOSE and DESTROY.

## 7. HCP-1 — Correlation Permission

Fields:

- CorrelationPermissionID
- ActorOrProcessRef
- InputRecordClasses
- PermittedJoinKeysOrRelationshipTypes
- ProhibitedJoinKeysOrRelationshipTypes
- LegitimateFunction
- Purpose
- AuthoritySourceRef
- Scope
- ActivationTime
- ExpiryOrTerminationCondition
- OutputRestrictions
- IdentityExposureLimit
- AuditRequirement
- ReviewRequirement

**Access(A) + Access(B) ≠ PermissionToCorrelate(A,B).**

## 8. HMHR-1 — Minimum Necessary Historical Residue

Fields:

- ResidueID
- DestroyedObjectClassRef
- ExistenceMarkerPermitted
- TransitionType
- AuthorisingProcessRef
- EffectiveTime
- DestructionScope
- AffectedDerivativeClasses
- AuditReference
- ProhibitedContentDescription
- ReconstructionRiskAssessment
- AccessState
- RetentionState

The residue must not contain sufficient sensitive substance to defeat the destruction decision.

**Destruction Provenance ≠ Reconstruction of Destroyed Content.**

## 9. HSE-1 — Historical Secrecy Envelope

Fields:

- SecrecyEnvelopeID
- ProtectedObjectRef
- SecrecyJustification
- AuthoritySourceRef
- AuthorityEventRef
- Scope
- PermittedActorsOrClasses
- PermittedActions
- EffectiveStart
- ReviewTime
- ExpiryCondition
- DisclosureCondition
- CurrentSecrecyState
- ReviewHistoryRefs
- PartialDisclosureRefs
- ResidualProtectedElements
- ProvenanceRefs

States include ACTIVE_OPERATIONAL_SECRECY, SEALED_PENDING_REVIEW, CONTINUED_SECRECY_REJUSTIFIED, PARTIALLY_DISCLOSED, DISCLOSED, SECRECY_EXPIRED and STATUS_DISPUTED.

A permanent unqualified Boolean such as Secret=true is insufficient.

## 10. HSB-1 — Historical Search Boundary

Fields:

- SearchBoundaryID
- QueryOrQuestion
- CorpusRefs / CorpusVersions
- SearchMethod
- SearchTermsOrSelectors
- TraversalPath
- DepthOrCoverage
- Exclusions
- InaccessibleAreas
- KnownMissingSources
- StartTime / StopTime
- StoppingRule
- SaturationBasis
- ResultType
- CompletenessClaimScope
- ReopeningCondition

A consequential NO_RECORD_FOUND result should reference this object.

**No Record Found Within Evaluated Space ≠ Event Did Not Occur.**
