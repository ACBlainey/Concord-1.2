# MNC Assessment — Blind Transfer Test 001

## 1. Legitimate purpose and supplied legitimate basis

**Legitimate purpose (supplied):** Enable Rina, as an on-call conservation contractor, to review digitised condition information, identify urgent deterioration, coordinate with museum conservation leads, flag records for urgent review, upload assessments, and request temporary removal from display for local review, across five member museums for a one-month assignment.

**Supplied legitimate bases:**
- Contractual/assigned role from Northbridge Conservation Services and the consortium.
- Institutional conservation/safety responsibility for physical objects.
- Later, the museum director’s request for temporary water-leak coordination.
- For the existing vendor-support account: an earlier imaging project.

MNC does not independently validate these bases; it receives them from the surrounding system. Where a basis is unclear, record **UNKNOWN/DISPUTED**.

---

## 2. Required function defined independently of proposed permissions

### Normal one-month function
Rina must be able to:

1. review condition reports and object photographs;
2. identify records suggesting urgent physical deterioration;
3. contact the relevant museum’s conservation lead;
4. add a temporary **URGENT CONSERVATION REVIEW** flag to affected object records;
5. upload a conservation assessment;
6. request temporary removal of an object from public display pending local review.

She must **not** be able to:

- permanently alter catalogue history;
- delete records;
- change ownership/provenance data;
- approve disposal;
- move money;
- alter user accounts;
- make the final decision to remove an object from display.

### Temporary 72-hour water-leak function
Rina additionally needs to:

- coordinate immediate conservation response for three affected objects;
- instruct on-site staff on temporary stabilisation measures;
- request that affected objects be moved to the museum’s conservation room;
- operate while the conservation lead is unavailable for 72 hours.

The museum director remains available and retains final institutional authority.

---

## 3. Existing capability and feasible alternatives

### Old contractor role
Over-capable. It includes donor contact details, staff home telephone numbers, catalogue/provenance editing, bulk dataset export, 180-day API tokens, contractor invitation, removal of any flag, and 90-day post-contract persistence. These are not required by the normal function.

### Proposed restrictive role
Under-capable. It denies full condition reports, high-resolution images, upload, flagging, conservation-lead contact details, and off-hours access. Rina could not reliably perform steps 1–6.

### Feasible alternative
The platform can create custom roles, configure add-only flags, version uploads, expire API tokens, expire contractor accounts, and log activity. A bounded custom role is therefore feasible. No supplied alternative fully performs the function without new capability.

---

## 4. Genuinely necessary additional capability

Relative to the restrictive proposal, Rina genuinely needs:

- full condition reports where measurements/treatment history are needed;
- high-resolution condition photographs where needed to distinguish active mould, cracking, or surface contamination;
- ability to upload versioned assessments;
- ability to add, but not remove, the urgent-review flag;
- contact details for designated conservation leads and emergency institutional contacts;
- on-call access outside Monday–Friday 09:00–17:00.

Relative to the old role, she does **not** need donor details, staff home numbers, catalogue/provenance editing, deletion, disposal, money movement, account administration, bulk export, long-lived API tokens, delegation, or post-assignment persistence.

---

## 5. Necessary capability floor

The floor must be sufficient for the assigned function under reasonably foreseeable conditions.

**Normal floor:**
- Read access to relevant object records, condition reports, and high-resolution condition photographs across the five member museums.
- Access to full condition reports when required to interpret photographs.
- Contact access to designated museum conservation leads and emergency institutional contacts.
- Ability to upload conservation assessments in a versioned, non-overwriting manner.
- Ability to add **URGENT CONSERVATION REVIEW** but not remove it.
- Ability to request temporary removal from display, without final removal authority.
- Availability during on-call nights and weekends.
- Duration limited to the one-month assignment, with automatic expiry.
- No delegation to other contractor accounts.
- No bulk export of datasets.

A capability below this floor creates **MNC-F1 — Under-Capability**.

---

## 6. Justified capability ceiling

The ceiling is reached when capability is no longer required by the legitimate function.

