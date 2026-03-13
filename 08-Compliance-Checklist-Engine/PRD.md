# Product Requirements Document: Compliance Checklist Engine

## 1. Executive Summary
Small businesses face an average of $83,019/year in regulatory compliance costs, with 87% of owners citing compliance as their most time-consuming non-revenue activity. The fundamental problem is not that regulations are hard to follow -- it is that business owners do not know which regulations apply to them, discovering gaps only when fines arrive. Compliance Checklist Engine solves this by auto-generating a personalized, comprehensive checklist of every applicable regulation based on the business's industry, state, city, employee count, and revenue. Each checklist item includes what the regulation is, why it matters, how to comply, the deadline, and the renewal frequency. The app tracks completion, sends deadline alerts, stores uploaded permits and licenses, and provides a compliance score. Targeting regulated SMBs (restaurants, childcare, construction, healthcare clinics, salons) at $19.99/month, the product fills an unserved niche -- no affordable, self-service compliance tool exists for multi-industry SMBs. With a $3.4B SAM and LTV:CAC of 10.7:1, the path to $2.4M ARR by Year 3 is driven by high stickiness (24-month average retention) and a consultant portal that enables bookkeepers to bring multiple businesses onto the platform.

## 2. User Personas

### Persona 1: Rosa, the Restaurant Owner
- **Age**: 47
- **Job**: Owner-operator of a 30-seat Mexican restaurant in Houston, TX
- **Income**: $180,000 restaurant revenue, $45,000 personal income
- **Pain Points**: Received a $2,500 fine last year because her grease trap inspection had lapsed; has no idea how many permits and certifications she needs across health department, fire marshal, liquor board, ADA, and employment law; relies on her accountant to remind her of renewals but things still slip through; spends 10 hours/month on compliance paperwork she barely understands
- **Goals**: Know exactly what she needs to comply with in one list; get reminded before deadlines so she never gets fined again; feel confident she's covered everything
- **Tech Comfort**: Low-moderate -- uses a smartphone and POS system but is not tech-savvy; needs plain language and step-by-step guidance

### Persona 2: David, the New Business Founder
- **Age**: 31
- **Job**: About to open a childcare center in Portland, OR
- **Income**: $70,000 from previous job (investing savings into the business)
- **Pain Points**: Overwhelmed by the number of licenses, permits, and certifications required to open a childcare center (state licensing, background checks, facility inspections, insurance, zoning); doesn't know what he doesn't know; has been Googling requirements for weeks and still isn't confident he has a complete list; worried he'll open and then get shut down for missing a requirement
- **Goals**: Get a complete, authoritative list of everything required before opening; check items off as he completes them; know the order of operations (what to do first, what depends on what)
- **Tech Comfort**: High -- comfortable with SaaS tools, expects modern UX, willing to pay for time savings

### Persona 3: Linda, the Bookkeeper/Consultant
- **Age**: 52
- **Job**: Independent bookkeeper managing 12 small business clients (mix of restaurants, salons, and contractors)
- **Income**: $85,000/year
- **Pain Points**: Several clients have been fined for lapsed permits and blamed her; she tracks renewals in a spreadsheet but it's unmanageable across 12 businesses and 50+ compliance items each; needs a tool that works across industries and states; wants to look professional and proactive with her clients
- **Goals**: Manage compliance for all clients in one dashboard; get alerted to upcoming deadlines across all clients; generate compliance reports to show clients their status; differentiate her service with compliance management as an add-on offering
- **Tech Comfort**: Moderate-high -- uses QuickBooks, Google Workspace, and various SaaS tools daily

