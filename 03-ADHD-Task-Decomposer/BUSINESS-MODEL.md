# Business Model: ADHD Task Decomposer

## Value Proposition
Turn overwhelming, paralyzing tasks into dopamine-friendly micro-steps you can actually start — so you stop losing hours to task paralysis and start finishing what matters.

## Customer Segments
- **Primary**: US adults aged 22-40 diagnosed or self-identified with ADHD, earning $35K-$90K/year. They've tried Todoist, Things, Notion, and multiple productivity systems — all of which eventually fail because they're designed for neurotypical brains. They're active on ADHD TikTok, r/ADHD, and ADHD Twitter.
- **Secondary**: Parents of ADHD teens (13-18) who need homework and chore decomposition tools. Also therapists and ADHD coaches who recommend tools to clients.
- **Psychographics**: Self-aware about their ADHD challenges, hungry for tools that "get" them, and deeply loyal to products that don't shame them for inconsistency. Strong community identity — they share tools with each other.

## Revenue Model
- **Free tier**: 3 task decompositions per day, basic micro-step view, completion tracking
- **Paid tier**: $6.99/month — unlimited decompositions, energy-level matching, body-doubling timers, "just start" mode, ADHD-friendly streak mechanics, calendar integration
- **Premium/Enterprise**: $12.99/month — therapist/coach dashboard (assign tasks to clients, track completion), family plan (up to 3 users), custom celebration sounds
- **Projected conversion rate**: 5% (benchmarked against Todoist's 4% freemium conversion; improved by serving an underserved niche with high emotional attachment to the product)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (Vercel/Railway) | $100 |
| OpenAI API (task decomposition) | $350 (at ~$0.003/decomposition, 100K+ decompositions/month) |
| Audio CDN (body-doubling sounds) | $50 |
| Push notification service | $30 |
| Marketing | $400 |
| Total Monthly Burn | $930 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $8 (blended: $2 organic from ADHD TikTok/Reddit virality + $18 paid via Instagram/TikTok ads) |
| LTV | $56 (average retention 8 months at $6.99/mo, benchmarked against Headspace's 6-month ADHD-adjacent app retention, adjusted upward for niche loyalty) |
| LTV:CAC | 7:1 |
| Payback Period | 1.1 months |
| Gross Margin | 89% (API costs ~$0.75/user/month against $6.99 ARPU) |

## Go-to-Market: First 100 Users
1. **ADHD TikTok creators**: Partner with 3-5 micro-creators (10K-100K followers) in the ADHD niche (e.g., @connordewolfe, @catieosaurus) for organic-feeling "this app changed my morning routine" content. Offer free premium + $50-100 per video.
2. **r/ADHD engagement**: Participate genuinely in r/ADHD (2.1M members) for 4 weeks before soft-launching. Share the app as "something I built for myself" — the community rewards authenticity and punishes marketing.
3. **Goblin Tools comparison content**: Create TikToks and posts showing "Goblin Tools Magic ToDo is great, but here's what happens AFTER you decompose the task" — position as the workflow Goblin Tools is missing.
4. **ADHD coaches and therapists**: Email 50 ADHD coaches on Psychology Today and CHADD's provider directory. Offer free premium accounts in exchange for recommending to clients.
5. **Product Hunt launch**: Frame as "the first task manager designed for ADHD brains" — a fresh angle that generates curiosity clicks.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 2,500 paid | $210K | 50K free users at 5% conversion; ADHD TikTok virality drives organic growth |
| 2 | 10,000 paid | $838K | Blended ARPU $6.99; therapist referral network builds; launch iOS/Android apps |
| 3 | 30,000 paid | $2.5M | Premium tier adoption raises ARPU to $8.50; ADHD coaching integrations |
| 4 | 55,000 paid | $5.1M | International expansion (UK/Canada/Australia); localized content; ARPU $7.75 |
| 5 | 85,000 paid | $8.5M | Enterprise tier for ADHD coaching platforms; ARPU $8.30; partnerships with telehealth providers |

## Key Weekly Metrics
1. **Daily active decompositions** (are people using the core feature daily?)
2. **Free-to-paid conversion rate** (target: 5%+)
3. **Task completion rate** (% of decomposed micro-steps actually completed; target: 60%+)
4. **Day 7 retention** (target: 40%+ for free users — critical for ADHD apps where novelty wears off)
5. **Body-doubling session starts per user** (measures engagement with premium feature; target: 3+/week)
6. **NPS score** (target: 50+ — ADHD community is vocal; high NPS = referrals)
7. **TikTok/Reddit mentions** (organic word-of-mouth tracking)

## Top 3 Risks
1. **Novelty fatigue — ADHD users abandon new tools after the dopamine wears off** — This is the #1 killer of ADHD apps. Mitigation: Design for inconsistency — no punishment for missed days, "welcome back" flows instead of guilt, variable reward mechanics (surprise celebrations), and periodic UI refreshes to maintain novelty.
2. **OpenAI API quality degrades or pricing changes** — Decomposition quality depends on LLM output. Mitigation: Fine-tune a smaller open-source model (Llama/Mistral) on 50K+ decomposition examples as a fallback; cache common task decompositions to reduce API calls by 40%.
3. **Goblin Tools adds workflow features and becomes a direct competitor** — Goblin Tools has massive brand awareness in the ADHD community. Mitigation: Move fast on the timer/energy/body-doubling features that are hard to bolt on. Build community-driven decomposition templates that create a data moat.
