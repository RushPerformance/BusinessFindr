# Product Requirements Document: Restaurant Waste Tracker

## 1. Executive Summary
US restaurants waste 4-10% of purchased food before it reaches customers, costing the average independent restaurant $25,000-$75,000 per year, yet 70% of restaurants (independents) have no affordable way to measure or reduce waste because enterprise solutions like LeanPath and Winnow cost $500-$2,000/month and require IoT hardware. Restaurant Waste Tracker is a software-only B2B SaaS tool that enables kitchen staff to log waste by category (overproduction, spoilage, prep trim, plate waste) in 30 seconds via a tablet interface, then surfaces cost analytics, category breakdowns, shift-level insights, and AI-powered ordering recommendations that help restaurants cut food costs by 2-8%. At $49/month per location with a projected LTV:CAC of 13.6:1, the tool pays for itself 5-10x over by reducing waste, with a clear path to $1.8M ARR within three years through direct sales, food supplier partnerships, and POS integrations.

## 2. User Personas

### Persona 1: Marco, the Independent Restaurant Owner
- **Age**: 42
- **Job**: Owner-operator of a 60-seat Italian restaurant
- **Income**: $85,000/year (restaurant nets $120K, shared with partner)
- **Pain Points**: Food costs are 34% of revenue (wants to get below 30%); he knows waste is a problem but can't quantify it; his head chef over-preps specials "just in case"; he doesn't have time to implement a complex system; tried a spreadsheet for waste logging and abandoned it after one week
- **Goals**: Know exactly how much money he's losing to waste; get actionable recommendations to reduce food costs; hold his kitchen team accountable without micromanaging
- **Tech Comfort**: Moderate — uses Toast POS and QuickBooks; has a tablet in the kitchen for online orders

### Persona 2: Keisha, the Kitchen Manager
- **Age**: 35
- **Job**: Kitchen manager at a farm-to-table restaurant
- **Income**: $58,000/year
- **Pain Points**: She's responsible for food cost targets but has no tools to identify where waste happens; she suspects the morning prep shift over-produces sauces but can't prove it; the owner asks for waste data she doesn't have; she's too busy during service to log anything
- **Goals**: Quick logging that her line cooks can do at the end of each shift; clear reports she can show the owner; proof that her team is improving
- **Tech Comfort**: Moderate — uses kitchen display systems and POS daily

### Persona 3: Brian, the Multi-Unit Ops Director
- **Age**: 48
- **Job**: Operations director for a 6-location fast-casual chain
- **Income**: $110,000/year
- **Pain Points**: Can't compare waste performance across locations; LeanPath quoted him $3,500/month for 6 locations; inconsistent prep practices between locations; no standardized waste reporting
- **Goals**: Cross-location benchmarking; standardized waste categories; identify which locations need intervention; set waste reduction targets with accountability
- **Tech Comfort**: High — uses restaurant management software and analytics dashboards

