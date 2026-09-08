# Meeting 2 — Regulatory / Prudential SME Discovery Notes

## Discussion Points

* The Regulatory Reporting Manager opened by explaining that the purpose of the session was to understand how regulatory experts establish whether an answer is reliable, particularly in the context of the UK Basel 3.1 implementation, and to identify which parts of that process could reasonably be supported by an AI assistant.

* The Prudential Regulatory SME said that the first mistake to avoid is treating "the PRA website" as a single source of truth. There are different types of regulatory material with different purposes, status and authority. An analyst needs to understand what type of document they are looking at before relying on it.

* The SME described the main sources encountered by the reporting team as the PRA Rulebook, policy statements, supervisory statements, reporting instructions and templates, and other PRA publications. Basel material and other explanatory material may also be useful for understanding the background, but should not automatically be treated as the operative UK requirement.

* The SME said that a search result containing the correct terminology does not necessarily mean that the result provides the correct answer. The system would need to distinguish between material that explains a policy decision, material that establishes a requirement, material that provides reporting instructions, and material that is historical or superseded.

* The Compliance representative added that consultation papers are particularly important to distinguish from final requirements. A consultation may contain language that looks almost identical to a final rule, but it represents a proposal rather than necessarily the requirement that firms ultimately have to follow.

* The SME said that the same issue applies to older policy statements or previous versions of reporting instructions. Historical material can be extremely useful for understanding why a requirement exists, but it should not be presented as though it were the current requirement.

* The SME said that "latest document" is also not necessarily equivalent to "applicable requirement". A newer publication can discuss a future implementation date, while an older requirement may remain applicable until that date.

* The group discussed the Basel 3.1 implementation timeline. The SME said that the transition creates a particularly difficult research environment because analysts may simultaneously encounter requirements relating to the existing framework and requirements that will apply from 1 January 2027.

* The SME said that an answer to a regulatory question should therefore ideally establish at least three things: what requirement is being discussed, which version or period it relates to, and whether it is applicable to the question being asked.

* The Reporting Change SME asked whether the AI system could simply prioritise the newest PRA document. The Prudential SME said that this would be unsafe. A newer document may amend only part of an existing requirement, may have a future effective date, or may apply only to a particular population or reporting context.

* The SME said that effective dates should be treated as first-class information rather than something an analyst has to infer from a document's publication date.

* The SME gave an example of a situation where an analyst finds a final Basel 3.1 policy statement and assumes that the new requirement applies immediately. The analyst may then produce a technically accurate description of the future requirement but an incorrect answer to a question about the firm's current reporting obligation.

* The Compliance representative said that this is one reason they would be uncomfortable with an AI system simply producing an answer with a confidence score. A high-confidence model output does not establish regulatory applicability.

* The SME said that the system should ideally be able to show the regulatory basis for its answer and make clear when the evidence relates to a future or historical state.

* Analyst 1 asked whether the system should automatically determine the hierarchy between regulatory documents. The SME said that there is a hierarchy in the sense that some material has a different regulatory status or purpose from other material, but the relationship is not always reducible to a simple ranking such as "Rulebook always wins."

* The SME explained that a reporting instruction may answer a question that a high-level rule does not answer. Conversely, a reporting template instruction should not be interpreted in isolation if understanding the underlying prudential requirement is necessary.

* The SME said that a useful AI assistant would therefore need to understand **relationships between sources**, not simply assign a universal authority score to every document.

* The Compliance representative said that the product should avoid language such as "the regulation says" when the evidence is actually a supervisory statement, explanatory publication or internal interpretation.

* The SME said that terminology is another significant problem. Analysts often begin with the terminology used in a business question, whereas the regulatory material may use a different term, abbreviation or more technical definition.

* The SME said that a useful search system should therefore be capable of finding conceptually related material rather than requiring an exact keyword match.

* However, the SME cautioned that semantic similarity can also be dangerous. Two concepts can sound similar while having materially different regulatory meanings.

* The group discussed the example of an analyst searching for a particular capital treatment. The SME said that a search system might return several apparently relevant provisions covering different exposure classes or calculation approaches. The system should not imply that the first semantically similar result is necessarily the applicable provision.

* The SME said that citations need to allow an analyst to independently verify the answer. A generic document link is useful but insufficient for a high-confidence research workflow.

