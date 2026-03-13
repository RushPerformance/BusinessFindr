# Product Requirements Document: Gig Tax Autopilot

## 1. Executive Summary
Gig workers -- 59 million strong in the US -- overpay the IRS by $3,000-$5,000 annually because they miss deductions, fail to track mileage, and skip quarterly estimated payments, incurring penalties. Gig Tax Autopilot solves this by connecting to gig platform accounts and bank feeds, auto-importing 1099 income, tracking mileage via GPS, using AI to find gig-specific deductions, and calculating real-time quarterly tax estimates with set-aside alerts. The target user is the Uber/DoorDash/Etsy worker earning $20K-$80K/year who is intimidated by taxes and wants an app that tells them exactly what to do -- not an accounting suite that requires expertise. At $7.99/month (half the price of Keeper Tax), the app targets a $920M SAM with a clear path to $2.3M ARR by Year 3, capitalizing on the gap left by Hurdlr's shutdown and gig economy growth.

## 2. User Personas

### Persona 1: Marcus, the Full-Time Rideshare Driver
- **Age**: 29
- **Job**: Full-time Uber and Lyft driver
- **Income**: $52,000/year gross from gig platforms
- **Pain Points**: Drives 1,200 miles/week but tracks zero of them for deductions; got hit with a $1,400 IRS penalty last year for not making quarterly payments; overwhelmed by the idea of calculating self-employment tax; has a shoebox of gas receipts he never organizes
- **Goals**: Know exactly how much to set aside for taxes each week; never get surprised by a tax bill again; maximize deductions so he keeps more of what he earns
- **Tech Comfort**: High -- lives on his phone, uses 3 gig apps daily, comfortable with GPS tracking

### Persona 2: Priya, the Side-Hustle Etsy Seller
- **Age**: 34
- **Job**: Marketing coordinator (W-2) plus Etsy jewelry shop earning $18,000/year
- **Income**: $67,000 combined
- **Pain Points**: Unsure how to separate W-2 and self-employment taxes; doesn't know which supplies, shipping costs, and home office expenses are deductible; files taxes in April and hopes for the best; used TurboTax last year but it didn't help during the year
- **Goals**: Understand her actual tax obligation from Etsy income in real-time; track deductible expenses automatically; feel confident she's not leaving money on the table
- **Tech Comfort**: Moderate -- comfortable with apps but doesn't want complexity; prefers guided experiences

### Persona 3: DeAndre, the Multi-Platform Gig Worker
- **Age**: 24
- **Job**: DoorDash, Instacart, and TaskRabbit worker
- **Income**: $38,000/year across 3 platforms
- **Pain Points**: Juggles income from 3 platforms with no single view of total earnings; living paycheck to paycheck with variable income; got three different 1099 forms last year and had no idea how to reconcile them; doesn't make quarterly payments because he doesn't know how
- **Goals**: See all gig income in one dashboard; get told the exact dollar amount to set aside each week; file taxes without panic
- **Tech Comfort**: High -- digital native, but has zero financial literacy; needs the app to think for him

