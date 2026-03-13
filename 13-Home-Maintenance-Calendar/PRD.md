# Product Requirements Document: Home Maintenance Calendar

## 1. Executive Summary
The average homeowner spends $3,000-$4,000/year on maintenance and repairs, yet 35% perform no preventive maintenance — turning $30 problems into $5,000 emergencies. Home Maintenance Calendar generates a personalized annual maintenance schedule based on a homeowner's specific property (age, location, HVAC type, roof material, appliances, yard size), delivers monthly task reminders with DIY instructions and cost estimates, and tracks maintenance expenses over time. The primary target user is a first-time homeowner aged 28-40 who just closed on their first house and has no idea what upkeep it requires. At $4.99/month for the personalized experience (free tier offers a generic checklist), the product addresses a $610M market segment with high natural retention — home maintenance is ongoing and seasonal. Year 1 revenue target is $120K from 2,000 paid subscribers, driven by SEO content ("home maintenance checklist by month"), Reddit engagement in r/homeowners and r/firsttimehomebuyer, and partnerships with real estate agents who can gift the app to closing clients.

## 2. User Personas

### Persona 1: Tyler and Priya Mehta
- **Ages**: 31 and 29
- **Jobs**: Tyler is a high school teacher; Priya is a UX designer (remote)
- **Income**: $115,000 combined household
- **Location**: Just purchased their first home — a 2004-built 3BR/2BA ranch in Raleigh, NC
- **Pain Points**: Don't know what maintenance a house needs; their home inspector gave them a binder at closing and they haven't opened it; worried about the HVAC (original from 2004) but don't know what to do; already had a minor plumbing issue they ignored until it got worse
- **Goals**: Get a simple, month-by-month guide for what to do and when; avoid surprise repair costs; feel confident they're taking care of their investment
- **Tech Comfort**: High — both use apps daily; want something that integrates with their existing calendar

### Persona 2: Greg Donovan
- **Age**: 52
- **Job**: Operations manager at a logistics company
- **Income**: $95,000
- **Location**: Owns a 1988-built 4BR colonial in suburban Chicago, IL; has lived there for 15 years
- **Pain Points**: Just had a $7,500 HVAC replacement because he never serviced the system; knows he's been neglecting his home but doesn't have a system for keeping track; hates calling contractors because he doesn't know who to trust
- **Goals**: Get a proactive maintenance system so he doesn't have another expensive surprise; find reliable local contractors for tasks he won't DIY; track what he's spent on the house
- **Tech Comfort**: Moderate — uses his phone for basics but prefers straightforward apps without too many features

### Persona 3: Lisa Moreno
- **Age**: 36
- **Job**: Nurse practitioner
- **Income**: $88,000
- **Location**: Owns a 2018-built 2BR condo in Phoenix, AZ
- **Pain Points**: Thought condo maintenance was handled by the HOA, but many items (HVAC filters, water heater, appliance maintenance) are her responsibility; the desert climate creates specific maintenance needs (AC maintenance, evaporative cooler care) she's unfamiliar with
- **Goals**: Know exactly which maintenance items are her responsibility vs. the HOA's; get climate-specific reminders (e.g., AC tune-up before Arizona summer); keep a record for her own reference and for resale
- **Tech Comfort**: High — uses health/wellness apps regularly; appreciates push notifications

