---
name: find-the-right-version-and-date
summary: Match the question to the correct Jersey source state and date before drawing conclusions.
version: 0.2
depends_on:
  - orient-the-text-on-jlib
enables:
  - cite-and-link-jersey-legislation-properly
  - read-a-provision-as-logic
  - boundary-check-legislation-alone-or-not
---

# Purpose

Determine which source state and date the reading task actually requires.

# Use When

- the question is about the law now
- the question is about the law at a past date
- the question is about the original enacted text
- the material may be `Pending`, `Archive`, or otherwise not fit for the task
- the user is asking about a future or proposed change

# Do Not Use For

- detailed amendment tracing
- commencement analysis beyond the immediate source-state problem
- substantive interpretation before the source and date are fixed

# Inputs

- orientation output from skill 01
- the user's question
- any date stated by the user
- any version or date range shown on the source page

# Method

1. State the question type: present law, past law, original text, or future/proposed change.
2. State the target date if given. If no date is given and the question could be historical, say that the target date is missing.
3. Match the question to the source state:
   - present law -> `Current`
   - past law from `1 January 2019` onward -> `Current point-in-time`
   - original text -> `Enacted`
   - older or non-official historical work -> `Archive`, with limitation stated
   - future or proposed change -> `Pending` or a States Assembly draft proposition
4. Check whether the available source matches the needed source state.
5. If the available source does not match, stop and state the mismatch plainly.
6. Record the safe next step before any substantive reading.

# Output Format

- Question type:
- Target date:
- Needed source state:
- Available source state:
- Fit for task:
- Version / date caution:
- Safe next step:

# Common Traps

- answering a present-law question from `Enacted`, `Archive`, or `Repealed` material
- treating `Pending` text as current law
- forgetting that `Enacted` text is original text, not updated law
- forgetting that `Current point-in-time` versions are available only from `1 January 2019`
- confusing a States Assembly proposition with legislation already on JLIB

# Dependency Notes

This skill depends on correct orientation first. After the source state and date are fixed, move to `03-cite-and-link-jersey-legislation-properly`.
