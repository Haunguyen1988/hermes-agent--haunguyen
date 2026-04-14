# Vendor Question Pack — AIMS Crew Management Module Gaps

| **Reference** | VQP-AIMS-CRW-001 |
|---|---|
| **Date** | [DD/MM/YYYY] |
| **From** | Nguyễn Đình Hậu — AIMS Coordinator |
| **To** | [Vendor Name] — AIMS Support / Product Team |
| **Subject** | Clarification Required — Crew Management Module (Pairing, Rostering, FTL, Integration) |
| **Priority** | High — Impacts implementation timeline and operational readiness |

---

## 1. Purpose

We are conducting an internal fit-gap assessment of the AIMS Crew Management module to prepare for the upcoming system upgrade and operational expansion.

Several gaps have been identified between our current system configuration and our desired operating model. This question pack is intended to obtain vendor clarification on system capability, configuration options, known limitations, and recommended approaches before we finalize the upgrade scope and work order.

---

## 2. Background

Our airline is currently using the AIMS Crew Management module for pairing generation, rostering, and basic crew data management. As part of the planned upgrade, we need to confirm the following:

- whether identified gaps can be resolved through configuration
- whether additional module activation is required
- whether custom development or enhancement requests are needed
- what timeline and effort should be expected for each item

Departments affected: Crew Planning, Crew Control, OCC, Training, Flight Operations, ICT.

---

## 3. Current Understanding

Based on our internal review, we understand that:
- The pairing optimizer and legality engine support regulatory rules, but company-specific rules may require additional parameter configuration.
- The crew portal and notification modules are available within the current license but have not been activated.
- FTL calculation is operational, but local regulatory variations may not be fully parameterized.
- No standard integration currently exists between the training management system and AIMS crew qualification records.

**Please confirm or correct the above understanding in your response.**

---

## 4. Questions by Topic

### 4.1 Pairing — Rule Configuration (Ref: FGA CRW-01, CRW-02)

| # | Question | Context |
|---|----------|---------|
| Q1 | Can the pairing optimizer be configured to enforce company-specific rules (e.g., custom rest time, base constraints, maximum duty limits) beyond the regulatory minimums? | Currently, pairings require extensive manual adjustment because company rules are not reflected in the optimizer output. |
| Q2 | If yes, what is the process for configuring and validating additional rules? Please provide the recommended steps, responsible party (airline vs. vendor), and estimated effort. | We need to understand whether this is a self-service configuration or requires vendor engagement. |
| Q3 | Can the legality check engine be extended to include company-specific constraints in addition to regulatory checks? | Currently, legality only flags regulatory violations, not internal policy violations. |

### 4.2 Pairing — Deadhead Optimization (Ref: FGA CRW-03)

| # | Question | Context |
|---|----------|---------|
| Q4 | Does the pairing optimizer support automatic consideration of deadhead legs for crew positioning, including cost optimization? | Currently, deadhead legs are manually inserted and tracked outside the optimizer. |
| Q5 | If this capability exists, what configuration or data input is required to enable it? | We need to assess feasibility before including this in the upgrade scope. |
| Q6 | If not currently supported, is this a planned enhancement? What is the expected availability timeline? | This will help us decide whether to maintain the current manual workaround or plan for system support. |

### 4.3 Crew Portal and Notifications (Ref: FGA CRW-04, CRW-06)

| # | Question | Context |
|---|----------|---------|
| Q7 | Please confirm that the crew portal module is included in our current license and can be activated without additional licensing cost. | We plan to activate the crew portal for roster publication and crew self-service features. |
| Q8 | What is the standard activation process and estimated timeline for crew portal deployment (including notification workflow configuration)? | We would like to understand dependencies, prerequisites, and recommended pilot approach. |
| Q9 | Does the crew portal support crew swap/trade requests with planner approval workflow? If yes, how is this configured? | We want to reduce manual swap handling currently done via email. |
| Q10 | What notification channels are supported (email, push notification, SMS, in-app)? Are there any prerequisites for each channel? | We need to select the most practical notification method for our crew base. |

### 4.4 FTL / Duty Time Configuration (Ref: FGA CRW-09, CRW-10)

