# Business Model: Plant Parent Scheduler

## Value Proposition
Stop killing your houseplants — get personalized care schedules based on your specific plants, pots, and light conditions, with timely reminders that prevent the #1 cause of houseplant death (overwatering) and keep your growing collection thriving year-round.

## Customer Segments
- **Primary**: Millennial and Gen Z plant owners (ages 22-38), predominantly women, owning 5-20 houseplants. Household income $35K-$90K. Psychographically: identify as "plant parents," emotionally attached to their plants, active on Instagram/TikTok plant communities, aesthetically driven, feel guilty when plants die.
- **Secondary**: New plant owners (ages 25-45) who have killed multiple plants and are seeking structured guidance. Psychographically: frustrated, self-described "black thumbs," willing to pay for success after repeated failure.
- **Tertiary**: Serious hobbyists (ages 30-55) with 20-100+ plants who need organizational tools to manage complex care schedules across many species.

## Revenue Model
- **Free tier**: Up to 5 plants, basic watering reminders (species-level defaults), plant identification (3/month)
- **Paid tier**: $2.99/month — unlimited plants, personalized schedules (pot size + light + season), fertilizing calendar, repotting alerts, plant journal with photos, diagnosis tool, seasonal auto-adjustments
- **Premium/Enterprise**: $5.99/month — AI plant doctor (photo diagnosis), product recommendations, rare plant care guides, community access, multi-location support (home + office)
- **Projected conversion rate**: 7% (benchmarked against Planta's estimated 5-8% conversion; lower price point and strong emotional attachment to plants support conversion)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $100 |
| Plant identification API (PlantNet) | $150 |
| AI diagnosis (OpenAI Vision API) | $200 |
| Marketing (social + influencer) | $900 |
| App store fees (15-30%) | $100 |
| Total Monthly Burn | $1,450 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $7 |
| LTV | $47 (avg 16-month retention at $3/mo; plant ownership is ongoing but casual users churn) |
| LTV:CAC | 6.7:1 |
| Payback Period | 2.3 months |
| Gross Margin | 83% |

## Go-to-Market: First 100 Users
- **Reddit**: r/houseplants (1.3M), r/plantclinic (600K), r/IndoorGarden (310K), r/succulents (400K), r/proplifting (170K) — post plant care tips, diagnosis help, and watering schedules
- **Instagram**: Plant Instagram is enormous; partner with 15 micro-influencers (5K-50K followers) in the #plantparent, #houseplantclub, #plantsofinstagram communities; free premium for reviews
- **TikTok**: "Why your monstera is dying" and "plant care routine" videos; demonstrate the app in plant-care-day content
- **Plant shop partnerships**: Partner with 10 local plant shops and nurseries to include app QR codes with plant purchases ("Your new plant comes with a free care schedule")
- **Facebook Groups**: "Houseplant Hobbyist" (700K+), "House Plant Addicts" (200K+) — share seasonal care adjustment reminders

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 13,000 free / 900 paid | $32K | Instagram/TikTok + plant community organic growth; 7% conversion |
| 2 | 50,000 free / 4,500 paid | $162K | Plant shop partnerships in 20 cities; premium tier launches |
| 3 | 150,000 free / 9,000 paid | $324K | Affiliate revenue from plant product recommendations adds $30K |
| 4 | 350,000 free / 18,000 paid | $648K | + $80K affiliate; brand partnerships with Miracle-Gro, The Sill, Bloomscape |
| 5 | 700,000 free / 32,000 paid | $1.2M | + $150K affiliate/sponsorship; expansion to outdoor gardening; plant marketplace |

## Key Weekly Metrics
1. **Watering reminders completed (marked done)** — core engagement; target 80%+ completion rate
2. **Plants added per user** — measures depth of adoption; target 8+ plants per active user
3. **Plant journal entries** — indicates emotional engagement and long-term retention
4. **Diagnosis tool usage** — high-value feature; track weekly queries
5. **Free-to-paid conversion rate** — target 7%+
6. **7-day retention** — target 55%+ (reminder apps face early drop-off if reminders feel nagging)
7. **Seasonal schedule adjustment engagement** — do users interact with seasonal changes? Validates personalization value

## Top 3 Risks
1. **Planta is well-established at $7.99/month with a large plant database** → Compete on price ($3 vs $8), target casual plant owners Planta doesn't serve well, and differentiate on environmental personalization (pot size, exact light conditions) rather than just species defaults
2. **Users find reminders annoying and disable notifications** → Smart notification timing (mornings on watering days only); batch notifications ("3 plants need water today"); allow snooze/skip without guilt; let users set quiet days
3. **Seasonal adjustments require complex environmental modeling that's hard to get right** → Start with simple season-based rules (winter = less water) and refine with user feedback; allow manual overrides; transparent explanation of why schedules change; user-reported outcomes improve the algorithm over time