## 3. User Stories (20+)
1. As a business owner, I want to enter my industry, state, city, employee count, and revenue so that the app generates a personalized compliance checklist.
2. As a business owner, I want to see every applicable regulation with a plain-language explanation so that I understand what I need to comply with without legal jargon.
3. As a business owner, I want each checklist item to include step-by-step instructions for how to comply so that I can take action without hiring a consultant.
4. As a business owner, I want to see deadlines and renewal frequencies for each compliance item so that I know when things are due.
5. As a business owner, I want email and SMS reminders before compliance deadlines so that I never miss a renewal or filing date.
6. As a business owner, I want to mark checklist items as complete so that I can track my progress toward full compliance.
7. As a business owner, I want to upload permits, licenses, and certificates and attach them to their corresponding checklist items so that all compliance documentation is in one place.
8. As a business owner, I want a compliance score (percentage of items completed) so that I can see my overall compliance health at a glance.
9. As a business owner, I want a calendar view showing all upcoming compliance deadlines so that I can plan my month around regulatory requirements.
10. As a business owner, I want to be notified when a regulation changes or a new requirement is added so that I stay current without researching myself.
11. As a new business founder, I want to see compliance items in recommended order (prerequisites first) so that I complete requirements in the right sequence.
12. As a restaurant owner, I want industry-specific checklist items (health permits, food handler certs, grease trap inspections, liquor license renewals) so that the checklist reflects my actual regulatory environment.
13. As a multi-location business owner, I want to manage compliance checklists for each location separately so that location-specific requirements are tracked independently.
14. As a bookkeeper, I want a consultant portal where I can view and manage compliance for all my client businesses in one dashboard.
15. As a bookkeeper, I want to generate compliance audit reports for each client so that I can provide a professional compliance status document.
16. As a business owner, I want to search and filter my checklist by category (health, fire, employment, tax, licensing) so that I can focus on specific areas.
17. As a business owner, I want to see the penalty/fine amount associated with non-compliance for each item so that I can prioritize high-risk items.
18. As a business owner, I want to add custom compliance items (internal policies, insurance renewals) to my checklist so that everything is tracked in one system.
19. As a business owner, I want to assign compliance tasks to team members (managers, HR) so that I can delegate responsibility for specific items.
20. As a business owner, I want to see a "last verified" date and source link for each regulation so that I can trust the information is current and verify it myself.
21. As a business owner, I want to export my compliance checklist as a PDF so that I can share it with my insurance carrier, landlord, or partners.
22. As a business owner, I want to receive a monthly compliance digest email summarizing my status, upcoming deadlines, and newly added requirements.
23. As a childcare center operator, I want DCFS licensing requirements, background check compliance, and staff certification tracking specific to my state.

## 4. Feature Requirements

### MVP (v1.0) -- Must Have
- [ ] Business profile setup: industry selector (restaurant, childcare, construction, healthcare clinic, salon/spa), state, city, employee count, revenue range -- with validation and guided tooltips
- [ ] Compliance checklist auto-generation: based on business profile, produce a comprehensive list of all applicable federal, state, and local regulations using an internal regulatory database seeded with data for 3 industries in 5 states
- [ ] Checklist item detail: each item includes regulation name, plain-language description, step-by-step compliance instructions, deadline/renewal date, renewal frequency, and source link
- [ ] Completion tracking: checkboxes to mark items as complete, with date stamped; overall compliance score (percentage) displayed on dashboard
- [ ] Deadline calendar: monthly/weekly calendar view showing all upcoming compliance deadlines; color-coded by urgency (red = overdue, yellow = due within 7 days, green = on track)
- [ ] Deadline reminders: automated email and SMS alerts sent at configurable intervals before each deadline (default: 30 days, 14 days, 3 days)
- [ ] Document upload: attach files (PDF, image) to individual checklist items; stored encrypted in S3; viewable from item detail screen
- [ ] Category filtering and search: filter checklist by category (Health & Safety, Licensing, Employment, Tax, Fire, ADA, Environmental); free-text search across all items
- [ ] User authentication and business account management with secure login
- [ ] Compliance dashboard: home screen showing compliance score, items due soon, overdue items, and recent regulatory updates
- [ ] Responsive web application optimized for desktop and tablet (business owners manage compliance at their desk, not on mobile)

