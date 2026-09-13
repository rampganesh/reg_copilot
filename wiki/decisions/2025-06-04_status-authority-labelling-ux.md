---
type: decision
status: active
date: 2025-06-04
decider: PM (approving consolidated stakeholder responses from the email digest)
updated: 2025-06-04
---

# Status/authority labelling in core UX with evidence-led language

## Context
Compliance flagged "the regulation says" mislabelling risk (source: 2025_05_26_meeting_followup.md, L39) and the "applicable requirement" vs "relevant sources indicate" distinction (source: 2025_05_26_meeting_followup.md, L105); the SME required relationship-aware authority rather than a universal score (source: 2025_05_26_meeting_followup.md, L37).

## Options considered
1. **Status as hidden metadata** — rejected: users should not have to interpret model internals or metadata to judge trustworthiness (source: 2025_05_26_meeting_followup.md, L107).
2. **Evidence-led language + visible status labels in core UX** — adopted (source: 2025_06_04_digest_clarifications.md, row 7).

## Decision & rationale
Language is **evidence-led and appropriately cautious**: preferred formulations "Relevant sources indicate…", "The cited PRA material states…", "The following sources appear relevant…". "The applicable requirement is…" is **reserved for cases where applicability has been validated/approved**. Material is labelled by status/type: **final/operative, future effective, superseded/historical, proposed/consultation, explanatory/supporting**. Status and authority labelling is built into the **core UX**, not hidden metadata. The assistant never silently resolves conflicting sources or presents a proposal as a requirement; ambiguous/conflicting evidence triggers an explicit warning or escalation path (source: 2025_06_04_digest_clarifications.md, row 7).

## Reversal conditions
- If label taxonomy proves too coarse or too noisy for real corpus material, propose a revised taxonomy to Compliance/SMEs (relabel, not remove).
- If user testing shows the cautious language hides genuinely validated findings and reduces usefulness, revisit the "validated/approved applicability" wording path with Compliance.

## Related
- [[../problems/authority-overstatement-risk]]
- [[../problems/conflict-exposure]]
- 2025-06-04_date-based-temporal-mode; 2025-06-04_minimum-provenance-standard