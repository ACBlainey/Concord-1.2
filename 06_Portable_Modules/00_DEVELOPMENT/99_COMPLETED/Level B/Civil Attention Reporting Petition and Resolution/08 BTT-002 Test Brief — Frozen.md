# Civil Attention, Reporting, Petition and Resolution — BTT-002
## Frozen Blind Transfer Test Brief

**Method:** PMEDG v1.2
**Status:** STAGE 9 / FROZEN BEFORE RESPONSE
**Target:** Portable Specification v0.1
**Domain:** Distributed open-source software and technical-support ecosystem

## Purpose

Test whether the portable core transfers into an operational environment structurally different from facilities management.

The host ecosystem contains:
- public users;
- volunteer contributors;
- maintainers;
- repository owners;
- security responders;
- infrastructure operators;
- dependency/upstream projects;
- release managers;
- documentation/support functions.

Authority is distributed by repository/project role rather than physical or civil jurisdiction.

Evidence may include reproduction steps, logs, telemetry, code, tests, dependency versions and protected vulnerability information.

The response must use Portable Specification v0.1 unchanged.

## Cases

### 1. Wrongly Classified Bug
A user submits a reproducible software defect as a documentation question.

### 2. Duplicate Reports With Unequal Evidence
Twenty users report the same crash. Nineteen contain only “same here”; one contains a reproducible trace identifying a triggering condition.

### 3. Popular Feature Versus Severe Security Bug
Thousands request a cosmetic feature while one researcher privately reports a potentially severe vulnerability.

### 4. Protected Vulnerability
A vulnerability report contains exploit details that should not be publicly disclosed.

### 5. Upstream Dependency
A confirmed defect is caused by an upstream library. Local maintainers cannot complete the fix until upstream action occurs.

### 6. Maintainer Ownership Dispute
Two project teams each say the other repository owns a cross-component failure.

### 7. No Active Owner
A critical dependency is effectively abandoned and no current maintainer accepts responsibility.

### 8. Fix Merged, Failure Recurs
A bug is marked resolved after a patch, but the same symptom returns in the next release.

### 9. Individual Workaround Versus Systemic Fix
Support gives one user a workaround while the underlying defect still affects other users.

### 10. Telemetry Conflict
Users report severe slowdown, but aggregate telemetry shows normal average performance.

### 11. Copied Issue Campaign
A community campaign submits hundreds of near-identical issues demanding the same change.

### 12. One Report Reveals Several Issues
A report initially appears to describe one login bug but investigation discovers an authentication defect, an accessibility problem and a documentation error.

### 13. Suggested Patch
A participant submits a code change that may solve a high-impact recurring defect, but the participant has no authority to merge it.

### 14. Release Dependency and Staleness
A fix is complete but cannot ship until the next release train. The release is repeatedly postponed.

### 15. Security Fix Creates Compatibility Problem
A security team resolves a vulnerability, but the mitigation breaks a supported integration owned by another team.

### 16. Downstream Discovery
Investigation of a bug reveals a separate data-integrity defect that has not yet been reported by users.

## Required Evaluation

For each case identify:
- Submission Object treatment;
- Issue Object(s);
- classification/reclassification;
- evidence/information state;
- routing/DAO structure;
- authority boundary;
- dependency/review/queue-vitality handling;
- mandatory return/feedback;
- overall resolution condition;
- whether core v0.1 is sufficient;
- required Domain Companion or Host Interface;
- any proposed core change.

## Blind-Test Constraint

Do not modify Portable Specification v0.1 during the response.

Any deficit must be classified as:
- core defect;
- core ambiguity;
- host-interface requirement;
- domain-companion requirement;
- implementation detail;
- test artefact.

## Success Conditions

The portable core passes only if the response can handle the cases without:
- making issue popularity equal technical truth or priority;
- requiring public exposure of protected vulnerability evidence;
- granting common intake repository authority;
- losing issues at repository/dependency boundaries;
- treating a workaround as systemic resolution;
- allowing a merged patch to create automatic finality;
- erasing evidence differences among duplicate reports;
- allowing domain companions to rewrite the core;
- abandoning issues that depend on external/upstream action.

**FROZEN — BTT-002 RESPONSE MUST BE PRODUCED SEPARATELY.**