## 3. User Stories (20+)
1. As a gig worker, I want to connect my Uber account so that my income is automatically imported without manual entry.
2. As a gig worker, I want to connect my bank account so that the app can identify gig-related deposits and expenses.
3. As a rideshare driver, I want automatic GPS mileage tracking so that I never miss a deductible mile.
4. As a multi-platform gig worker, I want to connect DoorDash, Instacart, and Uber simultaneously so that I see all income in one dashboard.
5. As a gig worker, I want the app to classify trips as business or personal so that I only claim legitimate mileage deductions.
6. As a gig worker, I want an AI-powered deduction finder that scans my expenses so that I catch every write-off I'm entitled to.
7. As a gig worker, I want to see my estimated quarterly tax obligation in real-time so that I know exactly how much to set aside.
8. As a gig worker, I want set-aside alerts after each pay period so that I don't spend money I owe the IRS.
9. As a gig worker, I want to generate IRS quarterly payment vouchers with one click so that paying estimated taxes is frictionless.
10. As a gig worker, I want a year-end tax document package so that I can hand everything to a CPA or import into TurboTax.
11. As a gig worker, I want to see my total deductions year-to-date so that I understand how much the app is saving me.
12. As an Etsy seller, I want the app to identify shipping costs, supplies, and platform fees as deductions so that I reduce my taxable income.
13. As a rideshare driver, I want to track car maintenance expenses (oil changes, tires, repairs) as deductions so that I maximize vehicle-related write-offs.
14. As a gig worker, I want to see the percentage of my phone bill that is deductible so that I claim the business-use portion accurately.
15. As a gig worker, I want home office deduction calculation so that I can claim workspace expenses if I qualify.
16. As a gig worker, I want to receive reminders 2 weeks before quarterly tax deadlines so that I never miss a payment and incur penalties.
17. As a new gig worker, I want an onboarding walkthrough that explains self-employment tax basics so that I understand what I owe and why.
18. As a gig worker, I want to compare my tax savings this year versus last year so that I can see the value the app provides.
19. As a gig worker, I want to export a mileage log in IRS-compliant format so that I have documentation in case of an audit.
20. As a multi-platform gig worker, I want the app to reconcile multiple 1099 forms against actual income so that I catch discrepancies before filing.
21. As a gig worker, I want to see a breakdown of self-employment tax, federal income tax, and state income tax so that I understand where my money goes.
22. As a gig worker, I want to manually add cash income (tips, side jobs) so that my tax estimate is complete and accurate.
23. As a gig worker, I want to categorize expenses with one swipe (deductible / not deductible / unsure) so that expense tracking is fast.
24. As a gig worker with a W-2 job, I want to input my W-2 withholding so that the app calculates only the additional tax I owe on gig income.

## 4. Feature Requirements

### MVP (v1.0) -- Must Have
- [ ] Gig platform account connection via Plaid (Uber, Lyft, DoorDash, Instacart) with automatic income import and transaction categorization
- [ ] Bank account connection via Plaid for expense identification and deposit matching
- [ ] Automatic GPS mileage tracking with motion-activity-triggered activation to minimize battery drain
- [ ] Trip classification (business vs. personal) with swipe-to-classify interface and smart suggestions based on location/time patterns
- [ ] AI deduction finder that scans connected bank transactions and flags gig-specific write-offs (phone bill %, supplies, platform fees, car expenses)
- [ ] Real-time quarterly tax estimate calculator accounting for self-employment tax, federal income tax, and standard deduction
- [ ] Set-aside alerts: push notifications after each gig pay period telling the user exactly how much to set aside
- [ ] IRS quarterly payment voucher (Form 1040-ES) generation as downloadable PDF with pre-filled amounts
- [ ] Income dashboard showing total earnings by platform, week, month, and year-to-date
- [ ] Deduction summary dashboard showing total deductions found, categorized by type, with year-to-date savings estimate
- [ ] User authentication (email + password, Google Sign-In) with secure data encryption at rest and in transit
- [ ] Onboarding flow: guided setup connecting platforms, enabling mileage tracking, setting tax filing status

### v2.0 -- Should Have
- [ ] Multi-state tax support for gig workers who operate across state lines
- [ ] Year-end tax document package: organized 1099 reconciliation, deduction summary, mileage log exportable for CPA or tax software import
- [ ] W-2 income integration for side-hustle workers to calculate net additional tax obligation from gig income
- [ ] Etsy, eBay, and Upwork platform integrations for seller/freelancer income import
- [ ] Manual income entry for cash tips, side jobs, and platforms not yet integrated
- [ ] CPA review add-on ($29.99): year-end deduction review by a licensed tax professional
- [ ] Expense receipt photo capture with OCR-based auto-categorization
- [ ] Historical tax comparison: show year-over-year savings and tax obligation trends

### v3.0 -- Nice to Have
- [ ] EFTPS direct integration for one-click quarterly tax payments to the IRS
- [ ] Bluetooth OBD-II device pairing for automatic trip start/stop detection without GPS battery drain
- [ ] TurboTax / H&R Block direct export integration for seamless year-end filing
- [ ] Community features: anonymous benchmarking ("drivers in your city set aside an average of $X/week")
- [ ] Tax audit risk score based on deduction patterns, with audit preparation document bundle

