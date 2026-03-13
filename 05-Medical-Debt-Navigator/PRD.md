# Product Requirements Document: Medical Debt Navigator

## 1. Executive Summary
100 million Americans carry medical debt, with medical bills being the number one cause of personal bankruptcy in the US. The vast majority of patients do not know that virtually every non-profit hospital is legally required to offer financial assistance (charity care) under IRS 501(r) regulations, yet only 50% of eligible patients apply because hospitals bury these programs in fine print. Meanwhile, medical bills are wildly inflatable -- the same procedure can cost $800 or $8,000 depending on whether you negotiate. Medical Debt Navigator is a self-service tool that guides uninsured and underinsured patients through the process of reducing their medical bills by 40-80%: it identifies hospital financial assistance programs, generates pre-filled applications based on the patient's income, provides word-for-word negotiation scripts for phone calls, compares bills against Medicare rates to identify overcharges, and tracks dispute status. At $9.99/month or $29.99 one-time (dramatically cheaper than human negotiation services that take 25-35% of savings), the product serves the massive underserved market of working-class Americans who feel powerless against the medical billing system. Year 1 target is $220K revenue from 7,300 paying users, scaling to $1.5M by Year 3 through Reddit/TikTok virality and healthcare social worker referrals.

## 2. User Personas

### Persona 1: Maria Gonzalez
- **Age**: 32
- **Job**: Restaurant shift manager
- **Income**: $38,000/year (no employer health insurance)
- **Pain Points**: Received a $6,400 ER bill after a car accident. Has no health insurance. Did not know the hospital (a non-profit) has a financial assistance program that could reduce her bill by 80% based on her income. She called the billing department once, was told to pay in full or set up a payment plan, and felt too intimidated to push back. The bill is now 60 days old and she is terrified it will go to collections and ruin her credit.
- **Goals**: Wants to know if she qualifies for financial assistance, what to say when she calls the hospital, and how to avoid collections. Needs the tool to cost a fraction of what she owes -- paying a human negotiator 25% ($1,600) is out of the question. Needs step-by-step guidance because she has never navigated the medical billing system before.
- **Tech Comfort Level**: Moderate -- uses her phone for everything (banking, social media, messaging). Comfortable with mobile apps but needs clear, simple language. English is her second language, so plain-language content is essential.

### Persona 2: James Wright
- **Age**: 44
- **Job**: Freelance photographer
- **Income**: $55,000/year with a high-deductible health plan ($5,000 deductible)
- **Pain Points**: Had a planned knee surgery. His insurance covered most of it, but he owes $4,800 out-of-pocket (his full deductible). He noticed the surgery was billed at $18,000 -- three times the Medicare rate for the same procedure. He suspects he is being overcharged but does not know how to verify this or what leverage he has to negotiate. He has decent credit and does not want medical debt affecting it.
- **Goals**: Wants to compare his bill against fair-market and Medicare rates to identify overcharges. Wants a negotiation script that helps him request the hospital's "uninsured discount" or negotiate a lower rate. Wants to set up an interest-free payment plan that does not go to collections. Willing to pay $30-80 for a tool that saves him thousands.
- **Tech Comfort Level**: High -- uses financial apps, comfortable researching online. Wants data and evidence to support his negotiation, not just generic advice.

### Persona 3: Patricia Coleman
- **Age**: 58
- **Job**: School cafeteria worker
- **Income**: $29,000/year (insured through employer but plan has high copays and limited coverage)
- **Pain Points**: Has $12,000 in accumulated medical debt from multiple providers (primary care, specialist, hospital, lab) over the past 2 years. She has been making minimum payments on three different payment plans but is barely keeping up. Two accounts are with collection agencies. She feels overwhelmed managing multiple bills and does not know that charity care applications can sometimes be submitted retroactively, even after bills go to collections. She is ashamed of her medical debt and has not told her family.
- **Goals**: Wants help organizing all her medical debts in one place. Wants to know which providers offer financial assistance (even retroactively). Needs guidance on dealing with collection agencies (what to say, what not to say, her rights under the FDCPA). Wants a payment strategy that prioritizes the most urgent accounts. The tool needs to feel supportive and non-judgmental.
- **Tech Comfort Level**: Low -- uses her phone for calls, texts, and Facebook. Would need a very simple, guided interface. Might need the option of phone coaching (premium tier).

## 3. User Stories (20+)

