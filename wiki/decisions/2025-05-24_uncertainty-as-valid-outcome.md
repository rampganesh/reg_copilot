---
type: decision
status: active
date: 2025-05-24
decider: Regulatory Reporting Manager
updated: 2026-09-06
---

# Uncertainty as Valid Outcome

## Context

Analyst 2 stated they would want the system to indicate when it lacks sufficient evidence. The manager agreed that "escalation should be treated as a valid outcome rather than a product failure." **(source: 2025_05_24_meeting_kickoff.md, L89, L91)**

## Options Considered

### Option A: "Insufficient evidence" is a valid system response

**Evidence for**:
- "Analyst 2 said that they would want to know when the system is uncertain or cannot find adequate evidence. A response such as 'I couldn't find sufficient evidence to answer this' would be preferable to a plausible-looking answer without strong support" (L89)
- "The manager agreed and said that escalation should be treated as a valid outcome rather than a product failure" (L91)
- "speed is important, but accuracy and trust are more important for regulatory work. They would rather spend another minute checking an answer than use a fast answer that cannot be verified" (L69)

**Evidence against**:
- None from this source — the preference was explicit and the manager agreed.

### Option B: System should always produce an answer, even if uncertain

**Evidence for**: None from this source.

**Evidence against**:
- L89: "A response such as 'I couldn't find sufficient evidence to answer this' would be preferable to a plausible-looking answer without strong support"
- L69: "accuracy and trust are more important" than speed

## Decision & Rationale

**Decision**: "Insufficient evidence" or "uncertain" responses are valid outcomes — **proposed**.

**Rationale**: L89–L91 record explicit agreement that escalation/uncertainty is a valid system output. This is critical for trust and accuracy, which analysts prioritized over speed (L69).

**Caveat**: No formal decision recorded in L111 ("No decision was made...on...MVP feature set, technical architecture..."). This captures what was stated, not a formalized decision.

## Reversal Conditions

This decision would be reopened if:
1. Discovery shows analysts would rather have an uncertain answer than no answer (contrary to current statements)
2. Measured escalation rate makes the tool non-useful (e.g., 80%+ of queries return "insufficient evidence")
3. Technical constraints prevent implementing uncertainty detection

## Related

- **Problem pages**: evidence-assembly-overhead (L33–L35)
- **Assumptions**: A3 (uncertainty handling preferred over unsupported answers)
- **Overview**: Not Yet Decided — MVP feature set uncertainty
