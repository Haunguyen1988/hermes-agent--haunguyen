# Fit-Gap Assessment — AIMS Crew Management Module

| **Document Code** | FGA-AIMS-CRW-001 |
|---|---|
| **Version** | 1.0 |
| **Date** | 2026-04-14 |
| **Prepared By** | Nguyễn Đình Hậu — AIMS Coordinator |
| **Reviewed By** | [Reviewer Name / Title] |
| **Classification** | Internal Use Only |

---

## 1. Objective

This fit-gap assessment evaluates the current AIMS Crew Management module against the airline's operational requirements to:
- identify gaps between the current system capability and the desired operating model
- determine root causes and operational impact of each gap
- propose actions with clear ownership and priority
- support vendor discussion, implementation planning, and management decision-making

---

## 2. Scope

This assessment covers the following areas within the AIMS Crew Management module:

| Area | In Scope |
|------|----------|
| Crew Pairing | ✅ |
| Crew Rostering | ✅ |
| Crew Notification / Communication | ✅ |
| Crew Qualification & Currency Tracking | ✅ |
| Crew Duty Time / FTL Monitoring | ✅ |
| Crew Self-Service (Portal / Mobile) | ✅ |
| Reporting & Dashboard | ✅ |
| Integration with OCC / Flight Ops | ✅ |
| Payroll Integration | ❌ (out of scope for this phase) |

---

## 3. Assessment Context

- **Current situation:** The airline currently operates crew management through a combination of AIMS modules and manual processes (spreadsheets, email-based notifications, offline tracking).
- **Why now:** The airline is preparing for an AIMS upgrade and operational expansion. Crew department has raised several operational pain points that need to be assessed before finalizing the upgrade scope and vendor work order.
- **Stakeholders affected:** Crew Planning, Crew Control, OCC, Training Department, Flight Operations, ICT, Vendor/Support Team, Management.

---

## 4. Fit-Gap Table

### 4.1 Crew Pairing

| ID | Process / Function | Current State | Desired State | Gap | Root Cause | Impact | Feasibility | Proposed Action | Owner | Priority | Status |
|----|--------------------|---------------|---------------|-----|------------|--------|-------------|-----------------|-------|----------|--------|
| CRW-01 | Pairing generation | Pairings are generated in AIMS but require extensive manual adjustment due to limited rule configuration | System-generated pairings that comply with regulatory and company rules with minimal manual adjustment | Pairing optimizer does not fully reflect current company rules (rest time, base constraints, duty limits) | Rule engine configuration incomplete; some company-specific rules not parameterized | High manual effort; risk of non-compliant pairings; slow turnaround | Medium — requires vendor support for rule configuration | 1. Audit current rule set vs. actual company rules. 2. Submit gap list to vendor for configuration. | AIMS PIC + Crew Planning | 🔴 High | Open |
| CRW-02 | Pairing legality check | Legality check runs but does not flag all company-specific constraints (only regulatory minimums) | Legality check includes both regulatory and company-specific rules | Company rules not fully configured in system rule engine | Configuration gap | Crew planners must manually verify each pairing against internal policy | Low — configuration change, no development | Request vendor to update rule parameters | AIMS PIC | 🔴 High | Open |
| CRW-03 | Deadhead management | Deadhead legs are manually inserted and tracked | Deadhead legs automatically considered during pairing optimization and displayed in crew views | Optimizer does not account for deadhead cost/positioning logic | Feature limitation or configuration gap — needs vendor confirmation | Suboptimal positioning; increased cost; manual tracking | Medium — may require vendor enhancement | Raise clarification with vendor on optimizer capability | AIMS PIC + Vendor | 🟡 Medium | Pending vendor |

### 4.2 Crew Rostering

| ID | Process / Function | Current State | Desired State | Gap | Root Cause | Impact | Feasibility | Proposed Action | Owner | Priority | Status |
|----|--------------------|---------------|---------------|-----|------------|--------|-------------|-----------------|-------|----------|--------|
| CRW-04 | Roster publication | Rosters are finalized in AIMS and published via email/PDF | Rosters published directly to crew via crew portal or mobile app with instant notification | Crew portal not configured or not deployed; notification module not enabled | Deployment gap — module available but not activated | Crew receive roster updates late; complaints and manual follow-up | Low — activation and configuration | 1. Activate crew portal module. 2. Configure notification workflow. 3. Pilot test with one crew base. | ICT + AIMS PIC | 🔴 High | Open |
| CRW-05 | Roster change management | Changes communicated by phone or email; no audit trail in system | All roster changes logged in system with timestamp, reason, and approver | Change log feature exists but not consistently used; process not enforced | Process gap — no SOP mandating system-based change logging | Poor traceability; dispute risk; audit weakness | Low — process and SOP change | 1. Draft SOP for roster change logging. 2. Configure mandatory fields in AIMS. | Crew Planning + AIMS PIC | 🟡 Medium | Open |
| CRW-06 | Crew swap / trade | Crew swaps handled manually via email between planners | Crew can submit swap requests via portal; planner approves in system | Self-service swap feature not enabled | Module not activated | Manual workload on planners; slow response to crew requests | Medium — requires portal activation + workflow configuration | Bundle with CRW-04 portal activation | ICT + AIMS PIC | 🟡 Medium | Open |

