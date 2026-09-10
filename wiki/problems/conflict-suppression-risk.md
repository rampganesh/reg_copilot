---
type: problem
status: emerging
severity: high
mentions: 1
updated: 2026-09-09
---

# Conflict Suppression Risk

## Statement

Conflicts between regulatory sources must be **exposed rather than silently resolved**. "The first requirement should be to expose the conflict rather than silently resolve it" (L67); "apparent conflicts can arise because documents relate to different dates, different scopes, different populations or different levels of detail" (L69); "an AI-generated resolution of a regulatory conflict should therefore be treated very cautiously" (L71). **(source: 2025_05_26_meeting_followup.md, L67, L69, L71, L75)**

## Who has it

- **Prudential Regulatory SME**: explicitly requires conflict exposure (L67, L69, L71)
- **Compliance representative**: supports "I don't have sufficient evidence to answer this" as acceptable (L77)
- **Analysts**: need to understand why conflicts exist before deciding applicability (L69)

## Evidence

- **Expose conflicts rule**: "the first requirement should be to expose the conflict rather than silently resolve it" (L67)
- **Conflict origins**: "apparent conflicts can arise because documents relate to different dates, different scopes, different populations or different levels of detail. An analyst needs to understand why the conflict exists before deciding which statement applies" (L69)
- **Caution on AI resolution**: "an AI-generated resolution of a regulatory conflict should therefore be treated very cautiously. In some cases the correct outcome may be to escalate the issue to a human expert" (L71)
- **First capability for conflict handling**: "a safer first capability would be to identify situations where the available evidence is insufficient, conflicting, ambiguous or clearly associated with different effective dates" (L75)
- **Valid refusal**: "'I don't have sufficient evidence to answer this' should be considered an acceptable system outcome" (L77)

## Contradicting evidence

- **Refusal can reduce usefulness**: "an answer that refuses unnecessarily can also reduce usefulness" (L141) — suggests the system must balance conflict exposure with responsiveness.
- **Escalation detection is hard**: "this would be valuable, but it would be difficult to define reliably at the outset" (L73) — the ability to identify conflict situations may not be easily codified.

## Related

- **Open questions**: Q14 (justified vs unnecessary refusal), Q16 (conflict exposure vs resolution)
- **Assumptions**: A3 (uncertainty handling)
- **Overview**: hard constraints - expose conflicts, not resolve