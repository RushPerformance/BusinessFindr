# Neighborhood Internet Speed Map

**One-Line Pitch:** Crowdsourced internet speed data mapped by address for apartment hunters and homebuyers — because ISP advertised speeds and actual speeds are very different things.

| Field | Details |
|---|---|
| **Category** | Home & Property |
| **Target Audience** | Apartment renters, homebuyers, remote workers choosing where to live |
| **Monetization** | Free tier + $2.99/mo premium |
| **Recession Resistance** | Medium |
| **Solo-Dev MVP Timeline** | 8-10 weeks |
| **Composite Score** | 35/100 |

---

## Problem

The FCC's 2023 Broadband Data Collection found that ISPs overstate coverage and speeds in 42% of census blocks, and a Consumer Reports study revealed that actual download speeds average only 72% of advertised speeds. For the 43 million Americans who moved in 2023, internet quality is now a top-5 factor in choosing where to live — ranked alongside commute time, school districts, and safety. Remote workers, in particular, cannot afford to discover after signing a lease that their new apartment has 15 Mbps when they need 100 Mbps for video calls. Currently, the only way to check real internet speeds at a specific address is to ask current residents or rely on ISP coverage maps, which show availability but not actual performance. Ookla's Speedtest collects billions of data points but does not make address-level data available to consumers. This information gap leads to costly mistakes: breaking a lease ($2,000-$5,000 in penalties) or purchasing expensive supplementary internet (Starlink at $120/mo).

---

## Solution

1. **Address-Level Speed Map** — Interactive map showing real internet speeds (download, upload, latency) reported by actual users at specific addresses and buildings.
2. **Speed Test Integration** — Built-in speed test tool that automatically tags results with the user's address and ISP, growing the database with every test.
3. **ISP Comparison by Address** — Shows which ISPs serve each address with real user-reported speeds vs. advertised speeds for each provider.
4. **Building-Level Reports** — For apartments and condos, aggregate speed data by building showing performance across different units, floors, and ISPs.
5. **Speed History Trends** — Track how internet performance at an address has changed over time, revealing ISP infrastructure investments or degradation.
6. **Remote Work Readiness Score** — Rates each address on its suitability for remote work based on speed, latency, reliability, and ISP competition.
7. **Move Planning Alerts** — Set alerts for an address or neighborhood you are considering, and get notified when new speed data is reported there.
8. **ISP Negotiation Data** — Shows what speeds other customers at your address are getting, giving leverage to negotiate with your ISP for better performance.

---

## Market Size

- **TAM (Total Addressable Market):** $2.8B — the neighborhood and real estate data market (including school ratings, crime data, and demographics).
- **SAM (Serviceable Addressable Market):** $560M — the segment of movers and remote workers willing to pay for address-level internet quality data.
- **SOM (Serviceable Obtainable Market):** $2.7M — capturing 75,000 premium subscribers at $2.99/mo within 3 years.

---

## Existing Alternatives

1. **Ookla Speedtest** — The gold standard for speed testing but does not share address-level data publicly; aggregate data sold only to enterprises.
2. **ISP Coverage Maps** — Show availability and advertised speeds but not actual performance; notoriously inaccurate per FCC findings.
3. **BroadbandNow** — Provides ISP availability by zip code but relies on ISP-reported data rather than user-verified speeds at specific addresses.
4. **FCC Broadband Map** — Shows ISP-reported coverage but not actual speeds; updated infrequently and known for accuracy issues.
5. **Reddit/Nextdoor Anecdotal Reports** — Some residents share internet experience but data is unstructured, unverifiable, and hard to find for specific addresses.

---

## Why This Wins

- **Network effects create a moat** — every speed test adds value to the platform; early movers in data collection become the definitive source.
- **Remote work dependency** — with 35M+ remote workers, internet speed is no longer a convenience but a career necessity, justifying paid data.
- **Real estate integration potential** — apartment listing sites (Zillow, Apartments.com) and real estate agents want this data for their own platforms.
- **ISP partnership revenue** — ISPs performing well in certain areas will pay to highlight their scores; underperforming ISPs will pay for competitive intelligence.
- **Low-cost data acquisition** — users generate the data for free by running speed tests; the platform's cost is storage and visualization, not data collection.

---

## Revenue Potential

- **Year 1:** $72K revenue — 50,000 free users generating data, 2,000 premium subscribers at $2.99/mo, plus $24K in ISP advertising.
- **Year 3:** $540K revenue — 25,000 premium subscribers plus data licensing to apartment listing platforms ($100K/year) and ISP competitive intelligence reports.