## 5. Technical Architecture
- **Frontend**: React Native (Expo) -- cross-platform iOS/Android from a single codebase; critical for a solo dev to ship on both platforms fast; Expo provides built-in location/GPS APIs needed for mileage tracking
- **Backend**: Node.js with Express on AWS Lambda -- serverless architecture keeps hosting costs near-zero at low user counts and scales automatically during tax season spikes; JavaScript across the stack reduces context switching for a solo developer
- **Database**: PostgreSQL on AWS RDS -- relational database for structured financial data (transactions, deductions, tax calculations) where data integrity is paramount; JSONB columns for flexible platform-specific data schemas
- **Key APIs**:
  - Plaid (bank account + gig platform income connections)
  - Google Maps / Apple MapKit (mileage verification and route logging)
  - OpenAI GPT-4o (deduction classification and expense categorization)
  - IRS EFTPS API (future: direct quarterly payment submission)
  - Twilio / Firebase Cloud Messaging (push notifications and set-aside alerts)
  - Stripe (subscription billing)
- **Hosting**: AWS (Lambda + RDS + S3) -- estimated $200/month at MVP scale; auto-scaling handles tax season traffic spikes without over-provisioning; S3 for document storage (receipts, vouchers)

## 6. Data Model

### Users
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| email | String | Unique, required |
| password_hash | String | Bcrypt hashed |
| name | String | Display name |
| filing_status | Enum | Single, Married Filing Jointly, etc. |
| state | String | Primary state for tax calculation |
| subscription_tier | Enum | Free, Paid, Premium |
| created_at | Timestamp | |

### Platform Connections
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| platform_name | String | Uber, Lyft, DoorDash, Etsy, etc. |
| plaid_access_token | String | Encrypted |
| status | Enum | Active, Disconnected, Error |
| last_synced_at | Timestamp | |

### Transactions
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| platform_connection_id | UUID | FK to Platform Connections (nullable for bank transactions) |
| amount | Decimal | |
| type | Enum | Income, Expense |
| category | String | Platform fee, supplies, phone, etc. |
| is_deductible | Boolean | AI-classified, user-overridable |
| description | String | Transaction description |
| date | Date | |

### Trips (Mileage)
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| start_location | Point | GPS coordinates |
| end_location | Point | GPS coordinates |
| distance_miles | Decimal | Calculated from GPS route |
| classification | Enum | Business, Personal, Unclassified |
| date | Date | |
| route_polyline | Text | Encoded route for verification |

### Tax Estimates
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| quarter | String | e.g., "2026-Q1" |
| gross_income | Decimal | Total gig income for quarter |
| total_deductions | Decimal | Sum of all deductions |
| estimated_se_tax | Decimal | Self-employment tax portion |
| estimated_income_tax | Decimal | Federal income tax portion |
| estimated_state_tax | Decimal | State income tax portion |
| recommended_set_aside | Decimal | Total to set aside |
| voucher_generated | Boolean | Whether PDF was created |
| created_at | Timestamp | |

### Deductions
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| transaction_id | UUID | FK to Transactions (nullable for mileage deductions) |
| trip_id | UUID | FK to Trips (nullable for expense deductions) |
| category | String | Mileage, phone, home office, supplies, etc. |
| amount | Decimal | Dollar value of deduction |
| confidence | Float | AI confidence score (0-1) |
| status | Enum | Auto-classified, User-confirmed, User-rejected |
| tax_year | Integer | |

**Relationships**: Users have many Platform Connections, Transactions, Trips, Tax Estimates, and Deductions. Each Transaction can generate one Deduction. Each Trip can generate one Deduction (mileage). Tax Estimates aggregate Transactions and Deductions for a given quarter.

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Onboarding -- Welcome & Platform Connection
The user sees a friendly welcome screen explaining "Save $3,000+/year on taxes." Three steps are shown: Connect Platforms, Enable Mileage, Set Tax Profile. Tapping "Get Started" leads to a list of gig platforms (Uber, Lyft, DoorDash, Instacart, Etsy) with Connect buttons beside each. The user authenticates via Plaid. A progress indicator shows connected vs. remaining platforms. A "Skip for now" link allows moving ahead.

