# Product Requirements Document: Side Hustle Tax Tracker

## 1. Executive Summary
36% of Americans have a side hustle, yet most have no idea how much they owe in taxes on that extra income until a surprise bill arrives in April. Side Hustle Tax Tracker is a dead-simple app that answers one question: "How much do I owe in taxes on my side income?" Users log income and expenses, and the app provides a real-time tax liability estimate (federal + state + self-employment tax), tells them exactly how much to set aside from each payment, sends quarterly payment reminders with pre-filled vouchers, and generates a year-end Schedule C/SE summary. At $4.99/month or $39.99/year, it is 3x cheaper than Keeper Tax and 10x simpler than QuickBooks Self-Employed, targeting the 59 million Americans earning $1K-$50K/year from Etsy, DoorDash, tutoring, freelancing, and reselling. The product can reach $114K in Year 1 revenue through SEO targeting "side hustle tax calculator" queries and community-driven growth in Reddit's side hustle and tax subreddits.

## 2. User Personas

### Persona 1: Jenna Torres
- **Age**: 26
- **Job**: Elementary school teacher (W-2) + Etsy shop owner selling handmade candles
- **Income**: $44,000 salary + $8,500/year from Etsy
- **Pain Points**: Has no idea she owes self-employment tax on her Etsy income; got hit with a $1,400 surprise tax bill last April plus a $200 underpayment penalty; doesn't know what expenses she can deduct (supplies, shipping, Etsy fees)
- **Goals**: Know exactly how much to set aside from each Etsy sale; never get surprised by a tax bill again; maximize deductions
- **Tech Comfort**: High — comfortable with apps, uses Etsy seller dashboard daily

### Persona 2: DeShawn Williams
- **Age**: 34
- **Job**: IT support specialist (W-2) + weekend DoorDash/Uber Eats driver
- **Income**: $62,000 salary + $14,000/year from gig driving
- **Pain Points**: Tracks nothing — just deposits DoorDash payments into his checking account; paid a CPA $350 last year just to figure out his tax situation; doesn't understand quarterly estimated payments
- **Goals**: Replace his CPA with a self-service tool; track mileage and car expenses as deductions; get quarterly payment reminders so he doesn't owe penalties
- **Tech Comfort**: High — tech-savvy, prefers automated solutions over manual tracking

### Persona 3: Carla Nguyen
- **Age**: 41
- **Job**: Stay-at-home parent + freelance graphic designer
- **Income**: $0 W-2 + $22,000/year from freelance design clients
- **Pain Points**: Her freelance income is her household's secondary income; she tracks everything in a spreadsheet but doesn't know how to calculate self-employment tax; misses quarterly deadlines regularly; overwhelmed by Schedule C
- **Goals**: Have the app calculate her exact quarterly payment amounts; export a clean Schedule C summary for her tax preparer; keep receipt photos organized so she never loses a deduction
- **Tech Comfort**: Moderate — uses design software professionally but finds financial apps intimidating

