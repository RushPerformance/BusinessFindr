# Business Model: Pothole Reporter Plus

## Value Proposition
Turn road frustration into fixed roads — report potholes in one tap, automatically file complaints with the right municipal department, track repairs, and avoid hazards on your commute, while potentially recovering the $300/year the average driver loses to pothole damage.

## Customer Segments
- **Primary**: Daily commuters (ages 25-55) driving 20+ minutes to work in cities with poor road infrastructure (Midwest, Northeast, cities with harsh winters). Psychographically: frustrated by government inaction, civic-minded, willing to take 10 seconds to report a problem if they believe it will actually lead to a fix.
- **Secondary**: Cyclists and motorcycle riders (ages 20-45) for whom potholes are a serious safety hazard, not just a vehicle damage issue. Psychographically: safety-conscious, community-oriented, active on cycling forums.
- **Tertiary**: Municipal governments and road departments seeking crowdsourced data to prioritize repair budgets.

## Revenue Model
- **Free tier**: Hazard reporting with GPS tagging, crowdsourced hazard map, community upvotes
- **Paid tier**: $2.99/month — auto-file municipal complaints, repair status tracking, route hazard alerts for daily commute, damage claim letter generator, analytics dashboard
- **Premium/Enterprise**: $500-2,000/month (B2B/municipal) — aggregated hazard data dashboard, priority heat maps, citizen engagement analytics, API access
- **Projected conversion rate**: 5% (benchmarked against Waze's premium conversion concepts and SeeClickFix's engagement; civic apps have lower conversion but high engagement)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $150 |
| Maps API (Google Maps/Mapbox) | $300 |
| Municipal complaint filing integration | $200 |
| Marketing (local + social) | $800 |
| App store fees (15-30%) | $100 |
| Total Monthly Burn | $1,550 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $8 |
| LTV | $43 (avg 14-month retention at $3/mo; seasonal — more active in pothole season) |
| LTV:CAC | 5.4:1 |
| Payback Period | 2.7 months |
| Gross Margin | 78% |

## Go-to-Market: First 100 Users
- **Reddit**: r/cycling (540K), r/bikecommuting (130K), city-specific subreddits (r/chicago 450K, r/detroit 80K, r/pittsburgh 100K, r/boston 320K — all pothole-heavy cities)
- **Local news pitches**: "New app lets residents file pothole complaints in one tap" — local TV and newspapers love civic tech stories; pitch to 10 worst-road cities
- **Cycling advocacy groups**: Partner with local cycling coalitions in 5 target cities; bike shops as distribution partners (QR code flyers)
- **Nextdoor**: Post in neighborhood forums about specific pothole clusters with before/after repair stories
- **City council meetings**: Attend public meetings in 3 pilot cities and demonstrate the tool; city officials are often looking for citizen engagement solutions

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 18,000 free / 900 paid | $32K | Launch in 5 pothole-heavy cities; local media coverage; 5% conversion |
| 2 | 60,000 free / 3,500 paid | $126K | 15 cities; first municipal contracts ($24K); viral local news coverage |
| 3 | 180,000 free / 9,000 paid | $324K | + $100K municipal contracts; 30 cities; damage claim feature drives paid upgrades |
| 4 | 400,000 free / 18,000 paid | $648K | + $250K municipal contracts; state DOT partnerships; national brand |
| 5 | 800,000 free / 30,000 paid | $1.1M | + $500K municipal/B2B; national coverage; insurance company partnership for claims data |

## Key Weekly Metrics
1. **Hazard reports submitted** — core content generation; target 500+/week by month 6
2. **Municipal complaints auto-filed** — differentiator feature usage; target 60% of reports auto-filed
3. **Repairs confirmed (community-verified)** — measures real-world impact; use in marketing
4. **Route hazard alert engagement** — % of commuters who check alerts before driving
5. **Free-to-paid conversion rate** — target 5%+
6. **Geographic density** — reports per square mile in active cities; critical mass needed for map value
7. **Municipal response rate** — % of auto-filed complaints that get a response; validates government integration

## Top 3 Risks
1. **Municipalities don't respond to auto-filed complaints, eroding user trust** → Track and publish municipal response rates by city; partner with responsive cities first; use non-responsive cities' data in advocacy and media coverage to pressure change; offer direct escalation to city council members
2. **Seasonal usage — potholes worsen in spring but interest fades in summer** → Expand to year-round road hazards (construction zones, flooding, debris, broken signals); build data retention features that show year-over-year trends; winter road condition reporting
3. **Waze adds pothole-specific reporting and municipal filing** → Waze is focused on real-time navigation, not civic engagement or repair tracking; our moat is the municipal complaint integration, repair tracking, and damage claim features that Waze has no incentive to build
