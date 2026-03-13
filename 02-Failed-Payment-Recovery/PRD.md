# Product Requirements Document: DunningGuard (Failed Payment Recovery)

## 1. Executive Summary
Failed payments (involuntary churn) silently drain 9% of annual MRR from the average SaaS company, with Stripe's built-in retry logic recovering only 15-25% of failed charges. DunningGuard is a B2B SaaS platform that plugs into Stripe, Paddle, and Braintree to automatically recover failed subscription payments through smart retry logic optimized by time-of-day and card type, pre-dunning emails before cards expire, SMS/email recovery campaigns with one-click payment update links, and Account Updater API integration to refresh expired card details. The target customer is SaaS founders and heads of growth at companies with $50K-$500K MRR who lack the engineering bandwidth to build sophisticated dunning flows. With a hybrid pricing model ($49-199/month platform fee plus 3-5% of recovered revenue), the product aligns incentives directly with customer outcomes. The $1.5B SMB dunning/payment recovery market has a clear competitive gap following the shutdown of Baremetrics Recover and the restriction of ProfitWell Retain to Paddle-only customers. Year 1 target is $240K revenue from 80 customers, scaling to $2.4M by Year 3.

## 2. User Personas

### Persona 1: Sarah Kim
- **Age**: 33
- **Job**: Co-founder and CEO of a project management SaaS (12 employees, $180K MRR)
- **Income**: $120,000/year salary + equity
- **Pain Points**: Loses approximately $16,000/year to failed payments. Her engineering team is focused on product features, not billing infrastructure. She set up basic Stripe retry and a single dunning email a year ago but has not optimized it since. Does not know what recovery rate is "good" and has no visibility into how much revenue is slipping through the cracks.
- **Goals**: Wants a plug-and-play solution that recovers failed payments without requiring any engineering work. Needs a clear dashboard showing dollars recovered and ROI. Wants to stop worrying about involuntary churn so she can focus on product and sales.
- **Tech Comfort Level**: High -- uses Stripe dashboard daily, comfortable with API integrations, reads SaaS metrics religiously.

### Persona 2: Marcus Johnson
- **Age**: 41
- **Job**: Head of Growth at an online education platform (subscription model, $320K MRR, 8,500 subscribers)
- **Income**: $145,000/year
- **Pain Points**: Their payment failure rate spikes at the end of each month (card limits) and in January (expired cards). He has built a custom dunning email sequence but it recovers only 20% of failures. He spends 5+ hours per month manually reviewing failed payments and reaching out to high-value customers. The CEO asks about churn every board meeting, and involuntary churn makes the numbers look worse than they are.
- **Goals**: Wants to automate the entire failed payment recovery process end-to-end. Needs to segment recovery efforts by customer value (enterprise customers get different treatment than $9/month subscribers). Wants to present a clean "recovered revenue" number in board decks.
- **Tech Comfort Level**: Moderate -- uses Stripe and analytics tools but relies on engineering for API work. Comfortable reading dashboards and configuring email sequences.

### Persona 3: Priya Patel
- **Age**: 28
- **Job**: Solo founder of a niche subscription box company (organic snacks, $65K MRR, 2,200 subscribers)
- **Income**: $70,000/year
- **Pain Points**: Card failures are her biggest source of churn -- about 8% of charges fail each month. She cannot afford a dedicated engineer to build retry logic. She manually emails customers when payments fail, which takes hours and feels awkward. She uses Stripe only (no multi-processor need) and wants the simplest possible solution.
- **Goals**: Wants to set up DunningGuard in 15 minutes and never think about failed payments again. Needs the cost to be justified by recovered revenue from Day 1. Wants SMS recovery because her customers (health-conscious millennials) respond better to texts than emails.
- **Tech Comfort Level**: Low-to-moderate -- can navigate Stripe and Shopify but avoids anything that requires code. Needs a guided setup wizard.

## 3. User Stories (20+)

