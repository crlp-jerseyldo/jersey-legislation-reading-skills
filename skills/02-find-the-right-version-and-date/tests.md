# Tests

## Prompt Set

1. A user asks what the law is now, but the only text provided is labelled non-current. What should happen?
2. A user asks for the law as enacted. The text available is a consolidated current version. What mismatch should be identified?
3. A user asks whether a pending amendment already applies. What version-and-date warning is required?
4. No target date is given, but the question could be historical. How should the output handle this?
5. A user provides a date and a current-looking extract. What should be checked before proceeding?
6. A present-law question is paired with translated material only. What should be said about fitness for task?
7. A historical question is asked about UK-extended material. What extra caution should be flagged?
