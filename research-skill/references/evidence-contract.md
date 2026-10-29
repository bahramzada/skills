# Evidence contract

Use these logical records whether notes are tables, structured data or in memory. A database or additional software is not required.

## Entity

Record a stable unique ID, name/aliases, entity type, scope/version, relevant relations and identity sources. Choose an ID convention appropriate to the user; lowercase Latin letters/digits/hyphens are a reasonable default. Different entities or versions must not be merged just because their names look alike. A missing attribute remains unknown rather than being inferred from the entity's existence.

## Source

| Field | Meaning |
|---|---|
| source_id | Unique coordinator-assigned S001-style ID, unless the user supplies another convention |
| title / organization_author | Observed metadata, or explicitly unknown |
| url | Exact public document/page URL if known; having a URL does not mean it was opened |
| content_access | Live page opened, supplied full document read, supplied excerpt read, partial, failed or discovery-only |
| original_url_opened | Whether the original URL was actually opened during this run |
| publication_date / effective_date | Stated publication or effective date; keep distinct |
| data_as_of | Period or version the facts describe |
| retrieved_at | Actual date the material was read |
| lineage | Underlying original document/data; identify mirrors and copied accounts |
| supported_claim_ids | Specific claims supported by the material |

Only used, actually read materials belong in the final registry. For offline supplied documents/excerpts, label the content-access type and original URL if known, and state that the original page was not independently opened/reverified. An excerpt supports what the excerpt says, not omitted context or current validity. Failed/search-only leads belong in gaps and do not support verified facts.

Do not expose private filesystem paths, credentials, cookies or signed URLs in a public-facing registry. Use a safe document label. Do not invent publication dates from a footer or retrieval timestamp.

## Claim

Record claim_id, entity/topic, particular field, value/unit, claim kind, source IDs, supporting paraphrase/locator, relevant dates, scope/qualifiers, verification status and conflict note. Claim kinds are directly supported fact, attributed estimate, inference and editorial proposal. Verification statuses include verified, partially verified, conflicting and unverified.

Every important factual assertion needs its actual supporting source. A source supporting one field does not support an entire row or paragraph. Preserve populations, versions, time periods, denominators and conditions when they affect meaning. Recommendations and assumptions need transparent rationale rather than fabricated factual support.

Capture concise paraphrased evidence and respect quotation/copyright limits. AI answers are leads, not primary records. Confidence is qualitative and tied to observed support; agreement between AIs is not independent evidence.

## Unknowns and conflicts

Keep unknown, zero, false, unavailable and not applicable distinct. Compare conflicting claims for identity, units, period and qualifiers before declaring disagreement. Prefer sources by authority for the particular claim, specificity, effective date and supersession evidence; do not silently choose the newest or majority value.

Retain conflicting sources, the reason for any selected value and the unresolved issue. Propagate unresolved uncertainty into conclusions, proposed features, priorities and readiness claims. Numerical plausibility alone is not validation.
