# Attribution and modifications

This instruction-only research package adapts five workflows from [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) at commit `2574e29377c7173d0cecffef29a6ecbd7f8ccb5d`.

The relevant enterprise-search, data and product-management directories contain the Apache License, Version 2.0. Their identical license text is retained in [LICENSES/Apache-2.0.txt](LICENSES/Apache-2.0.txt). No upstream NOTICE file was listed in the reviewed tree. Attribution does not imply upstream endorsement.

| Upstream skill | Adapted reference | Purpose |
|---|---|---|
| search-strategy | references/search-and-verification.md | Question decomposition, claim-specific authority and bounded fallback |
| knowledge-synthesis | references/synthesis.md | Attribution, deduplication, conflicts and uncertainty |
| validate-data | references/quality-gate.md | Coverage, nulls, counts, reasoning and evidence checks |
| write-spec | references/product-planning.md | Optional needs, requirements, behavior and scope |
| roadmap-update | references/product-planning.md | Optional priorities, phasing and dependencies |

These are modified versions. Active corporate chat/email/private-source routing and tracker integrations were removed. Generic quantitative analysis was adapted to claim/record validation. PRD and roadmap outputs became optional modules rather than mandatory report formats. Unmeasured scores, capacity assumptions and mandatory parallel execution were not adopted.

The orchestration, evidence contract, coverage editor, generic report contract and comparison protocol are additional reusable guidance. No fixed topic, location, organization, domain inventory, proprietary brief or numbered report outline is required.

[sources.lock.json](sources.lock.json) records immutable upstream URLs, scoped licenses, hashes and adaptation mappings. Five exact unmodified `sources/*.md` snapshots preserve upstream frontmatter and examples for audit; they are not active skill entrypoints. The coordinator uses adapted references.

Updates require another source and safety review. No automatic updater is included.
