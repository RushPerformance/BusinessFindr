# Restaurant Health Score Lookup

**One-Line Pitch:** Aggregates health inspection scores for restaurants with violation details, trend data, and alerts for repeat offenders — so you can check before you eat, not after you get sick.

| Field | Details |
|---|---|
| **Category** | Food / Health |
| **Target Audience** | Health-conscious diners, food bloggers, parents with young children, travelers |
| **Monetization** | Free tier + $1.99/mo premium |
| **Recession Resistance** | Medium |
| **Solo-Dev MVP Timeline** | 10-12 weeks |
| **Composite Score** | 36/100 |

---

## Problem

The CDC estimates that 48 million Americans get foodborne illness each year, resulting in 128,000 hospitalizations and 3,000 deaths. Every county health department in the US conducts restaurant inspections, but the results are scattered across thousands of different county websites with inconsistent formats, scoring systems, and update frequencies. A 2022 study in the American Journal of Public Health found that restaurants with critical violations are 2.3x more likely to cause foodborne illness outbreaks, yet consumers rarely check inspection scores before dining. Los Angeles County found that when inspection grades were posted prominently (A/B/C letter grades), hospitalizations for foodborne illness dropped 13.1%. The data exists and is public — it is just inaccessible. The average consumer would need to visit their specific county health department website, navigate an often-outdated search tool, and interpret violation codes to make sense of a restaurant's safety history.

---

## Solution

1. **Nationwide Inspection Database** — Aggregates health inspection data from county health departments across major US metros, normalized into a consistent scoring format.
2. **Restaurant Safety Score** — Converts raw inspection data into a simple A-F letter grade with a numerical score (0-100) for quick comparison.
3. **Violation Details** — Lists specific violations found during inspections with plain-English explanations (e.g., "improper food storage temperature" instead of "violation code 7-201.11").
4. **Trend Analysis** — Shows inspection score trends over the last 3-5 inspections, highlighting restaurants that are improving or declining.
5. **Repeat Offender Alerts** — Flags restaurants with recurring critical violations (rodent activity, temperature abuse, handwashing failures) that indicate systemic problems.
6. **Map-Based Search** — Find restaurant inspection scores near your current location or a planned destination with filter options for score minimums.
7. **Favorites and Watchlist** — Save frequently visited restaurants and receive alerts when new inspection results are posted.
8. **Integration with Review Platforms** — Browser extension that overlays health scores on Yelp, Google Maps, and DoorDash listings.

---

## Market Size

- **TAM (Total Addressable Market):** $899B — the US restaurant industry total revenue.
- **SAM (Serviceable Addressable Market):** $4.5B — the restaurant information and review market where health data adds value.
- **SOM (Serviceable Obtainable Market):** $3.6M — capturing 150,000 premium subscribers at $1.99/mo within 3 years, plus advertising revenue.

---

## Existing Alternatives

1. **County Health Department Websites** — The primary source but fragmented across thousands of jurisdictions with poor UX and inconsistent data formats.
2. **Yelp Health Score Badges** — Shows scores in some cities but coverage is inconsistent, historical data is absent, and violation details are not included.
3. **Hazel Analytics** — Aggregates health inspection data but sells exclusively to enterprise clients (restaurant chains, real estate investors), not consumers.
4. **Iwaspoisoned.com** — Crowdsourced food poisoning reports but relies on self-reporting, has no official inspection data, and covers only a fraction of incidents.
5. **Google Maps** — Occasionally displays health scores in select markets but coverage is limited and there is no trend data or violation detail.

---

## Why This Wins

- **Public data, private value** — the data is free and public; the value is in aggregation, normalization, and presentation in a consumer-friendly format.
- **Trust and transparency trend** — consumers increasingly demand transparency about the businesses they patronize, especially regarding health and safety.
- **Viral potential** — "This popular restaurant just got an F on their health inspection" is inherently shareable content that drives organic growth.
- **Advertising model scalability** — restaurants with good scores will pay to promote their grades; food delivery platforms will pay for integration.
- **Parent market segment** — parents of young children are especially motivated to check restaurant safety and have strong word-of-mouth networks.

---

## Revenue Potential

- **Year 1:** $90K revenue — 30,000 free users with 3,000 premium subscribers at $1.99/mo, plus $36K in restaurant advertising revenue.
- **Year 3:** $720K revenue — 50,000 premium subscribers plus advertising from restaurants promoting good scores and food delivery platform API licensing fees.
