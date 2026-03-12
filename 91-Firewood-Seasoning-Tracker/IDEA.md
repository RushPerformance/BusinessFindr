# Firewood Seasoning Tracker

> Tracks firewood drying time by species, split date, and storage conditions with "ready to burn" alerts.

| Field | Detail |
|-------|--------|
| Category | Home |
| Target Audience | Niche — homeowners who heat with wood or use fireplaces |
| Monetization | One-time purchase — $1.99 |
| Recession Resistance | Medium-High — wood heating increases during recessions as people seek cheaper alternatives to oil and gas |
| Solo-Dev MVP Timeline | 3 weeks |
| Composite Score | 7/100 |

## The Problem
Approximately 12.5 million US households burn wood for heating or ambiance (US Census Bureau), and the $5.2B heating fuel market includes a significant firewood segment. Burning unseasoned (wet) wood is the single biggest mistake wood burners make — it produces 60% less heat, creates dangerous creosote buildup (the #1 cause of chimney fires — 25,000 per year per NFPA), and generates excessive smoke. Different wood species require different seasoning times: oak needs 12-24 months, pine needs 6-12 months, birch needs 12 months. Most people guess whether their wood is ready, and they guess wrong. Moisture meters ($20-40) help but require individual log testing and don't track batches over time.

## The Solution
1. Batch logging: record when wood was split with species, quantity (cords/face cords), and split date
2. Species-specific drying database: expected seasoning time for 30+ common firewood species
3. Storage condition factors: covered vs. uncovered, stacked vs. piled, sun exposure, and airflow rating
4. "Ready to burn" alerts based on species, split date, and storage conditions
5. Moisture content estimator: predicted moisture level based on elapsed time and conditions
6. Burn order recommendations: which batch to burn first based on readiness
7. Annual wood supply planner: calculate how many cords you need per season and when to start splitting

## Market Size
- **TAM**: $5.2B — US heating fuel market (wood segment)
- **SAM**: $52M — firewood management and wood heating tools
- **SOM**: $20K — 10,000 one-time purchases x $1.99

## Existing Alternatives
- **Moisture meters**: Hardware tool ($20-40) that tests individual logs but doesn't track batches or predict readiness
- **Firewood forums / Reddit**: Community advice on seasoning times but generic and not batch-specific
- **Memory / notebooks**: The most common approach — "I think I split that oak in March 2024?"
- **General note-taking apps**: Can record dates but have no species database or readiness calculations
- **Firewood supplier advice**: Often unreliable — suppliers may sell "seasoned" wood that's still wet

## Why This Wins
- Species-specific drying times are the key insight — a simple app solving a non-obvious problem
- "Ready to burn" alerts automate what wood burners currently guess at (often incorrectly)
- Preventing chimney fires is a safety argument that justifies a $1.99 purchase immediately
- Extremely simple to build — small database, basic date math, push notifications
- Passionate niche audience (wood burners love talking about wood) creates organic word-of-mouth

## Revenue Potential
- **Year 1**: $10K (5,000 one-time purchases x $1.99)
- **Year 3**: $50K (25,000 cumulative purchases x $1.99) — limited by one-time pricing but very low support costs
