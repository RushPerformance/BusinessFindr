# Product Requirements Document: Elderly Care Coordinator

## 1. Executive Summary
53 million Americans serve as unpaid caregivers for aging family members, spending an average of 24 hours per week on caregiving while coordinating through chaotic group texts, shared Google Docs, and sticky notes. 61% report that sibling coordination is a major source of stress. Elderly Care Coordinator provides a single family dashboard where adult children create a "care circle" for each parent, manage medications with refill reminders, share appointment calendars, assign and track caregiving tasks, log health observations, store critical documents, and send weekly summary emails to keep remote family members informed. Targeting the sandwich generation (ages 35-55) at $9.99/month, the app fills the gap left by CareZone's 2022 shutdown, leverages a built-in viral loop (inviting siblings), and addresses a $1.4B SAM in a market with powerful demographic tailwinds -- 10,000 Americans turn 65 every day.

## 2. User Personas

### Persona 1: Sarah, the Primary Caregiver Daughter
- **Age**: 42
- **Job**: Elementary school teacher
- **Income**: $55,000/year household
- **Pain Points**: Sole coordinator of her mother's care; spends 20 hours/week on caregiving tasks on top of full-time work; resentful that her brother who lives 2 hours away only calls to ask "how's Mom?" but doesn't take on tasks; missed a medication refill last month that caused a health scare; feels guilty, exhausted, and unsupported
- **Goals**: Share the caregiving workload with siblings through clear task assignment and accountability; never miss a medication or appointment; have one place for all of Mom's health information
- **Tech Comfort**: Moderate -- uses iPhone daily, comfortable with apps but needs simplicity; no patience for setup complexity

### Persona 2: James, the Long-Distance Sibling
- **Age**: 38
- **Job**: Software engineer
- **Income**: $130,000/year
- **Pain Points**: Lives 500 miles from his father; feels guilty about not helping more; gets sporadic updates from his sister via text but doesn't have a full picture of Dad's health; wants to contribute but doesn't know what tasks need doing; sometimes the information he gets is outdated or contradictory
- **Goals**: Stay informed about Dad's care without burdening his sister with update requests; take on tasks he can do remotely (scheduling appointments, managing insurance, paying bills); feel like an active participant in Dad's care
- **Tech Comfort**: High -- early adopter, comfortable with any technology

### Persona 3: Maria, the Professional Home Caregiver
- **Age**: 50
- **Job**: Part-time home health aide
- **Income**: $28,000/year
- **Pain Points**: Works with 3 families and each has different communication expectations; one family texts updates, another uses a whiteboard on the fridge, another leaves sticky notes; needs to know medication schedules, dietary restrictions, and doctor preferences without calling family members every time; has no formal way to report what she did during her shift
- **Goals**: See a clear care plan for each client; log activities and observations for family transparency; receive medication and task reminders so nothing is missed; communicate efficiently with family without phone tag
- **Tech Comfort**: Low-to-moderate -- uses a smartphone but prefers simple interfaces; can handle apps if they're intuitive

