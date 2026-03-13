# Business Model: Utility Bill Auditor

## Value Proposition
Households save $200-$600/year by catching billing errors, switching to optimal rate plans, and detecting usage anomalies across electricity, gas, water, and internet — with one bill upload, the app finds money you're currently wasting.

## Customer Segments
- **Primary**: Homeowners and renters ages 28-55, household income $40K-$100K, who auto-pay their utility bills and never look at them. They're vaguely aware they're overpaying but don't know where to start. They've seen their electric bill creep up $20/month over 2 years and assumed it was rate increases.
- **Secondary**: Landlords managing 2-10 rental units who pay utilities and want to minimize costs across properties.
- **Psychographics**: Passive about bills but reactive to "found money." They won't proactively research rate plans, but they'll upload a bill if an app promises to find savings. They love the dopamine of "this app saved me $47" stories. They share financial wins on social media.

## Revenue Model
- **Free tier**: Upload 1 utility bill; get a basic error scan and savings estimate; see if you're on the optimal rate plan (yes/no, without details)
- **Paid tier**: $3.99/month — unlocks unlimited bill uploads across all utilities, detailed error reports, rate plan comparison with savings projections, usage anomaly detection ("possible water leak"), internet bill price-creep alerts, and negotiation scripts for calling providers
- **Premium/Enterprise**: $7.99/month — adds auto-switching to better rate plans (where deregulated markets allow), multi-property support, seasonal usage optimization tips, and historical bill archive with trend analysis
- **Projected conversion rate**: 9% free-to-paid (benchmarked against Rocket Money's 8-10% conversion for bill-related features; the free tier delivers a clear savings number that motivates upgrade)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $60 |
| APIs/Services (OCR for bill scanning, utility rate databases, OpenAI for analysis) | $400 |
| Marketing (SEO, social media, partnerships) | $450 |
| Total Monthly Burn | $910 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $11 |
| LTV | $86 (avg 21.5-month retention at $4/mo; utility bills are monthly and ongoing) |
| LTV:CAC | 7.8:1 |
| Payback Period | 2.8 months |
| Gross Margin | 85% |

## Go-to-Market: First 100 Users
1. **Reddit (weeks 1-6)**: Post "I audited my utility bills and found $340/year in savings" breakdowns in r/Frugal (2.3M), r/personalfinance (18M), r/povertyfinance (1.4M), and r/homeowners (310K). Show the specific errors and rate plan switches with redacted bill screenshots. These posts consistently go viral in money-saving communities.
2. **SEO (weeks 1-12)**: Target "how to lower electric bill," "utility billing errors," "best electricity rate plan," and "internet bill keeps going up." Publish 10 guides with embedded free bill audit tool as lead magnet.
3. **TikTok/Reels (weeks 2-8)**: Create 4 short-form videos per week in the "money-saving hack" format: "I uploaded my electric bill to this app and found out I've been overpaying $37/month for 2 years." Target #moneytok and #savingmoney hashtags.
4. **Energy efficiency program partnerships (weeks 6-10)**: Contact 10 state energy efficiency programs and utility cooperatives that already promote conservation — offer the app as a free tool for their members (drives user acquisition while aligning with their mission).

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 5,500 | $90K | 1,875 paid at $4/mo; SEO + Reddit + social media growth |
| 2 | 20,000 | $360K | 7,500 paid; TikTok content compounds; deregulated market auto-switching launches |
| 3 | 50,000 | $900K | 18,750 paid; utility company partnerships for rate comparison (affiliate model) |
| 4 | 90,000 | $1.7M | 33,000 paid; multi-property tier drives higher ARPU; expand to small businesses |
| 5 | 150,000 | $2.8M | 55,000 paid + $200K in affiliate revenue from provider switching; expand to UK/Canada deregulated energy markets |

## Key Weekly Metrics
1. Bills uploaded per week (target: 300/week by month 6)
2. Free-to-paid conversion rate (target: 9%)
3. Monthly churn rate (target: <4.5%)
4. Average savings identified per user (target: $25/month across all utilities)
5. Billing errors detected per 100 bills analyzed (target: 18-22 — consistent with industry 1-in-5 rate)
6. Rate plan switch recommendations acted on (target: 20% of recommendations lead to a switch)
7. Social shares of savings results (viral loop indicator — target: 5% of users share)

## Top 3 Risks
1. **OCR accuracy across diverse bill formats** — Utility bills vary enormously by provider, state, and format (paper vs. PDF vs. screenshot); inaccurate parsing leads to false savings claims or missed errors. → Mitigation: Start with the top 30 utility providers (covering ~60% of US households) and hand-tune OCR templates for each; allow manual correction of parsed values; display confidence scores on parsed data; use GPT-4 vision as a fallback parser for unrecognized formats; expand provider coverage based on user upload frequency.
2. **Utility rate data freshness** — Rate plans change quarterly; stale rate data could recommend a plan that no longer exists or has different pricing. → Mitigation: Scrape or partner with utility rate aggregators (like OpenEI or EnergySage) for real-time rate data; display "rate data last updated" timestamps; focus initial launch on the 10 largest deregulated energy markets where rate comparison has the most value; let users flag outdated rates.
3. **Regulatory complexity of auto-switching** — Switching utility providers on behalf of a user involves regulated processes that vary by state and provider; errors could leave users without service. → Mitigation: Launch auto-switching only in Texas, Pennsylvania, and Ohio (the 3 most mature deregulated residential electricity markets) where switching is standardized; partner with licensed retail energy brokers rather than switching directly; require explicit user confirmation before any switch; maintain the recommendation-only model as the default in all other markets.
