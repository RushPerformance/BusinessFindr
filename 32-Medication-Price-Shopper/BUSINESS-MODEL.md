# Business Model: Medication Price Shopper

## Value Proposition
Cut your prescription costs by 50-90% by finding the cheapest pharmacy near you, surfacing manufacturer coupons and patient assistance programs that most people don't know exist, and suggesting generic alternatives — saving uninsured and underinsured Americans an average of $150/month on medications.

## Customer Segments
- **Primary**: Uninsured adults (ages 25-64), 29M Americans, disproportionately self-employed, gig workers, or between jobs. Household income $20K-$50K. Psychographically: highly price-sensitive, anxious about healthcare costs, resourceful, often skip doses or split pills to save money.
- **Secondary**: Underinsured adults with high-deductible health plans (ages 30-65), paying out-of-pocket until deductible is met. Psychographically: frustrated by insurance complexity, willing to shop around, motivated by concrete savings.
- **Tertiary**: Seniors on Medicare with coverage gaps (Part D "donut hole"), managing 3+ medications.

## Revenue Model
- **Free tier**: Price comparison across nearby pharmacies, basic coupon display, generic alternative lookup
- **Paid tier**: $3.99/month — patient assistance program finder, therapeutic alternative suggestions with doctor-shareable comparison, refill reminders, pharmacy transfer assistance, annual cost report
- **Premium/Enterprise**: N/A for consumers; explore pharmacy affiliate commissions ($1-3 per transferred prescription) as supplementary revenue
- **Projected conversion rate**: 6% (benchmarked against GoodRx Gold's ~4% conversion; patient assistance program finder is a strong differentiator for the uninsured)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $180 |
| Drug pricing APIs (RxNav, Pharmacy APIs) | $500 |
| AI alternative suggestions (OpenAI API) | $200 |
| Marketing (community + content) | $1,200 |
| App store fees (15-30%) | $150 |
| Total Monthly Burn | $2,230 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $14 |
| LTV | $115 (avg 29-month retention at $4/mo; medication needs are ongoing) |
| LTV:CAC | 8.2:1 |
| Payback Period | 3.5 months |
| Gross Margin | 79% |

## Go-to-Market: First 100 Users
- **Reddit**: r/HealthInsurance (85K), r/uninsured (5K), r/povertyfinance (1.7M), r/personalfinance (17M), r/pharmacy (115K) — post specific drug savings examples ("I saved $340 on my Lipitor by switching pharmacies")
- **Community health centers**: Partner with 20 FQHCs (Federally Qualified Health Centers) that serve uninsured patients; free printed flyers in waiting rooms
- **TikTok/Instagram**: "Pharmacy price check" comparison videos showing the same drug at $15 vs. $450 — outrage content drives shares
- **Free clinic partnerships**: Social workers at free clinics constantly advise patients on medication costs; provide them free premium accounts
- **Spanish-language content**: 30% of uninsured Americans are Hispanic; translate core content and target Spanish-language social media

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 21,000 free / 1,250 paid | $60K | Organic + community health center partnerships; 6% conversion |
| 2 | 70,000 free / 5,500 paid | $264K | Pharmacy affiliate revenue adds $40K; viral social content; bilingual launch |
| 3 | 200,000 free / 12,500 paid | $600K | + $150K affiliate revenue; patient assistance program database becomes a moat |
| 4 | 400,000 free / 25,000 paid | $1.2M | + $300K affiliate; insurance company partnerships for member cost reduction |
| 5 | 800,000 free / 45,000 paid | $2.2M | + $600K affiliate; pharmacy chain partnerships; employer benefits integration |

## Key Weekly Metrics
1. **Price searches completed** — core usage indicator; target 5,000+/week by month 6
2. **Average savings displayed per search** — validates value proposition; target $50+
3. **Patient assistance program applications initiated** — differentiator metric
4. **Pharmacy transfers completed** — measures real-world action taken
5. **Free-to-paid conversion rate** — target 6%+
6. **Drug database coverage** — % of searched drugs with complete pricing data
7. **User-reported savings** — track self-reported dollar amounts saved for marketing

## Top 3 Risks
1. **GoodRx dominance makes user acquisition expensive** → Differentiate on patient assistance programs (GoodRx doesn't cover these), therapeutic alternatives, and the uninsured/underinsured niche; avoid competing on coupon breadth where GoodRx has network effects
2. **Drug pricing data is difficult to aggregate and keep current** → Use a combination of public APIs (RxNav, OpenFDA), pharmacy partnerships, and user-reported prices; start with top 200 most-prescribed drugs covering 80% of searches
3. **Regulatory scrutiny of drug price comparison tools** → Consult healthcare compliance attorney; ensure no kickback violations (Anti-Kickback Statute); transparent disclosure of affiliate relationships; comply with pharmacy advertising regulations in each state