1. As a patient with a medical bill, I want to upload or enter my bill details (provider name, amount, procedure codes, date of service) so that the app can analyze my situation and recommend next steps.
2. As a patient, I want the app to identify my hospital/provider and tell me if they have a financial assistance (charity care) program so that I know if I am eligible for a bill reduction.
3. As a patient, I want the app to generate a pre-filled financial assistance application based on my income and household size so that I do not have to figure out the paperwork myself.
4. As a patient, I want word-for-word negotiation scripts for calling the hospital billing department so that I know exactly what to say to request a discount or payment plan.
5. As a patient, I want to compare my bill against Medicare rates for the same procedure codes so that I have evidence of overcharges to use in negotiation.
6. As a patient, I want to see the "fair price" for my procedures based on my geographic area so that I know what a reasonable bill should look like.
7. As a patient, I want a step-by-step action plan (first do this, then do this) so that I do not feel overwhelmed by the process of disputing or reducing my bill.
8. As a patient, I want to track the status of my financial assistance applications and disputes so that I do not lose track of where things stand with each provider.
9. As a patient, I want reminders to follow up on pending applications and disputes so that I do not miss deadlines that could result in my bill going to collections.
10. As a patient, I want to know my rights when dealing with collection agencies so that I am not intimidated into paying more than I owe or agreeing to unfavorable terms.
11. As a patient with multiple medical debts, I want to enter all my bills in one place and see a prioritized action plan (which to address first) so that I can manage the process systematically.
12. As a patient, I want to understand the difference between non-profit and for-profit hospitals and why it matters for financial assistance so that I know which providers are legally required to offer help.
13. As a patient, I want to know if I can apply for financial assistance retroactively (after the bill has already been sent to collections) so that I do not assume it is too late.
14. As a patient, I want to receive a customized letter to send to my provider requesting an itemized bill so that I can verify every charge and identify potential billing errors.
15. As a patient, I want to learn about payment plan options and how to negotiate interest-free payment plans so that I can spread payments without additional cost.
16. As a patient, I want to share my success story (anonymized) within the app community so that others can learn from my experience and feel less alone.
17. As a patient, I want the app's interface and language to be simple, supportive, and non-judgmental so that I do not feel ashamed about my medical debt while using it.
18. As a patient on the premium tier, I want a 30-minute phone coaching session with a trained advocate so that I can get personalized guidance for my specific situation.
19. As a patient, I want to know if any of my medical debt is eligible for dispute based on billing errors (duplicate charges, unbundling, upcoding) so that I do not pay for mistakes.
20. As a patient, I want to understand how medical debt affects my credit score and what protections exist (such as the 2023 credit reporting changes) so that I can make informed decisions about payment timing.
21. As a healthcare social worker, I want to share the app with my patients so that they have a self-service tool to supplement the guidance I provide during limited appointment time.
22. As a patient, I want to calculate my estimated savings from financial assistance before I start the application process so that I am motivated to complete all the steps.
23. As a patient, I want to upload supporting documents (pay stubs, tax returns) and have the app identify which documents each provider's financial assistance program requires so that I gather everything I need before applying.
24. As a patient, I want the app to tell me the specific deadlines for financial assistance applications at my provider so that I do not miss eligibility windows.

## 4. Feature Requirements

### MVP (v1.0) -- Must Have
- [ ] Bill entry and analysis: user enters provider name, bill amount, procedure/diagnosis codes (CPT/ICD-10), and date of service; the app identifies the provider type (non-profit vs. for-profit) and flags relevant next steps (acceptance criteria: supports manual entry and photo upload of bill, correctly identifies non-profit status for top 500 US hospital systems)
- [ ] Hospital financial assistance database: a searchable database of financial assistance policies for major US non-profit hospitals, including eligibility criteria (income thresholds as % of FPL), required documents, application URLs/PDFs, and deadlines (acceptance criteria: covers at least 500 non-profit hospital systems representing 70% of non-profit beds, data verified within the last 6 months)
- [ ] Pre-filled financial assistance application generator: based on user's income, household size, and provider, generate a pre-populated financial assistance application with instructions for submission (acceptance criteria: application fields match the provider's actual form, output as downloadable PDF, includes a cover letter template)
- [ ] Medicare rate comparison: compare the billed amount against Medicare reimbursement rates for the same procedure codes and geographic area to quantify overcharges (acceptance criteria: uses CMS Physician Fee Schedule and Hospital Outpatient data, displays Medicare rate, billed rate, and percentage difference)
- [ ] Negotiation script library: word-for-word phone scripts for common scenarios -- requesting uninsured discount, negotiating bill reduction using Medicare rate comparison, requesting interest-free payment plan, requesting itemized bill, responding to collection calls (acceptance criteria: at least 8 distinct scripts covering the most common negotiation scenarios, scripts include what to say and how to respond to common pushback)
- [ ] Step-by-step action plan: a guided checklist that walks the user through the recommended sequence of actions based on their specific situation (acceptance criteria: adapts based on whether the user is uninsured vs. underinsured, whether the provider is non-profit vs. for-profit, and whether the bill is pre-collections vs. in-collections)
- [ ] Dispute and status tracker: track the status of each bill (new, application submitted, in negotiation, resolved, in collections) with dates, notes, and next-action reminders (acceptance criteria: supports multiple bills per user, sends SMS/email reminders for upcoming deadlines, allows file attachments)
- [ ] Fair price lookup: show the average and median price for procedures in the user's geographic area using publicly available CMS and transparency data (acceptance criteria: covers the 200 most common procedures, data refreshed quarterly)
- [ ] Billing error detection: flag common billing errors (duplicate charges, unbundled charges, upcoding) based on the entered procedure codes and amounts (acceptance criteria: detects at least the 5 most common billing error patterns, provides plain-language explanation of each error)
- [ ] User authentication with progressive data collection: allow anonymous bill analysis to start (enter bill details without account), prompt for account creation when saving or generating applications (acceptance criteria: anonymous first interaction, gentle prompt for signup, guest data migrates to account)
- [ ] Itemized bill request letter generator: generate a customizable letter requesting an itemized bill from the provider, citing the patient's right to receive one (acceptance criteria: letter includes provider name, patient name, account number, and appropriate legal references)

