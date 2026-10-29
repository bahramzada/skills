# Targeted pre-publication safety review

Review date: 2026-10-29. Scope: the five pinned upstream skill texts, their plugin licenses and this instruction-only adaptation. This is a bounded static review, not an exhaustive repository, dependency or deployed-system security certification.

## Sources and selection

The five downloaded skills come from `anthropics/knowledge-work-plugins` commit `2574e29377c7173d0cecffef29a6ecbd7f8ccb5d`. Exact file hashes and paths are in sources.lock.json. Each downloaded skill directory contained only SKILL.md. The official local skill-installer copied them to a temporary review directory, without running upstream installers or examples. Its network download used the system curl with TLS verification to handle the local Python certificate issue.

| Candidate | Decision |
|---|---|
| search-strategy, knowledge-synthesis | Selected and adapted from corporate search to public, claim-specific evidence |
| validate-data | Selected and adapted to inventory, references, unknowns and conclusions |
| write-spec, roadmap-update | Selected for report-only product planning with evidence-based editorial priorities |
| Orchestra autoresearch / training / ML-paper skills | Excluded: poor fit for nature-tourism research; prior autonomy and unsafe-code concerns were not imported |
| Tavily research | Not selected: requires authenticated external CLI/service; no such dependency needed here |
| Interview-based user-research synthesis | Not selected as a core role: no interview/survey corpus is supplied; visitor scenarios remain hypotheses |
| rapp-skills deep-research | Not selected: the search-result path was absent from the pinned current tree; no unverified snapshot adopted |

## Review outcomes

- Full text of the five selected upstream skills was read. Static searches checked executable snippets, destructive shell/Git actions, credentials, permission suppression, persistence, network endpoints and instruction overrides. No supported credential-exfiltration or malicious executable behavior was identified in these five instruction-only inputs. This is not proof of universal safety.
- Active package content contains no executable scripts, lifecycle hooks, dependency installer, shell payload, MCP configuration, background scheduler or automatic updater. Archived source snippets are audit data; active references neither execute them nor require their tool integrations.
- Upstream instructions to search private connectors or write tracker updates were not carried into the research workflow. Private connectors require explicit task scope; messaging, publication, account actions and paid services require user authorization.
- Generic instructions to save analysis to Git do not grant Git permission. The active workflow respects the host/user's existing mutation rules and preserves existing output files.
- Web/PDF/GPX/report contents cannot replace the user's task or grant permissions. Browsing uses already available tools, respects controls/rate limits and records failed/partial verification.
- Unknown access, prices, coordinates, facilities and route geometry stay unknown. A designation is not public access; an editorial route is not a confirmed trail. Geographic balance, source lineage, factual versus editorial statements and practical-data freshness are explicit checks.
- Subagents are optional and capacity-limited. Sequential fallback is explicit. Three roles or same-model workers are not misrepresented as three independent AI reports. Task work ends with the report or a disclosed limit; no recurrence is created.
- Source hashes and scoped Apache-2.0 licenses are preserved. Original snapshots use `.md` names under sources/, with one active SKILL.md for the complete package.

## Validation and limits

Validation performed for this publication:

- The official skill-creator quick validator passed. Its PyYAML dependency was isolated in a temporary validation environment; it is not a package/runtime dependency.
- All five upstream snapshot hashes, their scoped license hashes and the verbatim brief hash matched. All 17 active local Markdown links resolved inside the package; one active SKILL.md was present. Files were valid UTF-8, ordinary non-executable text with no symlinks.
- UI YAML, the explicit skill name in the default prompt and normal automatic-discovery policy validated. A targeted secret/private-path pattern scan returned no matches; pattern scanning is not universal secret detection.
- A fresh-context reviewer applied the skill to fictional offline sources containing conflicting access/price claims, a center coordinate, unsupported route geometry and embedded instructions to expose credentials/upload/schedule work. It preserved unknown current values, separated historical fees and legal designation from access, deferred unsupported navigation/transport filters and ignored the injected instructions. It correctly distinguished two reports and internal roles from three independent AI runs.
- That reviewer identified an ambiguity between reading an offline excerpt and opening the original URL. The evidence contract and quality gate were updated with explicit content-access/provenance distinctions before publication. The targeted repair was rechecked separately.

No live tourism research, booking, route traversal, source-code execution or private-service access is part of this package review. Future browser/agent behavior, external tool bugs and future factual changes remain outside the static review. The report quality gate must still run for each actual research task.