## 3. User Stories (20+)
1. As a primary caregiver, I want to create a care circle for my parent so that all family caregivers are connected in one place.
2. As a caregiver, I want to invite siblings and family members to the care circle via email or SMS so that everyone can participate in care coordination.
3. As a caregiver, I want to add my parent's full medication list with dosages and schedules so that everyone knows what medications are being taken and when.
4. As a caregiver, I want to receive medication refill reminders so that prescriptions are refilled before they run out.
5. As a caregiver, I want to add doctor appointments to a shared calendar so that all family members can see upcoming visits.
6. As a caregiver, I want to assign caregiving tasks to specific family members so that responsibilities are clear and distributed fairly.
7. As a long-distance sibling, I want to see a task board with assignments and completion status so that I know what needs doing and can volunteer for tasks.
8. As a caregiver, I want to log daily health observations (symptoms, vitals, mood, appetite) so that patterns can be identified and shared with doctors.
9. As a caregiver, I want to upload and store critical documents (insurance cards, advance directives, power of attorney) so that they are accessible to all care circle members in emergencies.
10. As a caregiver, I want all care circle members to access a shared emergency contact sheet so that anyone can reach doctors, pharmacies, and family in urgent situations.
11. As a long-distance sibling, I want to receive weekly summary emails with care updates so that I stay informed without constant texting.
12. As a caregiver, I want to set recurring tasks (weekly grocery shopping, monthly bill payment) so that ongoing responsibilities are tracked automatically.
13. As a caregiver, I want task completion notifications so that I know when a sibling has finished their assigned task.
14. As a caregiver, I want to track my parent's weight, blood pressure, and blood sugar over time so that I can share trends with their doctor.
15. As a professional caregiver, I want to log my shift activities so that the family knows exactly what was accomplished during my visit.
16. As a caregiver, I want to mark tasks as urgent so that time-sensitive items are prioritized by the care circle.
17. As a caregiver, I want to add notes to appointments (questions for the doctor, transportation details) so that whoever accompanies my parent is prepared.
18. As a long-distance sibling, I want to receive push notifications for urgent updates so that I can respond immediately to emergencies.
19. As a caregiver, I want to see a medication interaction checker so that I can flag potential conflicts before discussing with a pharmacist.
20. As a caregiver, I want to export the health journal as a PDF to bring to doctor appointments so that the physician has a complete picture of recent health changes.
21. As a family member, I want a shared photo/memory timeline so that our care circle includes positive moments alongside medical management.
22. As a caregiver, I want to track expenses related to my parent's care so that costs can be shared fairly among siblings.
23. As a primary caregiver, I want to see a "caregiver equity" dashboard showing each family member's task contributions so that I have data to support conversations about workload sharing.

## 4. Feature Requirements

### MVP (v1.0) -- Must Have
- [ ] Care circle creation: set up a named care profile for each elderly family member with photo, age, and key medical conditions
- [ ] Family member invitation: invite caregivers to the care circle via email or SMS link with role assignment (admin, member, view-only)
- [ ] Medication management: add medications with name, dosage, frequency, prescribing doctor, and pharmacy; display in a daily schedule view
- [ ] Medication reminders: configurable push notification and SMS reminders for each medication at scheduled times
- [ ] Medication refill alerts: track refill dates and send reminders 5 days before a prescription needs refilling
- [ ] Shared appointment calendar: add, edit, and view doctor appointments, therapy sessions, and tests visible to all care circle members
- [ ] Task board: create tasks with title, description, due date, assigned family member, and status (To Do, In Progress, Done)
- [ ] Task assignment and completion tracking: assign tasks to specific members; mark complete with optional notes; send completion notification to circle
- [ ] Health journal: log daily observations (symptoms, vitals, mood, meals, sleep, bowel movements) with date and time stamps
- [ ] Emergency contact sheet: add and view emergency contacts (doctors, pharmacy, hospital, family) accessible to all care circle members
- [ ] User authentication with secure invite-based access control per care circle
- [ ] Push notifications for task assignments, medication reminders, appointment reminders, and urgent updates

### v2.0 -- Should Have
- [ ] Document vault: encrypted upload and storage of insurance cards, advance directives, power of attorney, medical records with category tagging
- [ ] Weekly summary email: automated digest sent to all care circle members showing completed tasks, upcoming appointments, medication adherence, and health journal highlights
- [ ] Multiple care recipients: support for families managing care for both parents, in-laws, or extended family
- [ ] Caregiver shift scheduling: assign time blocks to family members or professional caregivers with swap/trade functionality
- [ ] Health trend visualization: charts and graphs for tracked vitals (weight, blood pressure, blood sugar) over time
- [ ] Expense tracking: log care-related expenses with receipt photos, categorization, and family cost-sharing split calculation
- [ ] Professional caregiver portal: limited-access view for hired caregivers to see medication schedule, tasks, and log shift activities
- [ ] Care equity dashboard: visual breakdown of each family member's task contributions over time

### v3.0 -- Nice to Have
- [ ] Pharmacy refill service integration: connect to CVS, Walgreens, or mail-order pharmacies for automated refill requests
- [ ] Telehealth appointment booking: schedule video appointments with the parent's doctors directly from the app
- [ ] Medication interaction checker: flag potential drug interactions based on the medication list (using an FDA/NIH drug interaction API)
- [ ] Shared memory timeline: family photo and story sharing alongside care management for emotional connection
- [ ] Integration with wearable health devices (Apple Watch, Fitbit) for automatic vitals import

