# Product Requirements Document: Rent Increase Negotiator

## 1. Executive Summary
Millions of US renters receive rent increase notices each year and accept them without pushback because they lack data, legal knowledge, and confidence to negotiate. Rent Increase Negotiator arms tenants with comparable local listings, rent trend analytics, jurisdiction-specific rent control law lookups, and AI-generated negotiation letters and call scripts — all for a one-time $14.99 fee or $3.99/month monitoring subscription. The target user is an urban renter aged 25-45 earning $35K-$75K who feels powerless after receiving a rent increase notice. With 22 million cost-burdened renter households in the US and no dedicated negotiation tool at consumer scale, this product fills a clear gap and can reach $135K in Year 1 revenue through Reddit-driven organic growth, SEO content targeting "is my rent increase legal," and partnerships with tenant advocacy organizations.

## 2. User Personas

### Persona 1: Maya Chen
- **Age**: 28
- **Job**: Marketing coordinator at a mid-size agency
- **Income**: $52,000/year
- **Location**: Denver, CO (renting a 1BR apartment for $1,650/month)
- **Pain Points**: Just received a $200/month rent increase notice; doesn't know if this is normal for her area; afraid confronting her landlord will make things worse; can't afford to move (first/last/deposit)
- **Goals**: Push back with data so the increase is reduced to $50-$75; avoid confrontation by sending a professional email
- **Tech Comfort**: High — uses apps for everything, comfortable with self-service tools

### Persona 2: Marcus Johnson
- **Age**: 38
- **Job**: Delivery driver (gig worker)
- **Income**: $41,000/year
- **Location**: Austin, TX (renting a 2BR with a roommate for $1,900/month)
- **Pain Points**: Landlord raises rent every year by 8-12%; doesn't know his rights in Texas; already spending 38% of income on rent; has moved twice in 3 years to escape increases
- **Goals**: Find out if there are legal limits on his increase; get a script for calling his landlord; find cheaper alternatives nearby if negotiation fails
- **Tech Comfort**: Moderate — uses phone for everything but prefers simple, guided experiences

### Persona 3: Sandra Reeves
- **Age**: 43
- **Job**: Case manager at a legal aid nonprofit
- **Income**: $48,000/year (professional income); serves clients earning $20K-$35K
- **Pain Points**: Her clients frequently face rent increases but she doesn't have time to research comparables for each one; needs a self-service tool to hand to tenants
- **Goals**: Distribute a reliable, easy-to-use negotiation tool to her client base; reduce intake volume for rent increase cases
- **Tech Comfort**: Moderate — uses standard office tools; needs the tool to be simple enough for her clients who may have limited tech literacy

## 3. User Stories (20+)
1. As a renter, I want to enter my current rent and proposed increase so that I can see whether the increase is above or below local averages.
2. As a renter, I want to see comparable rental listings within a 1-mile radius so that I have concrete data to reference in my negotiation.
3. As a renter, I want to know if my city or state has rent control or stabilization laws so that I understand my legal protections.
4. As a renter, I want to generate a customized negotiation email to my landlord so that I can respond professionally without writing it myself.
5. As a renter, I want a phone call script with specific data points so that I can confidently call my landlord and negotiate verbally.
6. As a renter, I want to see rent trend data for my neighborhood over the past 12-24 months so that I can argue whether the increase is justified by market conditions.
7. As a renter, I want to compare my current rent to the median for my unit type and location so that I know if I'm already overpaying or getting a deal.
8. As a renter, I want to see cheaper comparable listings nearby so that I have a backup plan if negotiation fails.
9. As a renter, I want to receive alerts when my lease renewal is approaching so that I can prepare for potential increases in advance.
10. As a renter, I want to track local rent trends over time so that I can anticipate future increases.
11. As a renter, I want to save my negotiation history so that I can reference past letters and outcomes.
12. As a renter, I want to share my negotiation success story anonymously so that other tenants in my building or area can benefit.
13. As a renter, I want to receive guidance on when to negotiate versus when to move so that I make the best financial decision.
14. As a renter, I want to see the estimated cost of moving versus accepting an increase so that I can do a full cost comparison.
15. As a renter, I want the negotiation letter to include my specific unit details, lease history, and comparables so that it feels personalized, not generic.
16. As a renter, I want to know common landlord counter-arguments and how to respond so that I'm prepared for pushback.
17. As a renter, I want to export my negotiation letter as a PDF so that I can print it or attach it to an email.
18. As a tenant advocate, I want to bulk-generate negotiation kits for multiple clients so that I can serve more people efficiently.
19. As a renter, I want to log the outcome of my negotiation (accepted, partially accepted, rejected) so that the platform can improve its recommendations.
20. As a renter, I want to see success rates for negotiations in my area so that I know my odds before starting.
21. As a renter, I want to receive a notification when new comparable listings appear near me so that my data stays current during an ongoing negotiation.
22. As a renter, I want plain-English explanations of legal terms in my lease so that I understand what I'm agreeing to.
23. As a renter, I want to know the median lease renewal increase percentage for my building or complex so that I can set realistic expectations.

