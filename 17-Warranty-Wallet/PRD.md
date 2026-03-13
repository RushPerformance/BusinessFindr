# Product Requirements Document: Warranty Wallet

## 1. Executive Summary
The average US household owns $15,000-$20,000 in warrantied products, yet only 20% of valid warranty claims are ever filed because people lose receipts, forget coverage periods, and find the claims process confusing. Warranty Wallet is a mobile and web application that stores all product warranties and receipts in one searchable vault, sends countdown alerts before coverage expires, and guides users through filing claims with pre-written letters and manufacturer contact information. The target user is a homeowner aged 30-55 who has experienced the frustration of a product breaking just outside (or unknowingly inside) the warranty window. With a freemium model ($3.99/mo for unlimited warranties, email auto-import, and guided claim filing), a projected LTV:CAC of 13.8:1, and a $2.8B serviceable market, the app can reach $1.0M ARR within three years plus affiliate revenue from an extended warranty marketplace.

## 2. User Personas

### Persona 1: Rachel, the Organized Homeowner
- **Age**: 38
- **Job**: Accountant
- **Income**: $92,000/year
- **Pain Points**: Bought a new house 3 years ago and has 15+ appliances under warranty; receipts are scattered across email, a kitchen drawer, and a filing cabinet; her dishwasher broke at month 10 of a 12-month warranty and she almost missed filing a claim because she couldn't find the receipt
- **Goals**: One place for every warranty; alerts well before expiration; clear instructions if something breaks
- **Tech Comfort**: High — manages personal finances digitally

### Persona 2: Tom, the Small Landlord
- **Age**: 47
- **Job**: Property manager (owns 4 rental units)
- **Income**: $130,000/year
- **Pain Points**: Manages appliance warranties across 4 properties; tenants report broken appliances but he can't quickly determine if something is still under warranty; has lost thousands replacing items that were still covered
- **Goals**: Multi-property warranty tracking; fast lookup when a tenant calls; organized records for tax deductions
- **Tech Comfort**: Moderate — uses property management software but not tech-savvy beyond that

### Persona 3: Devon, the Frugal Shopper
- **Age**: 29
- **Job**: Graphic designer (freelance)
- **Income**: $55,000/year
- **Pain Points**: Buys quality electronics and appliances but is meticulous about getting value; has tried storing receipts in Evernote but it's disorganized and doesn't remind him of expirations; wants to know when to consider extended warranties
- **Goals**: Never miss a valid warranty claim; compare extended warranty prices; know the exact dollar value of products he's protecting
- **Tech Comfort**: Very high — early adopter

## 3. User Stories (20+)
1. As a homeowner, I want to scan a paper receipt with my phone camera so that the app auto-detects the product, purchase date, and warranty period.
2. As a homeowner, I want to connect my Gmail account so that the app auto-imports purchase receipts and warranty confirmations from my email.
3. As a user, I want to see a list of all my warranties sorted by expiration date so that I know which coverages are ending soonest.
4. As a user, I want to receive push notifications 90, 60, and 30 days before a warranty expires so that I can inspect the product and file a claim if needed.
5. As a user, I want guided claim-filing instructions for my specific product manufacturer so that I know exactly what steps to take.
6. As a user, I want pre-written claim letter templates that auto-fill with my product and purchase details so that I can submit a claim in minutes.
7. As a user, I want manufacturer contact information and direct links to their claim portals so that I don't have to search for how to reach them.
8. As a user, I want to store warranty documents (PDFs, photos) attached to each product so that everything is in one place.
9. As a user, I want to search my warranties by product name, brand, or category so that I can quickly find any item.
10. As a user, I want to see the total dollar value of products currently under warranty so that I understand the value the app is protecting.
11. As a landlord, I want to organize warranties by property so that I can quickly check coverage when a tenant reports an issue.
12. As a user, I want to compare extended warranty plans from third-party providers so that I can decide if additional coverage is worth the cost.
13. As a user, I want to export my warranty inventory as a home inventory report for insurance purposes so that I have documentation if there is a theft or disaster.
14. As a user, I want to manually add a warranty by entering product name, brand, purchase date, and warranty length so that I can track items even without a receipt.
15. As a user, I want to mark a warranty claim as filed and track its status so that I can follow up if needed.
16. As a user, I want to receive product recall alerts for items I have registered so that I'm aware of safety issues.
17. As a user, I want a monthly "warranty health" email summarizing upcoming expirations and total protected value so that I stay engaged even when I'm not using the app daily.
18. As a user, I want to categorize warranties by type (electronics, appliances, vehicles, furniture) so that I can browse by category.
19. As a user, I want to share a warranty record with my spouse or co-owner so that they can also file a claim if needed.
20. As a user, I want to see a dashboard showing claims filed, money saved, and warranties expiring soon so that I feel the app is delivering value.
21. As a user, I want to forward a receipt email to a dedicated app email address so that it's automatically added without granting full inbox access.
22. As a user, I want to add notes to a warranty (e.g., "slight scratch on delivery, documented with photos") so that I have supporting evidence for future claims.

