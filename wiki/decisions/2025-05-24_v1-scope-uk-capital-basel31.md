---
type: decision
status: active
date: 2025-05-24
decider: Regulatory Reporting Manager
updated: 2026-09-06
---

# v1 Scope: UK Capital Regulatory Reporting + Basel 3.1 Transition

## Context

The team is preparing for the transition to the Basel 3.1 framework, with the largest operational changes expected around the 1 January 2027 implementation date. The initial product needs a narrow regulatory domain rather than covering every regulatory question handled by the bank. **(source: 2025_05_24_meeting_kickoff.md, L5, L83)**

## Options Considered

### Option A: Narrow scope — UK capital reporting + Basel 3.1

**Evidence for**:
- "the initial product should probably focus on a relatively narrow regulatory domain" (L83)
- "capital regulatory reporting provides a realistic initial domain because the team is already spending significant effort understanding the changes and their reporting implications" (L85)
- "initial scope centred on UK capital regulatory reporting and the Basel 3.1 transition" (L109)

**Evidence against**:
- SME warned that "determining the downstream impact of a regulatory change on systems, processes, reporting templates and controls is a much larger problem than simply finding the relevant regulatory text" (L61)
- L111 explicitly states "No decision was made...on...MVP feature set..." — this scope is a statement of fact from the meeting, not a formal decision

### Option B: Broader scope covering multiple regulatory domains

**Evidence for**:
- None from this source; manager explicitly prefers narrow first release (L83)

**Evidence against**:
- L83: "manager said that the initial product should probably focus on a relatively narrow regulatory domain rather than attempting to cover every regulatory question handled by the bank"
- L105: "she did not want the team to assume that all of these belong in the first product release"

## Decision & Rationale

**Decision**: Initial domain = UK capital regulatory reporting + Basel 3.1 transition **(proposed)**.

**Rationale**: L83, L85, L109 record the manager's stated preference for narrow scope and identify capital reporting as the realistic initial domain. This aligns with the stated goal to distinguish capabilities that solve the **core research problem** from attractive extensions (L107).

**Caveat**: L111 records "No decision was made during the meeting on the final MVP feature set..." — this document captures what was *stated*, not what was formally decided. Formal decision requires PM approval and explicit reversal conditions.

## Reversal Conditions

This decision would be reopened if:
1. Basel 3.1 implementation date moves materially from 1 Jan 2027
2. Discovery shows the research problem is fundamentally domain-agnostic (capital reporting is just one instance)
3. Team effort shifts off capital reporting due to resource constraints or strategic change

## Related

- **Problem pages**: version-and-effective-date-ambiguity (L17, L19), knowledge-locked-in-individuals (L21, L23)
- **Open questions**: Q7 (non-static corpus), Q11 (Basel 3.1 feasibility)
- **Overview**: Agreed Scope section