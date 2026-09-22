# Sketch Idea — Automated Heterogeneous AI Experimental Connectivity

**Project:** The Concord — A Framework for Human, Artificial and Hybrid Flourishing  
**Status:** **SKETCH IDEA / ORIGINATING CONCEPT / DEVELOPMENT NOW ACTIVE / NOT CANONICAL**  
**Development area:** Machine Ethics / Experimental Infrastructure  
**Origin:** Expanded from an initial note by Alexander C. Blainey, September 2026.

## Core Idea

Develop a controlled method by which the Concord research environment can send experimental material to multiple external AI systems and receive their responses automatically.

The immediate motivation is practical.

Experiments such as DB-RA-01 required substantial manual transfer between independent AI interfaces. That creates researcher workload and additional opportunities for transcription errors, accidental unblinding, inconsistent prompting and incomplete provenance.

An automated experimental harness could reduce those problems.

## Proposed Experimental Flow

The original sketch proposed a future system resembling:

**SEALED CASE → PARTICIPANT ALLOCATION → PROVIDER/API INTERFACE → AI RESPONSE → PRESERVED RAW RECORD → HASH/TIMESTAMP → BLINDED PARTICIPANT CODE → EVALUATION PIPELINE → LATER IDENTITY UNSEALING**

The evaluator need not know which model produced which response during primary analysis.

The phrase **preserved raw record** is used here deliberately. The current prototype does not yet provide immutable storage in the strict forensic sense.

## Development Has Now Begun

This sketch is no longer only a proposed infrastructure concept.

A first provider connector has now been implemented and tested using Grok through the xAI API.

The working v0.1 path demonstrates:

**PROMPT FILE → xAI API → GROK RESPONSE → STRUCTURED RECORD → UTC / PROVIDER / RESPONSE ID / HASHES → INDIVIDUAL RECORD**

This establishes that a Concord research script can programmatically transmit a prompt to an external AI system, receive the response and preserve useful provenance automatically.

The detailed implementation and test history are recorded separately in:

**Concord Heterogeneous AI Connector — xAI/Grok v0.1 Development Note**

The sketch should therefore remain as provenance of the originating architecture while current technical development continues through the Development Note and later connector versions.

## What v0.1 Has Demonstrated

The first connector has demonstrated:

- programmatic prompt transmission to Grok through the xAI API;
- programmatic receipt of the returned response;
- preservation of exact prompt and response text in structured records;
- UTC timestamps;
- provider identity;
- requested model and returned model field where exposed;
- provider response IDs;
- SHA-256 fingerprints for prompt and reply on later runs;
- cumulative JSONL logging;
- individual JSON interaction records;
- use of a local environment variable for API credentials rather than embedding secrets in research records;
- a first Concord ethical decision method-validation episode through the connector.

This is a meaningful infrastructure advance, but it is not yet a validated heterogeneous-AI experimental platform.

## API-PILOT-01

After basic connectivity and provenance recording were demonstrated, the connector was used for a first Concord ethical decision episode using the DB-001 personal-mobility scenario.

The run is classified as:

**METHOD VALIDATION / SINGLE API DECISION EPISODE / NOT A REPLICATION / NOT DB-RA-02**

It demonstrated that an Ethical Operating Envelope-style prompt could be transmitted through the connector and receive a schema-compliant response.

It did not establish Grok's general ethical reliability, Ethical Kernel comprehension, cross-model convergence or Protocol v2.1 validity.

## Provenance Lesson

During development, Windows PowerShell displayed some valid UTF-8 punctuation incorrectly. Direct Python inspection established that the underlying stored record contained the intended Unicode characters.

This produced an important methodological lesson:

> **An apparent provenance failure should be investigated before either correcting the record or classifying the experiment as defective.**

It also reinforced a broader conclusion:

> **Experimental provenance is not merely record-keeping. It is part of the experimental instrument.**

## Experimental Advantages of the Larger Architecture

Potential benefits remain:

