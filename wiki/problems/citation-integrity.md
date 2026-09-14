---
type: problem
status: confirmed
severity: high
mentions: 5
updated: 2025-06-18
cluster: evidence-workflow
---

# Citation integrity

## Statement
Citations are only useful if an analyst can independently verify them. The system must identify the document, the relevant section or paragraph, and enough surrounding context to see how the cited text supports the answer — and it must never manufacture paragraph numbers, section references or quotations that the source does not contain. An incorrect citation is worse than no citation because it creates a false impression of auditability.

## Who has it
All analysts relying on system output in a high-confidence research workflow; Compliance views citation fabrication as a trust-breaking failure mode.

## Evidence
- "A generic document link is useful but insufficient for a high-confidence research workflow" — Prudential Regulatory SME (source: 2025_05_26_meeting_followup.md, L49)
- Analysts want the citation to identify the document, relevant section or paragraph, and enough surrounding context (source: 2025_05_26_meeting_followup.md, L51)
- "The system should not manufacture paragraph numbers, section references or quotations when the source does not contain them" — Prudential Regulatory SME (source: 2025_05_26_meeting_followup.md, L53)
- "An incorrect citation may be worse than no citation because it creates a false impression of auditability" — Compliance representative (source: 2025_05_26_meeting_followup.md, L55)
- Quotations must preserve context — extracting a single sentence can remove a qualification, exception or condition (source: 2025_05_26_meeting_followup.md, L57)
- Tension: larger excerpts improve context but make answers cumbersome; the objective is enough surrounding material to validate the claim without re-searching the document (source: 2025_05_26_meeting_followup.md, L59)
- Extraction complication: much operative meaning sits in tables/templates, not prose, so a quotable paragraph may not exist for what answers the question — see [[non-prose-regulatory-content]]

### From email digest (2025-06-04) — status: confirmed (2 source types: meeting + digest)
- Minimum provenance standard established: provenance should normally identify the document/source, version or status, relevant section, and where applicable the paragraph, table, reporting instruction/template reference, or page/location (source: 2025_06_04_digest_clarifications.md, row 4)
- Provenance must allow an analyst to independently verify the claim quickly; document-level references alone are insufficient for important answers (source: 2025_06_04_digest_clarifications.md, row 4)
- "The system must not fabricate quotations or references" — restated as a hard requirement (source: 2025_06_04_digest_clarifications.md, row 4)
- Evaluation should test citation correctness and completeness (source: 2025_06_04_digest_clarifications.md, row 4)

### From interviews (2025-06-17/18)
- Rejected research patterns: broad document-only citations, interpretations without underlying regulatory wording, unclear status/date, confident conclusions despite diverging sources — Analyst 1 (source: 2025_06_17_interview_analyst1exp.md, L46-53); "a citation is useful only if it reduces the effort required to verify the answer" (L57)
- Analyst 2's rejection list adds: screenshots without context, "PRA guidance" without precise location, secondary explanations when primary material was available, non-reproducible citations, statements inconsistent with the cited document's status/effective date (source: 2025_06_18_interview_analyst2prov.md, L50-57)
- Fastest path to trust: "click or navigate directly to the exact supporting provision and verify that the source actually said what the answer claimed" (source: 2025_06_18_interview_analyst2prov.md, L59)
- Granularity is situational: section/paragraph suffices for textual requirements; reporting questions need template/table/row/field/instruction references (source: 2025_06_18_interview_analyst2prov.md, L63-71; source: 2025_06_17_interview_analyst1exp.md, L65)
- "The tool would lose trust quickly if it produced a confident answer with an impressive-looking but incorrect citation" — Analyst 1 (source: 2025_06_17_interview_analyst1exp.md, L143)
- "Provenance part of the answer itself, rather than supporting material added later" — Analyst 2 (source: 2025_06_18_interview_analyst2prov.md, L75)

## Contradicting evidence
None recorded.

## Related
- [[evidence-assembly-time-cost]]
- [[authority-overstatement-risk]]
- open-questions.md — provenance precision (Q5)
