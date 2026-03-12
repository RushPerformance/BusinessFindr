# Tip Tracker Service Worker

> Tracks daily tips, estimates taxes owed on tip income, and provides income verification documents for loan and apartment applications.

| Field | Detail |
|-------|--------|
| Category | Finance |
| Target Audience | Mass Market — 5.5M tipped workers (servers, bartenders, delivery drivers, hairstylists) |
| Monetization | Subscription — $3.99/mo |
| Recession Resistance | High — tipped workers need to track income regardless of economy; tax obligations are constant |
| Solo-Dev MVP Timeline | 5 weeks |
| Composite Score | 53/100 |

## The Problem
5.5 million Americans work in tipped occupations. Cash tips are notoriously hard to track — most workers don't log them, leading to two major problems. First, tax surprise: the IRS requires reporting all tip income, but workers who don't track face unexpected tax bills or audit risk. Second, income verification: when tipped workers apply for apartments, car loans, or mortgages, they can't prove their full income because cash tips don't appear on pay stubs. Landlords and lenders see only base wages ($2.13-7.25/hr for tipped minimum wage), making workers appear far poorer than they are.

## The Solution
1. Daily tip logging: quick entry of cash tips, credit card tips, and tip-outs by shift
2. Tax estimator: running estimate of taxes owed on tip income with quarterly payment reminders
3. Income verification reports: professional documents showing total earnings (base + tips) for landlords and lenders
4. Shift analytics: best days, worst days, average hourly rate including tips
5. Tip-out tracker: log tip shares to bussers, bartenders, and hosts
6. IRS Form 4070 helper: auto-generate monthly tip reports required by IRS
7. Annual tax summary: total tips by month, estimated 1099 supplement, export for tax prep
8. Goal tracker: "You need $X more in tips this month to hit your income goal"

## Market Size
- **TAM**: $1.8B — US payroll and income tracking tools for gig/service workers
- **SAM**: $360M — tip and income tracking for tipped workers
- **SOM**: $480K — 10,000 paid users × $4/mo

## Existing Alternatives
- **TipSee**: Basic tip tracker, limited features, dated UX
- **Tip Tracker (various)**: Several simple apps, none with tax or income verification features
- **Excel/Notes app**: Most common method, no automation or reporting
- **Payroll systems**: Track credit card tips only, not cash
- **QuickBooks Self-Employed**: $15/mo, overkill for tip tracking

## Why This Wins
- Income verification documents are the killer feature — no competitor helps tipped workers prove their income
- Tax estimation prevents the painful surprise of owing thousands at tax time
- IRS Form 4070 generation automates a tedious compliance requirement
- Deeply underserved market: 5.5M workers with a real financial pain point and no good tool
- Low price point ($4/mo) is accessible to workers who often live paycheck to paycheck

## Revenue Potential
- **Year 1**: $48K (1,000 paid users × $4/mo)
- **Year 3**: $384K (8,000 paid users × $4/mo)
