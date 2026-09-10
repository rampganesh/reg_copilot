---
type: overview
updated: 2026-09-09
---

# Regulatory Research Assistant — Living Overview

## Current State (as of 2026-09-09)

This wiki contains findings from **Meeting 1 — Business & User Discovery** (2025-05-24) and **Meeting 2 — Regulatory / Prudential SME Discovery** (2025-05-26). All problems are `status: emerging` because both sources are `meeting` type with overlapping participants; `confirmed` requires ≥3 independent sources or ≥2 source types per AGENTS.md L83–L84.

**Stakeholders**: 6 distinct roles — Regulatory Reporting Manager, Analyst 1, Analyst 2, Prudential Regulatory SME, Compliance representative, Reporting Change SME, Data/Reporting SME.

**Problems**: 11 pages (7 from source 1, 4 new from source 2).

**Open questions**: 24 questions (Q1–Q11 from source 1, Q12–Q24 from source 2).

**Assumptions**: 9 entries (A1–A6 from source 1, A7–A9 new from source 2), all `status: untested`.

**Decisions**: 3 held proposals pending PM approval (2025-05-24).

---

## The Core Problem (manager's framing)

The team's research burden is **not** access to regulatory documents:

> "the amount of **time and effort required to find, connect, validate and present regulatory information**, rather than a lack of access to regulatory documents themselves" (source: 2025_05_24_meeting_kickoff.md, L99)

Evidence assembly dominates the task: analysts spend **5 minutes** understanding an answer but **15–20 minutes** finding the exact supporting section and presenting evidence clearly (L33).

---

## Stakeholders

| Role | Key concerns |
|------|--------------|
| **Regulatory Reporting Manager** | Consistency between analysts (L67), time-savings while maintaining quality (L73), no dependence on AI answers (L67), adoption depends on experienced analysts believing it saves time (L75) |
| **Analyst 1** | Normal-language queries (L43), experienced analysts want reduced repetitive searching (L77) |
| **Analyst 2** | Inspectable provenance (L45), accuracy > speed (L69), less experienced analysts need ramp support (L79) |
| **Regulatory Change/Reporting SME** | "Assistant for regulatory research, not as the final authority" (L71), finding vs. interpreting distinction (L37), cross-referencing importance during transitions (L17), material authority levels matter (L49) |
| **Prudential Regulatory SME** | Authority is relational, not hierarchical (L7, L9, L11, L13, L15, L33, L35, L37); effective dates are first-class metadata (L25, L113); no automatic applicability decisions (L95, L97, L99) |
| **Compliance representative** | No fabricated citations (L49, L51, L53, L55); no confidence scores (L29, L107); expose conflicts (L67, L69); no definitive applicability (L95, L99); retention/ownership concerns (L79, L81, L83, L151) |
| **Reporting Change SME** | Information gathering vs. regulatory determination (L101); downstream impact analysis is larger problem (L61) |
| **Data/Reporting SME** | Effective dates as first-class metadata (L113); corpus boundedness (L109, L111) |
- **Risk to avoid**: "An incomplete search, outdated source or misunderstood requirement can lead to an incorrect interpretation being circulated internally" (source: 2025_05_24_meeting_kickoff.md, L101)

## Hard Constraints from Meeting 2

**No confidence scores**: "A high-confidence model output does not establish regulatory applicability" (source: 2025_05_26_meeting_followup.md, L29); "users should not have to interpret a model's confidence score to understand whether an answer is trustworthy" (L107).

**No fabricated citations**: "the system should not manufacture paragraph numbers, section references or quotations when the source does not contain them" (L53); "an incorrect citation may be worse than no citation because it creates a false impression of auditability" (L55).

**Expose conflicts, don't resolve**: "the first requirement should be to expose the conflict rather than silently resolve it" (L67); "an AI-generated resolution of a regulatory conflict should therefore be treated very cautiously" (L71).

**No automatic applicability**: "the initial product should not claim to make definitive applicability decisions unless sufficient structured context and validated rules are available" (L99).

**No downstream impact analysis**: "determining which internal systems, controls, processes or reports are affected would require access to internal bank information and business context that is outside the initial regulatory research problem" (L129); "this should not be assumed to be part of the first product" (L131).

**Bounded corpus + metadata**: "the SME recommended beginning with a deliberately defined corpus relating to UK capital regulatory reporting and the Basel 3.1 implementation, with explicit inclusion and exclusion criteria" (L111); "each source should ideally have metadata such as publication date, effective date where applicable, document type, subject area, version/status and relationships to other regulatory material" (L113).

**Evaluation criteria**: "realistic historical regulatory questions answered using the correct source material, with citations that an expert can quickly verify" (L133); "test deliberately difficult cases, including outdated documents, future requirements, similar terminology, multiple relevant sources and questions where the correct answer is that the evidence is insufficient" (L135); "an evaluation containing only straightforward questions would give a misleading impression of product quality" (L137); "evaluation should include the risk of confidently wrong answers, not just whether the system produces an answer" (L139).

