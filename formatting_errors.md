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

## 2026-09-14 - stakeholders activation
- Schema defines stakeholder pages only as "positions + evidence" without a mandated frontmatter or section template; I used type/role/updated frontmatter and Positions/Evidence/Related sections. Confirm convention.
- Role names normalized to one page per distinct voice; "Reporting Manager" and "Regulatory Reporting Manager" treated as one role (regulatory-reporting-manager) per earlier formatting note.
- analyst-1/analyst-2 slugs chosen without bracketed descriptors (e.g. analyst-2.md not analyst-2-accuracy-focused.md) though page titles carry descriptors.

## 2025-06-10 - ingest of 2025_06_10_research_docversions.md
- Source uses URL-style external citations ([1]-[4], bankofengland.co.uk / regulationtomorrow.com) rather than line numbers; citations in wiki use L<n> for this file. Confirm whether external URLs are an acceptable citation form for research sources or should be normalized.
- Source has an internal inconsistency: [3] is a July 2025 consultation link (market risk framework) but the text does not cite it inline; body text cites [1,2] and [4] only. Filed as-is; PM may want to clarify reference [3].

## 2025-06-14 - ingest of 2025_06_14_meeting_latedocuments.md
- Editor slip: no-feedback-loop.md status briefly set to confirmed unintentionally; reverted to emerging per approved plan. Confirmation is now formally proposed (meets >=3 sources / >=2 source types).
- Four meeting participants (AI/ML Engineer, Data Engineer, AI Governance/Model Risk rep, Technology Architecture rep) have no stakeholder pages per PM instruction - logged only. Watch for their voices in future sources.

## 2025-06-18 - ingest of analyst interviews
- Path typo during A2 status edit briefly created a stray DS\ directory under reg_copilot; deleted immediately. No content affected.
- Personas: schema has no personas page template; used type/name/updated frontmatter with Job to be done / Behaviour / Value proposition / Non-delegable sections. Confirm convention.
- Newer-analyst persona is built entirely from second-hand accounts plus one kickoff line; consider a direct newer-analyst interview before relying on it for design.
- Severity of no-feedback-loop raised medium->high alongside PM-approved confirmation (impact-tracing evidence justifies it) - confirm severity change was in scope.
