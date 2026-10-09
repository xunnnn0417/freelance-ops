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


## Additional practice — spoken-style zh-TW transcript normalization (2026-10-09)

**Purpose:** Illustrate language-quality control for ASR/transcription projects. All utterances below are invented text, **NOT recordings, real customer audio, paid deliverables, or any employer's qualification test**. Without original audio, no one can independently verify whether a transcription really matches what was said. Always follow the actual employer's style guide instead of imposing these example decisions.

*Illustrative rubric*: check factual preservation **before** cosmetic normalization. A style guide may allow numerals, punctuation or abbreviations differently; those style-dependent cases are marked *Conditional*.

| ID | Invented words as-if spoken (not an audio source) | Draft display text | Example judgment | Why / reviewer next step |
|---|---|---|---|---|
| ASR-01 | 「明天早上九點半開會」 | 「明天早上 9:30 開會。」 | Conditional pass | Same time and intent; use Arabic numerals only if employer's style guide permits |
| ASR-02 | 「這筆費用是五萬元」 | 「這筆費用是 5,000 元。」 | Fail — amount | 50,000 was converted to 5,000; this changes the fact |
| ASR-03 | 「你不用再付款」 | 「你需要再付款。」 | Fail — negation | Reverses the instruction |
| ASR-04 | 「寄到臺中市北屯區」 | 「寄到臺中市北投區。」 | Fail — named entity | Different district; must verify against original recording in a real project |
| ASR-05 | 「這個月三號下午兩點」 | 「本月 3 日下午 2:00。」 | Conditional pass | Date/time preserved, but don't invent the month/year or time zone |
| ASR-06 | 「有三件還沒收到」 | 「有 3 件還沒收到。」 | Conditional pass | Count and unfinished state retained; spacing is style-guide specific |
| ASR-07 | 「我講的是二十三，不是三十二」 | 「我講的是 32，不是 23。」 | Fail — swapped quantities | Numerals reversed, even if punctuation is polished |
| ASR-08 | 「呃，我還不確定」 | 「我還不確定。」 | Needs guide check | Filler omission depends on *verbatim vs clean-read* instruction; do not assume |

### Reviewer checklist for a real recording
1. Verify **audio versus transcript** first; a readable sentence can still be wrong.
2. Keep dates, units, digits, time references, negation, names and qualifiers intact; mark unresolved sound segments as **uncertain**, not made-up content.
3. Separate **meaning-critical error**, **format-only issue**, **regional naturalness**, **inaudible audio**, and **needs rubric clarification**.
4. For each actual issue, report source timestamp or segment ID (only when supplied), draft phrase, issue type, reason, and recommended correction if the employer permits it.
5. Do not upload a client's voice, unreleased test prompts, screenshots, or annotated transcripts to a public GitHub repository without written authorization.

This sample demonstrates **self-directed preparation only**, not professional audio/QC experience or guaranteed accuracy on unseen audio.

*For demonstrating a learning/QA process, not representing prior professional assignments.*
