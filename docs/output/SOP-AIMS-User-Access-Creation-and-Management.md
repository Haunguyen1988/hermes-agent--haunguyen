# SOP — AIMS User Access Creation and Management

| **Document Code** | SOP-AIMS-UAM-001 |
|---|---|
| **Version** | 1.0 |
| **Effective Date** | [DD/MM/YYYY] |
| **Prepared By** | Nguyễn Đình Hậu — AIMS Coordinator |
| **Reviewed By** | [Reviewer Name / Title] |
| **Approved By** | [Approver Name / Title] |
| **Classification** | Internal Use Only |

---

## Document Control

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | [DD/MM/YYYY] | Nguyễn Đình Hậu | Initial release |

---

## 1. Purpose

This procedure defines the standard process for requesting, approving, creating, amending, reviewing, and revoking user access in the AIMS platform.

The objectives are to:
- ensure controlled and traceable user access management
- define clear responsibilities across requesting departments, approvers, AIMS coordination, and ICT
- maintain governance, auditability, and access integrity throughout the user lifecycle
- support operational continuity by providing timely and correct access setup

---

## 2. Scope

This procedure applies to all AIMS user access activities, including:
- new user account creation
- access role assignment or change
- module-level access amendment
- temporary or project-based access
- access suspension or deactivation
- access removal for resignation, transfer, or contract end
- periodic access review

**Applicable departments:** All departments using or requesting access to AIMS, including but not limited to OCC, Crew, Maintenance, Ground Operations, and supporting functions.

**Applicable systems:** AIMS and associated modules as configured in the production environment.

---

## 3. Definitions

| Term | Definition |
|------|-----------|
| **AIMS** | Airline Information Management System — the operational system platform supporting airline business processes |
| **Requester** | The individual or department representative who initiates the access request |
| **Approver** | The department manager or authorized person who approves the access request |
| **AIMS PIC** | AIMS Person-in-Charge / Coordinator — responsible for coordination, verification, and tracking |
| **ICT Administrator** | The ICT team member responsible for executing user access setup in the system |
| **Key User** | A designated department representative with functional knowledge of AIMS relevant to their area |
| **Privileged Access** | System access that includes administrative, configuration, or cross-department data visibility rights |
| **Access Scope** | The specific modules, functions, data views, or permissions assigned to a user |

---

## 4. Responsibilities

### 4.1 Requesting Department / Requester
- Submit the user access request with complete and accurate information.
- Confirm the business justification and required access scope.
- Obtain department manager approval before submission.
- Notify the AIMS PIC of any subsequent changes to the request.

### 4.2 Department Manager / Approver
- Review and verify the access request against the user's role and operational need.
- Confirm that the requested access is appropriate and does not conflict with segregation of duties.
- Approve or reject the request in writing (email or signed form).
- Take accountability for access assigned to personnel under their authority.

### 4.3 AIMS PIC / Coordinator
- Receive and log the access request.
- Verify request completeness, role logic, and access scope appropriateness.
- Coordinate with ICT for system execution.
- Coordinate with the vendor or support team when access setup requires system-level configuration.
- Maintain the access request tracker.
- Confirm access setup completion to the requesting department.
- Initiate periodic access reviews.

### 4.4 ICT / System Administrator
- Execute user creation, modification, or deactivation in AIMS upon approved instruction.
- Confirm completion to the AIMS PIC.
- Escalate to vendor support if the access configuration requires vendor-level action.
- Maintain system-level access logs.

### 4.5 Key User (where applicable)
- Assist in validating functional access requirements for their department.
- Support user onboarding or system orientation after access is granted.

### 4.6 Vendor / Support Team (where applicable)
- Execute access setup or configuration beyond the scope of internal ICT capability.
- Provide confirmation of completed configuration changes.

---

## 5. Procedure

### 5.1 Request Initiation

5.1.1. The requester shall complete the **AIMS User Access Request Form** (Appendix A) containing the following information:

