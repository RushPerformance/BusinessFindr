# Product Requirements Document: HOA Simplified

## 1. Executive Summary
60% of the 365,000 HOAs in the US are managed by volunteer board members using a chaotic mix of Venmo, spreadsheets, email chains, and filing cabinets — while professional HOA software costs $200-500/month and is designed for management companies, not volunteers. HOA Simplified is a lightweight, all-in-one management tool for small HOAs and condo associations (20-200 units) that handles dues collection via Stripe, violation tracking, document storage, resident communication, maintenance requests, and basic budgeting — all for a flat $29.99/month per community. The target customer is a volunteer board member aged 45-65 who is overwhelmed, not tech-savvy, and spending 10+ hours/month on administrative chaos. At $30/month with 30-month average retention and 20:1 LTV:CAC, this is a high-margin, low-churn B2B SaaS product. Year 1 revenue target is $180K from 500 communities, driven by Reddit/Facebook community outreach, direct mail to small HOAs identified through county records, and attendance at Community Associations Institute regional events.

## 2. User Personas

### Persona 1: Diane Crawford
- **Age**: 58
- **Job**: Retired school administrator; serves as HOA board president for a 65-unit townhome community
- **Income**: $72,000/year (pension + investments)
- **Pain Points**: Collects dues via Venmo and personal checks; tracks finances in an Excel spreadsheet that only she understands; sends community updates via a Yahoo email list that half the residents don't read; spends 12+ hours/month on HOA tasks she volunteered for; has no system for tracking violation complaints
- **Goals**: Get a single tool that handles dues collection, communications, and document storage; reduce her time commitment to 3-4 hours/month; make the treasurer role transferable when she steps down
- **Tech Comfort**: Low-moderate — uses email and basic Office tools; intimidated by complex software; needs a guided setup process

### Persona 2: Kevin Park
- **Age**: 39
- **Job**: Software engineer; newly elected HOA board treasurer for a 110-unit condo association
- **Income**: $135,000/year
- **Pain Points**: Inherited a mess — the previous treasurer kept all records on paper; Venmo dues collection makes reconciliation impossible; half the residents pay late because there's no automated reminder system; the board spends 45 minutes per meeting arguing about who paid and who didn't
- **Goals**: Set up online dues payment with automated reminders; get a real-time view of who's paid and who hasn't; automate financial reporting so board meetings focus on decisions, not bookkeeping
- **Tech Comfort**: High — comfortable with any software; wants something that works well, not just something that exists

### Persona 3: Alicia Fernandez
- **Age**: 47
- **Job**: Marketing manager; HOA board secretary for a 35-unit garden-style condo community
- **Income**: $68,000/year
- **Pain Points**: Responsible for meeting minutes, CC&R document access, and resident communications; stores documents on a shared Google Drive that's disorganized and missing key files; residents constantly ask for copies of the CC&Rs or parking rules; violation complaints come via text, email, and in-person and there's no tracking
- **Goals**: Have one place for all community documents that residents can access themselves; track violations from complaint through resolution; send announcements that actually reach everyone
- **Tech Comfort**: Moderate — uses marketing tools at work; comfortable learning new software if it saves time

