# Product Requirements Document: Freelancer Invoice Chaser

## 1. Executive Summary
Freelancers in the US are owed $50,000+ in unpaid invoices over their careers, with the average invoice paid 13 days late and 71% experiencing payment trouble at least once. Chasing payments is awkward, time-consuming, and emotionally draining -- most freelancers either give up or spend hours crafting polite-but-firm follow-ups. Existing invoicing tools (FreshBooks, Wave) send basic reminders but lack strategic escalation sequences, late-fee calculation, or scripts for difficult conversations. Freelancer Invoice Chaser is a laser-focused payment follow-up system: import invoices from existing tools, set automated escalation sequences (Day 1 friendly reminder through Day 30 final notice), use professional pre-written templates, calculate state-specific late fees, track client payment reliability scores, and access awkward conversation scripts and small claims court filing guides. At $6.99/month -- a fraction of FreshBooks or Bonsai -- the app targets 59M US freelancers in a $690M SAM, with the lowest marginal cost of any app idea (91% gross margin) and a clear path to $1.4M ARR by Year 3 through integration marketplace distribution on FreshBooks, QuickBooks, and Wave.

## 2. User Personas

### Persona 1: Anika, the Freelance Graphic Designer
- **Age**: 31
- **Job**: Freelance brand and web designer
- **Income**: $72,000/year from 8-12 active clients
- **Pain Points**: Currently owed $8,500 across 4 overdue invoices; dreads writing follow-up emails because they feel unprofessional and she worries about damaging client relationships; one client is 45 days late and she doesn't know whether to escalate or write it off; spends 4 hours/month on payment chasing instead of design work; uses FreshBooks for invoicing but its reminders are too generic
- **Goals**: Get paid on time without the emotional burden of chasing; have a professional, automated system that escalates appropriately; know which clients are reliable and which to avoid; recover the $8,500 she's owed right now
- **Tech Comfort**: High -- uses multiple SaaS tools daily (Figma, FreshBooks, Notion); expects modern UX and integrations

### Persona 2: Carlos, the Freelance Web Developer
- **Age**: 27
- **Job**: Freelance full-stack developer, 2 years into freelancing
- **Income**: $95,000/year from 5-8 clients
- **Pain Points**: Charges $100-150/hour but doesn't enforce late fees because he doesn't know what's legally allowed; one client owes $4,200 from 3 months ago and he's considering small claims court but doesn't know how; sends the same awkward follow-up email template he found on Google; too conflict-averse to have "the money conversation" on client calls
- **Goals**: Enforce late fees professionally and legally; have escalation handled automatically so he doesn't have to think about it; understand his options when a client truly won't pay; spend zero hours per month on collections
- **Tech Comfort**: Very high -- developer who evaluates tools on API quality and automation capability

### Persona 3: Rachel, the Small Creative Agency Owner
- **Age**: 44
- **Job**: Owner of a 3-person branding agency
- **Income**: $280,000/year agency revenue, $85,000 personal
- **Pain Points**: Managing invoices for 15-20 clients across her team; collectively owed $22,000 at any given time; different team members handle different clients so follow-up is inconsistent; needs visibility into which invoices are overdue across the whole agency; uses QuickBooks for accounting and doesn't want to switch
- **Goals**: Centralized view of all outstanding invoices with aging reports; consistent, professional follow-up process across all team members; integration with QuickBooks so she doesn't duplicate work; reduce average days-to-payment from 18 days late to under 5
- **Tech Comfort**: Moderate-high -- comfortable with business SaaS tools; values reliability over novelty

