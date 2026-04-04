# Repository Principles

## Purpose

This repository is a modular framework for reading Jersey legislation carefully. It is not a single narrative guide. Its job is to break legislation reading into stable, reusable operations that can be executed by humans, LLMs, and agents.

## Why The Skills Are Modular

Reading legislation properly requires several distinct moves:

- locate the right JLIB page or collection for the task
- identify the source and whether it is official
- fix the relevant date and version
- cite the provision precisely
- read the provision as structure and logic
- apply definitions and cross-references
- apply limited Jersey-wide defaults where needed
- stop where legislation alone does not answer the question

Keeping these separate helps in three ways:

- each step can be tested and improved on its own
- examples can show different sequences for different tasks
- future expansion does not require rewriting the whole repo

## Relationship Between Skills, Examples, Tests, And Source Notes

- `skills/` contains the reusable methods
- `examples/` shows how the methods compose in practice
- `tests/` probes whether the methods behave safely across scenarios
- `source-notes/` stores distilled upstream material that informed the methods

The layers should remain distinct. Source notes are not instructions. Examples are not authority. Tests are not explanations. Skills are the operative layer.

## Architectural Philosophy

- prefer a small number of strong foundations
- preserve a shared Jersey/JLIB taxonomy across the repo
- track source status and date as first-class reading facts
- use plain Markdown so content can move into other systems later
- keep uncertain or limited points explicit instead of smoothing them away

## Jersey-Specific Foundation

This repository assumes that serious Jersey legislation reading usually starts on JLIB and therefore depends on recognising source states such as:

- `Current`
- `Current point-in-time`
- `Enacted`
- `Pending`
- `Archive (non-current)`
- `Repealed`
- `Translated`
- `Annotated`

The architecture therefore treats locating the right JLIB page, then source classification, officiality, and date control as foundational rather than optional.

## Adding New Skill Families

Add a new skill only if it solves a distinct reading problem that cannot be handled well by:

- refining an existing skill
- adding a dependency note
- adding examples or tests

Good future candidates might include:

- commencement tracking
- amendment tracing
- subordinate-legislation chains
- offence analysis overlays

## Adding Future Jurisdictions

If the repo later expands beyond Jersey:

- keep the current Jersey layer intact
- add jurisdiction-specific overlays rather than diluting existing skills
- keep shared methods separate from local source-state rules

That allows a future `jurisdictions/` area to sit alongside the current repo without breaking existing references or naming.