## Hard Constraints from Meeting 2

**No confidence scores**: "A high-confidence model output does not establish regulatory applicability" (source: 2025_05_26_meeting_followup.md, L29); "users should not have to interpret a model's confidence score to understand whether an answer is trustworthy" (L107).

**No fabricated citations**: "the system should not manufacture paragraph numbers, section references or quotations when the source does not contain them" (L53); "an incorrect citation may be worse than no citation because it creates a false impression of auditability" (L55).

**Expose conflicts, don't resolve**: "the first requirement should be to expose the conflict rather than silently resolve it" (L67); "an AI-generated resolution of a regulatory conflict should therefore be treated very cautiously" (L71).

**No automatic applicability**: "the initial product should not claim to make definitive applicability decisions unless sufficient structured context and validated rules are available" (L99).

**No downstream impact analysis**: "determining which internal systems, controls, processes or reports are affected would require access to internal bank information and business context that is outside the initial regulatory research problem" (L129); "this should not be assumed to be part of the first product" (L131).

**Bounded corpus + metadata**: "the SME recommended beginning with a deliberately defined corpus relating to UK capital regulatory reporting and the Basel 3.1 implementation, with explicit inclusion and exclusion criteria" (L111); "each source should ideally have metadata such as publication date, effective date where applicable, document type, subject area, version/status and relationships to other regulatory material" (L113).

**Evaluation criteria**: "realistic historical regulatory questions answered using the correct source material, with citations that an expert can quickly verify" (L133); "test deliberately difficult cases, including outdated documents, future requirements, similar terminology, multiple relevant sources and questions where the correct answer is that the evidence is insufficient" (L135); "an evaluation containing only straightforward questions would give a misleading impression of product quality" (L137); "evaluation should include the risk of confidently wrong answers, not just whether the system produces an answer" (L139).

---

## Agreed Scope (what we know, not decided yet)

- **Initial domain**: UK capital regulatory reporting (L83, L85)
- **Transition focus**: Basel 3.1 implementation (L5, L55, L109)
- **Initial scope centre**: "UK capital regulatory reporting and the Basel 3.1 transition" (L109)
- **Initial product type**: "internal tool for regulatory-reporting professionals" (L109)
- **Role**: Research assistant that helps find/organize evidence, not interpret (L37, L39, L41)
- **Risk to avoid**: "An incomplete search, outdated source or misunderstood requirement can lead to an incorrect interpretation being circulated internally" (L101)

---

## Not Yet Decided (L111 explicitly states none of these are decided)

Per L111: "No decision was made during the meeting on the final MVP feature set, technical architecture, model, retrieval approach, evaluation methodology, implementation timeline or success metrics."

**MVP feature set**: Narrow domain (capital reporting) but unclear whether it includes:
- Normal-language queries → terminology mapping (L43, L10)
- Cross-referencing automation (L11–L17, Q1)
- Version/effective-date handling (L17, L19, Q2)
- Material authority distinction (L49, Q4)
- "What has changed?" comparison (L59)
- Auto-applicability (L93 — "did not agree" in v1)

**Technical architecture**: Not decided. Implications:
- Is "insufficient evidence" escalation a first-class feature (L89, Q3)?
- How do we handle a non-static corpus (L87, Q7)?
- What model/retrieval approach handles terminology fragmentation (L13, L43, Q10)?

**Success metrics**: None defined yet (L111). Manager's stated goals:
- "reduce the time analysts spend searching and assembling evidence while maintaining or improving the quality of the resulting answers" (L73)
- "improve consistency between analysts" (L67)

But L111 says these are not yet success metrics — just goals to be measured against.

---

## Problems Identified (all `status: emerging`)

**Source 1** (7 pages, `mentions: 1` → `2` after ingest):
1. [validating-the-right-source](wiki/problems/validating-the-right-source.md) — Validation (right source, applicable, not superseded) is harder than discovery (L11)
2. [evidence-assembly-overhead](wiki/problems/evidence-assembly-overhead.md) — 5 min understanding + 15–20 min evidence assembly (L33)
3. [version-and-effective-date-ambiguity](wiki/problems/version-and-effective-date-ambiguity.md) — Technically correct answers can be operationally wrong (L19)
4. [terminology-fragmentation](wiki/problems/terminology-fragmentation.md) — Same concept in different document types with different wording (L13)
5. [knowledge-locked-in-individuals](wiki/problems/knowledge-locked-in-individuals.md) — Experienced vs. newer analysts' knowledge gap (L21, L23, L27)
6. [no-feedback-loop-on-answers](wiki/problems/no-feedback-loop-on-answers.md) — No mechanism to track which sources resolved questions (L63, L65)
7. [material-authority-conflation](wiki/problems/material-authority-conflation.md) — Final rules vs. reporting instructions vs. consultation documents should not appear to have same authority (L49)

