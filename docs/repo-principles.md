# Repository Principles

## Purpose

This repository is built as a framework for careful legislation reading, not as a monolithic guide. The aim is to make small, durable components that can be reused across human workflows, LLM prompts, and agent systems.

## Why The Skills Are Modular

Legislation reading is not one task. A reader may need to:

- orient the text first
- control for version and date
- cite accurately
- unpack logic
- trace definitions
- check background rules
- decide whether to stop and escalate

Keeping these as separate skills makes it easier to combine them in different sequences, revise one part without disturbing others, and test failures more clearly.

## Relationship Between Skills, Examples, Tests, And Source Notes

- `skills/` contains reusable operating instructions
- `examples/` shows how several skills can be used together
- `tests/` checks behaviour across broader repo-level scenarios
- `source-notes/` stores upstream reference material and distilled notes that inform the framework

The repository should treat these as different layers. Source notes inform skills, but they are not themselves the skill instructions. Examples demonstrate usage, but they are not the rule source. Tests probe behaviour, but they are not explanatory essays.

## Design Philosophy

- keep the number of top-level concepts small
- prefer stable names and predictable structure
- make room for future metadata without forcing it now
- keep content plain enough to port into other systems later
- separate high-confidence guidance from areas where uncertainty must be flagged

## Adding New Skill Families

New skill families should be added only when they solve a distinct reading problem. If a new topic can be expressed as a dependency note or a worked example, prefer that over creating a broad catch-all skill.

Possible future families might cover:

- amendment-tracing
- commencement analysis
- subordinate legislation reading
- comparative Jersey and UK extension issues

## Adding Future Jurisdictions

If the repository later expands beyond Jersey, do not dilute the Jersey-specific modules. Instead:

- preserve the current Jersey skill set as one stable layer
- add jurisdiction-specific overlays in a dedicated top-level area
- keep shared reading methods separate from local legal system notes

This allows common methods and local variations to coexist without confusion.
