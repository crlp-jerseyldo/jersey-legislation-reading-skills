---
name: cite-and-link-jersey-legislation-properly
summary: Cite Jersey legislation at provision level with source-state and date information that matches the task.
version: 0.2
depends_on:
  - orient-the-text-on-jlib
  - find-the-right-version-and-date
enables:
  - read-a-provision-as-logic
  - apply-definitions-and-cross-references
---

# Purpose

Produce precise provision-level citations and links that preserve the source status and date context of the text being used.

# Use When

- referring to a specific provision
- quoting or summarising legislation
- linking a reader back to JLIB
- recording authority for a reading output

# Do Not Use For

- vague whole-document citation where a provision can be identified
- page-number citation as a first choice
- hiding that the source is `Pending`, `Enacted`, `Archive`, `Translated`, `Annotated`, or `UK-extended`

# Inputs

- instrument title
- provision reference
- source or collection
- officiality status
- date range or target date
- direct JLIB link if available

# Method

1. Identify the smallest useful provision unit.
2. Cite the instrument title and provision reference together.
3. Add the source status.
4. Add the date range shown on the page, or the target date if the task is date-anchored.
5. Add a direct JLIB link if available.
6. If a precise provision cannot be identified, say so. Use a page-based reference only as a fallback.

# Output Format

- Instrument title:
- Provision reference:
- Source / collection:
- Officiality:
- Date range or target date:
- Direct link:
- Citation note:

# Common Traps

- citing only the instrument when one article or paragraph is doing the work
- omitting that the source is not straightforward current official Jersey legislation
- treating a PDF page number as the main citation
- failing to distinguish `Current` from `Current point-in-time`
- linking only to a search page when a direct page is available

# Dependency Notes

This skill follows source and date control. It prepares a stable reference for logic reading and cross-reference work.
