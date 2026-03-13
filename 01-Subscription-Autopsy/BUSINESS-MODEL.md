# Business Model: Subscription Autopsy

## Value Proposition
Save $1,600/year by automatically finding and killing hidden subscriptions you forgot about — and catch zombie charges that keep billing after you cancel.

## Customer Segments
- **Primary**: US adults aged 25-45 with 10+ active subscriptions, digitally active, earning $40K-$120K/year. They value convenience and hate feeling "scammed" by companies making cancellation difficult. Over-indexed on streaming, fitness apps, and SaaS trials.
- **Secondary**: Budget-conscious parents (35-55) managing household subscriptions across multiple family members, often discovering kids signed up for services without their knowledge.
- **Psychographics**: Mild financial anxiety, motivated by "quick wins" and instant savings. They love sharing savings on social media ("Look how much I was wasting!").

## Revenue Model
- **Free tier**: One-time bank/email scan, subscription list with total spend breakdown and waste score
- **Paid tier**: $4.99/month — auto-cancel via bots, zombie charge monitoring, weekly spend alerts, recurring scans
- **Premium/Enterprise**: $9.99/month — family plan (up to 4 connected accounts), priority cancellation queue, annual savings report
- **Projected conversion rate**: 8% (benchmarked against Rocket Money's ~6% free-to-paid conversion, improved by lower price point and flat-fee vs. percentage model)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS/Vercel) | $150 |
| Plaid API (bank connections) | $800 (at $0.30/connection for ~2,700 active users) |
| Email parsing API (Nylas) | $200 |
| OpenAI API (categorization) | $120 |
| Marketing | $500 |
| Total Monthly Burn | $1,770 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $12 (blended: $3 organic via viral sharing + $25 paid via Reddit/Instagram ads) |
| LTV | $48 (average retention 9.6 months at $4.99/mo, benchmarked against Truebill's ~10-month retention) |
| LTV:CAC | 4:1 |
| Payback Period | 2.4 months |
| Gross Margin | 82% (Plaid + API costs are ~18% of revenue per user) |

## Go-to-Market: First 100 Users
1. **Reddit organic**: Post weekly "subscription audit" breakdowns in r/personalfinance (18M members), r/Frugal (2.3M), and r/povertyfinance (1.8M) showing anonymized before/after savings screenshots. Participate in "what subscriptions should I cancel" threads with helpful advice and a soft mention.
2. **TikTok/Reels content**: Create 15-second "I just found $137/month in zombie subscriptions" reaction videos. The savings reveal format is proven viral (Rocket Money's TikTok ads use this exact hook).
3. **Product Hunt launch**: Target a Tuesday launch with an "audit your subscriptions free" angle. Aim for top 5 of the day.
4. **"Subscription Autopsy Report" sharing mechanic**: After scan, users get a shareable card showing total waste found — designed for Twitter/Instagram stories with a referral link.
5. **Hacker News "Show HN"**: Position as a privacy-first alternative to Rocket Money (no percentage-of-savings model, flat fee).

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 3,000 paid | $180K | Organic growth + Product Hunt launch; 8% conversion from 37,500 free users |
| 2 | 12,000 paid | $720K | Viral sharing mechanic drives 4x growth; introduce family plan upsell |
| 3 | 30,000 paid | $1.8M | Reddit/TikTok content flywheel; blended ARPU rises to $5.50 with premium tier |
| 4 | 55,000 paid | $3.6M | Paid acquisition at scale ($20 CAC); partnerships with financial literacy creators |
| 5 | 90,000 paid | $6.5M | Enterprise/family segment grows; annual plan discounts improve retention to 14 months |

## Key Weekly Metrics
1. **New free scans completed** (leading indicator of top-of-funnel growth)
2. **Free-to-paid conversion rate** (target: 8%+)
3. **Zombie charges detected** (validates unique value prop; target: 0.3 per user/month)
4. **30-day retention rate** (target: 70%+ for paid users)
5. **Viral coefficient** (shares per user; target: 0.3+ to sustain organic growth)
6. **Plaid connection success rate** (target: 95%+; failure here kills activation)
7. **Total dollar savings delivered** (the north star metric for marketing and PR)

## Top 3 Risks
1. **Plaid dependency and cost escalation** — Plaid could raise prices or restrict access for small developers. Mitigation: Build MX Financial and Finicity as backup providers; email-scanning path works without bank connection.
2. **Auto-cancel bots break when companies change flows** — Companies like Adobe and NYT frequently update cancellation flows, breaking automated bots. Mitigation: Build a community-reported "cancellation flow changed" alert system and maintain a manual cancellation guide fallback.
3. **Rocket Money dominates paid acquisition channels** — Rocket Money (backed by Rocket Companies) spends heavily on ads, making paid channels expensive. Mitigation: Double down on organic/viral channels (Reddit, TikTok) and differentiate on flat-fee pricing and zombie charge monitoring, which Rocket Money doesn't emphasize.
