# Redaction Policy

This file defines how real documents, notes, emails, case summaries, trackers, and work products should be sanitized before being added to `kb/examples-real/`.

The goal is to preserve useful working patterns while preventing exposure of private, sensitive, operational, commercial, or security-relevant information.

---

## 1. Purpose

The `kb/examples-real/` folder should help the agent learn from realistic material.
However, it must not become a storage location for raw confidential content.

This policy answers three questions:
- what may be kept
- what must be masked or generalized
- what level of sanitization is safe enough for repository storage

## 2. Core Principle

Keep the pattern. Remove the sensitivity.

The purpose of a sanitized example is to preserve:
- structure
- tone
- workflow logic
- decision pattern
- communication style
- template usage
- useful reasoning pattern

The purpose is NOT to preserve:
- exact identity
- exact confidential data
- exact commercially sensitive detail
- real secrets or internal-only operational information

## 3. What Can Usually Be Kept

The following items are usually safe to keep if they do not reveal confidential context:

### A. Document Structure
- headings
- section order
- numbering style
- table structure
- template layout
- responsibility breakdown style

### B. Writing Pattern
- formal tone
- concise style
- recommendation format
- management summary structure
- vendor communication pattern
- issue escalation wording style

### C. Generalized Business Logic
- request -> review -> approval -> execution -> confirmation flow
- incident detection -> escalation -> workaround -> recovery -> closure flow
- fit-gap logic
- dashboard/reporting logic
- action tracking pattern
- risk escalation logic

### D. Generalized Roles
These may usually be kept in generic or department-level form:
- requester
- approver
- PIC
- ICT
- vendor
- management
- department representatives

Department names such as OCC, Crew, Maintenance, Ground Ops, ICT are usually acceptable when used at a generic level, unless the specific scenario itself is sensitive.

### E. Generic Time References
These are usually safe if generalized:
- "same day"
- "within 24 hours"
- "weekly review"
- "during implementation phase"

## 4. What Must Be Masked Or Generalized

The following should be masked, replaced, or generalized before storing in the repo.

### A. Personal Identifiers
Always mask or remove:
- full names of staff
- personal email addresses
- phone numbers
- employee IDs
- signatures
- personal usernames
- personal messaging handles

### B. Sensitive Organization Identifiers
Mask or generalize when not necessary for pattern learning:
- specific internal team names below department level
- direct names of individuals in leadership or support chains
- internal distribution lists
- personal contact points

### C. Sensitive Operational Data
Always mask or generalize:
- crew names
- passenger data
- flight-specific sensitive details if not essential
- exact disruption event details if operationally sensitive
- internal movement or scheduling details that should not be exposed
- unpublished operational thresholds or internal control values

### D. Security And Access Information
Never store directly:
- passwords
- API keys
- access tokens
- system credentials
- MFA details
- exact privileged access information
- full system URLs if sensitive
- internal server or environment details not needed for pattern learning

### E. Commercially Sensitive Information
Mask or generalize when present:
- pricing
- commercial terms
- contract clauses
- vendor commercial negotiation positions
- confidential cost data
- internal savings or business case detail if sensitive

### F. Exact Client / Vendor Escalation Details
Mask where needed:
- direct ticket numbers if traceable outside intended context
- specific case references tied to sensitive incidents
- named individuals in vendor threads
- private escalation chain details

## 5. What Should Usually Be Rewritten Instead Of Masked

Some content is safer when rewritten into a sanitized pattern rather than heavily blacked out.

Prefer rewriting for:
- real emails
- incident narratives
- vendor escalation threads
- meeting notes with many named participants
- case studies containing sensitive operational timelines

Instead of preserving raw text, convert it into:
- pattern summary
- generalized example
- anonymized case note
- abstracted workflow example

## 6. Safe Levels For Repository Inclusion

Use the following three-level model.

### Level 1 — Safe Pattern Example
Safe to store in the repo.
Content is generalized and does not expose identifiable or sensitive details.

Examples:
- sanitized SOP section
- anonymized vendor question pattern
- generalized fit-gap note
- abstracted management summary

### Level 2 — Sanitized But Sensitive-Adjacent
Can be stored only if reviewed carefully.
Content has been sanitized, but the scenario may still hint at a real internal case.

Examples:
- incident summary with generalized timing and impact
- implementation issue note with masked stakeholders
- reporting problem case with source names generalized

Rule: keep only if the business pattern value is high and the residual sensitivity is low.

### Level 3 — Not Safe For Repo Storage
Do not store in `kb/examples-real/`.
Keep outside the repo or do not use.

Examples:
- raw email threads
- live incident logs
- documents containing names, contacts, IDs, or credentials
- files with contract detail, exact cost, or sensitive vendor terms
- unredacted operational data extracts
- screenshots containing internal system details or identifiable data

## 7. Recommended Redaction Method

When converting a real document into a repo-safe example, use this sequence:

1. Identify the real value of the document.
   Ask: what does the agent need to learn from it?

2. Remove or generalize all direct identifiers.

3. Remove or generalize sensitive operational and commercial details.

4. Rewrite the remaining content into a pattern-first version.

5. Add a sanitization note at the top of the file.

6. Make sure the document still teaches something useful:
- structure
- logic
- workflow
- tone
- decision pattern

## 8. Recommended Placeholder Conventions

Use consistent placeholders where needed:
- `[Department]`
- `[Role]`
- `[System / Module]`
- `[Vendor]`
- `[Date]`
- `[Time]`
- `[Ticket Reference]`
- `[User Group]`
- `[Operational Process]`

Avoid placeholders that still reveal too much, such as exact titles or unique internal labels.

## 9. Minimum Safe Standard

A document is safe enough for `kb/examples-real/` only if all of the following are true:
- it contains no direct personal contact or identity data
- it contains no credentials or security-sensitive information
- it contains no unnecessary confidential commercial detail
- it contains no raw operational data that should remain private
- the remaining scenario is generalized enough that it cannot be easily traced back to a sensitive real case
- the document still retains useful pattern value for the agent

If any of these conditions is not met, the document is not yet safe.

## 10. Preferred File Header For Sanitized Examples

Use a simple header like this:

- Document Type
- Sanitization Note
- Purpose
- Agent Use Guidance

This helps future reviewers understand why the file exists and how safe it is.

## 11. Review Rule Before Commit

Before adding any real-derived file to the repo, check:
- Does this file teach pattern or only expose detail?
- Could an outsider identify a real person, case, system, or incident from this version?
- Does the file contain any credential, commercial term, or sensitive operational reference?
- Would I be comfortable if this exact sanitized version were reviewed later as a reusable internal AI example?

If the answer is no, sanitize further or do not include it.

## 12. Final Standard

A good sanitized example should feel realistic and useful, but not traceable or sensitive.

The repository should become a high-value pattern library, not a storage place for raw confidential work materials.
