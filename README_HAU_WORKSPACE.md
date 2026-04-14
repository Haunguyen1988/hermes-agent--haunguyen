# README — Hau Workspace

This document explains how to use the Hau-specific workspace layer built on top of the Hermes agent repository.

The purpose of this workspace is to make the agent more useful for Hau's real work in airline operational systems, especially around AIMS, SOP/document writing, implementation coordination, vendor follow-up, analytics/reporting, and management communication.

---

## 1. What This Workspace Is

This is not a generic note collection.
It is a structured operating layer for a professional AI copilot designed around Hau's working style and domain.

The workspace is intended to help with:
- AIMS-related analysis and documentation
- SOP drafting and optimization
- implementation planning and project coordination
- vendor clarification and structured follow-up
- dashboards, reporting, and governance outputs
- management-ready summaries and executive notes

## 2. Main Building Blocks

### Identity And Style
These files define who the agent is supporting and how it should write:
- `SOUL.md`
- `AGENTS_HAU_LAYER.md`
- `context/user-profile/hau-profile.md`
- `context/user-profile/writing-style.md`

### Core Skills
These are the three main working skills:
- `skills/sop_writer/`
- `skills/aims_analyst/`
- `skills/project_coordinator/`

Each skill includes:
- `SKILL.md` — when and how to use the skill
- `examples/` — sample outputs that show the expected style and use case

### Domain Knowledge
These files help the agent understand Hau's working environment:
- `context/airline-domain/aims-overview.md`
- `context/airline-domain/department-roles.md`
- `context/airline-domain/vendor-engagement-rules.md`
- `context/airline-domain/analytics-reporting-rules.md`
- `context/airline-domain/integration-rules.md`

### Reusable Templates
These files help the agent generate structured outputs consistently:
- SOP template
- executive memo template
- project plan template
- MOM template
- fit-gap template
- action log template
- vendor question template
- dashboard spec template
- access request SOP template
- issue escalation template
- approval matrix template
- risk register template
- weekly status template

## 3. When To Use Each Skill

### Use `sop_writer`
Use this for:
- SOP drafting
- rewriting notes into internal documents
- formalizing responsibilities and procedures
- service down / escalation procedures
- access request procedures

### Use `aims_analyst`
Use this for:
- AIMS workflow analysis
- access segregation or user management analysis
- vendor clarification interpretation
- fit-gap assessment
- executive notes on AIMS topics
- operational impact and governance review

### Use `project_coordinator`
Use this for:
- rollout planning
- workshop preparation
- MOM creation
- action log tracking
- risk review
- stakeholder and dependency coordination

## 4. How To Work With The Agent

A practical working pattern is:
1. define the audience
2. define the output type
3. choose the most relevant skill
4. pull the nearest template
5. use an example if a similar output already exists
6. tailor the result to the exact use case

### Good prompt style
A strong prompt usually includes:
- the task
- the audience
- the intended output format
- any length or tone requirement
- any operational or approval constraint

Example:
"Write a management-ready executive note on AIMS access segregation using Recommendation / Rationale / Risk / Decision Needed. Keep it short and suitable for leadership review."

## 5. How The Files Should Influence Output

### If the task is documentation-heavy
Use:
- `context/user-profile/writing-style.md`
- `skills/sop_writer/SKILL.md`
- related SOP or access templates

### If the task is AIMS or vendor analysis
Use:
- `skills/aims_analyst/SKILL.md`
- AIMS overview
- vendor engagement rules
- fit-gap / vendor question templates

### If the task is project or follow-up oriented
Use:
- `skills/project_coordinator/SKILL.md`
- project plan template
- MOM template
- action log / risk / weekly status templates

### If the task is analytics or dashboard related
Use:
- analytics and reporting rules
- dashboard spec template
- weekly status or management summary pattern where needed

## 6. How To Extend This Workspace

The best way to improve the workspace is not to add random files.
The best way is to add:
- more real examples from Hau's work
- stronger templates for recurring outputs
- clearer rules where repeated editing patterns are visible

Recommended future additions:
- more examples under each skill
- bilingual examples if vendor and internal communication both matter
- a small set of approved document layouts for Word-ready outputs
- selected anonymized real cases for fit-gap, incident, and governance work

## 7. Examples Folder Guidance

The `examples/` folders are important.
They help the agent understand not only structure, but also tone, level of detail, and how Hau usually turns a problem into a usable artifact.

Current examples cover themes such as:
- SOP for access and service disruption
- department responsibilities
- AIMS fit-gap and vendor clarification summary
- executive note for management
- rollout plan, MOM, and action log

## 8. Recommended Default Workflow

For most tasks, use this internal decision flow:
- Is this a document? -> `sop_writer`
- Is this an AIMS / system / access / vendor analysis topic? -> `aims_analyst`
- Is this planning / follow-up / execution tracking? -> `project_coordinator`

Then ask:
- who is the audience?
- what decision or action should the output support?
- what template fits best?

## 9. Quality Standard

A good output in this workspace should be:
- easy to read quickly
- usable with minimal editing
- structured for real work
- operationally and managerially relevant
- clear on recommendation, ownership, or next action

## 10. Final Note

This workspace should gradually become Hau's professional AI operating layer.
It is most powerful when used with:
- clear task framing
- reusable templates
- example-driven refinement
- practical review after real use

The goal is not just to generate text.
The goal is to reduce manual rework and help Hau move faster with better structure, better clarity, and better execution support.