## 4. Feature Requirements

### MVP (v1.0) — Must Have
- [ ] User onboarding flow: enter current rent, unit type (studio/1BR/2BR/3BR+), square footage, location (address or zip code), lease start date, and proposed increase amount
- [ ] Comparable listings display: pull and show 10-20 comparable rental listings within a configurable radius (default 1 mile) with rent price, unit size, and amenities
- [ ] Rent increase benchmarking: show whether the proposed increase is above, below, or in line with local averages (percentage comparison with visual indicator)
- [ ] Rent control/stabilization law lookup: display applicable local and state rent regulations for the user's jurisdiction, with plain-English summaries
- [ ] AI-generated negotiation email: produce a customized, professional negotiation letter using the user's data, comparables, and legal context — editable before sending/downloading
- [ ] Phone call script generator: create a structured call script with key talking points, data citations, and suggested responses to common landlord objections
- [ ] PDF export: allow users to download the negotiation letter and call script as a formatted PDF
- [ ] Alternative listings view: show cheaper comparable units nearby as a fallback if negotiation fails, with links to listing sources
- [ ] Payment integration: Stripe checkout for $14.99 one-time negotiation kit purchase
- [ ] Free tier experience: allow free users to check if their increase is above/below average and view 3 comparable listings before hitting the paywall
- [ ] Mobile-responsive web app: fully functional on mobile browsers (majority of users will access on phone after receiving a notice)
- [ ] Data freshness indicator: show when comparable data was last updated and display confidence scores when data is sparse

### v2.0 — Should Have
- [ ] Lease renewal monitoring: $3.99/month subscription with alerts 60-90 days before lease expiry
- [ ] Rent trend charts: interactive visualization of neighborhood rent trends over 6-24 months
- [ ] Negotiation outcome tracking: let users log results (success, partial success, failure) with savings amount
- [ ] Success rate dashboard: show aggregate negotiation success rates by market/city
- [ ] Move vs. stay calculator: compare the total cost of accepting the increase versus moving to a new unit
- [ ] Multi-language support: Spanish language version (largest non-English renter demographic)
- [ ] Building-level data: aggregate anonymized data from multiple users in the same building or complex
- [ ] Email delivery: option to send the negotiation letter directly via the app (not just download)

### v3.0 — Nice to Have
- [ ] Tenant advocacy org portal: bulk access dashboard for legal aid clinics to generate kits for clients
- [ ] Roommate cost-splitting calculator: divide rent increases among roommates based on room size or income
- [ ] Security deposit recovery tool: generate a demand letter for unreturned deposits using state-specific timelines and laws
- [ ] Community forum: anonymous discussion board for renters in the same building or neighborhood
- [ ] Landlord reputation scoring: aggregate user-reported data on landlord negotiation responsiveness

## 5. Technical Architecture
- **Frontend**: Next.js 14 (React) — server-side rendering for SEO on state-specific landing pages; React for interactive components like the comparable listings map and trend charts; strong ecosystem for rapid solo-dev iteration
- **Backend**: Next.js API Routes + Node.js — keep the stack unified to reduce complexity; serverless functions handle letter generation and data lookups without managing infrastructure
- **Database**: PostgreSQL (via Supabase) — relational model fits the structured data (users, kits, comparables, jurisdictions); Supabase provides auth, row-level security, and real-time subscriptions out of the box
- **Key APIs**:
  - Rentometer API — comparable rental data and median rent by location
  - OpenAI GPT-4o API — negotiation letter and call script generation
  - Google Maps/Geocoding API — address validation and proximity-based comparable search
  - Stripe API — one-time payments and subscription billing
  - Mapbox GL JS — interactive map displaying comparable listings
- **Hosting**: Vercel (frontend + API routes) — $20/month Pro plan; generous free tier for early stage; excellent Next.js integration and edge caching for SEO pages

## 6. Data Model

### Users
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| email | String | User email, unique |
| created_at | Timestamp | Account creation date |
| location_zip | String | User's zip code |
| subscription_status | Enum | free, kit_purchased, monitoring_active |
| stripe_customer_id | String | Stripe customer reference |

