# Product Requirements Document: Subscription Autopsy

## 1. Executive Summary
The average American household wastes approximately $1,600 per year on forgotten or unwanted subscriptions, with 42% of consumers unaware of at least one active recurring charge. Subscription Autopsy solves this by automatically scanning bank transactions and email receipts to detect, categorize, and cancel unwanted subscriptions -- then continuously monitoring for "zombie charges" that persist after cancellation. The target user is any digitally active US adult aged 25-45 with multiple subscriptions who values convenience and wants immediate savings without manual effort. At a $4.99/month flat fee (dramatically cheaper than Rocket Money's percentage-of-savings model), the product addresses a $2.1B market with a clear viral mechanic: users share their savings reports on social media, driving organic acquisition. The business targets $180K in Year 1 revenue from 3,000 paid users, scaling to $1.8M by Year 3 through a content-driven growth flywheel on Reddit and TikTok.

## 2. User Personas

### Persona 1: Maya Chen
- **Age**: 28
- **Job**: UX Designer at a mid-size tech company
- **Income**: $85,000/year
- **Pain Points**: Has signed up for dozens of free trials over the years (design tools, streaming services, fitness apps) and routinely forgets to cancel. Gets frustrated by dark-pattern cancellation flows that require calling a phone number. Noticed a $14.99/month charge she cannot identify on her bank statement.
- **Goals**: Wants a one-time "audit" of all her subscriptions and an easy way to kill the ones she does not use. Would love to share savings with friends who are in the same boat.
- **Tech Comfort Level**: Very high -- uses Figma, Notion, and multiple SaaS tools daily. Comfortable connecting bank accounts via Plaid.

### Persona 2: David Thompson
- **Age**: 42
- **Job**: Operations Manager at a logistics company
- **Income**: $110,000/year
- **Pain Points**: Manages household subscriptions for a family of four. His kids (14 and 17) have signed up for gaming subscriptions, Patreon pledges, and Discord Nitro without his knowledge. He does not have time to manually audit bank statements. Dreads the process of canceling anything that requires a phone call.
- **Goals**: Wants a single dashboard showing everything the family is paying for, with the ability to cancel in one tap. Wants alerts when new subscriptions appear.
- **Tech Comfort Level**: Moderate -- uses standard apps and online banking, but would not describe himself as "techy." Needs a simple, clean interface with no jargon.

### Persona 3: Jasmine Rivera
- **Age**: 34
- **Job**: Freelance Graphic Designer
- **Income**: $52,000/year
- **Pain Points**: Income fluctuates month to month, making subscription costs feel more painful. Has experienced zombie charges twice -- canceling a gym membership and a meal kit service, only to see charges continue for 2-3 months. Filed disputes with her bank but the process was exhausting.
- **Goals**: Wants proactive monitoring that catches charges the moment they appear after she cancels something. Wants hard data on her total subscription spending to make informed decisions about what to keep.
- **Tech Comfort Level**: High -- manages her own invoicing and financial tools. Privacy-conscious and wants to understand how her data is used.

## 3. User Stories (20+)

1. As a new user, I want to connect my bank account securely via Plaid so that the app can automatically detect my recurring subscriptions.
2. As a new user, I want to forward my receipt emails so that the app catches subscriptions that do not appear in bank statements (PayPal, crypto, annual charges).
3. As a user, I want to see all my detected subscriptions in a single categorized list (entertainment, fitness, news, software, etc.) so that I can quickly understand where my money goes.
4. As a user, I want to see my total monthly and yearly subscription spend so that I understand the full financial impact.
5. As a user, I want to receive a "waste score" that tells me how much I am likely overspending so that I feel motivated to take action.
6. As a user, I want to cancel a subscription with one tap so that I do not have to navigate dark-pattern cancellation flows myself.
7. As a user, I want the app to handle cancellation via automated email, chat, or call bots on my behalf so that I save time on companies that make cancellation deliberately difficult.
8. As a user, I want to be notified when a zombie charge appears (a charge from a subscription I already cancelled) so that I can dispute it immediately.
9. As a user, I want to receive weekly spend alerts summarizing my subscription activity so that I stay on top of new charges.
10. As a user, I want to see the billing date, amount, and frequency for each subscription so that I can plan my budget.
11. As a user, I want to tag subscriptions as "keep," "review," or "cancel" so that I can triage my list before taking action.
12. As a user, I want to generate a shareable "Subscription Autopsy Report" card showing my total waste found so that I can share it on social media and help friends discover the app.
13. As a user, I want to invite family members to a shared dashboard so that I can see and manage household subscriptions together.
14. As a user, I want to see price increase alerts when a subscription raises its rate so that I can decide whether to keep or cancel.
15. As a user, I want to receive a notification before free trials expire so that I can cancel before being charged.
16. As a user, I want to see similar or cheaper alternatives to my current subscriptions so that I can save money without losing functionality.
17. As a user, I want to view my subscription spending trends over time (month-over-month chart) so that I can see if I am spending more or less.
18. As a user, I want to search and filter my subscriptions by category, price, or status so that I can quickly find what I am looking for.
19. As a user, I want to export my subscription data as CSV or PDF so that I can share it with a financial advisor or use it for budgeting.
20. As a user, I want to receive an annual savings report showing how much the app saved me so that I can justify the subscription cost.
21. As a user, I want to set a monthly subscription budget and be alerted when I approach or exceed it so that I stay within my financial goals.
22. As a user, I want to see which payment methods (credit cards, PayPal, etc.) are linked to which subscriptions so that I can update or cancel cards without losing services I want.
23. As a privacy-conscious user, I want to understand exactly what data is collected and have the ability to delete my data at any time so that I feel safe using the app.
24. As a returning user, I want to see what changed since my last visit (new charges detected, cancellations confirmed, zombie charges caught) so that I get immediate value on every login.

## 4. Feature Requirements

### MVP (v1.0) -- Must Have
- [ ] Plaid bank account integration for automatic recurring charge detection with support for major US banks (acceptance criteria: 95%+ connection success rate for top 50 banks)
- [ ] Email forwarding and parsing system to detect subscription receipts not visible in bank transactions (acceptance criteria: supports Gmail and Outlook forwarding, parses sender, amount, and date)
- [ ] Subscription dashboard displaying all detected subscriptions with name, category, amount, frequency, and next billing date (acceptance criteria: renders within 2 seconds, supports 100+ subscriptions per user)
- [ ] Automatic categorization of subscriptions into predefined categories (entertainment, fitness, news, software, food delivery, gaming, music, cloud storage, other) using OpenAI API (acceptance criteria: 90%+ categorization accuracy)
- [ ] Monthly and yearly total spend calculator with visual breakdown by category (acceptance criteria: pie chart and bar chart views, accurate to the cent)
- [ ] Waste score algorithm that identifies likely unused subscriptions based on usage signals and charge patterns (acceptance criteria: score displayed as 0-100 with explanation of contributing factors)
- [ ] One-tap cancellation request system that generates and sends cancellation emails/chats on the user's behalf (acceptance criteria: supports at least 50 of the most common subscription services at launch)
- [ ] Zombie charge monitoring that detects charges from previously cancelled subscriptions and sends push/email alerts within 24 hours (acceptance criteria: zero false negatives on charges from services marked as cancelled)
- [ ] Weekly subscription spend summary email with new charges, upcoming renewals, and total spend (acceptance criteria: delivered every Monday by 9 AM user's local time)
- [ ] User authentication with email/password and Google OAuth, including secure session management (acceptance criteria: SOC 2-aligned security practices, bcrypt password hashing, JWT tokens)
- [ ] Free trial expiration reminder system that alerts users 3 days and 1 day before any detected trial converts to a paid subscription (acceptance criteria: notification delivered via push and email)
- [ ] Basic subscription triage workflow allowing users to tag each subscription as "keep," "review," or "cancel" (acceptance criteria: tags persist across sessions, filterable by tag)

### v2.0 -- Should Have
- [ ] Family plan supporting up to 4 connected accounts on a shared dashboard with role-based permissions (owner vs. viewer)
- [ ] Price increase detection that alerts users when a subscription charge increases compared to the previous billing cycle
- [ ] Subscription alternatives engine that suggests cheaper or free alternatives to current subscriptions based on category
- [ ] Shareable "Subscription Autopsy Report" card optimized for Instagram Stories, Twitter, and TikTok with a referral link embedded
- [ ] Spending trend charts showing month-over-month and year-over-year subscription cost trajectory
- [ ] CSV and PDF export of subscription list and spending data for budgeting or financial advisor sharing
- [ ] Monthly subscription budget cap with alerts when spending approaches 80% and 100% of the set limit
- [ ] In-app dispute assistant that generates pre-written dispute letters for zombie charges to send to the bank or merchant

### v3.0 -- Nice to Have
- [ ] Payment method mapping showing which credit cards/PayPal accounts are linked to which subscriptions, with alerts when a card is about to expire
- [ ] Annual savings report with year-end summary of total savings achieved, cancellations completed, and zombie charges caught
- [ ] Browser extension that detects subscription sign-up pages and warns users ("You already have 3 streaming services -- are you sure?")
- [ ] Integration with budgeting apps (YNAB, Mint successor, Copilot) to sync subscription data
- [ ] Dark web monitoring for compromised payment methods used in subscriptions (partnership with identity protection service)

## 5. Technical Architecture
- **Frontend**: React with Next.js 14 (App Router) -- chosen for server-side rendering (improves SEO for the landing page and marketing content), fast initial load times, and a mature ecosystem of component libraries. Tailwind CSS for styling. React Query for server state management.
- **Backend**: Node.js with Express.js running on serverless functions (AWS Lambda or Vercel Edge Functions) -- chosen for rapid development speed, JavaScript ecosystem consistency with the frontend, and excellent Plaid SDK support. TypeScript throughout for type safety.
- **Database**: PostgreSQL on Supabase -- chosen for relational data integrity (users, subscriptions, transactions, cancellation statuses have complex relationships), strong support for time-series queries (spend trends), and Supabase's built-in auth and real-time subscription capabilities. Redis (Upstash) for caching Plaid token sessions and rate limiting.
- **Key APIs**:
  - Plaid API -- bank account connection and transaction retrieval for recurring charge detection
  - Nylas API -- email parsing for receipt/subscription detection from forwarded emails
  - OpenAI API (GPT-4o-mini) -- subscription categorization, waste score analysis, and cancellation email generation
  - Twilio SendGrid -- transactional emails (weekly summaries, alerts, cancellation confirmations)
  - Stripe -- payment processing for the $4.99/month and $9.99/month subscription tiers
  - Firebase Cloud Messaging / Apple Push Notification Service -- push notifications for zombie charge alerts and trial expiration reminders
- **Hosting**: Vercel for frontend and serverless API routes (~$20/month Pro plan), Supabase for database (~$25/month Pro plan), Upstash for Redis (~$10/month). Total infrastructure cost: ~$55-150/month at launch, scaling with usage. AWS Lambda overflow for heavy background jobs (Plaid syncs, email parsing) at ~$50-100/month.

## 6. Data Model

### Users
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| email | String | Unique, indexed |
| password_hash | String | bcrypt hashed |
| name | String | Display name |
| plan | Enum | free, paid, premium |
| stripe_customer_id | String | Nullable |
| created_at | Timestamp | |
| updated_at | Timestamp | |

### PlaidConnections
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| plaid_access_token | String | Encrypted at rest |
| institution_name | String | Bank name |
| status | Enum | active, disconnected, error |
| last_synced_at | Timestamp | |

### Subscriptions
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| name | String | Service name |
| category | Enum | entertainment, fitness, news, software, etc. |
| amount | Decimal | Charge amount |
| currency | String | Default USD |
| frequency | Enum | weekly, monthly, quarterly, annual |
| next_billing_date | Date | Predicted next charge |
| detection_source | Enum | plaid, email, manual |
| status | Enum | active, cancelled, zombie |
| user_tag | Enum | keep, review, cancel (nullable) |
| waste_score | Integer | 0-100 |
| created_at | Timestamp | |

### CancellationRequests
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| subscription_id | UUID | FK to Subscriptions |
| method | Enum | email, chat, call |
| status | Enum | pending, sent, confirmed, failed |
| cancelled_at | Timestamp | Nullable |
| zombie_watch_until | Date | Monitor for charges until this date |

### ZombieAlerts
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| subscription_id | UUID | FK to Subscriptions |
| transaction_amount | Decimal | Charge amount detected |
| transaction_date | Date | |
| alert_sent_at | Timestamp | |
| resolved | Boolean | Default false |

### Relationships
- A User has many PlaidConnections (one per bank account)
- A User has many Subscriptions
- A Subscription has zero or one CancellationRequest
- A Subscription has zero or many ZombieAlerts
- Family plans: a FamilyGroup table links multiple Users with an owner_id and member role

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Landing Page / Marketing
The user sees a bold headline: "Find and kill the subscriptions draining your bank account." Below it, a large CTA button: "Scan My Subscriptions Free." Below the fold: three-step process illustration (Connect > Discover > Cancel), social proof (total savings reported by users), and a pricing comparison table vs. Rocket Money. Footer includes privacy policy, terms, and security badges (Plaid, 256-bit encryption).

### Screen 2: Onboarding / Connection
After signup, the user sees two options side by side: "Connect Your Bank" (Plaid widget launches in a modal) and "Forward Your Emails" (instructions for setting up email forwarding with a unique address). A progress indicator shows Step 1 of 3. Below each option, a brief explainer about what data is accessed and how it is protected. A "Skip for now" link allows manual entry.

### Screen 3: Scanning / Loading
While data is being processed, the user sees an animated "autopsy" graphic -- a magnifying glass scanning through stylized subscription icons. A progress bar shows "Scanning 247 transactions..." with real-time counts: "Found 14 subscriptions so far." This screen is designed to build anticipation and takes 10-30 seconds.

### Screen 4: Subscription Dashboard (Main Screen)
The primary screen users see on every return visit. Top section: total monthly spend (large number), total yearly spend, and waste score (displayed as a circular gauge with color coding: green/yellow/red). Below: a scrollable list of all detected subscriptions, each showing the service logo, name, category tag, amount, frequency, and next billing date. Each item has a swipe-left action to "Cancel" and a tap to expand details. Filter tabs at the top: All, Keep, Review, Cancel, Zombie. A floating action button allows manual subscription entry.

### Screen 5: Subscription Detail
Tapping a subscription opens a detail view showing: full charge history (list of past transactions from Plaid), the detection source (bank/email/manual), category, billing frequency analysis, and the waste score explanation ("You haven't used this service's app in 45 days"). Action buttons: "Cancel This" (launches cancellation flow), "Mark as Keep," "Set Reminder." If the subscription is cancelled, a zombie monitoring badge shows: "Monitoring for zombie charges until [date]."

### Screen 6: Cancellation Flow
The user taps "Cancel This" and sees a confirmation screen: "We'll cancel [Service Name] for you." The app displays the cancellation method it will use (email bot, chat bot, or call bot) and an estimated timeline. The user taps "Confirm Cancellation." A status card appears: "Cancellation request sent -- we'll notify you when confirmed." If manual steps are required (e.g., the service requires the user to call), the app shows a step-by-step guide with the phone number, what to say, and a "Mark as Done" button.

### Screen 7: Zombie Charge Alert
When a zombie charge is detected, the user receives a push notification and sees an alert banner at the top of the dashboard. Tapping it opens a detail screen showing: the cancelled subscription name, the charge amount and date, and three action buttons: "Dispute with Bank" (generates a pre-written dispute letter), "Contact Merchant" (generates a refund request email), and "Dismiss" (marks as resolved). A timeline shows the cancellation date vs. the zombie charge date for evidence.

### Screen 8: Weekly Summary / Report
Accessible from the dashboard or delivered via email. Shows a week-in-review: new subscriptions detected, charges processed this week, upcoming renewals in the next 7 days, total spend this week vs. last week, and any zombie alerts. A "Share My Report" button generates the shareable Subscription Autopsy Report card with the user's total waste found and a referral link.

### Screen 9: Settings & Account
User profile (name, email, password change), connected accounts (Plaid connections with reconnect/disconnect options), notification preferences (push, email, SMS toggles for each alert type), subscription plan management (current plan, upgrade/downgrade, billing history), data privacy controls (download my data, delete my account), and a "Refer a Friend" section with a unique referral link and tracking of successful referrals.

### Screen 10: Paywall / Upgrade Screen
Triggered when free users attempt to cancel a subscription, enable zombie monitoring, or access weekly reports. Shows a comparison of Free vs. Paid ($4.99/mo) vs. Premium ($9.99/mo) features in a clean table format. Highlights the user's specific situation: "You have 3 subscriptions marked for cancellation worth $47/month -- upgrade to cancel them with one tap." A 7-day free trial CTA with fine print about auto-renewal. Testimonials from users showing savings amounts.

## 8. Monetization Implementation

### Paywall Placement
The free tier provides a one-time bank/email scan and a subscription list with total spend and waste score. This is the "aha moment" -- seeing how much you waste is emotionally powerful and free. The paywall activates when users try to take action: cancelling subscriptions, enabling zombie monitoring, receiving weekly alerts, or running recurring scans. This "show the problem for free, charge for the solution" model maximizes conversion because users are emotionally primed to pay after seeing their waste.

### Upgrade Triggers
- Tapping "Cancel" on any subscription (free users see: "Upgrade to cancel with one tap")
- Zombie charge detection (free users see: "Upgrade to monitor for zombie charges")
- After the initial scan, a prompt: "Your subscriptions will change. Upgrade to keep monitoring."
- Weekly email teaser: "We detected 2 new charges this week. Upgrade to see details."
- 30-day re-engagement email: "You've been charged $X since your last scan. Want to check?"

### Pricing Psychology
- $4.99/month is positioned as "less than the cost of one subscription you forgot about"
- The flat-fee model is explicitly contrasted with Rocket Money's percentage-of-savings model, which feels punitive ("Why should we take more money when you save more?")
- Annual plan at $39.99/year ($3.33/mo) offers a 33% discount to improve retention and LTV
- The Premium family plan at $9.99/month is positioned as "one price for the whole household" -- compelling for the David Thompson persona

## 9. Analytics & KPIs

| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| New free scans completed | 1,000 | 6,000/mo | 12,000/mo |
| Free-to-paid conversion rate | 5% | 8% | 10% |
| Paid subscribers (cumulative) | 50 | 800 | 3,000 |
| Monthly recurring revenue (MRR) | $250 | $4,000 | $15,000 |
| Zombie charges detected | 10 | 150/mo | 500/mo |
| Avg. savings per user | $45/mo | $75/mo | $90/mo |
| Total dollar savings delivered | $2,250 | $60,000/mo | $270,000/mo |
| 30-day paid user retention | 65% | 70% | 75% |
| Viral coefficient (shares/user) | 0.1 | 0.25 | 0.35 |
| Plaid connection success rate | 90% | 95% | 97% |
| Cancellation success rate | 60% | 75% | 85% |
| NPS score | 30 | 45 | 55 |

## 10. 12-Week Launch Plan

| Week | Milestone |
|------|-----------|
| Week 1 | Set up development environment: initialize Next.js project, configure Supabase database, set up Plaid developer sandbox account, establish CI/CD pipeline on Vercel. Design database schema and seed test data. |
| Week 2 | Build user authentication (email/password + Google OAuth), onboarding flow, and Plaid integration (bank connection modal, token exchange, initial transaction pull). |
| Week 3 | Build transaction analysis engine: recurring charge detection algorithm, subscription identification from transaction descriptions, and frequency/amount pattern recognition. |
| Week 4 | Build email forwarding and parsing system (Nylas integration): generate unique forwarding addresses, parse receipt emails for subscription data, merge with bank-detected subscriptions. |
| Week 5 | Build subscription dashboard UI: categorized list view, total spend calculator, waste score algorithm and display, and subscription detail screens. Integrate OpenAI for auto-categorization. |
| Week 6 | Build cancellation system: email bot for the top 50 services, cancellation request tracking, status updates, and manual cancellation guide fallback. Build zombie charge detection logic. |
| Week 7 | Build notification systems: weekly summary emails (SendGrid), push notifications for zombie alerts and trial expirations (FCM/APNs), and the shareable Autopsy Report card generator. |
| Week 8 | Build paywall and Stripe integration: free/paid/premium tier gating, subscription checkout flow, billing management, and upgrade prompts at key moments. |
| Week 9 | Internal QA and beta testing: recruit 20-30 beta users from r/personalfinance. Fix bugs, tune waste score algorithm, improve categorization accuracy, and stress-test Plaid connections across multiple banks. |
| Week 10 | Prepare launch assets: landing page copy and design, Product Hunt listing, Show HN post draft, TikTok/Reels content (3-5 "savings reveal" videos), Reddit posts for r/personalfinance and r/Frugal. |
| Week 11 | Soft launch: publish to Product Hunt (target Tuesday launch), post Show HN, begin Reddit engagement in personal finance subreddits. Monitor real-time analytics, fix critical issues, and respond to every piece of user feedback. |
| Week 12 | Post-launch iteration: analyze conversion funnel data, A/B test paywall copy, optimize waste score algorithm based on user feedback, publish first TikTok content, and begin weekly Reddit content cadence. Set Month 2 growth targets. |

## 11. Growth Loops

### Viral Savings Report
After every scan, users receive a beautifully designed "Subscription Autopsy Report" card showing total waste found, number of zombie charges caught, and total monthly savings. The card is sized for Instagram Stories and Twitter, with a built-in referral link. The psychological trigger is social proof and competitive comparison ("Can you beat my waste score?"). Each share exposes the app to the sharer's network, driving organic sign-ups.

### Tax Season and New Year Loop
January through April is peak "financial audit" season. The app sends re-engagement emails prompting users to re-scan after the holidays ("New year, new subscriptions -- time for an autopsy"). Content marketing around "subscription audit" keywords captures high-intent search traffic during this period, which converts to free scans and paid upgrades.

### Zombie Charge Word-of-Mouth
When the app catches a zombie charge, users experience a strong emotional reaction ("I would have lost $50!"). This creates a natural sharing moment -- users tell friends, post on Reddit, and share on social media. The more zombie charges caught, the more organic promotion the app receives.

### Referral Incentive
Paid users who refer friends receive one free month for each successful referral (friend must complete a scan). This directly reduces churn while growing the user base. The referral link is embedded in every shareable report and weekly summary email.

## 12. Regulatory & Compliance

### Financial Data Privacy
- **Plaid compliance**: Plaid is already SOC 2 Type II and ISO 27001 certified. The app accesses transaction data in read-only mode -- no ability to move money or initiate payments. Must comply with Plaid's data access policies and user consent requirements.
- **GLBA (Gramm-Leach-Bliley Act)**: As a service accessing financial data, the app must implement an information security program, provide privacy notices to users, and protect nonpublic personal information. Even though Plaid handles the bank connection, the app stores derived financial data (subscription amounts, spending patterns).
- **CCPA/CPRA (California)**: Must provide California residents the right to know, delete, and opt out of sale of personal information. Implement a "Do Not Sell My Information" link and data deletion workflow.
- **State money transmitter laws**: The app does NOT move money or process payments on behalf of users (Stripe handles subscription billing), so money transmitter licenses are not required. However, if future features involve refund processing, this must be re-evaluated.

### Cancellation Bots -- Legal Considerations
- **CAN-SPAM Act**: Cancellation emails sent on behalf of users must comply with CAN-SPAM (accurate headers, legitimate sender). The user must authorize each cancellation request.
- **CFPB "Click-to-Cancel" Rule (2024)**: The FTC's rule requiring companies to make cancellation as easy as sign-up works in Subscription Autopsy's favor -- it legitimizes automated cancellation tools. However, the app must not misrepresent itself as the user when interacting with merchants.
- **Terms of Service risks**: Some subscription services (e.g., Adobe, Planet Fitness) may have ToS provisions against automated cancellation. Risk is low (users authorize the action), but the app should clearly state it acts as the user's authorized agent.

### Data Security
- All financial data encrypted at rest (AES-256) and in transit (TLS 1.3)
- Plaid access tokens stored in encrypted database columns, never logged
- SOC 2 Type II compliance target within 18 months of launch
- Annual penetration testing after reaching 10,000 users
- GDPR compliance if expanding to EU markets (consent management, data portability, right to erasure)

## 13. Risk Register

| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| Plaid raises API pricing significantly, eroding gross margins | Medium | High | Build integrations with MX Financial and Finicity as backup bank connection providers. Optimize API calls by caching transaction data and reducing sync frequency for inactive users. Negotiate volume discounts with Plaid as user base grows. |
| Auto-cancel bots break when subscription services change their cancellation flows | High | Medium | Maintain a community-reported "flow changed" alert system. Build a modular cancellation bot architecture where each service's flow is a separate configurable script. Fall back to manual cancellation guides with step-by-step instructions when bots fail. Monitor success rates per service daily. |
| Rocket Money dominates paid acquisition channels with deep pockets (backed by Rocket Companies) | High | Medium | Do not compete on paid acquisition channels initially. Double down on organic/viral channels: Reddit, TikTok, Product Hunt, Show HN. Differentiate on flat-fee pricing and zombie charge monitoring -- features Rocket Money underemphasizes. Build brand loyalty in price-sensitive segments that find Rocket Money expensive. |
| Bank connection failures or Plaid outages prevent users from completing onboarding, killing activation | Medium | High | Provide email-scanning as a fully functional alternative path (no bank required). Display clear error messages with retry options. Implement a manual subscription entry fallback. Monitor Plaid status API and proactively notify users during outages. Target 95%+ connection success rate. |
| User data breach or security incident destroys trust and triggers regulatory action | Low | Critical | Encrypt all financial data at rest and in transit. Never store raw bank credentials (Plaid handles this). Conduct security audits quarterly. Implement rate limiting, input validation, and SQL injection prevention. Maintain an incident response plan. Carry cyber liability insurance. |
| Free-to-paid conversion rate significantly below 8% target, making unit economics unsustainable | Medium | High | A/B test paywall placement, copy, and timing. Test different price points ($3.99 vs. $4.99 vs. $5.99). Introduce a one-time purchase option ($19.99) for users who resist subscriptions. Improve the free-tier "aha moment" by making the waste score more emotionally impactful. Survey churned free users to understand objections. |

## 14. Success Criteria

- **6-month go/no-go**: 800 paid subscribers generating $4,000 MRR, with a free-to-paid conversion rate of 7%+, 30-day paid retention of 68%+, and total dollar savings delivered exceeding $50,000 per month. If these targets are not met, evaluate whether the issue is top-of-funnel (not enough free scans), conversion (paywall is not compelling), or retention (users cancel after one month) and pivot accordingly.
- **12-month milestone**: 3,000 paid subscribers generating $15,000 MRR, with a viral coefficient of 0.3+ (each user drives 0.3 new users through sharing), LTV:CAC ratio of 4:1+, and at least one viral content moment (Reddit post or TikTok video exceeding 100K views). Family plan adoption at 10%+ of paid users. Product featured in at least two personal finance publications or podcasts.
