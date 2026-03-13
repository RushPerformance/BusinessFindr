# Product Requirements Document: Divorce Finance Splitter

## 1. Executive Summary
With approximately 750,000 US divorces per year and average divorce costs of $15,000-$30,000, most couples cannot afford a Certified Divorce Financial Analyst ($200-$500/hour) to ensure their asset split is truly equitable after taxes and liquidity are considered. Divorce Finance Splitter is a web application that lets divorcing individuals inventory shared assets, calculate tax-adjusted net values, model equitable splits with a drag-and-drop interface, project post-divorce budgets, and estimate alimony/child support by state. The primary user is a 30-55-year-old going through divorce with moderate asset complexity who wants financial clarity without the cost of a CDFA. With a one-time purchase model at $49.99 (or $14.99/mo for 6 months), a 91% gross margin, and no direct competitor at consumer scale, the product can reach $950K in annual revenue within three years through SEO and divorce attorney referral partnerships.

## 2. User Personas

### Persona 1: Jennifer, the Worried Mom
- **Age**: 41
- **Job**: Elementary school teacher
- **Income**: $52,000/year
- **Pain Points**: Her husband earned more and managed investments; she doesn't understand the difference between a 401(k) and a brokerage account for split purposes; her lawyer charges $350/hour and she can't afford a CDFA on top of that; she's scared of accepting a deal that looks equal but isn't
- **Goals**: Understand the after-tax value of each asset; model different split scenarios; project what her monthly budget will look like post-divorce; feel confident she's getting a fair deal
- **Tech Comfort**: Moderate — uses basic apps, online banking, and Google Sheets

### Persona 2: David, the DIY Mediator
- **Age**: 36
- **Job**: IT project manager
- **Income**: $105,000/year
- **Pain Points**: He and his wife are doing a mediated divorce to save money; they agree on most things but can't figure out how to fairly split the house equity, his stock options, and her pension; a CDFA quoted him $3,000 for a full analysis
- **Goals**: A self-service tool that shows the real value of complex assets; model scenarios both parties can review; reduce the number of hours they need with the mediator
- **Tech Comfort**: High — comfortable with spreadsheets and financial software

### Persona 3: Maria, the Collaborative Divorce Attorney
- **Age**: 48
- **Job**: Family law attorney specializing in collaborative divorce
- **Income**: $165,000/year
- **Pain Points**: Many clients can't afford both her legal fees and a CDFA; she wastes billable hours explaining basic financial concepts; she needs a tool she can recommend to clients for financial self-education before mediation sessions
- **Goals**: A client-facing tool that handles the financial modeling so she can focus on legal strategy; wants to earn a referral commission; wants clients to arrive at mediation better prepared
- **Tech Comfort**: Moderate — uses legal software daily

