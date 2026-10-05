# Execution Plan — Case 08

1. Receive source files/instructions and preserve the client's column order and naming.
2. Create a working copy; never overwrite raw source.
3. Enter/import records in batches.
4. Normalize only explicitly allowed formatting (whitespace, obvious casing/format rules); do not infer unknown values.
5. QA pass: required-field completeness, duplicate rows/IDs, consistent date/number/text formats, malformed URLs/emails only if those fields exist, and row-count reconciliation against source.
6. Flag ambiguous/missing source values rather than guessing.
7. Deliver clean workbook plus a short note listing flagged rows and checks performed.

## QA checklist
- [ ] Raw source preserved
- [ ] Row count reconciled
- [ ] Required fields checked
- [ ] Duplicates checked
- [ ] Formatting consistent
- [ ] No invented values
- [ ] Ambiguities flagged
- [ ] Workbook opens cleanly and filters/headers remain usable

## Time/value guardrail
Because the budget is US$50 fixed, keep automation lightweight. If the source volume implies an unreasonable effective hourly rate, clarify scope before accepting the contract rather than silently expanding work.
