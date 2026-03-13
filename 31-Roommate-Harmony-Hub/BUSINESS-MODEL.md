# Business Model: Roommate Harmony Hub

## Value Proposition
Eliminate roommate conflict — the #1 cause of early lease breaks — with a single app that handles expense splitting, chore fairness, house rules, and structured conflict resolution, saving roommates the $2,500+ average cost of breaking a lease early.

## Customer Segments
- **Primary**: College students (ages 18-24) living with 1-3 roommates in dorms or off-campus housing. Psychographically: conflict-averse, digitally native, tight budgets, value fairness, socially active.
- **Secondary**: Young professionals (ages 24-35) sharing apartments in high-cost cities (NYC, SF, LA, Chicago, Seattle). Psychographically: income-earning but cost-conscious, expect polished UX, less tolerant of household friction, want adult solutions to adult problems.
- **Tertiary**: Non-traditional roommate situations — divorced parents sharing custody homes, older adults sharing housing for affordability.

## Revenue Model
- **Free tier**: Basic expense splitting (up to 4 roommates), simple chore checklist, shared shopping list
- **Paid tier**: $2.99/month — automated chore rotation with fairness scoring, conflict resolution templates, shared calendar, house rules builder, supply tracker, payment reminders via Venmo/Zelle integration
- **Premium/Enterprise**: $4.99/month per household — move-out calculator, security deposit documentation, noise/guest scheduling, priority support
- **Projected conversion rate**: 7% (benchmarked against Splitwise's 5-8% freemium conversion; broader feature set increases perceived value)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $120 |
| Push notification service (Firebase) | $50 |
| Payment integration APIs | $80 |
| Marketing (campus + social) | $1,000 |
| App store fees (15-30%) | $150 |
| Total Monthly Burn | $1,400 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $6 |
| LTV | $43 (avg 14-month retention at $3/mo; roommate situations are semi-permanent) |
| LTV:CAC | 7.2:1 |
| Payback Period | 2 months |
| Gross Margin | 85% |

## Go-to-Market: First 100 Users
- **Reddit**: r/roommates (35K), r/badroommates (130K), r/college (1.8M), r/AskNYC (380K), r/bayarea (390K) — post about chore fairness and expense splitting horror stories with app as solution
- **College campus ambassadors**: Recruit 10 ambassadors at large universities (ASU, Ohio State, UCLA, NYU, UT Austin); free premium + $5 per referral
- **TikTok**: "Roommate horror story" content is massively viral — create skits showing passive-aggressive sticky notes vs. the app
- **Move-in season targeting (Aug-Sep)**: Paid Instagram/TikTok ads targeting "new roommate" searches during August move-in season
- **Apartment listing partnerships**: Partner with Zillow/Apartments.com to include in "moving checklist" resources

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 22,000 free / 1,500 paid | $54K | Campus ambassador program + viral social; 7% conversion |
| 2 | 80,000 free / 7,000 paid | $252K | 20 campuses; word-of-mouth viral coefficient of 2.5x (each user invites roommates) |
| 3 | 250,000 free / 18,000 paid | $648K | Young professional segment grows; premium tier launched; move-in season campaigns |
| 4 | 500,000 free / 35,000 paid | $1.3M | Apartment complex partnerships (bulk licenses); all major metros covered |
| 5 | 1,000,000 free / 65,000 paid | $2.5M | International expansion (UK, Australia, Canada); property management integrations |

## Key Weekly Metrics
1. **Household activation rate** — % of new users who invite at least 1 roommate within 7 days; target 50%+
2. **Chore completion rate** — measures real engagement with core feature; target 60%+
3. **Expense settlements per household per week** — indicates financial feature usage
4. **Conflict resolution template usage** — leading indicator of high-value engagement
5. **Viral coefficient** — invites sent per user; target 2.0+ (natural roommate network)
6. **Monthly churn rate** — target below 6% (lease cycles create natural churn)
7. **App store rating** — target 4.5+; critical for organic discovery

## Top 3 Risks
1. **Natural churn when roommates move out or move in together** → Target lease renewal periods with re-engagement; build "new roommate onboarding" flow; track household continuity even when members change; offer move-out calculator as retention tool
2. **Splitwise already dominates expense splitting and could add chore features** → Differentiate on the holistic roommate experience (chores + conflict + rules); Splitwise's brand is "expense splitting" and pivoting dilutes it; focus on the 70% of roommate pain that isn't about money
3. **Low willingness to pay among college students** → Keep free tier genuinely useful to drive adoption; monetize the premium features that older/professional roommates value; explore ad-supported model for college segment as alternative
