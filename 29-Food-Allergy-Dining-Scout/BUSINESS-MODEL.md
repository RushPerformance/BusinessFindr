# Business Model: Food Allergy Dining Scout

## Value Proposition
Eat out with confidence, not fear — find restaurants verified safe for your specific allergens, see community-tested "safe dishes," and protect your family with allergy-aware dining intel that prevents the 200,000 ER visits caused by restaurant food each year.

## Customer Segments
- **Primary**: Parents of children with food allergies (ages 28-50), predominantly mothers, household income $50K-$120K. Psychographically: hypervigilant, research-driven, willing to pay any reasonable amount for their child's safety, active in allergy communities, strong word-of-mouth behavior.
- **Secondary**: Adults with food allergies (ages 20-45), managing conditions like celiac disease, peanut/tree nut allergies, shellfish allergies. Psychographically: frustrated by limited options, socially anxious about dining out, value autonomy and independence.
- **Tertiary**: Restaurants wanting to attract allergy-conscious diners (B2B segment).

## Revenue Model
- **Free tier**: Browse restaurant listings, see community ratings, search by allergen, view chain restaurant allergen data
- **Paid tier**: $4.99/month — verified allergen menus, custom multi-allergen alerts, travel mode (search any city), allergy card generator (12 languages), EpiPen reminders
- **Premium/Enterprise**: $49/month (B2B) — restaurant verification badge, allergy-training resources, featured listing in allergen searches
- **Projected conversion rate**: 10% (benchmarked against Find Me Gluten Free's 8-12% conversion; allergy parents have extremely high willingness to pay for safety)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $200 |
| Maps/Places API (Google) | $350 |
| Content moderation (reviews) | $300 |
| Marketing (community + content) | $1,200 |
| App store fees (15-30%) | $200 |
| Total Monthly Burn | $2,250 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $15 |
| LTV | $150 (avg 30-month retention at $5/mo) |
| LTV:CAC | 10:1 |
| Payback Period | 3 months |
| Gross Margin | 80% |

## Go-to-Market: First 100 Users
- **Facebook Groups**: "Food Allergy Parents" (45K), "Peanut Allergy Support Group" (30K+), "Celiac Disease Support Group" (60K+), "FPIES Support Group" (15K) — share restaurant safety tips and app
- **Reddit**: r/FoodAllergies (22K), r/Celiac (60K), r/glutenfree (125K) — post value-first content about dining safety
- **FARE (Food Allergy Research & Education) partnership**: Reach their 250K+ community; offer free premium for FARE members for 3 months
- **Instagram**: Allergy-parent influencers (many with 10K-100K followers) are highly engaged and trust-based; offer free premium for reviews
- **Local allergy support groups**: Partner with 20 local allergy support groups in top metro areas to seed restaurant reviews

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 10,000 free / 1,000 paid | $60K | Seeded in 5 metro areas; 10% conversion; community reviews build value |
| 2 | 50,000 free / 6,000 paid | $360K | 25 metro areas; B2B restaurant tier launches; allergy parent word-of-mouth |
| 3 | 150,000 free / 12,000 paid + 200 restaurants | $840K | National coverage; B2B contributes $120K; partnerships with allergy organizations |
| 4 | 350,000 free / 25,000 paid + 600 restaurants | $1.9M | Travel mode drives international data; chain partnerships; B2B at $360K |
| 5 | 700,000 free / 45,000 paid + 1,500 restaurants | $3.6M | Dominant allergy dining platform; insurance/pharma partnerships; B2B at $900K |

## Key Weekly Metrics
1. **New restaurant reviews submitted** — community content is the core asset; target 200+/week by month 6
2. **Safe dish verifications** — measures depth of crowdsourced safety data
3. **MAU by allergen type** — ensures multi-allergen coverage, not just gluten-free dominance
4. **Free-to-paid conversion rate** — target 10%+
5. **Restaurant search-to-visit rate** — measures real-world impact
6. **Geographic coverage gaps** — track cities with fewer than 50 reviewed restaurants
7. **B2B restaurant sign-up rate** — target 5 new restaurants/week by month 9

## Top 3 Risks
1. **Liability if a user has an allergic reaction at a "verified safe" restaurant** → Strong disclaimers that reviews are community-sourced and not medical guarantees; verification badge indicates training, not absolute safety; carry business liability insurance ($1M policy ~$500/year)
2. **Cold start problem — not enough reviews to be useful at launch** → Pre-seed database with chain restaurant official allergen menus (100+ chains); recruit 50 "founding reviewers" with free lifetime premium; focus on 5 metro areas rather than launching nationally
3. **User-generated review quality and accuracy** → Implement verified-diner badges (receipt upload), community flagging system, and restaurant-response feature; weight reviews by reviewer history and allergen match
