# Evidence synthesis

Adapted from upstream `knowledge-synthesis`; see NOTICE and sources.lock.json.

Merge records by entity and claim, not by source website or by which worker returned them. Deduplicate copied announcements using their underlying document lineage. Preserve distinct versions, visitor groups, dates and genuinely contradictory statements.

## Reconcile a claim

1. Identify the exact object, field, unit, period and qualifier.
2. Compare each candidate value with the actual source passage.
3. Prefer a source that is authoritative for that particular claim. Use specificity, legal/service effective date and supersession evidence; do not simply choose the newest article or the longest page.
4. If supported, explain the selected value and retain the superseded/conflicting record in section 10.
5. If unresolved, mark the claim conflicting/unknown and carry that status into every downstream profile, route, feature and MVP recommendation.

Use qualitative confidence grounded in observed evidence: directly supported, partially supported, conflicting or unverified. Do not compute a pseudo-precise source reliability score, multiply subjective weights, or treat a copied report as independent corroboration.

## Keep attribution inspectable

Every important factual statement gets source IDs. Where a row contains claims from different sources, associate each field/value with its supporting IDs. The final registry maps each ID to a full concrete page URL, organization/title, relevant dates and supported information. Remove unused sources from the registry; put failed discovery leads in gaps instead.

The executive summary should answer the product question using the established inventory and evidence. Keep editorial decisions explicit: proposed category structure, visitor scenarios, MVP selection, translations and untested itineraries are proposals, not measured facts.

Do not compress away missing information to make the report appear complete. Preserve the 12-section structure and claim distinctions even when several output parts are required.