## 3. User Stories (20+)
1. As a freelancer, I want to import my invoices from FreshBooks so that I don't have to re-enter invoice data manually.
2. As a freelancer, I want to import my invoices from QuickBooks so that the app works with my existing accounting setup.
3. As a freelancer, I want to import my invoices from Wave so that I can use the escalation features without switching invoicing tools.
4. As a freelancer, I want to create invoices directly in the app so that I have a complete tracking system if I don't use another invoicing tool.
5. As a freelancer, I want to set payment terms (Net 15, Net 30, Net 45) for each client so that the app knows when invoices become overdue.
6. As a freelancer, I want automated escalation sequences that send increasingly firm reminders at Day 1, 7, 14, and 30 overdue so that I don't have to manually follow up.
7. As a freelancer, I want pre-written email templates for each escalation stage so that I don't have to craft awkward follow-up emails myself.
8. As a freelancer, I want to customize the email templates so that the tone matches my brand and client relationships.
9. As a freelancer, I want to preview each escalation email before it sends so that I can approve or adjust the message for sensitive clients.
10. As a freelancer, I want a "tone slider" (gentle to firm) for each escalation step so that I control how aggressive the follow-up feels.
11. As a freelancer, I want to pause an escalation sequence for a specific client so that I can handle delicate situations manually.
12. As a freelancer, I want a late fee calculator that uses state-specific legal maximums so that I charge late fees correctly and legally.
13. As a freelancer, I want a dashboard showing total outstanding invoices, aging report, and payment trends so that I have a clear picture of my cash flow.
14. As a freelancer, I want client payment reliability scores based on historical payment behavior so that I can identify risky clients before accepting new work.
15. As a freelancer, I want "awkward conversation" scripts for phone and video calls so that I'm prepared when email follow-ups don't work.
16. As a freelancer, I want a small claims court filing guide with state-specific procedures and limits so that I know my options for truly delinquent clients.
17. As a freelancer, I want to mark invoices as paid when payment is received so that the escalation sequence stops and my dashboard updates.
18. As a freelancer, I want to see the average days-to-payment for each client so that I can adjust payment terms for slow payers.
19. As a freelancer, I want email open tracking on escalation emails so that I know whether the client has seen my follow-up.
20. As a freelancer, I want to add custom branding (logo, colors) to my reminder emails so that they look professional and match my business identity.
21. As a freelancer, I want to receive push notifications when a client opens an escalation email so that I know they've seen it and can follow up by phone if needed.
22. As a freelancer, I want to set up SMS reminders as an alternative or supplement to email escalation so that I can reach clients who ignore email.
23. As an agency owner, I want to manage invoices for multiple team members in one account so that I have a centralized view of all outstanding payments.
24. As a freelancer, I want monthly payment analytics showing recovery rate, average days-to-payment, and revenue at risk so that I can measure the app's impact.

## 4. Feature Requirements

### MVP (v1.0) -- Must Have
- [ ] Invoice creation: create invoices in-app with client name, email, invoice number, line items, total amount, payment terms (Net 15/30/45/60), and due date
- [ ] Invoice import via CSV: upload invoices from any invoicing tool via CSV file with field mapping
- [ ] Automated escalation sequences: configurable multi-step email sequences triggered by overdue status -- default 4-step: Day 1 (friendly reminder), Day 7 (firmer follow-up), Day 14 (late fee notice), Day 30 (final notice with collections warning)
- [ ] Pre-written email templates: professionally written, psychologically effective templates for each escalation stage; fully editable by the user with merge fields (client name, invoice number, amount, due date, late fee)
- [ ] Tone slider: per-step tone control (Gentle, Professional, Firm, Direct) that adjusts template language while preserving the core message
- [ ] Email preview and approval: option to preview and manually approve each email before sending (default for first 30 days, then auto-send if user opts in)
- [ ] Late fee calculator: input state, calculate maximum allowable late fee per state law, auto-include late fee amount in escalation emails
- [ ] Invoice dashboard: total outstanding, total overdue, aging report (0-30, 30-60, 60-90, 90+ days), and total recovered this month
- [ ] Client payment reliability scores: based on historical payment behavior (average days late, number of overdue invoices, total owed), displayed as a letter grade (A through F)
- [ ] Invoice status tracking: Open, Overdue, In Escalation, Paid, Written Off -- with manual status updates and automatic status transitions based on escalation progress
- [ ] User authentication and secure client data storage
- [ ] Pause/resume escalation: one-tap pause for individual client sequences with optional resume date

