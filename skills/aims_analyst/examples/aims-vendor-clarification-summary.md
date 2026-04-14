# Example — Vendor Clarification Summary

## Use Case
Convert a vendor response into a management-usable and project-usable internal summary.

## Example Prompt
Summarize a vendor response on AIMS capability into: confirmed points, open points, operational implication, and recommended next action.
Audience: Hau, management, project stakeholders.

## Example Output

# Vendor Clarification Summary — AIMS Capability Review

## Confirmed Points
- Vendor confirmed that the requested function is supported in principle within the current platform design.
- The setup appears to rely on role, configuration, or operational filtering rather than full physical separation.
- The vendor has indicated that similar arrangements have existed in other client environments.

## Open Points Requiring Clarification
- exact access restriction logic by entity / role / data scope
- reporting behavior in a shared environment
- operational support impact if more than one business structure uses similar fleet or data pattern
- limitations that would require workaround or manual governance control

## Operational Implication
The current vendor answer suggests that the concept may be feasible, but feasibility alone is not enough.
Hau's team still needs to confirm whether the operating model remains controllable, supportable, and governance-safe in day-to-day use.

## Recommendation
Proceed with a second-round clarification focused on:
1. access segregation logic
2. reporting and visibility logic
3. support and issue management impact
4. known client examples closest to Hau's use case

## Why This Is A Good Example
- translates vendor wording into internal business meaning
- separates confirmed points from unanswered questions
- useful for project follow-up and management review