### RentalUnits (user's current unit)
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| address | String | Full address |
| unit_type | Enum | studio, 1br, 2br, 3br_plus |
| square_footage | Integer | Unit size |
| current_rent | Decimal | Current monthly rent |
| lease_start_date | Date | Current lease start |
| lease_end_date | Date | Current lease end |

### NegotiationKits
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| rental_unit_id | UUID | FK to RentalUnits |
| proposed_increase | Decimal | Landlord's proposed increase amount |
| local_median_rent | Decimal | Median rent for comparable units |
| increase_vs_average | Decimal | % above or below local average increase |
| generated_letter | Text | AI-generated negotiation letter |
| call_script | Text | AI-generated phone script |
| outcome | Enum | pending, success, partial, failed, null |
| savings_reported | Decimal | User-reported monthly savings |
| created_at | Timestamp | Kit generation date |

### Comparables
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| kit_id | UUID | FK to NegotiationKits |
| address | String | Comparable listing address |
| rent_price | Decimal | Listed rent |
| unit_type | Enum | Unit type |
| square_footage | Integer | Size |
| distance_miles | Decimal | Distance from user's unit |
| source | String | Data source (Rentometer, etc.) |
| listing_date | Date | When the listing was posted |

### Jurisdictions
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| state | String | State code |
| city | String | City name (nullable for state-level laws) |
| has_rent_control | Boolean | Whether rent control exists |
| max_annual_increase | Decimal | Maximum allowed increase percentage (nullable) |
| law_summary | Text | Plain-English summary |
| source_url | String | Link to official law text |
| last_updated | Date | When this record was last verified |

**Relationships**: A User has one RentalUnit. A User has many NegotiationKits. Each NegotiationKit has many Comparables. Each RentalUnit is linked to one Jurisdiction via location.

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Landing Page
The user sees a bold headline: "Your landlord raised your rent. Fight back with data." Below is a single input field for zip code or address with a CTA button "Check My Increase." Below the fold: 3 value props with icons (comparable data, legal lookup, negotiation letter), a testimonial carousel, and a "How It Works" section with 3 steps. Footer includes links to state-specific pages for SEO.

### Screen 2: Unit Details Form
After entering their location, the user sees a step-by-step form: current monthly rent, proposed new rent, unit type (dropdown), square footage (optional), lease end date, and how they received the notice (letter/email/verbal). A progress bar shows "Step 1 of 3." The form is clean with large input fields optimized for mobile.

### Screen 3: Market Analysis Dashboard (Free Tier)
The user sees their proposed increase displayed as a percentage alongside the local average increase. A gauge visualization shows "Your increase: 12% | Local average: 5.2%." Below are 3 comparable listings (blurred remaining ones with a lock icon). A map shows their unit and the 3 visible comparables as pins. A prominent CTA reads "Unlock Full Analysis + Negotiation Letter — $14.99."

### Screen 4: Full Comparable Analysis (Paid)
After purchase, the user sees all 10-20 comparable listings displayed on an interactive map and as a sortable list. Each listing shows address, rent, unit type, square footage, and distance. Filters allow narrowing by unit type, price range, and distance. A summary card shows: "X of Y comparable units are cheaper than your proposed new rent."

### Screen 5: Rent Control Law Lookup
A card displays the applicable rent control or stabilization laws for the user's jurisdiction. It shows: whether rent control exists (yes/no badge), maximum allowed annual increase (if applicable), required notice period for increases, and tenant rights regarding lease renewal. A link to the official legal source is provided. If no rent control exists, the card explains what protections do exist (e.g., notice requirements).

### Screen 6: Negotiation Letter Generator
The user sees a generated negotiation letter in an editable rich-text area. The letter includes the user's name (optional), unit address, current rent, proposed increase, comparable data citations, relevant legal references, and a professional tone requesting a meeting or reduced increase. Buttons allow: "Copy to Clipboard," "Download as PDF," "Edit Letter," and "Send via Email."

### Screen 7: Phone Call Script
A step-by-step call script is displayed in a card format. Each card represents a phase: Opening (introduce yourself, state purpose), Data Presentation (cite comparables and market averages), Legal Context (mention applicable laws), Ask (specific counter-offer amount), and Closing (confirm next steps). Each card includes "If they say X, respond with Y" counter-argument prompts. A "Print Script" button is available.

### Screen 8: Alternative Listings
If negotiation seems unlikely to succeed, this screen shows a list of comparable or cheaper units nearby, sorted by price. Each listing includes rent, unit type, distance, and a link to the original listing. A "Moving Cost Calculator" widget estimates total moving costs (first/last month, deposit, movers, time off work) to help the user decide.

