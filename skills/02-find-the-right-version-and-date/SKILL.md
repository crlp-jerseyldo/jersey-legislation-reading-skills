---
name: find-the-right-version-and-date
summary: Anchor the reading task to the correct version and date before drawing conclusions.
version: 0.1
depends_on:
  - orient-the-text-on-jlib
enables:
  - cite-and-link-jersey-legislation-properly
  - read-a-provision-as-logic
  - boundary-check-legislation-alone-or-not
---

# Purpose

Determine which version of the legislative text is relevant and what date the reading exercise is anchored to.

# Use When

- the question is about the law now
- the question is about the law at an earlier date
- the material may be pending, historical, or as-enacted
- a consolidated view may differ from the original enacted text

# Do Not Use For

- deciding substantive meaning without first fixing the version issue
- tracing every amendment in detail
- replacing a full commencement or amendment analysis where one is needed

# Inputs

- oriented JLIB text
- the user’s target question
- any date mentioned by the user
- any visible version, status, or historical indicators

# Method

1. Extract the legal question being asked: now, then, pending change, or original text.
2. Identify the target date, or state that it is missing.
3. Match the task to the likely version type: current consolidated, non-current, pending, or as-enacted.
4. State whether the available text appears to fit that target.
5. If the date or version remains uncertain, stop and say what is missing.
6. Only then move to substantive reading.

# Output Format

- Question type:
- Target date:
- Needed version type:
- Available text appears to be:
- Fit for task:
- Next action:

# Common Traps

- answering a historical question from a current text
- treating pending material as current law
- assuming consolidated text answers an as-enacted question
- failing to surface that no target date was provided

# Dependency Notes

This skill depends on basic orientation first. It often feeds directly into citation and substantive reading.
