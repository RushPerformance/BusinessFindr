# Business Model: Babysitter Rate Calculator

## Value Proposition
Parents and sitters agree on a fair rate in under 60 seconds -- eliminating the awkward negotiation and ensuring both sides feel confident they're getting a market-appropriate deal for their exact situation.

## Customer Segments
- **Primary**: Parents aged 28-42 with children under 12, household income $60K-$150K, suburban/urban areas. Psychographically want to be fair employers but have no reference point, feel guilty about underpaying or anxious about overpaying.
- **Secondary**: Teenage and college-age babysitters (ages 15-24) setting rates for the first time. Uncomfortable with money conversations, want to appear professional, often undercharge because they lack market data.
- **Tertiary**: Professional nannies and au pairs negotiating full-time or part-time contracts. Higher stakes, more complex rate structures (benefits, overtime, holidays).

## Revenue Model
- **Free tier**: Basic rate lookup (zip code + number of kids), ad-supported, 3 lookups per month
- **Paid tier**: $1.99 one-time purchase -- Unlimited lookups, duty-based pricing, holiday/late-night premiums, rate card builder, tip guide, annual rate review
- **Premium/Enterprise**: $4.99 one-time -- Everything in paid, plus nanny contract templates, tax withholding calculator, rate comparison across 5 cities
- **Projected conversion rate**: 15% (benchmarked against simple utility apps like Tip Calculator Pro; low price point drives impulse purchases)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS/Vercel) | $30 |
| Rate data aggregation (BLS, Care.com scraping, surveys) | $100 |
| Ad network integration (AdMob) | $20 |
| App Store fees (15-30%) | $80 |
| Marketing | $200 |
| Total Monthly Burn | $430 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $1.50 |
| LTV | $2.40 (blended: 70% buy $1.99, 15% buy $4.99, 15% free with $0.60 ad LTV) |
| LTV:CAC | 1.6:1 |
| Payback Period | 0 months (one-time purchase) |
| Gross Margin | 78% |

## Go-to-Market: First 100 Users
- **Reddit**: Share rate data insights in r/Parenting (5.5M members), r/Nanny (90K), r/Babysitting (12K), r/Mommit (870K). Post "What babysitters actually charge in 2026 by city" content.
- **Facebook parent groups**: Target local mom groups (every city has dozens) with "Is $15/hour fair for 2 kids in [city]?" conversation starters that link to the app.
- **TikTok/Instagram**: Create "How much should you pay your babysitter?" content -- this format consistently performs well in parenting content niches.
- **Care.com forums and Sittercity blogs**: Comment and participate where parents and sitters already discuss rates.
- **Local parenting blogs and newsletters**: Pitch guest posts with embedded rate data for specific metro areas.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 12,000 purchases + 40K free | $24K + $8K ads = $32K | Organic growth via parenting communities; ad revenue from free tier |
| 2 | 40,000 purchases + 120K free | $80K + $24K ads = $104K | SEO rankings for "babysitter rates" keywords; app store visibility |
| 3 | 90,000 purchases + 250K free | $180K + $50K ads = $230K | Brand recognition as the go-to rate reference; nanny agency partnerships |
| 4 | 140,000 purchases + 400K free | $280K + $80K ads = $360K | Expansion to UK, Canada, Australia; employer childcare benefit partnerships |
| 5 | 200,000 purchases + 600K free | $400K + $120K ads = $520K | Category leader status; integration with booking platforms |

## Key Weekly Metrics
1. Rate lookups performed (core usage)
2. Rate cards created by sitters (two-sided adoption)
3. Free-to-paid conversion rate
4. Ad revenue per 1,000 free users (eCPM)
5. App Store keyword rankings for "babysitter rate" and "nanny pay"
6. Zip codes with active users (geographic coverage)
7. User reviews mentioning rate accuracy (data quality signal)

## Top 3 Risks
1. **Rate data accuracy and freshness** -- Stale or inaccurate data destroys trust instantly. Mitigation: Blend BLS childcare wage data with crowd-sourced rates from users; update quarterly; show data source and recency for transparency.
2. **Care.com or UrbanSitter adds this feature** -- Large platforms could bundle rate calculators into their existing products. Mitigation: Go deeper on rate nuance (duties, premiums, tips) than any platform would; maintain independence as a neutral tool trusted by both sides.
3. **Low LTV:CAC ratio limits paid growth** -- At $2 per purchase, paid acquisition channels are nearly impossible. Mitigation: Rely on organic/viral distribution; make the rate card shareable (sitters send to parents, creating natural viral loop); optimize for word-of-mouth.
