# Product Requirements Document: Pet Health Vault

## 1. Executive Summary
Pet owners across 86.9 million US households struggle to track vaccinations, medication schedules, and vet visit histories, with 40% of pets falling behind on vaccinations because owners lose paper records or forget due dates. Pet Health Vault is a mobile-first digital health record keeper that lets owners create pet profiles, log vet visits, receive automated vaccination and medication reminders, access breed-specific health alerts, and share a QR-code health card with any vet, groomer, or pet sitter. The target user is a 25-45-year-old "pet parent" who already uses apps for everyday tasks but has no digital system for pet health. With a freemium model (free for 1 pet, $3.99/mo for multiple pets and premium features), a projected LTV:CAC of 13.7:1, and a $1.4B serviceable addressable market, Pet Health Vault has a clear path to $1.2M ARR within three years.

## 2. User Personas

### Persona 1: Sarah, the Multi-Pet Millennial
- **Age**: 32
- **Job**: Marketing coordinator
- **Income**: $68,000/year
- **Pets**: 2 dogs (Golden Retriever, Dachshund), 1 cat
- **Pain Points**: Has vet records scattered across three different clinics; missed her Dachshund's DHPP booster because she confused it with the Golden's schedule; spent 20 minutes digging through email last time the boarding facility asked for proof of rabies vaccination
- **Goals**: One place for every pet's records; automated reminders so nothing slips; easy sharing when she boards dogs for vacation
- **Tech Comfort**: High — uses apps for banking, fitness, meal planning

### Persona 2: Mark, the New Dog Dad
- **Age**: 28
- **Job**: Software engineer
- **Income**: $95,000/year
- **Pets**: 1 puppy (Labrador, 4 months old)
- **Pain Points**: Overwhelmed by the puppy vaccination schedule (3-4 rounds in the first year); doesn't know which breed-specific screenings to request; wants to track weight gain to ensure healthy growth
- **Goals**: A clear vaccination timeline with reminders; breed health education; weight tracking with growth charts
- **Tech Comfort**: Very high — early adopter of new tools

### Persona 3: Linda, the Pet Sitter
- **Age**: 45
- **Job**: Professional pet sitter (manages 8-12 client pets)
- **Income**: $42,000/year
- **Pain Points**: Clients text her blurry photos of vet records; she needs to confirm vaccination status before accepting a new pet; no standardized way to see a pet's allergies or medications
- **Goals**: Receive a shareable health card from each client; quickly verify vaccination status; know emergency medication instructions
- **Tech Comfort**: Moderate — uses scheduling apps and Instagram for her business

## 3. User Stories (20+)
1. As a pet owner, I want to create a profile for each of my pets so that I have a central record of their breed, age, weight, and microchip number.
2. As a pet owner, I want to log vet visits with notes and diagnoses so that I have a complete medical history in one place.
3. As a pet owner, I want automated vaccination reminders sent before due dates so that my pets never fall behind on shots.
4. As a pet owner, I want medication reminders with dosage details so that I give the right amount at the right time.
5. As a pet owner, I want breed-specific health alerts so that I know which screenings to request at the right age.
6. As a pet owner, I want to generate a shareable QR code health card so that vets, groomers, and boarders can instantly view my pet's records.
7. As a pet owner, I want to track my pet's weight over time with charts so that I can monitor growth and detect unhealthy trends.
8. As a pet owner, I want to find emergency vets near me with after-hours availability so that I know where to go in a crisis.
9. As a multi-pet owner, I want a dashboard showing all my pets' upcoming appointments and reminders so that I can manage multiple schedules at a glance.
10. As a pet owner, I want to upload photos of paper vet records and have key data extracted automatically so that I don't have to type everything manually.
11. As a pet owner, I want to export my pet's full health history as a PDF so that I can share it with a new vet or keep a backup.
12. As a pet owner, I want to record my pet's allergies prominently so that any caregiver can see them immediately.
13. As a pet sitter, I want to receive a shared health card link so that I can view a client's pet records without creating an account.
14. As a pet owner, I want to log grooming appointments and notes so that I track skin/coat issues alongside medical records.
15. As a pet owner, I want to set a recurring flea/tick/heartworm prevention schedule so that I never miss a monthly dose.
16. As a pet owner, I want to see a timeline view of all vet visits and vaccinations so that I can visualize my pet's health history.
17. As a pet owner, I want to add my vet clinic's contact information so that I can call or navigate to them directly from the app.
18. As a pet owner, I want to receive a push notification when my pet is due for an annual checkup so that I schedule proactively.
19. As a pet owner, I want to store insurance policy details alongside health records so that I have claim information handy at the vet.
20. As a pet owner whose pet has passed away, I want a memorial mode that preserves records without sending reminders so that I am not hurt by notifications.
21. As a pet owner, I want to compare my pet's weight to breed-average growth curves so that I know if my puppy is on track.
22. As a pet owner, I want to attach lab results and diagnostic images to vet visits so that everything is in one file.

