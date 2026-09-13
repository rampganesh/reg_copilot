---
type: problem
status: confirmed
severity: high
mentions: 2
updated: 2025-06-04
cluster: evidence-workflow
---

# Conflict exposure (not suppression)

## Statement
When two sources appear to conflict, the system's first job is to expose the conflict rather than silently resolve it. Apparent conflicts arise from documents relating to different dates, scopes, populations or levels of detail, and the analyst must understand why a conflict exists before deciding which statement applies. AI-generated resolution of a regulatory conflict should be treated very cautiously; sometimes the correct outcome is escalation to a human expert.

## Who has it
All analysts; raised by the Compliance representative and the Prudential Regulatory SME as a required system behaviour.

## Evidence
- "The first requirement should be **to expose the conflict rather than silently resolve it**" — Prudential Regulatory SME (source: 2025_05_26_meeting_followup.md, L67)
- Apparent conflicts arise from different dates, scopes, populations or levels of detail; the analyst needs to understand why before deciding (source: 2025_05_26_meeting_followup.md, L69)
- "An AI-generated resolution of a regulatory conflict should therefore be treated very cautiously. In some cases the correct outcome may be to escalate the issue to a human expert." — Prudential Regulatory SME (source: 2025_05_26_meeting_followup.md, L71)
- A safer first capability is identifying situations where evidence is insufficient, conflicting, ambiguous or associated with different effective dates (source: 2025_05_26_meeting_followup.md, L75)
- Related constraint: the system should not present a historical document as an equally valid answer merely because its text is highly relevant (source: 2025_05_26_meeting_followup.md, L119)

### From email digest (2025-06-04) — status: confirmed (2 source types: meeting + digest)
- "The assistant should never silently resolve conflicting sources or present a proposal as a requirement. Ambiguous/conflicting evidence should trigger an explicit warning or escalation path." (source: 2025_06_04_digest_clarifications.md, row 7)

## Contradicting evidence
None recorded.

## Related
- [[requirement-applicability-determination]]
- [[no-feedback-loop]]
