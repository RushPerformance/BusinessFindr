# Podcast Listening Stats

**One-Line Pitch:** Cross-platform podcast listening analytics showing your total time spent, favorite genres, completion rates, and personalized recommendations — your Spotify Wrapped, but for all your podcasts year-round.

| Field | Details |
|---|---|
| **Category** | Social / Education |
| **Target Audience** | Avid podcast listeners (3+ hours/week), podcast enthusiasts, and content curators |
| **Monetization** | $2.99/mo subscription |
| **Recession Resistance** | Low-Medium |
| **Solo-Dev MVP Timeline** | 8-10 weeks |
| **Composite Score** | 35/100 |

---

## Problem

There are 100 million monthly podcast listeners in the US, with the average listener consuming 8 podcasts per week and spending 7 hours weekly listening. Yet unlike music (Spotify Wrapped), reading (Goodreads), or TV (Trakt), there is no way for podcast listeners to see their own listening data across platforms. Apple Podcasts shows a basic "Recently Played" list. Spotify wraps podcast data into its annual Wrapped feature but only for Spotify-exclusive listening. Overcast, Pocket Casts, and other apps show minimal stats if any. The result is that the average avid podcast listener spends 365 hours per year listening and has no way to reflect on that time — which shows are most valued, which are abandoned after 2 episodes, and whether listening habits are expanding or narrowing. This lack of data also means podcast recommendations remain primitive: algorithms suggest based on genre tags, not on actual completion patterns and listening behavior.

---

## Solution

1. **Cross-Platform Import** — Connects to Apple Podcasts, Spotify, Overcast, Pocket Casts, and Castro via OPML import and API integration to aggregate listening history.
2. **Listening Dashboard** — Total hours listened, episodes completed, unique shows, and daily/weekly/monthly listening trends with beautiful visualizations.
3. **Completion Rate Analysis** — Shows which podcasts you finish (high engagement) vs. abandon (low engagement), helping you curate your subscription list.
4. **Genre Breakdown** — Categorizes listening time by genre (true crime, business, comedy, news, tech) with pie charts and trend lines over time.
5. **Discovery Score** — Tracks how many new shows you try each month vs. sticking with familiar ones, encouraging exploration.
6. **Shareable Year-in-Review** — Generate Spotify Wrapped-style annual and monthly listening summaries designed for sharing on social media.
7. **Smart Recommendations** — Based on completion patterns (not just genre), suggest new podcasts that match your actual listening behavior.
8. **Listening Goals** — Set and track goals for listening diversity, new show exploration, or total hours.

---

## Market Size

- **TAM (Total Addressable Market):** $4B — the US podcast industry including advertising, subscriptions, and tools.
- **SAM (Serviceable Addressable Market):** $400M — the segment of avid podcast listeners willing to pay for analytics and recommendation tools.
- **SOM (Serviceable Obtainable Market):** $2.2M — capturing 60,000 subscribers at $2.99/mo within 3 years.

---

## Existing Alternatives

1. **Spotify Wrapped** — Annual snapshot but only covers Spotify listening, is not available year-round, and provides limited actionable data.
2. **Apple Podcasts Stats** — Shows recently played and a basic listening history but no analytics, no completion rates, and no cross-platform data.
3. **Goodpods** — Social podcast platform with ratings and reviews but no personal listening analytics or cross-platform aggregation.
4. **Podchaser** — Podcast database and discovery platform but focused on industry data (ratings, credits), not personal listening analytics.
5. **Pocket Casts** — Offers basic listening stats (total time) but only within its own app, with no genre analysis or completion tracking.

---

## Why This Wins

- **Social sharing drives virality** — shareable listening stats (like Spotify Wrapped) are proven viral content; monthly and annual summaries generate organic growth.
- **Data portability gap** — no podcast app shares listening data with other apps; a cross-platform aggregator fills a genuine platform fragmentation problem.
- **Podcast enthusiast identity** — avid listeners are proud of their podcast consumption and want to quantify and share it, similar to readers with Goodreads.
- **Recommendation quality** — completion-rate-based recommendations are significantly better than genre-tag-based suggestions, creating genuine user value.
- **Low development complexity** — OPML is a standard format, and most listening data can be imported without complex API integrations for the MVP.

---

## Revenue Potential

- **Year 1:** $72K ARR — 2,000 subscribers at $2.99/mo acquired through podcast community marketing, Twitter/X podcast discussions, and podcast newsletter sponsorships.
- **Year 3:** $540K ARR — 15,000 subscribers plus data insights sold (anonymized, aggregated) to podcast networks and advertising platforms seeking listener behavior data.