## 3. User Stories (20+)
1. As a board member, I want to set up my community with unit numbers, owner names, and dues schedule so that the system knows who owes what and when.
2. As a board member, I want residents to pay dues online via ACH or credit card so that I stop collecting Venmo payments and personal checks.
3. As a board member, I want automated late payment reminders sent to residents who haven't paid by the due date so that I don't have to chase people manually.
4. As a board member, I want a real-time dashboard showing who has paid, who is late, and total collected vs. expected so that I can report to the board instantly.
5. As a board member, I want to log a violation with the unit number, type, description, and photo so that there's a formal record.
6. As a board member, I want to send violation notices to residents via email directly from the app so that communication is documented.
7. As a board member, I want to track violation status (reported, notice sent, resolved, escalated) so that nothing falls through the cracks.
8. As a board member, I want to upload and organize community documents (CC&Rs, bylaws, meeting minutes, financial reports) so that everything is in one place.
9. As a resident, I want to access community documents without having to ask the board so that I can find what I need immediately.
10. As a board member, I want to post announcements that go to all residents via email and in-app notification so that I stop managing email chains.
11. As a resident, I want to submit a maintenance request with a description and photo so that the board knows about issues promptly.
12. As a board member, I want to track maintenance requests from submission through resolution so that I can manage vendor assignments and timelines.
13. As a board member, I want a simple annual budget tool to track HOA income and expenses so that I can produce basic financial reports.
14. As a board member, I want to generate a monthly or quarterly financial summary so that I can present it at board meetings without manual spreadsheet work.
15. As a board member, I want to create a board meeting agenda and take minutes in the app so that meeting records are organized and accessible.
16. As a resident, I want to see my payment history and current balance so that I know I'm in good standing.
17. As a board member, I want to set different dues amounts for different unit types (1BR vs. 2BR, or by square footage) so that billing is accurate.
18. As a board member, I want to apply late fees automatically after a grace period so that the policy is enforced consistently.
19. As a board member, I want to invite other board members with appropriate role permissions (admin, treasurer, secretary) so that we can share the workload.
20. As a board member, I want to export financial data as CSV or PDF so that I can share it with the community's CPA or bank.
21. As a board member, I want to send targeted communications to specific units or groups (e.g., all units in Building A) so that messages are relevant.
22. As a resident, I want to update my contact information (email, phone) so that I receive community communications.
23. As a board member, I want to see a history of all communications sent to a specific unit so that I have a complete record for disputes.
24. As a board member, I want to set up one-time special assessments in addition to regular dues so that unexpected costs can be collected efficiently.

## 4. Feature Requirements

