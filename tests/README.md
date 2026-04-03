# Repo-Level Tests

This folder contains scenario sets that test the behaviour of the repository as a whole.

## Purpose

Repo-level tests are meant to check:

- whether multiple skills compose properly
- whether uncertainty is surfaced at the right time
- whether JLIB navigation and version control are handled consistently
- whether the framework refuses or narrows overreaching requests appropriately

## Skill-Level vs Repo-Level Tests

Skill-level tests live inside each skill directory and focus on one module at a time.

Repo-level tests in this folder are broader. They test sequencing, boundaries, and failure modes across several skills together.