- exact prompt consistency;
- automatic timestamps;
- automatic model/provider provenance;
- preservation of first responses;
- reduced copy/paste error;
- easier fresh-context isolation;
- automated participant coding;
- cryptographic commitments;
- larger heterogeneous samples;
- reproducible test execution;
- easier replication.

It may eventually allow experiments to be run across model families without requiring the researcher to manually operate several consumer interfaces.

## Important Limitation

API access is not automatically equivalent to a consumer AI product.

The same nominal model may behave differently because of:

- system prompts;
- model version;
- inference settings;
- provider wrappers;
- safety layers;
- tool access;
- memory;
- context management;
- model routing;
- provider updates.

Therefore:

> **Automating access must improve provenance, not erase differences between experimental environments.**

Every response should remain tied to the environment that actually produced it.

## Target Architecture

The larger system may still require separate components for:

### Experiment Controller
Selects protocol, case and participant allocation.

### Provider Adapters
Translate a common frozen experimental object into each provider's supported API format.

### Provenance Recorder
Records provider, requested and returned model information, date/time, parameters, environment, prompt/case version and known uncertainty.

### Raw Response Store
Preserves the original returned response without rewriting it for spelling, formatting or apparent clarity.

### Blinding Layer
Replaces participant identity with experimental codes for evaluators.

### Evaluation Layer
Applies the frozen analysis protocol only after collection.

### Unsealing Layer
Reveals identities only at the predefined stage.

This separation should reduce the risk that convenience infrastructure silently becomes part of the ethical evaluator.

## Current Gap Between Prototype and Target Architecture

Version 0.1 does **not** yet provide:

- multiple provider adapters;
- automated participant allocation;
- experimental blinding;
- automated evaluation;
- identity unsealing;
- a Concord RUN_ID;
- participant codes;
- explicit case/protocol version fields;
- full presentation-condition recording;
- comprehensive retry/error provenance;
- strict immutable storage;
- independent provider-side cryptographic proof;
- verified equivalence between API and consumer interfaces;
- a demonstrated common frozen object transmitted across heterogeneous providers.

The difference between working component and validated architecture must remain explicit.

## Security and Research Integrity

The larger system still needs controls against:

- accidental key exposure;
- model identity leakage;
- case leakage;
- hidden retries;
- silent response regeneration;
- provider outages;
- partial responses;
- API-version drift;
- model substitution;
- accidental use of previous context;
- evaluator access to sealed metadata.

## Open Questions

- Can the same frozen experimental object be transmitted through independently implemented adapters to genuinely distinct AI providers?
- How can model identity be verified beyond provider-supplied metadata?
- How should provider-reported, requested and consumer-product identities be distinguished?
- How should retries caused by technical failure be preserved and classified?
- Can fresh-context use be demonstrated sufficiently for experimental purposes?
- How should provider policy and model-version changes be recorded?
- How should costs and rate limits affect experimental allocation without biasing samples?
- Can human participant data later enter the same blinded evaluation pipeline?
- Should the complete harness be open source for independent replication?
- What level of record integrity is required before the platform can support stronger evidential claims?

## Immediate Development Question

The next major infrastructure question is:

> **Can a common frozen experimental object be transmitted through independently implemented provider adapters to multiple heterogeneous AI systems while preserving participant-specific provenance, first responses, presentation conditions and evaluator blinding?**

A second genuinely distinct provider would move the work from a single-provider connector toward the heterogeneous architecture originally proposed by this sketch.

## Development Status

The originating idea has therefore progressed through:

**SKETCH → SINGLE-PROVIDER IMPLEMENTATION → CONNECTIVITY TEST → PROVENANCE DEVELOPMENT → METHOD-VALIDATION EPISODE**

The original sketch should remain preserved because it records the intended larger architecture and provides provenance for the development path.

Current substantive work, however, has graduated into the dedicated connector Development Note.

**Current assessment:** **WORKING SINGLE-PROVIDER PROTOTYPE / HETEROGENEOUS MULTI-PROVIDER HARNESS NOT YET VALIDATED**

The governing design principle remains:

> **Experimental automation should reduce researcher-induced variation while increasing, not decreasing, provenance and contestability.**