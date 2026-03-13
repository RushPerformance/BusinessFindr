# Business Model: Energy Usage Disaggregator

## Value Proposition
Homeowners and renters discover exactly which appliances are draining their wallet and get a prioritized upgrade plan that typically saves $200-$500/year on electricity -- all without buying any hardware.

## Customer Segments
- **Primary**: Homeowners aged 30-55, household income $50K-$120K, with smart meters (70%+ of US households by 2026). Psychographically cost-conscious, environmentally aware, frustrated by opaque utility bills, and willing to pay $5/month if it saves them $20+/month.
- **Secondary**: Renters aged 25-40 who pay their own electricity, cannot install hardware monitors, and want to identify energy waste in their units.
- **Tertiary**: Sustainability-minded consumers who want to reduce carbon footprint with data-driven decisions, not guesswork. Over-index on EV owners and solar panel considerers.

## Revenue Model
- **Free tier**: Total usage tracking, monthly bill comparison, neighbor comparison, 3-month usage history
- **Paid tier**: $4.99/month -- AI appliance-level disaggregation, cost-per-appliance breakdown, savings recommendations with ROI calculations, anomaly alerts, seasonal analysis
- **Premium/Enterprise**: $9.99/month -- Everything in paid, plus real-time monitoring, appliance upgrade marketplace with affiliate deals, home energy audit report for insurance/resale, API access for smart home integration
- **Projected conversion rate**: 6% (benchmarked against Sense app's conversion rate; lower because no hardware lock-in, but offset by lower price point)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS with ML inference) | $300 |
| Utility API integrations (Green Button, Utility API) | $200 |
| ML model training and maintenance | $150 |
| Data storage (usage history) | $80 |
| Marketing | $400 |
| Total Monthly Burn | $1,130 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $12 |
| LTV | $72 (avg 12-month retention at $4.99/mo, 10% upgrade to $9.99) |
| LTV:CAC | 6:1 |
| Payback Period | 2.4 months |
| Gross Margin | 74% |

## Go-to-Market: First 100 Users
- **Reddit**: Share energy-saving discoveries in r/homeowners (310K), r/Frugal (2.3M), r/solar (180K), r/electricvehicles (420K), r/homeautomation (1.5M). Post "I found out my old fridge was costing me $35/month" style content.
- **Utility company partnerships**: Approach municipal utilities and co-ops that want to offer demand management tools to customers. Offer white-label or co-branded version.
- **Energy audit communities**: Engage with Home Energy Score assessors and HERS raters who could recommend the tool.
- **Smart home YouTube channels**: Sponsor or collaborate with channels like Technology Connections, This Old House, and home automation creators.
- **SEO**: Target "why is my electric bill so high," "which appliances use the most electricity," "home energy monitor without hardware" -- high-intent searches with strong commercial value.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 600 paid | $36K | Organic acquisition; proving ML model accuracy on real smart meter data |
| 2 | 3,000 paid | $180K | Utility API integrations with 10+ major providers; model accuracy improves with scale |
| 3 | 6,000 paid | $360K | First utility partnership deal for co-branded distribution |
| 4 | 15,000 paid | $900K | Multiple utility partnerships; premium tier adoption at 20%; appliance marketplace affiliate revenue |
| 5 | 30,000 paid | $1.8M | Utility partnerships as primary channel; expansion to natural gas disaggregation; B2B energy management tier |

## Key Weekly Metrics
1. Smart meter accounts connected (activation funnel)
2. Disaggregation accuracy score (model quality)
3. Savings recommendations acted upon (value delivery)
4. Free-to-paid conversion rate
5. Monthly churn rate
6. Utility API uptime and data freshness
7. Customer-reported energy savings (outcome metric)

## Top 3 Risks
1. **ML disaggregation accuracy is insufficient** -- Non-intrusive load monitoring (NILM) from smart meter data alone has known accuracy limitations (~70-80% for major appliances). Mitigation: Set clear expectations ("estimates, not exact readings"); focus on the top 5 energy hogs where accuracy is highest (HVAC, water heater, fridge, dryer, EV charger); improve models with user feedback loops.
2. **Utility API access is fragmented and unreliable** -- Green Button adoption varies by utility; many require manual CSV upload. Mitigation: Support manual upload as fallback; prioritize the 20 largest utilities covering 50%+ of US households; build scraping integrations where APIs don't exist.
3. **Sense or Emporia launches a software-only competitor** -- Hardware energy monitor companies have proprietary data and could pivot to software-only. Mitigation: Move fast on utility partnerships (distribution moat); their business model depends on hardware margins, creating organizational resistance to a software-only product.