## 4. Feature Requirements

### MVP (v1.0) — Must Have
- [ ] Pet profile creation with name, breed, species, age, weight, photo, microchip number, and allergies (acceptance: user can create, edit, and delete profiles; all fields save and persist)
- [ ] Vet visit log with date, clinic name, vet name, diagnosis, treatment notes, and follow-up date (acceptance: entries display in reverse chronological order; support text and photo attachments)
- [ ] Vaccination tracker with vaccine name, date administered, and next-due date (acceptance: system auto-calculates next-due based on standard schedules by species)
- [ ] Automated push notification reminders for upcoming vaccinations (acceptance: reminders fire 30, 14, and 3 days before due date; user can customize intervals)
- [ ] Medication schedule with drug name, dosage, frequency, start/end date, and push reminders (acceptance: user receives reminders at scheduled times; can mark dose as given or skipped)
- [ ] Breed-specific health alerts based on known breed predispositions (acceptance: alerts surface on the pet profile screen at appropriate ages; sourced from AVMA/breed club guidelines)
- [ ] Shareable QR code health card containing vaccination status, allergies, and medications (acceptance: QR code opens a read-only web view accessible without login; owner can revoke access)
- [ ] Weight tracking with a simple line chart over time (acceptance: user enters weight with date; chart renders with at least 3 data points)
- [ ] Emergency vet locator using device GPS (acceptance: shows nearest 5 emergency vet clinics with phone number, address, and hours; opens in Maps app)
- [ ] User authentication with email/password and social login (acceptance: supports email, Google, and Apple sign-in; password reset flow works)
- [ ] Free tier limited to 1 pet profile; paywall prompt when adding a second pet (acceptance: upgrade screen displays pricing and feature comparison; links to App Store/Google Play subscription)

### v2.0 — Should Have
- [ ] OCR receipt and document scanning to auto-extract vaccination dates, product names, and vet clinic info from uploaded photos
- [ ] Gmail/email integration to auto-import vet invoices and vaccination confirmations
- [ ] PDF export of full pet health record with customizable sections
- [ ] Multi-user household sharing so both partners can access and edit pet profiles
- [ ] Vet clinic contact directory with phone, address, and one-tap navigation
- [ ] Grooming and dental appointment tracking
- [ ] Breed-average growth curve overlay on weight charts
- [ ] Insurance policy storage with carrier name, policy number, and claim phone number

### v3.0 — Nice to Have
- [ ] B2B vet practice dashboard allowing clinics to push records directly to owner accounts
- [ ] Pet insurance marketplace with comparison quotes (affiliate revenue)
- [ ] Integration with top 3 veterinary practice management systems (IDEXX, eVetPractice, Cornerstone)
- [ ] Community forum for breed-specific health discussions
- [ ] AI-powered symptom checker providing triage guidance (not diagnosis)

## 5. Technical Architecture
- **Frontend**: React Native (Expo) — enables a single codebase for iOS and Android, fast iteration, and over-the-air updates; Expo's camera and push notification modules accelerate MVP delivery
- **Backend**: Node.js with Express on AWS Lambda — serverless architecture keeps costs near zero at low scale and auto-scales as users grow; Lambda's pay-per-invocation model aligns with a bootstrapped budget
- **Database**: PostgreSQL on AWS RDS (db.t3.micro free tier to start) — relational structure fits the clearly defined entities (pets, visits, vaccinations, medications); strong data integrity for health records
- **Key APIs**:
  - Google Maps Platform (Places API) — emergency vet locator and clinic directory
  - Firebase Cloud Messaging / Apple Push Notification Service — vaccination and medication reminders
  - AWS Rekognition or Google Cloud Vision — OCR for receipt scanning (v2.0)
  - Stripe — subscription billing and payment processing
  - Auth0 or Firebase Auth — user authentication with social login support