### Screen 2: Onboarding -- Tax Profile Setup
The user selects filing status (Single, Married Filing Jointly, Head of Household), enters their state, and indicates whether they have W-2 income alongside gig work (with a field for approximate annual W-2 income). A toggle asks "Do you want automatic mileage tracking?" with a brief explanation of battery usage. Tapping "Finish Setup" triggers initial data sync and navigates to the dashboard.

### Screen 3: Main Dashboard
The primary screen shows a summary card at top: "Set Aside This Week: $XX.XX" in large, bold text with a color indicator (green = on track, yellow = behind). Below: Year-to-Date income (broken down by platform in a stacked bar), Total Deductions Found, and Estimated Quarterly Tax. A "Pay Quarterly Tax" button appears when a deadline is approaching (with days remaining). A bottom navigation bar provides access to Dashboard, Trips, Deductions, Expenses, and Profile.

### Screen 4: Trips / Mileage Screen
A map view shows today's tracked routes with color coding (green = business, gray = personal, orange = unclassified). Below the map, a scrollable list of recent trips displays date, distance, and classification. Unclassified trips have a swipe-to-classify gesture (swipe right = business, swipe left = personal). A running total at the top shows "X miles tracked this week | $Y deduction value." A toggle allows starting/stopping manual trip recording.

### Screen 5: Deduction Finder
A feed-style list of identified deductions, each showing the expense description, amount, deduction value, and AI confidence tag (High / Medium / Low). The user can tap to confirm, reject, or re-categorize each deduction. A summary bar at top shows total deductions this month and year-to-date. Filter buttons allow viewing by category (Mileage, Phone, Supplies, Platform Fees, Home Office, Other). A "Scan New Expenses" button triggers a fresh analysis of recent transactions.

### Screen 6: Quarterly Tax Estimator
A detailed breakdown screen showing: Gross Income, minus Deductions, equals Taxable Income. Below, three tax line items: Self-Employment Tax, Federal Income Tax, State Income Tax. The total Estimated Quarterly Payment is highlighted. A timeline shows all four quarterly deadlines with status (Paid, Due Soon, Upcoming). A "Generate Payment Voucher" button creates a pre-filled 1040-ES PDF. A "Set Aside Now" button links to the user's bank app or shows transfer instructions.

### Screen 7: Expense Feed
A chronological list of all bank transactions identified as potentially gig-related. Each entry shows merchant name, amount, date, and current classification (Deductible, Not Deductible, Needs Review). Swipe gestures allow quick classification. A search bar and category filters sit at top. Tapping an expense opens a detail view with the AI's reasoning for its classification and the option to override.

### Screen 8: Year-End Tax Summary
Available in January, this screen presents the full-year tax package: total income by platform, total deductions by category, total mileage with IRS-rate calculation, total estimated tax paid vs. owed. A "Download Tax Package" button generates a ZIP file with: mileage log CSV, deduction summary PDF, income summary by platform, and 1099 reconciliation notes. A CPA review upsell card appears for Premium users.

### Screen 9: Settings & Subscription
Profile settings (name, email, filing status, state, W-2 info), connected platforms with sync status and reconnect options, mileage tracking preferences (GPS sensitivity, battery mode), notification preferences (set-aside alerts, deadline reminders, weekly summary), and subscription management (current plan, upgrade/downgrade, billing history). A "Delete My Data" button provides full data export before deletion.

### Screen 10: Quarterly Deadline Reminder (Push Notification + Deep Link)
Two weeks before each IRS quarterly deadline, a push notification reads "Q1 taxes due in 14 days -- you owe approximately $X,XXX." Tapping opens the Quarterly Tax Estimator screen with the relevant quarter highlighted and the payment voucher ready to generate. A countdown banner persists at the top of the dashboard until the deadline passes or the user marks the payment as made.

## 8. Monetization Implementation

### Paywall Placement
The free tier allows connecting one gig platform, manual mileage logging (no GPS auto-tracking), and a basic quarterly tax estimate without deductions. The paywall triggers when the user attempts to: (a) connect a second platform, (b) enable automatic GPS tracking, (c) view AI-identified deductions, or (d) generate a payment voucher. The upgrade prompt shows the user's estimated annual savings ("You have $2,400 in unclaimed deductions -- upgrade to claim them").

