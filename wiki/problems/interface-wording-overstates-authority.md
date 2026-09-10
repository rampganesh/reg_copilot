---
type: problem
status: emerging
severity: medium
mentions: 1
updated: 2026-09-09
---

# Interface Wording Overstates Authority

## Statement

Interface language like "The applicable requirement is..." materially differs from "The relevant sources indicate..." followed by evidence and caveats. "The compliance representative said that the product should avoid language such as 'the regulation says' when the evidence is actually a supervisory statement, explanatory publication or internal interpretation" (L39); "a statement such as 'The applicable requirement is...' is materially different from 'The relevant sources indicate...' followed by evidence and a clear caveat" (L105). **(source: 2025_05_26_meeting_followup.md, L29, L39, L81, L83, L105, L107)**

## Who has it

- **Compliance representative**: explicitly warns against overstating authority (L39, L83, L84, L93, L105, L157)
- **Prudential Regulatory SME**: requires transparent evidence and source status (L31, L107)
- **Analysts**: need to understand the distinction between external regulatory sources and internal interpretations (L79, L81, L83)

## Evidence

- **Avoid "the regulation says"**: "the product should avoid language such as 'the regulation says' when the evidence is actually a supervisory statement, explanatory publication or internal interpretation" (L39)
- **Interface wording matters**: "a statement such as 'The applicable requirement is...' is materially different from 'The relevant sources indicate...' followed by evidence and a clear caveat" (L105)
- **Distinguish source types**: "an internal answer should ideally be labelled separately from an external regulatory source, especially if the answer represents a judgement rather than a direct statement from the regulator" (L81)
- **No model confidence scores**: "users should not have to interpret a model's confidence score to understand whether an answer is trustworthy. Trust should come primarily from transparent evidence, source status, date information and appropriate escalation" (L107)
- **No overstatement in copying**: "this distinction is particularly important if users begin copying AI-generated answers into formal reporting documentation or communications" (L83)
- **Support human judgment**: "the product should support human judgement rather than obscure it" (L157)

## Contradicting evidence

None identified from this source. The constraint is explicit.

## Related

- **Open questions**: Q21 (interface wording conventions)
- **Assumptions**: A2 (inspectable provenance), A7 (metadata availability)
- **Overview**: hard constraints - no confidence scores, interface wording