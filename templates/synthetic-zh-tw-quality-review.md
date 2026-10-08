# Traditional Chinese (Taiwan) language QA — synthetic practice
**Independently created training example, NOT a client delivery, professional translation credential, or Lionbridge qualification result.** Only public synthetic sentences are used.

## Goal
Practice comparing a source statement with a candidate Traditional Chinese (Taiwan) translation, deciding *pass / fail / needs review* under an explicit rubric. Real paid projects must use their own employer-supplied grading rubric.

## Rules (example only)
- **Fail/Meaning**: mistranslates facts, dates, amounts, negation, obligations or conditions.
- **Fail/Omission**: leaves out critical qualifying information.
- **Needs review/Naturalness**: literal calque, awkward phrasing or unsuitable Taiwan usage, but source meaning mostly survives.
- **Pass**: meaning preserved with natural wording, including acceptable paraphrase; don't penalize harmless style differences.
- If evidence insufficient, **flag uncertainty** rather than guessing.

| ID | English source | Candidate zh-TW | Decision | Rationale |
|---|---|---|---|---|
| EX-01 | The report is due **before** Friday. | 報告須在星期五**之前**繳交。 | Pass | Deadline condition retained |
| EX-02 | The discount applies **only** to new accounts. | 所有帳號都能使用這項折扣。 | Fail/Meaning | Incorrectly broadens scope; loses *only* |
| EX-03 | Do not share the access code with anyone. | 請將存取碼分享給所有人。 | Fail/Meaning | Reverses prohibition |
| EX-04 | Please attach a receipt if you have one. | 如有收據，請一併附上。 | Pass | Optional conditional preserved |
| EX-05 | Your request is being processed. | 你的請求正在被進行處理中。 | Needs review/Naturalness | Understandable but stilted passive wording;「正在處理您的申請」might be more natural depending on style |
| EX-06 | The package includes two cables, but **no charger**. | 包裝內含兩條線材及充電器。 | Fail/Meaning | Negation omitted; wrongly includes charger |
| EX-07 | Please contact support **within 30 days**. | 請在**30 天內**聯絡客服。 | Pass | Duration preserved |
| EX-08 | Available in the US **except** Alaska. | 在美國全境均可使用，**包含**阿拉斯加。 | Fail/Meaning | Exception reversed |

## Review and communication template
| Item | Decision | Error type | Confidence | Explanation (max 1 sentence) |
|---|---|---|---|---|
| e.g. EX-02 | Fail | Scope constraint lost | High | Source permits new accounts only |
| e.g. EX-05 | Needs review | Naturalness | Medium | Stilted passive construction without material semantic error |

## Quality gates
- Are negation, modality, conditions, quantities and deadlines checked?
- Did the reviewer distinguish factual error from style preference?
- Do regional terms fit Taiwan readers without changing meaning?
- Is there a **source-backed** reason for each fail?
- Was confidential/third-party source content excluded from any public sample?

*For demonstrating a learning/QA process, not representing prior professional assignments.*
