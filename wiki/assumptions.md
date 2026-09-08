---
type: assumptions
updated: 2026-09-06
---

# Assumption Register

All entries `status: untested` — one meeting (self-report) does not provide measurement or correlation. Per AGENTS.md L61–70, distinguish correlation from causation explicitly.

---

## A1: Adoption requires demonstrated time savings

- **statement**: Analysts will adopt the system only if it demonstrably reduces time spent searching and assembling evidence.
- **status**: untested
- **evidence for**:
  - "adoption would depend on whether experienced analysts believe the system saves them time" (L75)
  - "the biggest potential benefit for experienced analysts may therefore be reducing repetitive searching and evidence collection rather than eliminating expert judgement" (L77)
  - "the desired outcome is...to reduce the time analysts spend searching and assembling evidence while maintaining or improving the quality of the resulting answers" (L73)
- **evidence against**: None from this source.
- **history**: 2026-09-06 untested → untested (no new evidence)

**Notes**: This is the manager's own constraint (L75). Adoption measurement would be the first success metric.

---

## A2: Inspectable provenance drives trust more than answer polish

- **statement**: Analysts trust the system when they can inspect where answers come from, more than when answers look polished or complete.
- **status**: untested
- **evidence for**:
  - "Analyst 2 said that...they would be uncomfortable using an AI-generated answer if they could not immediately inspect the supporting source" (L45)
  - "Source references would need to be sufficiently precise. A link to a 300-page policy document would not be enough" (L47)
  - "speed is important, but accuracy and trust are more important for regulatory work. They would rather spend another minute checking an answer than use a fast answer that cannot be verified" (L69)
- **evidence against**: None from this source.
- **history**: 2026-09-06 untested → untested (no new evidence)

**Notes**: Per AGENTS.md L86–89, every claim must cite its source inline; claims without citation labeled `[unsupported]`.
---

## A3: "Insufficient evidence" escalation is preferred over unsupported answers

- **statement**: Analysts prefer the system to explicitly indicate uncertainty when evidence is insufficient, rather than produce a plausible-looking but unsupported answer.
- **status**: untested
- **evidence for**:
  - "Analyst 2 said that they would want to know when the system is uncertain or cannot find adequate evidence. A response such as 'I couldn't find sufficient evidence to answer this' would be preferable to a plausible-looking answer without strong support" (L89)
  - "The manager agreed and said that escalation should be treated as a valid outcome rather than a product failure" (L91)
  - "the team would welcome assistance with finding and organising evidence, but they would not want an AI system to present an uncertain interpretation as a regulatory conclusion" (L37–L39)
- **evidence against**: None from this source.
- **history**: 2026-09-06 untested → untested (no new evidence)

**Notes**: This was explicit agreement between analyst and manager (L89–L91).
---

## A4: UK capital reporting + Basel 3.1 is a viable narrow first domain

- **statement**: Focusing initially on UK capital regulatory reporting with the Basel 3.1 transition is a realistic and implementable domain.
- **status**: untested
- **evidence for**:
  - "the initial product should probably focus on a relatively narrow regulatory domain" (L83)
  - "capital regulatory reporting provides a realistic initial domain because the team is already spending significant effort understanding the changes and their reporting implications" (L85)
  - "initial scope centred on UK capital regulatory reporting and the Basel 3.1 transition" (L109)
- **evidence against**:
  - SME warned that "identifying regulatory changes is useful but determining the downstream impact of a regulatory change on systems, processes, reporting templates and controls is a much larger problem than simply finding the relevant regulatory text" (L61)
  - L111 records "No decision was made...on...MVP feature set, technical architecture, model, retrieval approach..."
- **history**: 2026-09-06 untested → untested (feasibility not established by source)

**Notes**: This assumption is ours, not theirs. The source states the preference for narrow scope, but L61 flags the complexity. Feasibility is unproven.
---

## A5: Two segments (experienced vs. newer analysts) diverge enough to need different product behavior

- **statement**: Experienced analysts and newer analysts have sufficiently different needs that one product behavior cannot effectively serve both.
- **status**: untested
- **evidence for**:
  - "Analyst 1 said that the biggest potential benefit for experienced analysts may therefore be reducing repetitive searching and evidence collection rather than eliminating expert judgement" (L77)
  - "Analyst 2 said that the biggest benefit for less experienced analysts may be helping them understand where to look and giving them a starting point for their research" (L79)
  - "The SME cautioned that these two use cases are related but not identical. A system designed to answer questions for experienced analysts may need to behave differently from one designed to teach newer analysts how to investigate a regulatory issue" (L81)
- **evidence against**:
  - None explicit, but the SME says they're "related but not identical" — not "unrelated" or "contradictory"
  - Manager wants consistency across analysts (L67) which may favor a unified approach
- **history**: 2026-09-06 untested → untested (opinion, not evidence)

**Notes**: This is the SME's **opinion** (L81), not evidence. It's one of the key signals for the Stage 2 persona trigger (AGENTS.md L146) if confirmed by discovery.
---

## A6: Version/effective-date handling is feasible within v1

- **statement**: The system can handle document versioning and effective dates within the first release.
- **status**: untested
- **evidence for**: None from source; this is an assumption.
- **evidence against**: None from source; this is an assumption.
- **history**: 2026-09-06 untested → untested (no evidence either way)

**Notes**: This is our belief, not theirs. The source states that "the product would therefore need to deal with document dates and versions rather than treating the regulatory corpus as a permanently fixed knowledge base" (L87), but says nothing about feasibility. This assumption is **unsupported** per AGENTS.md L88.
---

# Summary

All 6 assumptions remain `status: untested` because:
1. Single-source self-report cannot measure validity
2. No data source has been ingested yet
3. No experiments or correlation has been established

Per AGENTS.md L61–70, distinguish correlation from causation explicitly. A6 is labeled `[unsupported]` because the source doesn't address feasibility.

