# Roof Age Estimator

**One-Line Pitch:** Uses satellite imagery and public records to estimate roof age and remaining lifespan for homebuyers, real estate agents, and insurance underwriters — answering the most expensive unknown in home purchases.

| Field | Details |
|---|---|
| **Category** | Home & Property |
| **Target Audience** | Homebuyers, real estate agents, home inspectors, and insurance adjusters |
| **Monetization** | $9.99 per report |
| **Recession Resistance** | Medium |
| **Solo-Dev MVP Timeline** | 12-14 weeks |
| **Composite Score** | 38/100 |

---

## Problem

Roof replacement is the single most expensive maintenance item for homeowners, averaging $8,000-$15,000 for a standard asphalt shingle roof and up to $30,000+ for specialty materials. Yet when buying a home, roof age is often unknown or misrepresented — a 2023 National Association of Realtors survey found that 35% of homebuyers received inaccurate or no information about roof age before closing. Insurance companies are increasingly refusing to write or renew policies on roofs older than 15 years, with State Farm, Allstate, and others implementing strict roof age cutoffs in many states. The average home inspection provides only a visual assessment from ground level and costs $300-$500 with a separate $200-$400 charge for a dedicated roof inspection. Meanwhile, building permit records (which would document re-roofing) are scattered across 19,000+ local jurisdictions with no centralized database.

---

## Solution

1. **Satellite Image Analysis** — Processes current and historical satellite/aerial imagery to detect shingle wear patterns, color fading, moss growth, and visible damage that correlate with roof age.
2. **Permit Record Search** — Searches local building department records for roofing permits filed at the address, establishing documented replacement dates.
3. **Age Estimation Algorithm** — Combines imagery analysis, permit data, home construction date, and regional weather patterns to estimate roof age within a 2-3 year accuracy window.
4. **Remaining Lifespan Projection** — Based on estimated age and material type (asphalt, tile, metal, slate), projects remaining useful life and estimated replacement cost.
5. **Insurance Compatibility Check** — Flags whether the estimated roof age may trigger policy non-renewal or premium increases with major insurers active in that state.
6. **Comparable Roof Report** — Shows roof ages and recent replacements for neighboring homes, providing context for the local area.
7. **Pre-Purchase Negotiation Data** — Generates a clean report suitable for attaching to purchase offers, supporting price reduction requests based on roof condition.

---

## Market Size

- **TAM (Total Addressable Market):** $54B — the US roofing market including replacement, repair, and new construction.
- **SAM (Serviceable Addressable Market):** $3.2B — the intersection of real estate transactions (5.3M home sales/year) and roof-related due diligence.
- **SOM (Serviceable Obtainable Market):** $5M — selling 500,000 reports at $9.99 within 3 years to homebuyers, agents, and insurers.

---

## Existing Alternatives

1. **Professional Roof Inspections** — Accurate but cost $200-$400, require scheduling, and take 3-5 business days for a report.
2. **Betterview** — Enterprise satellite roof analysis platform but sold only to insurance carriers, not available to consumers or agents.
3. **EagleView** — Provides aerial roof measurements for contractors but focuses on dimensions, not age estimation or condition assessment.
4. **Home Inspection Reports** — General home inspectors assess roofs visually from the ground but cannot determine age and often use vague language like "appears to be in serviceable condition."
5. **Zillow/Redfin Listing Data** — Occasionally mentions roof age in listing descriptions but relies on seller self-reporting with no verification.

---

## Why This Wins

- **Instant answers vs. multi-day inspections** — a report generated in minutes replaces a $200-$400 professional inspection for initial screening purposes.
- **Insurance market urgency** — as more insurers enforce roof age cutoffs, demand for age verification is growing rapidly among both homeowners and agents.
- **Real estate agent distribution** — agents will recommend and even bulk-purchase reports as a value-add service for their buyer clients.
- **Scalable via satellite data** — unlike physical inspections, satellite-based analysis can cover any address in the country without sending anyone to the property.

---

## Revenue Potential

- **Year 1:** $150K revenue — 15,000 reports at $9.99 each, sold primarily to homebuyers and real estate agents through Zillow/Realtor.com advertising.
- **Year 3:** $1.5M revenue — 150,000 reports annually plus B2B bulk pricing for insurance carriers ($5/report at volume) and real estate brokerages.
