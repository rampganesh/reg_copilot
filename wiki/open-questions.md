---
type: open-questions
status: open
updated: 2026-09-09
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
- **Status**: open

**Context**: "the system should distinguish between different types of regulatory material. For example, a final rule, reporting instruction, supervisory statement and an older consultation document should not all appear to have the same authority" (L49).

**Why it matters**: Authority conflation could lead analysts to treat interpretive guidance as binding requirements, or vice versa.

---

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


## Q12: Should the system model inter-source relationships rather than applying a linear authority ranking?

- **Tag**: ask-stakeholder
- **Origin**: 2025_05_26_meeting_followup.md, L33, L35, L37
- **Status**: open

**Context**: "the relationship is not always reducible to a simple ranking such as 'Rulebook always wins'" (L33); "a reporting instruction may answer a question that a high-level rule does not answer. Conversely, a reporting template instruction should not be interpreted in isolation if understanding the underlying prudential requirement is necessary" (L35); "a useful AI assistant would therefore need to understand relationships between sources, not simply assign a universal authority score to every document" (L37).

**Why it matters**: If authority is relational rather than hierarchical, the system's retrieval and ranking logic must fundamentally change.

---

## Q13: Should the system warn when semantically similar provisions may have materially different regulatory meanings?

- **Tag**: run-experiment
- **Origin**: 2025_05_26_meeting_followup.md, L45, L47
- **Status**: open

**Context**: "the SME cautioned that semantic similarity can also be dangerous. Two concepts can sound similar while having materially different regulatory meanings" (L45); "a search system might return several apparently relevant provisions covering different exposure classes or calculation approaches. The system should not imply that the first semantically similar result is necessarily the applicable provision" (L47).

**Why it matters**: Over-reliance on semantic similarity could lead to false positives and incorrect applicability determinations.

---

## Q14: Where is the line between justified and unnecessary refusal, and how is it measured?

- **Tag**: run-experiment
- **Origin**: 2025_05_26_meeting_followup.md, L137, L139, L141
- **Status**: open

**Context**: "an answer that refuses unnecessarily can also reduce usefulness" (L141); "an evaluation containing only straightforward questions would give a misleading impression of product quality" (L137); "evaluation should include the risk of confidently wrong answers, not just whether the system produces an answer" (L139).

**Why it matters**: This is the signal that decision 3's reversal condition 1 may be partially triggered — balancing "insufficient evidence" with usefulness requires measurement.
## Q6: Should we build a feedback loop to capture which sources ultimately resolved questions?

- **Tag**: ask-users
- **Origin**: 2025_05_24_meeting_kickoff.md, L63, L65
- **Status**: open

**Context**: "The team currently has no consistent way of recording whether an answer produced by previous research was useful, whether it was subsequently corrected, or which source ultimately resolved the question" (L63). "Analysts sometimes discover after several weeks that a previous answer was based on an outdated document or incomplete interpretation. There is no systematic feedback mechanism for capturing this information" (L65).

**Why it matters**: Without feedback, the system cannot learn from corrections or improve over time. Consistency improvement (L67) presupposes tracking.


## Q15: What is the achievable citation granularity without fabrication, and how is fabrication detected?

- **Tag**: check-data
- **Origin**: 2025_05_26_meeting_followup.md, L49, L51, L53, L55
- **Status**: open

**Context**: "citations need to allow an analyst to independently verify the answer. A generic document link is useful but insufficient for a high-confidence research workflow" (L49); "the analysts said that they would ideally want the citation to identify the document, relevant section or paragraph, and enough surrounding context to understand how the cited text supports the answer" (L51); "the system should not manufacture paragraph numbers, section references or quotations when the source does not contain them" (L53); "an incorrect citation may be worse than no citation because it creates a false impression of auditability" (L55).

**Why it matters**: Fabricated citations destroy trust and auditability; the system needs detection mechanisms.

---

## Q16: What is the optimal excerpt size before context becomes cumbersome?

- **Tag**: run-experiment
- **Origin**: 2025_05_26_meeting_followup.md, L57, L59
- **Status**: open

**Context**: "quoting also need to preserve context. Extracting a single sentence from a paragraph can sometimes remove an important qualification, exception or condition" (L57); "the better objective would be to give the analyst enough surrounding material to validate the claim without requiring them to search the entire document again" (L59).

**Why it matters**: Too little context removes qualifications; too much makes answers cumbersome.

## Q17: Who owns corpus inclusion/exclusion criteria and metadata upkeep?

- **Tag**: ask-stakeholder
- **Origin**: 2025_05_26_meeting_followup.md, L111, L113, L115
- **Status**: open

**Context**: "the SME recommended beginning with a deliberately defined corpus relating to UK capital regulatory reporting and the Basel 3.1 implementation, with explicit inclusion and exclusion criteria" (L111); "each source should ideally have metadata such as publication date, effective date where applicable, document type, subject area, version/status and relationships to other regulatory material" (L113); "reporting templates and instructions need to be versioned alongside the relevant regulatory material" (L115).

**Why it matters**: A bounded corpus in a non-static domain requires ongoing governance; unclear ownership creates drift.

---

