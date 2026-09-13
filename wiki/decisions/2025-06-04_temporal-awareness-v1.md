---
type: decision
status: active
date: 2025-06-04
decider: PM (approving consolidated stakeholder responses from the email digest)
updated: 2025-06-04
---

# Temporal/version awareness in V1; interpretive change analysis deferred

## Context
Basel 3.1 creates a transition period where current and future requirements coexist; "latest" is not the applicable requirement (source: 2025_05_26_meeting_followup.md, L17, L23); the manager did not want What-changed assumed into V1 (source: 2025_05_24_meeting_kickoff.md, L59).

## Options considered
1. **Include full interpretive "What changed?" in V1** — rejected: determining regulatory significance of textual changes requires context and applicability understanding (source: 2025_05_26_meeting_followup.md, L125); a much larger problem than finding text (source: 2025_05_24_meeting_kickoff.md, L61).
2. **Defer all temporal awareness** — rejected: users need to distinguish current/future/superseded/proposed material during the transition (source: 2025_06_04_digest_clarifications.md, row 2).
3. **Basic temporal/version awareness in V1; defer sophisticated change analysis** — adopted.

## Decision & rationale
Include **basic temporal/version awareness in V1**: users can retrieve and compare relevant current/future sources manually. Defer automated/interpretive change analysis to a later release (source: 2025_06_04_digest_clarifications.md, row 2).

## Reversal conditions
- Transition-period work shows manual comparison is a dominant time cost that simple automation could safely remove.
- An evaluated, low-risk textual-diff plus status-aware presentation proves reliable in testing.

## Related
- [[../problems/source-validation-burden]]
- 2025-06-04_v1-scope-evidence-led-research; 2025-06-04_date-based-temporal-mode