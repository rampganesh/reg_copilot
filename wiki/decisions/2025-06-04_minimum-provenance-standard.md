---
type: decision
status: active
date: 2025-06-04
decider: PM (approving consolidated stakeholder responses from the email digest)
updated: 2025-06-04
---

# Minimum provenance standard

## Context
"A link to a 300-page policy document would not be enough" (source: 2025_05_24_meeting_kickoff.md, L47); citations must allow independent verification and must never be manufactured; an incorrect citation is worse than none (source: 2025_05_26_meeting_followup.md, L49-55); structured material has no quotable paragraph to cite (see [[../problems/non-prose-regulatory-content]]).

## Options considered
1. **Document-level links only** — rejected: insufficient for a high-confidence research workflow (source: 2025_05_26_meeting_followup.md, L49).
2. **Document + section/paragraph where prose permits** — rejected: fails for tables/templates (source: 2025_05_26_meeting_followup.md, L61).
3. **Minimum provenance standard including structured references** — adopted (source: 2025_06_04_digest_clarifications.md, row 4).

## Decision & rationale
Establish a **minimum provenance standard**: provenance normally identifies the **document/source, version or status, and precise location** — relevant section and, where applicable, the **paragraph, table, reporting instruction/template reference, or page/location** — such that an analyst can **independently verify the claim quickly**. Document-level references alone are insufficient for important answers. The system must not fabricate quotations or references. For structured reporting material, provenance may need to identify the specific **table, row/field, instruction or template reference**. Evaluation tests citation correctness and completeness (source: 2025_06_04_digest_clarifications.md, row 4).

## Reversal conditions
- If structured references prove unreliable to generate automatically, revisit the granularity floor with Compliance (fallback: refuse or mark provenance as partial rather than fabricate).
- If verification-time measurements show the standard is insufficient for expert verification, raise the bar rather than lower it.

## Related
- [[../problems/citation-integrity]]
- [[../assumptions|A2]]
- 2025-06-04_v1-balanced-scorecard