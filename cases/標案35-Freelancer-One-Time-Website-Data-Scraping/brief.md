# 標案35｜Freelancer｜One-Time Website Data Scraping｜Proposal Ready

- Platform: Freelancer
- Project ID: 40752808
- URL: https://www.freelancer.com/projects/data-scraping/one-time-website-data-scraping
- Budget: US$250–750 fixed
- Status: Open; posted 2026-10-06; 6 days remaining when screened
- Competition at screening: 166 proposals; average bid ~US$399
- Scope: one-off extraction of publicly available information from one website; Python preferred; CSV/JSON (+ images if in scope); commented script; README; polite throttling / robots respect.
- Deliverability: 92% after target URL and exact fields are provided.
- User dependency: target website, exact desired fields, any authorized credentials if login is legitimately required.
- Paid tools: none assumed.
- Safety: platform-mediated project; no visible request for upfront payment, crypto, gift cards, Telegram/WhatsApp, or suspicious executable. Do not bypass authentication, CAPTCHA, access controls, or explicit site restrictions.
- Commercial risk: scope is underspecified (“everything of value”), so bid must condition price/timeline on URL + final field list. Competition is high.
- Recommendation: worth bidding only through a zero-cost official bid route.

## Open-source quality enhancement
Use Scrapy (BSD-3-Clause) as the primary crawler when site structure suits it; Beautiful Soup (MIT) for parsing/fallback. Add AutoThrottle/retry, canonical URL normalization, deduplication, structured error log, schema validation, row-count reconciliation, and a small manual sample audit.

## Proposal
Hi — I can build this as a rerunnable Python extraction rather than a one-off manual dump.

I’d first map the target site and agree the exact output fields, then crawl it with polite throttling, normalize/deduplicate the results, and run a QA pass before delivery. You’ll receive the cleaned CSV/JSON, the commented source, and a short README with setup/run instructions.

For the current US$250–750 range, I’d confirm the final fixed price after seeing the target URL and whether the scope is text/tables only or also includes images/dynamic pages. I won’t rely on paid scraping services unless you explicitly approve them.

If you send the target URL, I can quickly confirm the extraction plan and likely turnaround before we lock the milestone.

## Blocker / next step
Need the target website and final field scope from the client before production work. Do not produce a large unpaid sample. If Freelancer requires deposit/balance/payment to bid, stop rather than funding the account.