### v2.0 -- Should Have
- [ ] Document upload and requirements matching: upload pay stubs, tax returns, and other supporting documents; the app identifies which documents each provider's financial assistance application requires
- [ ] Collection agency response scripts and FDCPA rights guide: specialized scripts for responding to collection calls, written cease-and-desist letter templates, and a plain-language guide to Fair Debt Collection Practices Act rights
- [ ] Multi-debt management dashboard: view all medical debts in one place with priority scoring (highest urgency first based on collections risk, deadlines, and potential savings)
- [ ] Anonymized success story community: browse success stories from other users showing their original bill, reduction achieved, and method used (financial assistance, negotiation, error dispute)
- [ ] Savings estimator: before starting the process, show the user an estimated savings range based on their income, provider, and bill amount
- [ ] Retroactive financial assistance guidance: specific instructions for applying for charity care after a bill has already been sent to collections (which is possible at many hospitals but poorly documented)
- [ ] Spanish language support: full app translation for the significant Spanish-speaking population that disproportionately carries medical debt
- [ ] Credit score impact education: explain how medical debt affects credit under current rules (2023 changes) and provide strategic advice on payment timing

### v3.0 -- Nice to Have
- [ ] Premium phone coaching: 30-minute call with a trained patient advocate for personalized guidance (contractor-based, not full-time employee)
- [ ] Small claims court guidance: step-by-step instructions for filing a small claims case against a provider for billing violations or failure to provide legally required financial assistance
- [ ] Employer benefit channel: white-label version offered to HR departments as an employee benefit
- [ ] Integration with patient advocacy organizations (Dollar For, Patient Advocate Foundation) for warm handoffs on complex cases
- [ ] Dental and vision debt expansion: extend the financial assistance database and negotiation scripts to dental and vision providers

## 5. Technical Architecture
- **Frontend**: React with Next.js 14 (App Router) -- chosen for server-side rendering (critical for SEO around high-intent search queries like "how to reduce medical bill" and "hospital financial assistance application"), fast page loads for users on slower mobile connections (lower-income user base), and built-in API routes. Tailwind CSS for responsive design. The app is web-first (not native mobile) because the target user base skews toward price-sensitive users who are unlikely to download a dedicated app for a one-time or short-term use case -- a mobile-responsive web app is more accessible.
- **Backend**: Node.js with Express.js on AWS Lambda -- chosen for cost efficiency (pay-per-invocation model suits a product with variable usage patterns), serverless scaling during Reddit/TikTok traffic spikes, and straightforward integration with the CMS data pipeline and OpenAI API. TypeScript throughout. Background jobs (database scraping, reminder emails) run on AWS Lambda with CloudWatch Events scheduling.
- **Database**: PostgreSQL on Supabase -- chosen for relational data integrity (users, bills, providers, applications, dispute statuses have complex relationships), strong text search capabilities (hospital name search), and Supabase's built-in auth and storage (for document uploads). The hospital financial assistance database is a critical data asset stored in PostgreSQL with full-text search indexing.
- **Key APIs**:
  - CMS (Centers for Medicare & Medicaid Services) public data -- Medicare Physician Fee Schedule and Hospital Outpatient Prospective Payment System data for price comparison (free, public data files updated annually)
  - OpenAI API (GPT-4o-mini) -- generate customized negotiation scripts, pre-fill financial assistance application content, identify billing errors from procedure codes, and produce plain-language explanations
  - Google Cloud Vision API (OCR) -- extract text from uploaded bill photos to auto-populate bill details (provider name, amount, procedure codes, dates)
  - Twilio API -- SMS reminders for application deadlines and follow-up actions
  - SendGrid API -- email delivery for reminders, progress updates, and re-engagement
  - Stripe API -- payment processing for $9.99/month subscription, $29.99 one-time purchase, and $79.99 premium tier
  - Supabase Storage -- secure storage for uploaded documents (pay stubs, tax returns, bills)
- **Hosting**: Supabase for database, auth, and storage (Pro plan, $25/month), Vercel for Next.js frontend and API routes ($20/month Pro plan), AWS Lambda for background jobs (scraping, CMS data processing, ~$20-30/month). Total infrastructure: ~$65-75/month at launch. Scales naturally with Lambda and Supabase's managed infrastructure.

