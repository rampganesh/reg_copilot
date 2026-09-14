---
type: decision
status: active
date: 2025-06-14
decider: PM (approving Meeting 3 outcomes — handling doc versions / late-arriving documents)
updated: 2025-06-14
---

# Corpus update process and staleness policy

## Context
Post-final amendments demonstrably arrive in the corpus (CP9/26 five months after final rules PS1/26; source: 2025_06_10_research_docversions.md, L8-9). Q3 asked how the system handles versions, dates and late-arriving amendments rather than treating the corpus as fixed. Meeting 3 was convened with the Regulatory Content Owner, AI/ML Engineer, Data Engineer, AI Governance/Model Risk representative and Technology Architecture representative (source: 2025_06_14_meeting_latedocuments.md, L5).

## Options considered
1. **Fully automated corpus refresh** — rejected: detection by the technical pipeline does not by itself establish that a change is relevant or authoritative (source: 2025_06_14_meeting_latedocuments.md, L6).
2. **Static corpus, manual rebuilds** — rejected: contradicts the demonstrated post-final amendment flow and the bounded-corpus decision's metadata requirements.
3. **Content-Owner-gated update process with technical detection support and explicit staleness handling** — adopted (source: 2025_06_14_meeting_latedocuments.md, L6-12).

## Decision & rationale
- **Ownership**: the Regulatory Content Owner is responsible for identifying and confirming relevant amendments and changes to the approved regulatory corpus; Technology supports automated monitoring/ingestion and flags newly detected or changed source material (source: 2025_06_14_meeting_latedocuments.md, L6).
- **Validation gate**: newly detected amendments are reviewed for source authority, regulatory status, effective date and relationship to existing material before being treated as an active corpus update (source: 2025_06_14_meeting_latedocuments.md, L7).
- **Affected prior answers**: answers are never silently treated as current when underlying sources changed; where an amendment affects a source used in a prior answer, the answer is identifiable as potentially stale and linked to the updated source/version (source: L8, L11).
- **Historical answers**: preserved for audit/research with original source and temporal context; never automatically rewritten (source: L9).
- **Staleness determined by source status and effective/applicability dates**, not publication date; user-facing behaviour flags superseded/amended-source reliance rather than silently returning answers as current (source: L10-11).
- **Explicit process**: detection → SME validation → publication/update → identification of potentially affected prior answers. No refresh frequency/SLA established — outside the system's functions (source: L12).

## Reversal conditions
- Analyst or stakeholder pressure for a defined refresh SLA/frequency (would reopen the process with an operations component).
- Detection pipeline proven unreliable (missed amendments or excessive false flags) — escalate to corpus governance.
- Evidence that flag-on-use staleness handling leaves risky stale answers unreviewed for too long (see Q10).

## Related
- [[../open-questions|Q3 (answered), Q10 (open)]]
- 2025-06-04_bounded-curated-corpus; 2025-06-04_date-based-temporal-mode; 2025-06-04_temporal-awareness-v1
- [[../problems/source-validation-burden]]; [[../problems/no-feedback-loop]]