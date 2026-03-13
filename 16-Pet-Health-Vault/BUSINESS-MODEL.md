# Business Model: Pet Health Vault

## Value Proposition
Pet owners never lose a vaccination record, miss a vet appointment, or scramble to share health history again — all pet health records live in one portable vault with a shareable QR code, breed-specific health alerts, and medication reminders that keep pets on track.

## Customer Segments
- **Primary**: Pet owners ages 25-45 with dogs or cats, especially multi-pet households (35% of pet owners). Household income $50K-$100K. They treat pets as family members, spend willingly on pet health, and are frustrated by paper vet records scattered across folders and email inboxes.
- **Secondary**: Pet sitters, dog walkers, and boarding facilities who need quick access to a pet's vaccination and health records.
- **Psychographics**: Emotionally invested "pet parents" who feel guilty when they miss a vaccination or forget medication dosages. They're organized in other areas of life (use apps for everything) but have no digital system for pet health. Active in r/dogs, r/cats, and breed-specific subreddits.

## Revenue Model
- **Free tier**: 1 pet profile with basic vaccination tracking and manual entry; vet visit log; shareable health card (view-only)
- **Paid tier**: $3.99/month — unlocks unlimited pets, medication reminders with dosage tracking, breed-specific health alerts, weight/wellness charts, receipt photo scanning, emergency vet locator, and exportable PDF reports
- **Premium/Enterprise**: $14.99/month per clinic — vet practice dashboard to push records directly to pet owner accounts (B2B, Year 2+)
- **Projected conversion rate**: 7% free-to-paid (benchmarked against pet app 11pets' estimated 5% conversion, adjusted up due to multi-pet household paywall and stronger feature differentiation)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $60 |
| APIs/Services (push notifications, cloud storage for documents/photos) | $200 |
| Marketing (social media, influencer partnerships) | $450 |
| Total Monthly Burn | $710 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $7 |
| LTV | $96 (avg 24-month retention at $4/mo; pets live 10-15 years, so need is ongoing) |
| LTV:CAC | 13.7:1 |
| Payback Period | 1.8 months |
| Gross Margin | 90% |

## Go-to-Market: First 100 Users
1. **Reddit pet communities (weeks 1-6)**: Share breed-specific health timelines (e.g., "Complete vaccination and screening schedule for Golden Retrievers, year by year") in r/dogs (4.7M), r/cats (5M), r/GoldenRetrievers (780K), r/Dachshund (300K), and r/puppy101 (580K). These posts provide genuine value and naturally lead to "I built an app that automates this."
2. **Pet influencer partnerships (weeks 3-8)**: Send free premium access to 10 Instagram/TikTok pet accounts with 10K-100K followers. Ask for an honest review showing the QR health card feature. Budget: $0-$200 per influencer (many pet accounts do product reviews for free product/access).
3. **Veterinary clinic partnerships (weeks 6-12)**: Visit 15 local vet clinics with printed QR code table cards: "Keep your pet's records in one place — scan to download." Offer clinics a free trial of the provider dashboard so they can push records directly to owners.
4. **Dog park and pet store flyers (weeks 4-8)**: Post flyers at 30 local dog parks, PetSmart/Petco community boards, and grooming salons. QR code to download with tagline: "Your pet's health records. Always with you."

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 8,000 | $120K | 2,500 paid at $4/mo; organic growth from pet communities |
| 2 | 28,000 | $420K | 8,750 paid; vet clinic partnerships in 10 metros drive adoption |
| 3 | 65,000 | $1.2M | 25,000 paid; B2B vet dashboard adds $80K; breed community partnerships |
| 4 | 120,000 | $2.3M | 45,000 paid; pet insurance company partnerships for record sharing |
| 5 | 200,000 | $3.8M | 70,000 paid + $300K B2B; expand to pet insurance marketplace (affiliate) |

## Key Weekly Metrics
1. New pet profiles created per week (target: 200/week by month 6)
2. Free-to-paid conversion rate (target: 7%)
3. Monthly churn rate (target: <3.5%)
4. Vaccination reminder completion rate (did the owner mark the vaccine as done? — target: 60%)
5. QR health card shares per week (viral loop indicator — target: 50/week)
6. Multi-pet upgrade rate (% of free users who add a 2nd pet and hit the paywall — target: 25%)
7. Vet clinic partnership sign-ups (target: 5 new clinics/month by month 6)

## Top 3 Risks
1. **Vet clinic adoption of push-records feature** — Vets use entrenched practice management software (IDEXX, eVetPractice) and may not want another system to manage. → Mitigation: Build integrations with top 3 practice management systems via their APIs rather than asking vets to use a separate dashboard; position the tool as reducing front-desk phone calls ("pet owners stop calling for records because they already have them").
2. **Data entry burden for existing pet records** — New users must manually enter years of existing pet health history, which is tedious and may cause drop-off during onboarding. → Mitigation: Build OCR receipt/document scanning that auto-extracts vaccination dates and types from vet invoices; allow users to start fresh ("track from today forward") with no backfill required; offer a one-time "records import" service for $4.99 where support manually enters records from uploaded photos.
3. **Emotional churn from pet loss** — When a pet dies, the owner churns and may associate the app with grief. → Mitigation: Handle this sensitively with a "memorial" mode that preserves the pet's profile without active reminders; offer to export all records as a PDF keepsake; send a genuine condolence message (not a retention email); if the owner has other pets, the multi-pet value keeps them subscribed.
