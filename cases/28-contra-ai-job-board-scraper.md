# 標案28｜Contra｜AI Job Board Scraper｜準備完成 / 登入後確認 Apply

## 公開資訊
- 來源：Contra Featured Programming Jobs
- 職缺：AI-Powered Job Board Scraper Development
- 預算：US$300–400 fixed
- 工期：1 week
- 公開頁面標示 programming jobs 可 apply free。
- 公開頁只顯示摘要；完整 scope/client/activity/apply form 需登入後確認。

## 為什麼列為 #1
最接近現有能力與公開作品：Python、資料擷取、研究流程、自動化、結構化資料與 QA。固定範圍、短工期、預算清楚，比長期高資歷角色更有機會快速成交與收款。

## 安全審核
- 目前無先付款、可疑下載、平台外付款或索取憑證跡象。
- 只接受 Contra 平台內 proposal / contract / payment。
- 若登入後要求下載未知執行檔、提供私人帳密、繞過網站存取控制或違反網站條款，停止並重新審核。
- 不承諾繞過 CAPTCHA、登入牆、反機器人或其他技術限制。

## 可交付判斷
可做，但登入後必須先確認：
1. 目標 job boards 數量與名稱。
2. 需要欄位（title/company/location/pay/url/date/etc.）。
3. 是否需要排程、自動去重、AI 分類/摘要、Google Sheets/CSV/API。
4. 是否需要登入站點或處理 CAPTCHA。
5. 資料量、刷新頻率、部署環境與交付方式。
6. 是否只是 prototype / one-time export，或 production scraper。

建議承諾：先做 bounded MVP / extractor pipeline，不在未確認 scope 前承諾大型 production system。

## 估價 / 工期框架
- 公開預算 US$300–400；建議先以 US$350–400 fixed 切入。
- 若只需 1–3 個公開 job boards、欄位標準化、去重、CSV/Sheets：3–5 天主體 + 1–2 天 QA/修正。
- 若需多站登入、排程部署、AI enrichment、proxy/anti-bot，必須重新估價，不硬塞進原預算。

## 自然提案文案
Hi — this looks like a good fit for the kind of research and automation work I build.

I can create a focused Python scraper that collects the required job fields, normalizes them into a clean schema, removes duplicates, and exports the result to CSV or Google Sheets. If AI enrichment is part of the scope, I can keep that as a separate, testable step rather than mixing it into the raw extraction.

For a one-week project, I’d suggest starting with the exact target boards and required fields, then delivering a working first pass early so we can catch layout or data issues before the final handoff.

I also keep the workflow reproducible: documented inputs, validation checks, and clear handling for missing fields instead of guessing values.

Relevant public work:
- github.com/xunnnn0417/finance-analytics-portfolio
- github.com/xunnnn0417/financial-research-assistant

If you share the target job boards and output format, I can confirm the exact scope quickly.

## QA 計畫
- 抽樣比對來源頁 vs 輸出欄位。
- 檢查空值、重複 URL、重複職缺、欄位型別。
- 日期/薪資/地點格式標準化。
- 對抓取失敗頁面保留 error log，不靜默遺失。
- 至少跑 2 次測試確認去重與增量邏輯。
- 最終交付前測試 script 可重跑，README 可讓客戶理解操作方式。

## 登入後要確認
- Apply 是否仍免費。
- 客戶名稱、所在地、付款/招聘歷史。
- proposal 數 / 活躍度 / posted time。
- 完整技術需求。
- 是否要求不存在的 production experience。
- 是否有 anti-bot / login / scraping policy 風險。
