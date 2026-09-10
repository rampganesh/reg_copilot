---
type: problem
status: emerging
severity: high
mentions: 1
updated: 2026-09-09
---

# Citation Integrity Risk

## Statement

Fabricated or context-stripped citations create a false impression of auditability. "A generic document link is useful but insufficient for a high-confidence research workflow" (L49); "the system should not manufacture paragraph numbers, section references or quotations when the source does not contain them" (L53); "an incorrect citation may be worse than no citation because it creates a false impression of auditability" (L55). **(source: 2025_05_26_meeting_followup.md, L49, L51, L53, L55)**

## Who has it

- **Compliance representative**: explicitly warns against fabricated citations (L55, L83, L93)
- **Prudential Regulatory SME**: requires citations that allow independent verification (L49, L51)
- **Analysts**: want citations with document, section/paragraph, and surrounding context (L51)

## Evidence

- **Citation granularity requirements**: "citations need to allow an analyst to independently verify the answer. A generic document link is useful but insufficient for a high-confidence research workflow" (L49)
- **Citation context needs**: "the analysts said that they would ideally want the citation to identify the document, relevant section or paragraph, and enough surrounding context to understand how the cited text supports the answer" (L51)
- **No fabrication rule**: "the system should not manufacture paragraph numbers, section references or quotations when the source does not contain them" (L53)
- **Risk of false auditability**: "an incorrect citation may be worse than no citation because it creates a false impression of auditability" (L55)
- **Context preservation**: "quoting also need to preserve context. Extracting a single sentence from a paragraph can sometimes remove an important qualification, exception or condition" (L57)
- **Excerpt size balance**: "the better objective would be to give the analyst enough surrounding material to validate the claim without requiring them to search the entire document again" (L59)

## Contradicting evidence

None identified from this source. The risk is described as operational reality.

## Related

- **Open questions**: Q15 (citation granularity), Q16 (excerpt size)
- **Assumptions**: A2 (inspectable provenance)
- **Overview**: hard constraints - no fabricated citations