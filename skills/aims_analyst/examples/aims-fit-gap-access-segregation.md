# Example — AIMS Fit-Gap: Access Segregation

## Use Case
Assess whether the current AIMS setup supports department or airline-specific access segregation.

## Example Prompt
Analyze whether AIMS can support access segregation by airline or department in a shared platform environment.
Summarize current understanding, operational impact, key gap, and recommended next action.

## Example Output

# AIMS Fit-Gap Note — Access Segregation in Shared Environment

## Current Situation
The target operating model requires multiple entities or departments to work within a common AIMS environment while maintaining controlled visibility and update rights.

## Desired State
Users should only see or modify data within their approved scope, while a limited number of group-level users may need broader visibility.

## Key Assessment
The main assessment point is not only whether the software is shared, but whether access, visibility, and workflow ownership can remain properly segregated in practice.

## Operational Impact
If segregation is weak or unclear:
- users may see irrelevant or sensitive data
- business ownership may become unclear
- reporting and workflow control may become harder to govern

## Gap / Open Point
The key gap is often not the existence of a shared platform itself, but the need to confirm:
- access control granularity
- data visibility rules
- operational filtering logic
- impact on future reporting and support governance

## Recommendation
Confirm with vendor in a structured way:
1. what access can be restricted by entity / role / data scope
2. what limitations exist
3. what workaround or standard client practice is available
4. what governance controls Hau should implement internally

## Why This Is A Good Example
- fit-gap style analysis
- business and operational framing, not only software commentary
- aligned with Hau's common AIMS evaluation work
