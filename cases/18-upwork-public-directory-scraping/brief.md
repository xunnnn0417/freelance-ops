# Case 18 — Upwork — Public Business Directory Research & Collection

Status: Candidate / proposal ready / 0 Connects
Checked: 2026-10-06 Asia/Taipei

## Listing
- Platform: Upwork
- Public title: SCRAPING sites for Realtors
- URL: https://www.upwork.com/freelance-jobs/apply/SCRAPING-sites-for-Realtors_~022106918692204216768/
- Budget shown: US$30 fixed
- Worldwide, one-time, Expert
- Posted October 5, 2026
- Activity at check: 20–50 proposals, 3 interviewing, 1 invite, client last viewed ~12h ago
- Client: United States; member since 2013; ~US$13K spent; 224 hires; 25 active; 590 hours

## Scope
Client supplies source material after hiring. Work through a large public business directory A–Z, open individual profiles, collect specified public business information, research missing fields from public sources, remove duplicates, and deliver a clean Excel/Google Sheets database. Several hundred records. Automation or manual methods are allowed. Client may start with a paid test.

## Safety
No public request for upfront payment, crypto, gift cards, suspicious downloads, off-platform payment, or private/sensitive personal data. Scope is public business-directory research. Main risk is economic: US$30 is too low for several hundred records unless it is only the initial/test budget or client accepts a materially higher full-project quote.

## Fit
Technical deliverability: ~90% once source directory/fields are provided. Python/Scrapy/Playwright/pandas + manual exception review can handle extraction, normalization, deduplication, and QA. No need to claim prior paid scraping clients; use truthful GitHub/automation work and a small sample if source becomes available.

## Open-source quality enhancement
- Scrapy (`scrapy/scrapy`) is a mature public scraping framework with a BSD-style 3-clause license, suitable for commercial use subject to its notice/disclaimer requirements.
- Prefer a simple requests/BeautifulSoup path when the directory is static; use Scrapy for scale; Playwright only for JS-rendered pages.
- QA should include normalized URLs/phones, deterministic dedup keys, required-field completeness, row-count reconciliation, source URL per record, and manual review of ambiguous matches.

## Proposal draft
DIRECTORY PROJECT

I can handle this as a structured data-collection job rather than simple copy/paste: extract the public directory records, normalize the requested fields, research missing business details from public sources, remove duplicates, and run a final completeness/accuracy check before delivery.

For several hundred records, I would normally automate the repeatable parts with Python where the site structure allows it, then manually review exceptions and ambiguous records. I can deliver in Excel or Google Sheets and keep a source URL for each record so the data is auditable.

I’m happy to begin with the paid test. Once I can see the directory and required columns, I can confirm the realistic turnaround and fixed price for the full directory rather than guessing from the listing alone.

## Bid rule
Do not bid US$30 for the entire several-hundred-record directory unless the actual scope proves unusually small/fast. Treat US$30 as acceptable only for a paid test or small first milestone. If the full project requires several hours, quote after inspecting source/fields.

## Blocker
Upwork account currently has 0 Connects. Do not buy Connects. Keep proposal ready for free Connects, invitation, or another genuinely free application route.