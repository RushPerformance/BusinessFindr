# Business Model: Immigrant Document Tracker

## Value Proposition
Never miss an immigration deadline again — get personalized alerts for visa renewals, filing windows, and policy changes that could cost you your status, while tracking every document and case milestone in one secure place, replacing the anxiety of managing a life-altering process with spreadsheets.

## Customer Segments
- **Primary**: Employment-based visa holders (H-1B, L-1, O-1) ages 25-45, predominantly in tech, healthcare, and finance. Household income $60K-$200K. Psychographically: highly educated, detail-oriented, anxious about status maintenance, willing to pay for peace of mind on something that determines their ability to live and work in the US.
- **Secondary**: Family-based green card applicants (ages 25-55) navigating the multi-year sponsorship process. Psychographically: patient but frustrated, often managing the process without an attorney, motivated by family reunification.
- **Tertiary**: DACA recipients, TPS holders, and asylum seekers with complex, evolving status requirements.

## Revenue Model
- **Free tier**: Basic visa type lookup, general requirement overview, single deadline reminder
- **Paid tier**: $7.99/month — full document checklist with completion tracking, unlimited deadline alerts, case status auto-tracker (USCIS integration), processing time estimator, policy change alerts, document vault
- **Premium/Enterprise**: $14.99/month — travel advisory, green card milestone tracker, attorney collaboration features, priority policy change alerts, family plan (spouse + dependents)
- **Projected conversion rate**: 12% (benchmarked against Lawfully's estimated 8-12% conversion; higher due to extreme consequence of missing deadlines)

## Cost Structure (Monthly)
| Cost | Estimate |
|------|----------|
| Hosting (AWS + encrypted storage) | $200 |
| USCIS case status API/scraping | $250 |
| Policy monitoring service | $300 |
| Marketing (community + SEO) | $1,400 |
| App store fees (15-30%) | $300 |
| Total Monthly Burn | $2,450 |

## Unit Economics
| Metric | Value |
|--------|-------|
| CAC | $20 |
| LTV | $288 (avg 36-month retention at $8/mo; immigration processes span years) |
| LTV:CAC | 14.4:1 |
| Payback Period | 2.5 months |
| Gross Margin | 81% |

## Go-to-Market: First 100 Users
- **Reddit**: r/immigration (150K), r/h1b (12K), r/USCIS (22K), r/greencard (8K), r/DACA (18K) — answer questions with genuine expertise and mention the tool
- **Blind (anonymous professional network)**: H-1B immigration is a dominant topic; create informational posts about deadline tracking
- **WeChat/WhatsApp groups**: Large immigrant communities share information through private messaging groups; target Indian and Chinese professional communities (largest H-1B populations)
- **Immigration attorney partnerships**: Offer free premium to 30 immigration attorneys who recommend it to DIY clients they can't serve affordably
- **Content SEO**: Target "H-1B renewal deadline," "green card processing time," "USCIS case status tracker," "immigration policy changes 2026" — high-intent, high-anxiety queries

## 5-Year Revenue Projection
| Year | Users | Revenue | Assumptions |
|------|-------|---------|-------------|
| 1 | 8,500 free / 1,000 paid | $96K | Organic + community growth; 12% conversion; high retention from day 1 |
| 2 | 30,000 free / 4,500 paid | $432K | Word-of-mouth in professional immigrant networks; premium tier launches |
| 3 | 80,000 free / 8,000 paid | $768K | Attorney collaboration features drive B2B; multilingual support (Spanish, Mandarin, Hindi) |
| 4 | 150,000 free / 15,000 paid | $1.4M | Immigration law firm partnerships; employer sponsorship tracking for HR departments |
| 5 | 280,000 free / 28,000 paid | $2.7M | Dominant immigration self-service platform; expansion to Canada/UK/Australia immigration |

## Key Weekly Metrics
1. **Deadline alerts sent** — core product function; tracks how many critical reminders users receive
2. **USCIS case status check frequency** — measures anxiety-driven engagement; target daily checks
3. **Policy change alert open rate** — target 80%+; these are must-read notifications
4. **Document vault upload rate** — measures depth of adoption; target 10+ documents per user
5. **Free-to-paid conversion rate** — target 12%+
6. **Retention rate (monthly)** — target 97%+ (immigration is a multi-year journey; churn should be near zero)
7. **NPS by visa category** — ensures value delivery across all immigrant segments, not just H-1B

## Top 3 Risks
1. **Immigration law complexity creates accuracy liability** → Prominent disclaimer that the app provides information, not legal advice; partner with immigration attorneys for quarterly content audits; user feedback loop for inaccuracies; focus on deadlines and procedures (objective facts) rather than legal strategy (subjective advice)
2. **USCIS case status scraping breaks or gets blocked** → Build redundancy with multiple data sources; negotiate official API access if USCIS opens one; provide manual status update option; alert users when automated tracking is disrupted
3. **Political changes dramatically alter immigration rules** → Policy change alerts are actually strengthened by volatility (more changes = more value); maintain rapid response capability to update the app within 48 hours of major policy announcements; this risk is actually a growth driver
