# Business Model: Small Claims Guide

## Value Proposition
Recover the money you're owed — get a step-by-step, state-specific guide that takes you from "I think I have a case" through filing, hearing prep, and judgment collection, without hiring a $3,000 attorney for a $5,000 dispute.

## Customer Segments
- **Primary**: Individuals (ages 25-55) with disputes under $10K — landlord/tenant security deposit fights, contractor no-shows, unpaid freelance invoices, car accident damage. Psychographically: frustrated, feeling powerless, willing to put in effort if given a clear path, motivated by justice and recovering real money.
- **Secondary**: Small business owners dealing with non-paying customers or vendor disputes. Psychographically: time-constrained, pragmatic, want ROI on effort.
- **Tertiary**: Defendants served with small claims complaints who need to understand the process and prepare a defense.

## Revenue Model
- **Free tier**: Case evaluator quiz (determines if small claims is appropriate), state-specific monetary limit lookup, general overview of the process
- **Paid tier**: $29.99 one-time per case — state-specific document generation (complaint, demand letter), evidence coaching, hearing prep guide, day-of checklist, collection guide
- **Premium/Enterprise**: $49.99 per case — everything in paid plus defendant mode, appeal guidance, 1-on-1 AI hearing simulation, post-judgment enforcement toolkit
- **Projected conversion rate**: 15% (benchmarked against LegalZoom's 10-18% conversion on legal self-help; high intent users with real money at stake)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $120 |
| AI document generation (OpenAI API) | $350 |
| Legal content review (contract) | $500 |
| Marketing (SEO + content) | $1,800 |
| Payment processing (Stripe 2.9%) | $200 |
| Total Monthly Burn | $2,970 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $12 |
| LTV | $35 (avg 1.15 purchases per user — some buy defendant mode or help a friend) |
| LTV:CAC | 2.9:1 |
| Payback Period | 0 months (one-time purchase) |
| Gross Margin | 85% |

## Go-to-Market: First 100 Users
- **SEO (primary channel)**: Target "how to file small claims court [state]" (50-state long-tail strategy), "small claims court guide," "demand letter template," "how to sue someone in small claims" — all high-intent, high-volume queries
- **Reddit**: Answer questions in r/legaladvice (2.5M members), r/landlord (55K), r/Tenant (28K), r/freelance (370K) with genuine guidance and link to tool
- **YouTube**: Create "How to File Small Claims in [State]" video series — each video targets a specific state and drives to the app
- **Avvo/Quora**: Answer small claims questions with detailed helpful answers and soft CTA
- **Local courthouse partnerships**: Flyers or digital signage in small claims court waiting areas (start with 5 counties)

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 20,000 visitors / 3,000 purchases | $90K | SEO ramp-up; 15% conversion; avg $30/purchase |
| 2 | 80,000 visitors / 12,000 purchases | $390K | SEO compounds; YouTube channel grows; premium tier at $50 drives blended price up |
| 3 | 200,000 visitors / 30,000 purchases | $900K | All 50 states covered; defendant mode launched; brand awareness via legal content |
| 4 | 350,000 visitors / 50,000 purchases | $1.7M | B2B partnerships with legal aid organizations; embedded in tenant rights sites |
| 5 | 500,000 visitors / 75,000 purchases | $2.6M | Expansion to mediation and arbitration guides; partnership with court systems |

## Key Weekly Metrics
1. **Case evaluator completions** — top-of-funnel engagement; target 500+/week by month 6
2. **Purchase conversion rate** — target 15%+ from evaluator to purchase
3. **Document generation completions** — measures product value delivery
4. **SEO rankings for target keywords** — track top 50 state-specific queries weekly
5. **Refund request rate** — target below 3%; signals content quality
6. **State coverage gaps** — track which states users request that aren't fully supported
7. **User satisfaction rating (post-hearing survey)** — target 4.2+/5

## Top 3 Risks
1. **Legal liability from inaccurate state-specific information** → Prominent disclaimers that the app provides legal information, not legal advice; contract with a legal content reviewer to audit all 50-state content quarterly; user feedback loop for corrections
2. **Low repeat purchase rate inherent to one-time transactions** → Expand into adjacent legal self-help (demand letters, lease disputes, consumer complaints); add defendant mode; referral program offering $5 credit for friend purchases
3. **State laws and court procedures change frequently** → Build a state-law monitoring system; partner with law school clinics for free content updates; prioritize the 10 highest-volume states for maintenance
