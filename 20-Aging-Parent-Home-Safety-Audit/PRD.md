# Product Requirements Document: Aging Parent Home Safety Audit

## 1. Executive Summary
Every year, 1 in 4 Americans aged 65+ falls, resulting in 3 million ER visits and $50 billion in medical costs, yet most homes are not safe for aging and professional home safety assessments cost $200-$500 with 3-6 month waitlists through Area Agencies on Aging. Aging Parent Home Safety Audit is a mobile application that guides adult children (or seniors themselves) through a room-by-room home safety assessment using photo-based checklists, generates a prioritized risk score, recommends modifications ranked by impact and cost, links directly to products (grab bars, non-slip mats, motion lights), and connects users to local aging-in-place contractors. The primary user is a 35-55-year-old adult child who worries about their aging parent's safety between visits. With a one-time purchase of $19.99 per full audit and a $4.99/month monitoring subscription, projected LTV of $32 and LTV:CAC of 3.2:1, the app can reach $800K in annual revenue within three years through organic search, caregiver community marketing, and senior center partnerships.

## 2. User Personas

### Persona 1: Amy, the Long-Distance Daughter
- **Age**: 43
- **Job**: Human resources manager
- **Income**: $78,000/year
- **Pain Points**: Lives 3 hours from her 74-year-old mother who lives alone; her mom had a near-fall in the bathroom last month; Amy doesn't know what to look for during her monthly visits; she called the local Area Agency on Aging and was told there's a 4-month waitlist for a professional assessment; she's anxious and guilty between visits
- **Goals**: A structured checklist she can complete on her next visit; clear recommendations prioritized by urgency; the ability to share a report with her siblings so they can coordinate modifications; peace of mind
- **Tech Comfort**: High — uses apps for everything

### Persona 2: Robert, the Proactive Retiree
- **Age**: 71
- **Job**: Retired engineer
- **Income**: $65,000/year (pension + Social Security)
- **Pain Points**: Had a hip replacement last year and realizes his home needs modifications; he's handy and wants to do some himself but doesn't know what's most important; his bathroom has no grab bars; his wife (69) has early-stage macular degeneration affecting her vision
- **Goals**: Assess his own home; prioritize the highest-impact modifications; find products he can install himself; know which modifications require a professional contractor
- **Tech Comfort**: Moderate — uses an iPad, email, and Amazon

### Persona 3: Dr. Patel, the Occupational Therapist
- **Age**: 38
- **Job**: Occupational therapist specializing in geriatric home health
- **Income**: $85,000/year
- **Pain Points**: She conducts professional home safety assessments but her waitlist is 6 weeks; she needs a structured tool she can recommend to families who can't wait; she wants a standardized assessment format that complements her clinical expertise
- **Goals**: Recommend a reliable self-assessment tool to families on her waitlist; use the app's output as a starting point for her professional assessments; refer families to the tool for initial screening
- **Tech Comfort**: High — uses clinical software and health apps daily