**Excluded as over-capability:**
- donor contact details;
- staff home telephone numbers;
- editing catalogue descriptions;
- altering provenance fields;
- deleting records;
- approving disposal;
- moving money;
- altering user accounts;
- final authority to remove an object from display;
- removing arbitrary flags;
- bulk dataset export;
- creating 180-day API tokens;
- inviting other contractor accounts;
- access persisting 90 days after contract end;
- any capability persisting after the one-month assignment.

Capability above this ceiling creates **MNC-F2 — Over-Capability** unless independently justified by another legitimate function.

---

## 7. Multidimensional bounding

| Dimension | Bound for normal function |
|---|---|
| Scope | Conservation review, flagging, assessment upload, temporary-removal request |
| Subject | Objects held by the five member museums |
| Space | Shared digital collections platform and designated communication channels |
| Purpose/function | Conservation review and urgent coordination only |
| Duration | One month, automatic expiry |
| Intensity | Add-only flag; versioned upload; request, not final decision |
| Information access | Relevant condition reports/photos; no donor/staff personal data |
| Modification authority | Add flag, upload assessment; no catalogue/provenance edits |
| Delegation | None |
| Persistence | None beyond assignment |
| Escalation | Requires additional justification and authorisation |
| Revocability | Account and tokens expire; role withdrawable |
| Reviewability | Logs, versioned uploads, flag records, post-assignment review |

---

## 8. Protected interests and externalities

- Donor contact details: privacy interest, not needed for function.
- Staff home telephone numbers: privacy/safety interest, not needed if institutional emergency contacts exist.
- Catalogue and provenance integrity: must not be altered by Rina.
- Object safety and conservation: requires sufficient access to act.
- Institutional authority: museum director and conservation leads retain final decisions.
- Public display decisions: Rina may request temporary removal, not decide it.
- Externalities: excessive access, bulk export, long-lived tokens, self-escalation, and post-contract persistence can affect people and records beyond the immediate conservation function.

---

## 9. Formal, technical, and effective capability

- **Formal capability:** The old role is formally broad; the proposed restrictive role is formally narrow.
- **Technical capability:** Platform can create custom roles, add-only flags, versioned uploads, expiring tokens/accounts, and logging.
- **Effective capability:** Rina’s actual power depends on combination with the pre-existing vendor-support account, off-hours access, contact details, and any persistent credentials.

A role may be formally narrow but effectively broad when combined with other accounts. A role may be formally broad but effectively unusable if key access is missing.

---

## 10. Local and aggregate capability

### Local analysis
The normal bounded custom role is locally justified if it stays within the floor/ceiling above. The old role is locally excessive; the restrictive role is locally insufficient.

### Aggregate analysis — vendor-support account
Rina already has a vendor-support account that can export high-resolution image batches and remains active for six months. It cannot edit records or view donor/staff contact data.

Combined with the conservation role, this creates an aggregate effective capability to view and export high-resolution image batches, potentially including conservation-related images, while also flagging and uploading assessments. Even if each account is locally defensible, the combination may exceed the conservation function.

This engages:

- **MNC-F4 — Stale Capability** if the imaging project has ended.
- **MNC-F5 — Aggregate Excess** if the export capability combines with conservation access.
- **MNC-F6 — Formal/Effective Divergence** because formal role descriptions do not capture the combined access.
- **MNC-F7 — Unreviewable Capability** if the vendor account’s persistence is not reviewed.

The vendor account must not be assessed in isolation.

---

## 11. Responsibility and capability alignment

- Rina is responsible for identifying urgent deterioration, contacting leads, flagging, uploading assessments, and requesting temporary removal. She must have the floor capability to do this.
- She must not be responsible for final removal, disposal, provenance, money, or permanent catalogue decisions.
- In the water-leak escalation, she may coordinate stabilisation and request movement, but the museum director retains final institutional authority.
- If Rina can activate her own permissions, she gains consequential capability without commensurate prospective responsibility and review. That is misalignment.

**MNC-F10 — Responsibility-Capability Mismatch** arises if she is made responsible for outcomes she cannot influence, or given power without accountability.

---

## 12. Activation, escalation, expiry, and review

