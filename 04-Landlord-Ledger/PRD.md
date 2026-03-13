# Product Requirements Document: Landlord Ledger

## 1. Executive Summary
There are 10.6 million individual landlords in the US, with 72% owning fewer than 5 rental units. These small landlords overwhelmingly track rent and expenses using spreadsheets or shoeboxes, while enterprise property management tools like AppFolio ($280/month minimum) and Buildium ($55/month plus per-unit fees) are dramatically overpriced for their needs. The number one pain point is tax time: most small landlords do not know which expenses are IRS-deductible, and generating Schedule E tax forms is confusing and costly ($200-500 in CPA fees). Landlord Ledger solves this with a simple, purpose-built rental property accounting app for 1-10 unit landlords at $9.99/month: track rent payments with automated late reminders, log expenses with receipt photo scanning auto-categorized by IRS Schedule E line items, connect bank accounts via Plaid for auto-importing property transactions, and generate one-click Schedule E tax reports. The Schedule E auto-generation feature is the killer differentiator that no competitor executes well. The business targets $150K in Year 1 revenue from 1,250 subscribers, scaling to $1.5M by Year 3 through landlord community word-of-mouth on BiggerPockets and Reddit.

## 2. User Personas

### Persona 1: Tom Brennan
- **Age**: 47
- **Job**: High school math teacher
- **Income**: $68,000/year salary plus $2,800/month rental income from 3 units (a duplex and a single-family home)
- **Pain Points**: Tracks rent in a Google Sheet that has become a mess of inconsistent formulas and missing months. Has a shoebox of receipts for property repairs that he sorts through in a panic every April. His CPA charges $400 to prepare Schedule E, and Tom is never sure if he is claiming all the deductions he is entitled to. He tried Buildium but it was too complex and expensive for just 3 units.
- **Goals**: Wants a simple system to track rent payments (who paid, who is late) and log expenses with receipt photos throughout the year. At tax time, he wants to press a button and get his Schedule E. Would love late-payment text reminders so he does not have to have awkward conversations with tenants.
- **Tech Comfort Level**: Low-to-moderate -- uses Google Sheets, email, and basic banking apps. Needs a clean, simple interface without property management jargon. If the app feels like enterprise software, he will not use it.

### Persona 2: Aisha Patel
- **Age**: 31
- **Job**: Software Engineer
- **Income**: $125,000/year salary plus $1,400/month rental income from 1 condo unit (her first investment property, purchased 8 months ago)
- **Pain Points**: New to being a landlord and overwhelmed by the financial tracking requirements. Does not fully understand what she can deduct on Schedule E (mortgage interest? repairs? property management software fees?). Currently tracks everything in a Notion database, which has no tax reporting capability. Wants to do everything right from the start so she does not have issues when she scales to more properties.
- **Goals**: Wants a tool that teaches her what is deductible while she tracks it -- essentially guided bookkeeping for landlords. Wants bank account connection so expenses are auto-imported. Wants to feel organized and confident at tax time. Plans to buy a second property next year and wants the tool to grow with her.
- **Tech Comfort Level**: Very high -- comfortable with any technology, API integrations, and complex software. But values simplicity and good design. Will not use an ugly or outdated-feeling tool.

### Persona 3: Miguel Santos
- **Age**: 55
- **Job**: Small business owner (auto repair shop)
- **Income**: $95,000/year from business plus $7,200/month rental income from 8 units across 3 properties
- **Pain Points**: Managing 8 units with a paper-and-spreadsheet system is becoming unsustainable. He spends 6+ hours per month tracking rent, logging expenses, and chasing late payments. Two of his tenants are chronically late, and he dislikes confrontation. He owns properties with a business partner, so their accounting needs to support split ownership and shared expenses. His CPA has urged him to keep better records.
- **Goals**: Wants automated late-payment reminders so he does not have to chase tenants personally. Wants receipt scanning so he can snap a photo of a repair bill from his phone instead of saving paper receipts. Needs multi-owner support for his partnership properties. Wants a clean monthly P&L by property.
- **Tech Comfort Level**: Moderate -- uses his phone for everything (texting, banking, social media) but does not use a computer regularly. The app must work great on mobile. Prefers tapping and scanning to typing.

## 3. User Stories (20+)