## 3. User Stories (20+)
1. As an adult child, I want a guided, room-by-room assessment checklist so that I know exactly what to inspect in each room of my parent's home.
2. As an adult child, I want photo-based examples of hazards (e.g., loose throw rugs, missing grab bars, poor lighting) so that I can visually compare to my parent's home.
3. As a user, I want an overall home risk score (1-10) so that I can quickly understand the severity of safety issues.
4. As a user, I want each room scored individually so that I know which room needs the most attention.
5. As a user, I want modification recommendations prioritized by impact (fall risk reduction) and cost so that I focus on the highest-value changes first.
6. As a user, I want direct product links to buy recommended items (grab bars, non-slip mats, motion-sensor lights) so that I can order them immediately.
7. As a user, I want to find local aging-in-place contractors for modifications I can't do myself (walk-in showers, stairlifts, ramp installation) so that I can get quotes.
8. As an adult child, I want to take before photos during the assessment and after photos once modifications are made so that I can track improvements.
9. As an adult child, I want to share the completed audit report with my siblings and my parent's doctor so that everyone is aligned on priorities.
10. As a user, I want reassessment reminders every 6 months so that I re-evaluate as my parent's capabilities change.
11. As a user, I want the audit to cover bathroom, bedroom, kitchen, living room, stairs/hallways, entryway, and outdoor areas so that no high-risk area is missed.
12. As a user, I want cost estimates for each recommended modification so that I can budget for changes.
13. As a senior doing a self-assessment, I want the app to frame suggestions positively as "independence enhancements" rather than "your home is unsafe" so that I feel empowered, not diminished.
14. As an adult child, I want conversation scripts for discussing safety modifications with a resistant parent so that I can approach the topic sensitively.
15. As a user, I want to mark checklist items as "not applicable" (e.g., no stairs in a single-story home) so that the assessment is tailored to the actual home.
16. As a user, I want to see which modifications I can DIY versus which require professional installation so that I plan accordingly.
17. As an occupational therapist, I want to recommend the app to families on my waitlist with confidence that it covers standard assessment criteria so that my patients get immediate value.
18. As a user, I want to track which modifications have been completed and see an updated risk score so that I measure progress.
19. As an adult child, I want to log my parent's mobility aids (walker, cane, wheelchair) so that the assessment accounts for their specific mobility level.
20. As a user, I want emergency contact information and fall response instructions included in the report so that the household is prepared.
21. As a user, I want the assessment to adapt its recommendations based on specific conditions I enter (e.g., vision impairment, balance issues, dementia) so that advice is personalized.
22. As an adult child, I want to receive a push notification when a reassessment is due so that I don't forget to re-evaluate every 6 months.

## 4. Feature Requirements