## 3. User Stories (20+)
1. As a kitchen staff member, I want to log waste in under 30 seconds by selecting ingredient, category, and estimated weight so that logging doesn't slow down service.
2. As a kitchen manager, I want to see total waste in dollars for today, this week, and this month so that I can quantify the problem.
3. As a restaurant owner, I want to see waste as a percentage of food cost so that I can benchmark against industry standards.
4. As a kitchen manager, I want waste broken down by category (overproduction, spoilage, prep trim, plate waste) so that I know which type of waste to tackle first.
5. As a kitchen manager, I want to see which specific ingredients are wasted most so that I can adjust ordering and prep for those items.
6. As a kitchen manager, I want waste data broken down by shift so that I can identify if morning or evening prep is the bigger problem.
7. As a restaurant owner, I want AI-powered ordering recommendations based on historical waste patterns so that I stop over-ordering.
8. As a kitchen manager, I want par level suggestions based on historical sales and waste data so that I prep the right amount.
9. As a restaurant owner, I want a weekly waste report emailed to me every Monday so that I stay informed without logging in daily.
10. As a kitchen manager, I want to set waste reduction goals and track progress over time so that my team has clear targets.
11. As a kitchen staff member, I want preset ingredient buttons for our most commonly wasted items so that logging is even faster.
12. As a restaurant owner, I want to see the dollar ROI of waste reduction month over month so that I can justify the subscription cost.
13. As a multi-unit operator, I want to compare waste metrics across all my locations on one dashboard so that I can identify underperformers.
14. As a kitchen manager, I want to log waste by station (grill, saute, prep, pantry) so that I can pinpoint which station to focus on.
15. As a restaurant owner, I want to see waste trends over time (daily, weekly, monthly charts) so that I know if we're improving.
16. As a kitchen manager, I want to attach a photo to a waste log entry so that I can document large waste events for investigation.
17. As a restaurant owner, I want to receive an alert when daily waste exceeds a threshold I set so that I can investigate immediately.
18. As a kitchen manager, I want to see recommended prep quantities for tomorrow based on projected sales and waste history so that I reduce overproduction.
19. As a restaurant owner, I want to integrate waste data with my POS system so that I can correlate waste with sales volume automatically.
20. As a multi-unit operator, I want team accountability scores showing which shifts/managers are logging consistently so that I can enforce compliance.
21. As a restaurant owner, I want a menu item profitability view that factors in waste so that I know the true cost of each dish.
22. As a kitchen manager, I want to log waste by reason (dropped, burned, expired, customer return) so that I can differentiate between skill issues and process issues.

## 4. Feature Requirements

### MVP (v1.0) — Must Have
- [ ] Waste logging interface optimized for kitchen tablets: large buttons, ingredient search with autocomplete, category selection (overproduction, spoilage, prep trim, plate waste), estimated weight or count, and dollar cost auto-calculated from ingredient cost database (acceptance: a waste entry can be completed in under 30 seconds; works on 10-inch tablets in landscape orientation; supports greasy-finger touch targets)
- [ ] Ingredient cost database with manual entry and bulk CSV import for a restaurant's top 100 ingredients with unit cost (acceptance: user can add, edit, and delete ingredients; supports lb, oz, kg, each; cost auto-calculates waste dollar value)
- [ ] Cost analytics dashboard showing total waste in dollars (daily, weekly, monthly), waste as a percentage of food cost, and trend line over time (acceptance: data updates in real time; date range selector; comparison to previous period)
- [ ] Category breakdown visualization showing waste by type (overproduction, spoilage, prep trim, plate waste) as a pie/bar chart with dollar amounts (acceptance: interactive chart; drill-down to specific ingredients within each category)
- [ ] Ingredient-level waste ranking: top 10 most wasted ingredients by dollar value and weight (acceptance: sortable by value or weight; links to waste history for each ingredient)
- [ ] Shift-level waste breakdown (AM/PM or custom shifts) so managers can identify which shift produces more waste (acceptance: shift definitions are configurable; shows waste per shift as chart and table)
- [ ] Weekly waste summary report auto-emailed to owner/manager every Monday at 7am (acceptance: includes total waste dollars, top 5 wasted ingredients, week-over-week trend, and one AI recommendation; configurable recipients)
- [ ] Waste reduction goal tracker: set a monthly target (e.g., reduce waste to 4% of food cost) and track progress with a visual gauge (acceptance: progress updates daily; shows green/amber/red status)
- [ ] AI-powered ordering recommendations using 30+ days of waste data to identify over-ordering patterns (acceptance: recommendations appear as cards on the dashboard; e.g., "You over-order romaine lettuce by 15% on Mondays — reduce Monday order by 3 cases"; accept/dismiss/snooze actions)
- [ ] User roles: Owner (full access), Manager (logging + reports), Staff (logging only) (acceptance: owner invites team via email; role-based access control; staff cannot view financial data)
- [ ] Restaurant profile setup with location name, operating hours, shift definitions, and food cost target percentage (acceptance: setup wizard on first login; settings editable later)

### v2.0 — Should Have
- [ ] Par level optimizer: AI-suggested prep quantities for each ingredient based on historical sales, waste, and day-of-week patterns
- [ ] Station-level waste tracking (grill, saute, prep, pantry, etc.) with comparative analytics
- [ ] POS integration with Toast and Square to auto-import daily sales data for waste-to-sales correlation
- [ ] Photo attachment for waste log entries to document large waste events
- [ ] Threshold alerts: push/email notification when daily waste exceeds a configurable dollar amount
- [ ] Cross-location benchmarking dashboard for multi-unit operators
- [ ] Manager accountability scoring showing logging compliance rates by shift and manager
- [ ] Bulk waste logging for end-of-day batch entries