| # | Question | Context |
|---|----------|---------|
| Q11 | Can the FTL calculation engine be configured to reflect local Civil Aviation Authority (CAA) regulations in addition to the ICAO baseline? | We have identified gaps between the current FTL calculation and local regulatory requirements. |
| Q12 | If yes, what is the process for validating that FTL calculations comply with our specific regulatory framework? Does the vendor provide a validation tool or test scenario support? | Accuracy of FTL calculation is critical for regulatory compliance. |
| Q13 | Is it possible to provide real-time FTL status visibility to OCC / Crew Control during disruption management? What display or integration options are available? | During disruption, OCC needs to quickly identify available crew by remaining duty time. |

### 4.5 Training Integration (Ref: FGA CRW-08)

| # | Question | Context |
|---|----------|---------|
| Q14 | Does AIMS offer a standard integration or import interface for crew training and qualification records from an external training management system? | Currently, training records are manually entered into AIMS, causing delays and data entry errors. |
| Q15 | If a standard connector is available, what data format and fields are supported? What setup effort is expected? | We need to evaluate build vs. maintain-manual-process decision. |
| Q16 | If no standard connector exists, what is the recommended approach for maintaining crew qualification data synchronization? Are there client examples or best practices? | We want to reduce dual maintenance and improve data currency. |

### 4.6 Reporting Capability (Ref: FGA CRW-11)

| # | Question | Context |
|---|----------|---------|
| Q17 | Does AIMS include a report builder or ad-hoc reporting tool that allows trained end users to create or customize crew management reports without vendor support? | Currently, all custom report requests must go through vendor or ICT. |
| Q18 | If yes, what training or certification is recommended for key users? | We plan to train 2-3 key users to handle routine reporting needs internally. |

---

## 5. Expected Response

We kindly request the following from your team:

1. **Written response** to each question above, organized by section number.
2. **Confirmation** of capability, limitation, or workaround for each item.
3. **Estimated effort and timeline** where configuration, activation, or development is required.
4. **Recommendation** on sequencing if multiple items should be addressed in a specific order.

We would appreciate receiving your response within **10 working days** to align with our internal planning cycle.

---

## 6. Priority / Critical Items

The following questions are **blocking our implementation planning** and require priority attention:

| Priority | Questions | Reason |
|----------|-----------|--------|
| 🔴 Critical | Q1, Q2, Q3 | Pairing rule configuration — directly affects crew scheduling quality |
| 🔴 Critical | Q11, Q12 | FTL compliance — regulatory exposure risk |
| 🔴 Critical | Q7, Q8 | Crew portal activation — impacts roster communication for entire crew base |
| 🟡 High | Q9, Q10, Q13 | Portal features and OCC integration — operational efficiency |
| 🟢 Normal | Q4-Q6, Q14-Q18 | Planning items — no immediate timeline dependency |

---

## 7. Internal Follow-Up Note

> ⚠️ **This section is for internal use only. Do NOT include in vendor communication.**

| Item | Internal Note |
|------|---------------|
| **Originating document** | FGA-AIMS-CRW-001 (Fit-Gap Assessment — Crew Management Module) |
| **Departments requesting** | Crew Planning, OCC, Training |
| **Decision depending on answer** | Upgrade scope finalization, portal activation timeline, FTL compliance validation |
| **After vendor response** | 1. Map confirmed capabilities to fit-gap table. 2. Update gap status. 3. Prepare management summary with recommendation. 4. Schedule workshop if complex items remain. |
| **Escalation if no response** | Follow up at T+7 days. Escalate to vendor account manager at T+14 days. |

---

## Appendix — Short Email Version

> Use this version for initial email. Attach the full question pack as a document.

---

**Subject:** Clarification Required — AIMS Crew Management Module (18 Questions)

Dear [Vendor Contact Name],

We are conducting an internal fit-gap review of the AIMS Crew Management module in preparation for our planned system upgrade.

We have identified several areas requiring vendor clarification, including:
1. Pairing optimizer and legality rule configuration (company-specific rules)
2. Crew portal and notification module activation
3. FTL calculation compliance with local CAA regulations
4. Training system integration options
5. Reporting capability for end users

Please find the detailed question pack attached (Reference: VQP-AIMS-CRW-001, 18 questions organized by topic).

We would appreciate your written response within **10 working days**. Priority items are highlighted in Section 6 of the document.

Please do not hesitate to contact us if any question requires further context from our side.

Best regards,
Nguyễn Đình Hậu
AIMS Coordinator
[Department / Organization]
[Contact information]

---

*End of Document*

*Reference: VQP-AIMS-CRW-001 | Version 1.0 | Classification: Internal Use Only (remove Section 7 before sending to vendor)*
