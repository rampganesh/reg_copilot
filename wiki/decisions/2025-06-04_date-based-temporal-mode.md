---
type: decision
status: active
date: 2025-06-04
decider: PM (approving consolidated stakeholder responses from the email digest)
updated: 2025-06-04
---

# Date-based "current vs future requirement" mode

## Context
The group discussed current/future modes but left terminology and behaviour undefined (source: 2025_05_26_meeting_followup.md, L121); effective dates should be first-class information (source: 2025_05_26_meeting_followup.md, L25); "latest" is unsafe as a proxy for applicable (source: 2025_05_26_meeting_followup.md, L23).

## Options considered
1. **Latest-document heuristic** — rejected: unsafe; newer documents may amend part of a requirement, have future effective dates, or narrower scope (source: 2025_05_26_meeting_followup.md, L23).
2. **Label-based current/future toggle** — rejected: ambiguous labels without a date basis reproduce the same error.
3. **Explicitly date-based mode** — adopted (source: 2025_06_04_digest_clarifications.md, row 6).

## Decision & rationale
Yes to current/future distinction, **explicitly date-based**: "current" = applicable **as of a specified/reference date**; "future" = requirements with a future effective/applicability date. Publication date must not be treated as equivalent to applicability. Users can see effective date/status and distinguish final requirements from proposals. Temporal awareness and explicit as-of/effective-date behaviour in V1; ambiguous labels such as "latest" avoided; the temporal basis is visible in both search and answers (source: 2025_06_04_digest_clarifications.md, row 6).

## Reversal conditions
- If as-of querying proves confusing to users in testing, revisit the interaction design (not the date-based principle).
- If metadata for effective dates cannot be reliably obtained for corpus material, the mode cannot ship — escalate to the corpus governance decision.

## Related
- [[../problems/source-validation-burden]]
- [[../problems/requirement-applicability-determination]]
- 2025-06-04_temporal-awareness-v1; 2025-06-04_bounded-curated-corpus