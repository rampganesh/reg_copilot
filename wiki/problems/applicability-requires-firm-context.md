---
type: problem
status: emerging
severity: high
mentions: 1
updated: 2026-09-09
---

# Applicability Requires Firm Context

## Statement

Determining whether a requirement applies depends on factors beyond the regulatory text alone: "whether a requirement applies can depend on factors such as the legal entity, consolidation perimeter, permissions, reporting regime, type of exposure, reporting basis and relevant date" (L97). The system "should not claim to make definitive applicability decisions unless sufficient structured context and validated rules are available" (L99). **(source: 2025_05_26_meeting_followup.md, L23, L95, L97, L99, L101)**

## Who has it

- **Prudential Regulatory SME**: explicitly warns against automatic applicability (L95, L97, L99)
- **Reporting Change SME**: distinguishes gathering information from making final regulatory determination (L101)
- **Compliance representative**: warns about users copying AI answers into formal documentation (L83, L84)

## Evidence

- **Applicability context complexity**: "applicability is highly dependent on context" (L95)
- **Required context factors**: "whether a requirement applies can depend on factors such as the legal entity, consolidation perimeter, permissions, reporting regime, type of exposure, reporting basis and relevant date" (L97)
- **No definitive decisions in v1**: "the initial product should not claim to make definitive applicability decisions unless sufficient structured context and validated rules are available" (L99)
- **Information gathering vs. determination**: "the system could instead ask the analyst for additional information when applicability is unclear. This could eventually be useful, but the product should distinguish between gathering information and making the final regulatory determination" (L101)
- **Context dependency reinforced**: "applicability is highly dependent on context" (L23)

## Contradicting evidence

None identified from this source. The constraint is explicit.

## Related

- **Open questions**: Q5 (auto-applicability in v1), Q16 (applicability context gathering)
- **Assumptions**: A4 (UK capital reporting viability), A9 (bounded corpus feasibility)
- **Overview**: hard constraints - no automatic applicability