## 3. User Stories (20+)
1. As a homeowner, I want to enter my home's details (age, location, systems, materials) so that I receive a personalized maintenance schedule.
2. As a homeowner, I want to see a month-by-month calendar of maintenance tasks so that I know what to do and when.
3. As a homeowner, I want push notification reminders for upcoming tasks so that I don't forget time-sensitive maintenance.
4. As a homeowner, I want each task to explain why it matters (cost of neglect) so that I'm motivated to complete it.
5. As a homeowner, I want DIY instructions or video links for each task so that I can do it myself if I choose.
6. As a homeowner, I want to see estimated costs for hiring a professional for each task so that I can budget accordingly.
7. As a homeowner, I want to mark tasks as completed so that I can track my maintenance history.
8. As a homeowner, I want to log the cost I spent on each completed task so that I can track my total maintenance spending.
9. As a homeowner, I want to see my cumulative "money saved" by doing preventive maintenance so that I see the value of my effort.
10. As a homeowner, I want reminders to be adjusted for my climate zone (e.g., winterizing in cold climates, AC prep in hot climates) so that they're relevant to where I live.
11. As a homeowner, I want to add my specific appliances (brand, model, age) so that maintenance intervals are accurate for my equipment.
12. As a homeowner, I want to find rated local contractors for tasks I don't want to DIY so that I can hire someone trustworthy.
13. As a homeowner, I want to see a "home health score" that reflects how well-maintained my home is so that I have a quick status overview.
14. As a homeowner, I want to receive a quarterly "home health report" via email so that I stay engaged even if I don't open the app daily.
15. As a homeowner, I want to snooze or reschedule a task if I can't get to it this month so that it doesn't disappear from my list.
16. As a homeowner, I want to add custom tasks (e.g., "stain the deck," "power wash driveway") to my calendar so that all maintenance is in one place.
17. As a homeowner, I want to see how each maintenance task impacts my home's resale value so that I understand the return on investment.
18. As a first-time homeowner, I want an onboarding guide explaining the most critical maintenance tasks for Year 1 so that I prioritize correctly.
19. As a homeowner, I want to share my maintenance calendar with my spouse or partner so that we can divide tasks.
20. As a homeowner, I want to see seasonal preparation checklists (winterizing, spring opening, hurricane prep) so that I'm ready for weather events.
21. As a homeowner, I want to store documents related to my home (warranty cards, contractor receipts, inspection reports) so that everything is in one place.
22. As a homeowner, I want to see which tasks I've been skipping so that I can address maintenance gaps before they become problems.
23. As a condo owner, I want to distinguish between my maintenance responsibilities and my HOA's so that I only see tasks relevant to me.

## 4. Feature Requirements

### MVP (v1.0) — Must Have
- [ ] Home profile setup: input home age (year built), location (zip code), HVAC type (central air, heat pump, boiler, etc.), roof material (asphalt shingle, metal, tile), foundation type, yard size, and number of bathrooms
- [ ] Personalized calendar generation: algorithm that produces a 12-month maintenance schedule based on the home profile, adjusting for climate zone and seasonality
- [ ] Monthly task cards: each task displays the task name, why it matters (cost-of-neglect framing), estimated time to DIY, estimated cost to hire, and a difficulty rating (easy/medium/hard)
- [ ] Push notification reminders: configurable reminders (1 week before, day-of) for each upcoming task; users can set preferred reminder time
- [ ] Task completion tracking: mark tasks as done with optional date and cost fields; completed tasks move to a history log
- [ ] Seasonal checklists: pre-built checklists for fall winterizing, spring opening, and summer AC prep, personalized to the user's climate zone
- [ ] DIY resource links: curated YouTube video links and article links for each maintenance task
- [ ] Expense tracker: log cost for each completed task; dashboard shows YTD and lifetime maintenance spending by category
- [ ] Home health score: a simple 0-100 score based on task completion rate, updated monthly
- [ ] Task snooze/reschedule: move an incomplete task to next month with a single tap; snoozed tasks appear with a warning indicator
- [ ] Free tier experience: generic annual maintenance checklist (not personalized) with 3 seasonal reminders per year; paywall gates personalization, monthly push reminders, cost tracking, and home health score
- [ ] User authentication: email/password + Apple/Google sign-in

### v2.0 — Should Have
- [ ] Vendor directory: searchable list of rated local contractors by trade (HVAC, plumbing, electrical, roofing, landscaping) with reviews and contact info
- [ ] Appliance inventory: add specific appliances with brand, model, purchase date, and warranty expiration; app adjusts maintenance intervals based on manufacturer recommendations
- [ ] Shared calendar: invite a household member (spouse, partner, roommate) to view and manage the same maintenance calendar
- [ ] Quarterly home health report: automated email report summarizing tasks completed, tasks skipped, estimated savings, and upcoming priorities
- [ ] Document storage: upload and store warranty documents, inspection reports, contractor receipts, and home insurance policies (up to 2GB)
- [ ] Custom task creation: add user-defined tasks with custom recurrence intervals
- [ ] Calendar integration: export maintenance tasks to Google Calendar, Apple Calendar, or Outlook via iCal feed
- [ ] Climate-event alerts: push notifications for severe weather prep (hurricane, freeze warning, wildfire smoke) based on location and weather data

### v3.0 — Nice to Have
- [ ] Vendor booking: request quotes and book contractors directly through the app; earn affiliate revenue per booked job
- [ ] Home value protection dashboard: estimate how deferred maintenance impacts resale value based on home age and market data
- [ ] Neighborhood maintenance benchmarks: anonymized comparison of maintenance spending and completion rates among homes in the user's area
- [ ] Smart home integration: connect to Nest/Ecobee thermostats or smart water leak detectors to trigger maintenance alerts based on real-time data
- [ ] Rental property support: manage maintenance calendars for multiple properties for landlords or investors

