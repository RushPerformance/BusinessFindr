# Business Model: Neighborhood Safety Pulse

## Value Proposition
Renters, homebuyers, and parents make confident neighborhood decisions with objective, contextualized safety scores — knowing not just how safe an area is today, but whether it's getting safer or more dangerous, without the fear-mongering of Citizen or Nextdoor.

## Customer Segments
- **Primary**: Renters and homebuyers ages 25-45 actively searching for a new neighborhood. They're evaluating 2-5 areas and safety is a top-3 decision factor. Household income $45K-$100K. They've used Zillow and Redfin for listings but can't find trustworthy, contextualized safety data.
- **Secondary**: Parents (especially mothers) ages 30-50 with young children, already living in a neighborhood and wanting ongoing monitoring. Also women living alone in urban areas who want data-driven awareness without fear-based apps like Citizen.
- **Psychographics**: Safety-conscious but rational — they don't want to be scared, they want to be informed. They're frustrated by Nextdoor's hysterical "suspicious person" posts and Citizen's anxiety-inducing real-time alerts. They want data, trends, and context. They search "is [neighborhood] safe" before signing a lease.

## Revenue Model
- **Free tier**: Safety score (1-100) for any US address; basic trend direction (improving/declining); city average comparison
- **Paid tier**: $3.99/month — unlocks detailed category breakdown (property vs. violent vs. traffic), 5-year trend analysis, side-by-side neighborhood comparison, time-of-day heat maps, customizable alerts for incidents near home/work, school safety data, and community reports
- **Premium/Enterprise**: $199/month — B2B API for real estate platforms, property management companies, and relocation services to embed safety scores in their listings (Year 2+)
- **Projected conversion rate**: 6% free-to-paid (benchmarked against AreaVibes' estimated 3-5% conversion and Citizen's premium uptake of ~8%; the free tier is useful enough to drive traffic but limited enough to motivate upgrade for active movers)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $80 |
| APIs/Services (crime data APIs, geocoding, mapping tiles, push notifications) | $450 |
| Marketing (SEO, social media, real estate partnerships) | $500 |
| Total Monthly Burn | $1,030 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $12 |
| LTV | $67 (avg 16.8-month retention at $4/mo; higher churn than utility apps because need decreases after moving) |
| LTV:CAC | 5.6:1 |
| Payback Period | 3 months |
| Gross Margin | 83% |

## Go-to-Market: First 100 Users
1. **SEO (weeks 1-12)**: Publish 50 city/neighborhood-specific pages: "Is [Neighborhood], [City] safe in 2026?" targeting queries like "is Bushwick safe," "East Nashville crime rate," "Capitol Hill Seattle safety." These are extremely high-intent, pre-lease/pre-purchase queries. Each page includes the free safety score as a hook.
2. **Reddit (weeks 1-8)**: Monitor and respond to "is [neighborhood] safe?" posts in city-specific subreddits: r/AskNYC (430K), r/LosAngeles (880K), r/Chicago (370K), r/Austin (420K), r/Denver (230K), r/Seattle (380K). Provide data-driven answers with citations, then link to the app for full analysis. These posts appear daily in every city subreddit.
3. **Real estate agent partnerships (weeks 4-10)**: Offer 30 real estate agents a free co-branded safety report they can share with clients evaluating neighborhoods. Agents love providing data that builds trust. Each report drives the buyer to the app for ongoing monitoring.
4. **Apartment listing site partnerships (weeks 8-12)**: Approach Apartments.com, Zumper, and Rent.com with a proposal to embed safety scores on listings. Start with a free widget that includes the app branding. This drives massive awareness among active renters at the decision point.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 7,000 | $70K | 1,450 paid at $4/mo; SEO-driven growth in 20 cities |
| 2 | 25,000 | $290K | 6,000 paid; city-specific pages rank in 50 metros; real estate agent referrals grow |
| 3 | 60,000 | $700K | 14,500 paid; B2B API launches with 3 real estate platforms adding $50K |
| 4 | 110,000 | $1.4M | 25,000 paid; B2B API grows to $300K with 10 platform clients; expand to Canadian cities |
| 5 | 180,000 | $2.5M | 40,000 paid; B2B API at $600K; relocation company partnerships; insurance company data licensing |

## Key Weekly Metrics
1. Safety score lookups per week (target: 5,000/week by month 6)
2. Free-to-paid conversion rate (target: 6%)
3. Monthly churn rate (target: <6% — higher than other tools due to post-move drop-off)
4. Neighborhood comparison tool usage (target: 40% of paid users use weekly)
5. Organic search traffic to city/neighborhood pages (target: 10,000 sessions/week by month 8)
6. Community report submissions per week (target: 50/week by month 6 — user-generated content flywheel)
7. B2B API query volume (once launched — target: 10,000 queries/month per client)

## Top 3 Risks
1. **Crime data availability, freshness, and inconsistency** — Public crime data varies enormously by jurisdiction; some cities publish daily, others quarterly; some don't publish at all. Data formats are non-standardized. → Mitigation: Start with the 30 cities that have the best open data portals (NYC, Chicago, LA, Seattle, Austin, Denver, etc.); supplement with FBI UCR data for cities without open portals; display "data freshness" indicators so users know when data was last updated; aggregate multiple sources (police reports, 911 call logs, court records) for the most complete picture.
2. **Algorithmic bias and discrimination concerns** — Safety scores could reinforce racial or socioeconomic biases if the underlying crime data reflects biased policing patterns (e.g., over-policing in minority neighborhoods inflating crime stats). → Mitigation: Normalize crime data against policing intensity (calls per officer, arrest rates) when possible; include socioeconomic context in reports; consult with criminal justice researchers on methodology; publish the scoring methodology transparently; avoid language that could be used for redlining; never associate safety scores with demographic data.
3. **User trust erosion from inaccurate or outdated scores** — A neighborhood scored as "safe" where a user experiences crime, or a "dangerous" score for a neighborhood that's clearly gentrified, destroys credibility immediately. → Mitigation: Always show confidence intervals and data recency ("score based on 847 incidents reported in last 12 months, updated 3 days ago"); allow user feedback on scores ("Does this match your experience?"); show trend direction prominently so users understand the score is a snapshot, not a guarantee; update scores at least monthly for all covered cities.
