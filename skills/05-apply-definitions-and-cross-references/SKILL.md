---
name: apply-definitions-and-cross-references
summary: Resolve defined terms and follow cross-references that may change how a provision should be read.
version: 0.1
depends_on:
  - read-a-provision-as-logic
enables:
  - apply-non-obvious-background-rules
  - boundary-check-legislation-alone-or-not
---

# Purpose

Check whether the meaning of a provision depends on definitions or cross-references that are not obvious from the text in isolation.

# Use When

- the provision uses capitalised, technical, or apparently loaded terms
- the provision explicitly cross-refers to another article, schedule, law, or external text
- the logic map cannot be completed safely without more text

# Do Not Use For

- speculative expansion into every remote cross-reference
- assuming a common-language meaning where a definition may govern
- treating a cross-reference as irrelevant without checking it

# Inputs

- logic map of the provision
- list of unresolved terms
- list of internal or external cross-references

# Method

1. List the terms that may be defined.
2. Check for local definitions first, then general definitions in the same instrument.
3. List explicit cross-references and classify them as internal or external.
4. Check whether each definition or cross-reference changes scope, threshold, procedure, or exception structure.
5. Update the reading summary to reflect those dependencies.
6. If the chain becomes too long or uncertain, say so rather than guessing.

# Output Format

- Defined terms checked:
- Definitions affecting meaning:
- Cross-references checked:
- Reading impact:
- Remaining unresolved dependencies:

# Common Traps

- ignoring an interpretation section
- following only one cross-reference in a chain
- assuming an external reference says the same thing now as at the target date
- failing to mark unresolved dependencies

# Dependency Notes

This skill is usually applied after the initial logic map. If unresolved issues remain after this stage, boundary-checking is often the next step.
