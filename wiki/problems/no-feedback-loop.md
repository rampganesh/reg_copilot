---
type: problem
status: confirmed
severity: high
mentions: 6
updated: 2025-06-18
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

### From Meeting 3 (2025-06-14) — staleness feedback loop
- Previously generated answers are not silently treated as current if their underlying source changed; affected answers must be identifiable as potentially stale and linked to the updated source/version (source: 2025_06_14_meeting_latedocuments.md, L8, L11)
- Prior answers preserved for audit/research with original source and temporal context; never automatically rewritten (source: 2025_06_14_meeting_latedocuments.md, L9)
- Explicit process: detection → SME validation → publication/update → identification of potentially affected prior answers (source: 2025_06_14_meeting_latedocuments.md, L12); filed as decision 2025-06-14_corpus-update-and-staleness-policy.md; residual gap = Q10 (staleness window; proactive re-review vs. flag-on-use)

### From interviews (2025-06-17/18) — impact tracing dimension
- On discovering a stale answer, the concerns go beyond correcting it: who received the original interpretation, whether anyone acted on it, what the replacement requirement is, and whether related questions were answered with the same interpretation — Analyst 1 (source: 2025_06_17_interview_analyst1exp.md, L88-93)
- Two separate concerns: correcting the original answer AND whether the outdated interpretation influenced other work; original temporal context must be preserved for later investigation — Analyst 2 (source: 2025_06_18_interview_analyst2prov.md, L91-96)
- Answers should be preserved with source and date "rather than treating answers as timeless pieces of knowledge" (source: 2025_06_17_interview_analyst1exp.md, L95)

## Contradicting evidence
None recorded.

## Related
- [[experience-dependency]]
- [[source-validation-burden]]