1. As a SaaS founder, I want to connect my Stripe account to DunningGuard in under 5 minutes so that I can start recovering failed payments immediately without engineering involvement.
2. As a SaaS founder, I want to see a real-time dashboard showing total failed payments, recovered payments, recovery rate, and net revenue impact so that I can quantify the ROI of the tool.
3. As a head of growth, I want DunningGuard to automatically retry failed payments using optimized timing (time-of-day, day-of-week) and card-type-specific logic so that recovery rates exceed Stripe's default retry.
4. As a head of growth, I want to receive pre-dunning alerts 14 days before a customer's card expires so that I can proactively prompt them to update their payment method before a failure occurs.
5. As a SaaS founder, I want DunningGuard to send automated email recovery campaigns with a one-click payment update link when a payment fails so that customers can resolve the issue without contacting support.
6. As a subscription box owner, I want DunningGuard to send SMS recovery messages to customers with failed payments so that I can reach them on their preferred channel.
7. As a head of growth, I want DunningGuard to use Account Updater APIs to automatically refresh expired or replaced card details so that payments succeed without any customer action.
8. As a SaaS founder, I want to customize the dunning email templates (subject, body, branding) so that recovery messages match my company's voice and design.
9. As a head of growth, I want to segment recovery campaigns by customer value (MRR tier) so that high-value enterprise customers receive personalized outreach while low-tier customers get automated flows.
10. As a SaaS founder, I want to see a timeline view of each failed payment showing every retry attempt, email sent, and customer action so that I can understand the recovery journey.
11. As a head of growth, I want to view recovery analytics broken down by failure reason (insufficient funds, expired card, bank decline, fraud flag) so that I can identify systemic issues.
12. As a SaaS founder, I want DunningGuard to integrate with Slack so that I receive real-time notifications when a high-value payment fails or is recovered.
13. As a subscription box owner, I want a guided setup wizard that walks me through connecting Stripe, configuring retry schedules, and customizing email templates in under 15 minutes so that I do not need technical help.
14. As a head of growth, I want to A/B test different dunning email subject lines and send times so that I can optimize recovery rates over time.
15. As a SaaS founder, I want to export recovery data as CSV so that I can include it in board reports and financial models.
16. As a SaaS founder, I want DunningGuard to support Paddle in addition to Stripe so that I can recover payments across multiple processors.
17. As a head of growth, I want to set up a multi-step recovery sequence (retry > email > wait > retry > SMS > final notice) with configurable delays between steps so that I have full control over the dunning cadence.
18. As a SaaS founder, I want to see a monthly "revenue saved" report showing total dollars recovered, recovery rate improvement over time, and comparison to Stripe's default recovery so that I can justify the subscription cost to my co-founder.
19. As a subscription box owner, I want to pause a customer's subscription automatically after a configurable number of failed retries (instead of cancelling) so that I can retain the relationship.
20. As a head of growth, I want DunningGuard to white-label the payment update page with my company's branding (logo, colors, domain) so that customers see a consistent experience.
21. As a SaaS founder, I want to receive a weekly digest email summarizing failed payments, recoveries, and net churn impact so that I stay informed without logging into the dashboard.
22. As a head of growth, I want to integrate DunningGuard with my CRM (HubSpot, Salesforce) so that failed payment events and recovery outcomes are logged against customer records.
23. As a SaaS founder, I want DunningGuard to detect and flag potentially fraudulent payment failures (repeated failures from the same IP with different cards) so that I do not waste recovery efforts on fraud.
24. As a subscription box owner, I want to offer customers a one-click option to switch to a different payment method (e.g., PayPal, bank transfer) during the recovery flow so that I maximize the chance of retaining them.

## 4. Feature Requirements