### v2.0 -- Should Have
- [ ] FreshBooks integration: bi-directional sync -- import invoices and payment status from FreshBooks; update FreshBooks when payment is marked received
- [ ] QuickBooks integration: bi-directional sync for invoice import and payment status updates
- [ ] Wave integration: import invoices from Wave accounts
- [ ] Stripe integration: import invoices from Stripe billing
- [ ] "Awkward conversation" scripts: pre-written phone/video call scripts for escalating beyond email, organized by scenario (first late payment, repeat offender, large amount, relationship client)
- [ ] Small claims court guide: state-specific filing procedures, dollar limits, required documentation, timeline expectations, and template demand letters
- [ ] Email open and click tracking: know when clients open escalation emails and click payment links
- [ ] Custom branding: add logo, brand colors, and custom email signature to all escalation emails

### v3.0 -- Nice to Have
- [ ] Multi-user/agency mode: manage invoices across team members with role-based access (Owner, Admin, Member) and team-wide aging reports
- [ ] Payment analytics dashboard: recovery rate, average days-to-payment reduction, revenue at risk, and client-by-client payment trend analysis
- [ ] SMS escalation: optional SMS reminders as supplement or alternative to email, sent via Twilio
- [ ] International payment tracking: multi-currency invoice support with exchange rate display for freelancers with international clients
- [ ] AI-powered payment prediction: predict which invoices are likely to be paid late based on client history and invoice characteristics

## 5. Technical Architecture
- **Frontend**: Next.js (React) -- web application accessible from any device; SSR for fast initial loads; responsive design for desktop (primary -- freelancers manage finances at their desk) and mobile (secondary -- checking dashboard on the go); Tailwind CSS for rapid UI development
- **Backend**: Node.js with Express on Vercel Serverless Functions -- serverless architecture keeps hosting costs near-zero ($80/month at MVP scale); background job processing via Vercel Cron for scheduled escalation email delivery; JavaScript full-stack reduces complexity
- **Database**: PostgreSQL on Supabase -- relational model for invoices, clients, escalation sequences, and payment history where referential integrity is critical; Supabase provides built-in auth, real-time subscriptions (dashboard updates when payments arrive), and generous free tier
- **Key APIs**:
  - SendGrid (escalation email delivery with open/click tracking, custom branding, and deliverability optimization)
  - Twilio (SMS reminders in v3)
  - FreshBooks API (invoice import and payment status sync)
  - QuickBooks Online API (invoice import and payment status sync)
  - Wave API (invoice import)
  - Stripe API (invoice import from Stripe Billing)
  - Stripe (subscription billing for the app itself)
- **Hosting**: Vercel (frontend + serverless functions) + Supabase (database + auth) -- estimated $80/month at MVP scale; lowest infrastructure cost of all 10 app ideas; Vercel Cron for scheduled email delivery; scales cost-effectively with user growth

## 6. Data Model

### Users
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| email | String | Unique, required |
| name | String | |
| business_name | String | For email branding |
| logo_url | String | For email branding (S3) |
| brand_color | String | Hex color for emails |
| state | String | For late fee calculation |
| subscription_tier | Enum | Free, Paid, Premium |
| created_at | Timestamp | |

### Clients
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| name | String | Client/company name |
| email | String | Primary contact email |
| payment_terms | Enum | Net15, Net30, Net45, Net60 |
| reliability_score | String | A, B, C, D, F -- calculated |
| avg_days_late | Float | Historical average |
| total_invoices | Integer | Lifetime count |
| total_paid | Decimal | Lifetime paid amount |
| total_outstanding | Decimal | Currently owed |
| notes | Text | User notes about client |
| created_at | Timestamp | |