## Q18: Do PRA documents actually expose extractable effective-date/version metadata?

- **Tag**: check-data
- **Origin**: 2025_05_26_meeting_followup.md, L25, L113, L117
- **Status**: open

**Context**: "effective dates should be treated as first-class information rather than something an analyst has to infer from a document's publication date" (L25); "each source should ideally have metadata such as publication date, effective date where applicable, document type, subject area, version/status and relationships to other regulatory material" (L113); "document versioning should be visible to users when it materially affects the answer" (L117).

**Why it matters**: Tests assumption A7 — the requirement is specified, but does the metadata actually exist in extractable form?

## Q19: Should internal prior answers be stored at all given retention/ownership/reliance concerns?

- **Tag**: ask-stakeholder
- **Origin**: 2025_05_26_meeting_followup.md, L79, L81, L83, L151
- **Status**: open

**Context**: "historical internal answers can be useful evidence of how the organisation has previously interpreted a question, but they should not automatically be treated as regulatory authority" (L79); "an internal answer should ideally be labelled separately from an external regulatory source, especially if the answer represents a judgement rather than a direct statement from the regulator" (L81); "this distinction is particularly important if users begin copying AI-generated answers into formal reporting documentation or communications" (L83); "this would raise additional considerations around data retention, ownership and potential reliance, and should not be assumed as part of the initial design" (L151).

**Why it matters**: Balancing learning capability against data governance risks.

---

## Q20: How should the system represent bidirectional template↔rule navigation?

- **Tag**: desk-research
- **Origin**: 2025_05_26_meeting_followup.md, L61, L63, L65
- **Status**: open

**Context**: "analysts sometimes start with a reporting template and work backwards to the underlying regulatory requirement. In other cases, they start from a regulatory rule and work forward to understand how the requirement is represented in reporting" (L63); "both directions of navigation are useful and that the product should not assume there is always a single starting point" (L65).

**Why it matters**: Navigation patterns affect the information architecture and user interface.

## Q21: What interface wording conventions separate "applicable requirement is" from "relevant sources indicate"?

- **Tag**: ask-stakeholder
- **Origin**: 2025_05_26_meeting_followup.md, L39, L105, L107
- **Status**: open

**Context**: "the product should avoid language such as 'the regulation says' when the evidence is actually a supervisory statement, explanatory publication or internal interpretation" (L39); "a statement such as 'The applicable requirement is...' is materially different from 'The relevant sources indicate...' followed by evidence and a clear caveat" (L105); "users should not have to interpret a model's confidence score to understand whether an answer is trustworthy. Trust should come primarily from transparent evidence, source status, date information and appropriate escalation" (L107).

**Why it matters**: Interface language directly impacts analyst trust and regulatory compliance.

---

## Q22: How should the system define "current" vs "future" requirement modes given L121's caution?

- **Tag**: ask-stakeholder
- **Origin**: 2025_05_26_meeting_followup.md, L19, L121, L123
- **Status**: open

**Context**: "the transition creates a particularly difficult research environment because analysts may simultaneously encounter requirements relating to the existing framework and requirements that will apply from 1 January 2027" (L19); "the group discussed whether the product should provide a 'current requirement' mode and a 'future requirement' mode. The SME said that this could be useful, but the terminology and behaviour would need to be carefully defined" (L121); "users may also want to investigate how a requirement evolved over time. Historical comparison is useful for regulatory change work, but it should not be confused with determining the current reporting obligation" (L123).

**Why it matters**: Modes must be clearly distinguished to avoid operational errors.

---

## Q23: Does a bounded corpus need change detection, and is "What changed?" in or out of v1?

- **Tag**: ask-stakeholder
- **Origin**: 2025_05_26_meeting_followup.md, L125, L127, L161
- **Status**: open

**Context**: "the Reporting Manager asked about 'What changed?' as a potential capability. The SME said that identifying textual changes between two documents is relatively different from determining the regulatory significance of those changes. The latter requires understanding context and applicability" (L125); "an automated change comparison could therefore be useful as research support, but the product should not imply that a textual difference automatically represents a change in the firm's obligation" (L127); "No final decision was made during the meeting on the MVP feature set, source hierarchy algorithm, technical architecture, model choice, retrieval method, evaluation thresholds, governance approval process or implementation timeline" (L161).

**Why it matters**: Change detection is useful but requires clear boundaries on regulatory significance.

---

## Q24: Is divergence driven by user seniority or by question-ambiguity type?

- **Tag**: ask-users
- **Origin**: 2025_05_26_meeting_followup.md, L143, L145 vs 2025_05_24_meeting_kickoff.md, L81
- **Status**: open

**Context**: "for straightforward factual retrieval and source identification, consistency should be high. For ambiguous interpretation, the appropriate behaviour may instead be to surface the relevant evidence and identify the ambiguity" (L143); "not every question should have a single expected natural-language answer" (L145); "The SME cautioned that these two use cases are related but not identical. A system designed to answer questions for experienced analysts may need to behave differently from one designed to teach newer analysts how to investigate a regulatory issue" (L81).

**Why it matters**: Determines whether persona-based behavior (Stage 2 personas trigger) or question-type-based behavior is the right design axis.