---
name: orient-the-text-on-jlib
summary: Identify what kind of JLIB text is being viewed before doing substantive reading.
version: 0.1
depends_on: []
enables:
  - find-the-right-version-and-date
  - cite-and-link-jersey-legislation-properly
  - read-a-provision-as-logic
---

# Purpose

Work out what the reader is actually looking at on JLIB before any substantive interpretation begins.

# Use When

- a JLIB page or extract has been provided
- the reader is not yet sure what collection or status the text comes from
- there is a risk of confusing current, pending, historical, translated, or annotated material

# Do Not Use For

- deciding the correct date-specific version on its own
- interpreting the legal effect of the provision in detail
- resolving disputes about meaning

# Inputs

- JLIB page, extract, link, screenshot, or copied text
- visible title, collection label, status indicators, and structural headings

# Method

1. Identify the instrument title and instrument family if visible.
2. Identify the collection or status marker shown on JLIB.
3. Note whether the text appears current, pending, non-current, translated, annotated, or otherwise special.
4. Identify the structural unit being viewed: article, paragraph, schedule, note, or other.
5. Record any immediate caution flags, such as historical status, translation, annotation, or UK-extended context.
6. Stop with an orientation summary before substantive reading.

# Output Format

Use a short orientation block:

- Instrument:
- Instrument family:
- JLIB collection or status:
- Structural unit in view:
- Special caution:
- Safe next step:

# Common Traps

- starting interpretation before identifying the collection
- treating annotation or translation as if it were always the operative text
- failing to notice that a page is historical or pending
- citing the whole page when only one provision matters

# Dependency Notes

This skill should usually come before all other reading skills. If date or version matters, hand off next to `02-find-the-right-version-and-date`.
