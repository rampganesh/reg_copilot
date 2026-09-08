---
type: open-questions
status: open
updated: 2026-09-06
---

# Open Questions Queue

## Q1: Can we automate cross-referencing to identify the right source?

- **Tag**: ask-users
- **Origin**: 2025_05_24_meeting_kickoff.md, L11–L17
- **Status**: open

**Context**: "finding the first potentially relevant document is generally not the hardest part. The difficulty is establishing that the document is actually the **right source**, that it is applicable to the question being asked, and that it has not been superseded by a later publication" (L11). The SME adds that cross-referencing is "particularly important during a regulatory transition" (L17).

**Why it matters**: If a system could identify the right source, analysts would save significant time. Without it, the core problem remains unsolved.

## Q2: How should we handle document versioning and effective dates?

- **Tag**: check-data
- **Origin**: 2025_05_24_meeting_kickoff.md, L17, L19, L87
- **Status**: open

**Context**: "An answer that is technically correct but refers to a requirement that is not yet applicable can still be operationally wrong" (L19). The corpus "is not static" — "New clarifications, amendments and related publications can appear after an analyst has already performed research" (L87). The Basel 3.1 transition adds complexity (L17, L55).

**Why it matters**: Failure to handle versioning leads to operational errors, not just research inefficiency.

## Q3: What level of assistance is needed — finding, interpreting, or both?

- **Tag**: ask-users
- **Origin**: 2025_05_24_meeting_kickoff.md, L37–L39, L41
- **Status**: open

**Context**: "the distinction between **finding information** and **interpreting information** is important. The team would welcome assistance with finding and organising evidence, but they would not want an AI system to present an uncertain interpretation as a regulatory conclusion" (L37–L39). Desired outcome: "analysts to reach the SME with better-prepared questions and stronger evidence" (L41).

**Why it matters**: Determining whether the system should just find/organize or also provide guidance on interpretation affects the scope dramatically.

## Q4: Should we distinguish material authority levels (final rule vs. reporting instruction vs. consultation document)?

- **Tag**: ask-stakeholder
- **Origin**: 2025_05_24_meeting_kickoff.md, L49
## Q7: How should we handle a non-static regulatory corpus?

- **Tag**: check-data
- **Origin**: 2025_05_24_meeting_kickoff.md, L87
- **Status**: open

**Context**: "The regulatory material is not static. New clarifications, amendments and related publications can appear after an analyst has already performed research. The product would therefore need to deal with document dates and versions rather than treating the regulatory corpus as a permanently fixed knowledge base" (L87).

**Why it matters**: A static corpus assumption breaks the model when the domain itself changes regularly.

## Q8: What success metrics should we use given that "no decision was made" on evaluation methodology?

- **Tag**: ask-stakeholder
- **Origin**: 2025_05_24_meeting_kickoff.md, L111
- **Status**: open

**Context**: "No decision was made during the meeting on the final MVP feature set, technical architecture, model, retrieval approach, implementation timeline or success metrics" (L111). Manager wants to "improve consistency between analysts" (L67) and "reduce the time analysts spend searching and assembling evidence while maintaining or improving the quality of the resulting answers" (L73).

**Why it matters**: Without defined success metrics, we cannot measure whether any solution works.

## Q9: Should we treat experienced vs. newer analysts as divergent segments needing different product behavior?

- **Tag**: ask-users
- **Origin**: 2025_05_24_meeting_kickoff.md, L75–L81
- **Status**: open

**Context**: "Analyst 1 said that the biggest potential benefit for experienced analysts may therefore be reducing repetitive searching and evidence collection rather than eliminating expert judgement" (L77). "Analyst 2 said that the biggest benefit for less experienced analysts may be helping them understand where to look and giving them a starting point for their research" (L79). The SME "cautioned that these two use cases are related but not identical. A system designed to answer questions for experienced analysts may need to behave differently from one designed to teach newer analysts how to investigate a regulatory issue" (L81).

**Why it matters**: If segments diverge enough, a single product may not serve both well. This is the Stage 2 persona trigger (AGENTS.md L146) if confirmed.

## Q10: Should we support normal-language queries that map to exact regulatory terminology?

- **Tag**: ask-users
- **Origin**: 2025_05_24_meeting_kickoff.md, L43, L47
- **Status**: open

**Context**: "Analyst 1 said that a useful system would allow an analyst to ask a question in normal language rather than having to know the exact regulatory terminology used in the source document" (L43). Source references must be "sufficiently precise" — "A link to a 300-page policy document would not be enough" (L47).

**Why it matters**: Natural-language-to-terminology mapping is a significant capability that affects model selection and retrieval approach.

## Q11: Can we handle Basel 3.1's complexity within a narrow first domain?

- **Tag**: desk-research
- **Origin**: 2025_05_24_meeting_kickoff.md, L5, L83, L85, L109, L111
- **Status**: open

**Context**: The team is "preparing for the transition to the Basel 3.1 framework, with the largest operational changes expected around the 1 January 2027 implementation date" (L5). "the initial product should probably focus on a relatively narrow regulatory domain" (L83), and "capital regulatory reporting provides a realistic initial domain" (L85). The initial scope is "centred on UK capital regulatory reporting and the Basel 3.1 transition" (L109).

**Why it matters**: Feasibility is uncertain — the SME warned that "identifying regulatory changes is useful but determining the downstream impact of a regulatory change on systems, processes, reporting templates and controls is a much larger problem" (L61).

- **Status**: open

**Context**: "the system should distinguish between different types of regulatory material. For example, a final rule, reporting instruction, supervisory statement and an older consultation document should not all appear to have the same authority" (L49).

**Why it matters**: Authority conflation could lead analysts to treat interpretive guidance as binding requirements, or vice versa.

## Q5: Should we include auto-applicability determination in v1?

- **Tag**: ask-stakeholder
- **Origin**: 2025_05_24_meeting_kickoff.md, L93
- **Status**: open

**Context**: "The manager said that the system should not directly submit regulatory returns, change production reporting systems, or make decisions that become part of the bank's regulatory reporting process without human review" (L95). On applicability: "The group did not agree that this should be treated as an automatic decision in the first version" (L93).

**Why it matters**: The group explicitly "did not agree" on this — it's an absence of decision, not a negative decision.

## Q6: Should we build a feedback loop to capture which sources ultimately resolved questions?

- **Tag**: ask-users
- **Origin**: 2025_05_24_meeting_kickoff.md, L63, L65
- **Status**: open

**Context**: "The team currently has no consistent way of recording whether an answer produced by previous research was useful, whether it was subsequently corrected, or which source ultimately resolved the question" (L63). "Analysts sometimes discover after several weeks that a previous answer was based on an outdated document or incomplete interpretation. There is no systematic feedback mechanism for capturing this information" (L65).

**Why it matters**: Without feedback, the system cannot learn from corrections or improve over time. Consistency improvement (L67) presupposes tracking.