### Screen 9: Monitoring Dashboard (Subscription)
For $3.99/month subscribers, this screen shows a live rent trend chart for their neighborhood, alerts for upcoming lease renewal (countdown timer), a feed of new comparable listings as they appear, and a "Prepare for Renewal" button that launches a fresh negotiation kit 60 days before lease expiry. A monthly email summary is also configurable here.

### Screen 10: Outcome Logging
After a negotiation, a simple form asks: "What happened?" with options (rent stayed the same, reduced increase, landlord rejected, I moved). If the increase was reduced, a field captures the final amount. The user sees: "You saved $150/month — that's $1,800/year!" A prompt asks if they'd like to share their story anonymously to help other renters.

## 8. Monetization Implementation

**Paywall Placement**: The paywall sits after the free market analysis (Screen 3). Free users see their increase vs. the local average and 3 comparable listings — enough to confirm the increase seems high and create urgency — but the full comparable set, negotiation letter, call script, and legal lookup are locked behind the $14.99 one-time purchase.

**Upgrade Triggers**:
- Seeing that their increase is significantly above average (the data creates the emotional hook)
- The blurred comparable listings with a lock icon create curiosity and FOMO
- A savings estimate: "Tenants who negotiate save an average of $1,200/year — this kit costs $14.99"

**Pricing Psychology**:
- $14.99 is anchored against the potential savings ($600-$2,400/year) — a 40-160x ROI
- One-time purchase removes subscription fatigue anxiety; users feel they're buying a specific outcome, not an ongoing commitment
- The $3.99/month monitoring subscription is offered post-purchase via an upsell modal: "Want us to watch your market and prep you for next year's renewal?" — 30% of kit purchasers are projected to convert
- Annual monitoring option ($39.99/year) offered for users who want to lock in savings

## 9. Analytics & KPIs
| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| Monthly Active Users | 500 | 5,000 | 12,000 |
| Negotiation Kits Purchased | 50 | 700 (175/week) | 1,500 |
| Free-to-Paid Conversion Rate | 5% | 8% | 8% |
| Monitoring Subscribers (MRR) | $40 | $600 | $2,000 |
| Average Savings Reported by Users | $100/month | $125/month | $150/month |
| Organic Search Traffic (monthly) | 200 | 8,000 | 25,000 |
| Negotiation Success Rate (reported) | 40% | 55% | 60% |
| Letter PDF Downloads | 60 | 800 | 1,800 |
| Reddit/Social Referral Traffic | 300 | 1,500 | 3,000 |
| Net Promoter Score | 40 | 50 | 55 |

## 10. 12-Week Launch Plan
| Week | Milestone |
|------|-----------|
| 1 | Finalize technical architecture; set up Next.js project, Supabase database, and Stripe integration; begin Rentometer API integration |
| 2 | Build unit details form and comparable data retrieval pipeline; design database schema and seed jurisdiction data for top 10 states |
| 3 | Implement free-tier market analysis dashboard with gauge visualization and 3-comparable preview; build paywall gate |
| 4 | Integrate OpenAI API for negotiation letter and call script generation; build the editable letter interface and PDF export |
| 5 | Build rent control law lookup feature; populate jurisdiction database for top 25 cities with rent control; implement Stripe checkout flow for $14.99 kit |
| 6 | Mobile optimization pass; end-to-end testing of the full purchase flow; deploy to Vercel staging environment; begin beta testing with 10 renters recruited from Reddit |
| 7 | Incorporate beta feedback; fix UX issues; publish first 3 SEO blog posts targeting "is my rent increase legal in [state]"; set up analytics (Mixpanel) |
| 8 | Public launch on Product Hunt, Reddit (r/personalfinance, r/AskNYC, r/LosAngeles), and Hacker News; activate Google Search Console and submit sitemap |
| 9 | Publish 5 additional SEO articles; begin outreach to 20 tenant advocacy organizations; launch first TikTok/Reels content (3 videos) |
| 10 | Analyze first 2 weeks of user data; optimize conversion funnel based on drop-off points; A/B test paywall copy; begin building monitoring subscription flow |
| 11 | Launch $3.99/month monitoring subscription with lease renewal reminders and rent trend alerts; email upsell sequence to existing kit purchasers |
| 12 | Month 3 retrospective: evaluate KPIs against targets; plan v2.0 features based on user feedback; publish case studies from successful negotiations; expand jurisdiction data to top 50 cities |

## 11. Growth Loops

