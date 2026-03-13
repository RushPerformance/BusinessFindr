# Business Model: Restaurant Waste Tracker

## Value Proposition
Independent restaurants cut food costs by 2-8% ($5,000-$30,000/year) by tracking waste at the prep level and getting AI-powered ordering recommendations — paying for the tool 5-10x over every month.

## Customer Segments
- **Primary**: Independent restaurant owners and kitchen managers running single-location restaurants with annual food costs of $100K-$500K. They know waste is a problem but have no systematic way to measure or reduce it. Typically 35-55 years old, tech-pragmatic (use Toast or Square POS already), and margin-obsessed.
- **Secondary**: Small restaurant chains (2-10 locations) that can't justify enterprise waste systems like LeanPath ($500+/mo) but want visibility across locations.
- **Psychographics**: Hands-on operators who work 60+ hour weeks. They'll adopt a new tool only if it saves money fast and doesn't add more than 5 minutes/day of work. They trust ROI numbers over marketing claims. They talk to other restaurant owners at industry meetups and supplier events.

## Revenue Model
- **Free tier**: 14-day free trial with full features; after trial, basic waste logging for 1 category (spoilage only) with weekly summary email
- **Paid tier**: $49/month per location — unlocks all waste categories (overproduction, spoilage, prep trim, plate waste), cost analytics dashboard, AI ordering recommendations, par level optimizer, shift/station breakdown, and weekly emailed reports
- **Premium/Enterprise**: $99/month per location (3+ locations) — adds cross-location benchmarking, inventory integration, manager accountability scoring, and waste reduction goal tracking with team leaderboards
- **Projected conversion rate**: 25% trial-to-paid (benchmarked against Toast's ~20% and MarketMan's ~25% trial conversion; restaurant owners convert when ROI is proven during the trial)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $100 |
| APIs/Services (OpenAI for ordering recommendations, email delivery) | $300 |
| Marketing (industry outreach, restaurant supplier partnerships) | $700 |
| Total Monthly Burn | $1,100 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $65 |
| LTV | $882 (avg 18-month retention at $49/mo; restaurant tools churn when restaurants close, not when they switch) |
| LTV:CAC | 13.6:1 |
| Payback Period | 1.3 months |
| Gross Margin | 84% |

## Go-to-Market: First 100 Users
1. **Restaurant industry Reddit and forums (weeks 1-6)**: Post actionable waste reduction tips in r/restaurateur (45K), r/KitchenConfidential (2.8M), r/smallbusiness (1.4M), and Chef's Forum. Share data: "We tracked waste for 30 days and found we were over-ordering romaine by 22% every Monday — here's how we fixed it." Link to tool as what enabled the tracking.
2. **Food supplier partnerships (weeks 4-10)**: Approach 10 local food distributors (Sysco reps, US Foods reps, local produce distributors) and offer co-marketing: "Help your restaurant clients reduce waste and order smarter." Suppliers benefit because smarter ordering = more consistent customers.
3. **Restaurant association events (weeks 6-12)**: Attend 3 local restaurant association meetups or National Restaurant Association regional events. Demo the tablet interface to owner-operators. Collect 30 trial sign-ups per event.
4. **Direct outreach to Toast/Square POS users (weeks 2-8)**: Run targeted ads on Facebook/Instagram to restaurant owners (targetable via business page category). Ad copy: "Your POS tracks sales. Nothing tracks waste. That's where your profit goes." Budget: $500/month.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 300 restaurants | $176K | Direct sales + trial conversions; avg $49/mo |
| 2 | 1,200 restaurants | $706K | Supplier partnerships drive referrals; expand to 15 metros |
| 3 | 3,000 restaurants | $1.8M | Premium multi-location tier drives ARPU up; enterprise tier adds $200K |
| 4 | 6,000 restaurants | $3.5M | POS integrations (Toast, Square) drive discovery; national supplier partnerships |
| 5 | 10,000 restaurants | $5.9M | Add food cost forecasting and menu engineering tools; expand to UK/Canada |

## Key Weekly Metrics
1. Daily waste logs submitted (target: 85% of active restaurants log at least 5 days/week)
2. Trial-to-paid conversion rate (target: 25%)
3. Monthly churn rate (target: <5% — restaurant closures are the main churn driver)
4. Average waste cost reduction per restaurant (target: $1,500/month by month 3 of usage)
5. AI ordering recommendation adoption rate (% of recommendations accepted — target: 40%)
6. New trial sign-ups per week (target: 15/week by month 6)
7. NPS from quarterly restaurant owner survey (target: 50+)

## Top 3 Risks
1. **Staff compliance with daily logging** — Kitchen staff are busy and may skip waste logging, especially during rush periods, making data incomplete and analytics unreliable. → Mitigation: Design a 30-second logging interface optimized for a greasy kitchen tablet; allow batch logging at end-of-shift rather than real-time only; gamify compliance with shift scores; let managers see which stations/shifts are logging and which aren't; make the first week's data entry a guided process with the owner present.
2. **ROI proof takes time** — Restaurants expect immediate results, but meaningful waste pattern detection requires 30-60 days of data. If owners don't see value in the trial period, they churn. → Mitigation: Show quick wins in week 1 (e.g., "You logged $847 in waste this week — that's 6.2% of food cost"), even before AI recommendations kick in; extend trial to 30 days (not 14) to ensure enough data for first recommendations; provide industry benchmarks to contextualize waste levels immediately.
3. **Restaurant industry downturn** — Restaurants have a 60% failure rate in the first 5 years; economic downturns accelerate closures, shrinking the customer base. → Mitigation: Position the tool as recession-essential ("Cut waste to survive margin compression"); target established restaurants (3+ years old) with stable operations; diversify into adjacent verticals (catering companies, hotel kitchens, university dining) that are more recession-resistant.