## 6. Data Model

### Users
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| email | String | Unique, nullable (anonymous until signup) |
| password_hash | String | bcrypt, nullable |
| name | String | Nullable |
| household_income | Decimal | For financial assistance eligibility |
| household_size | Integer | For FPL calculation |
| zip_code | String | For geographic pricing and provider lookup |
| plan | Enum | free, paid, premium |
| stripe_customer_id | String | Nullable |
| created_at | Timestamp | |

### MedicalBills
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| provider_id | UUID | FK to Providers |
| total_amount | Decimal | Billed amount |
| amount_owed | Decimal | After insurance |
| date_of_service | Date | |
| date_received | Date | Bill date |
| status | Enum | new, analyzing, application_submitted, negotiating, resolved, in_collections |
| resolved_amount | Decimal | Nullable -- final amount after reduction |
| savings | Decimal | Calculated: amount_owed - resolved_amount |
| notes | Text | Nullable |
| bill_image_url | String | Nullable, Supabase Storage |
| created_at | Timestamp | |

### BillLineItems
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| bill_id | UUID | FK to MedicalBills |
| cpt_code | String | Procedure code |
| description | String | Procedure description |
| billed_amount | Decimal | What provider charged |
| medicare_rate | Decimal | Nullable -- looked up from CMS data |
| fair_price | Decimal | Nullable -- geographic average |
| error_flag | Enum | none, duplicate, unbundled, upcoded |
| error_explanation | String | Nullable |

### Providers
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| name | String | Hospital/provider name |
| type | Enum | non_profit, for_profit, government |
| system_name | String | Parent health system |
| address | String | |
| city | String | |
| state | String | |
| zip | String | |
| cms_provider_id | String | CMS certification number |
| has_financial_assistance | Boolean | |
| last_verified_at | Timestamp | |

### FinancialAssistancePrograms
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| provider_id | UUID | FK to Providers |
| program_name | String | e.g., "Charity Care" |
| income_threshold_fpl | Integer | % of Federal Poverty Level (e.g., 200 = 200% FPL) |
| discount_percentage | Integer | Typical discount (e.g., 100 = full write-off) |
| application_url | String | Link to application form |
| required_documents | JSONB | Array of required document types |
| application_deadline_days | Integer | Days from date of service |
| retroactive_eligible | Boolean | Can apply after collections? |
| notes | Text | Special instructions |
| last_verified_at | Timestamp | |

### ActionItems
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| bill_id | UUID | FK to MedicalBills |
| step_number | Integer | Order in action plan |
| action | String | Description of the action |
| status | Enum | pending, in_progress, completed, skipped |
| due_date | Date | Nullable |
| reminder_sent | Boolean | Default false |
| completed_at | Timestamp | Nullable |
| notes | Text | Nullable |

### GeneratedDocuments
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| bill_id | UUID | FK to MedicalBills |
| document_type | Enum | financial_assistance_app, negotiation_script, itemized_request_letter, dispute_letter, cease_desist |
| content | Text | Generated document content |
| generated_at | Timestamp | |
| file_url | String | Nullable, PDF stored in Supabase Storage |

### Relationships
- A User has many MedicalBills
- A MedicalBill belongs to one Provider and has many BillLineItems, ActionItems, and GeneratedDocuments
- A Provider has many FinancialAssistancePrograms
- BillLineItems reference CMS Medicare rate data for comparison
- ActionItems form the step-by-step guided plan for each bill

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Landing Page
The user sees a supportive, empathetic headline: "You don't have to pay that full medical bill." Below: a statistic ("79% of medical bills contain errors or are eligible for reduction") and a prominent CTA: "Analyze My Bill Free." The page tone is warm and reassuring, not corporate. Below the fold: a three-step explainer (Enter Your Bill > Get Your Action Plan > Save Money), success stories showing real savings ("Maria reduced her $6,400 ER bill to $640"), and a FAQ section addressing common fears ("Will this affect my credit?" "Is it too late if my bill is in collections?"). The page is optimized for SEO targeting "how to reduce medical bill," "hospital financial assistance application," and "negotiate medical debt."

### Screen 2: Bill Entry
The user can enter their bill in two ways. Option A: manual entry form with fields for provider/hospital name (autocomplete from the database), total bill amount, amount owed (after insurance), date of service, and procedure codes (optional, with helper text: "Find these on your itemized bill -- they look like 5-digit numbers"). Option B: upload a photo of the bill, and OCR extracts the details automatically. The user reviews and confirms the extracted data. The tone is encouraging: "You're already doing the hardest part -- starting." No account required for this step.