- **Hosting**: AWS (Lambda + RDS + S3 for image storage) — estimated $60/month at MVP scale; S3 for pet photos and uploaded documents; CloudFront CDN for QR code health card web views

## 6. Data Model

### Users
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| email | String | Unique, required |
| password_hash | String | Bcrypt hashed |
| name | String | Display name |
| subscription_tier | Enum | free, premium |
| subscription_expires_at | Timestamp | Null for free tier |
| created_at | Timestamp | |

### Pets
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| name | String | Required |
| species | Enum | dog, cat, other |
| breed | String | Nullable |
| date_of_birth | Date | Nullable |
| weight_current | Decimal | Pounds or kg |
| microchip_number | String | Nullable |
| photo_url | String | S3 path |
| allergies | Text | Free-text |
| status | Enum | active, memorial |
| created_at | Timestamp | |

### Vet Visits
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| pet_id | UUID | FK to Pets |
| visit_date | Date | Required |
| clinic_name | String | |
| vet_name | String | Nullable |
| diagnosis | Text | |
| treatment_notes | Text | |
| follow_up_date | Date | Nullable |
| attachments | JSON | Array of S3 URLs |

### Vaccinations
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| pet_id | UUID | FK to Pets |
| vaccine_name | String | e.g., Rabies, DHPP |
| date_administered | Date | Required |
| next_due_date | Date | Auto-calculated or manual |
| administering_clinic | String | Nullable |
| lot_number | String | Nullable |

### Medications
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| pet_id | UUID | FK to Pets |
| drug_name | String | Required |
| dosage | String | e.g., "50mg" |
| frequency | String | e.g., "twice daily" |
| start_date | Date | |
| end_date | Date | Nullable (ongoing) |
| reminder_times | JSON | Array of times |

### Weight Logs
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| pet_id | UUID | FK to Pets |
| weight | Decimal | Required |
| recorded_date | Date | Required |

### Shared Health Cards
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| pet_id | UUID | FK to Pets |
| token | String | Unique, used in QR URL |
| is_active | Boolean | Owner can revoke |
| created_at | Timestamp | |

**Relationships**: A User has many Pets. A Pet has many Vet Visits, Vaccinations, Medications, Weight Logs, and Shared Health Cards.

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Onboarding / Sign Up
The user sees a 3-slide carousel highlighting key value props (vaccination reminders, shareable QR card, breed health alerts) with illustrations. Below is a "Get Started" button leading to email/social sign-up. After registration, the user is immediately prompted to add their first pet.

### Screen 2: Pet Dashboard (Home)
A card-based layout showing each pet with their photo, name, and a quick-status badge ("All vaccines current" in green, or "DHPP due in 12 days" in amber). Tapping a pet card opens that pet's detail view. A floating "+" button lets users add a new pet (triggers paywall for free-tier users with 1 existing pet). A bottom navigation bar provides access to Home, Reminders, Emergency Vet, and Settings.

### Screen 3: Pet Profile & Health Summary
At the top, the pet's photo, name, breed, age, and weight. Below are tabbed sections: Overview (upcoming reminders, last vet visit), Vaccinations (list with status indicators), Medications (active list with next dose time), Vet Visits (chronological log), and Weight (line chart). A "Share Health Card" button at the top generates/displays the QR code.

### Screen 4: Add/Edit Vet Visit
A form with fields for visit date (date picker), clinic name (autocomplete from previous entries), vet name, diagnosis (text area), treatment notes (text area), follow-up date, and an "Attach Photo/Document" button. Saving returns to the pet's vet visit log with the new entry at the top.

### Screen 5: Vaccination Tracker
A list of all vaccinations for the selected pet, each showing vaccine name, date administered, and next due date with a countdown badge. A color-coded system: green (current), amber (due within 30 days), red (overdue). Tapping a vaccination opens an edit view. A "+" button adds a new vaccination record with auto-calculated next-due dates based on standard schedules.

