---
type: problem
status: emerging
severity: medium
mentions: 3
updated: 2025-06-04
cluster: evidence-workflow
---

# Terminology and cross-referencing overhead

## Statement
The same regulatory concept appears in rules, supervisory statements, reporting instructions, template instructions and policy statements with differing wording and level of detail. Analysts follow references from document to document before they feel comfortable answering, and want related material (definitions, related instructions, relevant changes) surfaced automatically instead of manually discovered.

## Who has it
All analysts; notably visible in template/reporting-field questions where template instructions alone are insufficient.

## Evidence
- "The same concept can appear in a rule, supervisory statement, reporting instruction, template instruction, policy statement or another related document, but the wording and level of detail can differ. Analysts therefore often follow references from one document to another." — Analyst 2 (source: 2025_05_24_meeting_kickoff.md, L13)
- Example: a reporting-template question could not be answered confidently from template instructions alone; the analyst had to check the reporting rule, related definitions and previous regulatory material (source: 2025_05_24_meeting_kickoff.md, L15)
- "If an analyst searches for a particular reporting requirement, it would be helpful to see related definitions, reporting instructions and relevant regulatory changes without having to manually discover every connection." — Analyst 2 (source: 2025_05_24_meeting_kickoff.md, L51)
- Analysts want normal-language questions rather than needing exact source terminology — Analyst 1 (source: 2025_05_24_meeting_kickoff.md, L43)

### From Meeting 2 (2025-05-26)
- Analysts begin with business-question terminology; regulatory material may use a different term, abbreviation or technical definition — Prudential Regulatory SME (source: 2025_05_26_meeting_followup.md, L41)
- Search should find conceptually related material rather than requiring exact keyword match (source: 2025_05_26_meeting_followup.md, L43)
- Counter-risk: "semantic similarity can also be dangerous. Two concepts can sound similar while having materially different regulatory meanings" (source: 2025_05_26_meeting_followup.md, L45); a search for a capital treatment may return provisions for different exposure classes or calculation approaches, and the first semantically similar result is not necessarily the applicable provision (source: 2025_05_26_meeting_followup.md, L47)
- Navigation runs both ways: template → underlying requirement, and rule → reporting representation; there is not always a single starting point — Reporting Change SME (source: 2025_05_26_meeting_followup.md, L63-65)
- Table/template meaning may depend on definitions or instructions elsewhere — see [[non-prose-regulatory-content]]

### From email digest (2025-06-04)
- Natural-language querying confirmed as a core V1 capability, alongside discovery of related/cross-referenced material (source: 2025_06_04_digest_clarifications.md, row 1)

## Contradicting evidence
None recorded.

## Related
- [[source-validation-burden]]
- [[evidence-assembly-time-cost]]
