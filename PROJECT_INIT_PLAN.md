# Project Init Plan

## Objective
Initialize this repository with a practical project-start structure so the agent can support real project execution from day one.

The init will establish:
- project context files
- session continuity files
- governance and decision tracking files
- technical and product context files
- daily AI working rules

## Guiding Principle
The project should start with a lightweight but disciplined operating structure.
The goal is not documentation for its own sake.
The goal is to reduce context loss, improve AI continuity, and make planning, execution, and handoff easier.

## Phase 1 — Foundation Setup
Create the initial project memory structure:
- `memory-bank/projectbrief.md`
- `memory-bank/activeContext.md`
- `memory-bank/progress.md`
- `memory-bank/README.md`
- `memory-bank/SETUP_GUIDE.md`
- `CLAUDE.md`
- `AGENTS_PROJECT.md`

### Outcome
The repo has a working project memory system and session rules from the start.

## Phase 2 — Product / Technical Context
Create the project understanding layer:
- `memory-bank/productContext.md`
- `memory-bank/techContext.md`
- `memory-bank/systemPatterns.md`

### Outcome
The agent can understand why the project exists, how it should work, and what architecture or tech assumptions are in place.

## Phase 3 — Governance And Execution Control
Create tracking and decision files:
- `memory-bank/decisions-log.md`
- `memory-bank/SESSION_HANDOFF.md`

### Outcome
Major decisions, handoff context, and future continuity are controlled from the beginning.

## Phase 4 — First Fill-In Session
After file creation, complete the first working pass for:
1. project name
2. objective and scope
3. target user
4. initial phase / sprint
5. first 3 to 5 priority tasks
6. initial tech stack
7. known assumptions and blockers

### Outcome
The files stop being templates and become a live project operating system.

## Recommended First-Day Working Sequence
1. Fill `memory-bank/projectbrief.md`
2. Fill `memory-bank/activeContext.md`
3. Fill `memory-bank/productContext.md`
4. Fill `memory-bank/techContext.md`
5. Fill `memory-bank/progress.md`
6. Add first entry to `memory-bank/decisions-log.md`

## Suggested Ownership
- Hau: project objective, scope, business rules, priorities
- Agent: structure, drafting, update discipline, session continuity support
- Future contributors: append progress and decisions without breaking template discipline

## First Deliverables Expected After Init
Once the init is complete, the repo should be ready to support:
- planning sessions
- execution sessions
- structured follow-up
- session handoff
- better AI continuity
- reusable project memory

## Success Criteria
The init is successful when:
- all core memory-bank files exist
- the project can be resumed from `activeContext.md`
- the next session can continue with minimal explanation
- decisions and progress can be tracked without relying on chat history only
