---
name: boundary-check-legislation-alone-or-not
summary: Decide whether Jersey legislation alone supports the answer or whether further authority or factual context is required.
version: 0.2
depends_on:
  - read-a-provision-as-logic
  - apply-definitions-and-cross-references
enables: []
---

# Purpose

Prevent false certainty by separating what the legislative text itself supports from what would require more than legislation.

# Use When

- the user wants more than a descriptive reading
- the answer may depend on case law, court interpretation, facts, remedies, or broader legal context
- the source is `Pending`, `Translated`, `Annotated`, `Archive`, `Repealed`, or UK-extended material

# Do Not Use For

- refusing a straightforward descriptive reading that the text clearly supports
- giving final legal advice
- hiding the difference between text summary and applied legal outcome

# Inputs

- outputs from earlier skills
- the user's actual question
- the source state and date posture

# Method

1. State what the text itself supports descriptively.
2. State which source category the answer depends on.
3. Check for stop rules:
   - customary law or common law not listed on Jerseylaw.je
   - court interpretation or case law
   - draft legislation on the States Assembly site
   - public-law consequences or remedies
   - fact-sensitive application to a person's situation
4. State what further authority, evidence, or context would be needed.
5. Give the safe answer posture: descriptive only, cautious partial answer, or stop.

# Output Format

- Question asked:
- What the text itself supports:
- Source category relied on:
- What legislation alone does not settle:
- Further authority or context needed:
- Safe answer posture:

# Common Traps

- turning a reading result into a court-outcome prediction
- ignoring that Jersey law includes customary law and common law outside Jerseylaw.je
- treating `Pending`, `Translated`, or `Annotated` material as if it settled the answer by itself
- assuming ambiguity disappears because the text has been paraphrased cleanly

# Dependency Notes

This is the final checking skill. It compresses the limits discovered by earlier skills into an honest answer posture. It can follow `05-apply-definitions-and-cross-references` directly when no Jersey-wide background-rule trigger remains, or follow `06-apply-non-obvious-background-rules` where that shortlist has been used.