## 4. Feature Requirements

### MVP (v1.0) — Must Have
- [ ] Receipt scanning via phone camera with OCR to extract product name, brand, purchase date, price, and retailer (acceptance: correctly parses 80%+ of standard retail receipts; user can manually correct extracted fields)
- [ ] Manual warranty entry form with product name, brand, category, purchase date, warranty duration, price, and notes (acceptance: all fields validate and persist; warranty end date auto-calculates from purchase date + duration)
- [ ] Warranty dashboard showing all products sorted by expiration date with status badges (active/expiring soon/expired) (acceptance: color-coded badges; pull-to-refresh; search bar filters results in real time)
- [ ] Expiration countdown alerts via push notification at 90, 60, and 30 days before warranty end (acceptance: notifications fire on schedule; user can customize intervals; deep link opens the specific warranty)
- [ ] Guided claim filing: step-by-step instructions specific to the product's manufacturer (acceptance: covers top 50 manufacturers at launch; includes required documents checklist, contact info, and claim portal link)
- [ ] Pre-written claim letter templates auto-filled with product and purchase details (acceptance: user can edit before sending; export as PDF or copy to clipboard)
- [ ] Document and photo attachment per warranty (acceptance: supports JPEG, PNG, PDF; stored in cloud; viewable from the warranty detail screen)
- [ ] Product search and filter by name, brand, category, or status (acceptance: results update as user types; zero-state shows helpful prompts)
- [ ] Warranty value summary showing total dollar amount of products under active warranty (acceptance: updates in real time as warranties are added or expire)
- [ ] User authentication with email and social login (acceptance: supports email, Google, Apple sign-in; password reset; session persistence)
- [ ] Free tier with 10-warranty cap; paywall when adding the 11th warranty (acceptance: upgrade prompt shows pricing and feature comparison; smooth in-app purchase flow)

### v2.0 — Should Have
- [ ] Gmail and Outlook OAuth integration to auto-import purchase receipts and detect warranty information
- [ ] Dedicated forwarding email address (e.g., receipts@warrantywalletapp.com) for adding warranties via email
- [ ] Manufacturer contact directory with phone, email, chat links, hours, and claim portal URLs for top 200 brands
- [ ] Multi-property/multi-location organization for landlords
- [ ] Shared warranty records with household members (invite by email)
- [ ] Monthly "warranty health" email report with upcoming expirations, protected value, and claim reminders
- [ ] Product recall alert integration using CPSC recall database
- [ ] Claim status tracking (filed, in progress, approved, denied, resolved) with outcome notes

