# Electric Vehicle Charging Planner

**One-Line Pitch:** Route planning for EV owners showing charging stations, wait times, and cost estimates along any route.

| Field | Details |
|---|---|
| **Category** | Sustainability / Transportation |
| **Target Audience** | Electric vehicle owners (10M+ in the US), road-trippers, fleet managers |
| **Monetization** | $3.99/mo subscription |
| **Recession Resistance** | Medium |
| **Solo-Dev MVP Timeline** | 10-12 weeks |
| **Composite Score** | 34/100 |

---

## Problem

There are over 10 million registered electric vehicles in the United States as of 2025, yet range anxiety remains the #1 barrier to EV adoption cited by 58% of prospective buyers. The US has roughly 186,000 public charging ports, but availability varies wildly by region — rural stretches of I-70, I-80, and I-10 can have 100+ mile gaps between chargers. EV drivers currently must juggle 5-6 different apps (ChargePoint, Electrify America, Tesla Supercharger, EVgo, Blink, etc.) to plan a single road trip. Real-time wait times are virtually nonexistent, with 23% of drivers reporting they've arrived at a station only to find all chargers occupied or out of service. Pricing structures differ by network (per-kWh, per-minute, per-session), making cost comparison nearly impossible.

---

## Solution

1. **Unified Charging Map** — Aggregates all major charging networks (ChargePoint, Tesla, Electrify America, EVgo, Blink, and 30+ others) into a single searchable map with real-time availability status.
2. **Smart Route Planning** — Calculates optimal charging stops based on your specific vehicle model's range, current battery level, elevation changes, weather, and driving speed.
3. **Wait Time Predictions** — Uses crowdsourced data and historical usage patterns to predict wait times at each station by time of day and day of week.
4. **Cost Estimator** — Normalizes pricing across all networks and estimates total charging cost for your trip, including time-of-use electricity rates.
5. **Offline Route Caching** — Downloads planned routes and nearby charging stations for areas with poor cell coverage.
6. **Station Reviews & Photos** — Community-contributed reviews covering charger condition, amenities (restrooms, food, Wi-Fi), and safety ratings.
7. **Multi-Stop Trip Planner** — Plans complex road trips with multiple destinations, optimizing charging stops around meal breaks and points of interest.
8. **Battery Health Dashboard** — Tracks charging patterns over time and provides recommendations to maximize battery longevity.

---

## Market Size

- **TAM (Total Addressable Market):** $56B global EV charging infrastructure market (projected 2030)
- **SAM (Serviceable Addressable Market):** $8.4B North American EV charging software and services
- **SOM (Serviceable Obtainable Market):** $2.1M — capturing 0.025% of SAM with ~44,000 subscribers at $3.99/mo

---

## Existing Alternatives

1. **A Better Route Planner (ABRP)** — Popular free route planner with good vehicle-specific modeling, but cluttered UI and limited real-time availability data.
2. **PlugShare** — Large community-driven charging station map with reviews, but no route planning and outdated availability info.
3. **ChargePoint / Electrify America apps** — Network-specific apps that only show their own stations, requiring users to juggle multiple apps.
4. **Tesla Navigation** — Excellent for Tesla owners but locked to the Tesla ecosystem and only shows Supercharger/Tesla-compatible stations.
5. **Google Maps EV Mode** — Shows nearby chargers but offers minimal filtering, no wait time data, and limited cost information.

---

## Why This Wins

- **True aggregation** — No other app successfully combines real-time data from ALL major networks with accurate cost comparison in a clean mobile-first interface.
- **Predictive wait times** — Crowdsourced + ML-based wait predictions are a game-changer that no competitor does well, addressing the #1 pain point of arriving at occupied stations.
- **Vehicle-specific accuracy** — Factors in your exact vehicle model, driving habits, cargo load, and weather for range estimates within 5% accuracy.
- **Offline capability** — Essential for the rural corridors where charging stations are sparse AND cell coverage is unreliable.
- **Network-agnostic cost optimization** — Saves drivers 15-30% on charging costs by recommending the cheapest compatible station along their route.

---

## Revenue Potential

- **Year 1:** $180K ARR — ~3,750 subscribers at $3.99/mo, driven by organic search, EV forum partnerships, and social media content targeting road-tripping EV owners.
- **Year 3:** $1.4M ARR — ~29,000 subscribers plus affiliate revenue from charging network partnerships and referral fees, expanding to fleet management features at $19.99/mo per fleet vehicle.
