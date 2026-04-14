# Fit-Gap Template

Use this template when Hau needs to assess the difference between current system capability / current process and the desired business or operational requirement.

This template is intended for practical implementation work, vendor clarification, system assessment, and decision support.
It should help the agent produce outputs that are structured, comparable, and easy to act on.

This approach aligns with Hau's default system evaluation method: current state → desired state → gap → root cause → improvement proposal, with priority based on impact and feasibility fileciteturn22file1.

---

# [Fit-Gap Assessment Title]

## 1. Objective
State the purpose of the fit-gap review.
Example:
- assess whether the current AIMS setup supports the required operating model
- identify process and system gaps before implementation
- confirm whether vendor capability matches operational need

## 2. Scope
Define what is covered.
Examples:
- module / function
- department process
- access model
- reporting requirement
- integration point

## 3. Assessment Context
Briefly state:
- current business situation
- why the review is needed now
- which departments or stakeholders are affected

## 4. Fit-Gap Table

Use this baseline structure:
- ID
- Process / Function
- Current State
- Desired State
- Gap Description
- Root Cause / Constraint
- Impact
- Feasibility / Complexity
- Proposed Action
- Owner
- Priority
- Status / Note

### Guidance For Each Column

**Process / Function**
State the business process, module, report, integration point, or workflow area being reviewed.

**Current State**
Describe how it works now.
Keep the wording factual and concise.

**Desired State**
Describe what the business or operational team needs.

**Gap Description**
State the difference clearly.
This should be specific, not generic.

**Root Cause / Constraint**
State the main reason for the gap if known.
Examples:
- system limitation
- configuration not enabled
- unclear process ownership
- incomplete data structure
- access model constraint
- vendor clarification still pending

**Impact**
State the practical effect.
Examples:
- operational inefficiency
- control weakness
- reporting delay
- manual workaround
- risk to readiness
- data visibility issue

**Feasibility / Complexity**
Indicate whether the change is:
- low / medium / high effort
- config / process / integration / enhancement dependent

**Proposed Action**
State the best next action.
Examples:
- confirm with vendor
- redesign process
- apply configuration change
- maintain workaround temporarily
- escalate for decision

**Owner**
State who should drive the next step.

**Priority**
Use a simple scale such as High / Medium / Low unless the user asks otherwise.

## 5. Summary Of Key Gaps
After the table, summarize:
- top 3 to 5 most important gaps
- which ones are blocking implementation or operational readiness
- which ones can be managed by workaround
- which ones require leadership or vendor decision

## 6. Recommendations
State concise recommendations.
Preferred pattern:
- quick wins
- medium-term fixes
- decision-dependent items

## 7. Next Steps
List concrete follow-up actions.
Examples:
- validate desired state with department owner
- send clarification pack to vendor
- prioritize high-impact gaps
- confirm workaround until permanent solution is available

---

## Optional Prioritization Rule

When the user needs prioritization, classify gaps by:
- impact to operations
- control or governance risk
- implementation dependency
- effort / feasibility

A strong default decision lens is:
- high impact + high feasibility = prioritize first
- high impact + low feasibility = escalate / phase plan

## Writing Rules For This Template

When using this template:
- keep current state and desired state distinct
- avoid vague terms like "not good" or "needs improvement"
- make the gap explicit
- connect the gap to operational or business effect
- make the proposed action realistic
- use this as a working tool, not a theoretical assessment

## Quality Standard

A good fit-gap output should help Hau:
- compare current versus target state clearly
- identify what truly matters
- discuss with vendor or departments efficiently
- prioritize action
- support implementation or management decision-making
