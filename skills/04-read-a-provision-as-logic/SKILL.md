---
name: read-a-provision-as-logic
summary: Convert legislative prose into structured conditions, consequences, exceptions, and dependencies.
version: 0.1
depends_on:
  - orient-the-text-on-jlib
  - find-the-right-version-and-date
  - cite-and-link-jersey-legislation-properly
enables:
  - apply-definitions-and-cross-references
  - boundary-check-legislation-alone-or-not
---

# Purpose

Turn a provision into a clear logical structure without pretending that simplification removes legal nuance.

# Use When

- a reader needs to unpack a dense article or paragraph
- the provision contains conditions, alternatives, exceptions, or consequences
- a human or AI system needs a structured reading aid

# Do Not Use For

- replacing the original text
- skipping definitions or cross-references
- claiming that a logic map settles every interpretive question

# Inputs

- provision text
- provision-level citation
- version and status context

# Method

1. Identify the main operative verb or legal effect.
2. Break the text into conditions, decision points, consequences, and exceptions.
3. Separate mandatory elements from optional or alternative limbs.
4. Note any terms that need definition lookup.
5. Note any cross-references that may alter the logic.
6. Restate the structure in plain English while preserving uncertainty where needed.

# Output Format

- Provision:
- Main rule:
- Conditions:
- Alternatives:
- Exceptions or carve-outs:
- Terms needing definition:
- Cross-references to check:

# Common Traps

- flattening several limbs into one rule
- ignoring a proviso, exception, or schedule interaction
- treating undefined terms as self-explanatory
- converting ambiguity into false certainty

# Dependency Notes

This skill should usually be followed by `05-apply-definitions-and-cross-references`. If interpretation remains uncertain after that, hand off to `07-boundary-check-legislation-alone-or-not`.
