# Ecommerce listing preflight — small work sample

> **Synthetic demo; not a client engagement.** All products and IDs below are fictional. This sample illustrates spreadsheet QA **before** uploading to Shopee/momo/other marketplaces. It is not a claim of prior customer deliveries or direct marketplace automation experience.

## Example source sheet

| Row | SKU | Product title | Option | Price (TWD) | Image path | Observation |
|---:|---|---|---|---:|---|---|
| 2 | DEMO-101 | 玻璃水杯 350ml | 透明 | 199 | photos/101.jpg | Complete |
| 3 | DEMO-102 | 棉質收納袋 | 米白 / M | 149 | photos/102.jpg | Complete |
| 4 | DEMO-103 | 桌面收納盒 | 白色 | 329 | photos/103.jpg | Complete |
| 5 | DEMO-103 | 桌面收納盒 | 白色 | 329 | photos/103.jpg | Repeated SKU and variant |
| 6 | DEMO-105 | 不鏽鋼保溫瓶 | 黑色 / 500ml | 590 | *(blank)* | No product image reference |
| 7 | DEMO-106 | 筆記本 A5 | 綠色 | *(blank)* | photos/106.jpg | Missing source price |
| 8 | DEMO-107 | 筆記本 A5 | 藍色 | 120 | photos/107.jpg | Check whether a second SKU / parent grouping is needed |

## Pre-upload exception list

| Priority | Row | Rule | Required action |
|---|---:|---|---|
| Hold | 5 | Identical SKU + variant appears twice | Verify whether record 5 is a true duplicate before removing it |
| Hold | 6 | Missing image reference | Ask for corresponding image or explicit permission to leave unpublished |
| Hold | 7 | No price supplied | Ask the source owner; **never guess selling price** |
| Review | 8 | Parent/variation structure unresolved | Compare against the marketplace's latest valid import template |
| Pass | 2–4 | Required sample fields present | Ready for further platform-specific checks |

## Paid pilot scope (discussion framework; **no quote yet**)

- **Input:** client-supplied product sheet, image files, current marketplace field template, and any variant rules.
- **Process:** column map → normalize whitespace/formats → identify duplicate SKU/variant → missing-field checks → human review of ambiguous items → final sample QA.
- **Outputs:** clean spreadsheet, exception list with original row references, and compact QA summary. Marketplace upload is **separately scoped** depending on account authorization.
- **Acceptance:** 100% of required rows either mapped or listed as unresolved; never fabricate missing descriptions, prices, photos, attributes, or manufacturer facts.
- **Out of scope unless separately agreed:** image editing, copywriting, catalog/category strategy, pricing decisions, mass uploading with credentials, sales guarantees, advanced variation reconstruction.

**Commercial notes:** offer a paid 20–50-item trial only after the client shares a representative *non-confidential* sample and confirms final columns, variant counts, platform and timeline. No unpaid production-scale work.

*Prepared as a reusable example for agency overflow inquiries in October 2026.*
