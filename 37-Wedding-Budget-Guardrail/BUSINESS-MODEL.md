# Business Model: Wedding Budget Guardrail

## Value Proposition
Keep your wedding beautiful without going broke — get real-time budget protection with vendor price benchmarks, "budget impact" alerts before every spending decision, and hidden fee detection that saves the average couple $3,000-5,000 compared to planning with tools that profit from your overspending.

## Customer Segments
- **Primary**: Newly engaged couples (ages 25-38), combined household income $80K-$180K, planning a wedding in the $15K-$50K range. Psychographically: excited but financially anxious, overwhelmed by vendor pricing opacity, socially pressured to overspend, first-time event planners making unfamiliar decisions under time pressure.
- **Secondary**: Parents contributing to wedding costs (ages 50-65) who want budget visibility and guardrails on their contribution. Psychographically: generous but practical, want to help without going into debt.
- **Tertiary**: Budget-conscious couples planning weddings under $15K who need to make every dollar count.

## Revenue Model
- **Free tier**: Basic budget tracker with category allocation, 3 vendor expense entries, general industry benchmarks
- **Paid tier**: $9.99/month (avg 10-month subscription = $100 total) — unlimited vendor tracking, zip-code-specific cost benchmarks, budget impact alerts, hidden fee detector, trade-off calculator, payment schedule tracker, post-wedding settlement
- **Premium/Enterprise**: $14.99/month — vendor negotiation scripts, shared access for parents/wedding planner, priority support, vendor comparison tools
- **Projected conversion rate**: 18% (benchmarked against wedding app conversion rates of 15-22%; high-stakes, time-limited event creates urgency)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $120 |
| Vendor pricing data aggregation | $400 |
| AI budget analysis (OpenAI API) | $200 |
| Marketing (social + wedding SEO) | $1,500 |
| App store fees (15-30%) | $250 |
| Total Monthly Burn | $2,470 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $25 |
| LTV | $100 (avg 10-month subscription at $10/mo; wedding planning is finite) |
| LTV:CAC | 4:1 |
| Payback Period | 2.5 months |
| Gross Margin | 80% |

## Go-to-Market: First 100 Users
- **Reddit**: r/weddingplanning (650K), r/Weddingsunder10k (270K), r/wedding (180K), r/budgetwedding (15K) — share specific budget-saving tips and hidden fee discoveries
- **Instagram/TikTok**: "Wedding industry secrets they don't want you to know" content — expose hidden fees, upsell tactics, and pricing opacity; budget comparison reels
- **Wedding blogger partnerships**: Partner with 10 budget wedding bloggers (A Practical Wedding, Offbeat Bride) for reviews and guest posts
- **The Knot/Zola forums**: Engage in community discussions about budget anxiety with helpful advice and soft app mentions
- **Engagement ring retailer partnerships**: QR code in ring box inserts or post-purchase emails ("Just got engaged? Protect your wedding budget")

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 2,800 free / 500 paid | $60K | Organic + wedding community marketing; 18% conversion; 10-month avg subscription |
| 2 | 10,000 free / 2,000 paid | $240K | SEO for "wedding budget" queries matures; word-of-mouth from satisfied couples |
| 3 | 25,000 free / 4,000 paid | $480K | Premium tier adds $80K; vendor cost database becomes comprehensive and trusted |
| 4 | 50,000 free / 8,000 paid | $960K | B2B partnerships with wedding venues offering the tool to couples; parent-sharing feature |
| 5 | 100,000 free / 15,000 paid | $1.8M | Expansion to other high-cost events (bar/bat mitzvahs, quinceañeras, corporate events) |

## Key Weekly Metrics
1. **Budget alerts triggered** — core feature usage; each alert is a moment of value delivery
2. **Vendor expenses logged per user** — measures depth of adoption; target 8+ vendors tracked
3. **Hidden fee detections per user** — unique differentiator; track and use in marketing
4. **Budget variance (planned vs. actual)** — are users staying closer to budget than industry average?
5. **Free-to-paid conversion rate** — target 18%+
6. **Subscription duration** — average months active; target 10+ (full planning cycle)
7. **Total savings attributed** — aggregate savings across all users; headline marketing number

## Top 3 Risks
1. **The Knot/Zola adds budget-protection features to neutralize the threat** → Their business model depends on vendor advertising revenue, creating a structural conflict of interest; as long as they profit from vendor spending, true budget protection undermines their core business; publicize this misalignment
2. **Vendor cost benchmarks are inaccurate, leading to user distrust** → Aggregate from multiple sources (WeddingWire, Thumbtack, real user submissions); start with top 20 metro areas; implement user-verified pricing with confidence scores; update quarterly
3. **Short customer lifecycle (10-month avg) makes growth dependent on constant acquisition** → Build referral program ("tell your newly engaged friends"); capture post-wedding users for anniversary/event planning; create evergreen content that attracts new cohorts each engagement season
