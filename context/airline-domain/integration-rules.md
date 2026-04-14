# Integration Rules

## Purpose Of This File

This file defines how the agent should think about integrations in Hau's working context.

It is intended for airline operational systems, application management, data flow coordination, reporting dependency, and implementation planning.
The goal is to help the agent produce practical outputs for integration assessment, issue handling, documentation, vendor coordination, and project planning.

## Integration In Hau's Context

In Hau's work, integrations should be treated as operational dependencies, not only technical interfaces.
An integration affects:
- data availability
- process timing
- user trust in system outputs
- reporting accuracy
- cross-department coordination
- incident impact and recovery complexity

This is consistent with Hau's background in supporting operational alignment between AIMS and connected systems such as AMOS and PSS, while also driving reporting visibility and business use of system outputs.

## Default Integration Objective

When supporting an integration-related task, the agent should help Hau:
- clarify source and target systems
- understand what business process depends on the interface
- identify required data, timing, and ownership
- assess impact if the integration fails or is delayed
- structure questions, controls, and next steps clearly

## Core Integration Lens

When analyzing an integration topic, think through this sequence:
1. What business or operational process depends on the integration?
2. Which system is the source and which is the target?
3. What data or event must move between systems?
4. What timing or frequency is required?
5. Who owns the data, the process, and the technical support path?
6. What happens operationally if the interface is late, wrong, or unavailable?
7. What output is needed: question list, issue escalation, fit-gap note, design summary, tracker, or management summary?

## Integration Analysis Rule

When reviewing an integration, the agent should clarify:
- source system
- target system
- data items / fields involved
- trigger or schedule
- dependency on manual step or automated handoff
- validation / reconciliation need
- error handling path
- owner and support path

## Business-First Rule

Do not describe integration only in technical terms.
Always link the integration to business or operational use.
Examples:
- crew data availability
- maintenance information visibility
- reporting refresh reliability
- schedule support process
- access or approval dependency

## Timing And Dependency Rule

Timing matters.
The agent should explicitly consider:
- real-time versus batch need
- critical cutoff or operational timing
- dependency on upstream data quality
- downstream reporting or workflow dependency
- impact of delay on decision-making or execution

## Data Quality And Reconciliation Rule

Integration topics often create reporting and control issues when data is incomplete, delayed, duplicated, or mismatched.
The agent should consider:
- source-of-truth definition
- field mapping clarity
- reconciliation check
- missing or duplicate record risk
- exception handling and validation logic

## Issue Handling Rule

When an integration issue occurs, frame it as:
- issue summary
- affected interface or data flow
- period / timing affected
- business impact
- actions taken
- required support
- workaround if available
- next update expectation

## Vendor Coordination Rule

When the topic involves vendor clarification on an integration:
- ask what is supported natively
- ask what field / format / trigger is required
- ask where the responsibility boundary sits
- ask what existing client pattern or workaround exists if helpful
- separate confirmed capability from assumption

## Implementation Rule

When planning an integration activity, the agent should identify:
- business requirement
- source / target mapping
- dependency by department
- test and validation requirement
- owner for issue follow-up
- fallback / contingency if the interface is unstable

## Documentation Rule

When documenting integration content, the agent should make visible:
- system names
- business purpose
- data flow direction
- timing
- validation point
- owner / support path
- escalation path if the interface fails

## Reporting And Analytics Dependency Rule

The agent should recognize that many reporting issues are actually integration issues.
If KPI output, dashboard accuracy, or recurring report timing is weak, the agent should consider whether the root cause may involve:
- delayed source feed
- incorrect mapping
- inconsistent field definition
- failed refresh sequence
- mismatch between systems

## Writing Style Rule

Integration outputs should be:
- structured
- practical
- dependency-aware
- clear enough for both business and technical stakeholders

Avoid:
- pure technical jargon with no operational meaning
- vague statements such as "integration issue exists" without data flow or impact context

## Quality Standard

A good integration-related output should help Hau:
- understand what depends on what
- explain risk and impact clearly
- ask better questions to ICT or vendors
- plan follow-up and mitigation more effectively
- connect system interface behavior to business and operational use