## 5. Technical Architecture
- **Frontend**: React Native (Expo) — cross-platform mobile app (iOS + Android) for push notifications and on-the-go task management; calendar and task list interfaces are natively mobile patterns; Expo streamlines builds for a solo dev
- **Backend**: Node.js on AWS Lambda — serverless functions handle calendar generation, reminder scheduling, and vendor data lookups; low operational overhead; scales with user growth
- **Database**: PostgreSQL (via Supabase) — relational model for structured home profiles, task schedules, and completion logs; Supabase provides auth, file storage (for document uploads), and row-level security
- **Key APIs**:
  - OpenWeatherMap API — climate zone detection and weather-based reminder adjustments (freeze warnings, heat waves)
  - Firebase Cloud Messaging / APNs — push notification delivery for task reminders
  - Google Maps/Places API — location-based vendor directory and contractor search
  - Stripe API — subscription billing ($4.99/month and $9.99/month premium)
  - YouTube Data API — curated DIY video links for each maintenance task
  - AWS S3 (via Supabase Storage) — document and receipt image storage
- **Hosting**: AWS Lambda + Supabase — estimated $60/month at launch; Lambda handles API logic; Supabase handles database, auth, and storage; highly cost-effective for early stage

## 6. Data Model

### Users
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| email | String | User email, unique |
| subscription_status | Enum | free, standard, premium |
| stripe_customer_id | String | Stripe reference |
| created_at | Timestamp | Account creation |

### Homes
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| address | String | Home address |
| zip_code | String | For climate zone lookup |
| year_built | Integer | Year the home was built |
| hvac_type | Enum | central_air, heat_pump, boiler, baseboard, window_units |
| roof_material | Enum | asphalt_shingle, metal, tile, wood_shake, flat |
| foundation_type | Enum | slab, crawlspace, basement |
| yard_size | Enum | none, small, medium, large |
| num_bathrooms | Integer | Number of bathrooms |
| climate_zone | String | Auto-detected from zip code (humid, arid, cold, temperate, tropical) |
| property_type | Enum | single_family, condo, townhouse |

### MaintenanceTasks (template library)
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| name | String | Task name (e.g., "Change HVAC Filter") |
| description | Text | What to do and why it matters |
| cost_of_neglect | Text | What happens if you skip this |
| estimated_diy_time | String | Time estimate (e.g., "15 minutes") |
| estimated_pro_cost | String | Cost range to hire (e.g., "$75-$150") |
| difficulty | Enum | easy, medium, hard |
| applicable_months | Array[Int] | Months when this task should be done (1-12) |
| applicable_hvac_types | Array[Enum] | Which HVAC types this applies to |
| applicable_climate_zones | Array[String] | Which climate zones this applies to |
| video_url | String | Link to DIY video |
| recurrence | Enum | monthly, quarterly, biannual, annual |

### ScheduledTasks (per-user instances)
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| home_id | UUID | FK to Homes |
| task_id | UUID | FK to MaintenanceTasks |
| scheduled_month | Integer | Month (1-12) |
| scheduled_year | Integer | Year |
| status | Enum | upcoming, completed, snoozed, skipped |
| completed_date | Date | When the user marked it done |
| cost_spent | Decimal | User-logged cost |
| notes | Text | User notes |

### Appliances
| Field | Type | Description |
|-------|------|-------------|
| id | UUID | Primary key |
| home_id | UUID | FK to Homes |
| type | Enum | hvac, water_heater, dishwasher, washer, dryer, refrigerator, etc. |
| brand | String | Manufacturer |
| model | String | Model number |
| purchase_date | Date | When purchased or installed |
| warranty_expiry | Date | Warranty end date |

**Relationships**: A User has one or more Homes. Each Home has many ScheduledTasks. Each ScheduledTask references a MaintenanceTask template. Each Home has many Appliances. The calendar generation algorithm creates ScheduledTask instances by matching MaintenanceTask templates against the Home's profile attributes.

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Home Profile Setup
A guided wizard after sign-up. Step 1: "When was your home built?" — year picker or "I don't know" option. Step 2: "What type of property?" — single family, condo, townhouse with icons. Step 3: "Where is your home?" — zip code input (auto-detects climate zone and displays it: "Climate: Humid Subtropical"). Step 4: "Tell us about your systems" — dropdowns for HVAC type, roof material, foundation type. Step 5: "Yard and bathrooms" — yard size (none/small/medium/large) and bathroom count. Final screen: "Generating your personalized calendar..." with a loading animation.