* The analysts said that they would ideally want the citation to identify the document, relevant section or paragraph, and enough surrounding context to understand how the cited text supports the answer.

* The SME agreed but said that the system should not manufacture paragraph numbers, section references or quotations when the source does not contain them.

* The Compliance representative said that an incorrect citation may be worse than no citation because it creates a false impression of auditability.

* The SME said that quotations also need to preserve context. Extracting a single sentence from a paragraph can sometimes remove an important qualification, exception or condition.

* The Reporting Manager asked whether the system should therefore return larger excerpts. The SME said that this would improve context but could make answers cumbersome. The better objective would be to give the analyst enough surrounding material to validate the claim without requiring them to search the entire document again.

* The SME said that tables and reporting instructions present an additional challenge. Regulatory reporting requirements are not always expressed as simple prose. The meaning of a row, column, field or reporting template may depend on definitions or instructions elsewhere.

* The Reporting Change SME said that analysts sometimes start with a reporting template and work backwards to the underlying regulatory requirement. In other cases, they start from a regulatory rule and work forward to understand how the requirement is represented in reporting.

* The SME said that both directions of navigation are useful and that the product should not assume there is always a single starting point.

* The Compliance representative asked how the system should behave when two sources appear to conflict. The SME said that the first requirement should be **to expose the conflict rather than silently resolve it**.

* The SME said that apparent conflicts can arise because documents relate to different dates, different scopes, different populations or different levels of detail. An analyst needs to understand why the conflict exists before deciding which statement applies.

* The SME said that an AI-generated resolution of a regulatory conflict should therefore be treated very cautiously. In some cases the correct outcome may be to escalate the issue to a human expert.

* The Reporting Manager asked whether the system could identify questions that require escalation. The SME said this would be valuable, but it would be difficult to define reliably at the outset.

* The SME suggested that a safer first capability would be to identify situations where the available evidence is insufficient, conflicting, ambiguous or clearly associated with different effective dates.

* The Compliance representative said that "I don't have sufficient evidence to answer this" should be considered an acceptable system outcome.

* The analysts asked whether the system could use previous internal answers to improve future responses. The SME said that historical internal answers can be useful evidence of how the organisation has previously interpreted a question, but they should not automatically be treated as regulatory authority.

* The SME said that an internal answer should ideally be labelled separately from an external regulatory source, especially if the answer represents a judgement rather than a direct statement from the regulator.

* The Compliance representative said that this distinction is particularly important if users begin copying AI-generated answers into formal reporting documentation or communications.

* The Reporting Manager asked whether the system could learn from corrections made by SMEs. The SME said that a feedback mechanism would be valuable, provided that a correction can be associated with the underlying question, answer, evidence and version of the regulatory material used at the time.

* The SME said that simply recording a thumbs-up or thumbs-down would probably not provide enough information to improve regulatory research quality. More useful feedback categories could distinguish between an incorrect answer, insufficient evidence, incorrect source, outdated source, irrelevant source and a correct but poorly explained answer.

* The analysts agreed that the ability to report "this source is relevant but the answer missed an important qualification" would be useful.

* The SME said that the system should preserve enough information about an answer to allow someone to reconstruct how it was produced. This does not necessarily mean retaining every model-level technical detail for the end user, but the product should have an auditable record of the sources and evidence used.

* The Compliance representative said that auditability should not be confused with simply storing the AI response. The important question is whether the organisation can establish which regulatory material informed the response and whether that material was current and relevant at the time.

* The SME was asked whether automatic regulatory applicability should be included in the product. The SME said that applicability is highly dependent on context.

* The SME explained that whether a requirement applies can depend on factors such as the legal entity, consolidation perimeter, permissions, reporting regime, type of exposure, reporting basis and relevant date.

* The SME therefore recommended that the initial product should not claim to make definitive applicability decisions unless sufficient structured context and validated rules are available.

* The Reporting Manager asked whether the system could instead ask the analyst for additional information when applicability is unclear. The SME said this could eventually be useful, but the product should distinguish between gathering information and making the final regulatory determination.

* The SME said that the same principle applies to interpretation. The system can help an analyst find relevant provisions, compare related material and explain what the text appears to say, but there will be cases where professional judgement is required.

* The Compliance representative said that the wording of the product interface matters. A statement such as "The applicable requirement is..." is materially different from "The relevant sources indicate..." followed by evidence and a clear caveat.