### v3.0 — Nice to Have
- [ ] Menu item profitability analysis factoring in waste (true food cost per dish)
- [ ] Inventory integration: auto-track waste against standing inventory levels
- [ ] Food waste sustainability reporting (CO2 equivalent, landfill diversion) for ESG compliance
- [ ] Supplier scorecard: track which supplier's products have highest spoilage rates
- [ ] Catering and event waste module for off-premise operations

## 5. Technical Architecture
- **Frontend**: React (Next.js) for the analytics dashboard (desktop/tablet browser); Progressive Web App (PWA) for the kitchen logging interface — PWA enables offline logging during internet outages (common in kitchens), installable on kitchen tablets without app store deployment, and avoids Apple/Google app store fees on a B2B product
- **Backend**: Node.js with Express on AWS ECS (Fargate) — containerized for reliability (restaurants depend on the tool during service hours); Fargate auto-scales and avoids server management; more predictable performance than Lambda for the real-time dashboard
- **Database**: PostgreSQL on AWS RDS — relational model fits structured waste data (entries, ingredients, shifts, locations); time-series queries for trend analytics are well-supported; JSONB for flexible AI recommendation storage
- **Key APIs**:
  - OpenAI GPT-4 API — powers ordering recommendations and par level optimization using historical waste and sales data as context
  - Toast API / Square API — POS integration for auto-importing daily sales data (v2.0)
  - SendGrid — weekly report emails and threshold alert notifications
  - Stripe — subscription billing
  - AWS S3 — photo storage for waste log attachments
  - Chart.js or Recharts — client-side charting for the analytics dashboard
- **Hosting**: AWS (ECS Fargate + RDS + S3 + CloudFront) — estimated $100/month at MVP scale; Fargate provides consistent uptime critical for a B2B tool used during restaurant operating hours

## 6. Data Model

### Restaurants
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| name | String | Restaurant name |
| owner_user_id | UUID | FK to Users |
| address | String | |
| operating_hours | JSON | {mon: {open, close}, ...} |
| food_cost_target_pct | Decimal | e.g., 30.0 |
| shift_definitions | JSON | [{name: "AM", start: "06:00", end: "14:00"}, ...] |
| subscription_tier | Enum | trial, standard, premium |
| created_at | Timestamp | |

### Users
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| email | String | Unique |
| password_hash | String | |
| name | String | |
| restaurant_id | UUID | FK to Restaurants |
| role | Enum | owner, manager, staff |

### Ingredients
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| restaurant_id | UUID | FK to Restaurants |
| name | String | e.g., "Romaine lettuce" |
| unit | Enum | lb, oz, kg, each, case |
| cost_per_unit | Decimal | e.g., 2.50 per lb |
| category | String | e.g., "Produce," "Protein," "Dairy" |
| is_favorite | Boolean | For quick-access logging |

### Waste Entries
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| restaurant_id | UUID | FK to Restaurants |
| ingredient_id | UUID | FK to Ingredients |
| logged_by_user_id | UUID | FK to Users |
| waste_category | Enum | overproduction, spoilage, prep_trim, plate_waste |
| quantity | Decimal | In ingredient's unit |
| cost | Decimal | Auto-calculated: quantity x cost_per_unit |
| shift | String | AM, PM, or custom shift name |
| station | String | Nullable (v2.0) |
| reason | String | Nullable (dropped, burned, expired, etc.) |
| photo_url | String | Nullable, S3 path |
| logged_at | Timestamp | |

### Waste Goals
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| restaurant_id | UUID | FK to Restaurants |
| target_type | Enum | percentage, dollar_amount |
| target_value | Decimal | e.g., 4.0 (%) or 500 ($) |
| period | Enum | weekly, monthly |
| start_date | Date | |
| end_date | Date | |

