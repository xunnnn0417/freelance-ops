# Case 25 — Upwork — AI Lead Generation System Demo

Status: Candidate / proposal ready / 0 Connects
Checked: 2026-10-06 Asia/Taipei

## Public listing
- Platform: Upwork
- Title: AI Lead Generation System
- Posted: Oct 5, 2026 (~4 hours old at check)
- Worldwide
- Hourly: US$20–50/hr
- Duration: 6+ months, 30+ hrs/week shown
- Contract-to-hire
- Client: Cyprus, member since Sep 15 2024
- Activity at check: 20–50 proposals, 15 interviewing, 31 invites, 11 unanswered

## Scope
Client wants a demo-first system that finds Instagram/YouTube leads for USA marketing agency owners using follower/subscriber count, niche keywords, coaching offer, USA/UK/AU region, English language, last-30-day views, and excluding faceless channels. Client explicitly says they do not want to pay for the full system until they know they can sell it; if their buyers invest, they will pay for the system to be built.

## Safety / commercial review
- No public request for crypto, gift cards, off-platform payment, suspicious download, or unnecessary sensitive data.
- Main commercial risk: unpaid-demo wording. Do NOT build a full production system for free. Offer a deliberately limited, non-production demo/PoC with a small result set or recorded walkthrough. Full implementation begins only under an Upwork-funded contract/milestone.
- Client history/spend is not visible in the indexed result, so confidence is lower than established-client jobs.
- High competition/interview count lowers expected win probability.

## Fit
Estimated deliverability: 85–90% for a bounded demo; 75–85% for production until exact data-source/API constraints are known.
ChatGPT/Codex/Python can handle architecture, filtering, scoring, deduplication, exports, test fixtures, documentation, and most implementation. Production Instagram/YouTube collection must respect official APIs/platform terms and rate limits; do not promise unrestricted scraping.

## Proposal
Hi — I’d approach this as a small sellable demo first, not a large build before you’ve validated demand.

For the demo I can take a bounded sample of Instagram/YouTube prospects, apply the filters you listed (niche, geography/language, audience size, recent views, coaching offer and faceless-channel exclusion), and return a clean prospect table with the reason each lead passed the filter. I’d also include duplicate handling and a manual-review flag where a criterion can’t be verified confidently.

That gives you something concrete to show agency owners without pretending the first version is already a production-scale scraper. If the demo validates, the same pipeline can then be hardened around the agreed data sources/APIs, logging, retries and export/CRM workflow.

I can build the demo architecture and QA flow immediately. I would keep the initial PoC deliberately limited; the full production system would start once there is an Upwork-funded contract/milestone.

## Blocker
Current Upwork Connects balance is 0. Do not purchase Connects. Apply only if free Connects, an invitation, or another genuinely free official route becomes available.
