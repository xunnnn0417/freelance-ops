# Upwork — Bank Statement PDF to CSV — Ready Before Connects

## Public job facts
- Title: Type bank statement transactions from PDF into CSV (30 files, ~1,300 rows)
- Upwork opening UID: 2104732589492671823
- Detail route: https://www.upwork.com/jobs/~022104732589492671823
- Fixed price: US$250
- Worldwide
- Intermediate
- Payment method verified
- Client total spent shown: US$514
- Required Connects: 13
- Activity observed: 50+ proposals, 3 hires, 1 interviewing
- Milestones: US$30 for first 2 files within 48 hours; US$220 for remaining 28 files.

## Scope
Manual transcription because PDF text layer is corrupted.
Three CSV columns:
- Date (MM/DD/YYYY)
- Description exactly as printed
- Amount (money in positive; money out negative)

Per-statement QA:
- positives sum to printed Total Deposits/Credits
- negatives sum to printed Total Checks/Debits
- Previous Balance + credits - debits = Ending Balance
- If reconciliation fails, find the missing or mistyped row before delivery.

## Pre-send QA
- Excellent match for careful spreadsheet work and reconciliation.
- No accounting categorization or financial judgement required.
- No platform-outside payment request.
- Client payment verified.
- Main downside: 50+ proposals and job is about one week old.
- Do not boost proposal unless separate ROI review supports it.

## Screening answers
Question 1:
Assuming the statement header confirms the transaction year is 2024:
`01/02/2024,"DBT CRD 0254 12/28/23 20446980 HERTZ TOLL 92601915 VANCOUVER CD C#5506",-60.78`

If the statement header indicates a different year, use the statement year rather than guessing.

Question 2:
If the calculated credits are US$340 higher than the statement total, the first likely causes are:
1. a credit/deposit was duplicated or entered with the wrong amount;
2. a debit marked with a trailing minus was accidentally entered as a positive amount and therefore included in the credit total.

First check:
Filter the positive rows and reconcile them line-by-line against the statement's printed credit entries, starting with an exact US$340 value or a small combination that explains the difference; then check all trailing-minus transactions for sign errors.

## Draft proposal
Hi — I read the reconciliation requirements and would treat each statement as its own mini QA check, not just a typing task.

1) Assuming the statement header confirms the transaction year is 2024:
01/02/2024,"DBT CRD 0254 12/28/23 20446980 HERTZ TOLL 92601915 VANCOUVER CD C#5506",-60.78

2) If credits are US$340 too high, I would first suspect either a duplicated/mistyped credit or a trailing-minus debit that was entered as positive. I would filter the positive rows and reconcile them line-by-line to the printed credit entries first, then check every trailing-minus transaction for sign errors.

For each file I would verify the positive total, negative total, and Previous Balance + credits - debits = Ending Balance before delivery. If the numbers do not reconcile, I would correct the row before sending the file back.

I can start with the 2-file milestone and follow the provided CSV templates exactly.

## Status
Prepared / blocked only by Connects. Do not apply until Connects are available and a final pre-send QA is repeated.
