# Jersey Legislation Reading Skills

## What This Repository Is

This repository is a modular set of reusable skills for reading Jersey legislation carefully and consistently. It is designed for human readers, LLM workflows, and agent systems that need a practical framework for:

- orienting a text on JLIB before reading it
- identifying the right version and date
- citing Jersey legislation precisely
- reading provisions as structured logic
- applying definitions and cross-references
- spotting background rules that may affect reading
- deciding when legislation alone is not enough

The repository is Markdown-first, deliberately plain, and structured so parts can be reused, renamed, split, or replaced later.

## What This Repository Is Not

This repository is not:

- legal advice
- a chatbot product
- a definitive textbook on Jersey law
- a substitute for official sources, legal research, or professional judgment

It is a framework for disciplined reading.

## Skill Families

The current skill set is organised around seven core reading tasks:

1. JLIB orientation
2. version and date control
3. citation and linking
4. provision-to-logic reading
5. definitions and cross-references
6. restrained background-rule checking
7. boundary checking on whether legislation alone is enough

Each skill is intentionally narrow and composable. Worked examples show how multiple skills can be used together, and tests provide concise prompts for checking whether the skills behave as intended.

## How To Use This Repository

In practice, a careful reader or AI system would normally:

1. identify what text is being looked at and in which JLIB collection it sits
2. confirm whether the version and date are the right ones for the task
3. cite the relevant provision precisely
4. unpack the provision into operative logic
5. resolve definitions and cross-references
6. check whether background rules or external context may matter
7. stop and signal limits where the legislation alone may not answer the question

The repo can be used as:

- a reading checklist for humans
- a modular prompt source for LLM systems
- a test corpus for agent behaviour
- a starter framework for larger Jersey-focused legal reading tools

## Repository Layout

- `docs/` contains repo-level guidance and system maps
- `skills/` contains the reusable skill modules
- `examples/` contains multi-skill walkthroughs
- `tests/` contains repo-level scenario sets
- `source-notes/` contains upstream reference notes that inform the skills

## Future Extensibility

The structure is designed so future additions can be made without reorganising the whole repository. Likely expansions include:

- additional Jersey skill modules
- jurisdiction overlays or a future `jurisdictions/` folder
- machine-readable metadata alongside Markdown
- adapters for other AI systems in a future `adapters/` folder
- deeper example sets and more formal test suites

The main design rule is to keep foundations stable while letting modules evolve independently.