| Field | Required |
|-------|----------|
| Request Date | ✅ |
| User Full Name | ✅ |
| Employee ID | ✅ |
| Department | ✅ |
| Position / Role | ✅ |
| System / Module Requested | ✅ |
| Access Scope Description | ✅ |
| Justification / Reason | ✅ |
| Effective Date (requested) | ✅ |
| Duration (if temporary) | If applicable |
| Manager Approval | ✅ |

5.1.2. The completed form shall be submitted to the AIMS PIC via email or the designated request channel.

5.1.3. Requests without department manager approval shall not be processed.

### 5.2 Review and Verification

5.2.1. The AIMS PIC shall review the request within **2 working days** of receipt for:
- completeness of required fields
- appropriateness of the requested access relative to the user's role
- potential duplication or conflict with existing access
- segregation of duty concerns (e.g., conflicting operational roles)

5.2.2. If the request is incomplete or unclear, the AIMS PIC shall return it to the requester with specific clarification needed.

5.2.3. For privileged access requests, additional verification or escalation to a senior approver may be required as defined in the **Approval Matrix** (Appendix B).

### 5.3 Approval

5.3.1. Standard access requests require approval from the user's **department manager**.

5.3.2. Privileged access or cross-department access requests require additional approval as defined in the Approval Matrix (Appendix B).

5.3.3. Approval shall be documented by:
- signed request form, **or**
- email confirmation from the approver's official email address

5.3.4. No system action shall be taken before approval is confirmed and documented.

### 5.4 Access Setup / Execution

5.4.1. Upon verified approval, the AIMS PIC shall instruct ICT to proceed with access setup.

5.4.2. ICT shall create or modify the user account in AIMS according to the approved request, including:
- user profile creation
- role and permission assignment
- module-level access configuration
- data scope limitation (if applicable)

5.4.3. If the access setup requires vendor-level configuration, the AIMS PIC shall coordinate with the vendor support team and track completion.

5.4.4. Access setup shall be completed within **3 working days** of approved instruction, unless constrained by vendor or system factors.

### 5.5 Confirmation and Handover

5.5.1. Upon completion, ICT or the AIMS PIC shall confirm to the requesting department:
- user account has been created or amended
- access scope as configured
- any login credentials or initial instructions (via secure channel)

5.5.2. The Key User or AIMS PIC may provide basic orientation or system usage briefing to new users where relevant.

5.5.3. The requester shall verify that the access is functional and correct. Any discrepancy shall be reported to the AIMS PIC within **3 working days** of confirmation.

### 5.6 Record Retention and Tracking

5.6.1. The following records shall be retained for each access request:

| Record | Retention |
|--------|-----------|
| Access Request Form (completed) | Minimum 2 years |
| Approval evidence (email or signed form) | Minimum 2 years |
| ICT / system setup confirmation | Minimum 2 years |
| Access Tracker entry | Ongoing |

5.6.2. The AIMS PIC shall maintain an **Access Request Tracker** (Appendix C) to log all requests, statuses, and outcomes.

---

## 6. Special Cases and Exception Handling

### 6.1 Urgent Access Request
- When immediate access is required for operational continuity, the AIMS PIC may initiate setup based on verbal or messaging confirmation from the department manager.
- Formal approval documentation must be completed within **1 working day** after the urgent setup.
- Urgent requests shall be flagged in the tracker with the reason.

### 6.2 Temporary Access
- Temporary access requests must include an expiration date.
- The AIMS PIC shall schedule a review at the expiration date to confirm revocation.
- Extension requests must follow the standard approval process.

### 6.3 Contractor or Third-Party Access
- Contractor or vendor personnel access requires approval from both the sponsoring department manager and the AIMS PIC.
- Access scope shall be limited to the minimum necessary for the contracted scope of work.
- Access shall be revoked upon contract completion or early termination.

### 6.4 Resignation, Transfer, or Contract End
- The requesting department or HR shall notify the AIMS PIC of any user departure, transfer, or contract end.
- Access shall be deactivated within **1 working day** of notification.
- The AIMS PIC shall confirm deactivation and update the tracker.

### 6.5 Failed or Incomplete Request
- Requests that cannot be completed due to system constraints, missing information, or rejected approval shall be returned to the requester with documented reason.
- Status shall be updated in the tracker as "Returned" or "Rejected".

---

## 7. Periodic Access Review