### Screen 3: Income and Eligibility Assessment
After entering the bill, the user is asked for household income and household size to determine financial assistance eligibility. A Federal Poverty Level (FPL) calculator runs automatically and shows: "Your household is at 180% of the Federal Poverty Level." The app then checks the provider's financial assistance policy and displays: "Good news: [Hospital Name] offers financial assistance for households up to 200% FPL. You likely qualify for a 75-100% bill reduction." A savings estimate appears in large, encouraging text: "Estimated savings: $4,800-$6,400." If the user does not qualify for financial assistance, the app pivots to negotiation strategies: "You may not qualify for charity care, but we can help you negotiate a lower rate."

### Screen 4: Action Plan
The core value screen. The user sees a step-by-step action plan customized to their situation, displayed as a vertical checklist with status indicators. Example steps: (1) Request an itemized bill [Generate Letter button], (2) Review itemized bill for errors [Upload when received], (3) Compare charges to Medicare rates [View Comparison], (4) Complete financial assistance application [Generate Application], (5) Submit application with supporting documents [Checklist of required docs], (6) Call billing department to follow up [View Script], (7) Negotiate remaining balance [View Negotiation Script], (8) Set up interest-free payment plan [View Tips]. Each step expands to show detailed instructions, estimated time, and relevant tools (letter generator, script, etc.). A progress bar shows completion percentage. This screen makes the overwhelming process feel manageable and sequential.

### Screen 5: Financial Assistance Application Generator
The user enters or confirms their income, household size, and uploads required documents (the app tells them exactly which documents this provider requires). The app generates a pre-filled financial assistance application as a downloadable PDF, formatted to match the provider's application layout. A cover letter is included, professionally written, that introduces the patient, states their financial situation, and requests consideration. The user is shown submission instructions: where to mail or fax the application, or how to submit it online. A deadline warning displays if applicable: "This hospital requires applications within 240 days of service -- you have 180 days remaining."

### Screen 6: Medicare Rate Comparison
A table showing each billed procedure alongside its Medicare reimbursement rate and the geographic fair-market price. Columns: Procedure Code, Description, Billed Amount, Medicare Rate, Fair Price (Area Average), Overcharge Amount, Overcharge Percentage. Rows are color-coded: red for overcharges exceeding 200% of Medicare, yellow for 150-200%, green for within 150%. A summary at the bottom: "Your bill is 340% of the Medicare rate for these procedures. This gives you strong negotiation leverage." A "Use This in Negotiation" button generates a customized negotiation script that references these specific overcharges.

### Screen 7: Negotiation Scripts
A library of word-for-word phone scripts organized by scenario: "Requesting Uninsured Discount," "Negotiating with Medicare Rate Comparison," "Setting Up Interest-Free Payment Plan," "Requesting Itemized Bill," "Responding to Collection Calls," "Following Up on Financial Assistance Application." Each script is a conversation guide with the caller's lines in bold and expected responses from the billing department in gray, with branching paths ("If they say X, respond with Y"). Tips are interspersed: "Stay calm and polite -- billing reps deal with frustrated callers all day. Being kind gets better results." A "Practice Mode" option reads the script aloud so the user can rehearse.

### Screen 8: Dispute and Status Tracker
A dashboard showing all the user's medical bills with their current status (new, application submitted, negotiating, resolved, in collections). Each bill card shows: provider name, original amount, current status, next action item, and due date. A timeline view shows the full history of actions taken on each bill: dates of calls, applications submitted, responses received, amounts negotiated. A notification badge appears when a deadline is approaching. Resolved bills show the final amount and total savings achieved, with a "Share Your Win" button for social sharing.

### Screen 9: Billing Error Review
After the user uploads or enters an itemized bill, this screen displays detected potential billing errors. Each flagged item shows: the procedure code, the error type (duplicate charge, unbundling, upcoding), a plain-language explanation ("This code appears twice on your bill for the same date -- this may be a duplicate charge"), and a recommended action ("Request removal of the duplicate charge -- here's a letter you can send"). Error types are explained with icons and simple definitions. Even if no errors are detected, the screen reassures: "No obvious errors found, but requesting an itemized bill is still recommended -- 30% of bills contain errors that require detailed review."

### Screen 10: Paywall / Upgrade Screen
Triggered when free users try to generate financial assistance applications, access negotiation scripts, or use the dispute tracker. The design is empathetic and avoids pressure tactics. Headline: "Get the tools to fight your medical bill." Comparison: Free (one bill analysis, financial assistance eligibility check, basic overcharge flag) vs. Navigator ($29.99 one-time: pre-filled applications, full script library, Medicare comparison, dispute tracker, reminders) vs. Full Navigator ($79.99 one-time: everything in Navigator plus 30-minute phone coaching and human application review). Social proof: "Users save an average of $3,200 -- the Navigator pays for itself." Financial hardship option: "Can't afford this right now? Email us -- we offer reduced pricing for those in financial hardship." A monthly plan option ($9.99/month) is shown for users managing multiple bills over time.

## 8. Monetization Implementation

