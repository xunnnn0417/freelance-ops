# Case 18 — Execution Plan

1. Receive directory URL/source and exact required columns after contract/test starts.
2. Inspect robots/site terms and page structure. Use only publicly accessible business information and avoid bypassing access controls.
3. Choose lowest-complexity extraction path: requests/BeautifulSoup for static HTML; Scrapy for scalable pagination/profile traversal; Playwright only if JS rendering is necessary.
4. Capture source URL and raw values for traceability.
5. Normalize whitespace, company names, phone formats, URLs, state/location fields, and empty values without inventing missing facts.
6. Research missing business fields only from public authoritative/first-party sources when practical; preserve source URL.
7. Deduplicate using deterministic normalized keys plus manual review of fuzzy/ambiguous candidates.
8. QA: total profile count vs output rows; required-field completeness; duplicate count; invalid URL/phone checks; random sample review; exception sheet for unresolved records.
9. Deliver XLSX/Google Sheet with clean headers, filters/freeze panes, readable widths, source URL, and optional QA/Notes column.
10. Keep client data/source material out of the public `freelance-ops` repo.

Fallback: if anti-bot controls or site terms make automation inappropriate, switch to manual/semi-automated collection and renegotiate scope/price before doing the full directory.