1. As a small landlord, I want to add my rental properties with address, unit details, purchase price, and mortgage information so that the app has the foundation for tracking income and expenses per property.
2. As a small landlord, I want to record rent payments for each unit (paid, late, partial, missed) with the date and amount so that I have a clear record of rental income.
3. As a small landlord, I want to send automated late-payment reminders via text and email to tenants who have not paid by the due date so that I do not have to have uncomfortable conversations.
4. As a small landlord, I want to log expenses with a description, amount, date, and category so that I have a complete record for tax purposes.
5. As a small landlord, I want to scan receipt photos with my phone camera and have the app automatically extract the amount, date, and vendor so that I do not have to type expense details manually.
6. As a small landlord, I want expenses to be automatically categorized by IRS Schedule E line items (advertising, auto and travel, cleaning and maintenance, insurance, legal and professional fees, mortgage interest, repairs, supplies, taxes, utilities, depreciation, other) so that I do not have to figure out which category each expense belongs to.
7. As a small landlord, I want to connect my bank account via Plaid so that property-related transactions are automatically imported and categorized, reducing manual entry.
8. As a small landlord, I want to generate a one-click Schedule E tax report at the end of the year that is formatted correctly and ready to give to my CPA or enter into TurboTax so that I save hours and hundreds of dollars in tax preparation.
9. As a small landlord, I want to see a monthly profit-and-loss statement for each property showing rental income minus expenses so that I know how each property is performing financially.
10. As a small landlord, I want to view an annual summary of all properties showing total income, total expenses, and net income so that I can assess my overall rental portfolio performance.
11. As a small landlord, I want to store lease documents (PDFs, photos) for each unit so that I have a centralized place for all lease-related paperwork.
12. As a small landlord, I want tenants to submit maintenance requests through a portal so that I have a written record and can track the status of each request from submission to resolution.
13. As a small landlord, I want to set up multiple properties with multiple units each and track them independently so that the app scales from 1 unit to 10 without becoming complex.
14. As a small landlord, I want to track security deposits for each unit including the amount, date received, and disposition at move-out so that I comply with state regulations on deposit handling.
15. As a small landlord, I want to receive a notification when a lease is approaching expiration (30, 60, 90 days out) so that I can begin renewal conversations or prepare for turnover.
16. As a new landlord, I want to see tooltips explaining each Schedule E category with examples of deductible expenses so that I learn what I can deduct while I track.
17. As a landlord with a business partner, I want to invite a co-owner to view and edit shared property data so that we both have access to the same financial records.
18. As a small landlord, I want to export my data as CSV or PDF (monthly statements, annual summary, Schedule E) so that I can share it with my CPA, business partner, or lender.
19. As a small landlord, I want to mark a property as vacant and track vacancy periods so that I can report vacancy losses on Schedule E and understand my occupancy rate.
20. As a small landlord, I want to filter and search my expenses by property, category, date range, and amount so that I can quickly find specific transactions.
21. As a small landlord, I want to set up recurring expenses (mortgage, insurance, property tax) so that they are automatically logged each month without manual entry.
22. As a small landlord, I want to see year-over-year comparisons of income and expenses per property so that I can identify trends and make informed decisions about rent increases or cost reduction.
23. As a small landlord, I want to categorize capital improvements separately from repairs so that I handle depreciation correctly on my taxes.
24. As a small landlord, I want a dashboard that shows me at a glance: total rent collected this month, outstanding balances, upcoming expenses, and properties needing attention so that I can quickly understand my portfolio status.

## 4. Feature Requirements

