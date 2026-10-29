# Attribution and modifications

This package includes adapted workflow guidance and exact audit snapshots from [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) at commit `2574e29377c7173d0cecffef29a6ecbd7f8ccb5d`.

The relevant enterprise-search, data and product-management plugin directories each contain the Apache License, Version 2.0. Their identical license text is retained in [LICENSES/Apache-2.0.txt](LICENSES/Apache-2.0.txt). No upstream NOTICE file was listed in the reviewed repository tree. Attribution does not imply endorsement by the upstream authors.

| Downloaded upstream skill | Bundled adaptation | Why selected |
|---|---|---|
| enterprise-search / search-strategy | references/search-and-verification.md | Question decomposition, claim-specific source selection and bounded fallback |
| enterprise-search / knowledge-synthesis | references/synthesis.md | Deduplication, attribution, conflicting claims and calibrated uncertainty |
| data / validate-data | references/quality-gate.md | Completeness, nulls, unique counts, methodology and conclusion checks |
| product-management / write-spec | references/product-planning.md | Visitor needs, page behaviors, fields, scope and acceptance criteria |
| product-management / roadmap-update | references/product-planning.md | Evidence-dependent priorities, phasing and dependencies |

These adaptations are modified versions. Corporate chat, email, private-source discovery and tracker integrations were removed from active workflows. Generic revenue/SQL analysis became tourism evidence and inventory QA. A full PRD/roadmap output was replaced with the supplied 12-section report. Unmeasured RICE inputs, numeric confidence formulas, capacity assumptions, repetitive clarification and mandatory parallel execution were not adopted.

The orchestration, evidence contract, tourism identity/route rules and report-comparison protocol are project-specific additions based on the user's prompt. [references/research-brief.az.md](references/research-brief.az.md) preserves that prompt verbatim. Claims inside it remain research questions or project-context assertions to verify.

[sources.lock.json](sources.lock.json) records immutable upstream URLs, commit, file hashes, scoped licenses and adaptation mappings. The five unmodified `sources/*.md` files retain upstream frontmatter and examples for audit only. They are not independently discoverable skill entrypoints and are not active instructions; the coordinator reads the adapted references.

This package has no affiliation with the upstream project or any tourism authority. Updates require a new source and safety review; there is no automatic updater.
