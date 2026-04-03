---
name: apply-definitions-and-cross-references
summary: Resolve Jersey definitions and cross-references in a fixed lookup order before settling meaning.
version: 0.2
depends_on:
  - read-a-provision-as-logic
enables:
  - apply-non-obvious-background-rules
  - boundary-check-legislation-alone-or-not
---

# Purpose

Work out whether the provision's meaning changes once definitions and cross-references are properly applied.

# Use When

- a provision uses defined or technical terms
- the provision says `subject to`, `for the purposes of`, `under`, or otherwise points elsewhere
- the reading cannot safely be completed from the isolated text

# Do Not Use For

- speculative expansion into remote materials with no reading payoff
- skipping straight to ordinary-language meaning when a defined meaning may govern
- assuming cross-references can be ignored because the main rule looks clear at first sight

# Inputs

- logic map from skill 04
- provision-level citation
- source or collection
- unresolved terms
- explicit internal or external cross-references

# Method

Use this lookup order:

1. Check for a local scoped definition in the same provision or part.
2. Check the instrument-wide interpretation provision.
3. Check same-instrument cross-references.
4. If the text is subordinate legislation, check the parent enactment.
5. Check defaults from the `Interpretation (Jersey) Law 1954`, especially Articles `1`, `2`, `4`, `9`, `10`, and `11`.
6. Check external enactment cross-references against the same target date as the main question.
7. Update the reading and note any unresolved dependencies that still remain.

# Output Format

- Source / collection:
- Date range or target date:
- Provision reference:
- Defined terms checked:
- Cross-references checked:
- Interpretation (Jersey) Law 1954 defaults checked:
- Reading impact:
- Remaining unresolved dependencies:

# Common Traps

- ignoring a local definition because a general interpretation article exists
- missing that subordinate legislation may inherit meaning from the parent enactment
- following an external enactment without aligning dates
- missing Article 9's default treatment of references to enactments
- stopping after one cross-reference in a longer chain

# Dependency Notes

This skill usually follows logic mapping. If important uncertainty remains after this stage, move to `06-apply-non-obvious-background-rules` or directly to `07-boundary-check-legislation-alone-or-not`.
