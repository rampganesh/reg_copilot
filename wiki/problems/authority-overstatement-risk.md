---
type: problem
status: confirmed
severity: high
mentions: 4
updated: 2025-06-10
cluster: evidence-workflow
---

# Authority overstatement risk

## Statement
Regulatory material carries different status and purpose, and the relationships between sources are relational rather than a simple ranking — "Rulebook always wins" is not a safe model. A system risks overstating authority when it presents explanatory, supervisory, historical or internal material as if it were the operative requirement, or when its interface language ("The applicable requirement is…") implies more certainty than the evidence supports. Trust should come from transparent evidence, source status and dates — not from a confidence score.

## Who has it
All analysts and downstream readers of analyst answers; Compliance and the Prudential Regulatory SME both flagged it as a trust and auditability risk.

## Evidence
- "Treating 'the PRA website' as a single source of truth" is the first mistake to avoid; material types differ in purpose, status and authority (source: 2025_05_26_meeting_followup.md, L7)
- A useful assistant needs to understand **relationships between sources**, not assign "a universal authority score to every document" — Prudential Regulatory SME (source: 2025_05_26_meeting_followup.md, L37)
- "The product should avoid language such as 'the regulation says' when the evidence is actually a supervisory statement, explanatory publication or internal interpretation" — Compliance representative (source: 2025_05_26_meeting_followup.md, L39)
- "The applicable requirement is..." is materially different from "The relevant sources indicate..." followed by evidence and a caveat — Compliance representative (source: 2025_05_26_meeting_followup.md, L105)
- Internal answers can be evidence of prior organisational interpretation but must be labelled separately from external regulatory sources (source: 2025_05_26_meeting_followup.md, L79-83)
- "Users should not have to interpret a model's confidence score to understand whether an answer is trustworthy" — Prudential Regulatory SME (source: 2025_05_26_meeting_followup.md, L107); see also Compliance on confidence scores (source: 2025_05_26_meeting_followup.md, L29)

### From email digest (2025-06-04)
- Evidence-led, cautious language confirmed as preferred formulation set: "Relevant sources indicate…", "The cited PRA material states…", "The following sources appear relevant…"; "The applicable requirement is…" reserved for validated/approved applicability (source: 2025_06_04_digest_clarifications.md, row 7)
- Status/type labelling (final/operative, future effective, superseded/historical, proposed/consultation, explanatory/supporting) to be built into core UX, not hidden metadata (source: 2025_06_04_digest_clarifications.md, row 7)
- Using internal historical answers as an authoritative knowledge source explicitly deferred out of V1 (source: 2025_06_04_digest_clarifications.md, row 1)

### From desk research (2025-06-10) — status: confirmed (3 sources, 3 source types: meeting + digest + research)
- The risk is now factually demonstrated in the live corpus: consultation CP16/22 (2022), near-final PS17/23 and PS9/24, final rules PS1/26 (Jan 2026) and post-final consultation CP9/26 (June 2026) all coexist; presenting any of these without status labelling would overstate or misstate authority (source: 2025_06_10_research_docversions.md, L6-9)
- Post-final consultations (CP9/26) introduce "operational simplifications and targeted adjustments" — a document published *after* the final rules that is not an operative requirement (source: 2025_06_10_research_docversions.md, L9)

## Contradicting evidence
None recorded.

## Related
- [[source-validation-burden]]
- [[citation-integrity]]
- [[conflict-exposure]]
