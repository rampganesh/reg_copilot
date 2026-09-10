---
type: assumptions
updated: 2026-09-09
---

# Assumption Register

All entries `status: untested` — one meeting (self-report) does not provide measurement or correlation. Per AGENTS.md L126–L131, distinguish correlation from causation explicitly.

---

## A1: Adoption requires demonstrated time savings

- **statement**: Analysts will adopt the system only if it demonstrably reduces time spent searching and assembling evidence.
- **status**: untested
- **evidence for**:
  - "adoption would depend on whether experienced analysts believe the system saves them time" (source: 2025_05_24_meeting_kickoff.md, L75)
  - "the biggest potential benefit for experienced analysts may therefore be reducing repetitive searching and evidence collection rather than eliminating expert judgement" (L77)
  - "the desired outcome is...to reduce the time analysts spend searching and assembling evidence while maintaining or improving the quality of the resulting answers" (L73)
  - "the most valuable initial capability would likely be to help analysts find and connect authoritative regulatory evidence quickly, while clearly communicating source status, dates and uncertainty" (source: 2025_05_26_meeting_followup.md, L153)
  - "a successful assistant should make an analyst's research process faster without making the analyst less critical of the result" (L155)
- **evidence against**: None from these sources.
- **history**: 2026-09-06 untested → untested (no new evidence; 2026-09-09 added L153, L155)

**Notes**: This is the manager's own constraint (L75). Adoption measurement would be the first success metric. L149 (source 2) suggests tracking analysts who ignore the answer as the first testable proxy.

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
  - "Analyst 2 said that they would want to know when the system is uncertain or cannot find adequate evidence. A response such as 'I couldn't find sufficient evidence to answer this' would be preferable to a plausible-looking answer without strong support" (source: 2025_05_24_meeting_kickoff.md, L89)
  - "The manager agreed and said that escalation should be treated as a valid outcome rather than a product failure" (L91)
  - "the team would welcome assistance with finding and organising evidence, but they would not want an AI system to present an uncertain interpretation as a regulatory conclusion" (L37–L39)
  - "an answer that refuses unnecessarily can also reduce usefulness" (source: 2025_05_26_meeting_followup.md, L141) — *partial counterbalance*
  - "the first requirement should be to expose the conflict rather than silently resolve it" (L67)
  - "a safer first capability would be to identify situations where the available evidence is insufficient, conflicting, ambiguous or clearly associated with different effective dates" (L75)
  - "'I don't have sufficient evidence to answer this' should be considered an acceptable system outcome" (L77)
- **evidence against**:
  - "an answer that refuses unnecessarily can also reduce usefulness" (L141) — suggests the system must balance conflict exposure with responsiveness
- **history**: 2026-09-06 untested → untested (no new evidence; 2026-09-09 added L67, L75, L77, L141)

**Notes**: This was explicit agreement between analyst and manager (L89–L91). L141 introduces the first signal that unnecessary refusal can reduce usefulness, suggesting the real requirement is a balance, not a hard preference.
---

## A4: UK capital reporting + Basel 3.1 is a viable narrow first domain

- **statement**: Focusing initially on UK capital regulatory reporting with the Basel 3.1 transition is a realistic and implementable domain.
- **status**: untested
- **evidence for**:
  - "the initial product should probably focus on a relatively narrow regulatory domain" (source: 2025_05_24_meeting_kickoff.md, L83)
  - "capital regulatory reporting provides a realistic initial domain because the team is already spending significant effort understanding the changes and their reporting implications" (L85)
  - "initial scope centred on UK capital regulatory reporting and the Basel 3.1 transition" (L109)
  - "downstream impact analysis is even further removed from simple regulatory research. Determining which internal systems, controls, processes or reports are affected would require access to internal bank information and business context that is outside the initial regulatory research problem" (source: 2025_05_26_meeting_followup.md, L129)
  - "the Reporting Manager agreed that this should not be assumed to be part of the first product" (L131) — *removes a major complexity*
  - "attempting to ingest everything associated with the PRA would create unnecessary complexity" (L109)