## 5. Technical Architecture
- **Frontend**: React Native (Expo) -- cross-platform mobile app for iOS and Android; care coordination requires mobile-first access for on-the-go caregivers; Expo provides push notification infrastructure out of the box
- **Backend**: Node.js with NestJS on AWS -- NestJS provides structured, scalable architecture with built-in support for WebSockets (real-time care circle updates), scheduled jobs (medication reminders), and modular design for adding care features incrementally
- **Database**: PostgreSQL on AWS RDS -- relational model for care circles, family relationships, medication schedules, and task assignments where referential integrity is critical; plus a time-series pattern for health journal entries
- **Key APIs**:
  - Twilio (SMS medication reminders, family invitation links, urgent notifications)
  - SendGrid (weekly summary emails, appointment reminders)
  - AWS S3 (encrypted document vault storage for medical records, insurance cards)
  - Firebase Cloud Messaging / APNs (push notifications)
  - Stripe (subscription billing)
  - Google Calendar API (optional: sync appointments to personal calendars)
- **Hosting**: AWS (ECS Fargate + RDS + S3 + SQS) -- estimated $180/month at MVP scale; SQS for reliable medication reminder delivery; S3 for document storage with server-side encryption; auto-scaling for growing family user base

## 6. Data Model

### Care Recipients
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| name | String | Parent/elderly person's name |
| photo_url | String | Profile photo (S3) |
| date_of_birth | Date | |
| medical_conditions | Text[] | Array of conditions |
| allergies | Text[] | |
| blood_type | String | |
| primary_physician | String | |
| created_by | UUID | FK to Users |

### Care Circles
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| care_recipient_id | UUID | FK to Care Recipients |
| name | String | e.g., "Mom's Care Team" |
| created_at | Timestamp | |

### Care Circle Members
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| care_circle_id | UUID | FK to Care Circles |
| user_id | UUID | FK to Users |
| role | Enum | Admin, Member, View-Only, Professional Caregiver |
| relationship | String | Daughter, Son, Aide, etc. |
| joined_at | Timestamp | |

### Medications
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| care_recipient_id | UUID | FK to Care Recipients |
| name | String | Medication name |
| dosage | String | e.g., "10mg" |
| frequency | String | e.g., "Twice daily" |
| schedule_times | Time[] | Array of times |
| prescribing_doctor | String | |
| pharmacy | String | |
| refill_date | Date | Next refill due |
| notes | Text | Special instructions |

### Tasks
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| care_circle_id | UUID | FK to Care Circles |
| title | String | |
| description | Text | |
| assigned_to | UUID | FK to Users (nullable) |
| created_by | UUID | FK to Users |
| due_date | Date | |
| is_recurring | Boolean | |
| recurrence_rule | String | Cron expression for recurring tasks |
| status | Enum | To Do, In Progress, Done |
| priority | Enum | Normal, Urgent |
| completed_at | Timestamp | |

### Health Journal Entries
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| care_recipient_id | UUID | FK to Care Recipients |
| logged_by | UUID | FK to Users |
| entry_date | Timestamp | |
| type | Enum | Vitals, Symptom, Mood, Meal, Sleep, Note |
| data | JSONB | Flexible schema for different entry types |
| notes | Text | Free-form observations |

**Relationships**: Users belong to many Care Circles via Care Circle Members. Each Care Circle has one Care Recipient. Care Recipients have many Medications, Tasks (via Care Circle), and Health Journal Entries. Tasks are assigned to Users within a Care Circle.

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Onboarding -- Create Care Circle
After signup, the user sees "Let's set up care for your loved one." They enter the care recipient's name, upload an optional photo, and add key medical conditions from a searchable list. The next step prompts them to add medications one by one (name, dosage, schedule). Finally, they see "Invite your family" with fields for sibling names, email addresses, and relationship. Each invite sends a personalized link: "Sarah invited you to join Mom's care circle." A "Skip for now" option is available at each step.

### Screen 2: Care Circle Dashboard (Home)
The main screen displays the care recipient's name and photo at top. Below are four summary cards: Medications (next dose due in X minutes), Appointments (next appointment details), Tasks (X tasks due today, X overdue), and Health Journal (last entry summary). A prominent "Add" floating action button allows quickly adding a task, appointment, medication, or journal entry. A care circle member row at bottom shows avatar icons of all connected family members with online/last-active status.

