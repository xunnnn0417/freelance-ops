# Case 09 — Upwork — SwarmCRM Contact Reconciliation

Status: Candidate / proposal ready
Checked: 2026-10-06 Asia/Taipei

## Listing
- Title: Cross-Reference Follow Up Boss Contacts With SwarmCRM
- Platform: Upwork
- Pay: US$60 fixed
- Scope: ~645 contacts
- Task: use the client's PDF/Excel master list as source of truth, search each contact in SwarmCRM, verify/update name, phones, emails, lead info, and primary address.
- Client: USA; member since 2025-05-14; US$652 spent; 4 hires; 1 active at check.
- Activity at check: 20–50 proposals, 2 interviewing, 4 invites.
- Listing: https://www.upwork.com/freelance-jobs/apply/Cross-Reference-Follow-Boss-Contacts-With-SwarmCRM_~022106782465685923872/

## Safety
No public request for off-platform payment, advance purchase, crypto, Telegram/WhatsApp, suspicious downloads, or unnecessary sensitive identity data was observed. Work necessarily involves client CRM/contact data, so keep all client exports private and out of this public repository.

## Deliverability
Estimated deliverability: 95% once the client grants CRM access and supplies the master file. The task is procedural and can be accelerated with a local reconciliation/QA worksheet, but final CRM edits should remain deterministic and reviewable.

Main dependency: client-provided SwarmCRM access + master PDF/Excel. These cannot be created in advance.

## Economics
US$60 / 645 contacts = about US$0.093 per contact. This is worthwhile only if the workflow is efficient. At 30 sec/contact it is ~5.4 hours before QA (~US$11/hr gross); at 60 sec/contact it is ~10.75 hours (~US$5.6/hr). Proposal should therefore emphasize systematic cross-checking and batch QA, and we should inspect the Connects requirement before spending anything.

## Open-source quality enhancement
Candidate tools reviewed:
- `averya34/crm-data-quality` — MIT; validation, duplicate detection, reconciliation, reviewable rules, zero dependencies. Strong conceptual/tooling fit for pre/post reconciliation QA.
- `Rentenatus/pyxl_validator` — Apache-2.0; Excel row/cell comparison and highlighted discrepancies. Useful if the source is Excel and a post-export comparison is available.

Do not upload client contact data to GitHub. If used, run tooling locally on client-authorized data only.

## Proposal draft
Hi — I can work through the 645 contacts systematically and use your PDF/Excel master list as the source of truth for every change in SwarmCRM.

My workflow would be: match each contact, verify the required fields, update only clear mismatches/missing values, flag ambiguous records instead of guessing, and keep a simple reconciliation log so the full list can be checked for skipped or duplicate contacts before delivery.

I’m comfortable with Excel-based verification and structured data QA, and I can start as soon as you provide the master file and CRM access. If useful, I can also show you the reconciliation format I’ll use before I begin the full list.

## Next step / blocker
Inspect current listing and Connects requirement. Do not buy Connects without user approval. If Connects are available/free and listing economics remain sensible, apply with the proposal above.