# Business Model: DunningGuard (Failed Payment Recovery)

## Value Proposition
Recover 40-70% of failed subscription payments automatically — turning involuntary churn into retained revenue without your team lifting a finger.

## Customer Segments
- **Primary**: SaaS founders and heads of growth at companies with $50K-$500K MRR, 2-20 employees, using Stripe as their payment processor. They know failed payments are a problem but don't have engineering bandwidth to build smart retry logic or dunning flows.
- **Secondary**: Subscription box companies, membership sites (gyms, communities), and online course platforms with recurring billing and high card-failure rates.
- **Psychographics**: Data-driven, ROI-obsessed, willing to pay for tools that directly impact revenue. They read Lenny's Newsletter, hang out in SaaS Twitter, and track MRR religiously.

## Revenue Model
- **Free tier**: Dashboard showing failed payment analytics and recovery rate for up to $10K MRR (product-led growth hook — show them how much they're losing)
- **Paid tier**: $49/month + 5% of recovered revenue — smart retry, pre-dunning emails, SMS campaigns, payment method updater for up to $200K MRR
- **Premium/Enterprise**: $199/month + 3% of recovered revenue — multi-processor support, custom branding, dedicated Slack channel, priority retry queue, for $200K+ MRR
- **Projected conversion rate**: 15% (benchmarked against Baremetrics' historical 12% trial-to-paid conversion; improved by showing exact dollar recovery in free tier dashboard)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $300 |
| Stripe/Paddle API infrastructure | $200 |
| Twilio (SMS recovery campaigns) | $250 |
| SendGrid (dunning emails) | $100 |
| Marketing | $800 |
| Total Monthly Burn | $1,650 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $180 (blended: $50 organic from SaaS communities + $350 via targeted LinkedIn/Twitter ads) |
| LTV | $4,200 (average customer stays 24 months; avg monthly spend = $175 platform fee + performance fee) |
| LTV:CAC | 23:1 |
| Payback Period | 1.0 months (performance fee means revenue starts immediately on recovery) |
| Gross Margin | 88% (low marginal cost per customer; primary costs are infrastructure) |

## Go-to-Market: First 100 Users
1. **Stripe app marketplace listing**: List DunningGuard on the Stripe App Marketplace. SaaS founders actively browse this for revenue tools. Aim for top listing in "Revenue Recovery" category.
2. **SaaS Twitter/X threads**: Write weekly threads with anonymized data ("We analyzed 50K failed payments — here's when retries work best"). Tag founders with 10K+ followers like @paborenstein, @aaborenstein for engagement.
3. **Indie Hackers and r/SaaS**: Post detailed case studies showing recovery rate improvements. Target r/SaaS (45K members), r/startups (1.1M members), and the Indie Hackers forum.
4. **Free "Failed Payment Audit"**: Offer a free 14-day audit where you connect to their Stripe, analyze failed payment patterns, and present a recovery opportunity report. This becomes the sales conversation.
5. **MicroConf and SaaS meetup sponsorships**: Sponsor the virtual MicroConf community ($500/month) to reach bootstrapped SaaS founders directly.
6. **Cold outreach to SaaS companies with visible churn**: Use BuiltWith/Wappalyzer to find Stripe-powered SaaS companies, then send personalized Loom videos showing their estimated failed payment losses.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 80 customers | $240K | Avg $250/mo (platform + performance fees); organic + Stripe marketplace |
| 2 | 200 customers | $720K | Avg $300/mo as customers grow MRR; add Paddle integration |
| 3 | 400 customers | $2.4M | Avg $500/mo; enterprise tier gains traction; word-of-mouth referrals |
| 4 | 700 customers | $5.0M | Avg $600/mo; add Braintree/Recurly; hire first sales rep |
| 5 | 1,100 customers | $9.2M | Avg $700/mo; international expansion; multi-currency support |

## Key Weekly Metrics
1. **Total dollars recovered** (north star — directly tied to revenue and customer satisfaction)
2. **Recovery rate** (% of failed payments successfully recovered; target: 55%+)
3. **New trial activations** (leading indicator; target: 5+/week in Year 1)
4. **Trial-to-paid conversion rate** (target: 15%+)
5. **Net revenue retention** (target: 120%+ as customers' MRR grows, so does our performance fee)
6. **Median time to first recovery** (target: <48 hours — proves value fast)
7. **Customer churn rate** (target: <3% monthly; low churn = high LTV)

## Top 3 Risks
1. **Stripe builds better native retry logic** — Stripe could improve their built-in Smart Retries, reducing the need for third-party tools. Mitigation: Differentiate on pre-dunning, SMS campaigns, and multi-processor support. Stripe's incentive is to remain a platform, not build every vertical tool.
2. **Performance fee model creates misaligned incentives at scale** — Large customers may resist paying 3-5% of recovered revenue as their MRR grows. Mitigation: Offer flat-fee enterprise plans for customers recovering >$10K/month; lock in annual contracts with volume discounts.
3. **Payment processor API changes break integrations** — Stripe, Paddle, or Braintree could change webhook structures or rate limits. Mitigation: Build an abstraction layer across processors; maintain close relationships with Stripe's partner engineering team; invest in automated integration testing.