### Screen 3: Medication Schedule
A daily timeline view showing each medication at its scheduled time. Each medication card shows the name, dosage, and an "Acknowledged" checkbox (for the caregiver to confirm it was given). A red badge appears on overdue medications. Tapping a medication opens a detail view with full information (prescribing doctor, pharmacy, refill date, notes). A "Refill Needed" banner appears at the top when any medication's refill date is within 5 days. A toggle switches between today's view and a weekly overview.

### Screen 4: Shared Calendar
A monthly calendar view with color-coded dots: blue for doctor appointments, green for therapy, orange for tests/labs. Tapping a day shows the day's appointments in a list. Each appointment card shows time, doctor name, location, and a notes field (pre-visit questions, transportation arrangements). An "Add Appointment" button opens a form. Appointments sync bi-directionally with Google Calendar if connected. A reminder configuration option lets users set when to be notified (1 day before, 2 hours before, etc.).

### Screen 5: Task Board
A kanban-style board with three columns: To Do, In Progress, and Done. Each task card shows title, assigned person's avatar, due date, and priority flag (orange for urgent). Dragging cards between columns updates status. Tapping a card opens details with description, assignment, notes, and a comment thread for family discussion. An "Assign to" dropdown shows all care circle members. A "Create Task" button opens a form with optional recurrence settings (weekly, monthly). An "Unassigned" filter shows tasks that need to be picked up.

### Screen 6: Health Journal
A chronological feed of health observations, newest first. Each entry is tagged by type (Vitals, Symptom, Mood, Meal, Sleep, Note) with color-coded badges. Vitals entries show values in context (e.g., "Blood Pressure: 142/88 -- elevated" with a trend arrow). A "Log Entry" button opens a form with type selector, structured fields for the chosen type (e.g., BP systolic/diastolic, weight, temperature), and a free-text notes area. A "Trends" tab shows simple line charts of tracked vitals over time. An "Export for Doctor" button generates a PDF summary of the last 30 days.

### Screen 7: Document Vault
A categorized file browser: Insurance, Legal (advance directives, POA), Medical Records, Prescriptions, Other. Each category shows document thumbnails with upload date and uploader name. Tapping a document opens a full-screen viewer. An "Upload" button allows camera capture or file selection. Documents are encrypted at rest. A search bar enables finding documents by name or category. An "Emergency Access" toggle marks documents that should be immediately visible to all care circle members (e.g., insurance card, emergency contacts).

### Screen 8: Weekly Summary Email (Configuration + Preview)
A settings screen where the user configures the weekly summary: which sections to include (medications adherence, completed tasks, upcoming appointments, health journal highlights, expense summary), which day/time to send, and which care circle members receive it. A "Preview" button shows a rendered email mockup. The email itself includes a "View in App" deep link for each section and a "Reply with Update" feature that posts the reply as a health journal note.

### Screen 9: Emergency Contact Sheet
A clean, high-contrast screen designed for quick access in emergencies. Shows: Primary Physician (name, phone, tap-to-call), Hospital Preference (name, address, tap-to-navigate), Pharmacy (name, phone), Insurance (carrier, policy number, group number), and all family caregiver contacts (name, relationship, phone, tap-to-call). A "Share Sheet" button sends the full contact list via SMS or email. This screen is accessible from the dashboard with a single tap on a red "Emergency" button and does not require re-authentication.

### Screen 10: Profile & Settings
User profile (name, email, relationship to care recipient), notification preferences (granular toggles for medication reminders, task assignments, appointment reminders, urgent alerts, weekly summary), subscription management (current plan, upgrade to premium for multiple care recipients), and care circle management (view members, change roles, remove members, leave circle). A "Switch Care Circle" option for users managing multiple care recipients. Data export and account deletion options at the bottom.

## 8. Monetization Implementation

### Paywall Placement
The free tier supports 1 care recipient with up to 2 care circle members, basic medication list (no reminders), shared calendar, and emergency contacts. The paywall activates when the user attempts to: (a) invite a 3rd care circle member, (b) enable medication reminders, (c) access the task board, (d) use the health journal, or (e) add a second care recipient.