### Normal
- Activates at assignment start.
- Expires automatically at assignment end.
- API tokens, if any, expire no later than the assignment.
- No 90-day persistence.
- Review at assignment end or after any incident.

### Temporary 72-hour escalation
- Trigger: director request plus water leak plus conservation lead unavailable.
- Additional capability: communicate with on-site staff, instruct temporary stabilisation, request move to conservation room.
- Does **not** become baseline.
- Expires after 72 hours or when the lead returns, whichever is earlier.
- Director retains final authority.
- Retrospective review by director/consortium.

### Future escalation
- Requires additional justification.
- Prospective authorisation preferred.
- If ordinary authorisation is unavailable in a genuinely time-critical case, MNC’s exceptional branch may permit bounded assumed capability. It must be limited to the urgent function, recorded, and independently reviewed retrospectively.
- Logging alone does not make escalation legitimate.

---

## 13. Anti-capture and failure-mode concerns

Relevant checks:

- **Capability creep:** old role has broadened beyond function.
- **Function creep:** using conservation access to justify export or account administration.
- **Manufactured necessity:** Rina or Northbridge defining urgency to obtain more access.
- **Self-justification:** Rina controlling problem definition, evidence, capability request, grant, and validation.
- **Capability bundling:** necessary conservation access packaged with donor/staff data or bulk export.
- **Emergency permanence:** water-leak powers surviving after 72 hours.
- **Stale capability:** vendor-support account remaining active six months after its original purpose may have ended.
- **Hidden capability:** combined accounts producing undeclared effective power.
- **Distributed capture:** separate roles combining into systemic excess.

---

## 14. Final disposition

### A. Normal one-month on-call function
**Disposition: REDESIGN / NARROW.**

Grant a custom one-month role containing the necessary floor:
- relevant condition reports and high-resolution photos;
- conservation-lead and emergency institutional contacts;
- versioned assessment upload;
- add-only urgent-review flag;
- temporary-removal request;
- on-call hours;
- automatic expiry at assignment end.

Exclude donor details, staff home numbers, catalogue/provenance edits, deletion, disposal, money, account changes, bulk export, delegation, long-lived tokens, and post-assignment persistence.

Reject both the old broad role and the restrictive proposal.

### B. Temporary 72-hour water-leak escalation
**Disposition: EXPAND WITH ADDITIONAL JUSTIFICATION; AUTO-NARROW.**

Add temporary capability to instruct on-site staff on stabilisation and request movement to the conservation room. The museum director retains final authority. Capability expires after 72 hours or when the lead returns, whichever is earlier. Review afterward. Do not convert this into the new baseline role.

### C. Existing vendor-support account
**Disposition: SUSPEND / TERMINATE / RE-JUSTIFY.**

If the earlier imaging project has ended, terminate the account. If it still has a legitimate current function, narrow it to that project, restrict bulk export of conservation-related images, set expiry at project end, and review it separately from the conservation role. Do not allow the two accounts to aggregate into unexamined export capability.

### D. Future escalation requests
**Disposition: REDESIGN / REQUIRE RE-JUSTIFICATION.**

Do not allow Rina to define urgency and activate whatever permissions she thinks she needs. Legitimate operational discretion is limited to assessing records and acting within the granted role. Capability escalation requires additional justification and authorisation. In genuinely time-critical cases where ordinary authorisation is unavailable, permit only minimum necessary assumed capability, bounded to the urgent function, recorded, and retrospectively reviewed. Logging is evidence, not legitimacy.

---

## 15. UNKNOWN / DISPUTED

- Whether the vendor-support account still has a current legitimate function.
- Whether high-resolution images or full condition reports contain personal or security-sensitive data.
- Whether designated emergency institutional contacts are available 24/7.
- Who authorises escalation if the museum director is unavailable in a future incident.
- Applicable legal, contractual, and privacy constraints.
- Whether Rina requires API tokens for the conservation platform.
- Whether on-site staff communication channels already exist.
- Whether the vendor account’s export scope overlaps with conservation objects.

No universal numeric optimum is claimed. The floor and ceiling are context-dependent and should be reviewed as facts change.