### Paywall Placement
The free tier allows one bill analysis: upload a bill, check if the provider has a financial assistance program, and see a basic overcharge flag (whether the bill exceeds 150% of Medicare rates). This is the "aha moment" -- discovering that you might be eligible for financial assistance or that your bill is dramatically overcharged motivates action. The paywall activates when the user tries to generate a financial assistance application, access negotiation scripts, view the detailed Medicare rate comparison, or use the dispute tracker. The trigger is the transition from "understanding the problem" (free) to "taking action on the problem" (paid).

### Upgrade Triggers
- Generating a financial assistance application: "Get a pre-filled application ready to submit. Upgrade to Navigator ($29.99)." (The highest-intent moment -- the user has confirmed eligibility and wants to act)
- Viewing negotiation scripts: "See exactly what to say when you call the billing department. Upgrade to Navigator."
- After seeing the savings estimate: "You could save $4,800. The Navigator costs $29.99 -- that's a 160x return." (Explicit ROI framing)
- After 3 days without action: re-engagement email showing the user's bill amount, their eligibility status, and a reminder that the application deadline is approaching
- After a TikTok/Reddit referral landing: landing page shows the savings story that brought them, then immediately invites bill entry

### Pricing Psychology
- The $29.99 one-time price is explicitly positioned against human negotiation services: "Resolve Medical Bills and CoPatient charge 25-35% of your savings. On a $6,000 bill reduction, that's $1,500-$2,100. The Navigator is $29.99." The comparison makes $30 feel like a no-brainer.
- The $9.99/month option exists for users managing multiple bills over several months (the Patricia persona), but the one-time purchase is the default and anchor price
- The $79.99 premium tier ("Full Navigator") includes a 30-minute coaching call and human application review -- this exists to make the $29.99 tier feel like a great deal by comparison (price anchoring) and to serve users who genuinely need human help
- A financial hardship exception is offered (reduced or waived pricing upon request) -- this builds trust, aligns with the product's mission, and generates goodwill and word-of-mouth in a community that is price-sensitive

## 9. Analytics & KPIs

| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| Bills uploaded / entered | 300 | 3,000/mo | 8,000/mo |
| Financial assistance applications generated | 40 | 600/mo | 1,500/mo |
| Free-to-paid conversion rate | 12% | 18% | 20% |
| Paying users (cumulative) | 100 | 2,500 | 7,300 |
| Monthly revenue | $5,000 | $20,000 | $25,000 |
| Average bill reduction achieved (user-reported) | 40% | 50% | 55% |
| Total user-reported savings (cumulative) | $50,000 | $1,200,000 | $5,000,000 |
| Hospital database coverage (% of non-profit hospitals) | 50% | 70% | 85% |
| Referral rate (users who share the app) | 0.2 | 0.4 | 0.5 |
| Reddit/TikTok organic mentions per month | 5 | 30 | 80 |
| Healthcare social worker referral partners | 5 | 30 | 100 |
| User-reported action plan completion rate | 30% | 45% | 55% |

## 10. 12-Week Launch Plan

| Week | Milestone |
|------|-----------|
| Week 1 | Initialize Next.js project, set up Supabase (database, auth, storage), configure AWS Lambda for background jobs, set up CI/CD. Download and process CMS Medicare Physician Fee Schedule data and Hospital Outpatient data for price comparison. Design database schema for providers, financial assistance programs, bills, and action plans. |
| Week 2 | Build the hospital financial assistance database: research and enter data for the top 100 non-profit hospital systems (eligibility criteria, application URLs, required documents, deadlines). Build the Provider data model with full-text search. Set up automated scrapers for hospital financial assistance policy pages. |
| Week 3 | Build the bill entry flow: manual entry form with provider autocomplete, photo upload with OCR (Google Cloud Vision), and bill line item parsing. Build the income/eligibility assessment screen with FPL calculator and financial assistance eligibility matching. |
| Week 4 | Build the Medicare rate comparison engine: match CPT codes to CMS fee schedule data, calculate geographic adjustments, display billed vs. Medicare vs. fair-price comparison table. Build billing error detection (duplicate charges, unbundling, upcoding patterns). |
| Week 5 | Build the financial assistance application generator: create templated applications for the top 50 hospital systems, generate pre-filled PDFs with user income data, include cover letter generator (OpenAI). Build the negotiation script library with 8+ scenarios. |
| Week 6 | Build the step-by-step action plan engine: logic to generate customized action plans based on user situation (uninsured vs. underinsured, non-profit vs. for-profit provider, pre-collections vs. in-collections). Build the dispute and status tracker with reminder scheduling (Twilio SMS, SendGrid email). |
| Week 7 | Build paywall and payment system: Stripe integration for one-time purchases ($29.99, $79.99) and monthly subscription ($9.99). Build the upgrade screen with ROI framing. Implement the itemized bill request letter generator. Expand hospital database to 300+ systems. |
| Week 8 | Build the landing page optimized for SEO ("how to reduce medical bill," "hospital financial assistance," "negotiate medical debt"). Build the savings calculator for the landing page (enter bill amount, see estimated savings). Build shareable success story cards for social sharing. |
| Week 9 | Internal QA and beta testing: recruit 20-30 beta users from r/povertyfinance and r/personalfinance (users who have posted about medical debt). Test with real bills, verify financial assistance database accuracy, collect feedback on script quality and action plan usefulness. Verify that generated applications match actual provider forms. |
| Week 10 | Expand hospital database to 500+ systems. Prepare launch content: draft the "How I reduced my $8,400 ER bill to $840" Reddit post, create 3 "Did you know?" TikTok video scripts, draft emails to 50 hospital social workers and patient advocates, prepare Google Ads campaigns for high-intent keywords. |
| Week 11 | Public launch: post on r/povertyfinance and r/personalfinance with detailed medical bill reduction guide and soft app mention. Publish TikTok content. Launch Google Ads targeting "how to reduce medical bill" and "hospital financial assistance application." Email hospital social workers and Patient Advocate Foundation contacts. Offer a 50% discount for the first 100 users ($14.99 one-time). |
| Week 12 | Post-launch analysis: review conversion funnel (bill entry > eligibility check > paywall > purchase > action plan completion). Analyze which financial assistance programs users are applying to most (prioritize database accuracy for those). Collect user-reported savings data for marketing. Identify the top user-requested features. Begin outreach to medical debt Facebook groups. Set Month 2-3 targets. |