### v2.0 -- Should Have
- [ ] Multi-location support: manage separate compliance checklists per business location with location-specific requirements
- [ ] Regulatory change alerts: notify business owners when a regulation changes, is added, or is repealed for their industry and jurisdiction
- [ ] Consultant/bookkeeper portal: multi-business dashboard allowing bookkeepers to manage compliance for up to 10 client businesses from one account
- [ ] Compliance audit report: generate PDF/CSV report of compliance status for insurance carriers, landlords, or auditors with completion dates and attached documents
- [ ] Fine/penalty display: show estimated fine amounts for non-compliance per checklist item to help prioritize
- [ ] Task delegation: assign individual compliance items to team members (managers, HR, operations) with email notification on assignment and due date
- [ ] Monthly compliance digest email: automated summary of status, completed items, upcoming deadlines, and new/changed regulations
- [ ] Industry expansion: add construction, healthcare clinic, and salon/spa regulatory databases for 10 additional states

### v3.0 -- Nice to Have
- [ ] AI compliance assistant: chatbot that answers business-specific compliance questions using the regulatory database and the business's profile context
- [ ] Insurance carrier integration: share compliance score directly with insurance providers for premium discount eligibility
- [ ] API for integration with QuickBooks, Gusto, and Homebase for automatic employee count and payroll data sync
- [ ] Community-contributed regulatory updates: allow verified users to flag regulatory changes, reviewed by staff before publishing
- [ ] Compliance benchmarking: show how the business's compliance score compares to others in the same industry and state (anonymized)

## 5. Technical Architecture
- **Frontend**: Next.js (React) -- server-side rendered web application for SEO (business owners search for compliance checklists on Google), fast page loads, and responsive design optimized for desktop/tablet; Tailwind CSS for rapid UI development
- **Backend**: Node.js with NestJS on AWS -- structured modular architecture suited to the regulatory domain model; background job processing for deadline reminders and regulatory change monitoring; REST API with planned GraphQL layer for the consultant portal
- **Database**: PostgreSQL on AWS RDS -- relational model for the complex regulatory database (industries x states x cities x regulation types) with strong referential integrity; JSONB for flexible regulation detail fields that vary by industry; full-text search for regulation lookup
- **Key APIs**:
  - OpenAI GPT-4o (plain-language compliance instruction generation, regulatory document summarization, and AI compliance assistant in v3)
  - Twilio (SMS deadline reminders)
  - SendGrid (email reminders, monthly digest, consultant reports)
  - AWS S3 (encrypted document storage for permits, licenses, certificates)
  - Stripe (subscription billing, multi-tier: business, consultant)
  - Google Maps Geocoding API (city/jurisdiction identification for local regulations)
- **Hosting**: AWS (ECS Fargate + RDS + S3 + CloudWatch + SQS) -- estimated $200/month at MVP scale; SQS for reliable deadline reminder processing; CloudWatch for monitoring regulatory data pipeline health; auto-scaling for seasonal traffic (new business filings spike in January and spring)

## 6. Data Model

### Businesses
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| owner_id | UUID | FK to Users |
| name | String | Business name |
| industry | Enum | Restaurant, Childcare, Construction, Healthcare Clinic, Salon |
| state | String | |
| city | String | |
| employee_count | Integer | |
| revenue_range | Enum | Under $100K, $100K-$500K, $500K-$1M, $1M-$5M, $5M+ |
| subscription_tier | Enum | Free, Paid, Premium |
| compliance_score | Float | Calculated percentage |
| created_at | Timestamp | |

### Regulations
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| title | String | Regulation name |
| description | Text | Plain-language explanation |
| instructions | Text | Step-by-step compliance guide |
| category | Enum | Health & Safety, Licensing, Employment, Tax, Fire, ADA, Environmental |
| applicable_industries | Enum[] | Which industries this applies to |
| applicable_states | String[] | Which states (or "ALL") |
| applicable_city_rules | JSONB | City-specific overrides or additions |
| employee_threshold | Integer | Minimum employee count to apply (nullable) |
| revenue_threshold | String | Minimum revenue range to apply (nullable) |
| renewal_frequency | Enum | One-time, Annual, Biennial, Quarterly, Monthly |
| estimated_fine | Decimal | Typical penalty for non-compliance |
| source_url | String | Link to authoritative source |
| last_verified_date | Date | When staff last verified accuracy |
| is_active | Boolean | |