## 3. User Stories (20+)
1. As a divorcing individual, I want to create a comprehensive inventory of all shared assets (real estate, retirement accounts, bank accounts, vehicles, investments) so that nothing is overlooked in the settlement.
2. As a divorcing individual, I want to see the tax-adjusted net value of each asset so that I understand what a 401(k) is actually worth compared to a brokerage account after taxes.
3. As a divorcing individual, I want to drag assets between two columns (mine vs. spouse's) and see real-time after-tax totals for each side so that I can model different split scenarios.
4. As a divorcing individual, I want to project my post-divorce monthly budget so that I know if I can afford my lifestyle after the split.
5. As a divorcing individual, I want to estimate alimony payments based on my state's formula so that I have realistic expectations before negotiation.
6. As a divorcing individual, I want to estimate child support based on my state's guidelines and custody arrangement so that I can plan financially.
7. As a divorcing individual, I want a debt allocation worksheet so that I can model how to fairly divide mortgages, car loans, and credit card debt.
8. As a divorcing individual, I want a checklist of financial accounts to close, separate, or retitle after divorce so that I don't miss any administrative steps.
9. As a divorcing individual, I want to upload and organize financial documents (tax returns, account statements, property appraisals) so that everything is in one secure place.
10. As a divorcing individual, I want to save multiple split scenarios and compare them side by side so that I can discuss options with my attorney or mediator.
11. As a divorcing individual, I want to export my asset inventory and split model as a PDF report so that I can share it with my lawyer, mediator, or spouse.
12. As a divorcing individual, I want to understand how selling vs. keeping the family home affects my long-term finances so that I make an informed decision about the house.
13. As a divorcing individual, I want to account for the tax implications of transferring retirement accounts (e.g., QDRO requirements) so that I don't face unexpected tax bills.
14. As a divorcing individual, I want to see a timeline of financial steps to complete during and after divorce so that I feel organized and in control.
15. As a divorcing individual, I want tooltips explaining financial terms (QDRO, capital gains, cost basis, vested vs. unvested options) so that I can make informed decisions without a finance degree.
16. As a divorcing individual, I want to model the impact of different custody arrangements on child support amounts so that I see how custody and finances intersect.
17. As a divorcing individual, I want my data to be encrypted and private so that my spouse cannot access my scenarios without permission.
18. As a divorcing individual, I want to track post-divorce budget actuals against projections so that I adjust my spending in the first year.
19. As a divorce attorney, I want to send clients a referral link to the tool so that they arrive at mediation financially prepared and I earn a commission.
20. As a divorce mediator, I want to view a client's split model (with permission) so that I can facilitate negotiations more efficiently.
21. As a divorcing individual, I want to understand how Social Security benefits are affected by divorce so that I factor this into long-term planning.
22. As a divorcing individual, I want a credit rebuilding checklist so that I know how to establish independent credit after years of joint accounts.

## 4. Feature Requirements

### MVP (v1.0) — Must Have
- [ ] Asset inventory with categories: real estate, retirement accounts (401k, IRA, pension), bank accounts, investment/brokerage accounts, vehicles, personal property, and other (acceptance: user can add, edit, and delete assets; each asset has name, current value, type, and ownership fields)
- [ ] Tax-adjusted net value calculator that applies federal and state capital gains rates, early withdrawal penalties, and cost basis to each asset (acceptance: shows pre-tax and after-tax value side by side; covers the 10 most common asset types; tax rates update annually)
- [ ] Drag-and-drop equitable split modeler with two columns (Spouse A / Spouse B) showing real-time after-tax totals as assets are moved (acceptance: totals recalculate instantly; percentage split displays at the top; supports saving up to 5 scenarios)
- [ ] Post-divorce monthly budget projector with income, expenses, alimony, and child support factored in (acceptance: pre-populated expense categories; shows surplus/deficit; comparison to current household budget)
- [ ] Debt allocation worksheet for mortgages, auto loans, student loans, and credit card debt (acceptance: debts can be assigned to either spouse or split; net worth view deducts assigned debts from asset totals)
- [ ] Alimony estimator based on state-specific formulas for all 50 US states (acceptance: user selects state; inputs income for both spouses and marriage duration; output shows estimated monthly/annual alimony and duration)
- [ ] Child support estimator based on state guidelines with custody arrangement inputs (acceptance: supports income shares and percentage-of-income models; user inputs custody split, incomes, and number of children)
- [ ] Financial checklist of accounts to close, separate, or retitle post-divorce (acceptance: checklist items are categorized by urgency; user can mark items complete; covers 25+ common action items)
- [ ] Document organizer for uploading financial documents (PDFs, photos) organized by category (acceptance: supports drag-and-drop upload; 50MB per file; categorized by asset type)
- [ ] Secure user authentication with email/password; data encryption at rest and in transit (acceptance: AES-256 encryption for stored data; TLS 1.3 for transit; no data shared with third parties; account deletion removes all data within 30 days)
- [ ] One-time purchase flow at $49.99 with clear value proposition screen (acceptance: payment processed via Stripe; immediate access upon purchase; receipt emailed; no hidden recurring charges)

### v2.0 — Should Have
- [ ] Side-by-side scenario comparison tool (compare up to 3 saved split models on one screen)
- [ ] PDF export of full asset inventory, split model, and budget projection with professional formatting
- [ ] Financial glossary with tooltips explaining QDRO, capital gains, cost basis, vesting schedules, and 30+ other divorce finance terms
- [ ] Social Security benefit impact calculator for marriages over 10 years
- [ ] Subscription option at $14.99/month for 6 months with ongoing budget tracking and updated split models
- [ ] Post-divorce budget tracking: actual spending vs. projected budget with variance alerts
- [ ] Credit rebuilding checklist with step-by-step guidance
- [ ] Divorce attorney referral marketplace (connect users with collaborative divorce attorneys in their state)

### v3.0 — Nice to Have
- [ ] Business asset valuation module for divorces involving small business ownership
- [ ] Military divorce module with USFSPA rules for military pension division
- [ ] Mediator/attorney portal: professionals can view client models (with permission) and annotate
- [ ] International divorce asset handling (UK, Canada, Australia property and tax rules)
- [ ] AI-powered "fairness analysis" that flags potentially inequitable terms based on comparable case outcomes

## 5. Technical Architecture
- **Frontend**: Next.js (React) — server-side rendering for SEO on divorce calculator landing pages that drive organic traffic; React's component model suits the interactive drag-and-drop split modeler; responsive design for desktop and tablet (primary use case is desktop due to complex financial modeling)
- **Backend**: Node.js with Express on AWS Lambda — serverless keeps costs low; most computation is client-side (split modeling); backend handles authentication, payment processing, and data storage
- **Database**: PostgreSQL on AWS RDS — relational model fits structured financial data (assets, debts, scenarios); row-level security ensures one user cannot access another's data; encryption at rest via RDS encryption
- **Key APIs**:
  - Stripe — one-time purchase and subscription payment processing
  - Tax Foundation API / custom tax rate database — federal and state capital gains rates, income tax brackets (updated annually)
  - Auth0 — user authentication with email/password; SOC 2 compliant for sensitive financial data
  - SendGrid — transactional emails (purchase receipt, scenario export, password reset)
  - AWS S3 — encrypted document storage for uploaded financial documents
  - html2pdf.js or Puppeteer — server-side PDF generation for export reports
- **Hosting**: AWS (Lambda + RDS + S3 + CloudFront) — estimated $50/month at MVP scale; CloudFront serves the Next.js frontend; Lambda handles API requests; S3 stores documents with server-side encryption

## 6. Data Model

### Users
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| email | String | Unique, required |
| password_hash | String | Bcrypt |
| state | String | US state (for tax and alimony calculations) |
| purchase_type | Enum | one_time, subscription, free |
| purchased_at | Timestamp | |
| subscription_expires_at | Timestamp | Nullable |
| created_at | Timestamp | |

### Assets
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| name | String | e.g., "Family Home," "John's 401(k)" |
| category | Enum | real_estate, retirement_401k, retirement_ira, pension, bank_account, brokerage, vehicle, personal_property, other |
| current_value | Decimal | Market value |
| cost_basis | Decimal | For capital gains calculation |
| tax_adjustment_type | Enum | pre_tax, post_tax, capital_gains, no_tax |
| after_tax_value | Decimal | Calculated |
| notes | Text | |

### Debts
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| name | String | e.g., "Mortgage," "Visa credit card" |
| category | Enum | mortgage, auto_loan, student_loan, credit_card, other |
| balance | Decimal | Current balance owed |
| monthly_payment | Decimal | |
| interest_rate | Decimal | |

### Split Scenarios
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| name | String | e.g., "Scenario A: I keep house" |
| allocations | JSON | Array of {asset_id, assigned_to: "A" or "B"} and {debt_id, assigned_to: "A" or "B"} |
| spouse_a_total | Decimal | Calculated after-tax total |
| spouse_b_total | Decimal | Calculated after-tax total |
| created_at | Timestamp | |
| updated_at | Timestamp | |

### Budget Projections
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| scenario_id | UUID | FK to Split Scenarios |
| monthly_income | Decimal | Post-divorce income |
| alimony_amount | Decimal | Received or paid |
| child_support_amount | Decimal | Received or paid |
| expense_categories | JSON | Array of {category, amount} |
| monthly_surplus_deficit | Decimal | Calculated |

### Documents
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| asset_id | UUID | FK to Assets (nullable) |
| file_name | String | |
| file_url | String | Encrypted S3 path |
| category | Enum | tax_return, account_statement, appraisal, other |
| uploaded_at | Timestamp | |

**Relationships**: A User has many Assets, Debts, Split Scenarios, Budget Projections, and Documents. A Split Scenario references Assets and Debts via JSON allocations. A Budget Projection belongs to a Split Scenario.

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Landing Page
A clean, calming design (soft blues and grays — no aggressive reds or adversarial imagery). Headline: "Know What Your Split Is Really Worth." Subheadline: "Tax-adjusted asset modeling that saves you $3,000-$8,000 in financial advisor fees." Below: a free asset checklist download (email capture lead magnet), followed by a demo video, feature overview, pricing, and testimonials. "Start Free" button leads to account creation and the free-tier experience.

### Screen 2: Asset Inventory Dashboard
A table/list view of all added assets with columns: Name, Category, Market Value, After-Tax Value, and Assignment Status (unassigned, Spouse A, Spouse B). Users add assets via an "Add Asset" button that opens a modal with fields for name, category, value, cost basis, and notes. A summary bar at the top shows total marital estate value (pre-tax and after-tax). A sidebar shows the financial checklist progress.

### Screen 3: Tax-Adjusted Value Detail
When a user clicks an asset, a detail panel opens showing the market value, applicable tax treatment (e.g., "401(k): pre-tax — subject to income tax on withdrawal"), the calculated after-tax value, and an explanation of the tax logic. Tooltips define financial terms. An "Edit" button allows updating values.

### Screen 4: Drag-and-Drop Split Modeler
Two columns labeled "You" and "Spouse" with a pool of unassigned assets at the top. Users drag assets and debts into each column. Real-time totals at the bottom of each column show after-tax value and percentage of total estate. A "Difference" indicator shows the dollar gap between the two sides. A "Save Scenario" button names and stores the current arrangement. A "Compare Scenarios" button opens the side-by-side view (v2.0).

### Screen 5: Alimony & Child Support Calculator
Input fields for: state (dropdown), both spouses' annual incomes, marriage duration, number of children, and custody arrangement (percentage or days). Outputs: estimated monthly alimony, alimony duration, monthly child support, and total annual support obligations. A note explains that these are estimates based on state guidelines and actual amounts may vary. Results auto-feed into the budget projector.

### Screen 6: Post-Divorce Budget Projector
Two-column layout: Income (salary, alimony received, child support received, investment income) and Expenses (housing, transportation, food, insurance, childcare, debt payments, etc.). Pre-populated categories with editable amounts. A bottom bar shows monthly surplus or deficit with a color indicator (green for surplus, red for deficit). Users can toggle between "Current Household" and "Post-Divorce" budgets to compare.

### Screen 7: Debt Allocation Worksheet
A list of all debts with columns for name, balance, monthly payment, and assigned-to (dropdown: You, Spouse, Split). Summary shows total debt assigned to each spouse and net worth (assets minus debts) per side. Assigned debts automatically factor into the split modeler and budget projector.

### Screen 8: Document Organizer
A file-manager view with folders by category (Tax Returns, Account Statements, Property Appraisals, Other). Users drag-and-drop files or click to upload. Each document shows filename, upload date, and linked asset (if any). A "Download All" button exports everything as a ZIP file for sharing with an attorney.

### Screen 9: Financial Checklist
A categorized to-do list: "Before Filing" (gather tax returns, list all accounts), "During Divorce" (freeze joint credit cards, update beneficiaries), "After Finalization" (retitle property, update will, open individual accounts). Each item has a checkbox, brief explanation, and priority level. Progress bar shows overall completion percentage.

### Screen 10: Purchase / Upgrade Screen
Triggered when a free-tier user attempts to access the split modeler, alimony calculator, or budget projector. Shows a clear comparison: "Free: Asset inventory + basic checklist" vs. "Full Access ($49.99 one-time): Tax-adjusted modeling, split scenarios, alimony/child support estimates, budget projector, document organizer." A testimonial quote and money-saved calculation reinforce value. "One-time purchase — not a subscription" is prominently displayed. Alternative subscription option ($14.99/mo for 6 months) shown below for users who prefer monthly payments.

## 8. Monetization Implementation
The free tier includes the asset inventory list (with market values but not tax-adjusted values), the basic 50/50 calculator, and the financial checklist. The paywall activates when users attempt to access the core differentiating features: tax-adjusted asset valuation, drag-and-drop split modeler, alimony/child support estimators, post-divorce budget projector, or document organizer. This is effective because users first see their total estate value (engaging) and then realize a simple 50/50 split doesn't account for taxes (creating the "aha" moment that drives conversion). Pricing at $49.99 one-time is positioned as "less than one hour with a financial advisor" and "saves you $3,000-$8,000." The subscription alternative ($14.99/mo for 6 months = $89.94) is offered for users who want ongoing budget tracking as negotiations evolve, capturing higher total revenue from engaged users. Attorney referral partners receive a 20% commission ($10 per conversion), creating a strong incentive for distribution through the professional channel.

## 9. Analytics & KPIs
| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| New free accounts created | 100 | 600/month | 1,200/month |
| Free-to-paid conversion rate | 8% | 12% | 14% |
| Split models completed per paid user | 1.5 | 2.5 | 3.0 |
| Average session duration | 10 min | 15 min | 18 min |
| Organic search traffic (monthly) | 500 | 5,000 | 15,000 |
| Attorney referral sign-ups | 5 | 30 | 80 |
| PDF reports exported | 20 | 200/month | 500/month |
| Customer satisfaction (post-purchase survey) | 4.0/5 | 4.2/5 | 4.3/5 |
| Monthly revenue | $4,000 | $16,000 | $30,000 |
| Subscription vs. one-time purchase ratio | 20/80 | 30/70 | 35/65 |

## 10. 12-Week Launch Plan
| Week | Milestone |
|------|-----------|
| 1 | Finalize wireframes and data model; set up Next.js project, Node.js/Lambda backend, PostgreSQL on RDS; research state-specific alimony and child support formulas for all 50 states |
| 2 | Build user authentication with Auth0; implement asset inventory CRUD with all category types; build the asset list dashboard |
| 3 | Build the tax-adjusted value calculator covering 10 asset types (401k, IRA, Roth IRA, pension, brokerage, real estate, bank account, vehicle, stock options, personal property); validate formulas with CPA consultant |
| 4 | Build the drag-and-drop split modeler using react-beautiful-dnd; implement real-time after-tax total recalculation; scenario save/load functionality |
| 5 | Build alimony estimator with state selection (all 50 states); build child support estimator with custody arrangement inputs; connect outputs to budget projector |
| 6 | Build post-divorce budget projector with income/expense categories; build debt allocation worksheet; integrate debts into split modeler and budget |
| 7 | Build document organizer with S3 upload; build financial checklist with 30+ action items; implement PDF export of split model and budget |
| 8 | Implement Stripe payment (one-time purchase + subscription option); build paywall flow; set up attorney referral tracking with unique links and 20% commission |
| 9 | Internal QA; recruit 15 beta users from r/Divorce and divorce attorney contacts; validate tax calculations against 10 real-world scenarios; CPA review of all financial formulas |
| 10 | Public launch; publish first 5 SEO articles targeting "divorce asset calculator," "how to split 401K in divorce," "tax implications of divorce settlement"; begin Reddit GTM in r/Divorce, r/personalfinance |
| 11 | Begin outreach to 50 divorce mediators and collaborative attorneys for referral partnerships; launch Facebook group engagement in divorce support communities; run first Google Ads test ($200 budget) |
| 12 | Analyze Month 1 metrics; publish case study ("How I modeled my divorce split and saved $5,000 in advisor fees"); begin planning v2.0 features (scenario comparison, Social Security calculator); optimize conversion funnel based on data |

## 11. Growth Loops

**SEO Content Flywheel**: High-intent queries like "divorce asset calculator," "how to split 401K in divorce," and "is 50/50 divorce split fair" drive organic traffic to educational content pages that demonstrate the tool's value and convert visitors to free accounts. Each new article compounds search authority.

**Attorney Referral Network**: Divorce attorneys and mediators refer clients to the tool because (1) clients arrive at mediation better prepared, saving billable time, and (2) attorneys earn a 20% commission. As more attorneys join, referral volume compounds.

**Peer Referral Loop**: Divorcing individuals frequently know other divorcing people (support groups, divorce communities). A user who saves thousands of dollars tells their story, and the emotional resonance of "the tool that saved me during my divorce" creates powerful word-of-mouth.

**Free Checklist Lead Magnet**: The downloadable "Divorce Financial Checklist" captures email addresses of divorcing individuals at the top of the funnel. A drip email sequence educates them on tax-adjusted splits and converts them to free accounts and then paid users.

**Post-Divorce Budget Retention**: The subscription tier ($14.99/mo) keeps users engaged post-settlement with budget tracking, turning a one-time life event into a 6-month relationship that extends LTV and creates opportunities for cross-selling related services (credit rebuilding, financial planning).

## 12. Regulatory & Compliance

- **Not Financial or Legal Advice**: All outputs must be clearly labeled as estimates for informational purposes only. Prominent disclaimers on every screen: "This tool provides estimates and is not a substitute for a Certified Divorce Financial Analyst, CPA, or attorney." Terms of service must include hold-harmless clauses.
- **Tax Calculation Accuracy**: Tax rates and formulas must be updated annually; incorrect calculations could lead users to accept unfavorable settlements. Partner with a CPA to validate all formulas; compare outputs against 50 real CDFA case studies before launch.
- **Data Security (SOC 2 Level)**: Financial and personal data is extremely sensitive during divorce proceedings. Data must be encrypted at rest (AES-256) and in transit (TLS 1.3). Implement strict access controls; no employee should access user data without explicit justification. Consider SOC 2 Type I certification within 12 months.
- **CCPA / GDPR Compliance**: Users must be able to delete all data on request. Privacy policy must clearly state what data is collected, how it's used, and that it's never shared with third parties (including the other spouse).
- **State-Specific Legal Variations**: Alimony and child support formulas vary by state and change periodically. Formulas must be maintained and updated; incorrect state calculations could lead to financial harm. Display "last updated" dates for each state's formulas.
- **Attorney Referral Regulations**: Some states regulate attorney referral fees and services. Ensure the referral program complies with state bar association rules in each jurisdiction where it operates.

## 13. Risk Register
| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| Tax calculation errors leading to users accepting unfavorable settlements | Medium | Critical | Partner with a CPA for formula validation; compare against 50 real case studies; include "estimation only" disclaimers on all outputs; recommend professional review for estates over $500K |
| Emotional user state causing high support burden and negative reviews | High | Medium | Design calming UX with empathetic copy; build comprehensive in-app guidance and tooltips; create FAQ addressing emotional questions; route support to trained responders with empathetic scripts |
| Low repeat usage due to one-time life event limiting revenue growth | High | Medium | Offer subscription tier for ongoing budget tracking; build attorney referral network for continuous new user acquisition; expand to adjacent life events (prenups, estate planning); referral program for peer recommendations |
| State formula changes invalidating alimony/child support calculations | Medium | High | Monitor state legislative updates quarterly; build an admin interface for rapid formula updates; display "last updated" dates; allow user override if they have more current information |
| Liability from users claiming the tool caused financial harm | Low | Critical | Strong terms of service with hold-harmless clauses; "not legal or financial advice" disclaimers on every output screen; recommend professional review for complex estates; carry errors and omissions insurance |
| Attorney referral program running afoul of state bar association rules | Medium | Medium | Research referral regulations in each state before launching there; consult with a legal compliance advisor; structure as "advertising fee" where permitted; remove referral program in states with restrictions |
| Spouse accessing the other spouse's account during contentious divorce | Low | High | Strong authentication with 2FA option; no shared accounts; session timeout after 15 minutes of inactivity; data encryption at rest; clear privacy policy that data is never shared |

## 14. Success Criteria
- **6-month go/no-go**: 500+ paid purchases with 12% free-to-paid conversion rate; 5,000+ monthly organic search visitors; at least 15 attorney referral partners active; customer satisfaction score of 4.2/5; monthly revenue of $16,000; zero reported instances of materially inaccurate tax calculations
- **12-month milestone**: 3,800+ total purchases generating $190K+ cumulative revenue; 15,000 monthly organic visitors from SEO; 80+ attorney referral partners; subscription tier adopted by 30%+ of purchasers; CPA-validated formulas for all 50 states with quarterly updates; v2.0 features (scenario comparison, Social Security calculator) launched
