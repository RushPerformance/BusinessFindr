# Business Model: Receipt Tax Sorter

## Value Proposition
Save $500-1,000 in missed tax deductions annually by automatically categorizing every receipt to IRS-ready Schedule line items — eliminating the 5-15 hours of pre-tax-season sorting and ensuring no legitimate deduction is left on the table.

## Customer Segments
- **Primary**: Self-employed individuals and freelancers (ages 25-55), filing Schedule C, digitally comfortable but not accounting-savvy, earning $40K-$150K. Psychographically: anxious about audits, resentful of time spent on paperwork, motivated by saving money.
- **Secondary**: Itemizing taxpayers with significant medical or charitable expenses (ages 40-70), often homeowners. Psychographically: detail-oriented, value organization, willing to pay for peace of mind.
- **Tertiary**: Landlords filing Schedule E with 1-5 rental properties, tracking repair/maintenance receipts.

## Revenue Model
- **Free tier**: 15 receipt scans per month, basic categorization, no export
- **Paid tier**: $5.99/month ($49.99/year) — unlimited scans, AI categorization, IRS-ready PDF export, deduction tracker, 7-year receipt storage, mileage log
- **Premium/Enterprise**: $14.99/month — multi-user (married filing jointly or CPA collaboration), priority OCR, API export to TurboTax/QuickBooks, audit support documentation
- **Projected conversion rate**: 8% (benchmarked against Evernote's 5-8% freemium conversion, higher due to clear financial ROI)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS S3 + EC2) | $250 |
| OCR API (Google Vision / AWS Textract) | $400 |
| AI categorization (OpenAI API) | $300 |
| Marketing (SEO + seasonal ads) | $1,500 |
| App store fees (15-30%) | $350 |
| Total Monthly Burn | $2,800 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $18 |
| LTV | $144 (avg 24-month retention at $6/mo) |
| LTV:CAC | 8:1 |
| Payback Period | 3 months |
| Gross Margin | 78% |

## Go-to-Market: First 100 Users
- **Reddit**: Post value content in r/tax (328K members), r/selfemployed (67K), r/freelance (370K), r/smallbusiness (1.3M) during Q4 when tax anxiety peaks
- **Content SEO**: Target "how to organize receipts for taxes," "IRS deduction categories," "receipt tracking app" — high-intent queries with seasonal spikes
- **TikTok/Instagram Reels**: "I scanned 200 receipts in 10 minutes and found $1,200 in deductions" — visual before/after content
- **CPA partnerships**: Offer free premium access to 20 CPAs who recommend it to clients
- **Product Hunt launch**: Time for early January when New Year tax planning resolutions peak

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 12,000 free / 975 paid | $70K | Organic growth + tax season marketing; 8% conversion |
| 2 | 40,000 free / 4,800 paid | $345K | SEO compounds; CPA referral channel matures; 12% conversion with track record |
| 3 | 100,000 free / 11,700 paid | $840K | Brand recognition; content marketing drives inbound; Premium tier launches |
| 4 | 180,000 free / 20,000 paid | $1.6M | Android + web parity; partnership with tax prep software; churn stabilizes at 4%/mo |
| 5 | 300,000 free / 35,000 paid | $2.8M | B2B CPA tier; international expansion (UK, Canada); AI accuracy becomes a moat |

## Key Weekly Metrics
1. **Receipt scans processed** — leading indicator of engagement and API cost
2. **Free-to-paid conversion rate** — target 8%+, measures value delivery
3. **Weekly active users (WAU)** — healthy floor is 40% of total users
4. **OCR accuracy rate** — target 95%+, directly impacts trust and retention
5. **Churn rate (monthly cohort)** — target below 5% during non-tax-season months
6. **Deduction total tracked** — aggregate dollar value, used in marketing
7. **NPS score** — survey monthly, target 50+

## Top 3 Risks
1. **Seasonal usage cliff (Jan-Apr spike, May-Dec drop)** → Introduce year-round features like mileage tracking, business expense reports, and mid-year deduction estimates to maintain engagement; offer annual billing to lock in revenue
2. **OCR accuracy fails on faded/crumpled receipts** → Implement multi-engine OCR fallback (Google Vision + Textract), manual correction UI, and community-reported accuracy scores to build confidence
3. **Intuit/TurboTax builds similar feature** → Move fast to build a loyal user base and IRS-schedule-level categorization accuracy that generic tools won't match; focus on the self-employed niche where TurboTax's breadth is a weakness
