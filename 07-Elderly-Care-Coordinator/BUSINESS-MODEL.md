# Business Model: Elderly Care Coordinator

## Value Proposition
Stop the sibling arguments, missed medications, and forgotten appointments — get one family dashboard that coordinates everything for Mom or Dad's care so no one drops the ball and everyone shares the load.

## Customer Segments
- **Primary**: Adult children aged 35-55 (the "sandwich generation") who are primary caregivers for an aging parent while raising their own kids. Household income $50K-$120K. They're overwhelmed, juggling caregiving with work, and frustrated that siblings aren't pulling their weight. Active on r/AgingParents (90K members), r/CaregiverSupport (25K members), and caregiver Facebook groups.
- **Secondary**: Long-distance caregivers (siblings who live 100+ miles from the parent) who feel guilty and want to stay informed and contribute. Also professional in-home caregivers who need to coordinate with family members.
- **Psychographics**: High emotional stress, guilt-driven, conflict-avoidant with siblings but resentful about unequal distribution of care tasks. They want structure and accountability — a neutral system that assigns tasks fairly.

## Revenue Model
- **Free tier**: 1 care recipient, 2 care circle members, basic medication list, shared calendar, emergency contacts
- **Paid tier**: $9.99/month — unlimited care circle members, medication reminders with refill alerts, task board with assignment and completion tracking, health journal, document vault, weekly summary emails
- **Premium/Enterprise**: $19.99/month — multiple care recipients (for families with both parents or in-laws), caregiver shift scheduling, integration with pharmacy refill services, telehealth appointment booking, priority support
- **Projected conversion rate**: 10% (benchmarked against Cozi family organizer app's 8% conversion; improved by higher emotional stakes and clearer paid-tier differentiation)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $180 |
| Twilio (medication reminders, SMS notifications) | $200 |
| SendGrid (weekly summary emails) | $50 |
| Cloud storage (document vault) | $80 |
| Marketing | $400 |
| Total Monthly Burn | $910 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $18 (blended: $6 organic from caregiver communities + $35 paid via Facebook ads targeting "caring for aging parents" interests) |
| LTV | $180 (average retention 18 months at $9.99/mo; benchmarked against CareZone's estimated 20-month retention before shutdown — caregivers are extremely sticky once onboarded because the care recipient's data is in the system) |
| LTV:CAC | 10:1 |
| Payback Period | 1.8 months |
| Gross Margin | 87% (notification + storage costs ~$1.30/family/month against $9.99 ARPU) |

## Go-to-Market: First 100 Users
1. **r/AgingParents and r/CaregiverSupport**: Post a genuine story about building the app after experiencing caregiver coordination chaos. Share specific pain points — "My sister lives 3 states away and kept asking 'what can I do?' but there was no way to assign tasks." The caregiver community responds powerfully to empathy.
2. **Caregiver Facebook groups**: Join "Caregivers Support Group" (80K members), "Dementia Caregivers Support" (120K members), and "Long Distance Caregiving" (15K members). Share the app after providing value with caregiving tips for 2-3 weeks.
3. **AARP and local Area Agencies on Aging**: Contact 20 local Area Agencies on Aging (government-funded caregiver support) and offer free access for caregivers they serve. These agencies are always looking for tools to recommend.
4. **Caregiver podcasts**: Pitch as a guest on "The Caregiving Years" and "Happy Healthy Caregiver" podcasts (both 5K-20K listeners). These audiences are highly targeted and underserved by tech.
5. **The "care circle invite" viral loop**: When one sibling signs up and invites 2-3 others, each invite is a potential new family account. Build the invite flow to be frictionless with a "join [Sister's Name]'s care circle for Mom" message.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 1,200 paid families | $144K | Organic caregiver community growth; 10% conversion from 12,000 free families |
| 2 | 4,500 paid families | $540K | Care circle viral loop drives 3.5x growth; AARP partnership discussions |
| 3 | 15,000 paid families | $1.8M | Premium tier raises ARPU to $11; partnerships with home health agencies |
| 4 | 28,000 paid families | $3.7M | ARPU $11.50; add pharmacy integration; employer caregiver benefit channel |
| 5 | 45,000 paid families | $6.2M | ARPU $11.50; expand to UK/Canada; telehealth integration; demographic tailwind (10K Americans turn 65 daily) |

## Key Weekly Metrics
1. **Care circles created** (top-of-funnel; each circle = a family onboarded)
2. **Care circle members per family** (target: 3.2+ members; more members = stickier and validates viral loop)
3. **Free-to-paid conversion rate** (target: 10%+)
4. **Tasks completed per family per week** (target: 5+; indicates active coordination use)
5. **Medication reminder acknowledgment rate** (target: 85%+; measures core safety feature engagement)
6. **Weekly summary email open rate** (target: 60%+; keeps remote family members engaged)
7. **Monthly family churn rate** (target: <4%; once a family is on the platform, leaving is disruptive)

## Top 3 Risks
1. **Low tech adoption among elderly parents and older caregivers** — The care recipient (elderly parent) may not use the app, and some sibling caregivers may resist yet another app. Mitigation: Design the parent-facing experience as SMS-only (medication reminders via text, not app). Keep the sibling experience simple — email summaries + one-tap task completion via link. Don't require the care recipient to use the app at all.
2. **Apple Health / Google Health add caregiver coordination features** — Apple or Google could add family health coordination to their health apps, leveraging their install base. Mitigation: Move fast on features Big Tech won't prioritize (task assignment, sibling accountability, weekly summaries). Build emotional community features (shared memory timeline, gratitude notes) that create switching costs beyond functionality.
3. **HIPAA and health data privacy concerns** — Storing medication lists and health journals raises data privacy questions even if the app isn't technically a "covered entity." Mitigation: Encrypt all health data at rest and in transit. Get SOC 2 Type I certification by Year 2. Publish a transparent privacy policy. Offer data export and deletion. Never sell or share health data — make this a core brand promise.
