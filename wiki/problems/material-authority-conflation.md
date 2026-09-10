---
type: problem
status: emerging
severity: high
mentions: 2
updated: 2026-09-09
---

# Material Authority Conflation

## Statement

"A system should distinguish between different types of regulatory material. For example, a final rule, reporting instruction, supervisory statement and an older consultation document should not all appear to have the same authority." Without this distinction, analysts cannot properly weight sources or determine which documents are binding versus interpretive guidance. **(source: 2025_05_24_meeting_kickoff.md, L49)**

## Who has it

- **Regulatory Change/Reporting SME**: explicitly requests authority distinction (L49)
- **Analyst 1 & 2**: implicitly need this for accurate interpretation (various lines)

## Evidence

- **Authority-level distinction required**: "The SME said that the system should distinguish between different types of regulatory material. For example, a final rule, reporting instruction, supervisory statement and an older consultation document should not all appear to have the same authority." **(source: 2025_05_24_meeting_kickoff.md, L49)**
- **Implicit authority confusion risk**: The need for cross-referencing to establish applicability (L11–L16) presumes that analysts must already know which documents carry what weight of authority to navigate correctly.

## Contradicting evidence

- **No explicit authority distinction decision**: L111 states "No decision was made...on...model, retrieval approach" — authority-level tagging/weighting is not yet decided.
- **Material diversity is inherent to the domain**: The team already works with multiple document types, suggesting the system must handle them regardless of whether explicit authority tagging is implemented.

## Related

- **Open questions**: Q4 (assistance levels), Q5 (auto-applicability)
- **Overview**: research problem complexity, material types