### v3.0 — Nice to Have
- [ ] Extended warranty price comparison marketplace with affiliate links to providers like Asurion, SquareTrade, and Allstate Protection Plans
- [ ] Automatic warranty detection from email scanning (proactive alerts for warranties the user didn't manually add)
- [ ] B2B API for retailers to auto-register warranties at point of sale
- [ ] Home inventory insurance export with photos, values, and serial numbers formatted for major insurance carriers
- [ ] AI-powered "claim probability" score estimating likelihood of needing a claim based on product reliability data

## 5. Technical Architecture
- **Frontend**: React Native (Expo) for iOS and Android mobile apps; Next.js for optional web dashboard — React Native enables cross-platform development with a single codebase, while Next.js provides SSR for SEO on the warranty guide content pages
- **Backend**: Node.js with Express, deployed on AWS Lambda — serverless keeps infrastructure costs proportional to usage; ideal for a bootstrapped product with variable traffic patterns
- **Database**: PostgreSQL on AWS RDS — relational model fits the structured warranty data (products, warranties, claims, users); JSONB columns handle flexible manufacturer-specific claim requirements
- **Key APIs**:
  - Google Cloud Vision API — OCR for receipt scanning and text extraction
  - Gmail API / Microsoft Graph API — email receipt auto-import (v2.0)
  - CPSC Recalls API — product recall alerts (v2.0)
  - Stripe — subscription billing and payment processing
  - Firebase Cloud Messaging / APNs — push notifications for expiration alerts
  - SendGrid — transactional and monthly report emails
  - Amazon Product Advertising API — product identification and extended warranty affiliate links (v3.0)
- **Hosting**: AWS (Lambda + RDS + S3 for document/photo storage + CloudFront CDN) — estimated $70/month at MVP scale; S3 for receipt images and warranty documents

## 6. Data Model

### Users
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| email | String | Unique, required |
| password_hash | String | Bcrypt |
| name | String | |
| subscription_tier | Enum | free, paid, premium |
| created_at | Timestamp | |

### Products
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| name | String | Required |
| brand | String | |
| category | Enum | electronics, appliances, furniture, vehicle, other |
| purchase_date | Date | Required |
| purchase_price | Decimal | |
| retailer | String | |
| serial_number | String | Nullable |
| notes | Text | |
| property_id | UUID | FK to Properties (nullable, v2.0) |

### Warranties
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| product_id | UUID | FK to Products |
| warranty_type | Enum | manufacturer, extended, retailer |
| duration_months | Integer | |
| start_date | Date | Defaults to purchase_date |
| end_date | Date | Auto-calculated |
| status | Enum | active, expiring_soon, expired |
| document_urls | JSON | Array of S3 paths |

### Claims
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| warranty_id | UUID | FK to Warranties |
| filed_date | Date | |
| status | Enum | draft, filed, in_progress, approved, denied |
| description | Text | |
| outcome_notes | Text | |
| resolved_date | Date | Nullable |

### Manufacturers
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| name | String | Unique |
| claim_portal_url | String | |
| phone | String | |
| email | String | |
| claim_instructions | Text | Step-by-step |
| required_documents | JSON | List of items needed |

### Receipts
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| product_id | UUID | FK to Products |
| image_url | String | S3 path |
| ocr_raw_text | Text | Raw OCR output |
| source | Enum | camera_scan, email_import, manual_upload |
| created_at | Timestamp | |

**Relationships**: A User has many Products. A Product has one or more Warranties and one or more Receipts. A Warranty has zero or more Claims. Manufacturers are a reference table linked to Products by brand name.

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Onboarding
Three-slide carousel: (1) "Never lose a warranty again" with receipt scanning illustration, (2) "Get alerted before coverage expires" with notification mockup, (3) "File claims in minutes, not hours" with claim letter preview. "Get Started" button leads to sign-up. After registration, prompt to scan first receipt or add warranty manually.

### Screen 2: Warranty Dashboard (Home)
Top section shows a summary card: "You're protecting $14,280 in products" with a count of active warranties and upcoming expirations. Below is a scrollable list of warranties sorted by expiration date. Each card shows product name, brand icon, days remaining (color-coded green/amber/red), and purchase price. A search bar at the top filters the list. Floating "+" button opens add-warranty options (scan receipt or manual entry). Bottom nav: Home, Add, Claims, Settings.

### Screen 3: Scan Receipt
Camera view with a guide overlay for receipt alignment. User takes a photo; loading spinner shows OCR processing. Results screen shows extracted fields (product name, brand, date, price, retailer) with editable text fields. User confirms or corrects, then taps "Save Warranty." Warranty duration is either auto-detected from receipt text or entered manually.

### Screen 4: Warranty Detail
Header with product name, brand, and photo. Key info: purchase date, warranty end date, days remaining (large countdown), purchase price. Tabbed sections: Documents (attached receipts and warranty papers), Claim History (list of claims filed), and Manufacturer Info (contact details and claim portal link). Action buttons: "Start a Claim" and "Edit Warranty."

### Screen 5: Guided Claim Filing
Step-by-step wizard specific to the manufacturer. Step 1: Confirm product and purchase details. Step 2: Describe the issue (text field + option to attach photos of the defect). Step 3: Review required documents checklist (receipt, warranty card, photos). Step 4: Choose action — generate a pre-written claim letter (auto-filled), call the manufacturer (tap to call), or visit their claim portal (deep link). Step 5: Mark claim as filed and set a follow-up reminder.

### Screen 6: Claim Letter Generator
A preview of the pre-written claim letter with the user's name, product details, purchase date, issue description, and requested resolution auto-filled. The user can edit any section. Buttons to "Copy to Clipboard," "Export as PDF," or "Send via Email." A disclaimer notes this is a template and not legal advice.

### Screen 7: Expiration Alerts Feed
A timeline view of upcoming warranty expirations ordered chronologically. Each entry shows product name, expiration date, and a quick-action button: "Inspect Product" (reminder to check for issues before coverage ends) or "Start Claim." Past expirations show in gray with a "This warranty has expired" label.

### Screen 8: Home Inventory Summary
A categorized view of all products (electronics, appliances, furniture, etc.) with total value per category and photos. An "Export for Insurance" button generates a PDF report with product names, photos, purchase dates, prices, and serial numbers. This screen doubles as proof of ownership for insurance claims.

### Screen 9: Extended Warranty Marketplace (v3.0 preview / placeholder)
For warranties nearing expiration, a prompt appears: "Your Samsung TV warranty expires in 30 days. Compare extended warranty plans." Lists 3 provider options with price, coverage duration, and rating. Tapping a plan opens the provider's purchase page (affiliate link). "No thanks" dismisses the prompt.

### Screen 10: Settings & Subscription
Account settings, notification preferences (alert timing: 90/60/30 days, toggle email reports), and subscription management. Free-tier users see a comparison table: free (10 warranties, manual entry) vs. paid (unlimited, email import, guided claims, alerts). Upgrade button leads to in-app purchase. Premium tier upsell shows extended warranty marketplace and multi-property features.

## 8. Monetization Implementation
The primary paywall trigger is the 10-warranty cap on the free tier. Most homeowners have 15-25 warrantied products, so the cap is generous enough to demonstrate value but low enough to convert engaged users. When the user tries to add warranty #11, a full-screen upgrade prompt appears showing: "You're protecting $X,XXX in products. Unlock unlimited warranties for $3.99/mo." Secondary paywalls gate email auto-import (highest convenience feature), guided claim filing with pre-written letters, and expiration countdown alerts. Pricing: $3.99/month or $34.99/year (27% savings). The annual plan is presented as the recommended option. A 7-day free trial of the paid tier is offered after the user adds their 5th warranty (enough engagement to see value). The premium tier at $7.99/month adds the extended warranty marketplace and multi-property support, targeting landlords and power users. Affiliate commissions from the extended warranty marketplace (estimated 8-15% per sale) provide a secondary revenue stream that scales independently of subscription count.

## 9. Analytics & KPIs
| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| Warranties added per week | 100 | 500 | 1,200 |
| Monthly Active Users (MAU) | 200 | 2,500 | 7,000 |
| Free-to-paid conversion rate | 5% | 8% | 10% |
| Monthly churn rate (paid) | 5% | 3.5% | 3% |
| Receipt scan success rate (OCR accuracy) | 75% | 82% | 88% |
| Warranty claims initiated via app | 5 | 20/week | 40/week |
| Expiration alert open rate | 40% | 50% | 55% |
| Average warranties per paid user | 12 | 18 | 22 |
| Home inventory export downloads | 5 | 30/month | 80/month |
| MRR | $300 | $4,200 | $8,400 |

## 10. 12-Week Launch Plan
| Week | Milestone |
|------|-----------|
| 1 | Finalize data model and wireframes; set up React Native (Expo) project, Node.js/Lambda backend, PostgreSQL on RDS, and S3 bucket; configure CI/CD |
| 2 | Build user authentication (email + Google + Apple); implement manual warranty entry form with all fields; build product and warranty database schema |
| 3 | Integrate Google Cloud Vision API for receipt OCR scanning; build the scan-receipt flow with extracted field confirmation and manual correction |
| 4 | Build warranty dashboard with sorted list, search/filter, status badges, and protected-value summary card |
| 5 | Implement push notification expiration alerts (90/60/30 day countdowns); build the expiration alerts feed screen |
| 6 | Build guided claim filing wizard with step-by-step instructions for top 50 manufacturers; implement claim letter template generator with auto-fill |
| 7 | Build document/photo attachment system on S3; implement home inventory summary with PDF export; set up Stripe subscription billing and freemium paywall |
| 8 | Internal QA and bug fixes; recruit 25 beta testers from r/Frugal and r/homeowners; collect feedback on receipt scanning accuracy and claim filing flow |
| 9 | Iterate on beta feedback; polish UI and fix OCR edge cases; submit to App Store and Google Play; prepare ASO (screenshots, keywords, description) |
| 10 | Public launch; begin Reddit GTM in r/Frugal, r/BuyItForLife, r/homeowners, r/personalfinance; post warranty claim success stories with app mention |
| 11 | Publish first 5 SEO articles: "How to file a warranty claim with Samsung/LG/Whirlpool/Apple/Dyson"; begin outreach to real estate agents for new homeowner partnerships |
| 12 | Analyze Month 1 metrics; run first monthly "warranty health" email; begin planning Gmail/Outlook integration for v2.0; approach Home Depot and Best Buy affiliate programs |

## 11. Growth Loops

**Receipt Scanning Habit Loop**: Every new purchase becomes an occasion to open the app and scan the receipt. This regular micro-engagement keeps the app top-of-mind and increases switching costs as the warranty vault grows.

**Expiration Alert Action Loop**: When a user receives a "warranty expiring in 30 days" alert, they inspect the product, and many discover issues they hadn't noticed. Filing a successful claim creates a "the app paid for itself" moment that drives word-of-mouth and positive reviews.

**New Homeowner Surge**: New homeowners have 10-20 new warranties at once. Partnerships with real estate agents and home warranty companies place the app at the exact moment of peak need, and these users arrive with enough warranties to immediately see value.

**Household Sharing Loop**: When one partner adds a warranty, the other partner needs access too. Sharing invitations bring in new users who then add their own warranties (personal electronics, etc.).

**Warranty Claim Story Loop**: Successfully filing a warranty claim and saving hundreds of dollars is a story people tell friends. The app can prompt users to share their savings: "You saved $347 on your Whirlpool dishwasher repair. Share your win!" These stories are naturally compelling in frugality communities.

**SEO Content Loop**: Each "How to file a warranty claim with [Brand]" article ranks for high-intent searches, driving organic traffic. These visitors discover the app through genuinely helpful content and convert at high rates because they have an immediate need.

## 12. Regulatory & Compliance

- **Data Privacy (CCPA / GDPR)**: User data includes personal information, purchase history, and financial details (product prices). Must implement right to deletion, data export, and clear privacy policy. Receipt images may contain sensitive information (payment method last 4 digits) and must be stored securely.
- **Email Access Permissions (OAuth)**: Gmail and Outlook integration requires careful OAuth scope management. Use the most restrictive read-only scopes; clearly explain to users what data is accessed; never store full email content — only extract purchase-related data.
- **PCI-DSS**: Stripe handles payment processing; no credit card data stored on our servers. Receipt images containing partial card numbers should not be used for any purpose beyond OCR text extraction.
- **FTC Affiliate Disclosure**: Extended warranty marketplace must clearly label affiliate links with appropriate disclosure per FTC guidelines (e.g., "We may earn a commission if you purchase through this link").
- **Consumer Protection Laws**: Claim letter templates must not constitute legal advice. Include disclaimers: "This template is for informational purposes. Consult a legal professional for specific advice." Do not guarantee claim outcomes.
- **App Store Compliance**: Subscription pricing, auto-renewal terms, and trial details must be clearly disclosed per Apple and Google guidelines.

## 13. Risk Register
| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| OCR receipt scanning accuracy is too low, causing user frustration and manual re-entry | High | High | Use Google Cloud Vision (industry-leading OCR); allow manual correction of all extracted fields; train a custom model on common receipt formats over time; always offer manual entry as a fallback |
| Email integration privacy concerns deter users from connecting Gmail/Outlook | Medium | High | Make email import optional (not required for core value); offer the dedicated forwarding email address as an alternative; use read-only, receipt-specific OAuth scopes; publish a transparency page explaining exactly what data is accessed |
| Low perceived value between warranty events (months pass without needing to file a claim) | Medium | High | Send monthly "warranty health" reports with total protected value; add product recall alerts; show a running "money saved" counter; emphasize insurance framing ($4/mo protects $15K+ in products) |
| Manufacturer resistance to streamlined claims (intentionally difficult claims processes) | Low | Medium | Focus on consumer-side claim preparation (letters, documentation) rather than direct manufacturer API integration; publish "claim difficulty ratings" as PR pressure; position as consumer empowerment |
| Competitor entry from receipt scanning apps (Fetch, Amazon) adding warranty tracking | Medium | Medium | Build deep warranty-specific features (claim filing, manufacturer directory, expiration alerts) that horizontal apps won't prioritize; accumulate a proprietary manufacturer claim instructions database |
| App Store rejection due to subscription policy violations | Low | High | Follow Apple and Google subscription guidelines precisely; test in-app purchase flow during beta; use RevenueCat or similar for cross-platform subscription management |

## 14. Success Criteria
- **6-month go/no-go**: 2,500 MAU with 8% free-to-paid conversion rate; at least 20 warranty claims initiated through the app per week; receipt OCR accuracy above 82%; monthly churn below 4%; MRR of $4,200
- **12-month milestone**: 7,000 MAU with 2,100+ paid subscribers generating $8,400 MRR ($100K+ ARR); at least 5 published SEO articles ranking on page 1 for "[brand] warranty claim" queries; Gmail/Outlook integration live with 30% adoption among paid users; extended warranty marketplace in development with 2+ affiliate partnerships signed