### Checklist Items
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| business_id | UUID | FK to Businesses |
| regulation_id | UUID | FK to Regulations |
| status | Enum | Not Started, In Progress, Complete, Overdue |
| deadline | Date | Calculated from regulation + business context |
| next_renewal_date | Date | |
| completed_at | Timestamp | |
| completed_by | UUID | FK to Users |
| document_urls | String[] | S3 paths for uploaded documentation |
| notes | Text | User notes |
| assigned_to | UUID | FK to Users (nullable) |

### Regulatory Updates
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| regulation_id | UUID | FK to Regulations |
| change_type | Enum | New, Modified, Repealed |
| summary | Text | Plain-language change description |
| effective_date | Date | |
| published_at | Timestamp | |

**Relationships**: Users own one or more Businesses. Each Business has many Checklist Items, generated from the Regulations table based on industry, state, city, employee count, and revenue. Checklist Items reference Regulations. Regulatory Updates are linked to Regulations and trigger notifications to affected Businesses. The Consultant portal creates a many-to-many relationship between consultant Users and client Businesses.

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Onboarding -- Business Profile Setup
A clean, wizard-style form guiding the user through 5 steps: (1) Business name; (2) Industry selection from a visual card grid with icons (Restaurant, Childcare, Construction, Healthcare Clinic, Salon/Spa); (3) State and city dropdowns; (4) Employee count slider (1-50+); (5) Revenue range selector. Each step includes a brief explanation of why the information matters ("We use your employee count to identify employment law requirements"). A progress bar shows completion. Tapping "Generate My Checklist" triggers the checklist creation with a loading animation showing "Analyzing regulations for [Industry] in [City, State]..."

### Screen 2: Compliance Dashboard (Home)
The primary screen displays a large compliance score circle (e.g., "72% Compliant") with color coding (red <50%, yellow 50-80%, green >80%). Below: three summary cards -- "Overdue Items" (count, red badge), "Due This Month" (count, yellow badge), and "Recently Completed" (count, green badge). A "Quick Actions" bar allows one-tap access to: View Full Checklist, Open Calendar, Upload a Document. A sidebar (on desktop) or bottom nav (on mobile) provides navigation to Dashboard, Checklist, Calendar, Documents, Settings. At top right, notification bell shows unread regulatory updates and deadline alerts.

### Screen 3: Full Compliance Checklist
A scrollable list of all compliance items grouped by category (Health & Safety, Licensing, Employment, Tax, Fire, ADA, Environmental) with collapsible sections. Each item shows: regulation title, status badge (Complete/In Progress/Not Started/Overdue), deadline date, and an expand arrow. Expanding an item reveals: plain-language description, step-by-step instructions, source link, estimated fine for non-compliance, document upload button, assigned person, and a "Mark Complete" button with date stamping. Filter buttons at top allow viewing: All, Overdue, Due Soon, Complete. A search bar enables finding items by keyword.

### Screen 4: Checklist Item Detail
A full-page detail view for a single compliance item showing: regulation title and category badge, plain-language description ("What is this?"), step-by-step compliance instructions ("How to comply"), deadline and renewal frequency, estimated fine ("What happens if I don't comply: Up to $5,000"), source URL (clickable link to the authoritative regulation text), assigned team member (with reassign option), attached documents (thumbnails with upload button), completion status (with "Mark Complete" or "Mark In Progress" button), and a notes field for user annotations. A "Last verified: [date]" label at the bottom builds trust in data accuracy.

### Screen 5: Deadline Calendar
A monthly calendar view with dots color-coded by urgency: red (overdue), orange (due within 7 days), yellow (due within 30 days), blue (upcoming). Tapping a day reveals a sidebar list of items due that day with title, category, and status. An "Agenda" toggle switches to a chronological list view of all upcoming deadlines over the next 90 days. A "Sync with Google Calendar" button exports deadlines to the user's personal calendar. Reminder configuration (30 days, 14 days, 3 days before) is accessible from a gear icon on this screen.

