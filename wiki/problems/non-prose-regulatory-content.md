---
type: problem
status: emerging
severity: medium
mentions: 4
updated: 2025-06-18
cluster: evidence-workflow
---

# Non-prose regulatory content (extractability)

## Statement
Regulatory reporting requirements are not always expressed as simple prose. Much of the operative meaning sits in tables, templates, rows, columns and reporting fields, and the meaning of any one of those may depend on definitions or instructions located elsewhere in the corpus. A system built around prose passages may therefore find that the regulatory text does not contain cleanly extractable, self-contained statements to quote — which also complicates citation, since a "paragraph reference" may not exist for the thing that actually answers the question.

## Who has it
All analysts working with reporting templates and instructions; affects any system component that extracts, quotes or cites regulatory content.

## Evidence
- "Tables and reporting instructions present an additional challenge. Regulatory reporting requirements are not always expressed as simple prose. The meaning of a row, column, field or reporting template may depend on definitions or instructions elsewhere." — Prudential Regulatory SME (source: 2025_05_26_meeting_followup.md, L61)
- Related: template/instruction versioning must match the regulatory material, or an analyst could receive a current rule with an outdated instruction or vice versa — Data/Reporting SME (source: 2025_05_26_meeting_followup.md, L115)
- Related: navigation between reporting representation and underlying requirement runs both directions and does not always have a single starting point — Reporting Change SME (source: 2025_05_26_meeting_followup.md, L63-65)

## Contradicting evidence
None recorded.

## Related
- [[terminology-cross-referencing]]
- [[citation-integrity]]
- [[source-validation-burden]]

### From email digest (2025-06-04)
- The minimum provenance standard explicitly extends to structured material: provenance "may need to identify the specific table, row/field, instruction or template reference" (source: 2025_06_04_digest_clarifications.md, row 4)

### From interviews (2025-06-17/18)
- Analyst 1: for reporting requirements the useful reference may be "a particular table, reporting instruction, field or template reference" — document titles insufficient for material conclusions (source: 2025_06_17_interview_analyst1exp.md, L65)
- Analyst 2: reporting questions may require identifying the specific template, table, row/field, reporting instruction or instructional paragraph (source: 2025_06_18_interview_analyst2prov.md, L63-71); evaluation must test whether the system "correctly handles tables and reporting instructions" (L143)
