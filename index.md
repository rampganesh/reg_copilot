---
type: index
updated: 2026-09-09
---

# Wiki Index — Regulatory Research Assistant

## Problems (status: emerging, mentions: 2, updated: 2026-09-09)

- [validating-the-right-source](wiki/problems/validating-the-right-source.md) — Validation (right source, applicable, not superseded) is harder than discovery
- [evidence-assembly-overhead](wiki/problems/evidence-assembly-overhead.md) — 5 min understanding + 15–20 min evidence assembly
- [version-and-effective-date-ambiguity](wiki/problems/version-and-effective-date-ambiguity.md) — Technically correct answers can be operationally wrong
- [terminology-fragmentation](wiki/problems/terminology-fragmentation.md) — Same concept in different document types with different wording
- [knowledge-locked-in-individuals](wiki/problems/knowledge-locked-in-individuals.md) — Experienced vs. newer analysts' knowledge gap
- [no-feedback-loop-on-answers](wiki/problems/no-feedback-loop-on-answers.md) — No mechanism to track which sources resolved questions
- [material-authority-conflation](wiki/problems/material-authority-conflation.md) — Final rules vs. reporting instructions vs. consultation documents should not appear to have same authority
- [citation-integrity-risk](wiki/problems/citation-integrity-risk.md) — Fabricated or context-stripped citations create false auditability
- [conflict-suppression-risk](wiki/problems/conflict-suppression-risk.md) — Conflicts must be exposed, not silently resolved
- [applicability-requires-firm-context](wiki/problems/applicability-requires-firm-context.md) — Applicability depends on legal entity, perimeter, permissions, regime, exposure type, date
- [interface-wording-overstates-authority](wiki/problems/interface-wording-overstates-authority.md) — "The applicable requirement is…" vs "The relevant sources indicate…"

## Open Questions (status: open, updated: 2026-09-09)

- [open-questions](open-questions.md) — Q1–Q24: cross-referencing automation, versioning, finding vs. interpreting, authority levels, auto-applicability, feedback loop, non-static corpus, success metrics, segment divergence, normal-language queries, Basel 3.1 feasibility, inter-source relationships, semantic similarity, refusal line, citation granularity, excerpt size, corpus ownership, metadata extraction, prior answers storage, bidirectional navigation, interface wording, current vs future modes, change detection, divergence axis

## Decisions (status: active, date: 2025-05-24, updated: 2026-09-06)

Per AGENTS.md L96–101, new decision pages require PM approval before writing. These were created after this ingest as proposals — hold until PM replies.

- [2025-05-24_v1-scope-uk-capital-basel31](wiki/decisions/2025-05-24_v1-scope-uk-capital-basel31.md) — UK capital reporting + Basel 3.1 as narrow first domain
- [2025-05-24_human-review-guardrails](wiki/decisions/2025-05-24_human-review-guardrails.md) — No auto-submission, no production changes, human review required
- [2025-05-24_uncertainty-as-valid-outcome](wiki/decisions/2025-05-24_uncertainty-as-valid-outcome.md) — "I couldn't find sufficient evidence" is a valid outcome

**Note**: These decision pages carry `status: active` but require direct PM approval before use. L111 records "No decision was made...on final MVP feature set..." — these capture what was stated, not formal decisions.

## Assumptions (status: untested, updated: 2026-09-09)

Per AGENTS.md L96–101, assumption status changes require PM approval. All entries below are `status: untested`.

- [assumptions](wiki/assumptions.md) — A1–A9 (6 from source 1, 3 new from source 2): time savings, provenance, uncertainty, domain viability, segment divergence, versioning feasibility, metadata extraction, feedback mechanism, bounded corpus

## Overview (updated: 2026-09-06)

- [overview](overview.md) — Living synthesis: core problem, stakeholders, scope, not-yet-decided sections, problems, open questions, held proposals

## Log (updated: 2026-09-09)

- [log](log.md) — Append-only journal: [ingest 2026-09-06 Meeting 1](log.md#2026-09-06), [decision 2026-09-09 Product Context](log.md#2026-09-09), [ingest 2026-09-09 Meeting 2](log.md#2026-09-09-ingest)

---

**Notes**

- `wiki/problems/` — 11 pages, all `status: emerging`, `mentions: 2`, `status: confirmed` requires ≥3 independent sources or ≥2 source types (AGENTS.md L83–L84)
- `wiki/decisions/` — 3 pages created, all `status: active` (PM approval pending)
- `wiki/assumptions/` — 9 entries created (A1–A6 from source 1, A7–A9 new from source 2), all `status: untested` (PM approval pending)
- `wiki/open-questions.md` — 24 questions tagged by resolution path
- `wiki/overview.md` — Living synthesis, updated on every write
- `wiki/stakeholders/` — Directory created for Stage 2 stakeholders (pending content)
- `log.md` — Append-only, grep-able prefix `## [YYYY-MM-DD] ingest|query|lint|decision | <title>`