**Savings Share Loop**: After a successful negotiation, users are prompted to share their savings anonymously ("I saved $150/month on my rent using data"). This generates social proof content for Reddit, TikTok, and Twitter that drives new users who just received their own increase notices.

**Lease Renewal Re-engagement Loop**: The monitoring subscription sends alerts 60-90 days before lease renewal. This brings users back annually, and each return is an opportunity for them to share the tool with friends and neighbors who are also approaching renewals.

**Building Network Effect**: When multiple tenants in the same building use the tool, their anonymized data strengthens the comparable analysis for everyone. The app can surface: "3 other tenants in your building also received increases this month." This incentivizes users to share the tool with neighbors.

**Tenant Advocacy Distribution Loop**: Legal aid clinics and tenant unions distribute the tool to their clients, who then share it within their personal networks. Each advocacy org partnership creates a multiplier effect across their entire client base.

**SEO Content Flywheel**: State-specific landing pages ("Is my rent increase legal in California?") rank for high-intent queries that spike every spring during lease renewal season. Each page generates traffic year after year without additional marketing spend, and successful users become case study content.

## 12. Regulatory & Compliance

**Data Privacy**: Collect minimal personal data; do not require real names. Comply with CCPA (California users will be a significant segment). Implement data deletion requests within 30 days. Privacy policy must clearly state what data is collected and that it is not sold to landlords or property management companies.

**Legal Disclaimer**: All generated letters and scripts must be framed as "informational tools" and not "legal advice." A prominent disclaimer must appear on every generated document: "This letter was generated using publicly available data and is not legal advice. Consult a licensed attorney for legal guidance specific to your situation."

**Tenant Protection Laws**: Some jurisdictions have specific rules about tenant-landlord communications (e.g., required formats, certified mail). The app must not generate letters that violate these communication requirements. Have a tenant rights attorney review letter templates for the top 10 states at launch.

**Fair Housing Compliance**: Comparable data displays must not inadvertently enable or suggest discrimination based on protected classes. The tool must not recommend or discourage specific neighborhoods based on demographic data.

**Rental Data Usage**: Ensure compliance with Rentometer API terms of service regarding data display, caching, and attribution. Do not scrape listings from platforms that prohibit it (Zillow's Terms of Service restrict scraping).

## 13. Risk Register
| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| Rental data is sparse or inaccurate in smaller markets, making comparables unreliable | High | High | Launch in top 10 rental markets only; display confidence scores when data is thin; supplement with multiple data sources; allow users to manually add comparables they find |
| AI-generated negotiation letters contain inaccurate legal claims or aggressive language that exposes tenants to retaliation | Medium | High | Attorney review of letter templates for top 10 states; constrained AI prompts that stick to factual data; mandatory disclaimer on all output; user review step before sending |
| Landlord retaliation against tenants who use the tool (non-renewal, poor maintenance response) | Medium | High | Include anti-retaliation law information in every kit; advise users on documenting landlord behavior; connect users with local tenant rights hotlines |
| Extreme seasonality: 70%+ of revenue concentrated in spring lease renewal season | High | Medium | Push annual monitoring subscriptions; build year-round features (security deposit recovery, moving cost calculator); time marketing spend to match seasonal demand rather than fighting it |
| Competitor (DoNotPay, Zillow, or a well-funded startup) launches a dedicated rent negotiation tool | Medium | Medium | Move fast to establish brand and SEO dominance; build community trust and user-generated success stories that are hard to replicate; focus on depth (legal lookup, building-level data) over breadth |
| Stripe payment disputes or chargebacks from users who negotiate unsuccessfully and feel the kit didn't work | Medium | Low | Set clear expectations pre-purchase ("this tool provides data and templates — outcomes are not guaranteed"); offer a satisfaction guarantee with manual refund process; track and reduce refund rate |
| Rentometer API pricing increases or service discontinuation | Low | High | Abstract the data layer to support multiple comparable data sources; cache and store historical data; explore partnerships with alternative providers (Zillow Rental Manager API, ApartmentList) |

## 14. Success Criteria
- **6-month go/no-go**: 700+ negotiation kits sold per month, 8% free-to-paid conversion rate, 500+ monitoring subscribers generating $2,000 MRR, and at least 50% of users who report outcomes indicating a successful or partially successful negotiation
- **12-month milestone**: $135K cumulative revenue, 12,000 registered users, 3 tenant advocacy org partnerships active, top-3 Google ranking for "rent increase negotiation tool" and 5+ state-specific "is my rent increase legal" queries, and a documented average user savings of $100+/month
