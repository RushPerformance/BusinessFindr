# Business Model: Side Hustle Tax Tracker

## Value Proposition
Side hustlers know exactly how much to set aside for taxes after every payment — no surprise April bill, no overpaying a CPA, no spreadsheet math. The app saves the average user $200-$500/year in avoided penalties and unnecessary accountant fees.

## Customer Segments
- **Primary**: Ages 22-40, earning $1K-$20K/year from Etsy shops, DoorDash/Uber driving, freelance writing, tutoring, or reselling. They have a W-2 day job and their side income is "extra" money they don't want eaten by surprise taxes. They're anxious about IRS rules but not financially sophisticated enough for QuickBooks.
- **Secondary**: Gig economy workers (Uber, Instacart, TaskRabbit) earning $20K-$50K/year who need lightweight expense tracking without the overhead of full accounting software.
- **Psychographics**: Pragmatic, slightly anxious about taxes, price-sensitive (won't pay $15/mo for Keeper Tax when they're earning $500/mo on the side). They Google "do I have to pay taxes on Etsy income" and "how much tax on side hustle."

## Revenue Model
- **Free tier**: Log income and expenses manually; see estimated annual tax liability; get the $400 self-employment threshold explainer
- **Paid tier**: $4.99/month or $39.99/year — unlocks bank connection for auto-import, receipt photo scanning, quarterly payment reminders with pre-filled vouchers, state tax calculations, and Schedule C/SE export
- **Premium/Enterprise**: N/A (individual consumer product)
- **Projected conversion rate**: 6% free-to-paid (benchmarked against Mint's historical 4-5% and Keeper Tax's ~8%, weighted to middle given lower price point)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS/Vercel) | $75 |
| APIs/Services (Plaid bank connection, OCR for receipts, tax calculation engine) | $450 |
| Marketing (SEO content, Reddit, seasonal ads) | $500 |
| Total Monthly Burn | $1,025 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $12 |
| LTV | $108 (avg 22-month retention at $4.99/mo; side hustle tax is an annual recurring need) |
| LTV:CAC | 9:1 |
| Payback Period | 2.4 months |
| Gross Margin | 85% |

## Go-to-Market: First 100 Users
1. **Reddit (weeks 1-6)**: Post value-first content in r/sidehustle (220K), r/EtsySellers (130K), r/UberDrivers (115K), r/freelance (280K), and r/tax (340K). Share free tax calculators and "here's what most side hustlers get wrong about quarterly taxes" breakdowns. Link to app as the automated version.
2. **SEO (weeks 1-12)**: Publish 15 long-tail articles: "do I need to pay quarterly taxes on Etsy income," "side hustle tax deductions list 2026," "how much tax on $5,000 side income." These queries spike Q4 through April — plant content early.
3. **YouTube (weeks 4-8)**: Partner with 3-5 small finance/side hustle YouTubers (10K-50K subscribers) for sponsored walkthroughs. Cost: $200-500 per creator. Target creators like "Side Hustle Nation" or Etsy-focused channels.
4. **Tax season blitz (January-April)**: Run Google Ads on "side hustle tax calculator" ($1.50-$2.50 CPC); create a free "Side Hustle Tax Estimator" landing page that funnels to the full app.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 5,000 | $114K | 1,900 paid users; heavy SEO investment; organic Reddit and YouTube growth |
| 2 | 18,000 | $420K | SEO compounds; tax season virality; 7,000 paid users |
| 3 | 45,000 | $1.2M | 20,000 paid users; partnerships with gig platforms for distribution |
| 4 | 80,000 | $2.1M | 35,000 paid users; annual plan adoption rises to 40%; referral program launches |
| 5 | 130,000 | $3.4M | 55,000 paid users; expand to 1099-NEC filing (not just tracking); B2B gig platform API licensing |

## Key Weekly Metrics
1. Weekly active users logging income or expenses (target: 60% WAU/MAU)
2. Free-to-paid conversion rate (target: 6%)
3. Quarterly payment reminder completion rate (did the user actually file?)
4. Monthly churn rate (target: <4.5%)
5. Average revenue per user (target: $4.75/mo blended across monthly/annual)
6. SEO traffic to tax calculator landing pages (target: 5,000/week by tax season Year 2)
7. Receipt scan success rate (OCR accuracy target: >92%)

## Top 3 Risks
1. **Tax calculation accuracy** — Incorrect tax estimates could cause users to underpay (IRS penalties) or overpay (eroding trust). Tax rules change annually and vary by state. → Mitigation: Partner with a tax data provider (e.g., Tax Foundation or Avalara) for rate tables; add disclaimers; run annual audits against CPA-prepared returns for accuracy validation; start with federal + top 10 states only.
2. **Extreme seasonality** — Sign-ups spike January-April and crater May-September, creating uneven cash flow and high seasonal churn. → Mitigation: Offer annual plans at a discount ($39.99/yr vs. $4.99/mo) to lock in full-year revenue; build year-round engagement features like expense categorization and income goal tracking; time product launches to tax season.
3. **Plaid costs scaling** — Bank connection via Plaid costs $0.30-$1.50 per connection, which can eat margins at scale for a $5/mo product. → Mitigation: Make bank connection a paid-only feature (free tier is manual entry only); negotiate volume discounts with Plaid at 5,000+ connections; explore alternative providers (MX, Finicity) for better rates.
