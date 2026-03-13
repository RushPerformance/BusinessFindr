# Business Model: Contractor Bid Comparer

## Value Proposition
Homeowners save 10-25% on renovation projects by comparing contractor bids apples-to-apples — the app normalizes messy quotes into comparable line items, flags missing scope, and shows whether each price is fair for their zip code, turning a stressful guessing game into a confident decision.

## Customer Segments
- **Primary**: Homeowners ages 30-55 planning renovations costing $5K-$100K (bathroom remodels, kitchen renovations, roofing, decks). Household income $70K-$150K. They've received 2-4 contractor quotes and can't figure out which is actually the best deal. They're Googling "how to compare contractor bids" and feeling overwhelmed.
- **Secondary**: Real estate investors and house flippers managing multiple renovation projects who need to compare bids quickly and consistently.
- **Psychographics**: Risk-averse and research-oriented. They read every Yelp review, check licenses, and still feel uncertain. They want data to validate their gut feeling about which contractor to hire. They've been burned before (or heard horror stories) and are terrified of overpaying or hiring the wrong person.

## Revenue Model
- **Free tier**: Upload 1 bid; see a basic line-item breakdown; get 1 "missing scope" alert
- **Paid tier**: $9.99 one-time per comparison project (up to 5 bids) — unlocks full AI normalization, side-by-side comparison, complete missing scope analysis, local price benchmarks, red flag detection, weighted decision matrix, and questions-to-ask list
- **Premium/Enterprise**: $7.99/month unlimited — for active renovators or investors comparing bids across multiple projects; adds saved project history, contractor scorecards, and price trend tracking
- **Projected conversion rate**: 18% free-to-paid (benchmarked against HomeAdvisor's lead conversion rate of 15-20%; users arriving with bids in hand have extremely high purchase intent)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $60 |
| APIs/Services (OpenAI for bid normalization, OCR for PDF/photo parsing, price benchmark database) | $400 |
| Marketing (SEO, Google Ads, content) | $550 |
| Total Monthly Burn | $1,010 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $15 |
| LTV | $22 (weighted avg: 75% buy $9.99 one-time, 15% subscribe at $7.99/mo for 6 months, 10% buy multiple one-time projects) |
| LTV:CAC | 1.5:1 |
| Payback Period | 0 months (one-time purchase — immediate) |
| Gross Margin | 82% |

## Go-to-Market: First 100 Users
1. **SEO (weeks 1-12)**: Publish 15 project-specific guides: "How to compare bathroom remodel bids," "What should be included in a roofing quote," "Average cost of kitchen renovation in [city]." Target "how to compare contractor quotes" (22K monthly searches), "contractor bid template," and "is my contractor quote fair." These are high-intent, decision-stage queries.
2. **Reddit (weeks 1-8)**: Provide detailed bid analysis in r/HomeImprovement (5.5M), r/homeowners (310K), r/Renovations (60K), and r/RealEstateInvesting (350K). When users post "Got 3 quotes — which should I pick?", analyze their bids publicly and recommend the app for future projects.
3. **Google Ads (weeks 4-12)**: Run search ads on "compare contractor bids," "is my renovation quote fair," and "contractor bid comparison tool." CPC est. $2-$4. Budget: $300/month. These are transactional keywords with high conversion potential.
4. **Home improvement store partnerships (weeks 8-12)**: Create co-branded "Getting Quotes? Compare Them Free" flyers for Home Depot and Lowe's contractor referral desks. Many customers getting quotes at these stores are the exact target audience.

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 10,000 | $96K | 8,000 one-time purchases + 500 subscribers; SEO + Google Ads |
| 2 | 30,000 | $300K | SEO compounds; subscriber base grows to 2,000; add project-specific pricing databases |
| 3 | 70,000 | $960K | Contractor verification badges (paid by contractors) add $200K; investor tier drives recurring revenue |
| 4 | 120,000 | $1.8M | Contractor matching marketplace (connect users to vetted contractors for a referral fee); B2B API for real estate platforms |
| 5 | 200,000 | $3.0M | Full contractor marketplace with bid submission; $500K in contractor advertising revenue |

## Key Weekly Metrics
1. Bids uploaded per week (target: 200/week by month 6)
2. Free-to-paid conversion rate (target: 18%)
3. Comparison projects completed (target: 80% of paid users complete their full comparison)
4. Monthly subscriber retention rate (target: 75% month-over-month for unlimited plan)
5. Organic search traffic to project-specific landing pages (target: 3,000 sessions/week by month 8)
6. Price benchmark database coverage (% of zip codes with data — target: top 100 metros by month 6)
7. User-reported savings per project (tracked via optional follow-up survey — target: $2,500 avg)

## Top 3 Risks
1. **AI bid normalization accuracy** — Contractor bids use wildly inconsistent formats, terminology, and scoping. An AI that misclassifies a "demolition" line item or misses a critical exclusion could lead to a bad hiring decision. → Mitigation: Train the AI on 500+ real contractor bids across 10 project types before launch; always show the original bid alongside the normalized version so users can verify; flag low-confidence normalizations with "please verify" labels; let users correct errors (which improves the model); start with the 5 most common project types (bathroom, kitchen, roofing, painting, flooring) where bid formats are most standardized.
2. **Thin price benchmark data** — Local pricing benchmarks require large datasets per zip code per project type; outside top metros, data may be too sparse to be useful. → Mitigation: Start with metro-level (not zip-code-level) benchmarks for the 30 largest US metros; supplement with national data from RSMeans and HomeAdvisor cost guides; display confidence levels ("based on 47 comparable projects in your area" vs. "based on 6 comparable projects — limited data"); let users contribute their final contracted price to build the database over time.
3. **Low LTV:CAC ratio limits growth investment** — At 1.5:1 LTV:CAC, there's limited room for paid acquisition, which constrains growth speed. → Mitigation: Double down on SEO (free traffic) and Reddit community building (zero marginal cost); increase LTV by converting one-time users to subscribers through follow-up emails ("Planning another project?"); launch the contractor marketplace in Year 2-3 to add a high-margin revenue stream that improves unit economics; consider raising the one-time price to $14.99 after proving value.
