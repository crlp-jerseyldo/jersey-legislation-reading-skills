# AGENTS.md

## Repo Purpose

This repository stores reusable skills, examples, tests, and source notes for reading Jersey legislation properly. It is for disciplined source-reading, not for free-form legal answering.

## Non-Goals

Do not treat this repository as:

- legal advice
- a substitute for JLIB or other official sources
- a complete statement of Jersey law
- a case-law database
- a chatbot persona layer

## Core Reading Rules

- Always identify the JLIB source state before substantive reading.
- Always track `collection`, `officiality`, and `date range or target date`.
- Always distinguish between `Current`, `Current point-in-time`, `Enacted`, `Pending`, `Archive`, `Repealed`, `Translated`, and `Annotated` where relevant.
- Always distinguish Jersey legislation from UK-extended material.
- Always prefer provision-level citation over page references.
- Always signal uncertainty honestly.
- Always say when legislation alone is not enough.

## Jersey-Specific Defaults

- `Current` and `Current point-in-time` material in the current collection is official if the page states that it is official under the `Legislation (Jersey) Law 2021`.
- JLIB's current-laws guidance says current laws and current-collection point-in-time versions are authorised for use in court, except extended UK legislation.
- `Current point-in-time` versions are available back to `1 January 2019`.
- `Enacted` material is official as originally made, but is not up to date.
- `Pending` laws are not yet enacted or current and cannot have effect until the required later steps are completed.
- `Translated` laws are unofficial reading aids and the English translations are not admissible in court; the original French law must be used where authority matters.
- `Annotated` laws are not current-law substitutes and are not kept in step with every amendment.
- `UK-extended` material in the current collection is static and must be read with care.

## Writing Standards

- Use calm, plain English.
- Prefer short operational sections over essays.
- Do not overstate legal authority.
- Do not fabricate quotations, rules, or examples.
- Do not hide limits behind vague wording.
- Write so a careful human or LLM can execute the method.

## File Conventions

- Keep repo content in Markdown unless there is a strong reason otherwise.
- Each skill directory contains `SKILL.md`, `examples.md`, and `tests.md`.
- Preserve the ordered skill naming pattern `NN-skill-name`.
- Preserve the YAML front matter keys: `name`, `summary`, `version`, `depends_on`, `enables`.
- Keep output formats stable and field-based where possible.

## Skill Design Rules

- One skill should solve one reading problem.
- A skill should state when to use it and when not to use it.
- A skill should expose the source and date facts needed for safe reading.
- A skill should be executable without turning into a legal treatise.
- If content grows beyond one reading task, split the skill rather than expanding it indefinitely.

## Maintenance Rules

- Keep the Jersey/JLIB taxonomy consistent across docs, skills, examples, and tests.
- If official JLIB categories or warnings change, update repo-wide guidance first, then skills.
- Keep source notes upstream and clearly distinct from operative skill guidance.
- Keep examples schematic unless backed by a checked source.
- Do not blur descriptive reading into applied legal advice.

## Extension Rules

When extending the repo:

- add new skills as sibling modules
- keep jurisdiction-specific additions isolated and explicit
- do not bury important rules in examples only
- prefer stable terminology that can survive later renaming
- preserve a future path for `jurisdictions/` and `adapters/`

If an edit would make the repo sound more certain than the sources justify, revise it before merging.
