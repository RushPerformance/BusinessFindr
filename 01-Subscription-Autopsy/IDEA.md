# Subscription Autopsy

> Automatically finds, categorizes, and cancels unwanted subscriptions by scanning bank/email data — then monitors for zombie charges.

| Field | Detail |
|-------|--------|
| Category | Finance |
| Target Audience | Mass Market (anyone with a bank account and email) |
| Monetization | Freemium — free scan, $4.99/mo for monitoring + auto-cancel |
| Recession Resistance | High — demand increases in downturns as consumers cut discretionary spending |
| Solo-Dev MVP Timeline | 6 weeks |
| Composite Score | 92/100 |

## The Problem
The average American has 12 recurring subscriptions and unknowingly pays for 3-4 they don't use, wasting ~$133/month ($1,600/year) per household. 42% of consumers have forgotten about at least one active subscription (C+R Research, 2022). Subscription creep accelerates during recessions as people sign up for free trials and forget to cancel. The "dark pattern" cancellation flows used by companies like NYT, Planet Fitness, and Adobe make manual cancellation time-consuming and frustrating.

## The Solution
Users connect their bank account via Plaid or forward receipt emails. The app:
1. Scans transactions for recurring charges
2. Categorizes each subscription (entertainment, fitness, news, software, etc.)
3. Shows total monthly/yearly spend with a "waste score"
4. One-tap cancellation via automated email/chat/call bots
5. Monitors for zombie charges (charges that continue after cancellation)
6. Sends weekly spend alerts

## Market Size
- **TAM**: $2.1B — US subscription management tools market (Grand View Research, 2023)
- **SAM**: $840M — consumers actively seeking subscription tracking/cancellation
- **SOM**: $4.2M — capturing 0.5% of SAM in Year 1 with organic/viral growth

## Existing Alternatives
- **Rocket Money (Truebill)**: $3-12/mo, acquired by Rocket Companies. Full-featured but expensive and takes a % of savings
- **Trim**: Shut down in 2023
- **Bobby/Subdly**: Manual entry only, no bank connection
- **Spreadsheets**: Common but tedious, no auto-detection

## Why This Wins
- Zombie charge monitoring is a unique, underserved feature — no competitor does it well
- Flat fee vs. Rocket Money's percentage-of-savings model (which feels punitive)
- Email scanning catches subscriptions banks miss (annual charges, PayPal, crypto)
- Vertical focus: subscription management only, not a full finance app

## Revenue Potential
- **Year 1**: $180K (3,000 paid users × $5/mo)
- **Year 3**: $1.8M (30,000 paid users × $5/mo) with viral "I saved $X" sharing mechanic
