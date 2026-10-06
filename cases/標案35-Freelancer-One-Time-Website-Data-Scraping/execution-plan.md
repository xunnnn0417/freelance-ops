# Execution plan — Case 35

1. Intake: capture target URL, allowed/public scope, fields, image requirement, output schema, deadline.
2. Preflight: inspect robots/ToS/access pattern; identify static vs JS-rendered pages; estimate page count.
3. Small paid/limited validation sample: 10–20 representative records only if needed.
4. Build: Scrapy crawler; Beautiful Soup parsing fallback; browser automation only if legitimately necessary for public JS-rendered content.
5. Reliability: throttling, retries, timeouts, canonical URLs, pagination handling, checkpointing, structured logs.
6. Transform: normalize whitespace/types/URLs; preserve source URL; deduplicate deterministically.
7. QA: schema validation, required-field/null checks, duplicate checks, row-count reconciliation, random manual source audit.
8. Deliver: CSV/JSON, optional image folder, requirements/dependencies, commented source, README.
9. Final impression check: filenames, clean columns, reproducible commands, concise limitations/errors report.
10. Fallback: if site structure or policy prevents safe extraction, report the blocked subset and propose a compliant alternative instead of bypassing controls.
