# Energy Usage Disaggregator

> Uses smart meter data (no hardware) to break down electricity usage by appliance and identify energy hogs draining your wallet.

| Field | Detail |
|-------|--------|
| Category | Sustainability / Home |
| Target Audience | Mass Market — homeowners and renters with smart meters |
| Monetization | Subscription — $4.99/mo |
| Recession Resistance | Medium-High — energy costs are non-discretionary; savings motivation increases during downturns |
| Solo-Dev MVP Timeline | 7 weeks |
| Composite Score | 47/100 |

## The Problem
The average US household spends $2,000/year on electricity, but most people have no idea where that money goes. Utility bills show total usage, not which appliances are responsible. That old refrigerator might be costing $30/month; the space heater in the spare room might be $50/month. Without appliance-level data, households can't make informed decisions about what to replace, unplug, or use differently. Smart home energy monitors (Sense, Emporia) require hardware installation ($200-400) and electrical panel access — eliminating renters and non-technical homeowners.

## The Solution
1. Smart meter data connection: link your utility account (Green Button data, utility API, or manual upload)
2. AI disaggregation: machine learning breaks total usage into estimated appliance-level consumption
3. Energy hog identification: "Your top 3 energy consumers are: HVAC (42%), water heater (18%), old refrigerator (11%)"
4. Cost-per-appliance estimates: see monthly cost attributed to each major appliance
5. Savings recommendations: "Replacing your 15-year-old fridge would save $22/month — payback in 2.4 years"
6. Usage anomaly alerts: "Your energy usage spiked 40% this week — possible causes: space heater, HVAC malfunction"
7. Neighbor comparison: see how your usage compares to similar homes in your area
8. Seasonal analysis: understand how heating/cooling drives your bill throughout the year

## Market Size
- **TAM**: $3.5B — US home energy management market
- **SAM**: $700M — energy monitoring and optimization tools
- **SOM**: $600K — 10,000 paid users × $5/mo

## Existing Alternatives
- **Sense**: $299 hardware monitor + app, requires electrical panel installation
- **Emporia**: $150 hardware monitor, DIY installation
- **Utility company apps**: Show total usage, no appliance breakdown
- **Smappee**: $300+ hardware, European-focused
- **Kill-A-Watt**: $30 plug-in meter, measures one outlet at a time (tedious)
- **Energy Star calculators**: Generic estimates, not personalized to your home

## Why This Wins
- No hardware required is the critical differentiator — software-only approach using existing smart meter data
- Works for renters (can't install hardware in someone else's electrical panel)
- Cost-per-appliance framing makes abstract energy data personally relevant
- ROI calculations for appliance upgrades drive real purchasing decisions
- Utility company partnerships could provide distribution channel (utilities benefit from demand management)

## Revenue Potential
- **Year 1**: $36K (600 paid users × $5/mo)
- **Year 3**: $360K (6,000 paid users × $5/mo) + potential utility partnerships
