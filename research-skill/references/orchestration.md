# Research orchestration

## Establish the contract

Identify the question, intended decision/audience, scope, exclusions, time horizon, freshness needs, output format/language, available evidence/tools and any user resource limit. Use supplied context and reasonable labelled assumptions; ask only about material blockers. Read the report contract when the user has not supplied one.

Maintain a compact task-local ledger of entities, claims, sources and gaps. In-memory records or a Markdown table are enough; sidecar files are optional when the task needs them. This is evidence tracking, not permission to persist the conversation or modify unrelated repositories.

## Roles and dependencies

| Phase | Work product | Prerequisite |
|---|---|---|
| Question decomposition | Bounded subquestions and coverage map | User contract |
| Source discovery and reading | Source/claim records and unresolved leads | Source plan |
| Entity/coverage reconciliation | Canonical identities, versions and gaps | Initial evidence |
| Synthesis | Findings, conflicts and implications | Reconciled evidence |
| Optional decision/product planning | Requirements and priorities | Actual findings and constraints |
| Review and delivery | Checked answer with explicit limits | Draft and evidence ledger |

Use actual subagent capability and permissions. Divide independent subquestions by domain, entity group, source type or a genuinely different investigative perspective. Do not impose a fixed agent count. Research can proceed sequentially when delegation is unavailable; disclose that review was not independent.

Each packet includes its precise question, scope/exclusions, relevant role references, permitted sources/tools, existing IDs and output contract. Require observed evidence, source-access status, uncertainty, counterevidence and remaining work. Keep factual investigation distinct from optional recommendation drafting.

Workers return separate records. The coordinator owns the canonical entity/source map and final deliverable. Do not permit concurrent writes to shared outputs. Worker source IDs are provisional; reconcile duplicate documents and evidence lineages, assign global S001-style IDs, and replace provisional citations consistently.

## Integration

Resolve entity identity and version before comparing attributes. Merge only genuine duplicates; preserve different periods, populations and conflicting claims. Check important claims against the actual source content rather than accepting another agent's confidence label. Start product planning only once findings and actual field availability can support it.

Use a fresh quality reviewer when permitted. Otherwise apply the same checklist sequentially and state the limitation. Internal roles are not independently conducted research studies or different AI systems.

## Budget and stopping

Honor stated time, token, source or cost limits. Otherwise begin with targeted primary-source queries, reuse opened material and expand only for named gaps. For an unproductive query, try at most two meaningful reformulations before recording the gap. Respect rate-limit timing rather than retrying aggressively.

Review can trigger one targeted repair pass and one further focused repair for a remaining material issue. Recheck affected content; do not restart completed research. Stop when the requested questions have supported answers or explicit gaps, or a user limit is reached. Deliver partial work honestly rather than stretching quotas or creating future loops.

For independent-report comparison, use the separate comparison reference. Do not import other AI conclusions into a supposedly independent run unless the user requests that comparison.
