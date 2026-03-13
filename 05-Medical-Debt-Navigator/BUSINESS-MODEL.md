# Business Model: Medical Debt Navigator

## Value Proposition
Reduce your medical bills by 40-80% by finding financial assistance programs you didn't know existed, generating pre-filled applications, and giving you word-for-word negotiation scripts — without paying a human negotiator 25-35% of your savings.

## Customer Segments
- **Primary**: Uninsured or underinsured Americans aged 25-55 with household income $25K-$75K who have received a medical bill over $500. They're stressed, confused by the billing system, and don't know they have options. Found on r/povertyfinance, r/personalfinance, r/HealthInsurance, and medical debt TikTok.
- **Secondary**: Insured patients with high-deductible health plans (HDHPs) who face $3K-$8K in out-of-pocket costs for procedures. Also parents navigating bills for children's medical care.
- **Psychographics**: Feeling overwhelmed and powerless against a system that feels rigged. They want a guide, not just information. Highly price-sensitive — the tool needs to cost a fraction of what a human negotiator charges.

## Revenue Model
- **Free tier**: Upload one bill, see if the hospital has a financial assistance program, get a basic overcharge flag if the bill exceeds 150% of Medicare rates
- **Paid tier**: $9.99/month or $29.99 one-time — pre-filled financial assistance applications, full negotiation script library, Medicare rate comparison for all procedure codes, payment plan optimizer, dispute tracking
- **Premium/Enterprise**: $79.99 one-time "Full Navigator" — everything in paid tier plus a human review of the financial assistance application, 30-minute call coaching session, and small claims guidance
- **Projected conversion rate**: 18% (benchmarked against Credit Karma's 15% conversion on high-intent financial tools; improved because users arrive with an urgent, high-stakes problem — a bill they need to reduce)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $120 |
| Hospital financial assistance database maintenance | $300 (manual updates + web scraping) |
| Medicare rate API / CMS data processing | $100 |
| OpenAI API (script generation, application filling) | $200 |
| Marketing | $400 |
| Total Monthly Burn | $1,120 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $7 (blended: $2 organic from Reddit/TikTok virality + $15 paid via Google Ads targeting "reduce medical bill" keywords) |
| LTV | $32 (weighted avg: 60% buy $29.99 one-time, 25% subscribe at $9.99 for 3 months avg, 15% buy $79.99 premium) |
| LTV:CAC | 4.6:1 |
| Payback Period | Immediate (majority of revenue is one-time purchases) |
| Gross Margin | 86% (low per-user API costs; hospital database is a fixed cost amortized across users) |

## Go-to-Market: First 100 Users
1. **r/povertyfinance and r/personalfinance**: Post detailed guides like "I got my $8,400 ER bill reduced to $840 — here's exactly how" with step-by-step process. Include the tool as "I built an app to automate this." These posts routinely get 2K-10K upvotes.
2. **Medical debt TikTok**: Create a series of "Did you know?" videos — "Did you know every non-profit hospital MUST offer financial assistance by law?" Partner with creators like @medicalbillingcoach and @thefinancialdiet.
3. **Google Ads on high-intent keywords**: Target "how to reduce medical bill," "hospital financial assistance application," and "negotiate medical debt" — these have strong buyer intent and low competition ($2-5 CPC).
4. **Healthcare social workers and patient advocates**: Email 100 hospital social workers and patient advocacy organizations (Patient Advocate Foundation, Dollar For). Offer free access for them to share with patients.
5. **Medical debt Facebook groups**: Join and provide value in groups like "Medical Debt Help & Support" (15K+ members) and "Uninsured America" with actionable tips and soft tool mentions.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 7,300 paying users | $220K | Mix of one-time and subscription; 18% conversion from 40,500 free users |
| 2 | 22,000 paying users | $660K | Google Ads scale; social worker referral network; press coverage |
| 3 | 50,000 paying users | $1.5M | Add employer benefit channel (HR teams offer to employees); ARPU grows to $30 |
| 4 | 85,000 paying users | $2.8M | Partnership with patient advocacy nonprofits; expand to dental/vision debt |
| 5 | 130,000 paying users | $4.5M | White-label for health systems wanting to direct patients to assistance; ARPU $34 |

## Key Weekly Metrics
1. **Bills uploaded** (top-of-funnel volume; target: 500+/week by Month 6)
2. **Financial assistance applications generated** (core value delivery; target: 30%+ of uploads)
3. **Free-to-paid conversion rate** (target: 18%+)
4. **Average bill reduction achieved** (validates value prop; target: 50%+ reduction)
5. **User-reported savings** (north star for marketing; "users saved $X total")
6. **Hospital database coverage** (% of US hospitals with financial assistance data; target: 80%+ of non-profit hospitals)
7. **Referral rate** (target: 0.5 — each user tells at least one person about the tool)

## Top 3 Risks
1. **Hospital financial assistance policies change frequently and data goes stale** — If users generate applications based on outdated eligibility criteria, trust is destroyed. Mitigation: Build automated scrapers for the 500 largest non-profit hospital systems (covering 70% of volume). Crowdsource updates from users ("Was this policy accurate? Y/N"). Hire a part-time VA to verify top hospitals quarterly.
2. **Regulatory risk — could be classified as "debt settlement" requiring state licensing** — Some states regulate debt negotiation services. Mitigation: Position as an "educational tool and document generator," not as a negotiation service. Legal review of terms of service in all 50 states. The tool provides scripts and applications — it doesn't negotiate on the user's behalf.
3. **Users may not follow through on applications and scripts, leading to poor outcomes and bad reviews** — The tool generates documents, but users must still make phone calls and submit applications. Mitigation: Build a step-by-step tracker with SMS reminders. Offer the premium tier with human coaching for users who need hand-holding. Track completion rates and proactively re-engage users who stall.