### Screen 2: Calendar View (Home Screen)
The primary screen. A monthly calendar view with colored dots indicating tasks. Below the calendar, a list of this month's tasks displayed as cards. Each card shows: task name, a colored difficulty badge (green/yellow/red), estimated time, and a checkbox. Tapping a card expands it to show the full description. A tab bar at the bottom includes: Calendar, Tasks, Spending, and Profile. A "This Month: X tasks" summary badge appears at the top.

### Screen 3: Task Detail
Tapping a task card opens a full-screen detail view. Top section shows the task name and difficulty badge. Below: "Why This Matters" section with cost-of-neglect framing ("Skip this and risk a $5,000 compressor failure"). Then: "How to DIY" with step-by-step instructions and an embedded YouTube video. Below that: "Hire a Pro" showing estimated cost range and a "Find Local Contractors" button. At the bottom: "Mark as Done" button that opens the completion form (date, cost spent, optional notes).

### Screen 4: Task Completion
After tapping "Mark as Done," a short form appears: "When did you complete it?" (date picker, defaults to today), "How much did you spend?" (dollar input, optional), and "Any notes?" (text field, optional). After saving, a celebratory confirmation: "Nice work! You just prevented $X in potential repair costs. Your home health score is now Y." The task moves to the completed history.

### Screen 5: Seasonal Checklist
A dedicated screen for seasonal preparation. Users select a season (Fall Winterizing, Spring Opening, Summer AC Prep, Hurricane Prep). The screen shows a checklist of 8-15 tasks specific to their climate zone, each with a checkbox. Completed items show a green checkmark. A progress bar at the top shows "7 of 12 tasks complete." Tasks are linkable to the full task detail view.

### Screen 6: Spending Dashboard
A visual overview of maintenance spending. Top card shows: "Total Spent This Year: $X" and "Total Spent Lifetime: $Y." Below: a bar chart showing monthly spending over the past 12 months. Then: a category breakdown (HVAC, plumbing, electrical, exterior, landscaping) as a horizontal bar chart. A "Savings Estimate" card shows: "By doing preventive maintenance, you've avoided approximately $X in emergency repairs." Tapping any category shows individual expense entries.

### Screen 7: Home Health Score
A circular gauge showing the home health score (0-100) with color coding (red <40, yellow 40-70, green >70). Below: a breakdown of what's contributing to the score — tasks completed on time (positive), tasks skipped (negative), and tasks snoozed (neutral). A "Tasks Needing Attention" list shows overdue or snoozed items. A "Improve Your Score" button links to the most critical overdue tasks.

### Screen 8: Vendor Directory
A searchable list of local contractors organized by trade. Each listing shows: business name, trade specialty, average rating (stars), number of reviews, and phone number/website. Users can filter by trade (HVAC, plumbing, roofing, etc.) and sort by rating or distance. Tapping a listing shows a detail page with full reviews and a "Call" or "Request Quote" button. A "Recommended by Neighbors" badge appears on highly-rated contractors in the user's zip code.

### Screen 9: Document Storage
A file cabinet interface for home-related documents. Categories include: Warranties, Inspection Reports, Insurance Policies, Contractor Receipts, and Manuals. Users can upload photos or PDFs using the phone camera or file picker. Each document shows a thumbnail, upload date, and category tag. A search bar allows finding documents by name or category. A "Warranty Expiring Soon" alert appears for appliances approaching warranty expiration.

### Screen 10: Settings & Notifications
Profile settings: edit home details, update appliance inventory, manage subscription. Notification preferences: set preferred reminder time (morning/evening), toggle weekly digest email, enable or disable individual task category reminders. Shared access: invite a household member by email. Data management: export maintenance history as CSV, delete account.

## 8. Monetization Implementation