### MVP (v1.0) — Must Have
- [ ] Community setup wizard: add community name, address, number of units; import unit list via CSV or manual entry; set dues schedule (monthly, quarterly, annual) and amounts (support variable amounts by unit type)
- [ ] Online dues payment: ACH and credit card payments via Stripe Connect (funds go directly to HOA bank account, never through HOA Simplified's account); residents receive email invoice with a payment link
- [ ] Automated payment reminders: configurable email reminders sent X days before due date, on due date, and X days after (for late payments); customizable reminder text
- [ ] Payment dashboard: real-time view showing all units, payment status (paid, pending, late, partial), amount owed, and date paid; filterable by status; displays total collected vs. total expected
- [ ] Late fee automation: configurable late fee (flat amount or percentage) applied automatically after a grace period set by the board
- [ ] Violation tracking: create a violation record with unit number, violation type (dropdown: parking, noise, landscaping, exterior modification, pet, trash, other), description, photo upload, and date; assign status (reported, notice sent, follow-up, resolved, escalated)
- [ ] Violation notice delivery: send violation notice to the resident via email directly from the app; notice includes violation details, relevant CC&R reference, and requested action; all communications logged
- [ ] Document library: upload, categorize, and store community documents (CC&Rs, bylaws, rules & regulations, meeting minutes, financial reports, insurance certificates) with up to 2GB storage; residents can browse and download
- [ ] Announcement board: create and send community-wide announcements via email and in-app feed; support for text, images, and file attachments
- [ ] Resident portal: each resident has a login to view their payment history, current balance, community documents, announcements, and submit maintenance requests
- [ ] Board member roles: invite other board members with role-based permissions (admin has full access, treasurer sees finances, secretary manages documents and minutes)
- [ ] Mobile-responsive web app: fully functional on mobile browsers for both board members and residents

### v2.0 — Should Have
- [ ] Maintenance request portal: residents submit requests with description, category (plumbing, electrical, exterior, common area, landscaping), photo, and urgency level; board members assign to vendors, track status, and mark resolved
- [ ] Budget tool: simple income/expense tracker for the HOA's annual budget; categorized expenses (landscaping, insurance, utilities, maintenance, legal, reserves); monthly actual vs. budget comparison
- [ ] Financial reporting: auto-generated monthly and quarterly financial summaries; income statement and balance sheet; exportable as PDF
- [ ] Board meeting management: create meeting agendas from templates; take minutes in the app; attach minutes to document library automatically; track action items from meetings
- [ ] Special assessments: create one-time assessments with custom amounts, due dates, and payment tracking separate from regular dues
- [ ] SMS notifications: option for residents to receive payment reminders and urgent announcements via SMS (Twilio integration)
- [ ] Resident directory: opt-in directory of resident names and contact info for community building
- [ ] Payment reconciliation reports: detailed reports matching Stripe payouts to expected dues, downloadable for the HOA's accountant

### v3.0 — Nice to Have
- [ ] Reserve fund projections: model the HOA's reserve fund growth over 5-20 years based on current contributions, planned expenditures, and interest; assist with reserve studies
- [ ] Vendor marketplace: connect HOAs with vetted local vendors (landscaping, painting, cleaning, legal) with request-for-quote functionality
- [ ] Multi-community management: dashboard for property management companies overseeing 5+ communities; bulk onboarding and consolidated reporting
- [ ] Resident voting: online voting for board elections and community decisions with verifiable results
- [ ] Architectural review workflow: residents submit exterior modification requests with plans and photos; board members review, approve/deny, and track compliance

## 5. Technical Architecture
- **Frontend**: Next.js 14 (React) — server-side rendering for fast initial page loads (important for non-technical users who will abandon slow pages); React for interactive dashboards (payment tracking, violation management); web-based approach avoids App Store complexity and allows instant updates; mobile-responsive design serves both desktop board members and mobile residents
- **Backend**: Next.js API Routes + Node.js — unified stack for simplicity as a solo dev; serverless deployment handles variable load (payment processing spikes on the 1st of each month); TypeScript throughout for type safety on financial data
- **Database**: PostgreSQL (via Supabase) — relational model is essential for the structured, interconnected data (communities, units, residents, payments, violations, documents); row-level security ensures residents can only see their own payment data; Supabase provides built-in auth, file storage, and real-time subscriptions (useful for live payment status updates)
- **Key APIs**:
  - Stripe Connect API — payment processing for dues collection; funds route directly to the HOA's bank account via Stripe Connect; handles ACH, credit card, and automatic invoicing
  - Twilio API (v2) — SMS notifications for payment reminders and urgent announcements
  - SendGrid API — transactional email for payment reminders, violation notices, and announcements
  - Supabase Storage — document library storage (CC&Rs, bylaws, meeting minutes)
  - Supabase Auth — authentication for board members and residents with role-based access control
- **Hosting**: Vercel (frontend + API routes) + Supabase (database + storage + auth) — estimated $120/month at launch; Vercel handles frontend and serverless API routes; Supabase handles all data, file storage, and auth; predictable pricing scales with number of communities

## 6. Data Model

### Communities
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| name | String | Community name |
| address | String | Community address |
| total_units | Integer | Number of units |
| dues_frequency | Enum | monthly, quarterly, annual |
| default_dues_amount | Decimal | Standard dues amount |
| late_fee_amount | Decimal | Late fee (flat or percentage) |
| late_fee_type | Enum | flat, percentage |
| grace_period_days | Integer | Days after due date before late fee |
| stripe_account_id | String | Stripe Connect account for this community |
| subscription_status | Enum | free, standard, premium |
| created_at | Timestamp | Community creation date |

### Units
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| community_id | UUID | FK to Communities |
| unit_number | String | Unit identifier (e.g., "101," "A-3") |
| unit_type | String | Type (e.g., "1BR," "2BR," "Townhouse") |
| square_footage | Integer | Unit size (optional, for variable dues) |
| dues_amount | Decimal | Dues for this specific unit (overrides community default if set) |

### Residents
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| unit_id | UUID | FK to Units |
| email | String | Primary contact email |
| name | String | Resident name |
| phone | String | Phone number (optional) |
| role | Enum | owner, tenant, board_admin, board_treasurer, board_secretary |
| is_active | Boolean | Current resident flag |
| created_at | Timestamp | When added |

### Payments
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| unit_id | UUID | FK to Units |
| community_id | UUID | FK to Communities |
| amount | Decimal | Amount paid |
| due_date | Date | When the payment was due |
| paid_date | Date | When payment was received (null if unpaid) |
| status | Enum | pending, paid, late, partial, waived |
| payment_method | Enum | ach, credit_card, check, cash, other |
| stripe_payment_id | String | Stripe payment reference |
| late_fee_applied | Decimal | Late fee amount (if applicable) |
| period_label | String | Billing period (e.g., "March 2026") |

### Violations
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| community_id | UUID | FK to Communities |
| unit_id | UUID | FK to Units |
| type | Enum | parking, noise, landscaping, exterior_modification, pet, trash, other |
| description | Text | Violation details |
| photo_urls | Array[String] | Uploaded evidence photos |
| status | Enum | reported, notice_sent, follow_up, resolved, escalated |
| reported_date | Date | When the violation was reported |
| resolved_date | Date | When resolved (null if open) |
| notices_sent | Array[JSON] | Log of notices with dates and content |

### Documents
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| community_id | UUID | FK to Communities |
| name | String | Document name |
| category | Enum | ccrs, bylaws, rules, meeting_minutes, financial_report, insurance, other |
| file_url | String | Supabase Storage URL |
| uploaded_by | UUID | FK to Residents |
| uploaded_at | Timestamp | Upload date |

### Announcements
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| community_id | UUID | FK to Communities |
| title | String | Announcement headline |
| body | Text | Full announcement text |
| author_id | UUID | FK to Residents (board member) |
| attachment_urls | Array[String] | Attached files |
| sent_via | Array[Enum] | email, in_app, sms |
| created_at | Timestamp | When posted |

### MaintenanceRequests
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| community_id | UUID | FK to Communities |
| unit_id | UUID | FK to Units (nullable for common area requests) |
| submitted_by | UUID | FK to Residents |
| category | Enum | plumbing, electrical, exterior, common_area, landscaping, other |
| description | Text | Issue description |
| photo_urls | Array[String] | Uploaded photos |
| urgency | Enum | low, medium, high, emergency |
| status | Enum | submitted, in_progress, vendor_assigned, completed |
| assigned_vendor | String | Vendor name (if assigned) |
| submitted_at | Timestamp | When submitted |
| resolved_at | Timestamp | When completed |

**Relationships**: A Community has many Units, Violations, Documents, Announcements, and MaintenanceRequests. Each Unit has one or more Residents. Each Unit has many Payments. Violations reference both Community and Unit. Payments reference both Unit and Community. Board members are Residents with elevated roles.

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Community Setup Wizard
A guided 4-step onboarding for new board members. Step 1: "Name your community" — community name and address fields. Step 2: "Add your units" — option to upload a CSV (with a template download link) or manually add units one-by-one with unit number, type, and owner name/email. Step 3: "Set your dues" — choose frequency (monthly/quarterly/annual), set the default amount, configure late fees (amount, grace period). Step 4: "Connect your bank" — Stripe Connect onboarding flow to link the HOA's bank account for receiving payments. A progress bar and friendly copy ("You're 75% done — this is easier than a board meeting!") guides the non-technical user.

### Screen 2: Board Dashboard (Home Screen)
The command center for board members. Top row shows 4 summary cards: "Dues Collected This Month" ($X of $Y, with percentage bar), "Open Violations" (count with red/yellow/green indicator), "Pending Maintenance Requests" (count), and "Recent Announcements" (count with latest headline). Below: a "Needs Attention" section listing overdue payments, unresolved violations, and unanswered maintenance requests — each with a quick-action button. Left sidebar navigation: Dashboard, Payments, Violations, Documents, Announcements, Maintenance, Budget, Settings.

### Screen 3: Payment Management
A table view showing all units with columns: Unit #, Owner Name, Amount Due, Due Date, Status (color-coded badge: green=paid, yellow=pending, red=late), Date Paid, and Payment Method. Filters at the top: All, Paid, Pending, Late. A "Send Reminder" button appears next to each unpaid unit. Bulk actions: "Send All Reminders" and "Apply Late Fees." A summary bar at the top shows: Total Expected, Total Collected, Total Outstanding, and Collection Rate (%). Export button for CSV/PDF.

### Screen 4: Resident Payment Portal
What residents see when they log in. Top card: "Your Current Balance: $X" with a large "Pay Now" button that opens the Stripe payment form (ACH or credit card). Below: "Payment History" showing a chronological list of past payments with date, amount, method, and receipt download link. A "Next Due Date" card shows the upcoming payment deadline and amount. If the resident is late, a prominent alert bar shows the overdue amount plus any late fees.

### Screen 5: Violation Management
A list/card view of all violations, sortable by status, date, or unit. Each violation card shows: unit number, type (with icon), description snippet, photo thumbnail, status badge, and date reported. Tapping a violation opens a detail view with the full description, all photos, the communication history (notices sent with dates and content), and action buttons: "Send Notice," "Add Follow-Up Note," "Mark Resolved," or "Escalate." A "New Violation" floating action button opens the creation form.

### Screen 6: Document Library
A file cabinet interface organized by category tabs: CC&Rs, Bylaws, Rules & Regulations, Meeting Minutes, Financial Reports, Insurance, Other. Each category shows documents as a list with name, upload date, and file size. Board members see an "Upload" button within each category. A search bar at the top allows finding documents by name. Residents see the same interface but without upload capabilities. A "Most Accessed" section highlights frequently downloaded documents.

### Screen 7: Announcement Composer
A rich-text editor for creating community announcements. Fields include: Title, Body (with formatting toolbar: bold, italic, bullet lists, links), and Attachments (file upload). Distribution options: checkboxes for "Send via Email," "Post to In-App Feed," and "Send via SMS" (v2). A "Preview" button shows how the announcement will appear to residents. A "Send to:" selector allows targeting all residents or specific buildings/groups. After sending, a confirmation shows the delivery count.

### Screen 8: Maintenance Request View (Board Side)
A kanban-style board with columns: Submitted, In Progress, Vendor Assigned, Completed. Each card shows: unit number (or "Common Area"), category icon, description snippet, urgency badge (green/yellow/red), and submission date. Dragging a card between columns updates the status. Tapping a card shows: full description, photos, submitter contact info, and action fields (assign vendor, add notes, mark complete). A timeline shows the history of status changes.

### Screen 9: Budget Overview
A simple financial dashboard. Top section: "Annual Budget" showing total budgeted income (dues) vs. actual income collected, and total budgeted expenses vs. actual expenses. A bar chart compares budget vs. actual by month. Below: an expense category breakdown (landscaping, insurance, utilities, maintenance, legal, reserves) with budgeted vs. actual for each. An "Add Expense" button allows logging individual expenses. A "Generate Report" button creates a downloadable PDF financial summary.

### Screen 10: Resident Maintenance Request Submission
A simple form for residents to report issues. Fields: Category (dropdown: plumbing, electrical, exterior, common area, landscaping, other), Location (unit number auto-filled or "Common Area" option), Description (text area), Urgency (low, medium, high, emergency), and Photo Upload (camera or gallery). After submission, a confirmation screen shows: "Your request has been submitted. The board will respond within [X business days]." The resident can view their submitted requests and track status from their portal.

## 8. Monetization Implementation

**Paywall Placement**: The free tier supports communities up to 10 units with basic announcements and document storage (500MB). This is deliberately limited to serve only the smallest communities (or to let larger communities trial the product). The paywall sits at the unit limit: communities with 11+ units must upgrade to the $29.99/month plan to add more units and access online dues payment, violation tracking, and all other features.

**Upgrade Triggers**:
- When a board member tries to add the 11th unit: "Your community has grown beyond the free tier. Upgrade to manage all [X] units — $29.99/month."
- When a board member looks for payment collection: "Stop chasing Venmo payments. Upgrade to collect dues online with automated reminders."
- During free trial exploration: a "Premium Feature" badge appears on Payments, Violations, and Budget sections in the sidebar with a single-click upgrade path.

**Pricing Psychology**:
- $29.99/month is anchored against professional management companies ($200-500/month) and even PayHOA ($0.50-$1.50/unit/month, which costs $50-$150/month for a 100-unit community). The flat rate is simpler and cheaper.
- The flat rate means the per-unit cost decreases as the community grows: $1.50/unit for a 20-unit community, $0.30/unit for a 100-unit community. This makes the value proposition stronger for larger communities.
- The premium tier ($59.99/month) is positioned for boards that want meeting management, automated financial reporting, and reserve fund projections — features that replace even more manual work.
- HOA dues are community funds, not personal money, which reduces price sensitivity. A $30/month tool that saves the board 10+ hours/month is an easy approval.
- Payment processing fees (Stripe's 2.9% + $0.30 for cards, 0.8% for ACH) are passed through to the community or absorbed into dues — this is standard in HOA software.

## 9. Analytics & KPIs
| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| Communities Signed Up | 15 | 200 | 500 |
| Paid Communities | 5 | 150 | 400 |
| Monthly Recurring Revenue | $150 | $4,500 | $12,000 |
| Free-to-Paid Conversion Rate | 10% | 15% | 15% |
| Monthly Churn Rate | 5% | 3% | 2.5% |
| Average Units per Community | 50 | 60 | 65 |
| Dues Collection Rate (on-time payments) | 75% | 85% | 90% |
| Active Communities (1+ admin action/week) | 80% | 80% | 80% |
| Support Tickets per Community per Month | 2 | 0.8 | 0.5 |
| Stripe Payment Volume Processed (monthly) | $25,000 | $750,000 | $2,500,000 |

## 10. 12-Week Launch Plan
| Week | Milestone |
|------|-----------|
| 1 | Finalize tech stack; set up Next.js project, Supabase database and auth, Stripe Connect integration; design database schema; begin community setup wizard |
| 2 | Build community setup wizard: community details, unit import (CSV + manual), dues configuration, and Stripe Connect bank account linking |
| 3 | Build payment system: Stripe invoicing, ACH and credit card acceptance, payment status tracking, and the resident payment portal with payment history |
| 4 | Build automated payment reminders (email via SendGrid): configurable timing (before/on/after due date), late fee auto-application, and the board payment management dashboard |
| 5 | Build violation tracking: violation creation form, status workflow (reported > notice sent > resolved), violation notice email delivery, and photo upload |
| 6 | Build document library (upload, categorize, browse, download using Supabase Storage) and announcement board (compose, send via email, in-app feed); build resident portal with login, balance view, payment, and document access |
| 7 | Build board member role management (admin, treasurer, secretary permissions); implement free tier vs. paid tier access gates; internal QA and end-to-end testing of the full payment flow |
| 8 | Recruit 5 beta communities: reach out to HOA board members on r/HOA and HOA Facebook groups; offer 3-month free premium access in exchange for feedback; begin white-glove onboarding calls |
| 9 | Beta testing: validate payment processing with real dues collections; collect feedback on setup wizard difficulty, payment UX, and violation workflow; fix critical bugs; set up Mixpanel analytics |
| 10 | Public launch: post in r/HOA, r/CondoAssociation, and HOA Facebook groups; publish first SEO articles ("free HOA management tool for small communities," "how to collect HOA dues online"); begin direct mail campaign to 200 small HOAs in 5 target metros |
| 11 | Attend 2 regional Community Associations Institute (CAI) chapter meetings for in-person demos; analyze first 2 weeks of launch data; optimize onboarding completion rate; build maintenance request feature (v2, early start) |
| 12 | Month 3 retrospective: evaluate KPIs; plan v2 roadmap (maintenance requests, budget tool, meeting management, SMS); sign partnerships with 3 HOA attorneys or CPAs for referral agreements; publish case study from beta community showing dues collection improvement |

## 11. Growth Loops

**Board Member Network Effect**: HOA board members frequently know other board members in neighboring communities, at CAI events, and through social connections. When one board switches to HOA Simplified and their dues collection improves, they tell other boards. Each community acquired has a built-in referral radius of 3-5 other communities.

**Resident-to-Board Pipeline**: Residents who experience a smooth payment and communication experience through HOA Simplified at their current community become advocates when they move to a new community or join a new board. They bring the tool with them: "At my old community we used this — it was so much better."

**Treasurer Succession Loop**: When a board treasurer steps down and a new volunteer takes over, the outgoing treasurer hands off the HOA Simplified account — it's now the community's institutional tool, not a personal one. This creates structural lock-in and ensures continuity across board turnovers.

**CAI and HOA Attorney Referrals**: HOA attorneys and accountants serve dozens of communities each. A single partnership with an HOA attorney creates a distribution channel to their entire client base. The attorney recommends the tool because it reduces their own workload (clients are better organized).

**"Before/After" Dues Collection Stories**: Communities that switch from Venmo/checks to online dues collection via HOA Simplified see dramatic improvement in on-time payment rates (typically from 60% to 90%+). These transformation stories are shareable in HOA communities and serve as the most compelling marketing content.

## 12. Regulatory & Compliance

**Payment Processing Compliance**: Using Stripe Connect means funds route directly from residents to the HOA's bank account. HOA Simplified never holds community funds. This is critical: holding HOA funds would trigger money transmitter licensing requirements in most states. Stripe Connect's "connected accounts" model avoids this. Ensure the Stripe Connect integration uses the "Direct Charges" or "Destination Charges" model so HOA Simplified is the platform, not the funds handler.

**HOA Financial Records Laws**: Many states require HOAs to maintain financial records for a specified period (typically 7 years) and make them available to homeowners upon request. The document library and financial reporting features support compliance with these requirements. Clearly communicate data retention policies and offer data export so communities are never locked in.

**Data Privacy (Resident Information)**: The app stores resident names, email addresses, phone numbers, unit numbers, and payment histories. Comply with CCPA and applicable state privacy laws. Residents must be able to request deletion of their personal data. Board members must agree to terms that restrict use of resident data to community management purposes only.

**Fair Debt Collection Practices Act (FDCPA)**: Automated late payment reminders could be construed as debt collection activity. While HOA dues are generally not subject to FDCPA (HOAs are creditors, not debt collectors), the language in reminder emails must be professional and non-harassing. Provide templates that comply with state-specific collection notice requirements. Consult with an HOA attorney on reminder language.

**State-Specific HOA Governance Laws**: HOA governance varies significantly by state (meeting notice requirements, voting procedures, reserve fund mandates, document retention). The app should not provide legal advice but should offer features that help boards comply with common requirements (meeting minutes storage, financial reporting, document access for residents).

**Payment Card Industry (PCI) Compliance**: By using Stripe as the payment processor, HOA Simplified delegates PCI compliance to Stripe. The app never stores, processes, or transmits credit card numbers — Stripe handles all sensitive payment data. This must be maintained as the product scales; never build a custom payment form that touches card data directly.

## 13. Risk Register
| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| Slow adoption by non-technical volunteer board members who find onboarding confusing and revert to spreadsheets | High | High | Offer free 30-minute white-glove onboarding calls for every new community; build a setup wizard that imports unit lists from CSV; create video walkthroughs for every feature; design the UI with large buttons, clear labels, and minimal steps |
| Payment processing errors or delays that destroy trust (wrong amounts, failed transactions, delayed payouts) | Medium | Critical | Use Stripe Connect with direct charges (proven, reliable infrastructure); implement real-time payment confirmation emails; add reconciliation reports; test payment flows exhaustively before launch; maintain 99.9% uptime target for payment-related features |
| Enterprise competitors (AppFolio, Buildium) launch a "lite" tier targeting small HOAs and undercut on price | Medium | High | Move fast to establish brand as the "simple and affordable" option; build deep community loyalty through responsive support; focus on volunteer-specific UX (not stripped-down enterprise); enterprise players' cost structures make sub-$50/month pricing unattractive for them |
| A community has a payment dispute or embezzlement issue and HOA Simplified is implicated (even if not at fault) | Low | High | Stripe Connect ensures funds go directly to the HOA's bank account — never through our platform; maintain detailed audit logs of all transactions; provide clear terms of service disclaiming responsibility for community financial management; carry professional liability insurance |
| Data breach exposing resident personal information (names, emails, payment history, addresses) | Low | Critical | Encrypt all data at rest and in transit; use Supabase row-level security so residents can only access their own data; regular security audits; SOC 2 compliance by Year 2; incident response plan; minimize data collection |
| HOA boards switch to a competitor after setup because the switching cost is perceived as low | Medium | Medium | Make the product indispensable by combining payments, violations, documents, and communications into one tool (replacing 4-5 separate tools); build data portability features so boards feel they can leave (paradoxically, this increases trust and reduces churn); deliver rapid, responsive customer support that competitors can't match at their scale |
| Stripe Connect onboarding is too complex for non-technical board members, causing abandonment during setup | High | Medium | Create a step-by-step guide with screenshots specific to HOA use cases; offer to walk through Stripe Connect setup on the onboarding call; pre-fill as many fields as possible; provide a "skip for now, set up payments later" option so the rest of the platform is usable immediately |

## 14. Success Criteria
- **6-month go/no-go**: 150+ paid communities, $4,500+ MRR, 15% free-to-paid conversion rate, on-time dues collection rate above 85% for active communities, monthly churn below 3%, and at least 80% of paid communities performing 1+ admin action per week (demonstrating active usage, not just subscription inertia)
- **12-month milestone**: 400+ paid communities, $12,000+ MRR ($144K+ annualized, exceeding the $180K Year 1 target on a monthly run-rate basis), $2.5M+ in monthly Stripe payment volume processed, NPS above 50 from board member surveys, support ticket volume below 0.5 per community per month, and at least 3 HOA attorney or CPA referral partnerships actively generating leads