- **evidence against**:
  - SME warned that "identifying regulatory changes is useful but determining the downstream impact of a regulatory change on systems, processes, reporting templates and controls is a much larger problem than simply finding the relevant regulatory text" (source: 2025_05_24_meeting_kickoff.md, L61)
  - L111 records "No decision was made...on...MVP feature set, technical architecture, model, retrieval approach..."
  - "The regulatory material is not static. New clarifications, amendments and related publications can appear after an analyst has already performed research" (source: 2025_05_24_meeting_kickoff.md, L87) — *tension with bounded corpus*
- **history**: 2026-09-06 untested → untested (feasibility not established by source; 2026-09-09 added L129, L131, L109, L87)

**Notes**: This assumption is ours, not theirs. The source states the preference for narrow scope, but L61 flags the complexity. Feasibility is unproven. L129–L131 removes downstream impact analysis from v1, improving feasibility. L87 introduces tension with bounded corpus maintenance.
---

## A5: Two segments (experienced vs. newer analysts) diverge enough to need different product behavior

- **statement**: Experienced analysts and newer analysts have sufficiently different needs that one product behavior cannot effectively serve both.
- **status**: untested
- **evidence for**:
  - "the biggest potential benefit for experienced analysts may therefore be reducing repetitive searching and evidence collection rather than eliminating expert judgement" (source: 2025_05_24_meeting_kickoff.md, L77)
  - "the biggest benefit for less experienced analysts may be helping them understand where to look and giving them a starting point for their research" (L79)
  - "The SME cautioned that these two use cases are related but not identical. A system designed to answer questions for experienced analysts may need to behave differently from one designed to teach newer analysts how to investigate a regulatory issue" (L81)
- **evidence against**:
  - None explicit, but the SME says they're "related but not identical" — not "unrelated" or "contradictory"
  - Manager wants consistency across analysts (L67) which may favor a unified approach
  - Source 2 introduces a **competing divergence axis**: L143–L145 suggest divergence may be driven by **question ambiguity**, not user seniority. "for straightforward factual retrieval and source identification, consistency should be high. For ambiguous interpretation, the appropriate behaviour may instead be to surface the relevant evidence and identify the ambiguity"
- **history**: 2026-09-06 untested → untested (no new evidence; 2026-09-09 added L143, L145)

**Notes**: This is the SME's opinion (L81), not evidence. It's one of the key signals for the Stage 2 persona trigger (AGENTS.md L191) if confirmed by discovery. Source 2's L143–L145 introduces question ambiguity as a potentially more significant divergence factor than seniority.
---

## A6: Version/effective-date handling is feasible within v1

- **statement**: The system can handle document versioning and effective dates within the first release.
- **status**: untested
- **evidence for**:
  - "effective dates should be treated as first-class information rather than something an analyst has to infer from a document's publication date" (source: 2025_05_26_meeting_followup.md, L25)
  - "the system should ideally be able to show the regulatory basis for its answer and make clear when the evidence relates to a future or historical state" (L31)
  - "each source should ideally have metadata such as publication date, effective date where applicable, document type, subject area, version/status and relationships to other regulatory material" (L113)
  - "reporting templates and instructions need to be versioned alongside the relevant regulatory material. Otherwise an analyst could receive a current rule with an outdated reporting instruction or vice versa" (L115)
  - "document versioning should be visible to users when it materially affects the answer" (L117)
- **evidence against**: None from source; this is an assumption.
- **history**: 2026-09-06 untested → untested (no evidence either way; 2026-09-09 added L25, L31, L113, L115, L117)

**Notes**: This is our belief, not theirs. The source states that "the product would therefore need to deal with document dates and versions rather than treating the regulatory corpus as a permanently fixed knowledge base" (source: 2025_05_24_meeting_kickoff.md, L87), but says nothing about feasibility. This assumption is **unsupported** per AGENTS.md L129–L130. However, source 2 provides a clear specification of the *requirements* (L25, L113, L115, L117) while L99/L121 remain caution signals. Feasibility remains unproven.

