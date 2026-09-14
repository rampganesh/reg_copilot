# Overview - product state synthesis

Updated: 2025-06-04 (after ingest of Meetings 1-2 and the 2025-06-04 email digest)

## Product
Internal AI-powered regulatory research assistant for a UK bank's capital regulatory reporting team, preparing for the Basel 3.1 transition (implementation 1 January 2027). The initial product is an internal tool for regulatory-reporting professionals, with initial scope centred on UK capital regulatory reporting and the Basel 3.1 transition (source: 2025_05_24_meeting_kickoff.md, L83, L109; source: 2025_05_26_meeting_followup.md, L109-111).

## Core problem
Not access to documents but the time and effort to **find, connect, validate and present** regulatory information - corroborated in users' words: "five minutes understanding the answer and another fifteen or twenty minutes finding the exact section" (source: 2025_05_24_meeting_kickoff.md, L33, L99). Risk beyond wasted time: incomplete searches or outdated sources lead to incorrect interpretations circulating internally (source: 2025_05_24_meeting_kickoff.md, L101). The Prudential SME's synthesis: the most valuable initial capability is to help analysts "find and connect authoritative regulatory evidence quickly, while clearly communicating source status, dates and uncertainty" (source: 2025_05_26_meeting_followup.md, L153).

## Problem map
- Evidence assembly time cost (high, emerging) - the headline pain - wiki/problems/evidence-assembly-time-cost.md
- Source validation burden (high, CONFIRMED) - right source / applicability / superseded / effective dates - wiki/problems/source-validation-burden.md
- Experience dependency and knowledge fragmentation (high) - personal collections, repeated research - wiki/problems/experience-dependency.md
- Terminology and cross-referencing overhead (medium) - incl. the semantic-similarity risk - wiki/problems/terminology-cross-referencing.md
- No feedback loop on prior answers (medium) - incl. structured feedback categories and auditability - wiki/problems/no-feedback-loop.md
- Requirement applicability determination (high, CONFIRMED) - context-dependent; system must not make definitive applicability decisions - wiki/problems/requirement-applicability-determination.md
- Citation integrity (high, CONFIRMED) - no manufactured references; incorrect citation worse than none - wiki/problems/citation-integrity.md
- Conflict exposure (high, CONFIRMED) - expose conflicts, never silently resolve them - wiki/problems/conflict-exposure.md
- Authority overstatement risk (high) - relational authority, careful interface language, no confidence scores - wiki/problems/authority-overstatement-risk.md
- Non-prose regulatory content (medium) - tables/templates hold operative meaning; extractability and citation complications - wiki/problems/non-prose-regulatory-content.md

## First-class constraints (named explicitly per PM direction)
1. **Applicability**: whether a requirement applies is highly context-dependent (entity, perimeter, permissions, regime, exposure, date); the product gathers information but does not make the final regulatory determination (source: 2025_05_26_meeting_followup.md, L95-105)
2. **Citation integrity**: verifiable citations with context; no manufacturing references or quotes; incorrect citation worse than no citation (source: 2025_05_26_meeting_followup.md, L49-59)
3. **Conflicts are exposed, not suppressed**: first requirement is to surface the conflict; AI resolution treated cautiously; escalation sometimes correct (source: 2025_05_26_meeting_followup.md, L67-75)
4. **Authority is not overstated**: no universal authority score; relational source relationships; interface language must not imply more certainty than the evidence; internal interpretations labelled separately (source: 2025_05_26_meeting_followup.md, L7-17, L33-39, L79-83, L105, L107)

## State of decisions
No decisions taken in either meeting - none recorded in wiki/decisions. No MVP feature set, source hierarchy algorithm, architecture, model, retrieval method, evaluation thresholds, governance approval process or timeline chosen (source: 2025_05_26_meeting_followup.md, L161). Next discussions should distinguish capabilities improving **regulatory research** from those attempting to automate **regulatory judgement or downstream change management** (source: 2025_05_26_meeting_followup.md, L159) - see open-questions.md Q1.

## Stakeholder voices in these sources
Manager, Analyst 1, Analyst 2, Regulatory Change/Reporting SME, Prudential Regulatory SME, Compliance representative (Meeting 2 also touched Data/Reporting SME, L115). (Stakeholder pages to be created when stakeholder ingest is triggered.)


## Decisions (active, 2025-06-04)
1. V1 scope: evidence-led research assistant - find, connect, explain authoritative evidence; extensions deferred (wiki/decisions/2025-06-04_v1-scope-evidence-led-research.md)
2. Temporal/version awareness in V1; interpretive change analysis deferred (wiki/decisions/2025-06-04_temporal-awareness-v1.md)
3. V1 balanced scorecard with manual-process baseline; north-star: time to verified evidence-backed answer without quality/safety loss (wiki/decisions/2025-06-04_v1-balanced-scorecard.md)
4. Bounded, curated corpus; Content Owner governs content, Technology owns ingestion (wiki/decisions/2025-06-04_bounded-curated-corpus.md)
5. Date-based current vs future mode; publication date is not applicability (wiki/decisions/2025-06-04_date-based-temporal-mode.md)
6. Minimum provenance standard: source + version/status + precise location incl. structured references; no fabrication (wiki/decisions/2025-06-04_minimum-provenance-standard.md)
7. Status/authority labelling in core UX with evidence-led language (wiki/decisions/2025-06-04_status-authority-labelling-ux.md)

## Open questions state
Answered and filed to decisions: Q1, Q2, Q4, Q5, Q6, Q7, Q9. Still open: Q3 (corpus currency for late-arriving amendments) and Q8 (evaluation design specifics - partially shaped by the scorecard decision).

## New governance roles surfaced
Regulatory/Prudential SME or Regulatory Content Owner (content governance); Technology (ingestion/indexing) - source: 2025_06_04_digest_clarifications.md, row 5.

## Update 2025-06-18 - analyst interviews and personas
- Both analyst interviews behaviourally confirmed the core problems (walkthrough evidence); no-feedback-loop CONFIRMED and severity raised to high (impact-tracing dimension); source-validation-burden at 7 mentions.
- A1 and A2 now validated (correlational) - behavioural confirmation, no measured adoption yet. A3 remains untested.
- PERSONAS ACTIVATED: wiki/personas/ - experienced-analyst (evidence-chained) and newer-analyst (second-hand evidence only; direct interview pending). Divergence: experienced = jump-to-sources, provenance-as-answer, speed without losing verifiability; newer = learn the research path, why-trust, colleague dependence.
- Q8/Q10 enriched: analyst difficult-case lists converge with the SME specification; staleness now includes impact tracing (who received/acted on a stale answer). Both open.