### MVP (v1.0) -- Must Have
- [ ] Property and unit management: add properties with address, purchase price, purchase date, and mortgage details; add individual units with rent amount, tenant name, and lease dates (acceptance criteria: supports up to 10 units across multiple properties, data persists and syncs across devices)
- [ ] Rent tracking: record rent payments as paid, late, partial, or missed with date and amount; display a month-by-month rent roll showing payment status for every unit (acceptance criteria: supports partial payments, calculates outstanding balance automatically, color-codes payment status)
- [ ] Automated late-payment reminders: send text (SMS via Twilio) and/or email reminders to tenants when rent is not recorded as paid by the due date (acceptance criteria: configurable due date per unit, reminder sent on day-after-due and 7-days-late, tenant phone/email stored per unit, opt-out supported)
- [ ] Expense logging: manually enter expenses with description, amount, date, property assignment, and Schedule E category (acceptance criteria: supports all 15 IRS Schedule E line item categories, allows splitting an expense across properties, attached notes field)
- [ ] Receipt photo scanning: use phone camera to capture receipt images, OCR extracts amount, date, and vendor automatically (acceptance criteria: OCR accuracy of 85%+ on clear receipts, user can edit extracted values before saving, receipt image stored as attachment)
- [ ] Auto-categorization by Schedule E line items: AI-powered categorization of expenses into the correct IRS Schedule E category based on description and vendor (acceptance criteria: 80%+ accuracy, user can override suggested category, tooltip explains each category with examples)
- [ ] Bank connection via Plaid: connect bank accounts and automatically import transactions, filter for property-related expenses (acceptance criteria: supports top 50 US banks, transaction import within 24 hours, user confirms or dismisses each imported transaction before it is recorded)
- [ ] One-click Schedule E report: generate a pre-filled Schedule E tax report for each property showing income, all expense categories, and net income/loss (acceptance criteria: matches IRS Schedule E format, exportable as PDF, includes all recorded data for the selected tax year)
- [ ] Monthly property P&L: per-property profit-and-loss statement showing rental income minus categorized expenses (acceptance criteria: generated automatically from recorded data, viewable in-app, exportable as PDF)
- [ ] User authentication and multi-device sync: email/password and Google OAuth login with data synced across web and mobile (acceptance criteria: real-time sync, secure session management)
- [ ] Schedule E educational tooltips: contextual help explaining each expense category with 2-3 examples of deductible expenses, shown when the user selects a category or hovers over a category in reports (acceptance criteria: covers all 15 Schedule E categories, language is plain English not tax jargon)

### v2.0 -- Should Have
- [ ] Tenant maintenance request portal: a simple web form where tenants can submit maintenance requests with description and photos; landlord sees a queue and can update status (received, in progress, completed)
- [ ] Lease document storage: upload and organize PDF/photo lease documents per unit with expiration date tracking and renewal reminders (30/60/90 days)
- [ ] Multi-owner support: invite a co-owner to view and edit shared property data with configurable permissions (view-only vs. edit)
- [ ] Security deposit tracking: record deposit amounts, deductions at move-out, and disposition with compliance reminders for state-specific return deadlines
- [ ] Recurring expense templates: set up auto-logged monthly expenses (mortgage, insurance, HOA, property tax) that are recorded automatically each period
- [ ] Vacancy tracking: mark units as vacant with start/end dates, report vacancy losses on Schedule E
- [ ] Year-over-year comparison reports: compare income and expenses by property across tax years
- [ ] CSV and PDF export: export all financial data (rent roll, expenses, P&L, Schedule E) in multiple formats for CPA sharing

### v3.0 -- Nice to Have
- [ ] Capital improvement vs. repair categorization with depreciation tracking and schedule
- [ ] Annual property tax assessment tracker with appeal deadline reminders
- [ ] Integration with TurboTax and H&R Block for direct Schedule E data import
- [ ] Rent comparable analysis: show similar rental prices in the area to inform rent-setting decisions
- [ ] Tenant screening integration (credit check and background check via third-party API)

## 5. Technical Architecture
- **Frontend**: React with Next.js 14 (App Router) for the web application, plus React Native with Expo for the mobile app (iOS and Android) -- chosen because small landlords need both web access (for detailed reporting and data entry) and mobile access (for receipt scanning, quick rent recording, and on-the-go expense logging). Shared TypeScript types and API client between web and mobile. Tailwind CSS for web styling, NativeWind for mobile.
- **Backend**: Node.js with Express.js on AWS Lambda (serverless) -- chosen for cost efficiency (pay-per-invocation is ideal for an app with usage spikes around rent due dates and tax season), rapid development, and excellent ecosystem support for Plaid, Twilio, and OCR APIs. TypeScript throughout. API Gateway routes requests to Lambda functions.
- **Database**: PostgreSQL on AWS RDS -- chosen for relational data integrity (properties contain units, units have tenants, tenants have payment records, properties have expenses linked to Schedule E categories -- highly relational). Strong support for financial calculations, date-range queries (monthly/annual reporting), and aggregations. Redis (AWS ElastiCache) for caching Plaid sessions and rate limiting.
- **Key APIs**:
  - Plaid API -- bank account connection and transaction import for auto-detecting property-related expenses
  - Google Cloud Vision API (OCR) -- receipt photo text extraction (amount, date, vendor)
  - OpenAI API (GPT-4o-mini) -- auto-categorization of expenses by Schedule E line items based on description and vendor
  - Twilio API -- SMS delivery for late-payment reminders to tenants
  - SendGrid API -- email delivery for late-payment reminders, lease expiration alerts, and weekly landlord summaries
  - Stripe API -- payment processing for the $9.99/month and $19.99/month subscription tiers
  - RevenueCat -- mobile subscription management for iOS and Android