**Paywall Placement**: The free tier provides a generic annual maintenance checklist (not personalized to the user's home) and 3 seasonal reminders per year — enough to demonstrate the concept. The paywall gates the personalized calendar (based on home age, climate, systems), monthly push notification reminders, DIY video links, expense tracking, and the home health score.

**Upgrade Triggers**:
- After the user enters their home details and sees the generic checklist: "Your 2004-built home in a humid climate needs a very different maintenance plan than a 2020 build in the desert. Unlock your personalized calendar — $4.99/month."
- When a seasonal event approaches: "A freeze warning is expected next week. Upgrade for your personalized winterizing checklist."
- After a user marks a task as complete: "Nice! Track all your maintenance spending and see how much you're saving. Upgrade to unlock expense tracking."

**Pricing Psychology**:
- $4.99/month is framed against the cost of one emergency repair: "Less than a single HVAC service call to prevent a $5,000 breakdown."
- The premium tier ($9.99/month) adds contractor booking and detailed home inventory — positioned for homeowners who prefer to hire pros rather than DIY.
- Annual plan option at $49.99/year (17% savings) is offered after the first 2 months to reduce churn and lock in revenue.
- First-time homeowners are offered a 3-month free trial when onboarded through a real estate agent partner — this drives high initial adoption and converts to paid after the trial when users are already engaged.

## 9. Analytics & KPIs
| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| Monthly Active Users | 200 | 3,000 | 6,000 |
| Paid Subscribers | 15 | 800 | 2,000 |
| Free-to-Paid Conversion Rate | 5% | 7% | 7% |
| Monthly Recurring Revenue | $75 | $3,800 | $10,000 |
| Task Completion Rate (% of reminders marked done) | 30% | 40% | 45% |
| Monthly Churn Rate | 5% | 3.5% | 3% |
| Average Maintenance Spending Logged per User/Year | $500 | $1,500 | $2,500 |
| Home Profiles Created | 250 | 3,500 | 7,000 |
| Organic Search Traffic (monthly) | 300 | 5,000 | 15,000 |
| Net Promoter Score | 45 | 50 | 55 |

## 10. 12-Week Launch Plan
| Week | Milestone |
|------|-----------|
| 1 | Finalize tech stack; set up React Native (Expo) project, Supabase database, and AWS Lambda functions; design the maintenance task template library (research 60+ common maintenance tasks with seasonal and system-specific attributes) |
| 2 | Build home profile setup wizard (year built, location, HVAC, roof, foundation, yard); implement climate zone auto-detection from zip code using weather API |
| 3 | Build personalized calendar generation algorithm: match maintenance task templates against home profile attributes; create ScheduledTask instances for 12-month calendar |
| 4 | Build monthly calendar view and task card UI; implement task detail screen with "Why This Matters," DIY instructions, and estimated costs |
| 5 | Implement push notification system (Firebase Cloud Messaging); build task completion flow with cost logging; build home health score calculation |
| 6 | Build seasonal checklists (fall winterizing, spring opening, summer AC prep); implement free tier vs. paid tier access gates; integrate Stripe subscription billing |
| 7 | Build spending dashboard with charts; internal QA and end-to-end testing; recruit 15 beta testers from r/homeowners and r/firsttimehomebuyer |
| 8 | Beta testing: collect feedback on task relevance, calendar accuracy, and UX; fix critical bugs; curate DIY YouTube video links for top 40 maintenance tasks; set up Mixpanel analytics |
| 9 | Public launch: submit to App Store and Google Play; publish on Reddit (r/homeowners, r/firsttimehomebuyer, r/HomeImprovement); share free seasonal PDF checklists as lead magnets |
| 10 | Publish first 6 SEO articles ("home maintenance checklist by month," "first-year homeowner guide," "when to change HVAC filter"); begin outreach to 50 real estate agents for partnership pilot |
| 11 | Analyze first 2 weeks of launch data; optimize onboarding completion rate; A/B test push notification frequency and timing; begin building vendor directory (v2 feature, early research) |
| 12 | Month 3 retrospective: evaluate KPIs against targets; plan v2 roadmap (vendor directory, appliance inventory, shared calendar); sign 5 real estate agent partnerships for co-branded new homeowner packages; publish 6 more SEO articles |

## 11. Growth Loops

**Real Estate Agent Distribution Loop**: Agents gift a free 3-month premium trial to every buyer at closing. The new homeowner uses the app during the critical "just moved in" period, converts to paid, and tells other new homeowners. Agents share the partnership with other agents, creating a distribution flywheel.

**"Money Saved" Sharing Loop**: The app tracks estimated savings from preventive maintenance ("By changing your HVAC filter on time, you avoided a potential $5,000 compressor failure"). Users share these savings milestones on social media, creating organic testimonials.

**Seasonal Re-engagement Loop**: Four times a year, the app sends seasonal preparation checklists (winterizing, spring, summer, hurricane). These re-engage lapsed users and trigger sharing: "Have you winterized your house yet? This app told me exactly what to do."

**Home Inspector Referral Loop**: Home inspectors recommend the app to every buyer they work with, often at the same time as the inspection report. The app reinforces the inspector's findings, creating mutual value. Inspectors share the partnership with their network.

**Neighborhood Word-of-Mouth**: When one homeowner in a neighborhood starts maintaining their home better, neighbors notice and ask what changed. The app becomes a recommendation topic at neighborhood gatherings and on Nextdoor. The vendor directory reinforces this: "Who's your HVAC guy? The app told me to call them."

## 12. Regulatory & Compliance

**Data Privacy**: Home addresses and property details are sensitive personal information. Comply with CCPA and any applicable state privacy laws. Allow users to delete all data including their home profile. Do not sell or share home data with real estate companies, insurers, or data brokers.

**Contractor Directory Liability**: The app must clearly state that contractor listings are provided for convenience and do not constitute an endorsement. Verify that listed contractors hold valid licenses and insurance where required by state law. Include a disclaimer: "Home Maintenance Calendar does not employ, endorse, or guarantee the work of any contractor."

**Home Value Claims**: The "home value protection score" and "money saved" estimates are projections based on industry averages, not appraisals. Clearly label these as estimates: "Based on national average repair costs from HomeAdvisor. Actual costs vary by location and contractor."

**DIY Safety**: Maintenance instructions should include safety warnings where applicable (electrical work, roof access, chemical use). Include a general disclaimer that DIY tasks are performed at the user's own risk. Do not provide instructions for tasks requiring a licensed professional (e.g., gas line work, electrical panel modifications).

**Push Notification Consent**: Obtain explicit opt-in for push notifications per Apple and Google guidelines. Provide granular notification controls (task reminders, seasonal alerts, marketing) so users can customize their experience.

## 13. Risk Register
| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| User engagement decay: homeowners set up the app then ignore reminders after 2-3 months, leading to churn | High | High | Frame reminders with cost-of-neglect urgency; send quarterly home health reports via email; add cumulative "money saved" counter as ongoing motivation; offer seasonal checklists as re-engagement hooks |
| Personalization accuracy: different home ages, climates, and systems create thousands of permutations that are difficult to model correctly for every home | High | Medium | Start with 20 common home archetypes and expand based on feedback; let users override/customize their schedule; validate task recommendations with a licensed home inspector; display a "Does this apply to your home?" feedback button on each task |
| Contractor directory quality: a bad referral (unlicensed, overpriced, poor work) immediately destroys user trust | Medium | High | Launch vendor directory only in 5 metros initially; require license and insurance verification; collect user reviews and remove contractors below 4.0 stars; charge lead fees (not listing fees) to filter unserious providers |
| Competition from established home service marketplaces (Thumbtack, Angi, HomeAdvisor) adding maintenance scheduling features | Medium | Medium | Differentiate on personalization and simplicity (not a marketplace — a maintenance planner); build strong brand in the first-time homeowner segment; focus on content and education, not transactions |
| Low willingness to pay: homeowners may expect maintenance checklists to be free (many free PDFs exist online) | Medium | Medium | Demonstrate clear value differentiation: personalized scheduling, push reminders, climate adjustment, and expense tracking are meaningfully better than a static PDF; offer a generous free tier that hooks users before the paywall |
| Seasonal download spikes: new homeowners cluster around spring/summer buying seasons, creating uneven growth | Medium | Low | Time marketing spend to align with peak homebuying season (April-August); annual plans smooth revenue; build content and SEO presence year-round |
| DIY instructions leading to injury or property damage, creating liability exposure | Low | High | Include safety warnings on all tasks; restrict instructions to tasks appropriate for average homeowners; clearly state that electrical, gas, and structural work requires a licensed professional; carry general liability insurance |

## 14. Success Criteria
- **6-month go/no-go**: 800+ paid subscribers, $3,800+ MRR, 7% free-to-paid conversion rate, task completion rate above 40% (users are actually following the calendar), monthly churn below 4%, and at least 5 real estate agent partnerships actively distributing the app
- **12-month milestone**: 2,000+ paid subscribers, $10,000+ MRR ($120K annualized), 6,000+ registered users, 55+ NPS score, top-5 Google ranking for "home maintenance calendar app" and "first-time homeowner checklist," and at least $2,500 average annual maintenance spending tracked per active user
