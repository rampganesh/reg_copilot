# Formatting errors / observations

## 2025-05-24 — ingest of 2025_05_24_meeting_kickoff.md
- index.md (whole file): file existed but contained only a UTF-8 BOM and no content; overwritten with new catalog. PM may want to check no prior content was intended.
- log.md (line 1): same situation — BOM-only, no entries; overwritten with new journal.
- wiki/problems/*.md: frontmatter uses the optional `cluster` field only on the two `cluster: evidence-workflow` pages; other pages deliberately left unclustered. Confirm whether experience-dependency should join a cluster.
- overview.md: uses wiki-relative markdown links (e.g. `problems/evidence-assembly-time-cost`) rather than bare `[[wikilinks]]`; problems pages use `[[...]]` style. Schema does not mandate a link style — PM to pick one convention.
- Source line citations use `L<n>` format referencing the raw file's line numbers, not yet defined in schema — confirm convention.

## 2025-05-26 - ingest of 2025_05_26_meeting_followup.md
- Role-name variations across sources assumed to be same roles: "Reporting Manager" vs "Regulatory Reporting Manager"; "Reporting Change SME" vs "Regulatory Change/Reporting SME". PM to confirm or standardise.
- wiki/overview.md rewritten wholesale via Set-Content after an exact-text edit failed (likely encoding/whitespace mismatch); previous Meeting 1 content was fully superseded, nothing lost, but link style changed from wikilinks to plain relative paths in the problem map to match schema ambiguity noted 2025-05-24.
- Problem pages now mix a "### From Meeting 2" subsection heading style for appended evidence - confirm this convention is acceptable vs. flat bullet lists.

## 2025-06-04 - ingest of 2025_06_04_digest_clarifications.md
- Source file renamed by PM from 2025_06_04_email_clarifications.md to 2025_06_04_digest_clarifications.md; wiki references updated (index, log). Confirm old filename references elsewhere are not needed.
- Source is a table-format digest with row references (row 1-7) used in citations instead of L<n> line numbers - confirm this citation style is acceptable.
- Decision pages list decider as "PM (approving consolidated stakeholder responses from the email digest)" - confirm this attribution wording.
- Problem-page frontmatter for authority-overstatement-risk lacked a cluster field while others in evidence-workflow have it (observed, left as-is).