- **Hosting**: AWS serverless stack: Lambda for API ($20-50/month at launch), RDS PostgreSQL (db.t3.micro, $15/month), S3 for receipt image and lease document storage ($5-10/month), CloudFront CDN for web app ($5/month), ElastiCache Redis ($15/month). Vercel for Next.js web frontend ($20/month Pro plan). Total infrastructure: ~$80-115/month at launch. Tax season (Jan-Apr) traffic spikes handled seamlessly by Lambda auto-scaling.

## 6. Data Model

### Users
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| email | String | Unique, indexed |
| password_hash | String | bcrypt |
| name | String | Display name |
| plan | Enum | free, paid, premium |
| stripe_customer_id | String | Nullable |
| created_at | Timestamp | |

### Properties
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| address | String | Full street address |
| city | String | |
| state | String | 2-letter code |
| zip | String | |
| purchase_price | Decimal | For depreciation |
| purchase_date | Date | |
| mortgage_monthly | Decimal | Nullable |
| mortgage_interest_annual | Decimal | For Schedule E |
| property_type | Enum | single_family, duplex, triplex, fourplex, condo, other |

### Units
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| property_id | UUID | FK to Properties |
| unit_label | String | e.g., "Unit A" or "Main House" |
| rent_amount | Decimal | Monthly rent |
| rent_due_day | Integer | Day of month (1-28) |
| tenant_name | String | Nullable (vacant) |
| tenant_email | String | Nullable |
| tenant_phone | String | Nullable |
| lease_start | Date | Nullable |
| lease_end | Date | Nullable |
| security_deposit | Decimal | Nullable |
| status | Enum | occupied, vacant |

### RentPayments
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| unit_id | UUID | FK to Units |
| month | Date | First of the month |
| amount_due | Decimal | Expected rent |
| amount_paid | Decimal | What tenant paid |
| status | Enum | paid, partial, late, missed |
| paid_date | Date | Nullable |
| notes | String | Nullable |
| reminder_sent | Boolean | Default false |

### Expenses
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| property_id | UUID | FK to Properties |
| description | String | |
| amount | Decimal | |
| date | Date | |
| schedule_e_category | Enum | advertising, auto_travel, cleaning_maintenance, commissions, insurance, legal_professional, mortgage_interest, repairs, supplies, taxes, utilities, depreciation, other |
| vendor | String | Nullable |
| receipt_image_url | String | S3 URL, nullable |
| detection_source | Enum | manual, plaid, receipt_scan |
| plaid_transaction_id | String | Nullable |
| is_capital_improvement | Boolean | Default false |
| notes | String | Nullable |

### PlaidConnections
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| plaid_access_token | String | Encrypted |
| institution_name | String | |
| status | Enum | active, disconnected |
| last_synced_at | Timestamp | |

### LeaseDocuments
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| unit_id | UUID | FK to Units |
| file_name | String | |
| file_url | String | S3 URL |
| uploaded_at | Timestamp | |

### MaintenanceRequests (v2.0)
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| unit_id | UUID | FK to Units |
| description | String | |
| photo_urls | JSONB | Array of S3 URLs |
| status | Enum | submitted, in_progress, completed |
| submitted_at | Timestamp | |
| completed_at | Timestamp | Nullable |

### Relationships
- A User has many Properties
- A Property has many Units and many Expenses
- A Unit has many RentPayments, LeaseDocuments, and MaintenanceRequests
- A Unit belongs to one Property
- Expenses are linked to Properties (not individual units) as most expenses (repairs, insurance, taxes) apply at the property level
- PlaidConnections belong to Users and import transactions that become Expenses

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Dashboard (Main Screen)
The landlord opens the app and sees an at-a-glance portfolio overview. Top section: three summary cards showing Total Rent Collected This Month (with amount and percentage of expected rent), Outstanding Balances (number of units with unpaid/partial rent and total amount owed), and Net Income This Month (total rent minus total expenses). Below: a "Needs Attention" section listing actionable items -- units with late rent (tap to send reminder or record payment), upcoming lease expirations (within 90 days), and open maintenance requests. Below that: a property list showing each property as a card with address, number of units, occupancy status, and this month's P&L. The dashboard is designed so the landlord can check everything in 30 seconds.

