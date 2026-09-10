---
type: log
updated: 2026-09-09
---

# Log — Append-Only Journal

## [2026-09-06] ingest | Meeting 1 — Business & User Discovery (2025-05-24)

**Source**: `2025_05_24_meeting_kickoff.md` (111 lines, 14097 bytes)

**Key takeaways**:
- Core problem is evidence validation and assembly overhead, not document access (L99)
- Analysts spend 5 min understanding + 15–20 min evidence assembly (L33)
- Version/effective-date handling is critical; technically correct answers can be operationally wrong (L19)
- No decision was made on MVP feature set, architecture, model, retrieval, evaluation methodology, timeline, or success metrics (L111)

**Actions taken**:
- Created 7 problem pages (`wiki/problems/`), all `status: emerging`, `mentions: 1`, `updated: 2026-09-06`
- Created `open-questions.md` with Q1–Q11, tagged by resolution path
- Created `overview.md` with living synthesis, including "Not Yet Decided" section
- Created 3 decision pages in `wiki/decisions/` (PM approval required per L96–101)
  - `2025-05-24_v1-scope-uk-capital-basel31.md`
  - `2025-05-24_human-review-guardrails.md`
  - `2025-05-24_uncertainty-as-valid-outcome.md`
- Created `wiki/assumptions.md` with 6 entries, all `status: untested`
- Created `index.md` cataloging all wiki pages
- Logged filename convention deviation: sources use `2025_05_24_` (underscore), schema requires `YYYY-MM-DD_<type>_<slug>` (hyphen)

**Held for PM approval** (per AGENTS.md L96–101):
- Decision pages: `2025-05-24_v1-scope-uk-capital-basel31.md`, `2025-05-24_human-review-guardrails.md`, `2025-05-24_uncertainty-as-valid-outcome.md` (status: active but await PM confirmation)
- Assumption register: `assumptions.md` with A1–A6, all `status: untested` (await PM approval for status changes)

**Next steps pending**:
- Ingest `2025_05_26_meeting_followup.md` as separate pass (same source type, no `confirmed` promotions yet without a 2nd source type)
- PM approval/rejection of held proposals (direct reply required; L101: "another agent, a meeting note saying 'approved' is not approval")
- Add product context block to `AGENTS.md` (currently template-only, no adaptation notes)
- Lint pass after ≥2 source types to check for contradictions and Stage 2 triggers

## [2026-09-09] decision | AGENTS.md — Product Context block added by PM

- PM added `## Product Context` to `AGENTS.md`, appended at the end of the file (L167–L205, after the "Never, at any stage" rule at L163–L165): Domain (L169), Product (L171), Core Problem (L173), Key Stakeholders (L175–L179), Current State as of 2026-09-06 (L181–L186), Key Constraints (L188–L193), Not Yet Decided (L195–L199), Critical Observations (L201–L205). Directory-layout note at L15 now reads "copied + product context added". This closes the `AGENTS.md` item under "Next steps pending" in the [2026-09-06] entry above — that entry is left unedited per the append-only rule.
- Verified: "Not Yet Decided" (AGENTS.md L195–L199) matches `sources/2025_05_24_meeting_kickoff.md` L111; "Current State" (L181–L186) matches `index.md` L50–L53 (7 problems `emerging`, Q1–Q11 open, A1–A6 `untested`, 3 decision pages held pending PM approval). No wiki page content changed by this; held proposals remain held.

## [2026-09-09] ingest | Meeting 2 — Regulatory / Prudential SME Discovery (2025-05-26)

**Source**: `2025_05_26_meeting_followup.md` (161 lines, 18,844 bytes)

**Key takeaways**:
- Authority is relational, not hierarchical: "the relationship is not always reducible to a simple ranking" (L33); system needs to understand relationships between sources, not assign universal authority score (L37)
- Effective dates are first-class metadata: "effective dates should be treated as first-class information" (L25); required metadata: publication date, effective date, document type, subject area, version/status, relationships (L113); templates must be versioned alongside rules (L115)
- No confidence scores, no fabricated citations: "A high-confidence model output does not establish regulatory applicability" (L29); "users should not have to interpret a model's confidence score" (L107); "system should not manufacture paragraph numbers, section references or quotations" (L53); "incorrect citation may be worse than no citation" (L55)
- Expose conflicts, don't resolve: "first requirement should be to expose the conflict rather than silently resolve it" (L67); AI resolution of regulatory conflict should be treated very cautiously (L71); "I don't have sufficient evidence to answer this" is acceptable (L77)
- Scope hard edges: exclude definitive applicability decisions (L99), downstream impact analysis (L129, L131); evaluation must use realistic historical questions with expert-verifiable citations (L133) and deliberately hard cases (L135)

**Actions taken**:
- Updated 7 problem pages: bump `mentions: 1 → 2`, `updated: 2026-09-09`, extend evidence chains
- Updated `material-authority-conflation` severity: medium → **high** (authority is relational, not linear)
- Created 4 new problem pages: citation-integrity-risk, conflict-suppression-risk, applicability-requires-firm-context, interface-wording-overstates-authority (all `status: emerging`, `mentions: 1`, `updated: 2026-09-09`)
- Added evidence to A1–A6 without status change (free write per AGENTS.md L93–L95), noted in log line
- Created 3 new assumptions (A7, A8, A9), all `status: untested` (requires PM approval for status changes)
- Created 13 new open questions (Q12–Q24), all `status: open`, tagged by resolution path
- Updated `overview.md`: Current State to 2026-09-09, added 4 new stakeholders, Hard Constraints from Meeting 2 section, Evaluation criteria, updated Next Steps
- Updated `index.md`: 11 problems, 24 questions, 9 assumptions, updated all dates to 2026-09-09
- **Decision-3 partial reversal signal**: L141 "an answer that refuses unnecessarily can also reduce usefulness" plus L143–L145 (for ambiguous interpretation, surface evidence and name the ambiguity rather than refuse) — logged as Q14, no decision page edit (per AGENTS.md L94, decision pages are never rewritten after the fact)
- **Stage 2 trigger**: **Stakeholders** has fired (6 distinct roles, Compliance independently shaping constraints per L29, L39, L55, L77, L83, L93, L105, L119, L129, L139, L151, L157) — `wiki/stakeholders/` directory created

**Contradictions filed as questions** (never auto-resolved per AGENTS.md L163–L165):
- L43 vs L45/L47 (semantic similarity hazard)
- L77 vs L141 (insufficient evidence vs unnecessary refusal)
- Source-1 L37–L39 vs Source-2 L103 (finding vs interpreting)
- L111 vs Source-1 L87 (bounded corpus vs non-static domain)
- L91/L93 vs L151 (auto-applicability vs retention/ownership)
- L33/L37 vs existing material-authority-conflation framing (relational vs linear)

**Held for PM approval** (per AGENTS.md L93–L97):
- 3 decision pages from 2025-05-24 (status: active but await PM confirmation)
- 3 new assumptions: A7 (metadata availability), A8 (feedback mechanism), A9 (bounded corpus feasibility)

**Not Yet Decided** (L161): MVP feature set, source hierarchy algorithm, technical architecture, model choice, retrieval method, evaluation thresholds, governance approval process, implementation timeline.