### Invoices
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| client_id | UUID | FK to Clients |
| invoice_number | String | User-defined or auto-generated |
| line_items | JSONB | Array of {description, quantity, rate, amount} |
| total_amount | Decimal | |
| currency | String | Default USD |
| issue_date | Date | |
| due_date | Date | Based on payment terms |
| status | Enum | Open, Overdue, In Escalation, Paid, Written Off |
| paid_date | Date | Nullable |
| paid_amount | Decimal | Nullable (may differ from total if partial) |
| late_fee_amount | Decimal | Calculated based on state |
| external_id | String | FreshBooks/QuickBooks/Wave ID for sync |
| source | Enum | Manual, CSV, FreshBooks, QuickBooks, Wave, Stripe |
| created_at | Timestamp | |

### Escalation Sequences
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| invoice_id | UUID | FK to Invoices |
| status | Enum | Active, Paused, Completed, Cancelled |
| current_step | Integer | 1-4 (which stage in the sequence) |
| pause_until | Date | Resume date if paused |
| started_at | Timestamp | |
| completed_at | Timestamp | |

### Escalation Steps
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| sequence_id | UUID | FK to Escalation Sequences |
| step_number | Integer | 1, 2, 3, or 4 |
| trigger_day | Integer | Days overdue to trigger (1, 7, 14, 30) |
| tone | Enum | Gentle, Professional, Firm, Direct |
| email_subject | String | Customized or from template |
| email_body | Text | Customized or from template with merge fields |
| sent_at | Timestamp | Nullable (null if not yet sent) |
| opened_at | Timestamp | Email open tracking |
| clicked_at | Timestamp | Payment link click tracking |
| status | Enum | Pending, Sent, Opened, Clicked, Skipped |

### Email Templates
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users (nullable for system defaults) |
| step_number | Integer | Which escalation step |
| tone | Enum | Gentle, Professional, Firm, Direct |
| subject_template | String | With merge fields ({client_name}, {amount}, etc.) |
| body_template | Text | With merge fields |
| is_default | Boolean | System template vs. user-customized |

**Relationships**: Users have many Clients and Invoices. Each Client has many Invoices. Each Invoice can have one Escalation Sequence. Each Escalation Sequence has 4 Escalation Steps. Users can customize Email Templates per step and tone. Client reliability scores are computed from their Invoice payment history.

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Onboarding -- Setup & First Invoice
After signup, the user sees "Let's get you paid." Step 1: Enter business name and state (for late fee calculation). Step 2: Choose how to add invoices: "Import from FreshBooks/QuickBooks" (OAuth connection), "Upload CSV," or "Create your first invoice." Step 3: If creating manually, a simple invoice form: client name, client email, invoice number, line items (description, qty, rate), payment terms dropdown, and due date. Step 4: "Set up your escalation sequence" -- a preview of the 4-step default sequence with editable tone sliders. A "Let's Chase" button activates the sequence for overdue invoices. A progress bar shows setup completion.

### Screen 2: Invoice Dashboard (Home)
The primary screen displays four summary cards at top: Total Outstanding (dollar amount across all invoices), Total Overdue (with count), Recovered This Month (payments received), and At Risk (invoices 30+ days overdue). Below, an aging report bar chart shows invoices grouped by age: Current, 1-30 Days, 31-60 Days, 61-90 Days, 90+ Days. A scrollable list of all invoices follows, each showing: client name, invoice number, amount, due date, status badge (Open/Overdue/In Escalation/Paid), and days overdue (in red for overdue). Filter tabs: All, Overdue, In Escalation, Paid. A floating "+" button allows adding a new invoice. A search bar enables finding invoices by client name or number.

