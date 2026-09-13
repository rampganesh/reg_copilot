---
type: problem
status: confirmed
severity: high
mentions: 3
updated: 2025-06-04
cluster: evidence-workflow
---

# Source validation burden

## Statement
Finding a first relevant document is not the hard part. The hard part is establishing that it is the *right* source: that it is applicable to the question, that it has not been superseded by a later publication, and — during the Basel 3.1 transition — that it answers the question about the current regime, the future regime, or the transition between them. An answer that is technically correct but refers to a requirement that is not yet applicable is still operationally wrong.

## Who has it
All analysts; particularly acute during the Basel 3.1 transition where documents describe either existing or future requirements.

## Evidence
- "Finding the first potentially relevant document is generally not the hardest part. The difficulty is establishing that the document is actually the **right source**, that it is applicable… and that it has not been superseded by a later publication." — Analyst 1 (source: 2025_05_24_meeting_kickoff.md, L11)
- During a transition, one document describes the existing requirement and another the future one; analysts must know which regime they are answering about — Regulatory Change/Reporting SME (source: 2025_05_24_meeting_kickoff.md, L17)
- "Effective dates are therefore critical. An answer that is technically correct but refers to a requirement that is not yet applicable can still be operationally wrong." — Regulatory Change/Reporting SME (source: 2025_05_24_meeting_kickoff.md, L19)
- Previous internal interpretations are not automatically authoritative; the underlying source must be checked before reuse — SME (source: 2025_05_24_meeting_kickoff.md, L29)
- The system should distinguish document types (final rule, reporting instruction, supervisory statement, older consultation) so they do not appear to have equal authority — SME (source: 2025_05_24_meeting_kickoff.md, L49)

### From Meeting 2 (2025-05-26)
- Treating "the PRA website" as a single source of truth is the first mistake to avoid; material differs in purpose, status and authority — Prudential Regulatory SME (source: 2025_05_26_meeting_followup.md, L7)
- Main source types: PRA Rulebook, policy statements, supervisory statements, reporting instructions and templates, other PRA publications; Basel/explanatory material is background, not automatically the operative UK requirement (source: 2025_05_26_meeting_followup.md, L9)
- A search result with correct terminology does not necessarily give the correct answer; the system must distinguish explanatory vs. requirement-establishing vs. reporting-instruction vs. historical/superseded material (source: 2025_05_26_meeting_followup.md, L11)
- Consultation papers must be distinguished from final requirements — near-identical language can be a proposal, not the requirement (source: 2025_05_26_meeting_followup.md, L13)
- "Latest document" is not necessarily the applicable requirement — a newer publication may discuss a future implementation date while an older requirement remains in force (source: 2025_05_26_meeting_followup.md, L17)
- Effective dates should be "first-class information rather than something an analyst has to infer from a document's publication date" (source: 2025_05_26_meeting_followup.md, L25)
- Prioritising the newest PRA document is unsafe: it may amend only part of a requirement, have a future effective date, or apply to a particular population/context (source: 2025_05_26_meeting_followup.md, L23)
- The recommended corpus needs metadata per source: publication date, effective date, document type, subject area, version/status, relationships to other material — not just URLs (source: 2025_05_26_meeting_followup.md, L113); templates and instructions must be versioned alongside the regulatory material (source: 2025_05_26_meeting_followup.md, L115)

### From email digest (2025-06-04) — status: confirmed (2 source types: meeting + digest)
- Basic temporal/version awareness confirmed foundational for V1: users must distinguish current, future, superseded and proposed material because Basel 3.1 creates a transition period; sophisticated change analysis deferred (source: 2025_06_04_digest_clarifications.md, row 2)
- "Current" must mean applicable as of a specified/reference date; publication date must not be treated as equivalent to applicability; avoid ambiguous labels such as "latest"; the temporal basis should be visible in both search and answers (source: 2025_06_04_digest_clarifications.md, row 6)
- Corpus will be bounded and curated with explicit include/exclude criteria; material that could be mistaken for operative requirements when only explanatory/proposed is excluded (source: 2025_06_04_digest_clarifications.md, row 5)
- Status labels required: final/operative, future effective, superseded/historical, proposed/consultation, explanatory/supporting (source: 2025_06_04_digest_clarifications.md, row 7)

## Contradicting evidence
None recorded.

## Related
- [[evidence-assembly-time-cost]]
- [[terminology-cross-referencing]]
- [[requirement-applicability-determination]]
- [[authority-overstatement-risk]]
- Open question: how does the system handle document versions/dates without treating the corpus as fixed — see open-questions.md
