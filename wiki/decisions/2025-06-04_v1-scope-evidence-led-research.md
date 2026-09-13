---
type: decision
status: active
date: 2025-06-04
decider: PM (approving consolidated stakeholder responses from the email digest)
updated: 2025-06-04
---

# V1 scope: evidence-led research assistant

## Context
Discovery surfaced multiple candidate directions: regulatory search, question answering, evidence gathering, document comparison, regulatory-change analysis (source: 2025_05_24_meeting_kickoff.md, L105). The manager asked for a distinction between core-research capabilities and attractive extensions (source: 2025_05_24_meeting_kickoff.md, L107); the Prudential SME named "find and connect authoritative regulatory evidence quickly" as the most valuable initial capability (source: 2025_05_26_meeting_followup.md, L153).

## Options considered
1. **Broad regulatory assistant** covering search, change analysis, impact analysis from day one — rejected: "trying to solve every type of regulatory research problem in the first release would make the product too broad" (source: 2025_05_24_meeting_kickoff.md, L53); downstream impact requires internal bank context outside the research problem (source: 2025_05_26_meeting_followup.md, L129).
2. **Narrow evidence-led research core** — stakeholder-consolidated support (source: 2025_06_04_digest_clarifications.md, row 1).

## Decision & rationale
V1 focuses on **finding, connecting, and explaining authoritative evidence**. Core capabilities: authoritative regulatory search; natural-language querying; discovery of related/cross-referenced material; source/version/status awareness; evidence-backed explanations; precise citations; clear indication of uncertainty or insufficient evidence. Deferred extensions: sophisticated "What changed?" analysis; downstream impact analysis; autonomous applicability determination; automated reporting/system changes; internal historical answers as authoritative knowledge. Q&A is core, but the product stays evidence-led rather than becoming an autonomous compliance decision-maker (source: 2025_06_04_digest_clarifications.md, row 1).

## Reversal conditions
- A validated, bounded set of structured context/rules makes autonomous applicability reliable in testing (would reopen scope with strong governance).
- Stakeholders report that manual current/future comparison in V1 blocks the Basel 3.1 transition workflow.
- Evidence of the core not delivering measurable time savings (see scorecard decision) may trigger a scope re-think.

## Related
- [[../open-questions|Q1 (answered)]]
- [[../problems/requirement-applicability-determination]]
- 2025-06-04_temporal-awareness-v1, 2025-06-04_v1-balanced-scorecard