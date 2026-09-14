---
type: problem
status: confirmed
severity: high
mentions: 5
updated: 2025-06-18
cluster: evidence-workflow
---

# Evidence assembly time cost

## Statement
Understanding a regulatory answer is fast; assembling the evidence to support it is slow. Analysts spend about five minutes understanding an answer but another fifteen to twenty minutes finding the exact section, paragraph, table, reporting instruction or definition that supports it and presenting that evidence so another person can independently verify the conclusion.

## Who has it
All analysts on the UK capital regulatory reporting team; felt most acutely when responding to questions from the reporting team, other internal teams, or subject-matter experts.

## Evidence
- "The analyst may spend five minutes understanding the answer and another fifteen or twenty minutes finding the exact section that supports it and presenting the evidence clearly." — Analyst 1 (source: 2025_05_24_meeting_kickoff.md, L33)
- Analysts attach links, document references, extracts or screenshots so another person can independently verify the conclusion; producing this evidence takes significant time — Regulatory Reporting Manager (source: 2025_05_24_meeting_kickoff.md, L31)
- "Simply returning a regulatory document would not solve the problem. Analysts need help getting from a broad document to the specific section, paragraph, table, reporting instruction or definition relevant to the question." — Analyst 2 (source: 2025_05_24_meeting_kickoff.md, L35)
- The manager's success criterion for a first version is reducing time spent searching and assembling evidence while maintaining or improving answer quality (source: 2025_05_24_meeting_kickoff.md, L73)

### From Meeting 2 (2025-05-26) — evidence-presentation requirements that shape this problem
- Citations must identify document, relevant section or paragraph, plus surrounding context to verify how the cited text supports the answer (source: 2025_05_26_meeting_followup.md, L49-51)
- System must not manufacture paragraph numbers, section references or quotations not present in the source (source: 2025_05_26_meeting_followup.md, L53)
- Incorrect citations are worse than none — false auditability (source: 2025_05_26_meeting_followup.md, L55)
- Quotations must preserve qualifications, exceptions and conditions; single-sentence extraction can strip them (source: 2025_05_26_meeting_followup.md, L57)
- Excerpt sizing trade-off: larger excerpts give context but make answers cumbersome (source: 2025_05_26_meeting_followup.md, L59)
- The most valuable initial capability per the Prudential SME: help analysts "find and connect authoritative regulatory evidence quickly" (source: 2025_05_26_meeting_followup.md, L153)

→ See the dedicated [[citation-integrity]] page for the full treatment.

### From email digest (2025-06-04)
- Success metric for the product centres on this problem: "reduction in time required to produce a verified, evidence-backed answer without reducing evidence quality or increasing unsafe answers" (source: 2025_06_04_digest_clarifications.md, row 3); a manual-process baseline should be established first
- V1 focus confirmed as finding, connecting, and explaining authoritative evidence — the evidence-assembly workflow is the core, not an extension (source: 2025_06_04_digest_clarifications.md, row 1)

### From interviews (2025-06-17/18) — behavioural confirmation
- Analyst 1's end-to-end walkthrough: "the largest amount of effort was **not necessarily finding the first relevant document**. More time was spent confirming that it was the correct version and source, following cross-references, and assembling defensible evidence" (source: 2025_06_17_interview_analyst1exp.md, L24)
- Analyst 2: "assembling and validating provenance was one of the most time-consuming parts", particularly with multiple contributing documents (source: 2025_06_18_interview_analyst2prov.md, L25)
- Both define tool success as faster research while preserving the analyst's ability to verify (source: 2025_06_17_interview_analyst1exp.md, L145; source: 2025_06_18_interview_analyst2prov.md, L145)

## Contradicting evidence
None recorded.

## Related
- [[assumptions|A1: adoption conditional on time savings]]
- [[source-validation-burden]]
- [[citation-integrity]]
- Open question: what counts as "assembled evidence" worth measuring — see open-questions.md