### 4.3 Crew Qualification & Currency

| ID | Process / Function | Current State | Desired State | Gap | Root Cause | Impact | Feasibility | Proposed Action | Owner | Priority | Status |
|----|--------------------|---------------|---------------|-----|------------|--------|-------------|-----------------|-------|----------|--------|
| CRW-07 | Qualification tracking | Crew qualifications tracked in AIMS but currency expiry alerts are not automated | System-generated alerts for expiring qualifications sent to Training and Crew Planning 30/60/90 days before expiry | Alert/notification module not configured for qualification events | Configuration gap | Risk of rostering unqualified crew; late detection of expiring currency | Low — configuration and notification setup | Configure expiry alert rules in AIMS; link to email/portal notification | Training + AIMS PIC | 🔴 High | Open |
| CRW-08 | Training record sync | Training completion manually entered into AIMS from separate training tracker | Training records automatically flow from training system to AIMS | No integration between training system and AIMS | Integration gap — requires interface development or vendor connector | Delay in updating crew currency; data entry errors; dual maintenance | High — requires development or vendor support | 1. Check vendor for standard training integration. 2. If not available, evaluate manual sync SOP vs. custom interface cost. | AIMS PIC + ICT + Vendor | 🟢 Low (Phase 2) | Pending vendor |

### 4.4 Duty Time / FTL Monitoring

| ID | Process / Function | Current State | Desired State | Gap | Root Cause | Impact | Feasibility | Proposed Action | Owner | Priority | Status |
|----|--------------------|---------------|---------------|-----|------------|--------|-------------|-----------------|-------|----------|--------|
| CRW-09 | FTL calculation | FTL calculated in AIMS but does not include all local regulatory variations | FTL calculation fully reflects both ICAO baseline and local CAA requirements | Local regulatory rules not fully parameterized | Configuration gap — vendor needs to confirm rule customization capability | Risk of FTL violation; regulatory exposure | Medium — vendor configuration + validation | 1. Map local FTL rules vs. current AIMS config. 2. Submit to vendor for configuration review. 3. Validate with test scenarios. | AIMS PIC + Flight Ops + Vendor | 🔴 High | Open |
| CRW-10 | Real-time FTL monitoring | FTL status available in AIMS but not pushed to OCC/Crew Control in real-time | OCC and Crew Control have real-time visibility of crew FTL status during disruption management | FTL data not integrated into OCC operational display | Integration / display configuration gap | During disruption, OCC cannot quickly identify available crew by FTL status | Medium — may require dashboard or view configuration | 1. Clarify with vendor on real-time FTL view options. 2. Evaluate OCC display integration. | OCC + AIMS PIC + Vendor | 🟡 Medium | Pending vendor |

### 4.5 Reporting & Dashboard

| ID | Process / Function | Current State | Desired State | Gap | Root Cause | Impact | Feasibility | Proposed Action | Owner | Priority | Status |
|----|--------------------|---------------|---------------|-----|------------|--------|-------------|-----------------|-------|----------|--------|
| CRW-11 | Crew utilization report | Basic reports available; custom reports require vendor or ICT support | Standard crew utilization reports available; power users can build custom reports | Limited report customization capability for end users | Report builder not enabled or not trained | Crew management relies on ICT/vendor for every reporting request | Low — enable report builder + train key users | 1. Assess report builder module availability. 2. Train 2-3 key users. | AIMS PIC + Crew Planning | 🟡 Medium | Open |
| CRW-12 | Management dashboard | No consolidated crew KPI dashboard | Visual dashboard showing: utilization rate, FTL margin, qualification status, roster stability | No dashboard module configured | Feature gap | Management lacks quick operational view of crew performance | Medium — requires dashboard setup or Power BI integration | 1. Define top 5 crew KPIs. 2. Evaluate AIMS built-in dashboard vs. Power BI integration. | AIMS PIC + Management | 🟢 Low (Phase 2) | Open |

---

## 5. Summary of Key Gaps