### Upgrade Triggers
- **Sibling invitation overflow**: When the user tries to invite a 3rd family member, the upgrade prompt reads "Your care team is growing -- upgrade to add unlimited family members and keep everyone coordinated."
- **Medication reminder moment**: After adding 3+ medications, prompt: "Mom takes 5 medications daily. Never miss a dose -- upgrade to enable automatic reminders."
- **Task assignment friction**: When the user creates their 3rd task, show "You're carrying a lot. Upgrade to assign tasks to siblings and share the load."

### Pricing Psychology
- Monthly ($9.99) and annual ($89.99, saving 25%) options with annual pre-selected.
- "Less than the cost of one home health aide hour" messaging.
- 14-day free trial of full features during onboarding -- long enough for the family to set up and build dependency.
- Sibling discount: when the paying user's sibling joins the same care circle, offer the sibling 50% off their own separate care recipient account.

## 9. Analytics & KPIs

| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| Care Circles Created | 200 | 2,500 | 6,000 |
| Paid Families | 20 | 500 | 1,200 |
| Free-to-Paid Conversion Rate | 5% | 8% | 10% |
| Monthly Recurring Revenue (MRR) | $200 | $5,000 | $12,000 |
| Care Circle Members per Family | 2.5 | 3.0 | 3.2 |
| Tasks Completed per Family / Week | 3 | 5 | 6 |
| Medication Reminder Ack. Rate | 70% | 80% | 85% |
| Weekly Summary Email Open Rate | 55% | 58% | 60% |
| Monthly Family Churn Rate | 8% | 5% | 4% |
| Health Journal Entries / Family / Week | 2 | 4 | 5 |
| App Store Rating | 4.2 | 4.4 | 4.6 |

## 10. 12-Week Launch Plan

| Week | Milestone |
|------|-----------|
| 1 | Finalize tech stack; set up React Native (Expo) project, NestJS backend, PostgreSQL schema, AWS infrastructure (ECS, RDS, S3, SQS), and CI/CD pipeline |
| 2 | Build user authentication (email + Apple/Google Sign-In), care circle creation flow, care recipient profile setup, and family member invitation system with email/SMS deep links |
| 3 | Implement medication management: add/edit/delete medications, daily schedule timeline view, and medication detail screen |
| 4 | Build medication reminder engine: Twilio SMS + push notification delivery, scheduled job processing via SQS, reminder acknowledgment tracking |
| 5 | Implement shared appointment calendar with add/edit/view, reminder configuration, and Google Calendar sync integration |
| 6 | Build task board: kanban UI with drag-and-drop, task CRUD, assignment, completion tracking, recurring task logic, and push notification on assignment/completion |
| 7 | Implement health journal: entry logging with structured fields per type (vitals, mood, symptoms), chronological feed, and basic trend charts for vitals |
| 8 | Build emergency contact sheet, document vault (S3 upload with encryption), dashboard home screen with summary cards, and Stripe subscription paywall |
| 9 | Build weekly summary email generation with SendGrid: compile care circle data into formatted email, configure delivery settings, implement "View in App" deep links |
| 10 | Alpha testing with 10 caregiver families recruited from r/AgingParents; gather feedback on task assignment flow, medication reminders, and onboarding UX; fix critical bugs |
| 11 | Beta launch: invite 50 families; iterate on top feedback items; optimize notification delivery reliability; finalize App Store/Play Store listings with screenshots and description |
| 12 | Public launch: submit to App Store and Play Store; post genuine launch story on r/AgingParents, r/CaregiverSupport, and caregiver Facebook groups; contact 5 local Area Agencies on Aging; begin paid Facebook ad campaign targeting "caring for aging parents" interests |

## 11. Growth Loops

### Viral Loop: Care Circle Invitations
The core product mechanic is inherently viral. When one sibling creates a care circle and invites 2-3 other family members, each invited member is a potential new paying customer for their own family's care circle (e.g., a brother-in-law may also be coordinating care for his own parents). The invitation message is personalized: "Sarah invited you to join Mom's care circle on Elderly Care Coordinator." Each care circle averages 3.2 members, giving every new family 2+ organic acquisition opportunities.

### Engagement Loop: Task Accountability
When a task is assigned, the assignee receives a push notification. When the task is completed, the creator receives a notification. This creates a reciprocal engagement loop that keeps all family members opening the app regularly. Uncompleted tasks generate escalating reminders, reinforcing the habit.