### Upgrade Triggers
- **Deduction preview**: Free users see 3 blurred deductions with a total savings amount visible; tapping "See All Deductions" triggers the paywall.
- **Quarterly deadline urgency**: 2 weeks before a deadline, free users see "Your estimated tax is $X,XXX -- upgrade to see deductions that could reduce this by $Y."
- **Mileage value accumulator**: After 1 week of manual logging, show "You logged 340 miles worth $X -- upgrade to track automatically and never miss a mile."

### Pricing Psychology
- Monthly ($7.99) and annual ($59.99, saving 37%) options presented side-by-side with annual pre-selected.
- "Pays for itself with one missed deduction" messaging throughout.
- 7-day free trial of paid tier during onboarding to build habit before paywall.
- Tax season discount (January-April): first 3 months for $4.99/month to capture seasonal demand.

## 9. Analytics & KPIs

| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| Total Registered Users | 1,500 | 15,000 | 35,000 |
| Paid Subscribers | 50 | 750 | 2,000 |
| Free-to-Paid Conversion Rate | 3% | 5% | 7% |
| Monthly Recurring Revenue (MRR) | $400 | $6,000 | $16,000 |
| Average Miles Tracked / User / Week | 150 | 200 | 250 |
| Deductions Found / User / Month | $150 | $250 | $300 |
| Platform Connections / User | 1.5 | 2.0 | 2.3 |
| Day 14 Retention (Free) | 35% | 45% | 50% |
| Monthly Churn (Paid) | 12% | 8% | 6% |
| Quarterly Vouchers Generated | 20 | 600 | 1,800 |
| App Store Rating | 4.0 | 4.3 | 4.5 |

## 10. 12-Week Launch Plan

| Week | Milestone |
|------|-----------|
| 1 | Finalize tech stack, set up React Native (Expo) project, AWS infrastructure, PostgreSQL schema, CI/CD pipeline, and Plaid sandbox account |
| 2 | Build user authentication (email + Google Sign-In), onboarding flow UI, and tax profile setup (filing status, state, W-2 toggle) |
| 3 | Implement Plaid integration for bank account and gig platform connections; build transaction import pipeline with automatic sync |
| 4 | Build GPS mileage tracking with motion-activity-triggered activation; implement trip recording, route storage, and business/personal classification UI |
| 5 | Develop AI deduction finder: integrate OpenAI API for expense categorization; build deduction feed UI with confirm/reject gestures |
| 6 | Build quarterly tax estimation engine (self-employment tax, federal, state calculations); implement set-aside alert logic and push notifications |
| 7 | Create IRS payment voucher (1040-ES) PDF generation; build quarterly tax estimator screen and deadline timeline |
| 8 | Build main dashboard, expense feed, income breakdown by platform, and subscription paywall with Stripe integration |
| 9 | Internal alpha testing: dogfood with 5-10 gig workers recruited from Reddit; fix critical bugs, tune AI deduction accuracy, optimize GPS battery usage |
| 10 | Beta launch: invite 50 users from r/uberdrivers and r/doordash; collect feedback on tax estimates accuracy, mileage tracking reliability, and UX flow |
| 11 | Iterate on beta feedback: fix top 5 user-reported issues; optimize onboarding conversion; prepare App Store and Play Store listings with screenshots and description |
| 12 | Public launch: submit to App Store and Play Store; publish launch posts on r/uberdrivers, r/doordash, r/freelance; send launch email to beta waitlist; begin paid ad campaigns on Facebook/Instagram targeting gig worker interests |

## 11. Growth Loops

### Viral Loop: Tax Savings Sharing
After each quarter, users see a "Share Your Savings" card: "You saved $X,XXX on taxes this quarter with Gig Tax Autopilot." One-tap sharing to Instagram Stories, Twitter, or gig worker Facebook groups with a branded graphic and referral link. Referred users get a 30-day free trial; referrers get 1 month free for each conversion.

### Content Loop: Gig Worker Tax Tips
The app generates personalized, shareable tax tip cards ("Did you know you can deduct your phone charger?") based on the user's actual deductions. These tips are designed for social sharing on gig worker subreddits and groups, driving organic traffic back to the app.

