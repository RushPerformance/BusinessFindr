# Business Model: Divorce Finance Splitter

## Value Proposition
Divorcing individuals save $3,000-$8,000 in financial advisor fees by modeling equitable asset splits themselves — with tax-adjusted valuations that reveal the true after-tax value of a "50/50" division, so they walk away with a fair deal, not just an equal one.

## Customer Segments
- **Primary**: Adults ages 30-55 going through divorce, household income $50K-$150K, with moderate asset complexity (house, retirement accounts, some investments, car loans). They can't afford a Certified Divorce Financial Analyst ($200-$500/hour) but know their split has tax implications they don't understand. 60% female (women initiate 70% of divorces and are more likely to seek financial planning tools).
- **Secondary**: Divorce mediators and collaborative divorce attorneys who want a self-service tool to give clients as a lower-cost alternative to hiring a CDFA.
- **Psychographics**: Emotionally overwhelmed but trying to be rational about finances. They Google "is a 50/50 divorce split fair" and "divorce asset calculator" at 11 PM. They want clarity and control in a situation that feels chaotic. Price-sensitive because they're already hemorrhaging money on legal fees.

## Revenue Model
- **Free tier**: Basic asset inventory list; simple 50/50 split calculator (no tax adjustments); checklist of accounts to address during divorce
- **Paid tier**: $49.99 one-time purchase — unlocks tax-adjusted asset valuation, equitable split modeler (drag-and-drop), post-divorce budget projector, alimony/child support estimator by state, debt allocation worksheet, and document organizer
- **Premium/Enterprise**: $14.99/month for 6 months ($89.94 total) — adds ongoing budget tracking post-divorce, financial recovery planning, credit rebuilding checklist, and 2 updated split models as negotiations evolve
- **Projected conversion rate**: 12% free-to-paid (benchmarked against legal self-service tools like LegalZoom's 10-15% conversion; high urgency and clear monetary value drive higher conversion)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $50 |
| APIs/Services (tax calculation engine, state-specific alimony formulas) | $200 |
| Marketing (SEO, attorney partnerships, Google Ads) | $600 |
| Total Monthly Burn | $850 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $22 |
| LTV | $58 (weighted avg: 70% buy $49.99 one-time, 30% choose $89.94 subscription package) |
| LTV:CAC | 2.6:1 |
| Payback Period | 0 months (one-time purchase — immediate) |
| Gross Margin | 91% |

## Go-to-Market: First 100 Users
1. **SEO (weeks 1-12)**: Publish 15 high-intent articles targeting "divorce asset calculator," "how to split 401K in divorce," "tax implications of divorce settlement," "is 50/50 split fair in divorce." These are evergreen, high-intent queries with commercial value. Aim for featured snippets.
2. **Reddit (weeks 1-6)**: Provide thoughtful, helpful answers in r/Divorce (145K), r/DivorcedDads (18K), r/SingleMoms (25K), and r/personalfinance. Share specific examples: "Here's why a 50/50 split of a $500K 401K vs. $500K home equity isn't actually equal" with the math shown.
3. **Divorce attorney partnerships (weeks 4-10)**: Email 50 divorce mediators and collaborative divorce attorneys offering a 20% affiliate commission for every client they refer. Frame it as: "Give your clients financial clarity without hiring a CDFA — they'll come to mediation better prepared."
4. **Divorce support Facebook Groups (weeks 2-8)**: Contribute genuinely in "Divorce Support for Women" (60K+), "Divorce Recovery" (40K+), and state-specific divorce groups. Share the free asset checklist as a lead magnet.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 4,500 | $190K | 3,800 one-time purchases; SEO + attorney referrals ramp up |
| 2 | 12,000 | $520K | SEO compounds; attorney partnerships in 20 states; subscription option grows to 35% of purchases |
| 3 | 25,000 | $950K | 19,000 purchases; mediator platform integrations; add business asset valuation module |
| 4 | 40,000 | $1.6M | Expand to military divorce (unique rules) and high-asset divorce tiers; B2B licensing to law firms |
| 5 | 60,000 | $2.5M | International expansion (UK, Canada, Australia); B2B platform for mediators ($99/mo); referral network with 500+ attorneys |

## Key Weekly Metrics
1. New free accounts created (target: 100/week by month 6)
2. Free-to-paid conversion rate (target: 12%)
3. Split models completed (indicates engagement — target: 85% of paid users complete at least 1 model)
4. Attorney referral sign-ups and conversion rate
5. Organic search traffic to divorce calculator pages
6. Average session duration (target: 15+ minutes — indicates deep engagement with asset modeling)
7. Customer satisfaction score from post-purchase survey (target: 4.2/5)

## Top 3 Risks
1. **Tax calculation errors leading to financial harm** — Incorrect tax-adjusted valuations could cause a user to accept a bad settlement worth thousands less than they think. → Mitigation: Partner with a CPA specializing in divorce taxation to validate all formulas; include clear disclaimers that the tool is for estimation, not tax advice; compare outputs against 50 real CDFA case studies for accuracy; recommend professional review for assets over $500K.
2. **Emotional user state causing support burden** — Divorcing users are under extreme stress; they may contact support frequently, leave emotional negative reviews over minor issues, or misunderstand outputs due to cognitive overload. → Mitigation: Design the UX with empathy (calm colors, encouraging copy, progress indicators); build comprehensive in-app guidance for every input field; create a FAQ addressing the top 20 emotional questions ("Is this really fair?"); route support to trained responders with empathetic scripts.
3. **Low repeat usage (one-time life event)** — Unlike subscription products, divorce happens once; there's no natural retention mechanism. → Mitigation: The subscription option ($14.99/mo for 6 months) captures users who need ongoing modeling as negotiations evolve; post-divorce budget tracking extends the relationship; build a referral program (divorced users know other divorcing people); expand to related life events (estate planning, remarriage prenups) to extend LTV.
