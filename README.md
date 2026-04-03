# Jersey Legislation Reading Skills

## What This Repository Is

This repository is a reusable set of Markdown-first skills for reading Jersey legislation carefully, especially on JLIB (`jerseylaw.je`). This is not an official JLIB or LDO item and is still work in progress & open to consultation.

It is designed for:

- careful human readers
- LLM workflows
- agent systems
- testing and evaluation work

The focus is operational. Each skill is meant to help a reader identify the source, control for date and version, cite properly, read a provision as structured logic, apply definitions and cross-references, use Jersey-wide reading defaults cautiously, and stop where legislation alone is not enough.

## What This Repository Is Not

This repository is not:

- legal advice
- a chatbot product
- a substitute for JLIB or other official sources
- a complete account of Jersey law
- a substitute for case law, court practice, or professional judgment

It is a framework for disciplined reading of legislation.

## Jersey And JLIB Focus

The repository is built around the source states and cautions that matter on JLIB:

- `Current`: laws in force today
- `Current point-in-time`: earlier official versions in the current collection, available back to `1 January 2019`
- `Enacted`: legislation in the form originally made, not updated
- `Pending`: not yet enacted or current, and not yet in effect
- `Archive (non-current)`: a mixed collection of versions that are not current or are not official
- `Repealed`: legislation repealed, lapsed, expired, or otherwise ceased to be in force
- `Translated`: unofficial English translations of some French laws
- `Annotated`: article-level case-linked material from the superseded revised edition

The repo also treats `UK-extended` material as a special case. JLIB places such Orders in Council in the current collection, but the official JLIB guidance says they are static and need to be interpreted with care.

## Skill Families

The current skills cover seven linked tasks:

1. orient the text on JLIB
2. find the right version and date
3. cite and link Jersey legislation properly
4. read a provision as logic
5. apply definitions and cross-references
6. apply Jersey-wide reading defaults cautiously
7. boundary-check whether legislation alone is enough

The skills are narrow on purpose. A reader or system should be able to compose them in sequence without treating any single file as a complete legal method.

## How To Use The Repository

In a normal workflow:

1. identify what source is being used and whether it is official
2. fix the target date and the right version type
3. cite the exact provision
4. turn the provision into a structured reading
5. pull in definitions and linked provisions
6. apply Jersey-wide defaults only where they are genuinely relevant
7. say plainly when legislation alone does not settle the question

This can be used as:

- a reading checklist
- a prompt library
- a review standard for AI outputs
- a test corpus for agents
- a foundation for future Jersey-focused adapters

## Repository Layout

- `docs/` contains repo-wide guidance and Jersey/JLIB maps
- `skills/` contains the reusable skill modules
- `examples/` contains worked multi-skill walkthroughs
- `tests/` contains repo-level scenario lists
- `source-notes/` contains distilled upstream notes that informed the skills

## Extensibility

The structure is intentionally stable and plain. It should be easy later to add:

- new Jersey reading skills
- domain-specific overlays
- a future `jurisdictions/` layer
- machine-readable metadata
- a future `adapters/` layer for other AI systems

The guiding rule is to preserve a small number of strong foundations and let modules change independently.
