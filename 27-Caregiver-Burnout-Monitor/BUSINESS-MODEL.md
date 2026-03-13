# Business Model: Caregiver Burnout Monitor

## Value Proposition
Catch caregiver burnout before it becomes a crisis — giving family caregivers an early warning system that tracks their wellbeing, alerts loved ones when help is needed, and connects them to respite resources so they can sustain caregiving without sacrificing their own health.

## Customer Segments
- **Primary**: Adult children (ages 40-65) caring for aging parents, predominantly women (60%), middle-income households, sandwiched between caring for parents and their own children. Psychographically: guilt-driven, self-sacrificing, rarely prioritize their own health, skeptical of "self-care" messaging but responsive to data-driven health alerts.
- **Secondary**: Spouses caring for partners with chronic illness or disability (ages 50-75). Psychographically: isolated, reluctant to ask for help, motivated by duty.
- **Tertiary**: Siblings and family members of the primary caregiver who want to help but live far away and don't know when or how to step in.

## Revenue Model
- **Free tier**: Weekly check-ins, burnout score tracking, basic self-care suggestions
- **Paid tier**: $5.99/month — family alert system (notify up to 5 family members), respite resource finder, monthly doctor-shareable wellbeing report, community forum access, personalized self-care plans
- **Premium/Enterprise**: $14.99/month — family coordination dashboard (task assignment among siblings), professional caregiver matching, therapist directory integration
- **Projected conversion rate**: 6% (benchmarked against Calm's 4-6% conversion; higher emotional urgency drives willingness to pay)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $150 |
| Notification services (Twilio/SendGrid) | $120 |
| Respite resource database maintenance | $200 |
| Marketing (content + community) | $1,200 |
| App store fees (15-30%) | $200 |
| Total Monthly Burn | $1,870 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $22 |
| LTV | $180 (avg 30-month retention at $6/mo) |
| LTV:CAC | 8.2:1 |
| Payback Period | 3.7 months |
| Gross Margin | 82% |

## Go-to-Market: First 100 Users
- **Reddit**: Share burnout stories and app in r/CaregiverSupport (32K), r/AgingParents (48K), r/dementia (18K), r/Alzheimers (15K)
- **Facebook Groups**: Caregiver support groups are massive — "Caregiver Support Group" (200K+), "Alzheimer's and Dementia Caregivers" (180K+); share value content, not promotions
- **AARP partnership pitch**: Offer free premium to AARP members for first 3 months; AARP reaches 38M members
- **Content marketing**: Blog posts targeting "caregiver burnout signs," "am I burning out as a caregiver," "help for family caregivers" — high-emotion, high-search-volume terms
- **Social worker outreach**: Provide free accounts to 50 hospital social workers who counsel family caregivers daily

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 14,000 free / 835 paid | $60K | Organic + community-driven growth; 6% conversion |
| 2 | 45,000 free / 4,500 paid | $324K | AARP or similar partnership activated; media coverage of caregiver crisis |
| 3 | 120,000 free / 10,000 paid | $720K | Family tier drives 2.5x viral coefficient; respite matching revenue |
| 4 | 250,000 free / 20,000 paid | $1.4M | Enterprise tier sold to elder care agencies; insurance company partnerships |
| 5 | 500,000 free / 38,000 paid | $2.7M | National caregiver platform; data insights licensed to healthcare systems |

## Key Weekly Metrics
1. **Weekly check-in completion rate** — target 70%+; core engagement indicator
2. **Burnout score distribution** — population-level trends indicate product relevance
3. **Family alert activation rate** — % of paid users who connect family members
4. **Respite resource click-through rate** — measures value of recommendation engine
5. **Free-to-paid conversion rate** — target 6%+
6. **7-day retention** — target 60%+ (emotional apps face early drop-off)
7. **NPS score** — target 55+ (caregivers who feel supported become strong advocates)

## Top 3 Risks
1. **Users feel too overwhelmed to do even a 2-minute check-in** → Design ultra-minimal UX (5-tap check-in), allow voice entry, send gentle nudge notifications with affirming tone; offer skip-week option without guilt
2. **Respite resource database is incomplete or outdated across 50 states** → Start with top 10 metro areas, partner with Area Agencies on Aging (AAA), and crowdsource resource submissions from the community; expand geographically based on user demand
3. **Liability risk if burnout alerts are ignored and a crisis occurs** → Clear disclaimers that the app is not a medical device; partner with crisis hotlines (988 Suicide & Crisis Lifeline); escalation paths in the app for critical burnout scores
