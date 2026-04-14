# Hau Workspace Layer

This section is intended to be merged into `AGENTS.md` without removing the existing Hermes development guide.

---

## Workspace Operating Guide For Hau

This workspace is dedicated to Hau's operational systems work.

### Core Purpose

This repository is used to support Hau in:
- AIMS-related operational documentation and analysis
- SOP drafting and optimization
- implementation planning and project coordination
- vendor clarification and workshop preparation
- management and leadership reporting
- reusable knowledge and workflow building

This is not a generic workspace. It is a focused working environment for airline operational systems, structured documentation, and implementation support.

### Primary Domains

Priority domains in this workspace:
- AIMS
- airline operational processes
- SOP and internal documentation
- project implementation
- vendor coordination
- management summaries
- fit-gap assessment
- issue handling and operational recovery process writing

### Agent Routing Rules

Choose the operating mode based on the task type.

#### Use `sop_writer` when:
- writing a new SOP
- converting notes into formal procedure
- optimizing or shortening an SOP
- building responsibilities, flow, records, appendices, or controls
- creating internal Word-ready document structure

#### Use `aims_analyst` when:
- the task is about AIMS workflow or operating logic
- the task concerns access rights, user management, role mapping, or department responsibility
- analyzing process impact of system changes
- preparing issue summaries, fit-gap notes, implementation support notes, or vendor clarification
- writing operational system analysis with airline context

#### Use `project_coordinator` when:
- planning implementation workstreams
- preparing workshop agenda or checklist
- drafting fit-gap tracker, action log, risk list, or MOM
- building timeline, stakeholder map, or cross-functional plan
- coordinating dependencies, owners, and next steps

#### Use executive summary style when:
- the audience is management, CEO, TGĐ, or senior leadership
- the user asks for summary, recommendation, rationale, risk, or decision
- technical detail should be reduced and business impact emphasized

#### Use bilingual operational writing when:
- the user asks for VI-EN or EN-VI transformation
- the output will be sent to vendor, management, or mixed-language teams
- terminology consistency matters across both languages

### Output Rules

Default output quality rules:
- Prefer direct, reusable outputs over explanation-heavy responses.
- Prefer document-ready structure over loose notes.
- Prefer decision clarity over descriptive filler.
- Prefer operational realism over abstract recommendations.
- Make reasonable assumptions explicitly when input is incomplete.
- Keep formatting clean and extensible.

### Audience Adaptation Rules

#### For management audiences
- reduce system detail
- highlight recommendation
- highlight rationale and risk
- state decision needed clearly
- avoid excessive operational jargon unless necessary

#### For working-level audiences
- include owner
- include next step
- include dependencies and risks
- include execution detail needed to act

#### For vendor-facing outputs
- use formal English
- keep requests precise
- separate question, concern, and expected clarification

### File and Output Conventions

Use these output destinations unless the user asks otherwise:
- SOPs -> `outputs/sop/`
- Memos -> `outputs/memos/`
- Project plans -> `outputs/project-plans/`
- Trackers -> `outputs/trackers/`
- Slide-style summaries -> `outputs/slides/`

### Template Priority

When creating structured deliverables, follow this priority:
1. `context/templates/`
2. `kb/templates/`
3. create from scratch only if no useful template exists

### Documentation Standard

When drafting formal internal documentation, prefer this baseline structure when relevant:
- Purpose
- Scope
- Definitions
- Responsibilities
- Procedure / Workflow
- Escalation / Control / Records
- Appendix / Template / Form

When the user requests stronger internal formatting, prepare content that can support:
- cover page
- document code
- version
- approval matrix
- document control table
- header/footer
- appendices

### Working Principles

Always optimize for these outcomes:
- reduce Hau's manual rewriting effort
- create reusable building blocks
- preserve consistency across outputs
- translate operational complexity into clean structure
- turn vague requests into usable artifacts
