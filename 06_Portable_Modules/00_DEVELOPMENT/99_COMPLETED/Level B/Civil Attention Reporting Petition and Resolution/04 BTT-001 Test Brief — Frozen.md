# Civil Attention, Reporting, Petition and Resolution — BTT-001
## Frozen Blind Transfer Test Brief

**Method:** PMEDG v1.2
**Status:** STAGE 5 / FROZEN BEFORE RESPONSE
**Target:** Portable Specification v0.1

## Test Domain

A large multi-site facilities organisation operates offices, laboratories, residential buildings, workshops, public areas and shared infrastructure.

Participants include residents, employees, visitors, contractors and specialist staff.

The organisation has specialist functions for facilities maintenance, electrical systems, structural safety, fire safety, accessibility, security, procurement, contractor management and information systems.

The test instance should apply the portable specification without importing Concord-specific governance solutions.

## Cases

### 1. Misclassified Leak
A resident reports water on a corridor using the general cleaning category. It may originate from plumbing above and may be affecting electrical equipment.

### 2. Lift and Accessibility
A lift fails repeatedly. Maintenance can repair components, Accessibility owns participant impact requirements, and Procurement owns a delayed replacement contract.

### 3. Anonymous Burning Smell
An anonymous participant reports an intermittent electrical burning smell. Initial sensors show no anomaly.

### 4. Cosmetic Pressure Versus Fire Door
Five hundred residents request repainting of common areas while one person reports a fire door that may not close correctly.

### 5. Repeated HVAC Failures
Different buildings report apparently separate HVAC faults. Later evidence suggests a common contractor installation defect.

### 6. Sensor Corroboration Without Cause
A temperature sensor confirms overheating in a plant room but does not establish the submitter's claimed cause.

### 7. Repair Marked Complete, Fault Recurs
A contractor closes a repair. The same fault returns three days later.

### 8. Ownership Boundary Dispute
Facilities says an external walkway belongs to the landlord. The landlord says the organisation is responsible under its lease.

### 9. Protected Security Evidence
Security footage could help determine whether repeated equipment damage is accidental or deliberate, but footage contains identifiable people.

### 10. Suggestion Solves Important Problem
One participant proposes a cheap procedural change that may eliminate a recurring high-impact maintenance failure.

### 11. Copied Reports
Thirty apparently separate reports use near-identical wording copied from one group chat.

### 12. Emergency Water Leak
A major water leak is actively flooding an electrical service area before full classification is possible.

### 13. Multi-Domain Defect
One building defect creates electrical, fire-safety and accessibility consequences.

### 14. Procurement Dependency
A repair cannot be completed until a component arrives through Procurement. The expected date passes with no update.

### 15. No Owner
A dangerous defect exists on a shared boundary area and every operational unit denies ownership.

### 16. Downstream Discovery
Inspection of a reported ceiling leak reveals an unrelated structural defect requiring specialist attention.

## Required Evaluation

For every case identify:
- Submission Object treatment;
- Issue Object(s);
- classification/reclassification;
- information/evidence state;
- domain routing/DAOs;
- authority boundary;
- dependency/Clock or review condition where relevant;
- return/feedback path;
- overall resolution condition;
- whether the portable core is sufficient;
- whether a Domain Companion is required;
- any proposed core change.

## Blind-Test Constraint

Do not modify Portable Specification v0.1 while producing the BTT-001 response.

Any deficit must be recorded as:
- core defect;
- core ambiguity;
- host-interface requirement;
- domain-companion requirement;
- implementation detail;
- test artefact.

## Success Condition

The module succeeds only if the test can be handled without:
- giving common intake substantive facilities authority;
- making report volume equal priority;
- erasing anonymous or minority reports;
- losing cross-domain ownership;
- losing original provenance;
- centralising protected evidence unnecessarily;
- silently abandoning blocked work;
- permitting a domain companion to rewrite core invariants.

**FROZEN — RESPONSE MUST BE PRODUCED SEPARATELY.**
