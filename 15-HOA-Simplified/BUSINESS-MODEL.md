# Business Model: HOA Simplified

## Value Proposition
Volunteer HOA board members replace their chaotic mix of Venmo, spreadsheets, and email chains with one $30/month tool that handles dues collection, violation tracking, document storage, and resident communication — saving 10+ hours/month of volunteer time and reducing late dues by 40%.

## Customer Segments
- **Primary**: Volunteer HOA and condo association board members managing communities of 20-200 units. Typically 45-65 years old, not tech-savvy, doing this unpaid work out of civic duty. They're frustrated by the chaos of managing finances and communications with consumer tools never designed for this purpose.
- **Secondary**: Self-managed small condo associations (10-50 units) that can't justify a professional management company ($200-500/mo) but need more than spreadsheets.
- **Psychographics**: Overwhelmed, time-starved, and often dealing with irate residents about late fees or violation notices. They want something "that just works" without a steep learning curve. Price-conscious because they're spending the HOA's money, not their own.

## Revenue Model
- **Free tier**: Community setup for up to 10 units; basic announcement board; document storage (up to 500MB)
- **Paid tier**: $29.99/month per community — unlocks unlimited units, online dues payment via Stripe (ACH + credit card), automated late payment reminders, violation tracking, maintenance request portal, and budget tools
- **Premium/Enterprise**: $59.99/month — adds board meeting agenda builder, automated financial reporting, reserve fund projections, and bulk community onboarding for management companies overseeing 5+ communities
- **Projected conversion rate**: 15% free-to-paid (benchmarked against B2B SaaS tools like Slack's 30% and adjusted down for smaller, less tech-forward customer base; the free tier is intentionally limited to 10 units to force upgrade)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $120 |
| APIs/Services (Stripe payment processing, email/SMS notifications via Twilio) | $350 |
| Marketing (SEO, HOA conference attendance, direct outreach) | $600 |
| Total Monthly Burn | $1,070 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $45 |
| LTV | $900 (avg 30-month retention at $30/mo; HOAs switch tools very rarely due to high switching cost) |
| LTV:CAC | 20:1 |
| Payback Period | 1.5 months |
| Gross Margin | 82% (after Stripe processing fees on dues collected) |

## Go-to-Market: First 100 Users
1. **Reddit and online HOA communities (weeks 1-6)**: Post helpful content in r/HOA (150K), r/HOAHell (15K), r/CondoAssociation, and r/PropertyManagement. Share templates: "Free HOA meeting minutes template" and "How to send a violation notice that doesn't start a war." Link to app as the tool behind the templates.
2. **HOA board Facebook Groups (weeks 2-8)**: Join "HOA Board Members Support Group" (12K), "Condo Association Board Members" (8K), and state-specific HOA groups. Offer free walkthroughs for struggling boards.
3. **Direct outreach to small HOAs (weeks 4-10)**: Search county records for HOAs with 20-100 units in 5 target metros. Mail 200 postcards to HOA registered agents: "Still collecting dues on Venmo? There's a better way — $30/mo, all-in."
4. **Community Associations Institute (CAI) events (month 2-3)**: Attend 2 regional CAI chapter meetings ($50-100 per event); set up a demo station and collect leads from volunteer board members.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 500 communities | $180K | Organic growth + direct outreach; avg $30/mo per community |
| 2 | 1,800 communities | $648K | Word-of-mouth (board members talk to other boards); SEO for "HOA management software" |
| 3 | 5,000 communities | $1.8M | Premium tier adoption at 20%; management company partnerships begin |
| 4 | 10,000 communities | $3.6M | Expand to Canadian and UK markets; management company bulk tier drives 2,000 communities |
| 5 | 18,000 communities | $6.5M | Marketplace for HOA vendors (landscaping, painting, etc.) adds affiliate revenue |

## Key Weekly Metrics
1. New community sign-ups (target: 10/week by month 6)
2. Dues collection rate per community (target: 90%+ on-time payments)
3. Free-to-paid conversion rate (target: 15%)
4. Monthly churn rate (target: <2.5% — high switching costs make this realistic)
5. Active communities (defined as at least 1 admin action per week — target: 80%)
6. Stripe payment volume processed (leading indicator of community engagement)
7. Support ticket volume per community (target: <0.5/month — simplicity reduces support needs)

## Top 3 Risks
1. **Slow adoption by non-technical board members** — Volunteer board members skew older and less tech-savvy; if onboarding is confusing, they'll revert to spreadsheets. → Mitigation: Offer white-glove onboarding calls (30 minutes) for every new community; build a setup wizard that imports existing unit lists from CSV; create video walkthroughs for every feature; design the UI for "someone who still uses Internet Explorer."
2. **Payment processing liability and trust** — Collecting HOA dues means handling significant funds ($10K-$50K/month per community); any payment errors or delays destroy trust immediately. → Mitigation: Use Stripe Connect so funds go directly to the HOA's bank account (never touch our account); implement real-time payment confirmation emails; maintain a 99.9% uptime SLA for payment processing; add reconciliation reports that match Stripe payouts to expected dues.
3. **Enterprise competitors moving downmarket** — AppFolio or Buildium could launch a "lite" tier targeting small HOAs, leveraging their existing brand and features. → Mitigation: Move fast to own the "simple and affordable" positioning before they react; build deep community loyalty through responsive support and feature requests; focus on volunteer-specific UX (not just a stripped-down enterprise tool); the enterprise players' cost structures make sub-$50/mo pricing unattractive for them.