## 3. User Stories (20+)
1. As a side hustler, I want to log income from a payment I just received so that my tax liability estimate stays current.
2. As a side hustler, I want to log a deductible expense with a receipt photo so that I don't forget it at tax time.
3. As a side hustler, I want to see my estimated tax liability in real time (federal + state + self-employment) so that I know how much I owe right now.
4. As a side hustler, I want the app to tell me how much to set aside from each payment so that I always have enough saved for taxes.
5. As a side hustler, I want to receive quarterly payment reminders with the exact amount I owe so that I never miss a deadline.
6. As a side hustler, I want pre-filled quarterly tax vouchers (Form 1040-ES) so that I can submit my estimated payments without manual calculations.
7. As a side hustler, I want a year-end summary formatted for Schedule C and Schedule SE so that I (or my tax preparer) can file easily.
8. As a side hustler, I want to connect my bank account so that side hustle income is auto-imported without manual entry.
9. As a side hustler, I want to scan a receipt with my phone camera so that the app automatically extracts the amount, date, and vendor.
10. As a side hustler, I want to categorize expenses (supplies, mileage, home office, software, etc.) so that they map to the correct Schedule C line items.
11. As a side hustler, I want to learn what expenses are deductible for my type of side hustle so that I don't miss legitimate deductions.
12. As a side hustler, I want to understand the $400 self-employment tax threshold so that I know when I'm required to pay.
13. As a side hustler, I want to see a breakdown of my tax liability (income tax vs. self-employment tax vs. state tax) so that I understand where my money is going.
14. As a side hustler, I want to track multiple income sources separately (Etsy + tutoring) so that I can see profitability by hustle.
15. As a side hustler, I want to calculate my home office deduction (simplified or actual) so that I maximize my write-offs.
16. As a side hustler, I want to track mileage for business driving so that I can claim the standard mileage deduction.
17. As a side hustler, I want to see a monthly profit and loss summary so that I know if my side hustle is actually making money after taxes.
18. As a side hustler, I want to export my data as a CSV or PDF so that I can share it with a tax professional.
19. As a side hustler, I want plain-English explanations of tax concepts (quarterly payments, self-employment tax, estimated tax penalties) so that I can learn as I go.
20. As a side hustler, I want to set my W-2 income and filing status so that the app can calculate my effective marginal tax rate on side income accurately.
21. As a side hustler, I want to see a "tax savings" counter showing how much my tracked deductions have reduced my tax bill so that I feel motivated to keep logging.
22. As a side hustler, I want to receive a push notification after each deposit from a gig platform so that I'm prompted to log it immediately.
23. As a side hustler, I want to compare this quarter's income and expenses to last quarter so that I can spot trends in my business.

## 4. Feature Requirements

### MVP (v1.0) — Must Have
- [ ] Income logging: manually enter income with date, amount, source, and optional note; support for recurring income entries
- [ ] Expense logging: manually enter expenses with date, amount, category (from IRS Schedule C categories), vendor name, and optional receipt photo upload
- [ ] Receipt photo capture: take a photo of a receipt; store the image linked to the expense entry (OCR extraction in v2)
- [ ] Real-time tax liability calculator: display estimated federal income tax, self-employment tax (15.3%), and state income tax based on cumulative income minus deductions
- [ ] "Set aside" recommendation: after each income entry, display the exact dollar amount to save for taxes based on the user's marginal rate
- [ ] W-2 and filing status input: allow users to enter their W-2 salary and filing status (single, married filing jointly, head of household) so the marginal rate on side income is accurate
- [ ] Quarterly payment reminders: push notifications and email reminders 2 weeks and 3 days before each quarterly estimated tax deadline (April 15, June 15, September 15, January 15)
- [ ] Pre-filled quarterly voucher: generate a PDF approximating Form 1040-ES with the calculated quarterly payment amount
- [ ] Year-end tax summary: exportable PDF summarizing total income, expenses by category, and net profit — formatted to align with Schedule C line items
- [ ] Expense categorization: pre-built categories matching IRS Schedule C (advertising, car/truck, supplies, home office, insurance, legal/professional, office expenses, etc.)
- [ ] Dashboard: home screen showing YTD income, YTD expenses, YTD net profit, estimated tax owed, and amount set aside so far
- [ ] User authentication: email/password sign-up with option for Apple/Google sign-in

### v2.0 — Should Have
- [ ] Bank connection via Plaid: auto-import transactions from linked bank accounts; flag potential side hustle income for user confirmation
- [ ] OCR receipt scanning: extract amount, date, and vendor from receipt photos using OCR; auto-populate expense fields
- [ ] Mileage tracker: log business trips with start/end location, miles driven, and automatic IRS standard mileage rate calculation
- [ ] Home office deduction calculator: support both simplified method ($5/sq ft, max 300 sq ft) and actual expense method
- [ ] Multiple income source tracking: tag income by source (Etsy, DoorDash, tutoring) with per-source P&L views
- [ ] State tax support expansion: accurate state income tax calculations for all 50 states (MVP covers top 10 states)
- [ ] Tax education library: short articles and videos explaining common side hustle tax topics (self-employment tax, quarterly payments, deduction categories)
- [ ] CSV export: export all income and expense data as CSV for import into tax preparation software or sharing with a CPA

### v3.0 — Nice to Have
- [ ] AI-powered deduction suggestions: analyze expense patterns and suggest commonly missed deductions for the user's side hustle type
- [ ] Gig platform API integrations: auto-import earnings from Etsy, Uber, DoorDash, and Shopify via their seller/driver APIs
- [ ] Tax filing integration: partner with a tax filing service to allow users to file directly from the app (not the app itself becoming a filer)
- [ ] Year-over-year comparison: compare income, expenses, and tax liability across tax years
- [ ] CPA marketplace: connect users with affordable CPAs who specialize in side hustle/gig worker taxes for complex situations