### Screen 6: Medication Schedule
A list of active medications showing drug name, dosage, frequency, and next reminder time. Each medication has a "Mark as Given" quick-action button. Tapping a medication opens a detail view with the full schedule, start/end dates, and history of doses given/skipped. A "+" button adds a new medication with customizable reminder times.

### Screen 7: QR Health Card (Share View)
A screen displaying a large QR code and a shareable link below it. The user can toggle which sections to include (vaccinations, allergies, medications, emergency contact). Below the QR code is a preview of what the recipient will see: a clean, read-only web page with the pet's name, photo, vaccination status, allergies, and current medications. A "Revoke Access" button deactivates the link.

### Screen 8: Emergency Vet Locator
A map view centered on the user's current location with pins for the nearest emergency/24-hour vet clinics. Below the map is a scrollable list of clinics with name, distance, phone number (tap to call), and address (tap for directions). Filters for "Open Now" and "24-Hour Only."

### Screen 9: Breed Health Alerts
A feed of age-appropriate health alerts for the pet's breed, displayed as cards. Example: "Golden Retrievers: Schedule a hip dysplasia screening by age 2." Each card includes a brief explanation, recommended action, and a "Discuss with Vet" button that pre-populates a question to ask at the next visit. Alerts unlock progressively as the pet ages.

### Screen 10: Settings & Subscription Management
Account settings (name, email, password), notification preferences (reminder timing, quiet hours), units preference (lbs/kg), and subscription status. Free-tier users see a comparison table of free vs. premium features with an upgrade button. Premium users see their renewal date and a manage subscription link.

## 8. Monetization Implementation
The paywall is triggered naturally when a free-tier user attempts to add a second pet — this aligns with the fact that 35% of pet owners have multiple pets, making it a high-frequency conversion event. Additional premium gates include medication reminders (free tier shows the schedule but does not send push notifications for meds), breed-specific health alerts, weight charts, emergency vet locator, and PDF export. Pricing is set at $3.99/month or $34.99/year (27% annual discount) to encourage annual commitment. The annual plan is presented as the default with the monthly option secondary. A 7-day free trial of premium is offered at onboarding to demonstrate full value before the user hits a gate. Upgrade prompts appear contextually (e.g., "Upgrade to track Max's medications with reminders") rather than as interruptive pop-ups.

## 9. Analytics & KPIs
| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| New pet profiles created | 200 | 1,200/month | 2,500/month |
| Monthly Active Users (MAU) | 150 | 3,000 | 8,000 |
| Free-to-paid conversion rate | 4% | 7% | 8% |
| Monthly churn rate (paid) | 6% | 3.5% | 3% |
| QR health card shares/week | 10 | 50 | 120 |
| Vaccination reminder completion rate | 40% | 60% | 65% |
| Multi-pet upgrade rate | 15% | 25% | 28% |
| Average session duration | 3 min | 4 min | 5 min |
| App Store rating | 4.0 | 4.3 | 4.5 |
| MRR | $400 | $5,000 | $10,000 |

## 10. 12-Week Launch Plan
| Week | Milestone |
|------|-----------|
| 1 | Finalize wireframes and data model; set up React Native (Expo) project, backend repo, and CI/CD pipeline; provision AWS resources |
| 2 | Build user authentication (email + Google + Apple sign-in); implement pet profile CRUD; design and build database schema |
| 3 | Build vet visit logging with photo attachments; implement vaccination tracker with auto-calculated next-due dates |
| 4 | Build medication schedule with push notification reminders; implement weight logging and chart visualization |
| 5 | Build shareable QR health card (generation + read-only web view); implement breed-specific health alerts engine with data for top 30 dog and cat breeds |
| 6 | Build emergency vet locator with Google Maps integration; implement paywall and Stripe subscription billing; integrate freemium tier gating |
| 7 | Internal QA and bug fixes; closed beta with 20 pet owners recruited from r/dogs and personal network; collect feedback on onboarding flow and core features |
| 8 | Iterate on beta feedback; polish UI; submit to Apple App Store and Google Play Store for review; prepare App Store Optimization (ASO) assets |
| 9 | Public launch; begin Reddit GTM campaign in r/dogs, r/cats, r/GoldenRetrievers, r/puppy101; post breed-specific vaccination schedules as value content |
| 10 | Begin pet influencer outreach (10 Instagram/TikTok accounts, 10K-100K followers); launch referral program ("Give your pet sitter free access"); monitor analytics and fix critical bugs |
| 11 | Visit 15 local vet clinics with QR code table cards; begin dog park and pet store flyer campaign; post flyers at 30 locations |
| 12 | Analyze first 3 weeks of live data; publish Month 1 metrics report; prioritize v2.0 roadmap based on user feedback; begin OCR receipt scanning development |

