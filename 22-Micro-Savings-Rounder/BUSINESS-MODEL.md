# Business Model: Micro-Savings Rounder

## Value Proposition
People who "can't save" build a $1,000 emergency fund within 8-12 months by rounding up every purchase — automatically, painlessly, and with goal-based gamification that makes saving feel like progress instead of deprivation.

## Customer Segments
- **Primary**: Young adults ages 18-30, income $25K-$50K, living paycheck to paycheck. They've tried to save manually and failed. They may have a savings account with less than $500 in it. They want an emergency fund but can't carve out $200/month — yet they can round up $0.37 on a coffee purchase without noticing.
- **Secondary**: Parents of teens/young adults who want to teach saving habits; adults ages 30-45 rebuilding savings after a financial setback (job loss, medical bills, divorce).
- **Psychographics**: Financially anxious but aspirational. They follow financial literacy content on TikTok and Instagram. They respond to gamification (streaks, badges, progress bars) and are motivated by visual progress. They distrust complex financial products and prefer simplicity.

## Revenue Model
- **Free tier**: N/A — the app requires bank connection to function, so it's a subscription-only model with a 30-day free trial
- **Paid tier**: $2.99/month — full round-up functionality, savings goals with visual progress bars, streak tracking, boost feature (extra savings on payday), financial education nudges, and withdrawal friction ("Are you sure?")
- **Premium/Enterprise**: N/A (single-tier consumer product to maintain simplicity)
- **Projected conversion rate**: 35% trial-to-paid (benchmarked against Acorns' ~30% trial-to-paid; lower price point and simpler value proposition should outperform; savings-first framing eliminates investing anxiety)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $80 |
| APIs/Services (Plaid for bank connection, banking partner for FDIC savings, push notifications) | $600 |
| Marketing (social media, influencer partnerships) | $500 |
| Compliance/Legal (banking partner regulatory costs) | $300 |
| Total Monthly Burn | $1,480 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $14 |
| LTV | $54 (avg 18-month retention at $3/mo; churn higher than other categories due to young, price-sensitive demographic) |
| LTV:CAC | 3.9:1 |
| Payback Period | 4.7 months |
| Gross Margin | 72% (lower due to Plaid + banking partner costs) |

## Go-to-Market: First 100 Users
1. **TikTok/Instagram Reels (weeks 1-8)**: Create 5 short-form videos per week: "I saved $847 without noticing — here's how round-ups work," "Day 30 of rounding up every purchase — I have $127 I didn't know I had." Target #moneytok (50B views), #savingmoney, #financialliteracy, #emergencyfund hashtags. This demographic lives on TikTok.
2. **Reddit (weeks 1-6)**: Share savings milestones in r/povertyfinance (1.4M), r/FinancialPlanning (340K), r/personalfinance (18M), and r/Frugal (2.3M). Post: "I couldn't save for years. Then I started rounding up every purchase. 6 months later, I have $1,012."
3. **Financial literacy influencer partnerships (weeks 3-8)**: Partner with 5 personal finance TikTok/Instagram creators (20K-200K followers) targeting the "broke but trying" demographic. Creators like @herfirst100k, @personalfinanceclub, and smaller micro-influencers. Budget: $200-$500 per creator.
4. **College campus ambassador program (weeks 6-12)**: Recruit 10 college students as brand ambassadors at large universities. Provide them with referral codes and $5 per sign-up incentive. Students are the perfect demo and campuses are concentrated markets.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 8,000 | $90K | 2,500 paid at $3/mo; TikTok + Reddit organic growth |
| 2 | 30,000 | $360K | 10,000 paid; TikTok content compounds; college ambassador program in 25 schools |
| 3 | 80,000 | $1.1M | 30,000 paid; referral program drives viral growth; partnership with 2 neobanks for co-marketing |
| 4 | 150,000 | $2.0M | 55,000 paid; add interest on savings balances (revenue share with banking partner); expand to high-yield savings |
| 5 | 250,000 | $3.4M | 90,000 paid; launch investing round-ups as an add-on for users who've built emergency funds; B2B employee benefit partnerships |

## Key Weekly Metrics
1. Weekly active round-up users (target: 70% WAU of paid subscribers)
2. Trial-to-paid conversion rate (target: 35%)
3. Monthly churn rate (target: <5.5%)
4. Average weekly round-up amount per user (target: $8-$12)
5. Savings goal completion rate (% of users who reach their first goal — target: 40% within 12 months)
6. Streak length distribution (target: 50% of users maintain 30+ day streaks)
7. Withdrawal rate (target: <15% of users withdraw in any given month — lower is better)

## Top 3 Risks
1. **Banking partner and regulatory complexity** — Holding user savings requires a banking partner (or banking charter), FDIC insurance, state money transmitter licenses, and ongoing compliance costs that can be prohibitive for a startup. → Mitigation: Partner with an established BaaS (Banking as a Service) provider like Synapse (now Tabapay), Unit, or Treasury Prime that handles compliance; their per-account costs ($1-$3/mo) are factored into the cost structure; start in 5 states with simplest licensing requirements and expand gradually.
2. **Plaid costs eating margins** — At $0.30-$1.50 per bank connection and $3/mo subscription, Plaid fees can consume 10-50% of revenue per user. → Mitigation: Negotiate volume discounts aggressively (target $0.20/connection at 5K+ users); explore MX or Finicity as alternatives; batch round-up transfers weekly (not daily) to reduce API call frequency; the $3/mo price point is tight — consider raising to $3.99/mo after proving value.
3. **User trust with bank connection** — Linking a bank account is a high-trust action; young, low-income users are especially wary of financial apps accessing their accounts after Digit's controversial overdraft issues. → Mitigation: Use Plaid's trusted connection flow (users see their bank's login, not ours); prominently display FDIC insurance and read-only bank access; never withdraw more than the user sets as a daily max; add a "pause round-ups" button for tight weeks; publish a transparency report on how funds are held.