## 5. Technical Architecture
- **Frontend**: React Native (Expo) — cross-platform mobile app (iOS + Android) is essential since users log income and snap receipts on the go; Expo simplifies deployment for a solo dev; supplemented by a Next.js web dashboard for year-end reporting
- **Backend**: Node.js with Express on AWS Lambda — serverless architecture keeps costs proportional to usage; Lambda handles bursty traffic during quarterly deadline peaks without provisioning servers
- **Database**: PostgreSQL (via AWS RDS or Supabase) — relational model for structured financial data (income entries, expense entries, tax calculations); strong data integrity for financial records; JSON columns for flexible metadata
- **Key APIs**:
  - Plaid API — bank account connection for auto-importing transactions (paid tier only)
  - Google Cloud Vision API — OCR for receipt scanning
  - Tax rate data from Tax Foundation / Avalara — federal and state tax rate tables
  - Stripe API — subscription billing ($4.99/month and $39.99/year plans)
  - Firebase Cloud Messaging / APNs — push notifications for quarterly reminders
  - AWS S3 — receipt photo storage
- **Hosting**: AWS (Lambda + RDS + S3) — estimated $75/month at launch; scales cost-effectively; Lambda free tier covers early usage; S3 for receipt image storage at pennies per GB

## 6. Data Model

### Users
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| email | String | User email, unique |
| filing_status | Enum | single, married_joint, married_separate, head_of_household |
| w2_annual_income | Decimal | W-2 salary for marginal rate calculation |
| state | String | State of residence for state tax calculations |
| subscription_status | Enum | free, monthly, annual |
| stripe_customer_id | String | Stripe reference |
| created_at | Timestamp | Account creation |

### IncomeSources
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| name | String | Source name (e.g., "Etsy Shop," "DoorDash") |
| platform_type | Enum | etsy, uber, doordash, freelance, other |

### IncomeEntries
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| source_id | UUID | FK to IncomeSources |
| amount | Decimal | Gross income received |
| date | Date | Date payment received |
| note | String | Optional description |
| is_auto_imported | Boolean | Whether imported via Plaid |

### ExpenseEntries
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| amount | Decimal | Expense amount |
| date | Date | Date of expense |
| category | Enum | Maps to Schedule C categories |
| vendor | String | Vendor name |
| note | String | Optional description |
| receipt_image_url | String | S3 URL for receipt photo |
| source_id | UUID | FK to IncomeSources (nullable, for source-specific expenses) |

### TaxCalculations
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| tax_year | Integer | Tax year |
| quarter | Integer | 1-4 |
| ytd_income | Decimal | Year-to-date gross income |
| ytd_expenses | Decimal | Year-to-date deductible expenses |
| ytd_net_profit | Decimal | Income minus expenses |
| estimated_se_tax | Decimal | Self-employment tax estimate |
| estimated_federal_income_tax | Decimal | Federal income tax on side income |
| estimated_state_tax | Decimal | State income tax estimate |
| total_estimated_tax | Decimal | Sum of all tax components |
| quarterly_payment_amount | Decimal | Recommended quarterly payment |
| calculated_at | Timestamp | When this snapshot was computed |

**Relationships**: A User has many IncomeSources. Each IncomeSource has many IncomeEntries. A User has many ExpenseEntries. ExpenseEntries optionally link to an IncomeSource. TaxCalculations are computed snapshots generated on each income/expense update and stored for quarterly history.

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Onboarding Flow
A 3-step onboarding after sign-up. Step 1: "What's your day job income?" — input for annual W-2 salary and filing status (single/married/head of household). Step 2: "What's your side hustle?" — pick from a list (Etsy, DoorDash, freelance, tutoring, reselling, other) or add a custom name. Step 3: "What state do you live in?" — dropdown of states. A progress bar shows completion. Final screen: "You're set! Start logging your first income." This data configures the tax calculation engine.

