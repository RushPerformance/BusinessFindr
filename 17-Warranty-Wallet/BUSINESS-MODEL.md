# Business Model: Warranty Wallet

## Value Proposition
Households recover $200-$500/year in warranty claims they would have otherwise missed — the app stores every receipt and warranty, alerts you before coverage expires, and walks you through filing a claim in minutes instead of hours.

## Customer Segments
- **Primary**: Homeowners ages 30-55 with $15K-$30K in warrantied appliances and electronics. Household income $60K-$120K. They buy quality products but lose track of receipts and warranty periods. They've had at least one experience of a product breaking just after (or unknowingly during) the warranty period.
- **Secondary**: Small landlords managing 2-10 rental units who need to track appliance warranties across multiple properties.
- **Psychographics**: Organized-aspirational — they want to be the person who files warranty claims on time but aren't currently. They feel a pang of frustration every time they throw away a broken product they "probably could have gotten fixed for free." Slightly frugal, value getting what they paid for.

## Revenue Model
- **Free tier**: Store up to 10 warranties manually; view expiration dates; basic product catalog
- **Paid tier**: $3.99/month — unlocks unlimited warranties, email receipt auto-import (Gmail/Outlook), expiration countdown alerts (30/60/90 days), guided claim filing with pre-written letters, manufacturer contact lookup, and home inventory export for insurance
- **Premium/Enterprise**: $7.99/month — adds extended warranty price comparison marketplace (affiliate), automatic warranty detection from email scans, and multi-property support for landlords
- **Projected conversion rate**: 8% free-to-paid (benchmarked against receipt/document management apps like Evernote's historical 5-6%, adjusted up because the 10-warranty free cap creates a natural paywall for most households)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $70 |
| APIs/Services (Gmail API, OCR for receipt scanning, push notifications) | $350 |
| Marketing (SEO, social, partnerships) | $400 |
| Total Monthly Burn | $820 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $8 |
| LTV | $110 (avg 27.5-month retention at $4/mo; warranties are ongoing as people keep buying products) |
| LTV:CAC | 13.8:1 |
| Payback Period | 2 months |
| Gross Margin | 87% |

## Go-to-Market: First 100 Users
1. **Reddit (weeks 1-6)**: Share "warranty claim success stories" in r/Frugal (2.3M), r/BuyItForLife (1.8M), r/homeowners (310K), and r/personalfinance (18M). Post: "My dishwasher broke at month 11 of a 12-month warranty. Here's how I got a free replacement." Mention the app as what reminded you to check.
2. **SEO content (weeks 1-10)**: Publish guides for "how to file a warranty claim with [Samsung/LG/Whirlpool/Apple]" — these are high-intent, low-competition search queries. Each guide links to the app's guided claim feature.
3. **New homeowner partnerships (weeks 4-8)**: Partner with real estate agents and home warranty companies to include Warranty Wallet in closing packets. New homeowners have a house full of warrantied appliances and are highly receptive.
4. **Appliance retailer partnerships (weeks 8-12)**: Approach Home Depot and Best Buy affiliate programs — the app encourages users to track warranties on products they already bought, which is brand-positive for retailers.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 7,000 | $100K | 2,100 paid at $4/mo; SEO and Reddit-driven organic growth |
| 2 | 22,000 | $340K | 7,000 paid; email receipt import feature drives viral "I found warranties I forgot about" moments |
| 3 | 50,000 | $1.0M | 21,000 paid; extended warranty marketplace adds $100K in affiliate commissions |
| 4 | 90,000 | $1.9M | 38,000 paid; landlord/property manager tier adds $150K; affiliate revenue grows to $250K |
| 5 | 150,000 | $3.2M | 60,000 paid + $500K affiliate revenue; B2B API for retailers to auto-register warranties at point of sale |

## Key Weekly Metrics
1. Warranties added per week (target: 500/week by month 6)
2. Free-to-paid conversion rate (target: 8%)
3. Monthly churn rate (target: <3.5%)
4. Warranty claims initiated through the app (target: 20/week by month 6)
5. Email receipt import success rate (% of emails correctly parsed — target: 85%)
6. Expiration alerts sent vs. claims filed (conversion funnel — target: 15% of alerts lead to a claim)
7. Extended warranty marketplace click-through rate (for affiliate revenue tracking)

## Top 3 Risks
1. **Email integration complexity and privacy concerns** — Gmail/Outlook integration requires OAuth permissions that many users are uncomfortable granting; email parsing accuracy varies widely across retailer receipt formats. → Mitigation: Make email import optional (not required for core value); clearly explain what data is accessed and stored; use read-only scopes; build a receipt-specific email parser that only reads purchase-related emails; allow manual forwarding as an alternative to full inbox access.
2. **Low claim frequency reduces perceived value** — Most warranties last 1-3 years, meaning a user might not need to file a claim for months, making the $4/mo subscription feel wasteful. → Mitigation: Emphasize the insurance framing ("$4/mo protects $15K in products"); add home inventory value tracking ("your home contains $22,000 in tracked products"); send monthly "warranty health" reports; add product recall alerts as a bonus feature.
3. **Manufacturer resistance to streamlined claims** — Some manufacturers intentionally make claims difficult to reduce payouts; a tool that simplifies claims could face pushback or blocked access. → Mitigation: Position the app as consumer empowerment (manufacturers can't block a customer from using their own receipt and warranty terms); focus on claim preparation (letters, documentation gathering) rather than direct API integration with manufacturers; if specific manufacturers create friction, publish "claim difficulty ratings" that create PR pressure.