---

## A7: PRA material exposes effective-date/version/status metadata in extractable form

- **statement**: The PRA (and related regulatory bodies) publish regulatory material with metadata (publication date, effective date, version/status, document type) in a form that can be reliably extracted and maintained by an automated system.
- **status**: untested
- **evidence for**:
  - "each source should ideally have metadata such as publication date, effective date where applicable, document type, subject area, version/status and relationships to other regulatory material" (source: 2025_05_26_meeting_followup.md, L113)
  - "reporting templates and instructions need to be versioned alongside the relevant regulatory material" (L115)
- **evidence against**: None from source; metadata is specified as a requirement, not as an existing fact.
- **history**: 2026-09-09 untested → untested (new assumption; tests A6 feasibility)

**Notes**: This assumption is load-bearing for A6. The requirement is clear (L113), but nothing establishes the metadata actually exists in extractable form. Tested by Q18.

---

## A8: Analysts will supply structured feedback if the taxonomy is right

- **statement**: Given a well-designed feedback taxonomy, analysts will voluntarily provide structured feedback about answer quality and error types.
- **status**: untested
- **evidence for**:
  - "the SME said that a feedback mechanism would be valuable, provided that a correction can be associated with the underlying question, answer, evidence and version of the regulatory material used at the time" (source: 2025_05_26_meeting_followup.md, L85)
  - "simply recording a thumbs-up or thumbs-down would probably not provide enough information to improve regulatory research quality. More useful feedback categories could distinguish between an incorrect answer, insufficient evidence, incorrect source, outdated source, irrelevant source and a correct but poorly explained answer" (L87)
  - "the analysts agreed that the ability to report 'this source is relevant but the answer missed an important qualification' would be useful" (L89)
  - "the SME supported this but said that feedback should be structured enough to identify why an answer was considered poor" (L147)
- **evidence against**:
  - "the SME also recommended tracking cases where analysts ignored the AI answer and performed the research manually. Those cases could reveal important product shortcomings even if the analyst did not formally submit negative feedback" (L149) — implies voluntary feedback is insufficient
- **history**: 2026-09-09 untested → untested (new assumption; highlights tension between voluntary feedback and passive tracking)

**Notes**: L85–L89, L147 for; L149 against. The SME explicitly recommends tracking analysts who ignore the answer, suggesting voluntary feedback alone is insufficient.

---

## A9: A deliberately bounded corpus can stay bounded in a non-static domain

- **statement**: It is feasible to define and maintain a bounded corpus (UK capital reporting + Basel 3.1) with explicit inclusion/exclusion criteria despite the non-static nature of regulatory material.
- **status**: untested
- **evidence for**:
  - "the SME recommended beginning with a deliberately defined corpus relating to UK capital regulatory reporting and the Basel 3.1 implementation, with explicit inclusion and exclusion criteria" (source: 2025_05_26_meeting_followup.md, L111)
  - "attempting to ingest everything associated with the PRA would create unnecessary complexity" (L109)
- **evidence against**:
  - "The regulatory material is not static. New clarifications, amendments and related publications can appear after an analyst has already performed research" (source: 2025_05_24_meeting_kickoff.md, L87)
- **history**: 2026-09-09 untested → untested (new assumption; tension between bounded corpus requirement and non-static domain)

**Notes**: This assumption is tested by Q17 (who owns corpus maintenance). The requirement is clear (L111), but the tension with L87 remains unresolved.
---

# Summary

All 9 assumptions remain `status: untested` because:
1. Single-source self-report cannot measure validity
2. No data source has been ingested yet
3. No experiments or correlation has been established

Per AGENTS.md L126–L131, distinguish correlation from causation explicitly. A6 is labeled `[unsupported]` because the source doesn't address feasibility.

