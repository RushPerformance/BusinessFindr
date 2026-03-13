# Business Model: Secondhand Price Checker

## Value Proposition
Resellers and declutterers instantly know what any item is worth across all major platforms -- eliminating the 15-minute manual research process per item and ensuring they never underprice a find or overpay at a thrift store.

## Customer Segments
- **Primary**: Casual resellers aged 25-45 who sell 5-50 items/month on eBay, Poshmark, Mercari, or Facebook Marketplace. Income $30K-$80K, often supplementing primary income. Psychographically entrepreneurial, deal-hunting, frustrated by the time spent researching prices across multiple platforms.
- **Secondary**: Thrift store shoppers and garage sale flippers aged 20-55 who need instant price checks to make buy/don't-buy decisions on the spot. Time-pressured and volume-driven.
- **Tertiary**: Declutterers and Marie Kondo-inspired minimalists aged 25-50 who want to sell rather than donate items but don't know what anything is worth. Lower frequency, higher per-item uncertainty.

## Revenue Model
- **Free tier**: 5 price lookups per month, barcode scan only, single-platform pricing (eBay sold), basic condition pricing
- **Paid tier**: $2.99/month -- Unlimited lookups, barcode + photo search, cross-platform pricing (eBay, Poshmark, Mercari, Facebook Marketplace, Depop), sold vs. listed prices, condition-based pricing, best platform recommendation
- **Premium/Enterprise**: $7.99/month -- Everything in paid, plus listing optimizer (title, description, price), profit calculator with fee deduction, inventory tracker with cost basis, bulk scan mode, CSV export for tax reporting
- **Projected conversion rate**: 10% (benchmarked against WorthPoint's conversion rate for reseller tools; strong because free tier is deliberately limited and power users need unlimited lookups)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS) | $100 |
| Marketplace APIs and scraping (eBay, Poshmark, Mercari) | $350 |
| AI image recognition (for photo search) | $200 |
| Data storage (pricing history, user inventories) | $60 |
| Marketing | $400 |
| Total Monthly Burn | $1,110 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $7 |
| LTV | $54 (avg 10-month retention at $2.99/mo; 20% upgrade to $7.99 premium) |
| LTV:CAC | 7.7:1 |
| Payback Period | 2.3 months |
| Gross Margin | 72% |

## Go-to-Market: First 100 Users
- **Reddit**: Post finds and flips in r/Flipping (200K), r/ThriftStoreHauls (3M), r/poshmark (90K), r/Mercari (65K), r/eBay (115K), r/Frugal (2.3M). Content like "I scanned a $3 thrift store find and it was worth $85 on eBay" performs extremely well.
- **YouTube reseller community**: Sponsor or collaborate with reseller YouTubers (Hairy Tornado, Ralli Roots, Daily Refinement) who have audiences of 50K-500K actively looking for pricing tools.
- **TikTok thrift content**: Create "scan and reveal" content showing surprise valuations at thrift stores -- this format is extremely engaging and shareable.
- **Facebook reseller groups**: Hundreds of groups like "eBay Sellers" (150K+), "Poshmark Sellers" (100K+) where pricing is the #1 discussion topic.
- **Thrift store partnerships**: Place QR code stickers or flyers near registers at local thrift chains (Goodwill, Salvation Army, Savers).

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 720 paid | $26K | Organic growth from reseller communities; proving cross-platform data accuracy |
| 2 | 3,500 paid | $151K | YouTube/TikTok content gains traction; premium tier launched with inventory tracking |
| 3 | 7,200 paid | $259K + $50K affiliate = $309K | Affiliate revenue from marketplace sign-up referrals; accuracy improvements with user data |
| 4 | 15,000 paid | $540K + $120K affiliate = $660K | Brand recognition as the "Kelley Blue Book of secondhand"; B2B pricing API for resale shops |
| 5 | 25,000 paid | $900K + $200K affiliate + $100K API = $1.2M | Category leader; API licensing to consignment stores and estate sale companies; international expansion |

## Key Weekly Metrics
1. Price lookups performed (core usage)
2. Barcode scans vs. photo searches (feature mix)
3. Free-to-paid conversion rate
4. Premium tier upgrade rate
5. Cross-platform price accuracy (user-reported corrections)
6. Inventory items tracked (premium engagement depth)
7. DAU/MAU ratio (stickiness for regular resellers)

## Top 3 Risks
1. **Marketplace API access is restricted or expensive** -- eBay, Poshmark, and Mercari may limit API access or charge prohibitive fees; some may require scraping which violates TOS. Mitigation: eBay has a robust API program; for others, use a combination of official APIs where available and user-contributed data; build proprietary pricing database over time from user scans.
2. **Photo-based pricing accuracy is inconsistent** -- AI image recognition for unboxed, vintage, or clothing items has lower accuracy than barcode scans. Mitigation: Use photo search as a "best guess" with confidence scores; allow users to refine results by selecting from suggested matches; improve model with user feedback on accuracy.
3. **WorthPoint or eBay builds a cross-platform tool** -- WorthPoint has the data and eBay has the traffic to dominate this space. Mitigation: WorthPoint is expensive ($25/month) and focused on antiques; eBay is unlikely to promote competitor platforms' pricing; our mobile-first, instant-scan UX is differentiated from desktop research tools.
