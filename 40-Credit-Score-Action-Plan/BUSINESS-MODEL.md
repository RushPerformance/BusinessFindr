# Business Model: Credit Score Action Plan

## Value Proposition
Stop wondering why your credit score is stuck — get a ranked, personalized action plan that tells you exactly which account to pay down, which error to dispute, and which strategy to use next, with projected point impacts for each action, so you can reach your target score and save $50,000+ in lifetime interest costs.

## Customer Segments
- **Primary**: Adults ages 25-45 with credit scores between 580-720, actively trying to qualify for a mortgage, auto loan, or premium credit card. Household income $40K-$100K. Psychographically: goal-driven (specific financial milestone), frustrated by generic advice, willing to pay for a clear roadmap, anxious about being judged by a number.
- **Secondary**: Young adults (ages 18-28) building credit from scratch with limited credit history. Psychographically: financially aspirational, learning-oriented, responsive to gamification and progress tracking.
- **Tertiary**: Adults recovering from financial setbacks (bankruptcy, collections, divorce) ages 30-55 who need a structured rebuilding plan.

## Revenue Model
- **Free tier**: Credit score overview (via Credit Karma API or similar), top 3 general improvement tips, score simulator (2 scenarios)
- **Paid tier**: $6.99/month — full personalized action plan ranked by impact, utilization optimizer with specific dollar amounts, dispute assistant with letter generation, score simulator (unlimited scenarios), payment impact tracker, goal-based planning (mortgage readiness, etc.)
- **Premium/Enterprise**: $12.99/month — authorized user strategy, credit monitoring with alerts, bi-weekly score updates, 1-on-1 AI credit coach, debt payoff optimizer, credit-building product recommendations (non-affiliate, unbiased)
- **Projected conversion rate**: 9% (benchmarked against Credit Karma's 5-7% product conversion; action-oriented approach and goal urgency drive higher conversion)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $180 |
| Credit data API (Equifax/TransUnion) | $800 |
| AI action plan engine (OpenAI API) | $350 |
| Marketing (SEO + content) | $1,500 |
| App store fees (15-30%) | $250 |
| Total Monthly Burn | $3,080 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $22 |
| LTV | $126 (avg 18-month retention at $7/mo; users stay until they reach their goal score) |
| LTV:CAC | 5.7:1 |
| Payback Period | 3.1 months |
| Gross Margin | 76% |

## Go-to-Market: First 100 Users
- **Reddit**: r/personalfinance (17M), r/CRedit (140K), r/FirstTimeHomeBuyer (200K), r/povertyfinance (1.7M), r/FinancialPlanning (400K) — answer credit score questions with specific, actionable advice and link to the tool
- **Content SEO**: Target "how to improve credit score," "credit score action plan," "raise credit score 100 points," "credit utilization calculator," "dispute credit report errors" — high-volume, high-intent queries
- **YouTube**: "How I raised my credit score from 620 to 780" video series with screen recordings of the app; credit improvement content gets millions of views
- **Financial literacy communities**: Partner with non-profits like Operation HOPE, NFCC (National Foundation for Credit Counseling), and local financial literacy programs
- **First-time homebuyer workshops**: Partner with 10 real estate agents and mortgage brokers who run homebuyer seminars; offer 30-day free premium to attendees

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 11,000 free / 1,000 paid | $84K | SEO + Reddit; 9% conversion; high-intent users |
| 2 | 45,000 free / 5,000 paid | $420K | Content marketing compounds; YouTube channel grows; premium tier |
| 3 | 120,000 free / 7,000 paid | $588K | Mortgage broker referral channel; credit union partnerships |
| 4 | 250,000 free / 14,000 paid | $1.2M | Employer financial wellness programs; insurance company partnerships |
| 5 | 500,000 free / 25,000 paid | $2.1M | + $300K B2B financial institution licensing; international expansion |

## Key Weekly Metrics
1. **Action plan items completed** — core value delivery; target 2+ actions completed per user per month
2. **Score change tracking** — are users' scores actually improving? Measures real-world impact
3. **Dispute letters generated** — high-value feature usage; track success rate over time
4. **Utilization optimizer interactions** — unique feature engagement; measures actionable value
5. **Free-to-paid conversion rate** — target 9%+
6. **Goal achievement rate** — % of users who reach their target score; ultimate success metric
7. **Monthly churn rate** — target below 5%; users who see progress stay; users who don't leave

## Top 3 Risks
1. **Credit Karma adds action-plan-style features** → Credit Karma's revenue comes from financial product recommendations (credit cards, loans), creating a structural conflict — they benefit when users open new accounts, which can actually hurt scores; our subscription model aligns incentives with actual score improvement; publicize this difference
2. **Credit data API costs are high and access is gatekept by bureaus** → Start with free credit report data (AnnualCreditReport.com) and user-entered data; negotiate bureau partnerships as user base grows; explore partnerships with fintech credit data providers (Plaid, Nova Credit) for better rates
3. **Users blame the app if their score doesn't improve** → Set realistic expectations during onboarding ("most users see 20-50 point improvement in 3-6 months"); track and celebrate incremental wins; transparent methodology showing which factors are in the user's control; satisfaction guarantee (refund if no improvement in 90 days)