* The SME said that users should not have to interpret a model's confidence score to understand whether an answer is trustworthy. Trust should come primarily from transparent evidence, source status, date information and appropriate escalation.

* The Reporting Manager asked which regulatory material should be included in the first version. The SME said that attempting to ingest everything associated with the PRA would create unnecessary complexity.

* The SME recommended beginning with a deliberately defined corpus relating to UK capital regulatory reporting and the Basel 3.1 implementation, with explicit inclusion and exclusion criteria.

* The SME said that the corpus should not simply be a collection of URLs. Each source should ideally have metadata such as publication date, effective date where applicable, document type, subject area, version/status and relationships to other regulatory material.

* The Data/Reporting SME added that reporting templates and instructions need to be versioned alongside the relevant regulatory material. Otherwise an analyst could receive a current rule with an outdated reporting instruction or vice versa.

* The Prudential SME said that document versioning should be visible to users when it materially affects the answer.

* The Compliance representative said that the system should avoid presenting a historical document as an equally valid answer merely because its text is highly relevant to the user's query.

* The group discussed whether the product should provide a "current requirement" mode and a "future requirement" mode. The SME said that this could be useful, but the terminology and behaviour would need to be carefully defined.

* The SME said that users may also want to investigate how a requirement evolved over time. Historical comparison is useful for regulatory change work, but it should not be confused with determining the current reporting obligation.

* The Reporting Manager asked about "What changed?" as a potential capability. The SME said that identifying textual changes between two documents is relatively different from determining the regulatory significance of those changes. The latter requires understanding context and applicability.

* The SME said that an automated change comparison could therefore be useful as research support, but the product should not imply that a textual difference automatically represents a change in the firm's obligation.

* The Compliance representative said that downstream impact analysis is even further removed from simple regulatory research. Determining which internal systems, controls, processes or reports are affected would require access to internal bank information and business context that is outside the initial regulatory research problem.

* The Reporting Manager agreed that this should not be assumed to be part of the first product.

* The SME was asked what would make them trust a pilot of the product. They said that they would want to see realistic historical regulatory questions answered using the correct source material, with citations that an expert can quickly verify.

* They would also want to test deliberately difficult cases, including outdated documents, future requirements, similar terminology, multiple relevant sources and questions where the correct answer is that the evidence is insufficient.

* The SME said that an evaluation containing only straightforward questions would give a misleading impression of product quality.

* The Compliance representative said that evaluation should include the risk of **confidently wrong answers**, not just whether the system produces an answer.

* The SME said that an answer that refuses unnecessarily can also reduce usefulness. The product therefore needs to balance evidence requirements with the ability to provide useful research assistance.

* The Reporting Manager asked whether the SME would expect the AI system to reach the same conclusion as an expert in every case. The SME said that for straightforward factual retrieval and source identification, consistency should be high. For ambiguous interpretation, the appropriate behaviour may instead be to surface the relevant evidence and identify the ambiguity.

* The SME said that this distinction should be reflected in how the product is evaluated. Not every question should have a single expected natural-language answer.

* The group discussed the possibility of allowing analysts to rate answers. The SME supported this but said that feedback should be structured enough to identify why an answer was considered poor.

* The SME also recommended tracking cases where analysts ignored the AI answer and performed the research manually. Those cases could reveal important product shortcomings even if the analyst did not formally submit negative feedback.

* The Reporting Manager asked whether the product should retain analysts' final answers. The Compliance representative said that this would raise additional considerations around data retention, ownership and potential reliance, and should not be assumed as part of the initial design.

* The SME concluded that the most valuable initial capability would likely be to help analysts **find and connect authoritative regulatory evidence quickly**, while clearly communicating source status, dates and uncertainty.

* The SME said that a successful assistant should make an analyst's research process faster without making the analyst less critical of the result.

* The Compliance representative reiterated that the product should support human judgement rather than obscure it.

* The Reporting Manager concluded that the next product discussions should distinguish between capabilities that improve **regulatory research** and capabilities that attempt to automate **regulatory judgement or downstream change management**.

* No final decision was made during the meeting on the MVP feature set, source hierarchy algorithm, technical architecture, model choice, retrieval method, evaluation thresholds, governance approval process or implementation timeline.