**Source 2** (4 new pages, `mentions: 1`):
8. [citation-integrity-risk](wiki/problems/citation-integrity-risk.md) — Fabricated or context-stripped citations create false auditability (L49, L51, L53, L55)
9. [conflict-suppression-risk](wiki/problems/conflict-suppression-risk.md) — Conflicts must be exposed, not silently resolved (L67, L69, L71)
10. [applicability-requires-firm-context](wiki/problems/applicability-requires-firm-context.md) — Applicability depends on legal entity, perimeter, permissions, regime, exposure type, date (L97)
11. [interface-wording-overstates-authority](wiki/problems/interface-wording-overstates-authority.md) — "The applicable requirement is…" vs "The relevant sources indicate…" (L39, L105)

---

## Open Questions (Q1–Q24, all `status: open`)

The [open-questions.md](open-questions.md) page carries all 24 questions tagged by resolution path (ask-users / check-data / ask-stakeholder / desk-research / run-experiment). **Source 1** contributes Q1–Q11; **Source 2** contributes Q12–Q24. Four from Source 1 are **contradictions**:

- Q3: "finding" vs. "interpreting" — team wants help with finding (L37) but also asks "What does this reporting field mean?" (L57, Q10), which is interpretation-adjacent
- Q9: Manager wants consistency across analysts (L67) but SME says segments need different behavior (L81)
- Q5: "did not agree" auto-applicability in v1 — absence of decision, not a negative decision
- Q1: Cross-referencing automation is described as the core problem (L11) but no decision was made on whether to solve it

Source 2 introduces new tensions:
- Q14: "insufficient evidence" vs. "unnecessary refusal reduces usefulness" (L77 vs L141)
- Q13: Semantic similarity can be dangerous (L45, L47)
- Q24: Divergence by seniority (L81) vs. by question ambiguity (L143, L145)

---

## Decisions Held for PM Approval

Per AGENTS.md L96–101, proposal requires direct PM approval. Not written yet:

1. **2025-05-24_v1-scope-uk-capital-basel31.md** — UK capital reporting + Basel 3.1 as narrow first domain (L83, L85, L109)
2. **2025-05-24_human-review-guardrails.md** — No auto-submission, no production changes, human review required (L37, L39, L71, L95)
3. **2025-05-24_uncertainty-as-valid-outcome.md** — "I couldn't find sufficient evidence" is a valid outcome (L89, L91)

Each includes reversal conditions per schema.

---

## Assumptions Held for PM Approval

Per AGENTS.md L96–101, proposal requires direct PM approval. Not written yet — all `status: untested`:

- A1: Adoption requires demonstrated time savings (L75, L77)
- A2: Inspectable provenance drives trust (L45, L69, L103)
- A3: "Insufficient evidence" escalation is preferred over unsupported answers (L89, L91)
- A4: UK capital reporting + Basel 3.1 is a viable narrow first domain (L83, L85, L109)
- A5: Two segments diverge enough to need different behavior (SME opinion at L81)
- A6: Version/effective-date handling is feasible in v1 — **no source speaks to feasibility** (our belief, not theirs)
- A7: PRA material exposes effective-date/version/status metadata in extractable form — **testable by Q18**
- A8: Analysts will supply structured feedback if the taxonomy is right — **tension with L149 (track passive behavior)**
- A9: A deliberately bounded corpus can stay bounded in a non-static domain — **tension with L87 (non-static)**

---

## Notes and Deviations

- **Filename convention**: Source files use `2025_05_24_` and `2025_05_26_` (underscores), but schema requires `YYYY-MM-DD_<type>_<slug>` (hyphen). Sources are read-only, so we cite the real filename and note the deviation in the log.
- **Stage 2 triggers**: **Stakeholders** has fired (6 distinct roles, Compliance independently shaping constraints per L29, L39, L55, L77, L83, L93, L105, L119, L129, L139, L151, L157). **Personas** has not fired (source 2 is SME-driven, no ≥3 problem pages showing diverging user types). **Bets**, **competitors**, and **metrics** have not fired.
- **Competitors folder exists but empty**: `wiki/competitors/` is pre-created but Stage 2 says add only when competitor intel is ingested a 2nd time. Harmless, deletion would require approval.

---

## Next Steps

1. ~~Ingest `2025_05_26_meeting_followup.md`~~ — **done** (2026-09-09 ingest)
2. ~~PM review of proposed decision pages and assumption register~~ — **held pending PM approval** (3 decision pages, 3 new assumptions A7–A9)
3. ~~Add product context block to `AGENTS.md`~~ — **done** (2026-09-09)
4. **Lint pass** after ≥2 source types to check for contradictions and triggers — **ready** (source 2 ingested; stakeholders trigger fired)
5. **Create `wiki/stakeholders/`** — approved per AGENTS.md L191–L197