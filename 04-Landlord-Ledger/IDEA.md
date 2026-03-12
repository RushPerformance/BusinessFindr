# Landlord Ledger

> Simple rental property accounting for small landlords (1-10 units): tracks rent, expenses, generates Schedule E tax reports, and sends late payment reminders.

| Field | Detail |
|-------|--------|
| Category | Home & Property / Finance |
| Target Audience | Small landlords with 1-10 rental units |
| Monetization | Subscription — $9.99/mo per portfolio (unlimited units up to 10) |
| Recession Resistance | High — rental properties don't disappear in recessions; landlords need expense tracking regardless of economic conditions, and proper tax documentation becomes more important when margins tighten |
| Solo-Dev MVP Timeline | 7 weeks |
| Composite Score | 87/100 |

## The Problem
There are 10.6 million individual landlords in the US, and 72% own fewer than 5 units (US Census, American Housing Survey). These small landlords overwhelmingly use spreadsheets or shoeboxes for accounting — enterprise tools like AppFolio ($280/mo minimum) and Buildium ($55/mo + per-unit fees) are overkill and overpriced. r/landlord (350K members) is filled with posts asking "what do you use to track rent and expenses?" The #1 pain point is generating Schedule E tax forms — most landlords don't even know what expenses are deductible.

## The Solution
1. Add properties and units with address, purchase price, mortgage details
2. Track rent payments (mark paid/late/partial) with automated late-payment reminders via text/email
3. Log expenses with receipt photo scanning (categorized by IRS Schedule E line items)
4. Bank account connection via Plaid for auto-importing property-related transactions
5. One-click Schedule E report generation at tax time
6. Maintenance request tracker (tenant submits, landlord assigns/tracks)
7. Lease document storage

## Market Size
- **TAM**: $22B — US property management software market (Fortune Business Insights, 2023)
- **SAM**: $2.2B — small landlord segment (1-10 units)
- **SOM**: $5.5M — 46,000 subscribers at $10/mo

## Existing Alternatives
- **AppFolio**: $280/mo minimum — way too expensive for small landlords
- **Buildium**: $55/mo + per-unit fees — still pricey
- **Stessa**: Free basic, but acquired by Roofstock and pivoting to investor tools
- **Avail (Realtor.com)**: Free-ish but limited, clunky UX, pushing realtor services
- **Excel/Google Sheets**: Universal but no automation, no tax reports, no reminders
- **TurboTax**: Does Schedule E but doesn't track ongoing income/expenses

## Why This Wins
- Price point ($10/mo) is 5-28x cheaper than enterprise competitors
- Schedule E auto-generation is the killer feature — saves $200-500 in CPA fees
- Vertical focus on small landlords means simple UX, not enterprise complexity
- Receipt scanning + auto-categorization by Schedule E line items is unique

## Revenue Potential
- **Year 1**: $150K (1,250 subscribers × $10/mo)
- **Year 3**: $1.5M (12,500 subscribers × $10/mo) with referral program among landlord communities