### Seasonal Spike Loop
Tax season (January-April) creates a natural acquisition spike. Users who sign up during tax season and see the value of deduction tracking are retained year-round for mileage tracking. Each tax season, existing users share their refund/savings results, attracting new cohorts.

### Multi-Platform Network Effect
Users who connect 2+ gig platforms are 3x stickier. The app encourages adding more platforms by showing "You may be missing income from other platforms -- connect DoorDash to get a complete tax picture." Each additional platform increases switching costs.

## 12. Regulatory & Compliance

- **Tax Advice Disclaimer**: The app must prominently display that it provides tax estimates and information, not professional tax advice. Every deduction recommendation must include "Consult a tax professional for advice specific to your situation." Terms of service must include limitation of liability for tax calculations.
- **IRS Compliance**: Mileage logs must conform to IRS documentation requirements (date, destination, business purpose, miles driven) per IRS Publication 463. The 1040-ES voucher generator must use current-year IRS forms and tax rates, updated annually.
- **Financial Data Privacy (Plaid)**: Compliance with Plaid's data access policies and the Consumer Financial Protection Bureau (CFPB) guidance on open banking. Users must grant explicit consent for each connected account. Implement data minimization -- store only necessary transaction data.
- **State Privacy Laws**: CCPA (California), VCDPA (Virginia), CPA (Colorado), and emerging state privacy laws require: user data access/deletion requests honored within 30 days, clear privacy policy, no sale of personal data, opt-out of data sharing.
- **SOC 2 Type I**: Target by Month 12 for enterprise credibility and user trust. Encrypt all data at rest (AES-256) and in transit (TLS 1.3).
- **GPS/Location Data**: iOS and Android require explicit user permission for background location tracking. App Store guidelines mandate clear explanation of why location data is needed. Provide in-app battery usage transparency.

## 13. Risk Register

| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| GPS mileage tracking causes excessive battery drain, leading to 1-star reviews and uninstalls | High | High | Use motion-activity detection to activate GPS only during driving; offer Bluetooth OBD-II as alternative; display battery usage transparency in-app; allow user-configurable GPS accuracy settings |
| AI deduction finder misclassifies expenses, causing users to claim invalid deductions and face IRS penalties | Medium | Critical | Cross-reference all deductions against IRS Publication 463 rules; default to conservative (not deductible) when confidence is below 70%; require user confirmation for all AI-classified deductions; add CPA review add-on; carry errors & omissions insurance |
| Gig platforms restrict API access or change data-sharing policies, breaking income import | Medium | High | Use Plaid bank transaction import as primary method (gig deposits are recognizable); email parsing for 1099s and weekly earnings summaries as secondary; manual CSV upload as fallback; monitor platform API policy changes proactively |
| Tax season traffic spikes overwhelm infrastructure, causing downtime during the highest-value acquisition period | Medium | High | AWS Lambda auto-scaling handles compute spikes; load test to 10x expected traffic before January; implement queue-based processing for tax calculations; set up uptime monitoring with PagerDuty alerts |
| Competitor (Keeper Tax, QuickBooks) drops pricing to match, eliminating price advantage | Low | Medium | Differentiate on gig-specific features (multi-platform income view, trip classification, quarterly payment workflow) that generalist tools won't replicate; build community and brand loyalty; focus on UX simplicity as a moat |
| Regulatory changes to gig worker tax classification (e.g., reclassification as employees) reduce the TAM | Low | High | Monitor federal and state gig worker legislation; diversify to 1099 contractors beyond gig platforms (consultants, tutors, photographers); pivot messaging from "gig worker taxes" to "self-employment taxes" if needed |

## 14. Success Criteria
- **6-month go/no-go**: 750+ paid subscribers, 7%+ free-to-paid conversion rate, $6,000+ MRR, 50%+ Day-14 retention for free users, and average user deduction identification of $200+/month
- **12-month milestone**: 2,000+ paid subscribers, $16,000+ MRR, 4.3+ App Store rating, <6% monthly paid churn, successful tax season (Jan-Apr) with 3x normal signup rate, and at least 3 gig platform integrations live
