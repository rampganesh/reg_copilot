---
type: problem
status: emerging
severity: medium
mentions: 1
updated: 2026-09-06
---

# Terminology Fragmentation

## Statement

"The same concept can appear in a rule, supervisory statement, reporting instruction, template instruction, policy statement or another related document, but the wording and level of detail can differ. Analysts therefore often follow references from one document to another before they are comfortable answering a question." Users want to "ask a question in normal language" rather than knowing the exact regulatory terminology used in the source document. **(source: 2025_05_24_meeting_kickoff.md, L13, L43)**

## Who has it

- **Analyst 1**: wants to ask questions in normal language (L43)
- **Analyst 2**: explains how the same concept appears in different document types with different wording (L13–L16)
- **Regulatory Change/Reporting SME**: must know the exact regulatory terminology in sources (implicit operational requirement)

## Evidence

- **Cross-document terminology differences**: "The same concept can appear in a rule, supervisory statement, reporting instruction, template instruction, policy statement or another related document, but the wording and level of detail can differ. Analysts therefore often follow references from one document to another before they are comfortable answering a question." **(source: 2025_05_24_meeting_kickoff.md, L13)**
- **Same concept, different document types**: "The analyst had to look at the relevant reporting rule, then check related definitions and previous regulatory material before confirming what the field represented." **(source: 2025_05_24_meeting_kickoff.md, L15)**
- **Normal-language query desire**: "Analyst 1 said that a useful system would allow an analyst to ask a question in normal language rather than having to know the exact regulatory terminology used in the source document." **(source: 2025_05_24_meeting_kickoff.md, L43)**
- **Related material identification**: "Another useful capability would be identifying related material automatically. If an analyst searches for a particular reporting requirement, it would be helpful to see related definitions, reporting instructions and relevant regulatory changes without having to manually discover every connection." **(source: 2025_05_24_meeting_kickoff.md, L51)**

## Contradicting evidence

- **Need for exact terminology**: While users want to ask in normal language, the SME must "know the exact regulatory terminology used in the source document" to interpret correctly — this suggests terminology knowledge is unavoidable, not just a usability feature.
- **No terminology handling decision**: L111 explicitly states no decision on model, retrieval approach, or architecture — terminology translation/normalization is not yet decided.

## Related

- **Open questions**: Q3 (assistance levels), Q4 (material authority distinction), Q10 (normal-language queries)
- **Overview**: research problem complexity, domain scope
