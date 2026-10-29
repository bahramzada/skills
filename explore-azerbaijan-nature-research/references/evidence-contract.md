# Evidence contract

Use these logical records regardless of whether working notes are tables or structured data. They do not require a database or software implementation.

## Entity identity

| Field | Meaning |
|---|---|
| `id` | Unique stable lowercase Latin letters/digits/hyphens; coordinator-owned |
| `entity_type` | Place, route or administrative/geographic area |
| `names.az/en/ru` | Names and per-language status: official, verified common form, proposed translation/transliteration or unknown |
| `primary_category` | Main entity kind; keep legal status, landscape and activities in separate fields |
| `aliases` | Alternate names that help deduplication |
| `parent_place_id` | Related containing place, or null; not proof of administrative ownership |
| `district_ids` | Multiple districts allowed |
| `region_relations` | Label whether administrative, economic or editorial tourism geography |
| `source_ids` | Evidence for identity and category |

Use separate IDs for a national park, an enclosed lake and an adjacent tourism resort. IDs must survive later corrections of names. Do not merge similarly named objects without identity evidence. Transliteration is an editorial ID convention, not an official translated name.

## Source

| Field | Meaning |
|---|---|
| `source_id` | Coordinator-assigned S001, S002 and so on; no duplicates |
| `title`, `organization_author` | Actual page metadata, or explicitly unknown |
| `url` | Exact public page/document URL, if known; an original URL alone does not mean it was opened |
| `publication_date` | Publication date if stated; null otherwise |
| `effective_date` | Legal/service effective date if relevant and stated |
| `data_as_of` | Period the facts describe, if known |
| `retrieved_at` | Actual date opened; use the session's date/time context |
| `content_access` | Live page opened, supplied full document read, supplied excerpt read, partial, failed or discovery-only |
| `original_url_opened` | Whether the original URL was actually opened in this run; false for an offline excerpt |
| `lineage` | Original document/announcement; identify mirrors and copied articles |
| `supported_claim_ids` | Specific claims the source supports |

Only actually used, read materials belong in the final source registry. For live research this means the actual page/document was opened. Offline user-supplied full documents or excerpts may be listed as supplied material, with their content-access type, date read and original URL if known; explicitly state that the original page was not opened or independently reverified. A partial excerpt can establish what the supplied excerpt says, not omitted context or current validity. Do not label an offline excerpt as live-web verification. Distinguish the provided copy from the original document and keep its provenance without exposing private paths or signed URLs.

A failed URL or search-only lead can appear in the gaps table, clearly labelled unverified; it cannot support a verified claim. Exclude credentials, cookies and unnecessary tracking parameters from records. Do not invent a page's publication date from a footer or retrieval date.

## Claim

| Field | Meaning |
|---|---|
| `claim_id` | Unique working identifier, for example `C001` |
| `entity_id`, `field` | Object and particular asserted attribute |
| `value`, `unit` | Value and relevant unit; null where unknown |
| `claim_kind` | Directly supported fact, attributed estimate, inference or editorial proposal |
| `source_ids` | Specific supporting sources; proposals may have a stated rationale instead |
| `support` | Brief paraphrase plus page section/locator explaining what is actually supported |
| `dates` | Publication/effective/data-as-of/retrieval distinctions |
| `verification_status` | Verified, partially verified, conflicting or unverified |
| `qualifiers` | Visitor category, season, permission, endpoint or other conditions |
| `conflict_note` | Competing values and unresolved issue, if any |

Avoid long quotations or entire page copies. Capture sufficient paraphrased evidence to inspect the reasoning and respect applicable quotation/copyright limits. An AI response is not a primary source. Confidence is qualitative and claim-specific; agreement between AIs is not corroboration.

## Access status

The final report uses exactly:

- Açıq olduğu təsdiqlənib.
- İcazə və ya əvvəlcədən razılaşdırma tələb olunur.
- Məhdud və ya müvəqqəti bağlıdır.
- Ziyarət statusu təsdiqlənməyib.

Each status needs source IDs, applicable date and visitor/group qualifications. With no suitable evidence, use the fourth label. A legal decree establishing an area does not establish tourist access. An old tour advertisement cannot establish current access.

## Coordinates and routes

Coordinates require values, format/reference system if stated, source, precision and meaning: entrance, visitor point, trailhead or approximate center. Unknown coordinates remain null; never geocode from imagination or use the geographic center as an entrance. Approximate sourced points stay labelled approximate.

Route geometry needs operator/official provenance, endpoints and source date. Separate walking distance/time from driving approach, and one-way values from totals. An editor-created itinerary is labelled `redaksiya təklifi, yerində yoxlanmayıb`; connecting markers does not prove a trail exists. Keep official routes, commercial tour programs and editorial ideas distinct.

## Unknowns and conflicts

Unknown, zero, free, unavailable and not applicable are different values. A blank infrastructure field does not mean the facility is absent. Keep both conflicting sources and their dates; explain preference using claim authority, specificity and effective date. Retain unresolved conflicts in section 10 and propagate the uncertainty into profiles, maps, filters and MVP decisions.