7.1. The AIMS PIC shall conduct a **quarterly access review** covering:
- active user accounts versus current personnel roster
- access scope versus current user role
- inactive or dormant accounts
- accounts flagged for temporary or restricted access

7.2. Findings shall be reported to department managers for validation.

7.3. Accounts identified as unnecessary, excessive, or orphaned shall be flagged for deactivation following the standard revocation process.

7.4. Review results and actions taken shall be documented and retained.

---

## 8. Escalation

| Situation | Escalation To | Response Time |
|-----------|---------------|---------------|
| Request delayed beyond SLA | AIMS PIC → ICT Manager | Within 1 working day |
| Access scope dispute | AIMS PIC → Department Manager + ICT Manager | Within 2 working days |
| Privileged access concern | AIMS PIC → Senior Management / IT Security | Immediate |
| Vendor-dependent delay | AIMS PIC → Vendor Account Manager | As per vendor SLA |
| Security / unauthorized access incident | AIMS PIC → ICT → Management | Immediate |

---

## 9. Appendices

### Appendix A — AIMS User Access Request Form

| Field | Value |
|-------|-------|
| **Request ID** | UAR-[YYYY]-[NNN] |
| **Request Date** | |
| **Request Type** | ☐ New User ☐ Role Change ☐ Module Access ☐ Temporary ☐ Deactivation |
| **User Full Name** | |
| **Employee ID** | |
| **Department** | |
| **Position / Role** | |
| **System / Module** | |
| **Access Scope Requested** | |
| **Justification** | |
| **Effective Date** | |
| **Expiry Date (if temporary)** | |
| **Manager Approval** | Name: _________ Signature: _________ Date: _________ |
| **AIMS PIC Review** | Name: _________ Date: _________ Status: ☐ Approved ☐ Returned |
| **ICT Execution** | Executed By: _________ Date: _________ |
| **Completion Confirmed** | ☐ Yes Date: _________ |
| **Notes** | |

---

### Appendix B — Approval Matrix

| Access Type | Approver Level 1 | Approver Level 2 | Notes |
|-------------|-------------------|-------------------|-------|
| Standard user access | Department Manager | — | Normal flow |
| Cross-department access | Department Manager | Receiving Dept Manager | Both approvals required |
| Privileged / admin access | Department Manager | AIMS PIC + ICT Manager | Additional review |
| Temporary access (≤30 days) | Department Manager | — | Must include expiry date |
| Contractor / third-party | Sponsoring Dept Manager | AIMS PIC | Limited scope only |

---

### Appendix C — Access Request Tracker (Column Structure)

| Column | Description |
|--------|-------------|
| Request ID | Unique identifier (UAR-YYYY-NNN) |
| Request Date | Date submitted |
| User Name | Full name |
| Employee ID | Staff ID |
| Department | Requesting department |
| Request Type | New / Change / Temporary / Deactivation |
| Access Scope | Module and permission summary |
| Approver | Name of approver |
| Approval Date | Date approved |
| Status | Pending / Approved / In Setup / Completed / Returned / Rejected |
| ICT Executed By | Name of ICT staff |
| Completion Date | Date access setup confirmed |
| Expiry Date | For temporary access |
| Notes | Any special remarks |

---

### Appendix D — Role Mapping Reference (Sample)

| Department | Typical Role | Default AIMS Module Access | Notes |
|------------|-------------|---------------------------|-------|
| OCC | Dispatcher | Flight Schedule, MVT, Crew Display (read) | Core operational access |
| Crew | Crew Planner | Crew Pairing, Roster, Crew Info | May include publish rights |
| Maintenance | MOC Controller | Aircraft Schedule, MEL, Maintenance Events | Limited to assigned fleet |
| Ground Ops | Station Coordinator | Flight Info, Ground Handling, Pax Connection | Station-scoped |
| ICT | System Admin | Admin Console, User Management | Privileged access |

> **Note:** This is a reference sample. Actual role-to-access mapping shall be maintained separately and updated as system configuration evolves.

---

*End of Document*

*Document Code: SOP-AIMS-UAM-001 | Version 1.0 | Classification: Internal Use Only*
