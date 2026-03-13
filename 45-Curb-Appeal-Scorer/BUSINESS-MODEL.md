# Business Model: Curb Appeal Scorer

## Value Proposition
Home sellers get an objective, data-backed exterior improvement plan that maximizes resale value -- ensuring every dollar spent on curb appeal delivers the highest possible return, typically 2-5x ROI on recommended improvements.

## Customer Segments
- **Primary**: Homeowners aged 35-60 preparing to sell within 6-12 months, household income $80K-$200K. Psychographically motivated by maximizing sale price, anxious about buyer first impressions, and willing to invest in improvements but unsure where to start.
- **Secondary**: Real estate agents working with sellers who need data-driven staging recommendations to justify improvement requests and win listings.
- **Tertiary**: Homeowners not selling but wanting to improve their home's appearance for personal pride, HOA compliance, or neighborhood standing. Lower urgency, more price-sensitive.

## Revenue Model
- **Free tier**: One free curb appeal score (1-100) with top-level breakdown, watermarked report
- **Paid tier**: $4.99 per report -- Full factor breakdown (landscaping, paint, door, driveway, lighting, symmetry), ROI-ranked improvement suggestions, cost estimates, before/after AI visualization
- **Premium/Enterprise**: $14.99/month (agents) -- Unlimited reports, co-branded reports for client presentations, neighborhood comparison data, contractor referral integration
- **Projected conversion rate**: 10% (benchmarked against Photoroom and similar single-use AI photo analysis tools where the output has clear monetary value)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $80 |
| AI/ML inference (vision model API) | $250 |
| Home value and cost data APIs | $120 |
| Image storage | $40 |
| Marketing | $400 |
| Total Monthly Burn | $890 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $6 |
| LTV | $8.50 (blended: 80% one-time $4.99, 10% buy 2+ reports, 10% agent subscriptions) |
| LTV:CAC | 1.4:1 |
| Payback Period | 0 months (per-report purchase) |
| Gross Margin | 68% |

## Go-to-Market: First 100 Users
- **Reddit**: Share before/after improvement examples in r/RealEstate (1.1M), r/HomeImprovement (4.5M), r/FirstTimeHomeBuyer (120K), r/Flipping (30K). Post "AI scored my home's curb appeal and the #1 fix cost $50" content.
- **Real estate agent outreach**: Cold email top-producing agents in 10 major metros with free trial codes; agents become distribution channel to sellers.
- **Zillow/Redfin forum engagement**: Participate in seller Q&A threads where curb appeal questions arise regularly.
- **Instagram/Pinterest**: Post striking before/after visualizations -- this content is inherently shareable and performs well on visual platforms.
- **Home staging blogs and podcasts**: Guest appearances and partnerships with home staging educators who reach pre-sale homeowners.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 7,200 reports sold | $36K | Organic growth; proving AI scoring accuracy against appraiser feedback |
| 2 | 25,000 reports + 200 agent subs | $125K + $36K = $161K | Agent referral channel active; SEO for "curb appeal tips" keywords |
| 3 | 54,000 reports + 600 agent subs | $270K + $108K = $378K | Partnership with real estate brokerages for agent tier |
| 4 | 80,000 reports + 1,200 agent subs | $400K + $216K = $616K | Contractor referral marketplace adds revenue; national brand awareness |
| 5 | 120,000 reports + 2,000 agent subs | $600K + $360K = $960K | Integration with MLS platforms; expansion to commercial properties |

## Key Weekly Metrics
1. Photos uploaded / scores generated (top of funnel)
2. Free-to-paid report conversion rate
3. Agent subscription sign-ups and retention
4. AI score accuracy (user feedback vs. eventual sale price delta)
5. Before/after visualizations generated (premium feature engagement)
6. Contractor referral clicks (monetization signal)
7. Social shares of score results (viral coefficient)

## Top 3 Risks
1. **AI scoring accuracy is subjective and contested** -- "Curb appeal" is partly aesthetic judgment, and users may disagree with scores. Mitigation: Train model on actual sale price data correlated with exterior features; show confidence intervals; allow users to rate score accuracy to improve model.
2. **Low LTV:CAC limits scalability** -- At $4.99 per report, paid acquisition is barely viable. Mitigation: Agent subscription tier is the real business (higher LTV); individual reports serve as lead gen for agent channel; contractor referral fees add $2-5 per report in affiliate revenue.
3. **Zillow or Redfin builds this feature** -- Real estate platforms have the data, traffic, and AI talent to replicate this. Mitigation: Focus on actionable improvement plans (not just scores); build contractor marketplace that platforms won't prioritize; serve the agent workflow specifically.
