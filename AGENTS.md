# AGENTS.md

## Repo Purpose

This repository exists to store reusable skills, examples, tests, and source notes for reading Jersey legislation properly. It is meant to support careful human readers and AI systems that need a disciplined reading framework.

## Non-Goals

Do not treat this repository as:

- legal advice
- a substitute for official legal sources
- a free-form legal chatbot
- a place for broad legal essays detached from practical reading tasks

## Core Operating Rules

- Always distinguish, where relevant, between official, non-official, current, non-current, pending, as-enacted, and consolidated material.
- Always anchor reading to the relevant date when version questions matter.
- Always prefer provision-level citation over vague page or document references.
- Always signal uncertainty honestly.
- Always say when legislation alone may be insufficient.
- Keep skills narrow, composable, and reusable.

## Writing Standards

- Use calm, plain English.
- Prefer short operational sections over long theory.
- Do not overstate authority.
- Do not fabricate legal detail, quotations, or precise propositions.
- Avoid unexplained jargon.
- Write so both humans and AI systems can execute the guidance.

## File Conventions

- Keep primary content in Markdown unless there is a strong reason otherwise.
- Give each skill its own directory containing `SKILL.md`, `examples.md`, and `tests.md`.
- Use stable, ordered, slug-style skill directory names such as `01-name-of-skill`.
- Use concise headings with predictable section names.
- When adding metadata, prefer lightweight front matter that can later be extended.

## Skill Design Rules

- A skill should solve one reading problem well.
- A skill should declare what it depends on and what it enables.
- A skill should be executable as a checklist or method, not a long essay.
- A skill should separate method from examples and tests.
- If content grows large, split rather than overloading an existing skill.

## Maintenance Rules

- Preserve modularity when adding new material.
- Avoid hard-coding assumptions that block future jurisdictions or adapters.
- Update internal references when renaming files or skills.
- Keep examples schematic unless a source-backed worked example is intentionally added.
- Keep source notes clearly separate from normative instructions.

## Extension Rules

When extending the repo:

- add new skills as sibling modules, not as large appendices to existing ones
- add new jurisdictions or overlays in their own future top-level area
- keep repo-level guidance in `docs/`
- keep cross-skill dependencies explicit but light
- preserve backward-readable naming where possible

If a change would blur the boundary between reading guidance and legal conclusion, revise it before merging.
