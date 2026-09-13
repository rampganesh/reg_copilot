# Open questions

## Q1: Which capabilities solve the core research problem vs. attractive extensions?
- tag: ask-users
- origin: The manager asked that discovery distinguish core-research capabilities from extensions (source: 2025_05_24_meeting_kickoff.md, L105-107); candidates named: search, Q&A, evidence gathering, document comparison, regulatory-change analysis
- status: answered (source: 2025_06_04_digest_clarifications.md, row 1) → filed in wiki/decisions/2025-06-04_v1-scope-evidence-led-research.md. Core: authoritative search, NL querying, related-material discovery, version/status awareness, evidence-backed explanations, precise citations, uncertainty signalling. Extensions deferred: interpretive What-changed, downstream impact, autonomous applicability, automated changes, internal answers as authority.

## Q2: Should "What has changed?" (current vs. future requirement comparison) be in the first release?
- tag: ask-stakeholder
- origin: Analyst 2 raised it as useful; the manager explicitly did not want it assumed into the first release (source: 2025_05_24_meeting_kickoff.md, L59); the SME noted downstream-impact analysis is a much larger problem than finding text (source: 2025_05_24_meeting_kickoff.md, L61)
- update 2025-05-26: SME nuance — identifying textual changes between documents is different from determining regulatory significance; a change comparison can be research support, but a textual difference should not imply a change in the firm's obligation (source: 2025_05_26_meeting_followup.md, L125-127); downstream impact analysis explicitly not assumed for first product (source: 2025_05_26_meeting_followup.md, L129-131)
- status: answered (source: 2025_06_04_digest_clarifications.md, row 2) → filed in wiki/decisions/2025-06-04_temporal-awareness-v1.md. Full interpretive What-changed not a V1 requirement; basic temporal/version awareness is foundational; manual current/future comparison in V1, automated change analysis later.

## Q3: How should the system handle document versions, dates and late-arriving amendments rather than treating the corpus as fixed?
- tag: desk-research
- origin: "New clarifications, amendments and related publications can appear after an analyst has already performed research" — SME (source: 2025_05_24_meeting_kickoff.md, L87)
- status: open

## Q4: What success metrics should define the first version?
- tag: ask-stakeholder
- origin: "No decision was made during the meeting on … success metrics" (source: 2025_05_24_meeting_kickoff.md, L111); manager's stated goal is reduced search/assembly time with maintained or improved quality (source: 2025_05_24_meeting_kickoff.md, L73)
- status: answered (source: 2025_06_04_digest_clarifications.md, row 3) → filed in wiki/decisions/2025-06-04_v1-balanced-scorecard.md. Balanced scorecard: productivity, retrieval quality, answer/evidence quality, safe behaviour, adoption; manual baseline first; north-star candidate: time to verified evidence-backed answer without quality/ safety loss.

## Q5: What counts as sufficiently precise provenance in practice (section, paragraph, table, instruction reference)?
- tag: ask-users
- origin: "A link to a 300-page policy document would not be enough" — Regulatory Reporting Manager (source: 2025_05_24_meeting_kickoff.md, L47); extended by Meeting 2: document + section/paragraph + surrounding context (source: 2025_05_26_meeting_followup.md, L49-51)
- status: answered (source: 2025_06_04_digest_clarifications.md, row 4) → filed in wiki/decisions/2025-06-04_minimum-provenance-standard.md. Minimum standard: source + document/version/status + precise location (section, paragraph, table, row/field, instruction/template reference, or page/location); no fabrication; structured material covered.

## Q6: What are the inclusion/exclusion criteria for the deliberately defined first-version corpus?
- tag: ask-stakeholder
- origin: SME recommends a deliberately defined corpus for UK capital reporting / Basel 3.1 with explicit criteria and per-source metadata (publication date, effective date, document type, subject area, version/status, relationships) — not just a URL collection (source: 2025_05_26_meeting_followup.md, L109-113); partially answered — actual scope not yet chosen
- status: answered (source: 2025_06_04_digest_clarifications.md, row 5) → filed in wiki/decisions/2025-06-04_bounded-curated-corpus.md. Include: authoritative, relevant UK capital/reporting material with sufficient metadata. Exclude: unrelated domains, uncontrolled web content, unclear provenance/status, internal bank material (initially), sources mistakable for operative requirements. Governance: Regulatory/Prudential SME or Regulatory Content Owner governs inclusion/relationships; Technology owns ingestion/indexing.

## Q7: Should there be a "current requirement" vs "future requirement" mode, and how would its terminology/behaviour be defined?
- tag: ask-stakeholder
- origin: Raised and left undefined — "could be useful, but the terminology and behaviour would need to be carefully defined" (source: 2025_05_26_meeting_followup.md, L121)
- status: answered (source: 2025_06_04_digest_clarifications.md, row 6) → filed in wiki/decisions/2025-06-04_date-based-temporal-mode.md. Yes — explicitly date-based; "current" = applicable as of a specified/reference date; "future" = future effective/applicability date; publication date ≠ applicability; avoid "latest"; temporal basis visible in search and answers.

## Q8: How should the product be evaluated — what test set, what failure modes, what metrics?
- tag: run-experiment
- origin: SME wants realistic historical questions incl. deliberately difficult cases (outdated docs, future requirements, similar terminology, multiple sources, insufficient-evidence cases); easy-only evaluation misleads (source: 2025_05_26_meeting_followup.md, L133-137); evaluation should include confidently-wrong answers, not just answer production (source: 2025_05_26_meeting_followup.md, L139); not every question has a single expected natural-language answer (source: 2025_05_26_meeting_followup.md, L145); consider tracking ignored answers (source: 2025_05_26_meeting_followup.md, L149)
- status: open

## Q9: What interface language and status-labelling conventions should the product use?
- tag: ask-stakeholder
- origin: "The regulation says" must not be used when the evidence is a supervisory statement, explanatory publication or internal interpretation (source: 2025_05_26_meeting_followup.md, L39); "The applicable requirement is..." materially different from "The relevant sources indicate..." plus caveat (source: 2025_05_26_meeting_followup.md, L105); internal answers labelled separately from external regulatory sources (source: 2025_05_26_meeting_followup.md, L81)
- status: answered (source: 2025_06_04_digest_clarifications.md, row 7) → filed in wiki/decisions/2025-06-04_status-authority-labelling-ux.md. Evidence-led formulations adopted; status/type labels (final/operative, future effective, superseded/historical, proposed/consultation, explanatory/supporting) built into core UX; conflicts trigger warning/escalation; "The applicable requirement is…" reserved for validated applicability.
