# Case 09 Execution Plan

## Goal
Reconcile approximately 645 client contacts from the authoritative PDF/Excel master list against SwarmCRM without silently changing uncertain data.

## Workflow
1. Receive client master file and SwarmCRM access.
2. Preserve the original master file unchanged.
3. If PDF, extract/structure it only as needed and verify extracted values against the visible source before using them for edits.
4. Create a local reconciliation tracker with: source row/id, source name, CRM match status, fields checked, fields changed, ambiguity flag, notes, completed timestamp.
5. Search SwarmCRM one contact at a time using the source name and secondary identifiers when needed.
6. Compare name, phone(s), email(s), lead information, primary address.
7. Update only when the master value is clear. Never infer a missing phone/email/address.
8. Flag no-match, multiple-match, or contradictory records for client review.
9. Run completion QA and deliver a concise exception summary.

## QA gates
- Reconciled count + flagged count = source record count (~645).
- No source row is silently skipped.
- Duplicate source identities are flagged before CRM edits are merged.
- Normalize whitespace/casing for comparison without changing source meaning.
- Phone/email comparison may use normalized forms, but CRM writes preserve the client's authoritative value/format unless instructed otherwise.
- Randomly re-check at least 5% of completed contacts against the master list.
- If an export is available after editing, run a local reconciliation diff against the master and review all remaining discrepancies.

## Tooling
- Spreadsheet tracker: Excel/Google Sheets locally/client workspace.
- Optional local QA: concepts/tooling from MIT `crm-data-quality`; Apache-2.0 `pyxl_validator` for Excel comparisons.
- No client contact data in public GitHub, third-party demos, or unapproved services.

## Fallbacks
- SwarmCRM search produces multiple people: do not guess; use phone/email/address to disambiguate or flag.
- PDF text extraction is unreliable: visually verify source rows rather than trusting OCR/extraction.
- CRM lacks a requested field: log as schema limitation and ask client via Upwork message rather than mapping it arbitrarily.
- Bulk editing/import is offered: do not use it unless client explicitly approves; the brief asks for master-list verification and correctness is more important than speed.

## Delivery note template
Completed the reconciliation against your master list. I checked all source records, updated clear mismatches/missing fields, and kept ambiguous cases separate rather than guessing. I’m also including the exception count/notes so you can review anything that needs a business decision.