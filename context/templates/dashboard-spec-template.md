# Dashboard Specification Template

Use this template when Hau needs to define a dashboard, reporting view, KPI board, or management visibility product.

The purpose of this template is to convert a reporting request into a structured specification that is clear for business users, analysts, ICT teams, or developers.

---

# [Dashboard / Reporting Product Title]

## 1. Objective
State what the dashboard is intended to achieve.
Focus on the business or operational decision it should support.

Examples:
- improve management visibility of operational performance
- support weekly monitoring of key airline operations KPIs
- reduce time needed to prepare recurring reports
- highlight exceptions and action priorities for working teams

## 2. Audience
Define the primary audience.
Examples:
- senior management
- operations leadership
- OCC team
- crew management team
- ICT / system monitoring team

If there are multiple audiences, distinguish between primary and secondary users.

## 3. Business Questions To Answer
List the main questions the dashboard should answer.
Prefer 3 to 7 questions.

Examples:
- What are the current top operational performance signals?
- Where are the biggest deviations versus target?
- Which trend requires immediate attention?
- Which department or process needs follow-up?

## 4. KPI Scope
List the main KPIs to include.
For each KPI, define:
- KPI Name
- Definition
- Unit
- Data Source
- Calculation Logic
- Update Frequency
- Owner / Business Owner

## 5. Comparison / Benchmark Requirement
Define what comparison is required.
Examples:
- versus previous day
- versus previous week
- versus previous month
- versus same period last year
- versus target

## 6. Filter And Drilldown Requirement
List the filters or segmentation the dashboard should support.
Examples:
- date / period
- fleet
- station
- department
- route / network
- aircraft type
- operational category

If drilldown is required, state what users should be able to drill into.

## 7. Visual Layout Requirement
Describe the expected dashboard structure.

Suggested sequence:
- top summary KPI row
- trend section
- exception / alert section
- breakdown by category / owner / station / process
- detailed view or supporting table

State any preference for:
- one-page executive layout
- working-level detailed layout
- mobile-friendly or presentation-friendly view

## 8. Data Logic And Quality Requirements
State any important data rules.
Examples:
- source system priority
- definition alignment requirement
- handling of missing records
- data refresh timing
- reconciliation need between systems

## 9. Alert / Threshold Requirement
If the dashboard should highlight exceptions, define:
- threshold logic
- alert condition
- priority logic
- who should act when threshold is breached

## 10. Reporting Output Requirement
State whether the output should also support:
- weekly summary
- monthly report
- export to Excel / PowerPoint
- management email summary
- PDF snapshot

## 11. Risks / Constraints
Identify known reporting or implementation constraints.
Examples:
- incomplete data source
- inconsistent KPI definition
- manual data dependency
- unclear ownership
- system limitation

## 12. Recommendation / Next Steps
State the next actions needed to move the dashboard forward.
Examples:
- confirm KPI definitions
- validate data source mapping
- prioritize phase 1 KPI scope
- align audience and refresh frequency

---

## Optional KPI Table Structure

Use this simple table when needed:
- KPI
- Definition
- Source
- Logic
- Frequency
- Owner
- Note

## Writing Rules For This Template

When using this dashboard spec template:
- start from decisions and business questions
- keep KPI scope focused
- make data logic explicit
- distinguish management view from working-level detail
- avoid overloading the design with too many visuals or metrics

## Quality Standard

A good dashboard specification should help Hau:
- align stakeholders faster
- avoid KPI definition confusion
- guide analysts or developers clearly
- reduce rework during dashboard build
- ensure the reporting product is decision-useful from the start
