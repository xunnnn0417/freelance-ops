# freelance-ops

Public control center for freelance sourcing, screening, proposals, execution, QA, delivery, and handoff continuity.

## Rules
- Cash-flow-first: prioritize live, legitimate paid work that can be delivered with ChatGPT/Codex/Python/browser/spreadsheets plus limited user input.
- Never invent certifications, employment history, client work, ratings, or portfolio results.
- Every promising job gets safety screening, deliverability review, an execution plan, and client-facing quality checks.
- Use samples/templates honestly labeled as samples.
- Stop at user-only boundaries: first-time registration, 2FA, identity verification, legal agreements, paid Connects/tools, formal contract acceptance, or missing private client data.
- This repository is public for now. Store only public/sanitized information; never commit private client files, secrets, credentials, personal contact data, or contract-confidential material.

## Core files
- `WORKFLOW.md` — standard operating procedure
- `CASE_INDEX.md` — current cases, status, blockers, next actions
- `cases/` — sanitized per-case briefs and execution plans
- `templates/` — reusable proposal/update/delivery/QA templates
- `tools/` — reusable scripts and third-party license notes

## Rollover rule
Before a control-chat rollover: sync GitHub → produce handoff → open the next control chat → read back `CASE_INDEX.md` and `WORKFLOW.md` → verify active cases/blockers → stop adding work to the old chat.
