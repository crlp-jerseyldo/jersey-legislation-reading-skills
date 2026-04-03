---
name: cite-and-link-jersey-legislation-properly
summary: Cite Jersey legislation at provision level and link to the most relevant text without vague references.
version: 0.1
depends_on:
  - orient-the-text-on-jlib
  - find-the-right-version-and-date
enables:
  - read-a-provision-as-logic
  - apply-definitions-and-cross-references
---

# Purpose

Produce precise, provision-level citations and sensible linking habits for Jersey legislation reading work.

# Use When

- referring to a specific article, paragraph, schedule, or similar unit
- quoting or summarising legislation in notes, prompts, or outputs
- linking readers back to the relevant legislative text

# Do Not Use For

- making up citation formats unsupported by the text in view
- relying on page numbers where provision numbering exists
- masking uncertainty about the source or version

# Inputs

- identified instrument title
- provision number or structural unit
- version or status context
- stable JLIB link if available

# Method

1. Identify the smallest useful provision unit.
2. Cite the instrument title and the provision unit together.
3. Add status or date context if it matters to the task.
4. Link to the most direct available source location, not just a generic collection page.
5. If the precise provision cannot be identified, say so rather than citing vaguely.

# Output Format

- Citation:
- Link:
- Version or date note:
- Citation confidence:

# Common Traps

- citing a whole instrument when only one article matters
- using page references instead of provision references
- omitting that a citation is to pending or historical text
- linking to a general search result rather than the relevant source page

# Dependency Notes

This skill works best after orientation and version control. It supports later logic reading and cross-reference work.
