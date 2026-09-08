---
type: decision
status: active
date: 2025-05-24
decider: Regulatory Reporting Manager
updated: 2026-09-06
---

# Human Review Guardrails

## Context

The manager explicitly stated constraints on what the system should **not** do directly. The team wants an "assistant for regulatory research," not an authoritative decision-maker. **(source: 2025_05_24_meeting_kickoff.md, L37, L39, L71, L95, L97)**

## Options Considered

### Option A: Strict human-in-the-loop for all regulatory outputs

**Evidence for**:
- "the desired outcome is not to replace the regulatory SME. The team wants analysts to reach the SME with better-prepared questions and stronger evidence when escalation is necessary" (L41)
- "the system should not directly submit regulatory returns, change production reporting systems, or make decisions that become part of the bank's regulatory reporting process without human review" (L95)
- "even if the system eventually became capable of more advanced tasks, they would still want the initial version to make it obvious that the analyst remains responsible for reviewing the result" (L97)
- "analysts should regard the system as an **assistant for regulatory research**, not as the final authority on regulatory interpretation" (L71)
- The SME distinguishes "finding information" from "interpreting information" and states the team "would not want an AI system to present an uncertain interpretation as a regulatory conclusion" (L37–L39)

**Evidence against**: None from this source — the constraints were explicit and unanimous.

### Option B: Limited automation without strict human review

**Evidence for**: None from this source.

**Evidence against**:
- L95: "The manager said that the system should not directly submit regulatory returns, change production reporting systems, or make decisions that become part of the bank's regulatory reporting process without human review"
- L71: "assistant for regulatory research, not as the final authority"

## Decision & Rationale

**Decision**: Strict human-in-the-loop guardrails for all outputs entering the bank's regulatory reporting process — **proposed**.

**Rationale**: L37–L39, L41, L71, L95, L97 all converge on the same point: the system is an assistant, not a decision-maker. The manager's explicit statement (L95) prohibits direct submission or system changes without human review.

**Caveat**: No formal decision was recorded in L111 ("No decision was made...on final MVP feature set, technical architecture..."). This captures what was stated, not a formalized decision.

## Reversal Conditions

This decision would be reopened if:
1. The manager explicitly authorizes certain automated outputs that don't enter the regulatory reporting process
2. Discovery shows analysts don't want/require human review for specific output types
3. The regulatory environment changes to permit certain automated decisions

## Related

- **Problem pages**: evidence-assembly-overhead (L33), no-feedback-loop-on-answers (L63)
- **Assumptions**: A2 (provenance > speed), A3 (uncertainty handling)
- **Overview**: Agreed Scope — Research Assistant role
