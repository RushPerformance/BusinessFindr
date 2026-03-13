# Business Model: Gig Tax Autopilot

## Value Proposition
Stop overpaying the IRS by $3,000-$5,000/year — automatically track mileage, find gig-specific deductions, and get told exactly how much to set aside for quarterly taxes, all for half the price of Keeper Tax.

## Customer Segments
- **Primary**: US gig workers aged 22-45 who drive for Uber/Lyft/DoorDash or sell on Etsy/eBay, earning $20K-$80K/year from gig work. They know they should be paying quarterly taxes but don't, and they panic every April. Found on r/uberdrivers (240K members), r/doordash (350K members), r/Etsy (175K members), and gig worker Facebook groups.
- **Secondary**: Side-hustle freelancers (designers, writers, developers) who have a W-2 job plus freelance income and need to track deductions for the freelance portion. Also multi-platform gig workers juggling 3+ apps.
- **Psychographics**: Living paycheck to paycheck with variable income. Intimidated by taxes and distrustful of complex software. They want an app that tells them exactly what to do — not a tool that requires accounting knowledge.

## Revenue Model
- **Free tier**: Basic income tracking from 1 gig platform, manual mileage logging, estimated quarterly tax amount (no deductions)
- **Paid tier**: $7.99/month ($59.99/year) — unlimited platform connections, automatic GPS mileage tracking, AI deduction finder, quarterly tax estimates with deductions, set-aside alerts, IRS payment voucher generation
- **Premium/Enterprise**: $14.99/month — multi-state tax support, year-end tax document package, 1099-NEC/K reconciliation, priority support during tax season
- **Projected conversion rate**: 7% (benchmarked against Stride's estimated 5% conversion on their free-to-premium mileage tool; improved by offering quarterly tax estimation — a must-have feature Stride lacks)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $200 |
| Plaid API (bank + gig platform connections) | $600 |
| Google Maps API (mileage verification) | $150 |
| OpenAI API (deduction classification) | $180 |
| Marketing | $500 |
| Total Monthly Burn | $1,630 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $15 (blended: $5 organic from gig worker subreddits/groups + $30 paid via Facebook/Instagram ads targeting "DoorDash driver" interests) |
| LTV | $72 (average retention 9 months at $7.99/mo; benchmarked against Keeper Tax's estimated 10-month retention, discounted for lower price point and more price-sensitive audience) |
| LTV:CAC | 4.8:1 |
| Payback Period | 1.9 months |
| Gross Margin | 84% (API and GPS costs ~$1.30/user/month against $7.99 ARPU) |

## Go-to-Market: First 100 Users
1. **r/uberdrivers, r/doordash, r/lyftdrivers**: Post "I tracked every deduction as a DoorDash driver for 6 months — here's how much I saved" with real numbers. Gig worker subreddits have intense engagement around tax topics, especially Q1.
2. **Gig worker Facebook groups**: Join "Uber Drivers Forum" (500K+ members), "DoorDash Drivers" (200K+), and "Etsy Sellers" groups. Post tax tip content weekly; share the app when quarterly tax deadlines approach (Jan 15, Apr 15, Jun 15, Sep 15).
3. **Tax season content blitz on YouTube**: Create "Uber Driver Tax Deductions You're Missing" and "How to Pay Quarterly Taxes as a Gig Worker" videos. These keywords spike 5x every January-April on Google Trends.
4. **Partnership with gig worker advocacy orgs**: Reach out to the Gig Workers Collective and Rideshare Drivers United to offer discounted access to their members.
5. **Quarterly tax deadline email campaigns**: Capture emails via a free "Quarterly Tax Calculator" landing page. Send reminders with deadline urgency 2 weeks before each IRS quarterly due date.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 2,000 paid | $190K | 28,500 free users at 7% conversion; organic gig worker community growth |
| 2 | 7,500 paid | $720K | Annual plan adoption smooths revenue; add Etsy/eBay platform integrations |
| 3 | 24,000 paid | $2.3M | ARPU $8.50 with premium tier; tax season referral spikes |
| 4 | 42,000 paid | $4.2M | Add multi-state support; partner with tax filing services for Year-end handoff |
| 5 | 65,000 paid | $7.0M | ARPU $9.00; expand to 1099 contractors beyond gig platforms; TurboTax integration |

## Key Weekly Metrics
1. **Miles tracked** (core engagement metric; target: 80%+ of paid users tracking weekly)
2. **Free-to-paid conversion rate** (target: 7%+)
3. **Quarterly tax estimates generated** (seasonal spike; validates core value prop)
4. **Deductions found per user** (target: $200+/month in identified deductions)
5. **Platform connections per user** (target: 2.3 avg — multi-platform users are stickier)
6. **Day 14 retention** (target: 50%+ for free users; mileage tracking needs habit formation)
7. **Tax season signups vs. off-season** (track seasonality to plan marketing spend)

## Top 3 Risks
1. **Mileage tracking battery drain causes uninstalls** — Background GPS is notorious for battery complaints, which drives 1-star reviews and uninstalls. Mitigation: Use motion activity detection to activate GPS only during driving. Offer Bluetooth OBD auto-detection as an alternative. Show battery usage in-app ("Gig Tax Autopilot used 3% battery today") for transparency.
2. **Tax advice liability — incorrect deduction recommendations could cost users** — If the AI flags a non-deductible expense as deductible, users could face IRS penalties. Mitigation: Add disclaimers ("not tax advice"), cross-reference deductions against IRS Publication 463 rules, build in conservative defaults, and offer CPA review add-on for $29.99 at year-end.
3. **Gig platforms restrict API access or data sharing** — Uber, DoorDash, and others may not provide open APIs for income data. Mitigation: Use Plaid for bank transaction import as primary method (gig deposits appear as recognizable transactions). Email parsing for 1099s and weekly earnings summaries as secondary. Manual CSV upload as fallback.