## 11. Growth Loops

### Savings Story Virality
Medical bill reduction stories are inherently viral -- "I got my $6,400 ER bill reduced to $640" is the kind of content that gets thousands of upvotes on Reddit and millions of views on TikTok. Every user who successfully reduces their bill has a story worth sharing. The app generates a shareable savings card after resolution showing original bill, final amount, and savings percentage. Each card includes a referral link. The emotional intensity of medical debt relief makes sharing feel natural and cathartic, not promotional.

### Healthcare Social Worker Distribution
Hospital social workers and patient advocates interact with patients who have medical debt every single day. By providing free app access to social workers and making the tool easy to recommend (a simple URL they can text to patients), each social worker becomes a recurring referral source. One social worker at a busy hospital might refer 5-10 patients per month. The tool supplements their guidance with self-service capabilities they do not have time to provide one-on-one.

### SEO Content Flywheel
Medical debt queries have high search volume, high intent, and relatively low competition. Content targeting keywords like "how to apply for hospital financial assistance," "negotiate medical bill script," and "medical bill too high what to do" drives free organic traffic to the tool. Each piece of content solves a specific problem and presents the app as the next step. As the content library grows and earns backlinks from healthcare publications and personal finance sites, organic traffic compounds over time.

### Retroactive Application Discovery Loop
Many users arrive thinking it is "too late" to do anything about their medical debt (especially if it is in collections). When the app shows them that retroactive financial assistance applications are possible, it creates a surprise-and-delight moment that drives sharing: "I thought my $12,000 medical debt in collections was a lost cause -- turns out I could still apply for charity care and got the whole thing written off." These stories are the most powerful organic marketing because they reach people who have given up.

## 12. Regulatory & Compliance

### Not a Debt Settlement Service
- Medical Debt Navigator is an educational tool and document generator, not a debt negotiation or debt settlement service. The app provides information, generates documents, and offers scripts -- but it does not negotiate with providers on the user's behalf. This distinction is critical because debt settlement services are regulated under the FTC's Telemarketing Sales Rule and require state licensing in many states.
- The app's terms of service must clearly state: "Medical Debt Navigator provides educational resources, document generation tools, and self-advocacy guidance. It does not negotiate debts, contact providers on your behalf, or provide legal or financial advice."
- Marketing materials must avoid language that promises specific outcomes ("We'll reduce your bill by 50%") and instead use outcome ranges with disclaimers ("Users report saving 40-80% -- results vary").

### HIPAA Considerations
- The app collects health-adjacent information (provider names, procedure codes, bill amounts) but does NOT access electronic health records, treatment notes, or diagnosis details from providers. The app is a consumer-facing tool where the user voluntarily enters their own billing data.
- Medical Debt Navigator is likely not a "covered entity" or "business associate" under HIPAA because it does not receive protected health information (PHI) from covered entities. However, as a best practice: encrypt all user data at rest and in transit, minimize data collection, and maintain a privacy policy that explains how health-related data is used.
- If the premium tier includes human coaching or application review, the coaches must be trained on handling sensitive medical billing information and should not access clinical/diagnosis details beyond what is necessary for billing assistance.

### State Consumer Protection Laws
- Some states have specific medical debt protection laws (e.g., California's SB 1061, Colorado's HB 22-1285). The app should track state-specific protections and surface relevant information based on the user's location.
- The app should not charge fees that are disproportionate to the service provided. The $29.99 pricing is defensible because it is a fixed fee for a defined toolset, not a percentage of savings.