## 11. Growth Loops

**Multi-Pet Household Loop**: Free-tier users with one pet naturally want to add their second pet, hitting the paywall. This creates a built-in conversion trigger for the 35% of pet owners with multiple pets.

**Caregiver Sharing Loop**: Every time an owner shares a QR health card with a pet sitter, groomer, boarder, or dog walker, those caregivers see the app branding and a "Create your own Pet Health Vault" CTA on the shared view. Professional pet sitters who receive cards from multiple clients are motivated to recommend the app to all their clients.

**Vet Visit Loop**: After every vet visit, the app prompts the user to log the visit and update vaccinations. The act of logging creates a moment of engagement that reinforces the habit and increases switching costs.

**Breed Community Loop**: Breed-specific health alerts and vaccination schedules are designed to be screenshot-worthy and shareable in breed-specific subreddits and Facebook groups. Owners of the same breed share and discuss alerts, driving organic discovery.

**Pet Milestone Loop**: The app sends celebratory notifications for pet birthdays and adoption anniversaries, which owners screenshot and share on social media, creating organic brand impressions.

## 12. Regulatory & Compliance

- **Data Privacy (CCPA / GDPR)**: Pet health data is not covered by HIPAA, but user personal data (email, location, payment) is subject to CCPA and GDPR. Must implement data deletion requests, data export, and transparent privacy policy. Consent must be collected for push notifications and email communications.
- **Veterinary Practice Act**: The app must not provide veterinary diagnoses or medical advice. Breed health alerts and symptom checkers must include disclaimers: "This is informational only and not a substitute for veterinary advice." Language must avoid "diagnosis" or "prescription."
- **App Store Compliance**: Apple and Google subscription guidelines require clear disclosure of pricing, trial terms, and cancellation instructions. Auto-renewal must be explicitly stated.
- **Payment Processing (PCI-DSS)**: Using Stripe handles PCI compliance; no credit card data is stored on our servers.
- **Children's Privacy (COPPA)**: While the app targets adults, if any feature could attract users under 13, COPPA compliance is needed. Current design does not target minors, but age gate should be considered.
- **Affiliate Disclosure**: Any product links or insurance marketplace referrals must comply with FTC affiliate disclosure guidelines.

## 13. Risk Register
| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| Data entry burden causes onboarding drop-off (users must manually enter existing pet records) | High | High | Build OCR receipt scanning for v2.0; offer "start fresh" onboarding path; provide a one-time $4.99 records import service |
| Vet clinic resistance to QR health card adoption | Medium | Medium | Position as reducing front-desk phone calls; build integrations with top practice management systems in v3.0; health card is owner-controlled and doesn't require vet participation |
| Emotional churn from pet loss | Medium | Medium | Implement memorial mode that preserves records without active reminders; offer PDF export as a keepsake; send a genuine condolence message, not a retention email |
| Competition from vet-side platforms (PetDesk, IDEXX Petly) adding owner-facing features | Medium | High | Differentiate on portability (works across any vet), breed health alerts, and caregiver sharing; build switching costs through accumulated health records |
| Low perceived value for single-pet free-tier users who don't hit the paywall | Medium | Medium | Add premium-gated features that are valuable even for single pets (medication reminders, breed alerts, emergency vet locator); use contextual upgrade prompts |
| Push notification fatigue leading to users disabling notifications | Low | High | Let users customize reminder frequency and quiet hours; keep notifications actionable and infrequent; never send marketing notifications through the reminder channel |

## 14. Success Criteria
- **6-month go/no-go**: 3,000 MAU with 7% free-to-paid conversion rate and monthly churn below 4%; at least 50 QR health card shares per week indicating the viral loop is functioning; MRR of $5,000
- **12-month milestone**: 8,000 MAU with 2,500 paid subscribers generating $10,000 MRR ($120K ARR); at least 5 vet clinic partnerships active; App Store rating of 4.5+; OCR receipt scanning launched and used by 30% of new sign-ups