### MVP (v1.0) — Must Have
- [ ] Room-by-room guided assessment covering 7 areas: bathroom, bedroom, kitchen, living room, stairs/hallways, entryway, and outdoor/garage (acceptance: each room has 8-15 checklist items specific to that room's risks; items are based on CDC and OT fall-prevention guidelines; "not applicable" option for each item)
- [ ] Photo-based hazard examples for each checklist item showing both "hazard" and "safe" versions (acceptance: at least 2 reference photos per checklist item; photos load quickly on mobile; zoom capability)
- [ ] Room-level risk score (1-10) calculated from checklist responses, with overall home risk score aggregated across all rooms (acceptance: scoring weights bathroom and stairs higher due to elevated fall risk; score updates in real time as items are checked)
- [ ] Prioritized modification recommendations ranked by impact (fall risk reduction) and cost (acceptance: each recommendation includes description, estimated cost range, DIY vs. professional indicator, and priority level — high/medium/low; at least 40 distinct recommendations across all rooms)
- [ ] Product links for recommended items with direct links to Amazon, Home Depot, or equivalent retailers (acceptance: each product recommendation includes a clickable link; product name, approximate price, and a brief description; links open in external browser)
- [ ] Contractor finder using device location to suggest local aging-in-place remodelers and handyman services (acceptance: shows at least 3 nearby contractors with name, phone, and distance; results from Google Places API or similar; includes a "request quote" CTA)
- [ ] Before/after photo capture for each room (acceptance: user can take a "before" photo during initial assessment and an "after" photo once modifications are made; photos stored in the audit record; side-by-side comparison view)
- [ ] Shareable audit report as a PDF or web link that family members, doctors, or OTs can view (acceptance: report includes overall and room scores, prioritized recommendations, photos, and estimated costs; share via email, text, or link; view does not require login)
- [ ] Capability input: user enters parent's mobility aids (walker, cane, wheelchair, none), vision level, balance issues, and cognitive status so that recommendations are personalized (acceptance: input collected at audit start; recommendations adapt based on inputs; e.g., if wheelchair user, stair recommendations change to ramp focus)
- [ ] Free tier: bathroom-only audit with basic risk score and top 5 recommendations (acceptance: provides enough value to demonstrate the app's approach; clear prompt to upgrade for full home audit)
- [ ] One-time purchase at $19.99 for full audit unlocking all rooms (acceptance: Stripe payment; immediate access; receipt emailed; no recurring charge unless user opts into monitoring)

### v2.0 — Should Have
- [ ] Reassessment reminders at 6-month intervals with push notifications
- [ ] Capability change tracking: log changes in parent's mobility, vision, or cognitive status over time and recalculate risk scores
- [ ] Medication and emergency contact storage within the audit profile
- [ ] Conversation scripts and tips for discussing safety with a resistant parent
- [ ] Installation guides with video links for DIY modifications (grab bar placement, non-slip mat positioning, lighting upgrades)
- [ ] Updated product recommendations based on seasonal availability and price changes
- [ ] OT virtual consultation upsell ($50 per session) connecting users with occupational therapists for professional review
- [ ] Multi-home support for adult children with multiple aging parents or family members

### v3.0 — Nice to Have
- [ ] B2B licensing for home health agencies and Area Agencies on Aging (co-branded version)
- [ ] Insurance company integration: share audit results with insurance providers for fall-prevention premium discounts
- [ ] Smart home device recommendations (fall detection sensors, medical alert systems, smart lighting)
- [ ] Post-hospitalization discharge planning module (home safety assessment before a senior returns home from hospital)
- [ ] AI-powered photo analysis that auto-detects hazards from room photos (trip hazards, poor lighting, missing grab bars)

## 5. Technical Architecture
- **Frontend**: React Native (Expo) — cross-platform iOS and Android from a single codebase; Expo's camera module handles the photo-based assessment flow; offline capability via local storage so audits can be completed in homes with poor connectivity (syncs when online)
- **Backend**: Node.js with Express on AWS Lambda — serverless architecture keeps costs minimal ($40/month at MVP scale); the app is primarily a client-side assessment tool with backend handling authentication, payment, PDF generation, and contractor matching
- **Database**: PostgreSQL on AWS RDS (db.t3.micro) — relational model fits structured audit data (homes, rooms, checklist items, scores, recommendations); supports queries for reassessment tracking and capability change history
- **Key APIs**:
  - Google Maps Platform (Places API) — contractor finder for local aging-in-place remodelers and handyman services
  - Amazon Product Advertising API — product recommendation links with affiliate tracking
  - Stripe — one-time purchase and subscription payment processing
  - Firebase Cloud Messaging / APNs — push notifications for reassessment reminders
  - Puppeteer or html2pdf — server-side PDF generation for shareable audit reports
  - AWS S3 — photo storage for before/after room images
  - SendGrid — transactional emails (receipt, shared report links, reassessment reminders)
- **Hosting**: AWS (Lambda + RDS + S3 + CloudFront) — estimated $40/month at MVP scale; S3 for room photos with CloudFront CDN for shared report delivery; Lambda handles API calls on demand

## 6. Data Model

### Users
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| email | String | Unique, required |
| password_hash | String | Bcrypt |
| name | String | |
| relationship | Enum | adult_child, spouse, self, professional |
| purchase_type | Enum | free, one_time, monitoring_subscription |
| subscription_expires_at | Timestamp | Nullable |
| created_at | Timestamp | |

### Homes
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| name | String | e.g., "Mom's House" |
| address | String | For contractor matching |
| resident_name | String | The aging parent/senior |
| resident_age | Integer | |
| mobility_aids | JSON | ["walker", "cane", etc.] |
| vision_level | Enum | normal, mild_impairment, significant_impairment |
| balance_issues | Boolean | |
| cognitive_status | Enum | normal, mild_decline, moderate_decline |
| overall_risk_score | Decimal | 1-10, calculated |
| created_at | Timestamp | |

### Audits
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| home_id | UUID | FK to Homes |
| audit_date | Date | |
| overall_score | Decimal | 1-10 |
| status | Enum | in_progress, completed |
| shared_token | String | Unique token for shareable link |
| pdf_url | String | S3 path to generated PDF |
| completed_at | Timestamp | Nullable |

### Room Assessments
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| audit_id | UUID | FK to Audits |
| room_type | Enum | bathroom, bedroom, kitchen, living_room, stairs_hallways, entryway, outdoor |
| risk_score | Decimal | 1-10 |
| before_photo_url | String | S3 path |
| after_photo_url | String | S3 path, nullable |
| notes | Text | |

### Checklist Items
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| room_type | Enum | Which room this item belongs to |
| description | String | e.g., "Grab bars installed next to toilet" |
| hazard_photo_url | String | Reference photo of hazard |
| safe_photo_url | String | Reference photo of safe setup |
| risk_weight | Decimal | How much this item contributes to score |
| order | Integer | Display order |

### Checklist Responses
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| room_assessment_id | UUID | FK to Room Assessments |
| checklist_item_id | UUID | FK to Checklist Items |
| response | Enum | safe, hazard, not_applicable |
| photo_url | String | User's photo of this item, nullable |

### Recommendations
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| room_assessment_id | UUID | FK to Room Assessments |
| checklist_item_id | UUID | FK to Checklist Items (triggered by) |
| description | String | What to do |
| priority | Enum | high, medium, low |
| estimated_cost_low | Decimal | e.g., $15 |
| estimated_cost_high | Decimal | e.g., $50 |
| diy_or_professional | Enum | diy, professional, either |
| product_link | String | Affiliate URL |
| product_name | String | |
| is_completed | Boolean | User marks when done |
| completed_at | Timestamp | Nullable |

### Reassessment Schedule
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| home_id | UUID | FK to Homes |
| next_assessment_date | Date | 6 months from last audit |
| notification_sent | Boolean | |

**Relationships**: A User has many Homes. A Home has many Audits. An Audit has many Room Assessments. A Room Assessment has many Checklist Responses and Recommendations. Checklist Items is a reference table seeded with standard assessment criteria. Reassessment Schedule links to Homes.

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Onboarding / Landing
A warm, empathetic design with a calming color palette (soft greens, warm whites). Headline: "Protect Mom Before She Falls, Not After." Three-slide carousel: (1) "Room-by-room guided safety audit" with bathroom photo, (2) "Prioritized changes ranked by impact and cost" with a sample recommendation card, (3) "Share the plan with your whole family" with a shared report preview. "Start Your Free Bathroom Audit" button leads to account creation. Reassuring tone: "Simple changes like grab bars ($25) and better lighting ($15) prevent 30-40% of falls."

### Screen 2: Home Setup
Form to create the home profile: resident name, age, address. Then a capability questionnaire: mobility aids (checkboxes: none, cane, walker, wheelchair), vision level (normal / mild impairment / significant impairment), balance issues (yes/no), cognitive status (normal / mild decline / moderate decline). Clean, large-text design appropriate for possible use by seniors themselves. "Start Assessment" button proceeds to room selection.

### Screen 3: Room Selection Map
A visual floor plan or icon grid showing the 7 assessable areas: Bathroom, Bedroom, Kitchen, Living Room, Stairs & Hallways, Entryway, Outdoor/Garage. Each room shows a status indicator: not started (gray), in progress (amber), completed (green with risk score). Bathroom is highlighted as "Start Here (Highest Risk Room)" and is available in the free tier. Other rooms show a lock icon for free users with an "Unlock All Rooms — $19.99" prompt.

### Screen 4: Room Assessment (Checklist)
A scrollable checklist for the selected room (e.g., Bathroom: 12 items). Each item shows: a description ("Grab bars installed next to toilet and in shower"), a reference photo (tap to expand showing "Hazard" vs. "Safe" examples), and three response buttons (Safe / Hazard / N/A). Items flagged as "Hazard" immediately show a quick recommendation below. A camera button lets the user photograph the specific area. A progress bar at the top shows completion percentage. A running risk score updates as items are answered.

### Screen 5: Room Results & Recommendations
After completing a room's checklist, a results screen shows: room risk score (1-10) with color coding, number of hazards found, and a prioritized list of recommendations. Each recommendation card shows: what to do, estimated cost, DIY or professional indicator, priority badge (high/medium/low), and a "Buy Product" or "Find Contractor" button. User can mark recommendations as "Done" as they complete them. A "Take Before Photo" button captures the current state.

### Screen 6: Full Audit Summary
After all rooms are assessed, a comprehensive summary screen shows: overall home risk score (large, prominent), a breakdown by room (small score badges), total estimated cost for all recommended modifications (low and high range), and a count of high/medium/low priority items. A "Share Report" button generates a PDF or shareable link. A "What to Fix First" section highlights the top 5 highest-impact, lowest-cost changes.

### Screen 7: Shareable Family Report
A clean, printable/viewable report accessible via web link (no login required). Shows: resident name, assessment date, overall and room-by-room risk scores, prioritized modification list with costs, before photos, and a family action plan ("Amy: install grab bars. Mike: order non-slip mats. Dad: remove throw rug in hallway"). Designed to facilitate family coordination. A "Download PDF" button is available.

### Screen 8: Product Recommendations
A shopping-list view of all recommended products organized by room. Each product shows: name, photo, price range, retailer (Amazon/Home Depot), star rating, and a "Buy Now" affiliate link. Products are tagged as "Most Popular" or "Best Value." A total estimated cost appears at the top. Users can check off products they've ordered.

### Screen 9: Contractor Finder
A map view centered on the parent's home address with pins for local aging-in-place contractors, handyman services, and accessibility remodelers. Below the map: a list of contractors with name, distance, phone, website, and specialties (grab bars, ramps, bathroom remodels, stairlifts). A "Request Quote" button sends the contractor the audit summary (with user permission). Filter by specialty and distance.

### Screen 10: Progress Tracker & Reassessment
A dashboard showing: completed modifications (with checkmarks and after photos), remaining recommendations, updated risk score reflecting completed modifications, and next reassessment date. A "Reassess Now" button starts a new audit for comparison. A timeline view shows capability changes over time (if monitoring subscription is active). A celebratory banner appears when risk score drops below 3: "Great work! This home is now significantly safer."

## 8. Monetization Implementation
The free tier offers a bathroom-only audit (since the bathroom is the highest-risk room in any home) with a basic risk score and top 5 recommendations. This provides genuine, immediate value that demonstrates the app's approach and builds trust. The paywall activates when the user attempts to assess any room beyond the bathroom. The upgrade prompt appears naturally: "You've identified 4 hazards in the bathroom. There are 6 more rooms to assess. Unlock the full audit for $19.99." Pricing is anchored against the cost of a professional assessment ($200-$500) and the cost of a single ER visit ($3,500+ average for a fall). The $19.99 one-time price is positioned as "less than one grab bar installation" and "peace of mind for the price of a pizza dinner." The monitoring subscription at $4.99/month is offered after the initial audit is complete: "Your parent's capabilities change over time. Get reassessment reminders, updated product recommendations, and capability tracking for $4.99/month." Product affiliate links (Amazon Associates, Home Depot affiliate program) generate secondary revenue estimated at $2-$5 per audit from product purchases. Contractor referral fees (per lead or per completed job) provide a third revenue stream that scales with the user base.

## 9. Analytics & KPIs
| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| Free audits started (bathroom only) | 150 | 1,000/month | 2,500/month |
| Free audit completion rate | 60% | 70% | 75% |
| Free-to-paid conversion rate | 10% | 15% | 18% |
| Full audits completed (paid) | 15 | 150/month | 450/month |
| Monitoring subscription sign-ups | 5 | 50/month | 120/month |
| Family report shares per audit | 0.3 | 0.5 | 0.6 |
| Product affiliate click-through rate | 5% | 8% | 10% |
| Contractor finder usage rate | 8% | 15% | 18% |
| Monthly revenue | $500 | $5,000 | $12,000 |
| App Store rating | 4.2 | 4.5 | 4.7 |

## 10. 12-Week Launch Plan
| Week | Milestone |
|------|-----------|
| 1 | Finalize wireframes, data model, and checklist content; research CDC and OT fall-prevention guidelines to build checklist items; set up React Native (Expo) project, Node.js/Lambda backend, PostgreSQL on RDS |
| 2 | Source and curate reference photos (hazard vs. safe) for all checklist items across 7 rooms; build database schema and seed checklist items table |
| 3 | Build home setup flow (resident profile, capability questionnaire); build room selection screen; implement user authentication |
| 4 | Build the room assessment checklist UI with photo references, response buttons (Safe/Hazard/N/A), camera integration, and real-time risk score calculation |
| 5 | Build the room results and recommendations engine: scoring algorithm, prioritization logic, product link database, and DIY/professional tagging |
| 6 | Build the full audit summary screen; implement PDF report generation for sharing; build the shareable web view with unique tokens |
| 7 | Build contractor finder with Google Places API integration; build product recommendations shopping-list view with affiliate links; implement before/after photo capture and comparison |
| 8 | Implement Stripe payment for one-time purchase and monitoring subscription; build freemium gating (bathroom free, other rooms paid); build progress tracker screen |
| 9 | Internal QA; recruit 15 beta users from r/AgingParents and r/CaregiverSupport; conduct 3 in-home audit walkthroughs with beta users to validate checklist accuracy and UX |
| 10 | Iterate on beta feedback; refine checklist items and risk scoring based on real-world testing; submit to App Store and Google Play; prepare ASO assets |
| 11 | Public launch; begin Reddit GTM in r/AgingParents, r/CaregiverSupport, r/eldercare, r/occupationaltherapy; post room-specific safety checklists as value content; begin SEO content publishing ("home safety checklist for elderly," "how to prevent falls for seniors") |
| 12 | Contact 25 local senior centers and Area Agencies on Aging for co-branding partnerships; begin home health agency referral outreach; analyze Month 1 metrics; publish first case study ("I audited my mom's bathroom and fixed 7 hazards for under $100"); plan v2.0 reassessment and OT consultation features |

## 11. Growth Loops

**Caregiver Share Loop**: Every completed audit generates a shareable family report. The average user shares with 2-3 family members, each of whom has their own aging parents. The report includes app branding and a "Audit your parent's home too" CTA. This creates organic peer-to-peer spread among the sandwich generation.

**Before/After Social Proof Loop**: Before and after photos of home modifications (especially dramatic ones like walk-in shower conversions or grab bar installations) are compelling visual content. Users share these in caregiver support groups and on social media, creating organic discovery. The app prompts users to share after completing modifications.

**Senior Center Partnership Loop**: Senior centers and Area Agencies on Aging have 3-6 month waitlists for professional assessments. By co-branding the free bathroom audit as a community resource, these organizations funnel their waitlisted families to the app. Families get immediate value, and the organizations reduce their backlog, creating a win-win that encourages ongoing partnership.

**Reassessment Retention Loop**: The 6-month reassessment cycle keeps users returning and creates an ongoing relationship. Each reassessment may reveal new risks as the parent's capabilities change, driving additional product purchases and contractor referrals.

**OT Referral Loop**: Occupational therapists recommend the app to families on their waitlist. When those families complete the self-assessment, some opt for the OT virtual consultation upsell ($50), creating revenue for the OT and the platform. Satisfied OTs recommend the app to more families, compounding the referral source.

## 12. Regulatory & Compliance

- **Not Medical Advice**: The app must include prominent disclaimers that it supplements but does not replace a professional occupational therapy assessment. Language must avoid "diagnosis" or "clinical assessment." Use: "This is a self-guided safety checklist, not a substitute for a professional evaluation."
- **Product Safety Liability**: Recommendations for DIY modifications (e.g., grab bar installation) could lead to improper installation and injury. Include installation guides with video links; flag "professional installation recommended" for complex items (stairlifts, walk-in tubs, ramps); include a disclaimer that the app is not responsible for improper installation.
- **Data Privacy (CCPA / GDPR / HIPAA Considerations)**: While the app is not a healthcare tool and not subject to HIPAA, it collects health-related information (mobility status, vision, cognitive condition). Handle this data with healthcare-grade security practices. Encrypt at rest and in transit. Allow data deletion on request. Clear privacy policy explaining what data is collected and that it's never shared with third parties without consent.
- **Affiliate Disclosure (FTC)**: Product recommendation links with affiliate commissions must be clearly disclosed per FTC guidelines. Include: "We may earn a small commission if you purchase through these links, at no additional cost to you."
- **Contractor Referral Liability**: The app connects users with contractors but does not vet, license, or guarantee their work. Include disclaimers: "We recommend verifying the contractor's license, insurance, and references before hiring." Consider requiring contractors to be listed with verified licensing.
- **App Store Compliance**: Subscription pricing and auto-renewal terms must be clearly disclosed per Apple and Google guidelines.
- **Elder Abuse Sensitivity**: The app should be designed to empower, not to be used as a tool for pressuring or controlling an elderly person. Include guidance on collaborative use and respect for the senior's autonomy.

## 13. Risk Register
| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| User acts on recommendations without professional validation, creating a false sense of security (e.g., incorrectly installed grab bar fails during a fall) | Medium | Critical | Prominent disclaimers on every recommendation; installation guides with video; "professional installation recommended" flag for complex items; OT virtual consultation upsell for professional review |
| One-time purchase model limits revenue growth and LTV | High | Medium | Push monitoring subscription ($4.99/mo) after audit completion; expand into adjacent products (medication management, emergency contacts, caregiver coordination); build contractor marketplace with per-referral revenue; product affiliate commissions provide recurring passive income |
| Sensitive family dynamics — adult children's suggestions perceived as patronizing by parents, causing family conflict and negative app associations | Medium | Medium | Frame app as collaborative ("Do this together with Mom"); include conversation scripts; offer "self-assessment" mode for seniors; emphasize independence preservation language throughout; avoid clinical or institutional tone |
| Low audit completion rate — users start but don't finish all 7 rooms due to time or overwhelm | Medium | Medium | Allow saving progress and resuming later; show completion percentage and encouragement; highlight "quick wins" early; allow room-by-room completion over multiple visits; estimate time per room (5-8 minutes each) |
| Checklist items become outdated as safety standards and product recommendations evolve | Low | Medium | Review and update checklist items quarterly; partner with an OT advisory board; monitor CDC and AARP guidelines for changes; build admin interface for content updates without app releases |
| Contractor finder returns poor-quality results or contractors who are not aging-in-place specialists | Medium | Medium | Curate a verified contractor directory in initial markets; require contractors to confirm specialization; allow user reviews and ratings of contractors; flag "verified aging-in-place specialist" for certified contractors (CAPS certified) |
| Competition from AARP or CDC releasing a free interactive assessment tool | Low | High | Differentiate on personalization (capability-adjusted recommendations), photo documentation, contractor marketplace, and family sharing features; build community and brand loyalty before large organizations move into the space |

## 14. Success Criteria
- **6-month go/no-go**: 1,000 free bathroom audits started per month with 70% completion rate; 15% free-to-paid conversion (150 paid audits/month); 50 monitoring subscribers generating $250/month in subscription MRR; family report shared in 50%+ of completed audits (indicating the viral loop is working); 3 senior center or AAA partnerships active; App Store rating of 4.5+
- **12-month milestone**: 2,500 free audits and 450 paid audits per month; $12,000 monthly revenue (audits + subscriptions + affiliate + contractor referrals); 120 monitoring subscribers; at least 10 senior center/AAA partnerships across 3 states; OT virtual consultation feature launched; product affiliate revenue contributing $500+/month; v2.0 features (reassessment reminders, capability tracking) live and driving monitoring subscription growth