### AI Recommendations
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| restaurant_id | UUID | FK to Restaurants |
| type | Enum | ordering, par_level, general |
| message | Text | Human-readable recommendation |
| data | JSON | Supporting data (ingredient, amounts, day patterns) |
| status | Enum | pending, accepted, dismissed, snoozed |
| created_at | Timestamp | |

**Relationships**: A Restaurant has many Users, Ingredients, Waste Entries, Waste Goals, and AI Recommendations. A Waste Entry references one Ingredient and one User. Users belong to one Restaurant.

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Onboarding / Restaurant Setup
A 4-step wizard: (1) Restaurant name, address, and operating hours. (2) Define shifts (AM/PM or custom). (3) Add top 20 ingredients with unit costs (or import CSV). (4) Set food cost target percentage. Each step has a progress bar and clear "Next" button. After setup, the user lands on the dashboard with a "Start Logging Waste" prompt.

### Screen 2: Waste Logging Interface (Kitchen Tablet)
Designed for speed and greasy fingers. Large search bar at top with autocomplete for ingredients; below are 8-12 "favorite" ingredient buttons for the most commonly wasted items. After selecting an ingredient: a number pad for quantity entry, waste category selector (4 large buttons: Overproduction, Spoilage, Prep Trim, Plate Waste), shift auto-detected by current time, and a "Log" button. Confirmation toast appears for 2 seconds. An optional camera button allows attaching a photo. Total waste logged today appears in a small counter in the corner.

### Screen 3: Cost Analytics Dashboard (Owner/Manager View)
Top row of summary cards: Total Waste Today ($), Total Waste This Week ($), Waste as % of Food Cost, and Week-over-Week Trend (up/down arrow with percentage). Below: a line chart showing daily waste dollars over the past 30 days. Below the chart: a category breakdown (pie chart) and top 5 wasted ingredients (bar chart). Date range selector and period comparison toggle. All charts are interactive with drill-down.

### Screen 4: AI Ordering Recommendations
A feed of recommendation cards, each showing: ingredient name, the pattern detected (e.g., "You over-order romaine by 15% on Mondays"), the suggested action ("Reduce Monday romaine order from 20 cases to 17"), estimated savings ("Save ~$45/week"), and action buttons (Accept, Dismiss, Snooze 1 Week). A "Recommendation History" link shows past accepted and dismissed recommendations with outcomes.

### Screen 5: Ingredient Waste Detail
Accessed by tapping an ingredient in any chart or ranking. Shows: total waste for this ingredient over time (line chart), waste by category (which type of waste is most common for this ingredient), waste by shift, waste by day of week (heatmap), and cost impact. Provides context like "Romaine lettuce accounts for 18% of your total waste cost."

### Screen 6: Weekly Report Preview / Email
A clean, printable report showing: total waste dollars for the week, top 5 wasted ingredients, category breakdown, comparison to previous week, progress toward waste reduction goal, one AI recommendation highlight, and logging compliance rate. This is what gets emailed every Monday. Managers can also view it in-app and download as PDF.

### Screen 7: Waste Reduction Goals
A visual goal tracker showing the current month's target (e.g., "Reduce waste to 4% of food cost") with a gauge or progress bar. Below: a trend line showing daily waste percentage approaching or receding from the target. A "Set New Goal" button allows defining targets by percentage or dollar amount for weekly or monthly periods. Historical goal achievement displayed as a scorecard.

### Screen 8: Team Management
List of team members with name, role, email, and last login. Owner can invite new members, assign roles, and deactivate accounts. A logging compliance table shows which team members logged waste in the past 7 days and how many entries each submitted. This supports accountability without being punitive — framed as "logging activity" not "performance score."

### Screen 9: Multi-Location Overview (Premium)
A dashboard showing all locations in a table: location name, total waste this week ($), waste as % of food cost, week-over-week trend, and logging compliance rate. Color-coded rows highlight underperformers. Tapping a location drills into that location's full analytics dashboard. A "Compare" feature overlays waste trends for 2-3 locations on one chart.

### Screen 10: Settings & Billing
Restaurant profile settings (name, hours, shifts, food cost target), ingredient management (add/edit/delete/import), notification preferences (weekly report recipients, alert thresholds), and subscription management. Shows current plan, billing history, and upgrade options. For trial users: a prominent "Your trial ends in X days" banner with a "Subscribe" button.