### Screen 2: Dashboard (Home Screen)
The primary screen users see on every app open. Top section shows four cards: YTD Income, YTD Expenses, YTD Net Profit, and Estimated Tax Owed — each with a dollar amount and a small trend arrow. Below is a "Set Aside" banner: "You should have $X saved for taxes so far this year." A prominent "+ Log Income" and "+ Log Expense" floating action button sits at the bottom. A "Next Quarterly Payment" countdown card shows the deadline date and suggested payment amount.

### Screen 3: Log Income
A clean form with fields: Amount (large number input), Date (defaults to today), Source (dropdown of user's registered sources), and Note (optional). After submitting, a confirmation screen shows: "Income logged! Set aside $X from this payment for taxes." The set-aside amount is calculated in real time based on the user's marginal rate. A "Log Another" button allows rapid entry.

### Screen 4: Log Expense
A form with: Amount, Date, Category (dropdown with Schedule C categories and plain-English labels, e.g., "Supplies & Materials," "Advertising & Marketing"), Vendor Name, Note, and a "Snap Receipt" camera button. Tapping the camera opens the phone camera for a receipt photo. After submitting, the dashboard updates and shows: "This deduction saves you approximately $X in taxes."

### Screen 5: Tax Liability Breakdown
A detailed view of the user's estimated tax liability. A donut chart shows the three components: Federal Income Tax, Self-Employment Tax (15.3%), and State Income Tax, with dollar amounts for each. Below: a table showing the calculation: gross income, minus deductions, equals net profit, times applicable rates. A "How is this calculated?" expandable section explains each component in plain English. A "Download Quarterly Voucher" button generates the pre-filled 1040-ES PDF.

### Screen 6: Expense Categories & Deductions
A list view of all Schedule C categories with the user's YTD total for each. Tapping a category shows all expenses in that category. Categories with $0 are shown with a hint: "Common deductions you might be missing" — e.g., if the user hasn't logged any home office expenses, a tip explains the simplified deduction. A pie chart at the top shows the expense distribution across categories.

### Screen 7: Quarterly Payment Reminder
When a quarterly deadline approaches, this screen shows: the deadline date, the recommended payment amount, a breakdown of how it was calculated, and options to "Mark as Paid" or "Snooze Reminder." Below is a link to the IRS Direct Pay website and a downloadable 1040-ES voucher. After marking as paid, the user enters the actual amount paid, which adjusts future quarterly estimates.

### Screen 8: Year-End Tax Summary
Available in January, this screen shows the full-year summary: total income by source, total expenses by category, net profit, total estimated tax, quarterly payments made, and remaining balance owed or overpayment. A "Download Schedule C Summary (PDF)" button generates a formatted document that maps directly to Schedule C line items. A "Share with My CPA" button generates a shareable link or email with the PDF attached.

### Screen 9: Tax Education Hub
A library of short articles and explainer cards organized by topic: "Self-Employment Tax 101," "What Is a Quarterly Estimated Payment?", "Home Office Deduction: Simplified vs. Actual," "Mileage Deduction Guide," "What Happens If I Don't Pay Quarterly." Each article is 300-500 words with examples using real numbers. A "Recommended for You" section surfaces articles relevant to the user's side hustle type.

### Screen 10: Settings & Subscription Management
Profile settings: update W-2 income, filing status, state, and side hustle sources. Subscription management: current plan, upgrade/downgrade options, billing history. Data management: export all data as CSV, delete account. Notification preferences: toggle quarterly reminders, weekly summary emails, and income logging nudges.

## 8. Monetization Implementation

**Paywall Placement**: The free tier allows manual income and expense logging and shows an estimated annual tax liability — enough to demonstrate value and create the "aha moment" of seeing how much they owe. The paywall gates the features that save the most time and prevent the most costly mistakes: bank connection for auto-import, receipt OCR scanning, quarterly payment reminders with pre-filled vouchers, state tax calculations, and the Schedule C/SE export.

**Upgrade Triggers**:
- First quarterly deadline approaching: "Your Q1 estimated payment of $847 is due in 14 days. Upgrade to get your pre-filled voucher and never miss a deadline."
- After logging 10+ manual entries: "Tired of manual entry? Connect your bank to auto-import transactions."
- During tax season (January-April): banner emphasizing "Download your Schedule C summary with one tap — upgrade now."

**Pricing Psychology**:
- $4.99/month is anchored against the cost of a CPA ($200-500) and the cost of underpayment penalties ($200+ average)
- The annual plan ($39.99/year = $3.33/month) is positioned as a 33% savings and encouraged via a comparison table during upgrade
- Free tier is genuinely useful (manual logging + annual estimate) so users trust the app before paying
- No free trial of paid features — instead, the free tier builds habit and the paywall appears at natural friction points

## 9. Analytics & KPIs
| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| Monthly Active Users | 300 | 3,500 | 8,000 |
| Paid Subscribers | 20 | 800 | 1,900 |
| Free-to-Paid Conversion Rate | 4% | 6% | 6% |
| Monthly Recurring Revenue | $100 | $3,800 | $9,500 |
| Weekly Active Users Logging Income/Expenses | 60% of MAU | 60% of MAU | 60% of MAU |
| Quarterly Voucher Downloads | N/A (first Q deadline) | 400 | 1,000 |
| Receipt Photos Uploaded | 50 | 2,000 | 6,000 |
| Monthly Churn Rate | 6% | 4.5% | 4% |
| Average Revenue Per User (blended) | $4.50 | $4.75 | $4.80 |
| SEO Organic Traffic (monthly visits) | 500 | 8,000 | 20,000 |

## 10. 12-Week Launch Plan
| Week | Milestone |
|------|-----------|
| 1 | Finalize tech stack; set up React Native (Expo) project and Node.js/Lambda backend; configure Supabase/PostgreSQL database schema; set up AWS S3 bucket for receipt storage |
| 2 | Build onboarding flow (W-2 income, filing status, state, side hustle type); implement user authentication (email + Apple/Google sign-in) |
| 3 | Build income logging and expense logging forms with category selection; implement receipt photo capture and S3 upload |
| 4 | Build tax calculation engine: federal income tax (marginal brackets), self-employment tax (15.3% with the 92.35% multiplier), and state tax for top 10 states |
| 5 | Build dashboard home screen with YTD summary cards and "set aside" recommendation; implement "amount to save" calculation triggered on each income entry |
| 6 | Build quarterly payment reminder system (push notifications + email via SendGrid); generate pre-filled 1040-ES voucher PDFs; implement Stripe subscription billing |
| 7 | Build year-end tax summary with Schedule C mapping and PDF export; internal testing and QA pass; recruit 15 beta testers from r/sidehustle and r/EtsySellers |
| 8 | Beta testing period: collect feedback, fix critical bugs, refine tax calculation accuracy against CPA-validated test cases; set up Mixpanel analytics |
| 9 | Public launch: submit to App Store and Google Play; publish launch posts on Reddit (r/sidehustle, r/freelance, r/tax); publish first 5 SEO blog posts targeting "side hustle tax calculator" |
| 10 | Post-launch optimization: analyze onboarding drop-off; A/B test "set aside" notification copy; fix top 5 user-reported issues; publish 5 more SEO articles |
| 11 | Begin building Plaid bank connection integration (v2 feature, early start); launch YouTube creator partnerships (3-5 small finance/side hustle channels at $200-$500 each) |
| 12 | Month 3 retrospective: evaluate KPIs; plan v2 roadmap; prepare for Q1 tax season marketing blitz (January); publish tax season prep content; optimize App Store listing (ASO) |

## 11. Growth Loops

**Tax Season Viral Loop**: Every January-April, side hustlers frantically search for tax help. Users who had a smooth tax season share their experience: "This app told me to set aside $X each quarter — no surprise bill for the first time ever." These stories drive organic word-of-mouth on Reddit, TikTok, and in person.

**Quarterly Deadline Re-engagement**: The app contacts users 4 times per year at quarterly deadlines. Each touchpoint re-engages lapsed users and gives them a reason to recommend the app to friends who are also scrambling to figure out their quarterly payments.

**Deduction Discovery Loop**: When the app surfaces a commonly missed deduction ("Did you know you can deduct your Etsy listing fees?"), users save money and feel compelled to tell other sellers. Each deduction discovery is a shareable "I didn't know that!" moment.

**CPA Replacement Word-of-Mouth**: Users who previously paid $200-$500 for a CPA now handle their side hustle taxes for $5/month. The savings story is concrete and shareable: "I fired my CPA and replaced them with a $5 app."

**Content SEO Flywheel**: Blog posts targeting long-tail queries ("do I need to pay quarterly taxes on Etsy income") rank over time and compound traffic. Each article funnels readers to the free tax estimator, which funnels to the app. Content stays relevant year after year with minor annual updates.

## 12. Regulatory & Compliance

**Tax Calculation Accuracy Disclaimer**: The app must prominently state that it provides estimates, not tax advice. It is not a tax preparation tool and does not file returns. Disclaimer: "Estimates are based on current federal and state tax rates and your reported income. Consult a licensed tax professional for personalized tax advice."

**Financial Data Privacy**: All financial data (income, expenses, bank connections) must be encrypted at rest (AES-256) and in transit (TLS 1.3). Comply with CCPA and relevant state privacy laws. If using Plaid, comply with Plaid's consumer data usage policies and the CFPB's open banking guidelines.

**Plaid and Bank Data**: Plaid connections are subject to the consumer's explicit consent. Clearly disclose what data is accessed (transaction history only — not account balances or transfers). Provide a one-click disconnect option. Do not store raw bank credentials.

**Receipt and Document Storage**: Receipt images may contain sensitive information (credit card numbers, personal addresses). Implement automatic PII redaction on stored images or clearly disclose that images are stored as-is. Comply with data retention limits — allow users to delete all data.

**IRS Circular 230 Compliance**: The app must not represent itself as providing tax advice. Avoid language like "you should" or "you must" when discussing tax obligations. Use "estimated" and "may" throughout. This avoids triggering IRS Circular 230 requirements for written tax advice.

**State-Specific Tax Rules**: Tax calculations must be updated annually when federal and state tax brackets change (typically January). Maintain a changelog of rate updates. For the MVP, clearly label which states are supported and display a warning for unsupported states.

## 13. Risk Register
| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| Tax calculation errors cause users to underpay and incur IRS penalties, leading to legal liability and reputation damage | Medium | High | Partner with a tax data provider (Avalara/Tax Foundation) for rate tables; validate calculations against CPA-prepared test cases for each supported state; add prominent disclaimer; carry errors and omissions insurance |
| Extreme seasonality: 60%+ of sign-ups occur January-April, creating uneven revenue and high summer churn | High | Medium | Offer annual plans ($39.99/year) to lock in full-year revenue; build year-round engagement features (expense tracking, income goal setting); time marketing spend to match seasonal demand |
| Plaid API costs ($0.30-$1.50 per bank connection) erode margins for a $5/month product at scale | Medium | Medium | Gate bank connection behind paid tier only; negotiate volume discounts at 5,000+ connections; evaluate alternative providers (MX, Finicity); manual entry remains the free tier experience |
| Receipt OCR accuracy below 90% frustrates users and creates incorrect expense records | Medium | Medium | Use Google Cloud Vision API (industry-leading OCR); always show extracted data for user confirmation before saving; allow manual correction; track and report OCR accuracy rates weekly |
| App Store rejection or compliance issues due to financial/tax content policies | Low | High | Review Apple and Google developer guidelines for financial apps pre-submission; avoid claiming the app files taxes or provides tax advice; categorize as "Finance — Budgeting" not "Tax Preparation" |
| Competitor with more resources (Keeper Tax, QuickBooks, TurboTax) launches a similar low-cost product | Medium | Medium | Differentiate on simplicity (one question: "how much do I owe?") and price ($5 vs. $15+); build brand loyalty and SEO moat before competitors react; focus on side hustlers specifically, not all freelancers |
| User data breach exposing financial records and receipt images | Low | High | Encrypt all data at rest and in transit; implement SOC 2 controls by Year 2; regular security audits; use Supabase row-level security; minimize PII collection; maintain an incident response plan |

## 14. Success Criteria
- **6-month go/no-go**: 800+ paid subscribers, $3,800+ MRR, 6% free-to-paid conversion rate, quarterly voucher download rate of 70%+ among paid users during a quarterly deadline, and monthly churn below 5%
- **12-month milestone**: 1,900+ paid subscribers, $9,500+ MRR ($114K annualized revenue), 8,000+ registered users, top-5 Google ranking for "side hustle tax tracker" and "side hustle tax calculator," OCR receipt accuracy above 92%, and user-reported average tax savings of $200+/year from discovered deductions
