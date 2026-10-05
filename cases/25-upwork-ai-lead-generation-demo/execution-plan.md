# Case 25 — Execution Plan

## Goal
Produce a bounded, credible demo that lets the client demonstrate filtered Instagram/YouTube lead discovery without giving away a production system for free.

## Demo pipeline
1. Confirm a small demo niche and target geography from the listing defaults.
2. Acquire a bounded sample through permitted/available search/API sources; retain source URLs and timestamps.
3. Normalize channel/profile name, URL, platform, region/language, follower/subscriber count and recent-view metrics.
4. Classify niche/coaching-offer/faceless status with deterministic checks plus LLM assistance only where useful.
5. Score each lead against the requested criteria and record pass/fail/uncertain reason per criterion.
6. Deduplicate by canonical profile/channel URL and normalized handle/name.
7. Export a clean Google Sheet/Excel/CSV sample with a `Why qualified` and `Needs review` field.
8. Provide a short architecture diagram/readme describing how a paid production version would scale, without handing over production credentials or a full free build.

## QA
- Never invent unavailable metrics; mark unknown.
- Source URL for every prospect.
- Date-last-verified field.
- Duplicate check on canonical URL + normalized handle.
- Manual review for ambiguous region, coaching offer or faceless classification.
- Sample spot-check before delivery.
- Keep API keys/credentials out of GitHub and deliverables.

## Open-source quality enhancement
Useful permissive references found during screening:
- `serpapi/serpapi-python`: official Python wrapper for structured search / Google Images; useful if the client already has or funds SerpApi. Do not assume API usage is free.
- `SearchApi/n8n-nodes-searchapi`: MIT n8n community node for structured search; useful only if the production architecture uses SearchApi.
- `stephinliji/n8n-templates`: reusable n8n workflow patterns for Google Sheets/OpenAI/automation; inspect individual workflow fit before reuse.

Do not introduce a paid API merely to make the demo look sophisticated. Prefer the client's existing stack or a small permitted manual/API-backed demo, then price production data acquisition explicitly.

## Production fallback
If official APIs cannot expose one of the requested filters reliably, do not claim full automation. Use a two-stage pipeline: automated candidate discovery + human/LLM verification for ambiguous attributes, and report expected throughput/cost before implementation.