## 8. Monetization Implementation
The monetization model uses a 14-day free trial with full features (extended to 30 days for users who request it, since 30 days is the minimum for meaningful AI recommendations). After the trial, the free tier reverts to basic spoilage-only logging with a weekly summary email — enough to maintain the logging habit but missing the cost analytics, AI recommendations, and category breakdowns that drive ROI. The primary conversion trigger is the first AI ordering recommendation, which appears after 14 days of data and quantifies savings in dollars (e.g., "Save $45/week by adjusting your romaine order"). This "aha moment" directly justifies the $49/month subscription. The premium tier at $99/month per location targets multi-unit operators and adds cross-location benchmarking, inventory integration, and manager accountability scoring. Pricing is anchored against LeanPath ($500+/month) and Winnow ($1,000+/month), making $49/month feel like a bargain. The sales pitch is always ROI-based: "What's 5% of your monthly food spend? The app costs less than one day of waste."

## 9. Analytics & KPIs
| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| Restaurants in trial | 30 | 80/month new | 100/month new |
| Trial-to-paid conversion rate | 15% | 25% | 28% |
| Active paying restaurants | 10 | 150 | 300 |
| Daily logging compliance (% of active restaurants logging 5+ days/week) | 60% | 85% | 90% |
| Average waste cost reduction per restaurant | $200/month | $1,500/month | $2,000/month |
| AI recommendation acceptance rate | N/A (not enough data) | 40% | 50% |
| Monthly churn rate | 8% | 5% | 4% |
| MRR | $490 | $7,350 | $14,700 |
| NPS (quarterly survey) | N/A | 45 | 55 |
| Average waste entries per restaurant per day | 5 | 12 | 15 |

## 10. 12-Week Launch Plan
| Week | Milestone |
|------|-----------|
| 1 | Finalize wireframes and data model; set up Next.js project, Node.js/ECS backend, PostgreSQL on RDS; design the 30-second waste logging interface for tablets |
| 2 | Build restaurant setup wizard (profile, shifts, ingredient import); implement user authentication and role-based access control (owner, manager, staff) |
| 3 | Build the waste logging interface with ingredient search, autocomplete, favorite buttons, quantity entry, category selection, and shift auto-detection |
| 4 | Build ingredient cost database with manual entry and CSV import; implement auto-cost calculation on waste entries |
| 5 | Build the cost analytics dashboard: summary cards, daily waste trend chart, category breakdown, and top wasted ingredients ranking |
| 6 | Build shift-level waste breakdown; implement waste reduction goal tracker with visual gauge; build weekly email report with SendGrid |
| 7 | Integrate OpenAI GPT-4 API for ordering recommendations using historical waste data; build the recommendation cards UI with accept/dismiss/snooze actions |
| 8 | Implement Stripe subscription billing; build trial-to-paid conversion flow; implement team management and user invitation |
| 9 | Internal QA; recruit 10 pilot restaurants from local network and r/restaurateur; install on kitchen tablets; collect feedback on logging speed and usability |
| 10 | Iterate on pilot feedback; optimize tablet interface based on real kitchen usage; fix critical bugs; begin food supplier partnership outreach to 10 local distributors |
| 11 | Public launch; begin Reddit GTM in r/restaurateur, r/KitchenConfidential, r/smallbusiness; run first Facebook/Instagram ads targeting restaurant owners ($500 budget); attend 1 local restaurant association meetup |
| 12 | Analyze Month 1 metrics; first AI recommendations generated for pilot restaurants; publish first waste reduction case study; begin planning Toast/Square POS integration for v2.0 |

## 11. Growth Loops

**ROI Proof Loop**: Restaurants that reduce waste by $1,500+/month become case studies. Their quantifiable savings stories are shared in restaurant owner communities, supplier events, and industry publications, driving organic sign-ups from other restaurants.

**Food Supplier Partnership Loop**: Suppliers benefit from clients who order smarter (less return/spoilage, more consistent orders). Suppliers co-market the tool to their restaurant clients, and each new restaurant that reduces waste reinforces the supplier's incentive to refer more clients.

