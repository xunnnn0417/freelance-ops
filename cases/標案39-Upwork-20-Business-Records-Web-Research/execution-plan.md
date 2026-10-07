# Execution Plan

1. Confirm the agreed industry and location before collecting records.
2. Build a fixed schema: Company | Official Website | City | State | Contact Page | Public Business Email | Source URL | QA Note.
3. Research candidate businesses from legitimate public sources.
4. Resolve each candidate to its official website; reject ambiguous matches.
5. Capture the contact-page URL and only emails visibly published by the business or an authoritative public source.
6. If no public email is found, enter "Not found"; never infer or pattern-generate one.
7. Normalize company names, URLs, city/state formatting and email casing.
8. Deduplicate by normalized company + official domain.
9. QA all 20 rows: official-domain match, source URL opens, location match, no duplicates, no guessed emails.
10. Deliver XLSX or Google Sheet within the client's two-day window.

## Fallbacks
- Ambiguous company identity: exclude and replace with a better-supported business.
- JS-heavy contact page: browser-based inspection, without bypassing access controls.
- No email: "Not found".
- Conflicting addresses: retain the location supported by the official site and note the conflict.

## Pre-delivery quality gate
Exactly 20 valid businesses; all required columns present; 0 duplicates; every non-"Not found" email has a traceable public source; formatting is consistent; filenames and sheet name are professional.
