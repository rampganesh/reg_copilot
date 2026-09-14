---
type: problem
status: confirmed
severity: high
mentions: 7
updated: 2025-06-18
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

### From desk research (2025-06-10) — the overlap is concrete
- Live Basel 3.1 publication timeline with five overlapping states: CP16/22 consultation (Nov 2022, RWA/credit/market risk/output floor), near-final PS17/23 (Dec 2023, market/operational risk/CVA) and PS9/24 (Sep 2024, credit risk/output floor), final rules PS1/26 (Jan 2026), and post-final consultation CP9/26 (June 2026, IMA market-risk adjustments) (source: 2025_06_10_research_docversions.md, L6-9)
- A post-final consultation (CP9/26, June 2026) arrives after the final rules (PS1/26, Jan 2026) — so "newest document" sits alongside "final rules" and both differ in status; consultation language can look near-identical to requirements (source: 2025_06_10_research_docversions.md, L8-9)
- The PRA also publishes "what changed" comparison documents alongside subsequent publications (source: 2025_06_10_research_docversions.md, L10) — relevant to manual current/future comparison in V1 (see decision 2025-06-04_temporal-awareness-v1)

### From Meeting 3 (2025-06-14) — operational handling agreed
- Amendment validation gate: new amendments reviewed for source authority, regulatory status, effective date and relationship to existing material before entering the active corpus (source: 2025_06_14_meeting_latedocuments.md, L7)
- Staleness determined by source status and effective/applicability dates rather than publication date (source: 2025_06_14_meeting_latedocuments.md, L10); user-facing flagging when a response relies on superseded/amended material (L11)
- Detection by the technical pipeline does not establish relevance or authority — Content Owner confirmation required (source: 2025_06_14_meeting_latedocuments.md, L6); filed as decision 2025-06-14_corpus-update-and-staleness-policy.md

### From interviews (2025-06-17/18) — source validation is normal work, not an exception
- "Source validation is a normal part of the work, not an exceptional check" — Analyst 1 (source: 2025_06_17_interview_analyst1exp.md, L40); first result treated as a starting point, checked for document type, final/proposed/historical status, effective date, more-specific instructions, and reference chains (L28-38)
- Analyst 2's six-question validation checklist: authoritative? correct version? operative/future/proposed/historical? actually answers the question? more specific instruction? linked provisions changing interpretation? (source: 2025_06_18_interview_analyst2prov.md, L31-39)
- "Search relevance and regulatory correctness are two different things" — Analyst 2 (source: 2025_06_18_interview_analyst2prov.md, L42)

## Contradicting evidence
None recorded.

## Related
- [[evidence-assembly-time-cost]]
- [[terminology-cross-referencing]]
- [[requirement-applicability-determination]]
- [[authority-overstatement-risk]]
- Open question: how does the system handle document versions/dates without treating the corpus as fixed — see open-questions.md