**Kitchen Staff Mobility Loop**: Restaurant staff frequently change jobs. A line cook who used the waste tracker at one restaurant mentions it at their next job, introducing the tool to a new establishment. This organic spread accelerates as the user base grows.

**Multi-Location Expansion Loop**: When a single-location restaurant owner opens a second location, they naturally want the same waste tracking system at the new site. Premium tier pricing incentivizes multi-location adoption.

**Weekly Report Shareability Loop**: The Monday morning waste report is designed to be screenshot-worthy — clean, visual, and actionable. Owners share it in group chats with their management team, other restaurant owner friends, and on social media ("We cut waste by 22% in 3 months"), creating organic brand impressions.

## 12. Regulatory & Compliance

- **Food Safety Regulations**: The app tracks waste but does not replace food safety compliance (HACCP, ServSafe). Must include disclaimers that waste logging does not constitute food safety documentation. In jurisdictions with mandatory food waste reporting (e.g., California SB 1383), the app's data could support compliance but should not be marketed as the sole compliance tool without legal review.
- **Data Privacy (CCPA / GDPR)**: Restaurant and employee data is protected under CCPA. Staff logging data (which employees logged what) must be handled carefully — the app should avoid being perceived as an employee surveillance tool. Privacy policy must address employee data collection and usage.
- **Financial Data Security**: Ingredient costs and food cost percentages are competitively sensitive business data. Data must be encrypted at rest and in transit. No cross-restaurant data sharing without explicit consent.
- **AI Recommendation Disclaimers**: AI-powered ordering recommendations are suggestions, not guaranteed outcomes. Include disclaimers: "Recommendations are based on historical patterns and may not account for upcoming events, menu changes, or seasonal fluctuations."
- **PCI-DSS Compliance**: Stripe handles payment processing; no credit card data stored on our servers.
- **Terms of Service**: Must include provisions for data retention, deletion upon account closure, and limitations of liability for business decisions made based on the tool's analytics or recommendations.

## 13. Risk Register
| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| Kitchen staff non-compliance with daily waste logging, resulting in incomplete and unreliable data | High | High | Design 30-second logging interface; allow batch end-of-shift logging; gamify compliance with shift scores; manager visibility into logging rates; guided first-week onboarding with owner present |
| ROI proof takes too long (30-60 days of data needed for AI recommendations), causing trial churn | High | Medium | Show immediate value in week 1 with waste cost totals and industry benchmarks; extend trial to 30 days if requested; provide "quick wins" checklist based on common waste patterns before AI kicks in |
| Restaurant closures and industry downturns shrink the customer base | Medium | High | Target established restaurants (3+ years old); position as recession-essential ("cut costs to survive"); diversify into adjacent verticals (catering, hotel kitchens, university dining, corporate cafeterias) |
| AI ordering recommendations are inaccurate and damage user trust | Medium | High | Start with simple pattern detection (over-ordering on specific days) before complex predictions; allow restaurants to rate recommendations; continuously improve models with feedback; label confidence levels on each recommendation |
| POS integration complexity delays v2.0 and limits growth | Medium | Medium | Launch MVP without POS integration (manual food cost targets); prioritize Toast and Square (largest indie restaurant POS platforms); use their official APIs and partner programs; hire a contract developer for integration if needed |
| Competition from POS platforms (Toast, Square) adding built-in waste tracking features | Low | High | Build deep waste-specific analytics and AI recommendations that POS platforms won't prioritize; establish brand reputation and customer relationships before platforms enter; consider acquisition as an exit strategy if a POS platform shows interest |

## 14. Success Criteria
- **6-month go/no-go**: 150 paying restaurants at $49/month ($7,350 MRR); 25% trial-to-paid conversion rate; 85% daily logging compliance among active restaurants; average waste cost reduction of $1,500/month per restaurant after 3 months of usage; NPS of 45+
- **12-month milestone**: 300 paying restaurants generating $14,700 MRR ($176K ARR); at least 3 food supplier partnerships actively referring restaurants; AI ordering recommendations live with 40%+ acceptance rate; Toast or Square POS integration in development; expansion into 2 adjacent verticals (catering, hotel kitchens)