### Data Privacy
- **CCPA/CPRA**: California users must have rights to data access, deletion, and opt-out. Given the sensitive nature of medical billing data, proactive data privacy protections are important for trust.
- **Financial data sensitivity**: Income, household size, and medical bill data are highly sensitive. Implement strict access controls, encryption at rest (AES-256), and minimize data retention (delete uploaded documents after 12 months unless the user opts to keep them).
- **Transparency**: The privacy policy must clearly explain what data is collected, how it is used, and that it is never sold to third parties. This is a community where trust is paramount -- any data privacy incident would be catastrophic to the brand.

### IRS 501(r) Regulatory Alignment
- The app's financial assistance database is based on IRS 501(r) requirements for non-profit hospitals. The app should explain this regulation to users in plain language: "Federal law requires most non-profit hospitals to offer financial assistance to patients who qualify. This is not charity -- it is your right."
- The app must accurately represent financial assistance eligibility criteria. If a user applies based on the app's guidance and is rejected because the data was outdated, trust is destroyed. Data verification cadence (quarterly for top 100 hospitals, semi-annually for others) is a compliance-critical operational task.

## 13. Risk Register

| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| Hospital financial assistance policy data goes stale, leading users to submit applications with incorrect eligibility criteria and get rejected, destroying trust | High | Critical | Build automated web scrapers for the 500 largest non-profit hospital systems' financial assistance pages. Crowdsource accuracy reports from users ("Was this policy accurate? Y/N"). Hire a part-time virtual assistant to verify top 100 hospital policies quarterly. Display "last verified" dates on all policy data. Implement a "report inaccuracy" button on every provider page. |
| Regulatory classification as a debt settlement service, requiring state licensing in multiple states | Medium | Critical | Position explicitly as an "educational tool and document generator" in all marketing, terms of service, and in-app language. Never negotiate on the user's behalf, contact providers, or handle money. Consult with a consumer protection attorney in the 5 most restrictive states (California, New York, Texas, Florida, Illinois) before launch. Carry liability insurance. |
| Users generate applications and scripts but do not follow through (do not call, do not submit), leading to poor outcomes and bad reviews that say "this didn't work" | High | High | Build a step-by-step tracker with SMS and email reminders for every pending action item. Celebrate each completed step (not just final resolution). Offer the premium tier with phone coaching for users who need hand-holding. Track action plan completion rates and proactively re-engage users who stall at specific steps. Frame success stories around the full process (not just the outcome) so users understand that effort is required. |
| Google Ads on medical debt keywords become prohibitively expensive as competitors or larger players enter the space | Medium | Medium | Invest heavily in organic SEO content (medical debt guides, financial assistance explainers, negotiation tip articles) that compound over time and do not require ongoing ad spend. Build the social worker referral channel as a free acquisition source. Optimize Reddit and TikTok organic content as primary growth channels. Monitor CPC trends and shift budget to highest-ROI channels monthly. |
| Negative press or social media backlash framing the product as "profiting from people's medical debt" or "exploiting vulnerable populations" | Medium | High | Lead with mission-driven messaging: "We believe no one should go bankrupt from a medical bill." Offer a genuine financial hardship exception (reduced or free access upon request). Keep pricing transparent and dramatically below human negotiation services. Share total user savings publicly. Donate a percentage of revenue to a medical debt charity (e.g., RIP Medical Debt) once profitable. Respond to criticism with empathy and action, not defensiveness. |
| Inaccurate billing error detection flags legitimate charges as errors, leading users to file inappropriate disputes and damaging provider relationships | Medium | Medium | Set conservative thresholds for error detection: only flag charges that match clear patterns (exact duplicate on same date, unbundling patterns documented by CMS). Display all flags as "potential errors -- verify with your itemized bill" rather than definitive statements. Include a disclaimer that error detection is a screening tool, not a diagnosis. Continuously improve detection accuracy based on user feedback on flag accuracy. |

## 14. Success Criteria

- **6-month go/no-go**: 2,500 paying users generating $20,000/month in revenue, with a free-to-paid conversion rate of 18%+, hospital financial assistance database covering 70%+ of US non-profit hospitals, user-reported average bill reduction of 50%+, total user-reported savings exceeding $1,200,000, and at least 30 healthcare social worker referral partners. If conversion is below target, investigate whether the paywall is positioned correctly (too early in the funnel kills trust; too late misses the intent window) or whether the free tier's "aha moment" (seeing eligibility and estimated savings) is sufficiently compelling.
- **12-month milestone**: 7,300 paying users generating $25,000/month in revenue, with total user-reported savings exceeding $5,000,000 (the north star marketing metric), hospital database covering 85%+ of US non-profit hospitals, action plan completion rate of 55%+, referral rate of 0.5 (each user refers 0.5 new users), and at least 3 pieces of earned media coverage (healthcare publications, personal finance outlets, or local news features covering user success stories). App mentioned in at least one patient advocacy organization's resource list. Google organic traffic exceeding 5,000 monthly visits for medical debt-related search queries.
