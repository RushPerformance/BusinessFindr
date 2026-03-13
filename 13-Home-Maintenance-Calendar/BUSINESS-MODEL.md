# Business Model: Home Maintenance Calendar

## Value Proposition
Homeowners avoid $3,000-$10,000/year in preventable repair costs by following a personalized maintenance schedule tailored to their specific home — the app tells you exactly what to do, when, and why, before the $30 problem becomes a $5,000 emergency.

## Customer Segments
- **Primary**: First-time homeowners ages 28-40 who just bought a home in the last 0-3 years. They're overwhelmed, don't know what maintenance a house requires, and are actively searching r/homeowners and r/firsttimehomebuyer for guidance. Household income $60K-$120K.
- **Secondary**: Existing homeowners ages 35-55 who've been neglecting maintenance and recently had an expensive surprise repair (HVAC failure, water damage) that motivated them to get proactive.
- **Psychographics**: Responsible but inexperienced. They want to "do things right" but don't know where to start. They're willing to pay a small monthly fee to avoid the cognitive load of researching maintenance schedules themselves.

## Revenue Model
- **Free tier**: Basic annual maintenance checklist (generic, not personalized); 3 seasonal reminders per year
- **Paid tier**: $4.99/month — unlocks personalized calendar based on home age/location/systems, monthly push notifications, DIY video links, cost estimates for hiring pros, expense tracking, and home value protection score
- **Premium/Enterprise**: $9.99/month — adds vendor booking with vetted local contractors, priority scheduling, and detailed home inventory for insurance
- **Projected conversion rate**: 7% free-to-paid (benchmarked against HomeZada's estimated 5-8% conversion; personalization drives higher perceived value)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS/Vercel) | $60 |
| APIs/Services (weather API for climate-based reminders, push notifications) | $150 |
| Marketing (content, SEO, Reddit) | $500 |
| Total Monthly Burn | $710 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $10 |
| LTV | $156 (avg 26-month retention at $5/mo; home maintenance is ongoing — high natural retention) |
| LTV:CAC | 15.6:1 |
| Payback Period | 2 months |
| Gross Margin | 89% |

## Go-to-Market: First 100 Users
1. **Reddit (weeks 1-6)**: Share seasonal maintenance checklists (free PDF) in r/homeowners (310K), r/firsttimehomebuyer (260K), r/HomeImprovement (5.5M), and r/RealEstate (1M). Title: "I made a free first-year homeowner maintenance checklist — here's what your inspector didn't tell you." Link to the app for the automated, personalized version.
2. **Real estate agent partnerships (weeks 4-8)**: Email 50 local real estate agents offering a free co-branded "New Homeowner Care Package" they can give to closing clients. Agents love closing gifts that make them look thoughtful. Include 3-month free premium trial for the buyer.
3. **SEO (weeks 1-12)**: Target "home maintenance checklist by month," "when to change HVAC filter," "first-time homeowner maintenance guide" — these are high-volume, low-competition queries. Publish 12 monthly maintenance guides.
4. **Home inspector referrals (weeks 6-10)**: Partner with 20 home inspectors who can recommend the app at closing — they interact with every homebuyer and the app reinforces their inspection findings.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 6,000 | $120K | 2,000 paid at $5/mo; organic growth via SEO and Reddit |
| 2 | 22,000 | $480K | 8,000 paid; real estate agent partnerships scaling across 10 metros |
| 3 | 55,000 | $1.2M | 20,000 paid; vendor marketplace launches adding $2 per booked job |
| 4 | 100,000 | $2.3M | 35,000 paid + premium tier adoption at 15%; contractor marketplace revenue grows |
| 5 | 170,000 | $3.8M | 55,000 paid; expand to rental property owners managing maintenance across units |

## Key Weekly Metrics
1. Weekly task completion rate (what % of reminders are marked done — target: 45%)
2. Monthly active users (target: 70% MAU of total registered)
3. Free-to-paid conversion rate (target: 7%)
4. Monthly churn rate (target: <3.5% — low churn expected due to ongoing home needs)
5. Vendor bookings per week (once marketplace launches)
6. New user sign-up source breakdown (SEO vs. referral vs. agent partnership)
7. Net Promoter Score from in-app survey (target: 55+)

## Top 3 Risks
1. **User engagement decay** — Homeowners may set up the app enthusiastically then ignore push notifications after 2-3 months, leading to churn. → Mitigation: Tie reminders to "cost of neglect" framing ("Skip this $30 filter change and risk a $5,000 compressor failure"); add a cumulative "money saved" counter; send quarterly "home health reports" via email to re-engage.
2. **Personalization complexity** — Different home ages, climates, HVAC types, roof materials, and foundation types create thousands of permutations that are hard to get right for every home. → Mitigation: Start with the 20 most common home archetypes (e.g., "1990s ranch with gas furnace in humid climate"); let users override/customize; expand templates based on user feedback.
3. **Contractor marketplace quality control** — Bad contractor referrals could damage trust immediately. → Mitigation: Launch marketplace only in 5 metros initially; require contractors to be licensed and insured; collect user reviews after every job; remove contractors below 4.0 stars; charge contractors a lead fee (not a listing fee) to ensure only serious providers join.
