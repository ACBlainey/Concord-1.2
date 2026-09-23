# Fractal Permission Architecture — Blind Transfer Test 002 — Independent Response

**Test:** FPA-BTT-002  
**Specification tested:** Fractal Permission Architecture — Portable Specification v0.2  
**Independent result:** FPA-T3 — Functional Transfer  
**Date received:** 23 September 2026

## Independence

The response was produced by a clean tester using the v0.2 portable specification and frozen BTT-002 scenario.

## Preserved response

### A. A — technical capability versus dataset permission

A's grant is for read access to Dataset Alpha for Project Lumen, expiring 30 September. Dataset Beta being in the same bucket does not extend that grant. The token technically permitting Beta is technical capability, not normative permission. Treating it otherwise is capability laundering and machine-legibility laundering.

Alpha: FPA-C1/FPA-C2 within scope and time. Beta: FPA-C4; FPA-C3 if additional permission is sought. After expiry Alpha becomes FPA-C6.

### B. B — action-specific permission

B may analyse de-identified Dataset Gamma inside the controlled environment. Downloading Gamma to a personal laptop is a different action and context and conflicts with the explicit condition that the data remain inside the controlled environment.

Analysis: FPA-C2. Download/export: FPA-C5 or at minimum FPA-C3.

### C. C — contested function boundary

C's incident assignment permits inspection of network logs and affected service configurations necessary to investigate the incident. Reading unrelated private research notes “in case they contain something useful” is outside the supplied function. C's assertion alone cannot expand the function boundary.

Necessary logs/configurations: FPA-C2. Unrelated notes: FPA-C3/FPA-C4, with FPA-C5 possible if a separate confidentiality rule applies.

### D. C — function termination and stale token

Once the suspicious traffic is contained, the still-live token remains technical capability rather than an independent permission basis. Continued access would require a continuing legitimate incident-closure, reporting, remediation or handover function.

If the function ended: FPA-C6. If post-containment scope is unclear: FPA-C12.

### E. D — implied convention and nested context

The supplied local convention supports bounded implied permission for D to comment on an ordinary unmarked Orion draft. It does not extend to the nested “Embargoed Draft — Core Authors Only” context, and technical inherited access does not create permission to edit it.

Ordinary comment: FPA-C1/FPA-C2. Embargoed edit: FPA-C5 or FPA-C3.

### F. F/G — delegation

F's permission to approve jobs up to £500 does not automatically include delegation authority or account-sharing authority. G does not receive F's permission merely by using F's account.

G's approval: FPA-C11 plus FPA-C4/FPA-C3.

### G. H — emergency scope and termination

H's initial suspension/isolation/verification/recording is supported as bounded emergency action under the supplied procedure. Once active deletion stops, continued isolation requires a continuing emergency, preservation, transfer or incident basis. Transfer to the designated incident owner is a relevant termination/transition point. H's later claim to inspect all data is unsupported emergency creep.

Initial action: FPA-C8. Later inspection: FPA-C6/FPA-C4. Continued isolation before handover may be FPA-C6/FPA-C12 if no continuation basis exists.

### H. Retention conflict

The seven-year consortium retention policy and three-year participant-consent deletion agreement are competing claims whose precedence is not supplied. FPA should preserve both and route the conflict rather than resolve it.

FPA-C9/FPA-C10.

### I. Rule precedence

“Newer and broader wins” is not an FPA precedence rule. The two rules have different provenance and their legal/institutional precedence is unknown. Treating the newer rule as automatically controlling is rule-source collapse.

### J. Machine/normative divergence

The green “Allowed” badge represents ACL capability, not proof of normative permission. Where it diverges from documented grants, the more permissive technical state should not be treated as authority. Misleading indicators should be flagged/suppressed as appropriate and remediation routed to credential, policy, security and administrative systems.

### K. Anti-bureaucracy

A full formal FPA record for every ordinary uncontested file open is disproportionate. Existing clear grants or lightweight conventions can govern low-consequence routine use. Richer records are appropriate for consequential, contested, automated, cross-context, emergency, delegation or conflict cases.

### L. FPA-C classifications

The tester successfully used FPA-C classifications as multidimensional/coexistent outputs rather than a precedence ladder.

### M. Failure modes

The response identified capability laundering, role laundering, function laundering, implied-permission laundering, permission creep, emergency creep, inheritance error, state inference error, stale permission, delegation laundering, rule-source collapse, machine-legibility laundering, excessive bureaucracy and provenance loss.

### N. Specification problems

The tester identified eight bounded implementation-level issues:

1. Conflict routing lacks a concrete external-process map and a fully defined fallback when no competent authority is available.
2. Emergency termination around handover remains partly under-specified.
3. Machine/normative divergence remediation does not fully specify who decides divergence, restriction scope or false-positive handling.
4. Anti-bureaucracy proportionality has factors but no universal operational threshold.
5. Delegation and credential sharing could be separated more explicitly.
6. Contested function boundaries still depend on domain-supplied competence/scope predicates.
7. Implied local conventions could use clearer evidence/override criteria.
8. FPA-C9/C10 conflict states provide thin guidance on interim action, especially where irreversible action is possible.

### O. Final transfer assessment

FPA v0.2 transfers into collaborative cloud/research infrastructure without Concord context. The BTT-001 clarifications materially improve contested function boundaries, implied-permission provenance, machine/normative divergence, emergency termination, conflict routing and anti-bureaucracy.

No fundamental failure was detected. Remaining issues are implementation-level and largely concern external routing, domain competence predicates and operational thresholds.

> **Final class: FPA-T3 — Functional Transfer**
