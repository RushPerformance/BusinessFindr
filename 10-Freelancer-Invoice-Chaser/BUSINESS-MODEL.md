# Business Model: Freelancer Invoice Chaser

## Value Proposition
Get paid on time without the awkward emails — automated escalation sequences chase your overdue invoices professionally so you can focus on client work, not collections.

## Customer Segments
- **Primary**: Solo freelancers aged 25-45 (designers, developers, writers, photographers, consultants) earning $40K-$120K/year who invoice 3-15 clients per month. They hate chasing payments — it feels unprofessional, damages relationships, and eats 3-5 hours/month. Active on r/freelance (1.1M members), r/graphic_design (900K members), r/webdev (1M members), and freelancer Twitter/X.
- **Secondary**: Small creative agencies (2-5 people) and independent contractors in trades (electricians, plumbers, consultants) who deal with chronic late payments from larger clients. Also new freelancers who don't yet have processes for payment follow-up.
- **Psychographics**: Conflict-averse, creative-minded, and time-poor. They'd rather lose a payment than send an awkward follow-up. They want a system that feels professional and firm without being aggressive, because they depend on client relationships for repeat work.

## Revenue Model
- **Free tier**: 3 active clients, manual reminder sending (pre-written templates provided), basic invoice tracking, aging report
- **Paid tier**: $6.99/month — unlimited clients, automated escalation sequences (Day 1, 7, 14, 30), late fee calculator, client reliability scores, custom branding on reminder emails
- **Premium/Enterprise**: $14.99/month — multi-user (small agency), integration with FreshBooks/QuickBooks/Wave/Stripe, "awkward conversation" phone scripts, small claims court filing guide, payment analytics dashboard
- **Projected conversion rate**: 8% (benchmarked against Wave's estimated 6% conversion on invoicing tools; improved by the narrower, higher-pain-point focus — users arrive specifically because they have a collections problem, not a general invoicing need)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (Vercel/Railway) | $80 |
| SendGrid (escalation emails) | $100 |
| Twilio (optional SMS reminders) | $60 |
| FreshBooks/QuickBooks API integration costs | $50 |
| Marketing | $400 |
| Total Monthly Burn | $690 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $10 (blended: $3 organic from freelancer subreddits/communities + $22 paid via Instagram/LinkedIn ads targeting "freelancer" interests) |
| LTV | $63 (average retention 9 months at $6.99/mo; benchmarked against FreshBooks' ~12-month freelancer retention, discounted because this is a supplementary tool not a full accounting suite) |
| LTV:CAC | 6.3:1 |
| Payback Period | 1.4 months |
| Gross Margin | 91% (email + SMS costs ~$0.60/user/month against $6.99 ARPU; lowest marginal cost of all 10 ideas) |

## Go-to-Market: First 100 Users
1. **r/freelance "getting paid" threads**: r/freelance has weekly threads about late-paying clients. Post a detailed "My automated follow-up system that recovered $12K in overdue invoices" breakdown. Share the exact email templates (builds trust), then mention the app automates the process.
2. **Freelancer Twitter/X threads**: Write a viral thread — "I've freelanced for 8 years. Here are the 5 emails I send when clients don't pay (in order)." Include the escalation sequence word-for-word. Close with "I automated this into an app."
3. **Product Hunt launch**: Frame as "the collections agency freelancers actually want" — a fun, slightly provocative angle. Target Tuesday launch for maximum visibility.
4. **Freelance community partnerships**: Get featured in the Freelancers Union newsletter (500K+ members), CreativeMornings community, and Working Not Working network. Offer 3-month free premium to their members.
5. **Integration marketplace listings**: List on the FreshBooks App Store, QuickBooks App Store, and Wave marketplace as a "payment follow-up" add-on. Users of these tools already have the payment problem and are searching for solutions.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 1,650 paid | $139K | 20,600 free users at 8% conversion; organic from freelancer communities |
| 2 | 5,500 paid | $460K | FreshBooks/QuickBooks integrations drive distribution; ARPU $7 |
| 3 | 16,500 paid | $1.4M | Premium tier raises ARPU to $8; agency tier gains traction |
| 4 | 30,000 paid | $2.8M | ARPU $8.50; add international payment tracking (multi-currency); expand to UK/EU freelancers |
| 5 | 48,000 paid | $4.8M | ARPU $8.30; partner with freelance platforms (Upwork, Fiverr) for native integration; employer/agency bulk licenses |

## Key Weekly Metrics
1. **Invoices tracked** (total active invoices in the system; leading indicator of engagement)
2. **Free-to-paid conversion rate** (target: 8%+)
3. **Recovery rate** (% of overdue invoices that get paid after escalation sequence; target: 65%+; north star metric)
4. **Average days-to-payment reduction** (target: reduce from 13 days late to 5 days late)
5. **Escalation emails sent** (measures automation adoption; target: 80%+ of paid users have active sequences)
6. **Client reliability scores viewed** (are users checking scores before taking on new clients? measures engagement with preventive feature)
7. **Monthly churn rate** (target: <7%; freelancer tools have moderate churn — must prove ongoing value)

## Top 3 Risks
1. **FreshBooks, QuickBooks, or Wave add smart escalation sequences natively** — These platforms already send basic reminders and could upgrade to intelligent escalation. Mitigation: Go deeper than any invoicing platform will — client reliability scores, awkward conversation scripts, small claims guidance, and cross-platform tracking (not just invoices within one tool). Position as the specialist "collections layer" that sits on top of any invoicing tool.
2. **Freelancers find the automated emails too aggressive and fear damaging client relationships** — If a client receives a "final notice" email and gets offended, the freelancer blames the tool. Mitigation: Let users preview every email before it sends (opt-in for fully automated, manual approval by default for first 30 days). Provide a "tone slider" (gentle to firm) for each escalation step. Include "pause sequence" one-tap button for sensitive clients.
3. **Low willingness to pay among cash-strapped freelancers** — Freelancers who struggle with late payments are often the ones who can least afford another $7/month tool. Mitigation: Emphasize ROI — "one recovered $500 invoice pays for 6 years of the app." Offer a "pay from recovered invoice" option (first month free, charged only after the app helps recover a payment). Annual plan discount ($59/year = $4.92/month).