### Screen 6: Document Vault
A categorized document browser organized by compliance category. Each section shows attached documents with thumbnail, file name, upload date, and the checklist item it's attached to. An "Upload" button allows drag-and-drop (desktop) or camera/file picker (mobile) upload. Tapping a document opens a preview modal. A "Missing Documents" filter highlights checklist items marked complete but without attached documentation. All documents are encrypted at rest. A bulk download option exports all documents as a ZIP file for backup or audit preparation.

### Screen 7: Regulatory Updates Feed
A chronological feed of regulatory changes relevant to the user's business profile. Each update shows: change type badge (New Requirement, Modified, Repealed), regulation title, plain-language summary of the change, effective date, and an "Update My Checklist" button that adds or modifies the affected checklist item. Users can filter by category and severity. A "No action needed" label appears on updates that are informational only. Email notification settings for updates are configurable from this screen.

### Screen 8: Consultant Portal (Multi-Business View)
A table or card-based view showing all client businesses the consultant manages. Each card displays: business name, industry icon, compliance score, number of overdue items, and next deadline. Sorting options: by compliance score (lowest first), by next deadline, or alphabetically. Tapping a business opens that business's full compliance dashboard. A "Generate Report" button produces a PDF compliance audit report for the selected business. An "Add Client Business" button initiates a flow where the consultant enters client details or sends an invite link for the client to set up their own profile.

### Screen 9: Compliance Audit Report (Preview & Export)
A preview screen showing a professionally formatted compliance report: business name and details at top, overall compliance score, category-by-category breakdown of complete vs. incomplete items, overdue items highlighted, attached documentation status, and a signature line for the business owner. Export options: PDF download, email directly to insurance carrier, or share via link. A "Schedule Monthly Report" toggle automates report generation and delivery on the 1st of each month.

### Screen 10: Settings & Subscription
Business profile management (edit industry, location, employee count), team member management (add/remove users with role assignment: Owner, Admin, Viewer), notification preferences (granular controls for email reminders, SMS reminders, regulatory update alerts, monthly digest), subscription management (current plan, upgrade to multi-location or consultant tier, billing history), and data management (export all data, delete account). An "Integration" section shows future connections to QuickBooks, Gusto, and Google Calendar.

## 8. Monetization Implementation

### Paywall Placement
The free tier allows the business owner to enter their profile and receive a high-level compliance overview showing 5-10 major requirements without detailed instructions, deadlines, or reminders. The paywall activates when the user attempts to: (a) view detailed step-by-step instructions, (b) see deadlines and set reminders, (c) upload documents, (d) access the compliance score, or (e) view more than 10 checklist items.

### Upgrade Triggers
- **Fine preview shock**: On the free checklist overview, show estimated total fine exposure: "Your business faces up to $47,000 in potential fines across 23 compliance items. Upgrade to see every requirement and never get fined again."
- **Deadline urgency**: If a detectable deadline is approaching (e.g., annual liquor license renewal), show: "Your liquor license renewal is due in 45 days. Upgrade to get reminders and step-by-step renewal instructions."
- **Checklist completeness tease**: Show 10 of 23 items with the rest blurred: "You're seeing 43% of your compliance requirements. Upgrade to see the full picture."

### Pricing Psychology
- Monthly ($19.99) and annual ($199.99, saving 17%) options with annual pre-selected.
- "One prevented fine pays for 10 years of the app" messaging -- average fine is $2,500-$10,000.
- 14-day free trial of full features during onboarding to build dependency on deadline reminders.
- Consultant tier ($49.99/month) positioned as revenue-generating: "Charge your clients $50/month for compliance management and the tool pays for itself with one client."

## 9. Analytics & KPIs

| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| Businesses Onboarded | 150 | 1,500 | 4,000 |
| Paid Businesses | 20 | 350 | 1,000 |
| Free-to-Paid Conversion Rate | 10% | 12% | 14% |
| Monthly Recurring Revenue (MRR) | $400 | $7,000 | $20,000 |
| Checklist Completion Rate (Items completed within 30 days) | 50% | 60% | 70% |
| Deadline Reminder Open Rate | 80% | 85% | 90% |
| Average Compliance Score (Paid Users) | 55% | 70% | 80% |
| Monthly Churn Rate | 6% | 4% | 3% |
| Consultant Portal Activations | 2 | 20 | 50 |
| Industry-State Combinations Covered | 15 | 40 | 75 |
| App NPS Score | 30 | 45 | 55 |

