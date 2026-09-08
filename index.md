---
type: index
updated: 2026-09-06
---

# Wiki Index — Regulatory Research Assistant

## Problems (status: emerging, mentions: 1, updated: 2026-09-06)

- [validating-the-right-source](wiki/problems/validating-the-right-source.md) — Validation (right source, applicable, not superseded) is harder than discovery
- [evidence-assembly-overhead](wiki/problems/evidence-assembly-overhead.md) — 5 min understanding + 15–20 min evidence assembly
- [version-and-effective-date-ambiguity](wiki/problems/version-and-effective-date-ambiguity.md) — Technically correct answers can be operationally wrong
- [terminology-fragmentation](wiki/problems/terminology-fragmentation.md) — Same concept in different document types with different wording
- [knowledge-locked-in-individuals](wiki/problems/knowledge-locked-in-individuals.md) — Experienced vs. newer analysts' knowledge gap
- [no-feedback-loop-on-answers](wiki/problems/no-feedback-loop-on-answers.md) — No mechanism to track which sources resolved questions
- [material-authority-conflation](wiki/problems/material-authority-conflation.md) — Final rules vs. reporting instructions vs. consultation documents should not appear to have same authority

## Open Questions (status: open, updated: 2026-09-06)

- [open-questions](open-questions.md) — Q1–Q11: cross-referencing automation, versioning, finding vs. interpreting, authority levels, auto-applicability, feedback loop, non-static corpus, success metrics, segment divergence, normal-language queries, Basel 3.1 feasibility

## Decisions (status: active, date: 2025-05-24, updated: 2026-09-06)

Per AGENTS.md L96–101, new decision pages require PM approval before writing. These were created after this ingest as proposals — hold until PM replies.

- [2025-05-24_v1-scope-uk-capital-basel31](wiki/decisions/2025-05-24_v1-scope-uk-capital-basel31.md) — UK capital reporting + Basel 3.1 as narrow first domain
- [2025-05-24_human-review-guardrails](wiki/decisions/2025-05-24_human-review-guardrails.md) — No auto-submission, no production changes, human review required
- [2025-05-24_uncertainty-as-valid-outcome](wiki/decisions/2025-05-24_uncertainty-as-valid-outcome.md) — "I couldn't find sufficient evidence" is a valid outcome

**Note**: These decision pages carry `status: active` but require direct PM approval before use. L111 records "No decision was made...on final MVP feature set..." — these capture what was stated, not formal decisions.

## Assumptions (status: untested, updated: 2026-09-06)

Per AGENTS.md L96–101, assumption status changes require PM approval. All entries below are `status: untested`.

- [assumptions](wiki/assumptions.md) — A1 (adoption requires time savings), A2 (provenance > speed), A3 (uncertainty handling), A4 (UK capital reporting viable), A5 (two segments diverge), A6 (versioning feasible, **unsupported**)

## Overview (updated: 2026-09-06)

- [overview](overview.md) — Living synthesis: core problem, stakeholders, scope, not-yet-decided sections, problems, open questions, held proposals

## Log (updated: 2026-09-06)

- [log](log.md) — Append-only journal: [ingest 2026-09-06 Meeting 1](log.md#2026-09-06)

---

**Notes**

- `wiki/problems/` — 7 pages, all `status: emerging`, `status: confirmed` requires ≥3 independent sources or ≥2 source types (AGENTS.md L41)
- `wiki/decisions/` — 3 pages created, all `status: active` (PM approval pending)
- `wiki/assumptions/` — 6 entries created, all `status: untested` (PM approval pending)
- `wiki/open-questions.md` — 11 questions tagged by resolution path
- `wiki/overview.md` — Living synthesis, updated on every write
- `log.md` — Append-only, grep-able prefix `## [YYYY-MM-DD] ingest|query|lint|decision | <title>`