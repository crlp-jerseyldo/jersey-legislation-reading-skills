---
name: orient-the-text-on-jlib
summary: Identify the exact JLIB source state, officiality, date range, and caution before reading substance.
version: 0.2
depends_on: []
enables:
  - find-the-right-version-and-date
  - cite-and-link-jersey-legislation-properly
  - read-a-provision-as-logic
---

# Purpose

Work out exactly what text the reader is looking at on JLIB before any substantive reading begins.

# Use When

- a JLIB page, link, screenshot, PDF, or extract is provided
- the reader may be confusing `Current`, `Enacted`, `Pending`, `Archive`, `Repealed`, `Translated`, or `Annotated`
- the text may involve UK-extended material

# Do Not Use For

- choosing the final target version for the legal question
- interpreting the provision in detail
- deciding whether legislation alone answers the question

# Inputs

- JLIB page, link, PDF, screenshot, or copied extract
- page title
- collection label or breadcrumb
- officiality statement if visible
- date range shown on the page
- provision heading or structural unit in view

# Method

1. Record the instrument title.
2. Record the instrument type: Law, Regulations, Order, Act, Bye-law, Rule, or UK-extended Order in Council material.
3. Record the source or collection: `Current`, `Current point-in-time`, `Enacted`, `Pending`, `Archive`, `Repealed`, `Translated`, or `Annotated`.
4. Record whether the page presents an official version, an unofficial translation, or another non-official source state.
5. Record the date range shown on the page, such as `Showing the law from 11 January 2024 to Current`.
6. Record whether the material is Jersey legislation or UK-extended material.
7. Record the provision reference or structural unit currently in view.
8. State any immediate special caution before substantive reading starts.

# Output Format

- Instrument:
- Instrument type:
- Source / collection:
- Officiality:
- Date range shown on page:
- Jersey or UK-extended:
- Provision reference in view:
- Special caution:
- Safe next step:

# Common Traps

- treating every page in the current collection as the same kind of source
- missing that a page is `Pending`, `Enacted`, `Repealed`, `Translated`, or `Annotated`
- treating a translation as authoritative text
- missing that UK-extended material in the current collection is a special case
- starting interpretation before recording the page's own date range

# Dependency Notes

This skill should normally come first. After orientation, hand off to `02-find-the-right-version-and-date`.
