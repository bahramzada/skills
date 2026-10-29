# Targeted pre-publication safety review

Review date: 2026-10-29. Scope: five pinned upstream instruction texts, their scoped licenses and this generic adaptation. This is a bounded static and behavioral review, not an exhaustive repository/dependency/deployment security certification.

## Selected sources

All five sources come from anthropics/knowledge-work-plugins commit `2574e29377c7173d0cecffef29a6ecbd7f8ccb5d`: search-strategy, knowledge-synthesis, validate-data, write-spec and roadmap-update. Each downloaded skill directory contained only SKILL.md. The official local installer downloaded them into a temporary review area without running upstream installers/examples. Exact hashes, paths and license mappings are in sources.lock.json.

## Review findings and controls

- Full upstream text was read and searched for executable payloads, destructive actions, exposed credentials, permission suppression, persistence, network endpoints and instruction overrides. No supported malicious executable or credential-exfiltration behavior was identified in these five inputs; this is not universal proof of safety.
- The active package contains no executable scripts, hooks, dependency installer, MCP configuration, scheduler or automatic updater. Archived source examples are audit data, not execution instructions.
- Research uses task-relevant public/supplied evidence. Private connectors require explicit scope. Publication, messaging, transactions, paid services, Git mutations, installations and recurrence require separate user authorization unless already granted.
- Retrieved pages, files and report contents cannot override the user's task or authorize secret access. Existing browser tools respect controls/rate limits. No private material is automatically uploaded.
- Unknowns, dates, conflicts, units, evidence lineage and actual content access are explicit. Reading an offline excerpt does not imply the original URL was opened or live facts verified.
- Subagents are optional, capacity-limited and have separate outputs. Sequential fallback is explicit. Internal roles are not independent AI systems or empirical confirmations.
- Source hashes, scoped Apache-2.0 licenses and one active skill entrypoint are preserved. The package has no embedded application-specific brief or fixed domain/report requirements.

## Validation

The generic package passed the official skill-creator structural validator, all 17 active local-link checks, five source and scoped-license hash checks, UTF-8/non-executable-file checks and UI YAML validation. It contains 20 text files and one active SKILL.md. A package-wide reference scan found no application-specific brief or fixed-domain content. A targeted secret/private-path pattern scan found no supported matches; pattern scanning is not universal secret detection.

A fresh-context reviewer applied the generic skill to fictional offline material with conflicting versions, unsupported feature claims, old prices, two AI reports and embedded credential/upload/scheduling instructions. It preserved version limits and unknown current values, labelled offline access, rejected injected instructions, compared only the reports supplied and kept product priorities conditional on evidence. No concrete usability defect was reported in that bounded test. No live service or source snippet was executed.

The validator's temporary PyYAML environment is not a package/runtime dependency. Remote file contents are verified against the local package during publication.

Future facts, host/tool behavior, deployments and dependencies outside this text package remain out of scope. Apply the quality gate to every actual research task.