### 🔴 Critical Gaps (Blocking or High Risk)

| ID | Gap Summary | Why Critical |
|----|-------------|-------------|
| CRW-01 | Pairing optimizer rules incomplete | High manual effort, compliance risk |
| CRW-02 | Legality check missing company rules | Crew may be assigned non-compliant pairings |
| CRW-04 | Crew portal not activated | Delays in roster communication, crew dissatisfaction |
| CRW-07 | Qualification expiry alerts not configured | Risk of rostering unqualified crew |
| CRW-09 | Local FTL rules not fully configured | Regulatory exposure |

### 🟡 Important but Manageable (Workaround Available)

| ID | Gap Summary | Current Workaround |
|----|-------------|--------------------|
| CRW-03 | Deadhead optimization not automated | Manual insertion by planners |
| CRW-05 | Roster changes not logged in system | Email-based communication (no audit trail) |
| CRW-06 | Crew swap not self-service | Manual email process via planners |
| CRW-10 | Real-time FTL not visible to OCC | Planners check manually during disruption |
| CRW-11 | Custom reporting limited | ICT/vendor builds reports on request |

### 🟢 Phase 2 / Nice-to-Have

| ID | Gap Summary | Recommendation |
|----|-------------|----------------|
| CRW-08 | Training record integration | Evaluate in Phase 2 after core gaps resolved |
| CRW-12 | Management dashboard | Build after KPI definition and core data quality confirmed |

---

## 6. Recommendations

### Quick Wins (Low effort, High impact)
1. **Configure qualification expiry alerts** (CRW-07) — Low effort, immediate safety benefit
2. **Activate crew portal module** (CRW-04) — Module already available, needs activation and pilot test
3. **Draft SOP for roster change logging** (CRW-05) — Process change, no system development needed

### Medium-Term (Vendor support required)
4. **Audit and complete pairing rule configuration** (CRW-01, CRW-02) — Prepare rule gap list, submit to vendor
5. **Map and configure local FTL rules** (CRW-09) — Critical for regulatory compliance
6. **Evaluate deadhead optimization capability** (CRW-03) — Raise with vendor during next workshop

### Decision-Dependent
7. **Real-time FTL integration for OCC** (CRW-10) — Pending vendor clarification on technical feasibility
8. **Training system integration** (CRW-08) — Cost-benefit decision needed: custom interface vs. manual SOP
9. **Management dashboard** (CRW-12) — Requires KPI agreement from management + tool selection (AIMS vs. Power BI)

---

## 7. Next Steps

| # | Action | Owner | Target Date | Dependency |
|---|--------|-------|-------------|------------|
| 1 | Compile pairing rule gap list (CRW-01, CRW-02) | Crew Planning + AIMS PIC | [T+2 weeks] | Internal review |
| 2 | Submit rule gap list and FTL configuration request to vendor (CRW-01, CRW-02, CRW-09) | AIMS PIC | [T+3 weeks] | Step 1 complete |
| 3 | Activate crew portal and configure notification (CRW-04, CRW-06) | ICT + AIMS PIC | [T+4 weeks] | ICT resource |
| 4 | Configure qualification expiry alerts (CRW-07) | AIMS PIC + Training | [T+2 weeks] | None |
| 5 | Draft SOP for roster change logging (CRW-05) | AIMS PIC | [T+2 weeks] | None |
| 6 | Prepare vendor clarification pack for CRW-03, CRW-10, CRW-08 | AIMS PIC | [T+3 weeks] | None |
| 7 | Present fit-gap summary to management with recommendations | AIMS PIC | [T+4 weeks] | Steps 1-6 |

---

## 8. Prioritization Matrix

```
              HIGH IMPACT
                  │
    CRW-01 ●     │     ● CRW-07
    CRW-02 ●     │     ● CRW-04
    CRW-09 ●     │     ● CRW-05
                  │
──────────────────┼──────────────────
   HIGH EFFORT    │    LOW EFFORT
                  │
    CRW-08 ○     │     ○ CRW-11
    CRW-10 ●     │     ○ CRW-06
                  │     ○ CRW-12
              LOW IMPACT

● = Phase 1 priority    ○ = Phase 2 / manageable
```

**Decision rule:**
- Top-right quadrant (High impact + Low effort) → Implement immediately
- Top-left quadrant (High impact + High effort) → Plan vendor engagement
- Bottom-right quadrant (Low impact + Low effort) → Schedule in Phase 2
- Bottom-left quadrant (Low impact + High effort) → Defer or evaluate ROI

---

*End of Document*

*Document Code: FGA-AIMS-CRW-001 | Version 1.0 | Classification: Internal Use Only*