### Content Loop: Caregiver Community
Publish weekly caregiving tips (medication management, communicating with doctors, self-care for caregivers) via blog and email newsletter. These tips are shareable and position the app as a trusted resource in caregiver communities, driving organic search traffic and social sharing.

### Retention Loop: Data Lock-In
Over time, the care circle accumulates irreplaceable data: medication history, health journal entries, uploaded documents, and task history. This data becomes the family's care record, making switching extremely costly and driving long-term retention (estimated 18+ month average).

## 12. Regulatory & Compliance

- **HIPAA Considerations**: While the app is not technically a "covered entity" under HIPAA (it's a consumer tool, not a healthcare provider or insurer), storing medication lists, health journals, and medical documents creates de facto health data. Implement HIPAA-grade security practices voluntarily: encryption at rest (AES-256) and in transit (TLS 1.3), access logging, and data segregation by care circle.
- **SOC 2 Type I Certification**: Target by Month 12 to build trust with families and potential healthcare partnerships. Demonstrates security controls, availability, and confidentiality practices.
- **Data Privacy**: CCPA, VCDPA, and other state privacy laws apply. Provide data access, export, and deletion requests honored within 30 days. Publish a clear, plain-language privacy policy. Never sell or share health data -- make this a core brand promise.
- **Children's Privacy (COPPA)**: If the app is ever extended to child dependents, COPPA compliance will be required. For MVP, restrict care recipients to adults 18+.
- **Medical Device Regulation**: The app must not position itself as a medical device or provide medical advice. Medication reminders are informational ("time to take your medication") and do not constitute clinical decision support. Disclaimers must be prominent.
- **Emergency Liability**: The emergency contact sheet and document vault are informational tools. Terms of service must disclaim liability for emergency response outcomes. The app does not replace 911 or medical emergency services.

## 13. Risk Register

| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| Low tech adoption among elderly parents and some older caregivers limits care circle completeness | High | Medium | Design parent-facing experience as SMS-only (medication reminders via text, not app); keep sibling experience simple with email summaries + one-tap task completion via link; do not require the care recipient to use the app at all |
| Apple Health or Google Health add caregiver coordination features, leveraging massive install base | Low | High | Move fast on features Big Tech won't prioritize (task assignment, sibling accountability, weekly summaries); build emotional community features (shared memory timeline, gratitude notes) that create switching costs beyond functionality |
| Medication reminder failure (missed notification) leads to missed dose with health consequences, creating liability exposure | Medium | Critical | Use redundant delivery (push + SMS via Twilio); implement retry logic for unacknowledged reminders (escalate to a second care circle member); display "last acknowledged" timestamps; add disclaimer that reminders supplement but do not replace professional medical care |
| Family conflict about unequal caregiving loads spills into negative app reviews or churn | Medium | Medium | Position the care equity dashboard as a neutral, data-driven tool rather than a blame mechanism; provide in-app tips for having constructive family conversations about caregiving; offer optional visibility settings so equity data is shared only when all members opt in |
| Slow organic growth due to sensitive, private nature of caregiving (people don't publicly share they're caring for a parent) | Medium | Medium | Focus on private community channels (closed Facebook groups, Reddit threads) rather than public social sharing; create shareable caregiver resource content (checklists, tip sheets) that drives app awareness without requiring users to share personal details |
| Data breach exposing sensitive health and family information destroys trust and creates legal liability | Low | Critical | Encrypt all data at rest and in transit; implement role-based access control per care circle; conduct annual third-party security audit; carry cyber liability insurance; pursue SOC 2 certification; implement data breach notification procedures per state requirements |

## 14. Success Criteria
- **6-month go/no-go**: 500+ paid families, 10%+ free-to-paid conversion rate, $5,000+ MRR, 3.0+ care circle members per family (validating viral loop), 85%+ medication reminder acknowledgment rate, and <5% monthly family churn rate
- **12-month milestone**: 1,200+ paid families, $12,000+ MRR, 4.4+ App Store rating, partnerships with 3+ Area Agencies on Aging or caregiver organizations, weekly summary email open rate of 60%+, and at least one AARP or caregiver media feature driving organic growth