## 10. 12-Week Launch Plan

| Week | Milestone |
|------|-----------|
| 1 | Finalize tech stack; set up Next.js project, NestJS backend, PostgreSQL schema, AWS infrastructure (ECS, RDS, S3, SQS), and CI/CD pipeline; begin regulatory database research for restaurants in CA, TX, FL |
| 2 | Build user authentication, business profile setup wizard, and industry/state/city selection UI with validation |
| 3 | Seed regulatory database: complete restaurant compliance data for CA, TX, FL, NY, and IL (covering 35% of US restaurants); structure data with plain-language descriptions and step-by-step instructions |
| 4 | Build checklist auto-generation engine: match business profile against regulatory database and produce personalized checklist; implement compliance score calculation |
| 5 | Build full compliance checklist UI: grouped by category, expandable item details, status badges, mark complete functionality, and category/search filtering |
| 6 | Implement deadline calendar view, reminder engine (SQS + Twilio SMS + SendGrid email), and configurable reminder intervals (30/14/3 days before deadline) |
| 7 | Build document upload and vault: S3 integration with encryption, file attachment to checklist items, document preview, and missing-document detection |
| 8 | Build compliance dashboard home screen, regulatory updates feed, Stripe subscription paywall, and free tier checklist preview with upgrade triggers |
| 9 | Seed regulatory database: add childcare industry for 5 states; begin construction industry research; implement regulatory change alert system |
| 10 | Alpha testing with 10 restaurant owners recruited from r/smallbusiness and local SCORE chapters; gather feedback on checklist accuracy, UX, and reminder timing; fix critical bugs |
| 11 | Beta launch: invite 50 businesses (restaurants and childcare centers); iterate on top feedback items; verify regulatory data accuracy with industry contacts; finalize landing page with SEO-optimized content for "[industry] compliance checklist [state]" keywords |
| 12 | Public launch: publish launch post on r/smallbusiness and r/Entrepreneur with free California Restaurant Compliance Checklist PDF; begin Google Ads campaign targeting "[industry] compliance requirements [state]" keywords; contact 10 SCORE chapters and SBDCs for partnership; send launch email to beta waitlist |

## 11. Growth Loops

### Content SEO Loop
Publish free, SEO-optimized compliance checklist PDFs for high-volume search queries ("[state] restaurant compliance requirements"). These PDFs capture email addresses and rank on Google, driving ongoing organic traffic. Each PDF includes a CTA: "This checklist has 12 items. Your full personalized checklist has 23+ items with deadline tracking -- try the Compliance Checklist Engine." As the regulatory database grows, new content pages are auto-generated, compounding organic traffic.

### Consultant Multiplier Loop
Each bookkeeper or consultant who signs up brings 5-10 client businesses onto the platform. The consultant portal is free for the first year, creating zero-friction onboarding. Consultants become evangelists because the tool makes them look proactive and professional with their clients. Each client business is a potential direct-paying customer if the consultant relationship ends.

### Compliance Score Sharing
When a business reaches 90%+ compliance, they receive a "Fully Compliant" digital badge they can display on their website, Google Business Profile, or share with their insurance carrier. This creates social proof, brand awareness, and incentivizes other businesses in the same industry to sign up ("If Rosa's restaurant next door is verified compliant, I should be too").

### Fine Avoidance Word-of-Mouth
Business owners who avoid fines because of deadline reminders naturally share the story with peers ("I almost got fined $5,000 but the app reminded me to renew my grease trap inspection"). This word-of-mouth in tight-knit local business communities (restaurant owner groups, chamber of commerce meetings) drives high-intent referrals.

## 12. Regulatory & Compliance

