---
name: read-a-provision-as-logic
summary: Turn Jersey legislative prose into a structured reading of rules, limbs, exceptions, and dependencies.
version: 0.2
depends_on:
  - orient-the-text-on-jlib
  - find-the-right-version-and-date
  - cite-and-link-jersey-legislation-properly
enables:
  - apply-definitions-and-cross-references
  - boundary-check-legislation-alone-or-not
---

# Purpose

Restate a provision as structured logic without pretending that the structure itself resolves every interpretive issue.

# Use When

- a provision is dense or nested
- the text contains multiple limbs, alternatives, or exceptions
- a human or LLM needs a more operational reading aid

# Do Not Use For

- replacing the original text
- skipping definitions, cross-references, or source-state cautions
- turning a reading aid into a final legal conclusion

# Inputs

- provision text
- provision-level citation
- source or collection
- date range or target date

# Method

1. Read the whole provision before breaking it apart.
2. Identify the main operative rule or consequence.
3. Separate conditions, alternatives, exceptions, and consequences.
4. Track list connectors and nesting, especially where `and` and `or` operate at different levels.
5. Note whether a term is being used in ordinary language, by `means`, by `includes`, or by cross-reference.
6. Apply singular/plural and "always speaking" ideas cautiously as reading aids, not as automatic answers.
7. Record unresolved defined terms, cross-references, or source-state cautions for later skills.

# Output Format

- Source / collection:
- Officiality:
- Date range or target date:
- Provision reference:
- Main rule:
- Conditions and limbs:
- Exceptions or carve-outs:
- Definition cues:
- Cross-references to check:
- Special caution:

# Common Traps

- flattening several nested limbs into one rule
- losing the force of `and` or `or`
- ignoring a proviso, schedule interaction, or parenthetical definition cue
- treating `includes` as if it always meant `means`
- using singular or present-tense drafting to imply a narrower result than the drafting method supports

# Dependency Notes

This skill should usually hand off to `05-apply-definitions-and-cross-references` before any confident summary is given.