### MVP (v1.0) -- Must Have
- [ ] Stripe OAuth integration with guided setup wizard: connect a Stripe account in under 5 minutes, receive a webhook for every failed payment event (acceptance criteria: connection completes without code, webhook reliability 99.9%+)
- [ ] Smart retry engine: automatically retry failed payments using optimized timing based on failure reason, card type, day-of-week, and time-of-day (acceptance criteria: retry schedule is configurable, default schedule outperforms Stripe's native retry by 15%+ in A/B test)
- [ ] Pre-dunning card expiration alerts: detect cards expiring within 14 days and send branded email prompts to update payment method (acceptance criteria: emails sent 14 and 3 days before expiration with one-click update link)
- [ ] Email dunning campaign system: configurable multi-step email sequence triggered on payment failure with customizable templates, merge tags, and send timing (acceptance criteria: at least 4-step sequence configurable, supports HTML templates with brand customization)
- [ ] One-click payment update page: hosted page where customers can update their credit card or payment method via a secure link, branded with the customer's company logo and colors (acceptance criteria: PCI-compliant, loads in under 2 seconds, mobile responsive, supports all major card types)
- [ ] Recovery dashboard: real-time metrics showing total failed payments, total recovered, recovery rate, revenue at risk, recovered revenue, and comparison to baseline (Stripe default) (acceptance criteria: data refreshes within 5 minutes, supports date range filtering)
- [ ] Failed payment timeline: for each failed payment, show a chronological view of every retry attempt, email sent, customer click, and eventual outcome (acceptance criteria: timeline includes timestamps, event types, and status)
- [ ] SMS recovery campaign: send customizable SMS messages via Twilio with a payment update link when email recovery fails (acceptance criteria: SMS sent only after email sequence completes, configurable opt-in, compliant with TCPA)
- [ ] Slack integration: send real-time notifications to a configured Slack channel when payments fail, are recovered, or when high-value customers (above a configurable MRR threshold) are at risk (acceptance criteria: Slack OAuth connection, configurable notification thresholds)
- [ ] Account Updater integration: automatically use Stripe's Account Updater to refresh expired or replaced card numbers before retry (acceptance criteria: updates processed within 24 hours of card change, success rate tracked in dashboard)
- [ ] Webhook event processing: reliably ingest and process Stripe webhook events (invoice.payment_failed, invoice.paid, customer.subscription.updated) with idempotency and retry logic (acceptance criteria: zero duplicate processing, 99.99% event delivery)

### v2.0 -- Should Have
- [ ] Paddle integration: extend all recovery features to Paddle-processed payments with full parity to Stripe features
- [ ] Customer value segmentation: tag customers by MRR tier (low/medium/high/enterprise) and configure different recovery sequences per tier
- [ ] A/B testing for dunning emails: test different subject lines, send times, and email copy with statistical significance reporting
- [ ] CRM integration (HubSpot, Salesforce): sync failed payment and recovery events to customer records for sales team visibility
- [ ] CSV and PDF export: export recovery analytics and failed payment details for board reports and financial modeling
- [ ] Custom domain for payment update pages: allow customers to serve the payment update page on their own domain (e.g., billing.theircompany.com)
- [ ] Auto-pause (instead of cancel): after a configurable number of failed retries, pause the subscription instead of cancelling, with an automated reactivation email sequence
- [ ] Weekly digest email: automated summary of failed payments, recoveries, revenue impact, and trends sent to configurable recipients

### v3.0 -- Nice to Have
- [ ] Braintree and Recurly integration: extend to additional payment processors for multi-processor customers
- [ ] Fraud detection flags: identify patterns suggesting fraudulent payment failures (repeated failures, mismatched geolocation, velocity checks) and suppress recovery attempts
- [ ] Revenue forecasting: predict future payment failures based on card expiration patterns, historical failure rates, and seasonal trends
- [ ] Multi-currency support: handle recovery flows for international customers with localized dunning emails and currency display
- [ ] AI-optimized retry timing: use machine learning on the platform's aggregate recovery data to dynamically optimize retry timing per failure pattern (moving beyond rule-based optimization)

## 5. Technical Architecture
- **Frontend**: React with Next.js 14 (App Router) -- chosen for server-side rendering of the marketing site and fast dashboard interactions. Recharts for data visualization (recovery metrics, trend charts). Tailwind CSS and shadcn/ui for a polished, consistent design system. The dashboard is a single-page application with real-time updates via WebSocket connections.
- **Backend**: Node.js with NestJS framework -- chosen for its modular architecture that suits a multi-integration product (Stripe module, Paddle module, email module, SMS module), built-in dependency injection, and TypeScript support. Bull queue (backed by Redis) for reliable background job processing (retry scheduling, email campaigns, webhook ingestion). NestJS provides better structure than Express for a product that will scale to multiple integrations.
- **Database**: PostgreSQL on AWS RDS -- chosen for ACID compliance (financial data integrity is critical), complex query support (recovery analytics, cohort analysis, time-series aggregation), and mature ecosystem. Redis (AWS ElastiCache) for job queue management, rate limiting, and caching dashboard queries. Schema designed for multi-tenancy with row-level security.
- **Key APIs**:
  - Stripe API -- webhook ingestion for payment events, payment retry execution, Account Updater, customer and subscription management
  - Paddle API (v2.0) -- equivalent webhook and retry capabilities for Paddle-processed payments
  - Twilio API -- SMS delivery for recovery messages, delivery status tracking, opt-out management
  - SendGrid API -- transactional email delivery for dunning campaigns, pre-dunning alerts, and digest emails with template rendering
  - Slack API -- OAuth integration for real-time notification delivery to customer Slack workspaces
  - Stripe Connect -- for the OAuth connection flow that allows customers to connect their Stripe accounts securely
- **Hosting**: AWS (us-east-1) -- EC2 (t3.medium) or ECS Fargate for the NestJS application ($50-100/month), RDS PostgreSQL (db.t3.small) for the database ($30-50/month), ElastiCache Redis for queues ($25/month), S3 for email templates and static assets ($5/month), CloudFront CDN for the payment update pages ($10/month). Total infrastructure: ~$120-190/month at launch. ALB for load balancing as traffic scales. Estimated cost at 200 customers: ~$400/month.

## 6. Data Model

### Organizations (Tenants)
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| name | String | Company name |
| stripe_account_id | String | Connected Stripe account |
| paddle_account_id | String | Nullable, v2.0 |
| plan | Enum | free, growth, enterprise |
| mrr_tier | Enum | starter, growth, scale |
| slack_webhook_url | String | Nullable |
| brand_logo_url | String | For payment update page |
| brand_color | String | Hex code |
| created_at | Timestamp | |

### Users
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| organization_id | UUID | FK to Organizations |
| email | String | Unique per org |
| password_hash | String | bcrypt |
| role | Enum | owner, admin, viewer |

### FailedPayments
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| organization_id | UUID | FK to Organizations |
| stripe_invoice_id | String | Stripe reference |
| stripe_customer_id | String | Stripe customer |
| amount | Decimal | Failed charge amount |
| currency | String | e.g., usd |
| failure_reason | Enum | insufficient_funds, expired_card, bank_decline, fraud, other |
| card_type | String | visa, mastercard, amex |
| card_last_four | String | For display |
| customer_email | String | For outreach |
| customer_mrr | Decimal | For segmentation |
| status | Enum | open, recovering, recovered, lost |
| recovered_at | Timestamp | Nullable |
| created_at | Timestamp | |

### RetryAttempts
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| failed_payment_id | UUID | FK to FailedPayments |
| attempt_number | Integer | 1, 2, 3... |
| scheduled_at | Timestamp | When retry was scheduled |
| executed_at | Timestamp | When retry ran |
| result | Enum | success, failed, skipped |
| failure_code | String | Stripe decline code |

### DunningMessages
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| failed_payment_id | UUID | FK to FailedPayments |
| channel | Enum | email, sms |
| template_id | UUID | FK to EmailTemplates |
| sent_at | Timestamp | |
| opened_at | Timestamp | Nullable |
| clicked_at | Timestamp | Nullable |
| status | Enum | sent, delivered, opened, clicked, bounced |

### EmailTemplates
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| organization_id | UUID | FK to Organizations |
| name | String | Template name |
| subject | String | Email subject with merge tags |
| body_html | Text | HTML template |
| step_number | Integer | Position in sequence |
| delay_hours | Integer | Hours after previous step |

### RecoverySequences
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| organization_id | UUID | FK to Organizations |
| name | String | Sequence name |
| steps | JSONB | Ordered array of {type, delay, template_id} |
| mrr_segment | Enum | all, low, medium, high, enterprise |
| is_default | Boolean | |

### Relationships
- An Organization has many Users, FailedPayments, EmailTemplates, and RecoverySequences
- A FailedPayment has many RetryAttempts and DunningMessages
- A RecoverySequence defines the automation flow for a given customer segment
- DunningMessages reference EmailTemplates for rendering

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Marketing Landing Page
The user (SaaS founder) sees a headline: "Recover 40-70% of Failed Payments. Automatically." Below it, a live counter showing total dollars recovered across all DunningGuard customers (social proof). Three feature columns: Smart Retry, Pre-Dunning, SMS Recovery. A "Connect Stripe Free" CTA button leading to the onboarding flow. Below the fold: a comparison table (DunningGuard vs. Stripe Default vs. Churnkey vs. Manual), customer testimonials with recovered revenue stats, and a pricing section. The page is clean, data-driven, and speaks the language of SaaS metrics.

### Screen 2: Onboarding / Stripe Connection
After signup, the user sees a 3-step wizard. Step 1: "Connect Your Stripe Account" with a prominent Stripe Connect OAuth button. When clicked, Stripe's authorization modal opens. After successful connection, a loading animation shows "Analyzing your payment history..." and then displays: "We found X failed payments in the last 90 days worth $Y. You recovered Z% with Stripe default. DunningGuard can recover up to W%." This is the "aha moment." Step 2: Configure recovery sequence (or use default). Step 3: Customize email branding. A "Go Live" button activates the system.

### Screen 3: Recovery Dashboard (Main Screen)
The primary view after onboarding. Top row: four metric cards -- Revenue at Risk (total failed this period), Revenue Recovered (total recovered), Recovery Rate (percentage), and Net Revenue Impact (dollars saved vs. Stripe default). Below: a time-series line chart showing daily failed vs. recovered payments over the selected date range (7d, 30d, 90d, custom). Below the chart: a breakdown table by failure reason (pie chart: insufficient funds, expired card, bank decline, fraud) and by recovery method (retry, email, SMS, account updater). All metrics are filterable by date range and customer segment.

### Screen 4: Failed Payments List
A sortable, filterable table of all failed payment events. Columns: Customer Name, Email, Amount, Failure Reason, Status (open/recovering/recovered/lost), Recovery Method, Date. Each row is clickable to open the payment timeline. Filters: status, failure reason, amount range, date range, customer MRR tier. Bulk actions: export CSV, manually trigger retry, send dunning email. A search bar allows finding specific customers by name or email.

### Screen 5: Payment Timeline Detail
Clicking a failed payment opens a full-screen timeline view. At the top: customer name, email, MRR, subscription plan, card type (last four digits). The timeline shows every event chronologically: initial failure (with decline code), retry attempt 1 (scheduled time, result), dunning email 1 (sent, opened, clicked), retry attempt 2, SMS sent, payment update link clicked, card updated, final retry success. Each event has an icon, timestamp, and status indicator (green check, red X, yellow clock). Action buttons: "Retry Now," "Send Custom Email," "Mark as Lost."

### Screen 6: Recovery Sequence Builder
A drag-and-drop visual builder for configuring the dunning sequence. The user sees a vertical flow: Trigger (Payment Failed) > Step 1 (Smart Retry, delay: 4 hours) > Step 2 (Email #1, delay: 24 hours) > Step 3 (Smart Retry, delay: 48 hours) > Step 4 (SMS, delay: 72 hours) > Step 5 (Email #2 -- final notice, delay: 120 hours) > End (Pause or Cancel subscription). Each step is a draggable card that can be reordered, edited (change template, timing), or removed. Multiple sequences can be created for different customer segments (e.g., enterprise customers get a Slack DM to the account manager instead of SMS).

### Screen 7: Email Template Editor
A WYSIWYG email editor with brand customization. The user sees a split view: editor on the left, live preview on the right. The editor supports: logo upload, brand color picker, subject line with merge tags ({customer_name}, {amount}, {update_link}), body text with formatting, and a prominent CTA button ("Update Payment Method"). Pre-built templates are available: "Friendly Reminder," "Urgent Notice," "Final Warning," and "Card Expiring Soon." The preview shows the email rendered on desktop and mobile viewports.

### Screen 8: Payment Update Page (Customer-Facing)
This is the page the end customer (the SaaS founder's customer) sees when they click the payment update link. It displays the SaaS company's logo and brand colors, a message ("Your payment of $X for [Product Name] failed. Please update your card to continue your subscription."), a Stripe Elements card input field, and a "Update & Pay" button. Below: alternative payment method options (if configured). The page is simple, trustworthy, mobile-first, and loads in under 2 seconds. After successful update, a confirmation message and "Return to [Product Name]" link.

### Screen 9: Analytics & Reporting
A deep-dive analytics screen with multiple tabs: Recovery Performance (recovery rate by time period, by failure reason, by card type), Revenue Impact (total recovered, projected annual impact, comparison to baseline), Email Performance (open rates, click rates, conversion rates by template), SMS Performance (delivery rate, click rate), and Cohort Analysis (recovery rates for customers acquired in different months). All charts are exportable as PNG or CSV. A "Generate Board Report" button creates a PDF summary of key metrics.

### Screen 10: Settings & Billing
Organization settings: company name, branding (logo, colors), connected payment processors (Stripe status, add Paddle), Slack integration, notification preferences. Team management: invite users, assign roles (owner, admin, viewer). Billing: current plan (free/growth/enterprise), usage (total recovered this month, performance fee calculation), invoices, upgrade/downgrade. API keys: for headless integration. Danger zone: disconnect Stripe, delete account.

## 8. Monetization Implementation

### Paywall Placement
The free tier provides a read-only dashboard showing failed payment analytics and recovery rate for up to $10K MRR. This is a product-led growth hook: founders connect Stripe, see exactly how much money they are losing, but cannot activate smart retry, dunning emails, or SMS recovery. The data is the sales pitch -- the dashboard literally shows them the revenue they are leaving on the table.

### Upgrade Triggers
- During onboarding, after the initial Stripe analysis: "You lost $3,200 to failed payments last quarter. Activate DunningGuard to recover up to $2,240."
- On the free dashboard, every failed payment has a grayed-out "Recover" button with a tooltip: "Upgrade to Growth to activate automatic recovery."
- Weekly digest email for free users: "You had 12 failed payments this week worth $890. DunningGuard Growth customers recover 55% on average."
- When a card expiration is detected: "This customer's card expires in 7 days. Upgrade to send a pre-dunning alert."

### Pricing Psychology
- The $49/month Growth plan is positioned as "less than the cost of one lost customer" -- since the average SaaS customer is worth significantly more than $49/month, the tool pays for itself with a single recovery
- The 5% performance fee (Growth) vs. 3% performance fee (Enterprise) aligns incentives: DunningGuard only makes money when the customer makes money. This eliminates objections about ROI
- Enterprise customers who recover more than $10K/month can negotiate flat-fee pricing to avoid uncapped performance fees at scale
- Annual plan discount (20%) offered to Enterprise tier to lock in 12-month commitments and improve net revenue retention

## 9. Analytics & KPIs

| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| Total dollars recovered (all customers) | $15,000 | $180,000/mo | $600,000/mo |
| Average recovery rate | 35% | 50% | 60% |
| New trial activations | 20 | 15/week | 25/week |
| Trial-to-paid conversion rate | 10% | 15% | 18% |
| Paying customers (cumulative) | 10 | 50 | 80 |
| Monthly recurring revenue (MRR) | $2,000 | $12,500 | $20,000+ |
| Average revenue per customer | $200/mo | $250/mo | $300/mo |
| Customer churn rate | 5% | 3% | 2.5% |
| Net revenue retention | 105% | 115% | 125% |
| Median time to first recovery | 72 hours | 36 hours | 24 hours |
| Dunning email open rate | 40% | 50% | 55% |
| SMS click-through rate | 15% | 22% | 28% |

## 10. 12-Week Launch Plan

| Week | Milestone |
|------|-----------|
| Week 1 | Initialize NestJS project with TypeScript, set up PostgreSQL on AWS RDS, configure Redis for Bull queues, establish CI/CD pipeline (GitHub Actions to AWS ECS). Register Stripe Connect application and obtain OAuth credentials. Design database schema for multi-tenancy. |
| Week 2 | Build Stripe OAuth connection flow (Stripe Connect onboarding), webhook ingestion system (invoice.payment_failed, invoice.paid events) with idempotency keys, and initial failed payment data model. Test with Stripe test mode. |
| Week 3 | Build smart retry engine: implement retry scheduling logic with configurable timing based on failure reason, card type, and day-of-week. Integrate with Stripe API to execute retries. Build retry attempt logging and result tracking. |
| Week 4 | Build pre-dunning system: detect cards expiring within 14 days via Stripe customer data, generate expiration alerts, send branded emails via SendGrid. Build the one-click payment update page (Stripe Elements hosted page with brand customization). |
| Week 5 | Build email dunning campaign system: multi-step sequence engine, email template editor with merge tags and WYSIWYG preview, configurable delays between steps. Integrate SendGrid for delivery with open/click tracking. |
| Week 6 | Build SMS recovery: Twilio integration for sending recovery texts with payment update links, TCPA-compliant opt-in/out management, delivery status tracking. Build the recovery sequence builder UI (drag-and-drop flow editor). |
| Week 7 | Build the recovery dashboard: real-time metrics (revenue at risk, recovered, recovery rate), time-series charts, failure reason breakdown, recovery method attribution. Build the failed payments list with filtering and payment timeline detail view. |
| Week 8 | Build Slack integration (OAuth + webhook notifications), Account Updater integration (Stripe automatic card updates), CSV export, and weekly digest email. Build the settings/billing page with Stripe subscription for DunningGuard's own billing. |
| Week 9 | Internal testing and beta program: recruit 5-10 beta customers from SaaS Twitter/Indie Hackers network. Connect real Stripe accounts in live mode. Monitor recovery performance, fix bugs, tune retry timing, and gather feedback on email templates and dashboard UX. |
| Week 10 | Prepare launch assets: submit to Stripe App Marketplace (review process takes 1-2 weeks), write 3 SaaS Twitter threads with anonymized recovery data from beta, draft Indie Hackers and r/SaaS case study posts, create Product Hunt listing. |
| Week 11 | Public launch: publish Stripe App Marketplace listing, launch on Product Hunt, post case study on Indie Hackers and r/SaaS, publish SaaS Twitter threads. Offer "founding customer" pricing (50% off first 3 months) for the first 20 customers. Monitor support channels and respond to every inquiry within 2 hours. |
| Week 12 | Post-launch optimization: analyze conversion funnel from Stripe Marketplace to connected account to paid plan. A/B test onboarding messaging (emphasize dollars at risk vs. recovery rate vs. competitor comparison). Begin cold outreach to 50 Stripe-powered SaaS companies via personalized Loom videos. Set Month 2-3 growth targets based on launch data. |

## 11. Growth Loops

### Revenue Recovery Proof Loop
Every dollar recovered is proof the product works. Customers see the ROI in their dashboard daily, reinforcing retention. DunningGuard aggregates anonymized recovery data ("Our customers recovered $2.1M this quarter") for marketing content, social proof, and case studies. The better the product performs, the more compelling the marketing becomes, which drives new customer acquisition.

### Stripe App Marketplace Distribution
Listing on the Stripe App Marketplace provides a permanent acquisition channel. SaaS founders browsing Stripe's app ecosystem for revenue tools discover DunningGuard with one-click installation. As DunningGuard accumulates reviews and installs, it ranks higher in the marketplace, driving more organic discovery -- a self-reinforcing loop.

### SaaS Community Word-of-Mouth
SaaS founders talk to other SaaS founders about tools that impact revenue. When a DunningGuard customer shares their recovery rate improvement in a Slack group, Twitter thread, or podcast interview, it reaches a highly qualified audience. The performance-based pricing model makes the recommendation easy: "It's free unless it recovers money for you." This eliminates friction in the referral conversation.

### Customer Growth = Revenue Growth
As DunningGuard's customers grow their own MRR (and therefore process more payments), the volume of failed payments increases, which increases DunningGuard's performance fee revenue without acquiring new customers. This net revenue retention loop means each customer becomes more valuable over time without additional acquisition cost.

## 12. Regulatory & Compliance

### PCI DSS Compliance
- DunningGuard itself never stores, processes, or transmits raw credit card numbers. Payment method updates are handled through Stripe Elements (Stripe's PCI-compliant embeddable form), which tokenizes card data before it reaches DunningGuard's servers. This qualifies DunningGuard for SAQ-A (the simplest PCI self-assessment questionnaire).
- The payment update page must be served over HTTPS with TLS 1.2+ and must not include any JavaScript that intercepts or logs card input fields.

### TCPA Compliance (SMS)
- SMS recovery messages require prior express written consent from the end customer. DunningGuard must provide its B2B customers (SaaS founders) with compliant consent collection language for their own terms of service.
- Every SMS must include an opt-out mechanism ("Reply STOP to unsubscribe").
- DunningGuard must maintain opt-out lists per organization and suppress messages to opted-out numbers.

### Data Privacy (GDPR / CCPA)
- DunningGuard processes customer payment data on behalf of its B2B customers, making it a "data processor" under GDPR. A Data Processing Agreement (DPA) must be provided to all customers.
- End-customer data (email, card last four, payment history) must be deletable upon request (right to erasure). Implement a data retention policy: delete failed payment data 24 months after the event unless the customer requests earlier deletion.
- CCPA compliance: provide California residents (end-customers) with the right to know what data is collected and the right to delete.

### Financial Regulations
- DunningGuard retries payments on behalf of merchants through their existing Stripe/Paddle accounts. It does not process payments itself, so money transmitter licensing is not required.
- The performance-based fee model (% of recovered revenue) does not constitute debt collection (the payments are recurring subscription charges, not debts), so Fair Debt Collection Practices Act (FDCPA) does not apply.

### SOC 2 Compliance
- Target SOC 2 Type II certification within 12 months of launch. Financial data handling for B2B SaaS customers requires demonstrable security controls, and enterprise customers will request SOC 2 reports during procurement.

## 13. Risk Register

| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| Stripe improves its built-in Smart Retries to the point where third-party recovery tools add marginal value | Medium | Critical | Differentiate on features Stripe will not build: pre-dunning emails, SMS recovery, multi-step dunning campaigns, cross-processor support, and customer segmentation. Stripe's incentive is to remain a platform, not a vertical dunning solution. Build enough value beyond retry alone that Stripe improvement does not eliminate the product's utility. |
| Large customers push back on the performance-based fee as their MRR scales, demanding flat pricing or churning | High | High | Offer flat-fee enterprise pricing for customers recovering more than $10K/month. Lock in annual contracts with volume discounts. Monitor customer recovery volumes and proactively offer plan restructuring before customers reach pain points. The goal is to retain large customers at lower margins rather than lose them. |
| Payment processor API changes (webhook structure, rate limits, deprecations) break integrations without warning | Medium | High | Build a processor abstraction layer that normalizes events across Stripe, Paddle, and Braintree. Maintain automated integration test suites that run against processor sandbox environments daily. Subscribe to Stripe's API changelog and developer newsletter. Budget engineering time for integration maintenance every sprint. |
| Beta customers have low recovery rates due to insufficient data for optimization, leading to poor early testimonials | Medium | Medium | Set realistic expectations during onboarding ("optimization improves over 30 days as we learn your patterns"). Provide hands-on onboarding support for the first 20 customers. Supplement smart retry with manual recommendations based on industry benchmarks. Front-load email/SMS recovery to show immediate value even before retry optimization kicks in. |
| TCPA litigation from SMS recovery messages sent without proper consent documentation | Low | Critical | Require B2B customers to attest they have consent before enabling SMS. Provide template consent language and a compliance checklist. Implement a double opt-in flow as an optional safety measure. Carry TCPA liability insurance. Consult a telecommunications attorney before launching SMS features. |
| Competitor (e.g., Churnkey, new entrant) launches a comparable product with aggressive pricing or a free tier | Medium | Medium | Move fast on multi-processor support (Stripe + Paddle + Braintree) as a differentiation moat. Build deep integrations (CRM, Slack, custom sequences) that increase switching costs. Focus on recovery rate performance as the ultimate differentiator -- customers choose the tool that recovers the most money, not the cheapest. Maintain a transparent public comparison page. |

## 14. Success Criteria

- **6-month go/no-go**: 50 paying customers generating $12,500 MRR, with an average recovery rate of 50%+ across all customers, trial-to-paid conversion rate of 15%+, monthly customer churn below 3%, and at least $180,000 total dollars recovered for customers. If these targets are not met, evaluate whether the issue is top-of-funnel (insufficient trial activations from Stripe Marketplace and organic channels), recovery performance (smart retry is not outperforming Stripe default), or conversion (free users see the data but do not upgrade). Pivot or double down accordingly.
- **12-month milestone**: 80 paying customers generating $20,000+ MRR, with an LTV:CAC ratio of 15:1+, net revenue retention of 120%+ (customers' MRR growth increases performance fees), Paddle integration live and accounting for 15%+ of new customers, total recovered revenue exceeding $600,000/month across all customers, and Stripe App Marketplace listing achieving a 4.5+ star rating with 25+ reviews. Product recognized in at least one SaaS industry publication or podcast as a recommended tool for payment recovery.