- **Regulatory Data Accuracy Liability**: The app provides regulatory information, not legal advice. Every checklist item must include a "last verified" date and source link. Terms of service must prominently disclaim that the tool supplements but does not replace professional legal or compliance consulting. Carry errors and omissions (E&O) insurance to protect against claims arising from incorrect or outdated regulatory data.
- **State-by-State Legal Variations**: Compliance requirements vary not just by state but by city and county. The regulatory database must track jurisdiction-level variations. Where local data is incomplete, clearly label it as "state-level requirements -- local requirements may vary" with a prompt to consult local authorities.
- **Data Privacy**: CCPA, VCDPA, and other state privacy laws apply. Business data (industry, location, revenue, employee count) and uploaded documents (permits, licenses) are sensitive. Encrypt all data at rest (AES-256) and in transit (TLS 1.3). Provide data export and deletion requests honored within 30 days. Never sell or share business data.
- **Document Storage Security**: Uploaded permits, licenses, and certifications contain sensitive business information. Implement server-side encryption on S3, access logging, and role-based access control. Comply with data retention policies -- allow users to set document retention periods.
- **Unauthorized Practice of Law (UPL)**: Providing step-by-step compliance instructions could be construed as practicing law in some jurisdictions. Mitigate by framing all guidance as "informational," including disclaimers, and sourcing from publicly available government resources. Do not provide advice on how to interpret ambiguous regulations.
- **Government Data Usage**: Regulatory data is sourced from government websites and databases. Ensure compliance with any terms of use on government data portals. Attribute sources properly with direct links to official government pages.

## 13. Risk Register

| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| Regulatory database contains inaccurate or outdated information, causing a business to miss a requirement and receive a fine | High | Critical | Start with only 3 industries in 5 well-documented states; mark each item with "last verified" date and source link; hire part-time regulatory research contractors per industry vertical; implement community-contributed update flagging with staff review; carry E&O insurance |
| Scaling to 50 states and multiple industries is extremely labor-intensive (500+ state-industry combinations) | High | High | Prioritize by market size (restaurants in CA, TX, FL, NY, IL first); use LLM-assisted extraction from government websites with human verification; build modular regulatory database so each new state reuses federal requirements; charge premium for industries/states not yet covered |
| Large competitors (Gusto, Homebase, Square) add compliance checklist modules as add-on features | Medium | High | Go deeper than horizontal platforms with industry-specific regulations (grease trap inspections, food handler cert renewals) that Gusto will never build; position as the specialist tool that integrates with generalist platforms; build switching costs through document vault and compliance history |
| Low awareness among small business owners that a compliance tool exists (category creation challenge) | Medium | Medium | Lead with content marketing (free compliance checklists for SEO); partner with trusted intermediaries (SCORE, SBDCs, accountants) who already advise business owners; use fear-based messaging ("Find out what you're missing before the inspector does") to create urgency |
| Unauthorized Practice of Law (UPL) claims from bar associations in certain states | Low | High | Frame all guidance as "informational" with prominent disclaimers; source all instructions from publicly available government resources with direct links; do not interpret ambiguous regulations; consult with a legal compliance attorney in each expansion state; carry professional liability insurance |
| Businesses churn after achieving initial compliance because they perceive the tool as a one-time setup rather than ongoing service | Medium | Medium | Emphasize renewal tracking and deadline reminders as the core ongoing value; add regulatory change alerts that demonstrate continuous monitoring; show "days since last compliance check" to create re-engagement urgency; offer annual compliance audit reports that become a business operating requirement |

## 14. Success Criteria
- **6-month go/no-go**: 350+ paid businesses, 14%+ free-to-paid conversion rate, $7,000+ MRR, 70%+ compliance score among active users (indicating they're actually completing checklist items), <4% monthly churn, and regulatory database covering 3 industries in 10+ states with verified accuracy
- **12-month milestone**: 1,000+ paid businesses, $20,000+ MRR, 50+ consultant portal activations (each bringing 3+ client businesses), NPS of 55+, regulatory database covering 5 industries in 25+ states, and at least 3 SCORE/SBDC partnerships actively recommending the tool
