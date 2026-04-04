---
name: locate-the-right-jlib-page
summary: Choose the right JLIB legislation entrypoint, search move, and collection before source-state analysis.
version: 0.1
depends_on: []
enables:
  - orient-the-text-on-jlib
  - find-the-right-version-and-date
---

# Purpose

Find the best JLIB legislation page or collection to start from when the reader does not yet have a stable law page in view.

# Grounding Note

This skill is an operational restatement of official JLIB public guidance, especially the JLIB Search guide, the Current laws FAQ, the Types of legislation FAQ, and the Laws as enacted FAQ.

# Use When

- the reader has a legislation question but no JLIB page yet
- the reader has only a title, topic, citation, date, or partial reference
- the reader needs to choose between whole-site search and legislation-specific search
- the reader needs to move to `Current`, `Enacted`, `Pending`, `Archive (non-current)`, `Translated`, or `Annotated`

# Do Not Use For

- classifying the source state of a JLIB page already in view
- interpreting the substance of a provision
- replacing source-state checks, date control, or citation work

# Inputs

- the research target or user question
- any known instrument title, citation, year, provision number, or instrument type
- whether the task is about present law, past law, original text, future change, translation, or annotations
- whether the reader needs legislation only or whole-site material

# Method

1. Decide whether the search is legislation-specific or whole-site.
   - Operational recommendation from the JLIB search guide: for legislation research, start from the Laws search page rather than the homepage search bar.
   - Use the homepage search bar only when the task is genuinely whole-site or the reader is not yet sure the answer will be in legislation.
2. Choose the best JLIB legislation entrypoint.
   - present law or legislation generally -> Laws search, then `Current`
   - original text or amendments not yet in force -> Laws search, then `As Enacted`
   - future or not-yet-effective legislation -> `Pending`
   - older historical or non-official material -> `Non-current`
   - unofficial English aid for older French law -> `Translated`
   - case-linking context -> `Annotated`, then return to operative text
3. If the exact title or citation is known, search it as an exact phrase in quotation marks.
4. If only topic words are known, search on the Laws page and narrow results with the available filters and sorts.
5. Use official search-guide operators only where they genuinely improve the query:
   - quotation marks for exact phrases
   - `AND`, `OR`, `NOT` for inclusion or exclusion
   - `NEAR` or `ONEAR` when proximity matters
   - `WORDS` when treating terms as synonyms helps ranking
   - `*` when a word stem or uncertain spelling is the problem
6. Use filtering and sorting options on the relevant search page where helpful, including content type, date range, subject, and A-Z or newest / oldest ordering.
7. If the reader is on the Current laws page and needs to separate primary from secondary legislation, use the page's view toggle before choosing a candidate law.
8. If the reader lands on a current law and needs an earlier official version from `1 January 2019` onward, use the current-law page's point-in-time feature.
   - On desktop, open the point-in-time timeline.
   - On mobile, use the version dropdown.
   - A specific date can also be searched from the law page.
9. If the reader needs to know about amendments made but not yet in force, check the `Enacted` collection as well as the current law.
10. If the result is `Translated` or `Annotated`, state that it is a reading aid or context aid and route back to `Current` or `Enacted` for operative reading.
11. Hand off to `01-orient-the-text-on-jlib` once a stable JLIB page has been selected.

# Output Format

- Research target:
- Best JLIB entrypoint:
- Search or browse path:
- Candidate collection:
- Candidate page or result:
- Why this starting point fits:
- Official guidance anchor:
- Safe next step:

# Common Traps

- using whole-site search when the task is plainly legislation-specific
- going straight to `Current` when the task is actually historical, enacted, pending, translated, or annotated
- forgetting that point-in-time versions are reached from the current-law page
- overlooking the Current-laws view toggle when the task depends on primary versus secondary legislation
- forgetting that future amendments may appear in `Enacted` before they appear in `Current`
- treating `Translated` or `Annotated` material as the operative text
- using advanced search syntax where a quoted title or a filter would do the job more safely
- treating `XRANK` as a normal research move rather than an advanced official feature that is usually unnecessary for ordinary legislation research

# Dependency Notes

This skill comes before orientation when no stable JLIB page is available yet. Once a page is located, hand off to `01-orient-the-text-on-jlib`.