### Screen 2: Property Detail
Tapping a property from the dashboard opens its detail view. Top section: property address, photo (optional), purchase price, and mortgage details. Tabs below: "Units" (list of all units with tenant name, rent amount, this month's payment status), "Expenses" (filterable list of all expenses for this property), "P&L" (monthly profit-and-loss chart and table), and "Documents" (lease files and property documents). The Units tab is the default view, showing each unit as a card with a prominent "Record Payment" button and payment status badge (green=paid, yellow=partial, red=late, gray=vacant).

### Screen 3: Rent Roll
A month-by-month grid view of all units and their payment status. Columns: Unit (property + unit label), Tenant, Rent Due, Status (paid/partial/late/missed), Amount Paid, Date Paid. Rows are color-coded by status. A month selector at the top allows navigating to any month. Tapping a cell opens a payment entry form to record or edit the payment. A "Send Reminders" batch button sends late-payment texts/emails to all tenants with outstanding balances. Totals at the bottom: total expected, total collected, total outstanding. This screen gives the landlord a complete picture of rent collection status across their entire portfolio.

### Screen 4: Expense Entry and Receipt Scanner
Two entry modes accessible from a floating "+" button. Manual entry: a form with fields for description, amount, date, property (dropdown), and Schedule E category (dropdown with tooltips). Receipt scanner: opens the phone camera to capture a receipt photo. After capture, the OCR processes the image and auto-fills amount, date, and vendor. The landlord confirms or edits the extracted values, selects the property, and the AI suggests a Schedule E category (with a tooltip explaining why). A "Save Expense" button records the entry. Previously scanned receipt images are displayed as thumbnails on the expense detail view.

### Screen 5: Bank Transaction Import
After connecting a bank account via Plaid, the landlord sees a list of imported transactions that might be property-related. Each transaction shows: date, description, amount, and a suggested Schedule E category. The landlord can tap to "Accept" (records as an expense for a selected property), "Dismiss" (not property-related), or "Edit" (change category or property assignment). A "Select All Similar" feature lets the landlord batch-accept recurring transactions (e.g., monthly mortgage payments). Accepted transactions are marked as imported and do not appear again. A filter shows only unreviewed transactions.

### Screen 6: Schedule E Report Generator
The centerpiece feature. The landlord selects a tax year and property, and the app generates a formatted Schedule E report. The report displays: property address, total rental income (sum of rent payments), and each expense category with its total (matching IRS Schedule E line items). Net income/loss is calculated and highlighted. A "Potential Deductions You May Be Missing" section flags common deductions the landlord has not recorded (e.g., "Did you drive to the property this year? Auto and travel expenses are deductible."). Export buttons: "Download PDF" (formatted for CPA handoff) and "Copy to Clipboard" (for TurboTax manual entry). A "Accuracy Check" badge shows data completeness (e.g., "11 of 12 months have recorded rent payments").

### Screen 7: Late Payment Reminder Configuration
A settings screen for configuring automated tenant reminders. Per-unit settings: tenant contact info (phone, email), reminder timing (send on day-after-due, 3-days-late, 7-days-late -- configurable), reminder channels (SMS, email, or both), and message template (customizable with merge tags: {tenant_name}, {amount_due}, {property_address}, {days_late}). A preview shows exactly what the tenant will receive. A "Send Test" button lets the landlord preview the message on their own phone. At the bottom: a log of all reminders sent, showing date, recipient, and delivery status.

### Screen 8: Monthly P&L Report
A per-property financial report showing rental income, itemized expenses by Schedule E category, and net income/loss for the selected month. Displayed as both a clean table and a visual bar chart (income vs. expense categories). A month selector allows navigation. Below the current month: a 12-month trend chart showing net income over time with markers for significant expenses. A "Compare to Last Year" toggle overlays the previous year's data. Export button generates a PDF suitable for partner sharing or lender documentation.

### Screen 9: Tenant Communication / Maintenance Portal (v2.0)
A split view. Landlord side: a list of all maintenance requests across properties, sorted by status (new, in progress, completed). Each request shows the unit, tenant name, description, submitted date, and attached photos. The landlord can update status, add notes, and log associated expenses (which auto-link to the property). Tenant side (accessed via a unique link per unit): a simple form where the tenant describes the issue, uploads photos, and submits. The tenant can view the status of their submitted requests. No tenant account required -- access via a unit-specific URL with a simple verification (last 4 digits of phone number).

### Screen 10: Settings and Account
User profile (name, email, password). Subscription management (current plan, upgrade/downgrade, billing history). Bank connections (list of Plaid connections with status, reconnect, add new). Notification preferences (reminder timing, email digest frequency). Export and backup (full data export as CSV/PDF). Co-owner management (invite, remove, permissions). Help and support (FAQ, contact, link to r/landlord community). Data management (delete account, data retention policy).

## 8. Monetization Implementation

### Paywall Placement
The free tier allows one property with manual rent tracking and basic expense logging (no auto-categorization, no bank connection, no Schedule E report). This is enough for a new landlord with one property to experience the core value of organized tracking and see the structure of what the paid version offers. The paywall activates when users try to: add a second property, connect a bank account, scan a receipt, auto-categorize expenses, or generate the Schedule E report. The Schedule E report is the single most powerful upgrade trigger because it is the feature that saves immediate, quantifiable money (CPA fees).

### Upgrade Triggers
- Adding a second property: "Upgrade to Paid to track unlimited properties (up to 10 units)"
- Tapping "Generate Schedule E": "This feature saves you $200-500 in CPA fees. Upgrade for $9.99/month to unlock it." (Direct ROI framing)
- Tapping receipt scanner: "Upgrade to scan receipts and auto-categorize expenses by Schedule E line items"
- Tax season push (January): "Tax season is here. Generate your Schedule E in one click -- upgrade now." (Seasonal urgency)
- After recording 10 expenses manually: "You've logged 10 expenses. Upgrade to auto-import from your bank and never miss a deduction."
- After receiving a late rent: "Send automated reminders so you never have to chase rent again. Upgrade to Paid."

### Pricing Psychology
- $9.99/month is positioned as "5-28x cheaper than AppFolio or Buildium" -- landlords are very price-sensitive and comparison shopping is natural in this segment
- The Schedule E report alone saves $200-500 in CPA fees annually, making the $120/year subscription fee a clear 2-4x ROI that is easy to justify
- Annual plan at $89.99/year ($7.50/month) offers a 25% discount and targets tax-season sign-ups (landlords who sign up in January and commit for the year)
- The Premium tier at $19.99/month is positioned around the maintenance portal and multi-owner features -- targeted at landlords with 5-10 units who have more complex needs and higher willingness to pay

## 9. Analytics & KPIs

| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| Properties added (total) | 100 | 1,200 | 4,000 |
| Free-to-paid conversion rate | 8% | 12% | 14% |
| Paid subscribers (cumulative) | 30 | 500 | 1,250 |
| Monthly recurring revenue (MRR) | $300 | $5,000 | $12,500 |
| Schedule E reports generated | 0 (off-season) | 200 (tax season) | 800 (cumulative) |
| Bank connections active (% of paid users) | 50% | 70% | 80% |
| Receipt scans per user per month | 2 | 4 | 6 |
| Late payment reminders sent per month | 50 | 800 | 2,500 |
| Monthly churn rate | 6% | 4% | 3% |
| NPS score | 35 | 45 | 55 |
| Avg. properties per user | 1.4 | 1.8 | 2.1 |
| r/landlord and BiggerPockets mentions per month | 3 | 15 | 40 |

## 10. 12-Week Launch Plan

| Week | Milestone |
|------|-----------|
| Week 1 | Initialize Next.js project (web), Expo project (mobile), set up PostgreSQL on AWS RDS, configure Lambda functions, establish CI/CD pipelines. Design complete database schema for properties, units, tenants, rent payments, and expenses. Research IRS Schedule E line items and build the category taxonomy with educational tooltips. |
| Week 2 | Build property and unit management: CRUD for properties (address, purchase price, mortgage details) and units (rent amount, tenant info, lease dates). Build the dashboard showing portfolio overview with summary cards. |
| Week 3 | Build rent tracking system: record payments (paid/partial/late/missed), rent roll grid view with month-by-month navigation, payment status color coding, and outstanding balance calculations. |
| Week 4 | Build expense logging: manual entry form with Schedule E category dropdown and tooltips, expense list with filtering by property/category/date. Integrate Google Cloud Vision OCR for receipt photo scanning with auto-extraction of amount, date, and vendor. |
| Week 5 | Build AI auto-categorization of expenses by Schedule E line items (OpenAI integration). Build Plaid bank connection: transaction import, property assignment workflow, and batch accept/dismiss interface. |
| Week 6 | Build the Schedule E report generator: aggregate income and categorized expenses per property per tax year, format into IRS-matching layout, generate PDF export. Build monthly P&L report per property with charts. Build data export (CSV, PDF). |
| Week 7 | Build automated late-payment reminders: Twilio SMS and SendGrid email integration, configurable timing and message templates per unit, delivery tracking. Build Stripe subscription billing for paid and premium tiers. |
| Week 8 | Build mobile app (React Native/Expo): receipt camera scanner, rent recording, dashboard view, push notifications for late rent and lease expirations. Test on iOS and Android. Ensure feature parity for critical flows (receipt scan, rent recording, dashboard). |
| Week 9 | QA and beta testing: recruit 15-25 beta users from r/landlord and BiggerPockets forums (target landlords with 2-5 units). Test across multiple banks (Plaid connections), receipt types, and property configurations. Collect feedback on Schedule E report accuracy, auto-categorization quality, and receipt OCR reliability. |
| Week 10 | Prepare launch assets: landing page focused on the Schedule E angle ("Generate your Schedule E in one click -- save $400 in CPA fees"), BiggerPockets forum post draft, r/landlord post draft (authenticity-focused), App Store and Play Store listings, 3 educational blog posts about Schedule E deductions for SEO. |
| Week 11 | Public launch: post on r/landlord and r/realestateinvesting, publish on BiggerPockets forums with case study ("How I set up bookkeeping for my 3 rental units in 20 minutes"), submit to Product Hunt, begin Google Ads targeting "landlord bookkeeping" and "Schedule E software." Offer first 50 users a 3-month free trial. |
| Week 12 | Post-launch iteration: analyze conversion funnel (sign-up > add property > record first payment > upgrade), review Schedule E report feedback from CPAs (reach out to 10 CPAs for accuracy verification), fix bugs, optimize OCR accuracy, plan tax season content campaign (January launch of educational content blitz). Set Month 2-3 growth targets. |

## 11. Growth Loops

### Tax Season Viral Loop
January through April is when landlords desperately need Schedule E reports. The app sends re-engagement emails to free users: "Tax season is here -- generate your Schedule E in one click." Paid users who generate Schedule E reports save real money and talk about it in landlord communities. Content marketing around "Schedule E deductions for landlords" captures high-intent search traffic during this period. Each tax season builds on the previous year's user base and content SEO authority.

### Landlord Community Word-of-Mouth
The r/landlord subreddit (350K members) and BiggerPockets forums (2M+ members) are where small landlords ask for tool recommendations. Every week, threads appear asking "what do you use to track rent and expenses?" Each satisfied Landlord Ledger user who responds to these threads with a recommendation becomes an organic acquisition channel. The Schedule E report feature is the most shareable talking point because it delivers quantifiable savings.

### CPA Referral Loop
When a landlord hands their CPA a clean, properly formatted Schedule E report generated by Landlord Ledger, the CPA notices. CPAs who work with multiple landlord clients become referral sources -- they recommend the app to other clients because it saves them time too. Building a CPA partnership program (v2.0) formalizes this loop with referral incentives.

### Property Growth Expansion
As landlords add more rental properties (a common trajectory in real estate investing), they need more powerful tools. A landlord who starts with 1 unit on the free tier and buys a second property must upgrade to the paid plan. Their expanding portfolio naturally drives revenue growth without additional acquisition cost. The app grows with the landlord.

## 12. Regulatory & Compliance

### Tax Reporting Accuracy
- The Schedule E report is an informational tool, not tax advice. The app must include a clear disclaimer: "Landlord Ledger generates reports based on data you provide. This is not tax advice. Consult a qualified tax professional for tax filing decisions."
- The app must not auto-file taxes or connect directly to IRS systems. It generates a report the user can hand to their CPA or manually enter into tax software.
- Schedule E line item definitions must be reviewed and updated annually based on IRS updates to Form 1040 Schedule E. The most recent IRS instructions should be referenced when building category tooltips.

### Tenant Communication Laws
- **TCPA compliance for SMS**: Late-payment reminders sent via SMS to tenants require landlord attestation that they have tenant consent. The app should include a consent template the landlord can incorporate into their lease agreement.
- **Fair Debt Collection Practices Act (FDCPA)**: Late-payment reminders must not constitute debt collection harassment. The app should limit reminder frequency (no more than 3 per rent cycle by default) and avoid threatening or deceptive language. Templates should be reviewed by a real estate attorney.
- **State-specific landlord-tenant laws**: Different states have different rules about late fees, grace periods, and notice requirements. The app should allow customization of reminder timing to comply with local laws and include a disclaimer that landlords are responsible for knowing their local regulations.

### Financial Data Privacy
- **GLBA**: As the app accesses financial data via Plaid and stores expense/income information, it must implement appropriate data security safeguards.
- **CCPA/CPRA**: California landlords (and tenants whose data is stored) have rights to data access, deletion, and opt-out of sale.
- **Plaid compliance**: Follow all Plaid data access policies. Store access tokens encrypted. Provide clear consent flows explaining what financial data is accessed and why.

### Property and Tenant Data
- Tenant personal information (name, phone, email) stored in the app must be protected. If the app expands to tenant portals, additional privacy considerations apply.
- Receipt images and lease documents stored in S3 must be encrypted at rest and accessible only to the property owner (and authorized co-owners).
- Implement data retention policies: deleted accounts should have associated data purged within 30 days.

## 13. Risk Register

| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| Stessa (owned by Roofstock) adds auto-generated Schedule E reporting to their free tier, eliminating Landlord Ledger's key differentiator | Medium | Critical | Go deeper on the tax side than Stessa can justify: auto-categorize by specific Schedule E line items (not just broad categories), flag common missed deductions, provide educational tooltips, and offer accuracy checks. Stessa is pivoting toward investor analytics and deal sourcing (Roofstock's core business), not tax prep. Also differentiate on late-payment reminders and receipt scanning, which Stessa does not prioritize. |
| Tax season seasonality causes engagement to crater May through December, leading to high churn after tax season | High | High | Build year-round value through late-payment reminders (monthly utility), receipt scanning (ongoing expense tracking), monthly P&L reports, and maintenance tracking. Gate Schedule E behind the paid tier to drive annual subscriptions (users who sign up in January and cancel in May still got their Schedule E, but annual plans prevent this). Send monthly "property P&L" summaries to maintain engagement outside tax season. |
| Plaid bank connection failures with small or regional banks that landlords commonly use | Medium | Medium | Offer manual CSV bank statement import as a fallback. Receipt scanning provides an alternative expense entry path that does not require bank connection. Track Plaid connection success rates by institution and proactively recommend banks with high compatibility. Build a "no bank required" onboarding path that emphasizes manual entry + receipt scanning. |
| Receipt OCR accuracy is too low for property-related receipts (handwritten invoices, faded thermal paper, contractor estimates) | Medium | Medium | Use Google Cloud Vision (industry-leading OCR) and supplement with OpenAI for interpreting ambiguous extractions. Always allow manual override of OCR-extracted values. Display a confidence score and highlight fields that may need review. Build a training dataset from user corrections to improve accuracy over time. Set user expectations: "Scan captures the basics -- you verify the details." |
| IRS changes Schedule E format or deduction rules, requiring immediate updates to the report generator | Low | High | Monitor IRS publication updates annually (typically finalized by November for the following tax year). Build the Schedule E category system as a configurable data structure (not hardcoded) so line items can be added, removed, or relabeled without code changes. Maintain a relationship with a CPA advisor who reviews updates. Push app updates before January 1 each year. |
| Landlord sends excessive or inappropriate late-payment reminders to tenants, resulting in legal complaints or negative press | Medium | Medium | Implement default guardrails: maximum 3 reminders per rent cycle, minimum 24 hours between reminders, professional default templates. Display a warning if the landlord configures aggressive timing. Include a disclaimer that landlords are responsible for compliance with local landlord-tenant laws. Add a tenant opt-out mechanism (reply STOP) to every SMS. Review templates with a real estate attorney before launch. |

## 14. Success Criteria

- **6-month go/no-go**: 500 paid subscribers generating $5,000 MRR, with a free-to-paid conversion rate of 12%+, monthly churn below 4%, at least 200 Schedule E reports generated during tax season (Jan-Apr), bank connection rate of 70%+ among paid users, and receipt scan usage of 4+ scans per user per month (indicating ongoing engagement outside tax season). If tax season conversion is strong but off-season churn is high, invest in late-payment reminders and monthly P&L engagement features. If conversion is weak overall, investigate whether the Schedule E paywall trigger is compelling enough or if the free tier is too generous.
- **12-month milestone**: 1,250 paid subscribers generating $12,500 MRR, with an LTV:CAC ratio of 8:1+, monthly churn below 3% (landlords should be very sticky once properties are set up), 800+ cumulative Schedule E reports generated, NPS of 50+, and at least 30 organic mentions on r/landlord and BiggerPockets per month. 10%+ of paid users on the annual plan. App Store rating of 4.6+ with 200+ ratings. At least 3 CPA referral partnerships established informally (CPAs recommending the app to their landlord clients).
