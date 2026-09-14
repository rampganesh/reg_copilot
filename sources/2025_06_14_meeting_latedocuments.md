## Meeting - Handling doc versions, late arriving documents

## Discussion Points

* **Participants:** Regulatory/Prudential SME (Regulatory Content Owner), AI/ML Engineer, Data Engineer, AI Governance/Model Risk representative, Technology Architecture representative.
* **Late-arriving amendments:** The Regulatory Content Owner is responsible for identifying and confirming relevant amendments and changes to the approved regulatory corpus. Technology should support automated monitoring/ingestion and flag newly detected or changed source material, but detection by the technical pipeline does not by itself establish that a change is relevant or authoritative.
* **Change validation:** Newly detected amendments should be reviewed for source authority, regulatory status, effective date and relationship to existing material before being treated as an active corpus update.
* **Affected prior answers:** Previously generated answers should not be silently treated as current if their underlying source material has subsequently changed. Where an amendment affects a source used in a prior answer, the answer should be identifiable as potentially stale and linked to the updated source/version.
* **Historical answers:** Prior answers should remain available for audit/research purposes, with their original source and temporal context preserved. They should not automatically be rewritten to reflect later amendments.
* **Staleness policy:** The product should distinguish between **current, future-effective, superseded/historical and proposed** material. Staleness should be determined using source status and effective/applicability dates rather than simply the document publication date.
* **User-facing behaviour:** Where a response relies on superseded material or a source affected by a later amendment, the product should clearly flag the status rather than silently returning the answer as current.
* **Operational expectation:** There should be an explicit process for corpus updates, including detection, SME validation, publication/update, and identification of potentially affected prior answers. The meeting did not establish a specific refresh frequency or SLA. This would be outside the scope of the system's functions.
* **Open point:** The precise staleness window/threshold and whether affected prior answers should be proactively re-reviewed or only flagged on subsequent use require further definition.
