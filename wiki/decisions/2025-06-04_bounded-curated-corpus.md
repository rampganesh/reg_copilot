---
type: decision
status: active
date: 2025-06-04
decider: PM (approving consolidated stakeholder responses from the email digest)
updated: 2025-06-04
---

# Bounded, curated corpus with named governance

## Context
Ingesting everything PRA-related "would create unnecessary complexity"; a deliberately defined corpus with explicit inclusion/exclusion criteria and per-source metadata was recommended (source: 2025_05_26_meeting_followup.md, L109-113).

## Options considered
1. **Ingest all regulatory documents** — rejected: unnecessary complexity, no clear ownership of inclusion decisions.
2. **URL collection** — rejected: insufficient metadata for status/version awareness (source: 2025_05_26_meeting_followup.md, L113).
3. **Bounded, curated corpus with governance split** — adopted (source: 2025_06_04_digest_clarifications.md, row 5).

## Decision & rationale
**Include:** authoritative, relevant UK capital/regulatory-reporting material for the initial use case with sufficient metadata and version/status information — relevant PRA Rulebook material, policy/supervisory material, reporting instructions/templates, carefully identified supporting material. **Exclude:** unrelated regulatory domains, uncontrolled web content, unclear provenance/status, private/internal bank material (initially), and sources mistakable for operative requirements when only explanatory/proposed. Governance: a designated **Regulatory/Prudential SME or Regulatory Content Owner** governs inclusion, exclusion, relationships and meaning; **Technology** owns ingestion/indexing (source: 2025_06_04_digest_clarifications.md, row 5).

## Reversal conditions
- Stakeholder workflows show the bounded corpus misses questions users actually ask (expansion pressure with governance sign-off).
- If no Content Owner role is resourced, the curation model cannot operate — escalate to PM.

## Related
- [[../problems/source-validation-burden]]
- 2025-06-04_temporal-awareness-v1