# Business Model: Landlord Ledger

## Value Proposition
Save 10+ hours/month on rental property bookkeeping and $200-$500 in CPA fees at tax time — with auto-generated Schedule E reports, receipt scanning, and late rent reminders, all for $10/month.

## Customer Segments
- **Primary**: Small landlords aged 35-60 owning 1-5 rental units, earning $60K-$150K/year from their day job plus rental income. They self-manage their properties, track rent in spreadsheets, and dread tax season because they can't remember which expenses are deductible. Active on r/landlord (350K members), BiggerPockets forums, and local real estate investor meetups.
- **Secondary**: New real estate investors (25-40) who just bought their first rental property and are overwhelmed by the bookkeeping requirements. They consume BiggerPockets podcast and YouTube content.
- **Psychographics**: Pragmatic, cost-conscious, DIY-oriented. They chose small-scale landlording over REITs because they like control, but they're not professional property managers and don't want enterprise software.

## Revenue Model
- **Free tier**: 1 property, manual rent tracking, basic expense logging (no auto-categorization, no tax reports)
- **Paid tier**: $9.99/month — unlimited properties (up to 10 units), Plaid bank connection, auto-categorization by Schedule E line items, receipt photo scanning, late payment reminders, one-click Schedule E report
- **Premium/Enterprise**: $19.99/month — maintenance request portal for tenants, lease document storage, multi-owner support (for partnerships), priority support
- **Projected conversion rate**: 12% (benchmarked against Stessa's ~10% freemium conversion; improved by the Schedule E killer feature that free tier deliberately excludes)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS/Railway) | $150 |
| Plaid API (bank connections) | $400 (at $0.30/connection for ~1,300 connected accounts) |
| OCR API (receipt scanning) | $80 |
| Twilio (SMS late payment reminders) | $60 |
| Marketing | $400 |
| Total Monthly Burn | $1,090 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $22 (blended: $8 organic from landlord subreddits/forums + $40 paid via Facebook ads targeting "real estate investor" interests) |
| LTV | $180 (average retention 18 months at $9.99/mo; landlords are sticky — once they set up properties, switching costs are high, benchmarked against Buildium's 24-month SMB retention) |
| LTV:CAC | 8.2:1 |
| Payback Period | 2.2 months |
| Gross Margin | 85% (Plaid + OCR costs ~$1.50/user/month against $9.99 ARPU) |

## Go-to-Market: First 100 Users
1. **r/landlord and r/realestateinvesting**: Post a "How I built a Schedule E auto-generator for my 3 rental units" story. Show before (spreadsheet chaos) and after (clean tax report) screenshots. Landlords on these subs constantly ask for recommendations.
2. **BiggerPockets forums**: Create a detailed "Small Landlord Bookkeeping Setup Guide" in the forums. BiggerPockets has 2M+ members and landlord bookkeeping threads get 50-100 replies.
3. **Tax season content blitz (Jan-Apr)**: Publish "5 Schedule E Deductions Small Landlords Miss" articles and YouTube videos. Drive traffic to a free Schedule E checklist that captures emails.
4. **Local real estate investor meetups (REIA groups)**: Attend 5-10 local REIA meetings. Do a 5-minute demo showing the Schedule E auto-generation. Offer 3-month free trials to attendees.
5. **BiggerPockets podcast ad**: Negotiate a host-read ad on the BiggerPockets Real Estate podcast (1M+ downloads/month). A single episode could drive 200+ signups at $0.50-$1 CPL.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 1,250 paid | $150K | Organic from landlord communities; 12% conversion from 10,400 free users |
| 2 | 4,500 paid | $540K | BiggerPockets partnership; tax season viral loops; referral program |
| 3 | 12,500 paid | $1.5M | Blended ARPU rises to $11 with premium tier; podcast ads |
| 4 | 22,000 paid | $2.9M | Add CPA referral program; partner with property management courses |
| 5 | 35,000 paid | $4.8M | ARPU $11.50; expand to small commercial properties; annual plan adoption improves retention |

## Key Weekly Metrics
1. **Properties added** (leading indicator — each property = a sticky user)
2. **Free-to-paid conversion rate** (target: 12%+)
3. **Schedule E reports generated** (seasonal spike Jan-Apr; validates killer feature)
4. **Bank connections active** (target: 80%+ of paid users connected; drives auto-categorization usage)
5. **Late payment reminders sent** (measures engagement with automation features)
6. **Monthly churn rate** (target: <4%; landlords should be very sticky)
7. **Receipt scans per user** (target: 5+/month; measures ongoing engagement outside tax season)

## Top 3 Risks
1. **Stessa adds better Schedule E reporting and remains free** — Stessa (now owned by Roofstock) could add auto-generated Schedule E reports to their free tier. Mitigation: Go deeper on the tax side — auto-categorize by Schedule E line items (not just categories), flag audit risks, and provide deduction recommendations. Stessa is pivoting toward investor analytics, not tax prep.
2. **Seasonality — engagement drops after tax season** — Landlords may only use the app intensely from January to April. Mitigation: Late rent reminders, maintenance tracking, and expense logging are year-round features. Send monthly "property P&L" summaries to keep users engaged. Gate Schedule E behind paid tier to drive annual subscriptions (not monthly).
3. **Plaid bank connection issues with small/regional banks** — Many landlords use local credit unions and community banks that Plaid supports poorly. Mitigation: Offer manual CSV import as a fallback; build direct integrations with the top 5 banks landlords use; support receipt-only expense tracking without bank connection.
