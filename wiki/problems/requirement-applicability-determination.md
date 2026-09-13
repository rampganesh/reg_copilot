---
type: problem
status: confirmed
severity: high
mentions: 2
updated: 2025-06-04
cluster: evidence-workflow
---

# Requirement applicability determination

## Statement
Whether a requirement applies to the bank cannot be read off any single document. It depends on context — legal entity, consolidation perimeter, permissions, reporting regime, exposure type, reporting basis and the relevant date. Determining applicability is a large part of answering regulatory questions reliably, and an answer that describes a real requirement but applies it to the wrong entity, date or context is operationally wrong.

## Who has it
All analysts answering applicability questions ("does this apply to us?"); the Prudential Regulatory SME flagged it as a core reliability criterion for any AI-assisted answer.

## Evidence
- An answer should establish at least three things: what requirement is being discussed, which version or period it relates to, and whether it is applicable to the question — Prudential Regulatory SME (source: 2025_05_26_meeting_followup.md, L21)
- Applicability "can depend on factors such as the legal entity, consolidation perimeter, permissions, reporting regime, type of exposure, reporting basis and relevant date" — Prudential Regulatory SME (source: 2025_05_26_meeting_followup.md, L97)
- "The initial product should not claim to make definitive applicability decisions unless sufficient structured context and validated rules are available" — Prudential Regulatory SME (source: 2025_05_26_meeting_followup.md, L99)
- The product should distinguish between gathering information and making the final regulatory determination — Prudential Regulatory SME (source: 2025_05_26_meeting_followup.md, L101)
- Prior context: "latest document" is not necessarily the applicable requirement; a newer publication can discuss a future effective date while an older requirement remains applicable (source: 2025_05_26_meeting_followup.md, L17, L23)

### From email digest (2025-06-04) — status: confirmed (2 source types: meeting + digest)
- Autonomous applicability determination explicitly listed as an attractive extension, not a V1 capability (source: 2025_06_04_digest_clarifications.md, row 1)
- V1 remains evidence-led rather than an autonomous compliance decision-maker (source: 2025_06_04_digest_clarifications.md, row 1)

## Contradicting evidence
None recorded.

## Related
- [[source-validation-burden]]
- [[authority-overstatement-risk]]
- open-questions.md — applicability behaviour in v1
