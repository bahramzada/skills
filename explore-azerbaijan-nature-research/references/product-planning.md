# Product planning

Adapted from upstream `write-spec` and `roadmap-update`; see NOTICE and sources.lock.json. Produce report sections 06–09, rather than replacing the requested report with a generic PRD. This is planning, not implementation or a ticket-tracker update.

## Use the available evidence

Map a visitor need to an available field, a proposed page/function, its unknown-data behavior and its editorial priority. The six supplied scenarios are working hypotheses: Bakı day trip, family walk, car-free visit, experienced hiker, foreign tourist and wildlife observer. Do not invent interviews, usage statistics or research participants to validate them.

## Pages and flows — section 06

Specify nature landing, category catalogues, all-place catalogue, map, place detail, route detail and region-filtered results. For each include goal, blocks, main action, related links, mobile information priority and empty/unknown states. Address the supplied scenarios and identify nature information handed off to shared region pages. Keep other teammates' site sections out of redesign scope.

Optional acceptance-criteria examples should express behavior without code: if an entry point is unverified, the page labels the coordinate meaning and avoids presenting it as a navigation entrance; if current access is unknown, the page shows that status and source date.

## Filters and maps — section 07

Use the exact filter-table columns in the brief. Candidate filters include category, district/region, month/season, activity, difficulty/duration, transport and access/permission. For each inspect the current records to decide whether data is sufficient, partially sufficient or missing. Mark that assessment editorial; do not fabricate percentages or counts.

A filter with sparse/unverified data may belong to a later phase. Unknown values must stay discoverable and distinguishable, rather than being interpreted as a false/negative value.

Explain map markers, clustering, list synchronization, mobile behavior, entrance versus center and records lacking coordinates. Do not invent map points for completeness. Ratings, booking, live conditions and similar ideas require a stated user benefit, data/operational burden and priority.

## Content fields — section 08

Use the brief's field-table format for place, route, district/region relations, photo/attribution, source and fact-verification record. Capture:

- AZ/EN/RU names and name verification status.
- Stable IDs, parent relations and many-to-many place/district and route/place links.
- Claim-level sources and publication/effective/as-of/verification dates.
- Access status, visitor groups, dated prices, units, coordinate purpose and uncertainty.
- Photo source page, creator and verified license/reuse conditions.
- Null versus zero/free/not-applicable and behavior when data is unavailable.

Propose a simple editorial recheck practice for changing access, fees, hours, transport and road conditions. Frequency and publishing rules are editorial proposals, not scheduled automations. No database migration, framework choice or software architecture is required.

## MVP and phasing — section 09

Select approximately 20 places and 5 routes from the canonical inventory, only to the extent supported. Use evidence quality, confirmed access, geographic/category/scenario balance, reusable project content and maintenance effort. Explain choices and exclusions, including how unresolved access affects readiness. Do not silently treat the entire official inventory as visitor-ready.

Use qualitative priorities and the brief's three feature groups: first-version essential, useful later and deferred now. Do not manufacture RICE reach, impact estimates, visitor demand, engineering capacity or dates. If numerical scoring is explicitly requested, label every assumption and explain that it is an editorial model rather than measurement.

Show dependency chains: verified access/entrance before navigation, usable fields before filters, confirmed data supply before live features. Produce the requested priority table with missing information and next work. Planning does not authorize writing tickets, assigning owners, contacting anyone or publishing the report.
