---
name: boundary-check-legislation-alone-or-not
summary: Decide whether legislation alone is enough or whether further authority or context is needed.
version: 0.1
depends_on:
  - read-a-provision-as-logic
  - apply-definitions-and-cross-references
  - apply-non-obvious-background-rules
enables: []
---

# Purpose

Prevent false certainty by checking whether the reading task can responsibly be answered from legislation alone.

# Use When

- the user wants a legal conclusion, not just a reading summary
- interpretation turns on ambiguity, scope, or disputed application
- case law, court interpretation, facts, guidance, or procedural context may matter

# Do Not Use For

- pretending legislation alone always answers the question
- refusing simple descriptive tasks that the text clearly supports
- giving final legal advice

# Inputs

- reading output from earlier skills
- unresolved ambiguities
- the user’s actual question

# Method

1. Separate descriptive reading from applied legal conclusion.
2. Ask whether the text is clear enough for the exact question.
3. Identify missing elements such as case law, factual context, court practice, official guidance, or commencement detail.
4. State whether legislation alone is enough, probably enough, or not enough.
5. If not enough, stop and explain the boundary plainly.

# Output Format

- Question asked:
- What legislation alone can support:
- What remains uncertain:
- Extra material likely needed:
- Safe answer posture:

# Common Traps

- turning text reading into legal advice
- hiding that interpretation may depend on case law or facts
- assuming the absence of explicit ambiguity means no uncertainty exists
- refusing everything instead of distinguishing low-risk descriptive answers from high-risk conclusions

# Dependency Notes

This is usually the final checking skill in a workflow. It should compress the limits identified by earlier skills into a clear answer posture.