### Screen 3: Invoice Detail & Escalation Timeline
Tapping an invoice opens a full detail view: client name and email, invoice number, line items, total amount, issue date, due date, payment terms, and current status. Below, an escalation timeline shows all 4 steps as a horizontal progress bar: Step 1 (Day 1), Step 2 (Day 7), Step 3 (Day 14), Step 4 (Day 30). Completed steps show a green checkmark with sent date. The current/next step is highlighted with a preview of the email to be sent. Each step has: "Preview Email" (opens full email preview), "Edit" (customize this email), "Skip" (skip this step), and tone slider. Action buttons at bottom: "Mark as Paid" (with payment date and amount entry), "Pause Sequence" (with optional resume date), "Write Off" (with reason), and "Add Late Fee."

### Screen 4: Escalation Email Preview & Editor
A full-screen email preview showing exactly what the client will receive: from address (user's business email), subject line, and email body with all merge fields populated (client name, invoice number, amount, due date, late fee if applicable). The user can edit subject and body directly in this view. A tone slider at the top adjusts the overall language (switching between template variants). A "Send Now" button sends immediately; a "Schedule" button confirms the automated send date. A "Send Test Email to Myself" button lets the user preview the email in their own inbox. Template merge fields are highlighted in blue so the user knows which parts are dynamic.

### Screen 5: Client Reliability Scorecard
A client detail page showing: client name, email, total lifetime invoices, total paid, total outstanding, average days to payment, and a large reliability grade (A through F) with a color indicator (green A, red F). A history section lists all invoices for this client with date, amount, days to payment, and status. A trend line shows whether this client's payment behavior is improving or worsening. Notes field for the user to add context. An "Escalation History" section shows all past escalation sequences for this client. A warning banner appears for D/F clients: "This client has a pattern of late payment. Consider requiring upfront payment or shorter payment terms."

### Screen 6: Late Fee Calculator
A utility screen where the user selects their state from a dropdown. The app displays: maximum allowable late fee percentage, maximum flat fee, and any state-specific restrictions. The user enters the invoice amount and days overdue, and the calculator shows the legal late fee amount. A "Copy Late Fee Language" button provides a ready-to-paste clause for contracts and invoices. A note explains: "Late fee laws vary by state. This calculator provides general guidance -- consult a local attorney for specific situations." An "Apply to Invoice" button adds the calculated late fee to the selected invoice and includes it in the next escalation email.

### Screen 7: Awkward Conversation Scripts
A categorized library of phone and video call scripts organized by scenario: "First Late Payment" (diplomatic, assumes good faith), "Repeat Offender" (firmer, references pattern), "Large Invoice" ($5,000+, more formal), "Relationship Client" (warm but clear), "Final Warning Before Collections/Legal" (professional, documents intent). Each script includes: suggested opening line, key talking points, responses to common objections ("I'll pay next week" / "I never received the invoice" / "We're having cash flow issues"), and a suggested closing with next steps. Scripts are printable or shareable to email for pre-call preparation.

### Screen 8: Small Claims Court Guide
A state-specific reference screen: user selects their state and sees the small claims dollar limit, filing fee, required forms, typical timeline, and step-by-step filing instructions. A "Demand Letter Template" provides a formal pre-litigation letter that must be sent before filing in most jurisdictions. A checklist covers required documentation (signed contract, invoice copies, escalation email records, proof of delivery). A disclaimer reads: "This guide is informational and does not constitute legal advice. Consult an attorney for your specific situation." A "Download Guide as PDF" button saves the state-specific information for offline reference.

### Screen 9: Payment Analytics (Premium)
A comprehensive analytics dashboard showing: recovery rate (percentage of overdue invoices eventually paid after escalation), average days-to-payment before vs. after using the app, total revenue recovered, revenue at risk (outstanding 60+ days), and client reliability distribution (pie chart of A/B/C/D/F clients). Monthly trends for invoices sent, invoices paid, and invoices overdue. A "Top Delinquent Clients" table lists the worst offenders by total outstanding. An ROI calculator shows "The app has helped you recover $X, which is Y times your subscription cost."

### Screen 10: Settings & Subscription
User profile (name, business name, email, state), email branding settings (logo upload, brand color picker, custom email signature), default escalation sequence configuration (customize the default 4-step timing and tone for new invoices), integration connections (FreshBooks, QuickBooks, Wave, Stripe -- connect/disconnect with sync status), notification preferences (email and push notifications for payment received, escalation sent, email opened, weekly summary), and subscription management (current plan, upgrade/downgrade, billing history). A "Default Payment Terms" selector sets the default for new clients. An "Export Data" button downloads all invoice and payment data as CSV.

## 8. Monetization Implementation

### Paywall Placement
The free tier allows 3 active clients, manual reminder sending (pre-written templates provided but sent manually), basic invoice tracking, and an aging report. The paywall activates when the user attempts to: (a) add a 4th client, (b) enable automated escalation sequences, (c) access the late fee calculator, (d) view client reliability scores, or (e) use custom branding on emails.

### Upgrade Triggers
- **Overdue invoice urgency**: When a user has an overdue invoice and hasn't sent a reminder, prompt: "Invoice #1042 is 5 days overdue. Upgrade to activate automatic escalation -- the right email goes out at the right time without you lifting a finger."
- **Recovery ROI**: After the first manual reminder leads to payment, show: "You just recovered $2,500. Automate this for all your invoices for $6.99/month -- one recovered invoice pays for 6 years of the app."
- **Client count growth**: When the user adds their 4th client, prompt: "You're growing! Upgrade to unlimited clients and never lose track of a payment again."

### Pricing Psychology
- Monthly ($6.99) and annual ($59.99, saving 29%) options with annual pre-selected.
- "One recovered invoice pays for 6 years of the app" -- the ROI is irresistible.
- 14-day free trial of full automation features to demonstrate the relief of hands-off escalation.
- "Pay from recovered invoice" psychology: first month free, charged only after the app helps recover a payment (honor system, builds goodwill).
- Agency tier ($14.99/month) positioned as: "One late invoice covers your team's annual subscription."

## 9. Analytics & KPIs

| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| Total Registered Users | 1,000 | 12,000 | 25,000 |
| Paid Subscribers | 40 | 600 | 1,650 |
| Free-to-Paid Conversion Rate | 4% | 6% | 8% |
| Monthly Recurring Revenue (MRR) | $280 | $4,200 | $11,550 |
| Invoices Tracked (Total) | 500 | 15,000 | 50,000 |
| Recovery Rate (% overdue paid after escalation) | 50% | 60% | 65% |
| Average Days-to-Payment Reduction | 3 days | 6 days | 8 days |
| Escalation Emails Sent / Month | 200 | 8,000 | 25,000 |
| Active Escalation Sequences | 100 | 3,000 | 10,000 |
| Client Reliability Scores Viewed / Month | 50 | 1,500 | 5,000 |
| Monthly Churn Rate | 10% | 8% | 7% |

## 10. 12-Week Launch Plan

| Week | Milestone |
|------|-----------|
| 1 | Finalize tech stack; set up Next.js project, Supabase database with auth, Vercel deployment, and CI/CD pipeline; secure SendGrid API key; begin email template copywriting |
| 2 | Build user authentication, onboarding flow (business name, state, import method selection), and manual invoice creation form (client, line items, payment terms, due date) |
| 3 | Build invoice dashboard: summary cards (outstanding, overdue, recovered), aging report chart, invoice list with status badges, filter tabs, and search |
| 4 | Write all escalation email templates: 4 steps x 4 tones = 16 template variations; craft with professional copywriter input; test tone calibration with freelancer beta readers |
| 5 | Build escalation sequence engine: automated scheduling via Vercel Cron, SendGrid email delivery, step progression logic, pause/resume functionality, and email preview/approval flow |
| 6 | Implement tone slider UI, email template editor with merge field highlighting, "Send Test Email to Myself" function, and invoice detail view with escalation timeline |
| 7 | Build late fee calculator (state-specific data for all 50 states), client reliability scoring engine (letter grades based on payment history), and client detail/scorecard screen |
| 8 | Build CSV invoice import with field mapping, Stripe subscription paywall, free tier limits, settings screen, and email branding (logo upload, color picker) |
| 9 | Build "awkward conversation" scripts library and small claims court guide (state-specific data for top 10 states by freelancer population); implement email open tracking via SendGrid webhooks |
| 10 | Alpha testing with 15 freelancers recruited from r/freelance and r/graphic_design: test escalation email quality, automation reliability, late fee accuracy, and dashboard UX; fix critical bugs |
| 11 | Beta launch: invite 75 freelancers; iterate on top feedback (email tone calibration, approval flow UX, client scoring accuracy); begin FreshBooks API integration development; prepare Product Hunt launch assets |
| 12 | Public launch: post "My automated follow-up system that recovered $12K in overdue invoices" on r/freelance; write viral Twitter thread with escalation email templates; launch on Product Hunt (Tuesday); send launch email to beta waitlist; list on FreshBooks App Store as "payment follow-up add-on"; begin LinkedIn/Instagram ads targeting "freelancer" interests |

## 11. Growth Loops

### Integration Marketplace Distribution
Listing on the FreshBooks App Store, QuickBooks App Store, and Wave marketplace places the app directly in front of users who already have the payment problem and are actively searching for solutions. Each marketplace listing is a perpetual distribution channel that requires no ongoing marketing spend. Users searching for "payment follow-up" or "invoice reminders" in these marketplaces are the highest-intent leads possible.

### "I Got Paid" Sharing Loop
When a user marks an invoice as paid after an escalation sequence, they see a "You recovered $X,XXX!" celebration screen with a "Share" button. The shareable graphic reads "I recovered $X,XXX in overdue invoices with Freelancer Invoice Chaser" -- designed for Twitter/X, LinkedIn, and freelancer communities. Freelancers love sharing wins, and payment recovery stories are among the most engaged content in freelancer communities.

### Template Virality
The escalation email templates are inherently shareable content. A Twitter/X thread revealing "The exact 4 emails I send when clients don't pay" drives massive engagement (freelancers love tactical advice). The thread shares the templates word-for-word, building trust and awareness, with a CTA: "I automated these into an app so I never have to think about it." This content format is re-usable across Reddit, LinkedIn, and newsletters.

### Referral Program
Every escalation email includes a subtle, tasteful footer: "Payment tracking powered by Freelancer Invoice Chaser" (customizable/removable by the user). When freelancers refer other freelancers, both receive a free month. In freelancer communities, "this tool got me paid" recommendations carry enormous credibility.

### Client Score Network Effect
As more freelancers use the app, client reliability data becomes more valuable. A future feature could aggregate anonymized client payment behavior across multiple freelancers (with consent), creating a "client reputation" system that becomes more accurate with scale -- a powerful network effect that makes the tool more valuable as it grows.

## 12. Regulatory & Compliance

- **CAN-SPAM Compliance**: All escalation emails sent on behalf of users must comply with CAN-SPAM Act requirements: include the user's physical business address, provide an unsubscribe mechanism for the email recipient (the client), and honor opt-out requests within 10 business days. Note: payment reminder emails to existing business contacts are generally not considered marketing under CAN-SPAM, but best practices should still be followed.
- **State Late Fee Laws**: Late fee calculations must accurately reflect state-specific maximums. Laws vary significantly: some states cap late fees as a percentage (1-2% per month), others set flat-dollar maximums, and some prohibit late fees entirely without contractual agreement. The calculator must cite the relevant state statute and include a disclaimer that it provides general guidance, not legal advice.
- **Debt Collection Laws (FDCPA)**: While freelancers sending their own invoice reminders are generally not subject to the Fair Debt Collection Practices Act (which applies to third-party debt collectors), the app must not position itself as a collection agency. Language must be carefully framed as "your reminders" not "our collection actions." If the app ever sends emails on behalf of users in a way that could be construed as third-party collection, FDCPA compliance becomes mandatory.
- **Data Privacy**: CCPA, VCDPA, and other state privacy laws apply. Client contact information (names, emails) is personal data that must be protected. Encrypt all data at rest and in transit. Provide data access, export, and deletion requests honored within 30 days. Do not sell or share client data. Privacy policy must clearly explain how client data is used.
- **Email Deliverability**: Escalation emails sent via SendGrid must maintain high deliverability. Implement DKIM, SPF, and DMARC authentication. Monitor bounce rates and spam complaints. If SendGrid deliverability degrades, escalation fails silently and users lose trust. Maintain sender reputation through proper list hygiene and complaint handling.
- **Unauthorized Practice of Law**: The small claims court guide and late fee calculator provide informational guidance, not legal advice. Prominent disclaimers must be displayed. The demand letter template must be labeled as a "sample" and include a recommendation to consult an attorney. Do not provide advice on specific legal situations.

## 13. Risk Register

| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| FreshBooks, QuickBooks, or Wave add smart escalation sequences natively, eliminating the integration distribution channel | Medium | High | Go deeper than invoicing platforms with client reliability scores, awkward conversation scripts, small claims guidance, and cross-platform tracking (invoices from multiple tools in one dashboard); position as the specialist "collections layer" that sits on top of any invoicing tool; build switching costs through escalation history and client data |
| Freelancers find automated emails too aggressive, damaging client relationships, leading to blame and churn | Medium | High | Default to manual email approval for the first 30 days (user previews and approves each email before sending); provide a tone slider from gentle to firm; include a prominent "Pause Sequence" button for sensitive clients; let users preview the full escalation sequence before activating; offer a "relationship mode" that uses softer language |
| Low willingness to pay among cash-strapped freelancers who struggle with late payments | Medium | Medium | Emphasize ROI: "One recovered $500 invoice pays for 6 years of the app"; offer "pay from recovered invoice" option (first month free, charged after recovery); annual plan discount ($59/year = $4.92/month); student/new freelancer discount; 14-day free trial of automation features |
| Escalation emails get caught in spam filters, causing silent failure and user distrust | Medium | High | Use SendGrid's enterprise-grade deliverability with DKIM, SPF, DMARC authentication; monitor bounce rates and spam complaints proactively; implement email delivery confirmation and retry logic; alert users when an email fails to deliver; provide "send from your own email" option as fallback |
| Email open/click tracking blocked by email privacy features (Apple Mail Privacy Protection, Gmail proxy) | High | Low | Treat open tracking as a supplementary signal, not a core feature; clearly label tracked data as "approximate"; focus product value on the escalation automation and templates, not on tracking; use payment receipt (the actual goal) as the definitive success metric |
| Legal liability from inaccurate late fee calculations or small claims guidance that leads to a user's financial or legal harm | Low | High | Cite specific state statutes in the late fee calculator; add prominent disclaimers that all information is general guidance, not legal advice; recommend consulting an attorney for specific situations; carry errors and omissions insurance; have state-specific legal data reviewed by a legal professional before launch |

## 14. Success Criteria
- **6-month go/no-go**: 600+ paid subscribers, 8%+ free-to-paid conversion rate, $4,200+ MRR, 60%+ recovery rate (overdue invoices paid after escalation), average days-to-payment reduced by 6+ days, and at least one integration marketplace listing live (FreshBooks or QuickBooks App Store)
- **12-month milestone**: 1,650+ paid subscribers, $11,550+ MRR, <7% monthly churn, 65%+ recovery rate, FreshBooks and QuickBooks integrations live with positive marketplace reviews, successful Product Hunt launch with 200+ upvotes, and freelancer community recognition (featured in at least 2 freelancer newsletters or podcasts)
