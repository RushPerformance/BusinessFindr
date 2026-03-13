# Business Model: Rent Increase Negotiator

## Value Proposition
Tenants save $600-$2,400/year on rent by responding to increase notices with data-backed negotiation letters — turning a panic moment into a power move, in under 15 minutes.

## Customer Segments
- **Primary**: Urban renters ages 25-45, household income $35K-$75K, renting apartments in mid-to-high-cost markets (NYC, LA, Denver, Austin, Seattle). They've just received a rent increase notice and feel powerless. They're Reddit-savvy, financially stressed, and likely Googling "is my rent increase legal" within 24 hours of receiving a notice.
- **Secondary**: Tenant advocacy organizations and legal aid clinics looking for self-service tools to distribute to clients.
- **Psychographics**: Frustrated but not confrontational. They want to push back but need a professional script. They value fairness and data over emotional arguments.

## Revenue Model
- **Free tier**: Check if your rent increase is above or below local averages; view 3 comparable listings nearby
- **Paid tier**: $14.99 one-time per negotiation kit — unlocks customized negotiation letter, phone call scripts, rent control law lookup, and full comparable analysis
- **Premium/Enterprise**: $3.99/month monitoring — ongoing rent trend alerts, lease renewal prep 60 days before expiry, and unlimited negotiation kits
- **Projected conversion rate**: 8% free-to-paid (benchmarked against DoNotPay's estimated 5-10% conversion on utility tools, weighted toward higher end due to urgency of use case)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (Vercel/Railway) | $50 |
| APIs/Services (rental data via Rentometer API, OpenAI for letter generation) | $300 |
| Marketing (Reddit ads, content) | $400 |
| Total Monthly Burn | $750 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $8 |
| LTV | $26 (avg: 1 kit at $15 + 30% convert to $3.99/mo monitoring for 7 months) |
| LTV:CAC | 3.3:1 |
| Payback Period | 0 months (one-time purchase model — immediate payback) |
| Gross Margin | 88% |

## Go-to-Market: First 100 Users
1. **Reddit (weeks 1-4)**: Post weekly in r/AskNYC (430K), r/LosAngeles (880K), r/personalfinance (18M), r/povertyfinance (1.4M), and r/TenantHelp showing before/after screenshots of a negotiation letter alongside comparable data. Frame as "I built this after my landlord tried to raise my rent 18%."
2. **SEO content (weeks 1-8)**: Publish 10 long-tail blog posts targeting "is my rent increase legal in [state]", "how to negotiate rent increase letter", "average rent increase 2026" — these queries spike every spring/summer during lease renewals.
3. **Tenant advocacy partnerships (weeks 4-8)**: Email 20 local tenant unions and legal aid clinics (e.g., Met Council on Housing in NYC, Tenants Together in CA) offering free bulk access in exchange for distribution to their members.
4. **TikTok/Reels (weeks 2-6)**: Create 3 short-form videos per week: "My landlord wanted $200 more — here's the letter I sent" format. Target #renttok and #apartmentlife hashtags.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 12,000 | $135K | 9,000 kits sold + 500 monthly subscribers; organic + Reddit growth |
| 2 | 35,000 | $380K | SEO compounds; tenant org partnerships drive 3x user growth |
| 3 | 75,000 | $900K | City-specific landing pages for top 50 markets; monitoring subscriptions grow |
| 4 | 130,000 | $1.6M | B2B licensing to tenant advocacy orgs; API partnerships with apartment listing sites |
| 5 | 200,000 | $2.5M | National brand recognition; expanded to commercial lease negotiation; 20% monitoring conversion |

## Key Weekly Metrics
1. Negotiation kits purchased (target: 175/week by month 6)
2. Free-to-paid conversion rate (target: 8%)
3. Monitoring subscription MRR and churn rate (target: <6% monthly churn)
4. Average savings reported by users (track via optional follow-up survey)
5. Organic search traffic to state-specific landing pages
6. Reddit/social mention volume and sentiment
7. Comparable data API uptime and freshness (data must be <7 days old)

## Top 3 Risks
1. **Rental data accuracy and coverage** — Comparable listings may be sparse in smaller markets or rural areas, making the tool less useful outside top-30 metros. → Mitigation: Launch in top 10 rental markets first; supplement API data with manual Zillow/Craigslist scraping; display confidence scores so users know when data is thin.
2. **Legal liability from generated negotiation letters** — A poorly worded letter could expose a tenant to retaliation or violate local tenant-landlord communication laws. → Mitigation: Have a tenant rights attorney review letter templates for each state; include prominent disclaimers; frame output as "informational" not "legal advice."
3. **Seasonality and one-time use** — Rent negotiations happen once per year at lease renewal; most users buy one kit and leave. → Mitigation: Push monitoring subscriptions hard after purchase; build lease renewal reminder flow that re-engages users annually; expand to roommate cost-splitting and security deposit recovery tools to increase touchpoints.
