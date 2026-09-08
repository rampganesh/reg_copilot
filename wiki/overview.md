---
type: overview
updated: 2026-09-06
---

# Regulatory Research Assistant — Living Overview

## Current State (as of 2026-09-06)

This wiki contains findings from the **Meeting 1 — Business & User Discovery** (2025-05-24). All problems are `status: emerging` because a single source cannot confirm them; each requires ≥3 independent sources or ≥2 source types per AGENTS.md L41.

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

## Problems Identified (all `status: emerging`, `mentions: 1`)

1. **[validating-the-right-source](wiki/problems/validating-the-right-source.md)** — Validation (right source, applicable, not superseded) is harder than discovery (L11)
2. **[evidence-assembly-overhead](wiki/problems/evidence-assembly-overhead.md)** — 5 min understanding + 15–20 min evidence assembly (L33)
3. **[version-and-effective-date-ambiguity](wiki/problems/version-and-effective-date-ambiguity.md)** — Technically correct answers can be operationally wrong (L19)
4. **[terminology-fragmentation](wiki/problems/terminology-fragmentation.md)** — Same concept in different document types with different wording (L13)
5. **[knowledge-locked-in-individuals](wiki/problems/knowledge-locked-in-individuals.md)** — Experienced vs. newer analysts' knowledge gap (L21, L23, L27)
6. **[no-feedback-loop-on-answers](wiki/problems/no-feedback-loop-on-answers.md)** — No mechanism to track which sources resolved questions (L63, L65)
7. **[material-authority-conflation](wiki/problems/material-authority-conflation.md)** — Final rules vs. reporting instructions vs. consultation documents should not appear to have same authority (L49)

---

## Open Questions (Q1–Q11, all `status: open`)

The [open-questions.md](open-questions.md) page carries all 11 questions tagged by resolution path (ask-users / check-data / ask-stakeholder / desk-research). Four of them are **contradictions**:

- Q3: "finding" vs. "interpreting" — team wants help with finding (L37) but also asks "What does this reporting field mean?" (L57, Q10), which is interpretation-adjacent
- Q9: Manager wants consistency across analysts (L67) but SME says segments need different behavior (L81)
- Q5: "did not agree" auto-applicability in v1 — absence of decision, not a negative decision
- Q1: Cross-referencing automation is described as the core problem (L11) but no decision was made on whether to solve it

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

---

## Notes and Deviations

- **Filename convention**: Source files use `2025_05_24_` (underscore), but schema requires `YYYY-MM-DD_<type>_<slug>` (hyphen). Sources are read-only, so we cite the real filename and note the deviation in the log.
- **Stage 2 triggers not yet fired**: No problem pages have ≥2 source types yet (only one source ingested). No `wiki/personas/`, `wiki/bets/`, etc. until triggered.
- **Competitors folder exists but empty**: `wiki/competitors/` is pre-created but Stage 2 says add only when competitor intel is ingested a 2nd time. Harmless, deletion would require approval.

---

## Next Steps

1. Ingest `2025_05_26_meeting_followup.md` as a separate pass (same source type, so no `confirmed` promotions yet without a 2nd source type)
2. PM review of proposed decision pages and assumption register
3. Add product context block to `AGENTS.md` (currently template-only, no adaptation notes)
4. Lint pass after ≥2 source types to check for contradictions and triggers