---
type: problem
status: emerging
severity: medium
mentions: 3
updated: 2025-06-04
---

# No feedback loop on prior answers

## Statement
The team has no consistent way to record whether a previously produced answer was useful, whether it was later corrected, or which source ultimately resolved the question. Analysts sometimes discover weeks later that an answer rested on an outdated document or incomplete interpretation, but nothing systematically captures that correction — so incorrect interpretations can circulate internally.

## Who has it
All analysts; consequences (incorrect interpretations circulating) affect the whole team and downstream consumers of their answers.

## Evidence
- "The team currently has no consistent way of recording whether an answer produced by previous research was useful, whether it was subsequently corrected, or which source ultimately resolved the question." — Regulatory Reporting Manager (source: 2025_05_24_meeting_kickoff.md, L63)
- "Analysts sometimes discover after several weeks that a previous answer was based on an outdated document or incomplete interpretation. There is no systematic feedback mechanism for capturing this information." — Analyst 1 (source: 2025_05_24_meeting_kickoff.md, L65)
- "An incomplete search, outdated source or misunderstood requirement can lead to an incorrect interpretation being circulated internally." — Regulatory Change/Reporting SME (source: 2025_05_24_meeting_kickoff.md, L101)

### From Meeting 2 (2025-05-26) — what good feedback should look like
- SME corrections should be associated with the underlying question, answer, evidence and version of the regulatory material used at the time — Prudential Regulatory SME (source: 2025_05_26_meeting_followup.md, L85)
- Thumbs-up/down is probably insufficient; useful categories: incorrect answer, insufficient evidence, incorrect source, outdated source, irrelevant source, correct but poorly explained (source: 2025_05_26_meeting_followup.md, L87)
- Analysts want to report "this source is relevant but the answer missed an important qualification" (source: 2025_05_26_meeting_followup.md, L89)
- Track cases where analysts ignored the AI answer and researched manually — those reveal product shortcomings without formal negative feedback (source: 2025_05_26_meeting_followup.md, L149)
- The system should preserve enough information to reconstruct how an answer was produced — an auditable record of sources and evidence used, not just the AI response (source: 2025_05_26_meeting_followup.md, L91-93)
- Retaining analysts' final answers raises data retention, ownership and reliance considerations; not assumed in initial design — Compliance representative (source: 2025_05_26_meeting_followup.md, L151)

### From email digest (2025-06-04)
- Safe behaviour is a scorecard dimension: appropriate refusal/escalation and unsupported-answer rate are explicit V1 measures (source: 2025_06_04_digest_clarifications.md, row 3); clear indication of uncertainty/insufficient evidence is a core V1 capability (source: 2025_06_04_digest_clarifications.md, row 1)

## Contradicting evidence
None recorded.

## Related
- [[experience-dependency]]
- [[source-validation-burden]]
