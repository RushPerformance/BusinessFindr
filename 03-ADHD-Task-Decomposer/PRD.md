# Product Requirements Document: ADHD Task Decomposer

## 1. Executive Summary
Task paralysis -- the inability to start tasks that feel overwhelming -- is the number one complaint among the 8.7 million US adults with ADHD. Existing task managers like Todoist and Things are designed for neurotypical brains: they assume users can see "do taxes" and simply execute. For ADHD brains, that task is a wall. The ADHD Task Decomposer solves this by using AI to break overwhelming tasks into dopamine-friendly micro-steps with time estimates, then matching step order to the user's current energy level, providing body-doubling timers with ambient sound, and offering a "just start" mode that shows only the very next action. Goblin Tools proved massive demand for AI task decomposition (viral on TikTok, millions of users) but offers no workflow, persistence, or timers. This product fills that gap for the underserved ADHD productivity niche. At $6.99/month with a projected 5% freemium conversion, the business targets $210K in Year 1 revenue from 2,500 paid users, scaling to $2.5M by Year 3 through ADHD community word-of-mouth on TikTok and Reddit.

## 2. User Personas

### Persona 1: Alex Reyes
- **Age**: 26
- **Job**: Junior Software Developer
- **Income**: $72,000/year
- **Pain Points**: Diagnosed with ADHD at 22. Struggles with task initiation at work -- large tickets like "refactor the authentication module" sit in his sprint for days because he cannot figure out where to start. Uses Todoist but his task list has become a graveyard of undone items that generates shame. Has tried the Pomodoro technique, but the 25-minute blocks feel arbitrary and he often cannot sustain focus for that long. Uses Goblin Tools occasionally but the output disappears and is not connected to any workflow.
- **Goals**: Wants a tool that helps him break work tasks into small enough steps that he can actually start. Needs something that works with his variable energy levels -- some days he can focus for an hour, other days he can barely manage 10 minutes. Wants to feel a sense of progress and accomplishment, not shame for what he did not do.
- **Tech Comfort Level**: Very high -- uses multiple apps and browser extensions. Willing to try new tools and provide feedback.

### Persona 2: Keisha Washington
- **Age**: 34
- **Job**: Marketing Manager at a mid-size company
- **Income**: $88,000/year
- **Pain Points**: Undiagnosed but strongly suspects ADHD after seeing ADHD content on TikTok. Household tasks like "clean the apartment" or "organize finances" feel impossibly large. She procrastinates until things become emergencies, then hyperfocuses under deadline pressure, which is exhausting. Has tried Notion, Apple Reminders, and sticky notes -- nothing sticks for more than two weeks because the novelty wears off.
- **Goals**: Wants a tool that makes starting tasks feel easy and low-pressure, not another productivity system that becomes a source of guilt. Needs the app to stay engaging beyond the initial novelty period (the "ADHD app graveyard" problem). Would love to share the tool with her partner, who also struggles with executive function.
- **Tech Comfort Level**: Moderate -- uses standard consumer apps, comfortable with mobile apps but not power-user features. The app needs to be simple and visually appealing.

### Persona 3: Dr. Rachel Okonkwo
- **Age**: 45
- **Job**: Licensed Clinical Psychologist specializing in ADHD
- **Income**: $130,000/year
- **Pain Points**: Recommends various apps and strategies to her ADHD clients, but none of the available tools are specifically designed for ADHD brains. She frequently tells clients to "break tasks into smaller steps" but they struggle to do this independently. She wants a tool she can recommend that does the decomposition for them and includes built-in accountability structures.
- **Goals**: Wants to recommend a clinically-informed tool to clients and potentially assign tasks within it. Needs the tool to use ADHD-friendly design principles (no punishment for missed days, positive reinforcement, flexible structure). Wants reporting on client task completion to inform therapy sessions.
- **Tech Comfort Level**: Moderate -- uses electronic health records and standard apps. Needs the therapist-facing features to be clearly separated from the client experience.

## 3. User Stories (20+)

1. As a user with ADHD, I want to type in an overwhelming task and receive a list of 5-15 concrete micro-steps with time estimates so that the task feels achievable instead of paralyzing.
2. As a user with ADHD, I want to rate my current energy level (1-5) so that the app reorders my micro-steps to match -- putting easy wins first when my energy is low and harder steps when my energy is high.
3. As a user with ADHD, I want a "just start" mode that shows me only the very next micro-step with nothing else on screen so that I am not overwhelmed by the full list.
4. As a user with ADHD, I want to start a body-doubling timer that plays ambient lofi sounds and provides gentle check-ins ("Still going? You're doing great.") so that I feel less alone and more accountable while working.
5. As a user with ADHD, I want satisfying completion celebrations when I finish a micro-step (animations, sounds, encouraging messages) calibrated to provide the dopamine hit my brain needs so that I feel motivated to continue.
6. As a user with ADHD, I want streak mechanics that do not punish me for missing days so that I do not feel shame when I inevitably have off days (grace-based streaks, not guilt-based).
7. As a user with ADHD, I want to edit, reorder, add, or remove micro-steps generated by the AI so that the decomposition matches how I actually want to approach the task.
8. As a user with ADHD, I want to save my decomposed tasks and return to them later so that my work is not lost when I close the app.
9. As a user with ADHD, I want to see my completed tasks and total micro-steps finished in a progress view so that I can appreciate what I have accomplished rather than focusing on what remains.
10. As a user with ADHD, I want to set a "time budget" for a task (e.g., "I have 20 minutes") so that the app selects only the micro-steps I can realistically complete in that window.
11. As a user with ADHD, I want to receive gentle push notification reminders for tasks I have started but not finished so that I am nudged back without pressure.
12. As a user with ADHD, I want to choose from different body-doubling audio environments (lofi, rain, coffee shop, library) so that I can pick the ambiance that helps me focus best.
13. As a user with ADHD, I want to use the app without creating an account initially so that I can try the core decomposition feature immediately with zero friction.
14. As a returning user, I want to see a "welcome back" screen that celebrates my return instead of highlighting missed tasks so that I do not feel guilty for being away.
15. As a user, I want to integrate my decomposed tasks with my existing calendar (Google Calendar, Apple Calendar) so that micro-steps show up as time blocks in my schedule.
16. As a parent of a teen with ADHD, I want to share a decomposed task (like homework or chores) with my child so that they have a guided step-by-step plan they can follow independently.
17. As an ADHD coach, I want a dashboard where I can create and assign decomposed tasks to my clients and see their completion rates so that I can track progress between sessions.
18. As a user with ADHD, I want to re-decompose a micro-step that still feels too big into even smaller sub-steps so that no step ever feels overwhelming.
19. As a user with ADHD, I want the app to learn from my patterns over time (which tasks I complete easily, which I skip) and adjust future decompositions accordingly so that the suggestions get better the more I use it.
20. As a user with ADHD, I want to browse community-shared decomposition templates for common tasks (cleaning, meal prep, taxes, job applications) so that I can start with a proven plan instead of generating from scratch.
21. As a user with ADHD, I want to set a daily "focus intention" (one task I commit to starting today) so that I have a clear anchor for the day without an overwhelming to-do list.
22. As a user with ADHD, I want to use keyboard shortcuts and quick-add from anywhere on my device so that capturing a task requires minimal friction before I forget it.
23. As a user with ADHD, I want a weekly reflection screen that shows what I accomplished (not what I missed) and asks one question ("What felt good this week?") so that I build a positive relationship with my productivity.

## 4. Feature Requirements

### MVP (v1.0) -- Must Have
- [ ] AI task decomposition engine: user enters a task description, app generates 5-15 concrete micro-steps with time estimates using GPT-4o-mini (acceptance criteria: decomposition completes in under 3 seconds, each step is actionable and specific, time estimates sum to a reasonable total)
- [ ] Energy level matching: user rates energy 1-5, app reorders micro-steps so easy/quick wins surface first at low energy and harder/longer steps surface at higher energy (acceptance criteria: reordering is instant, the rationale is visible to the user)
- [ ] "Just start" mode: a distraction-free view that displays only the current micro-step, a timer, and a "Done" button, with the next step revealed only after completion (acceptance criteria: nothing else visible on screen -- no menu, no list, no progress bar in this mode)
- [ ] Body-doubling timer: ambient audio player (lofi beats, rain, coffee shop) that runs during task execution with configurable gentle check-in messages every 5-15 minutes (acceptance criteria: audio does not interrupt when the app is backgrounded, check-ins are non-intrusive and encouraging)
- [ ] Completion celebrations: animated celebration on micro-step completion with variation (not the same animation every time) -- confetti, encouraging messages, sounds (acceptance criteria: at least 10 different celebration variants, no two identical celebrations in a row)
- [ ] Grace-based streak system: tracks activity streaks but never punishes missed days -- after a gap, shows "Welcome back! Your streak picks up where you left off" instead of resetting to zero (acceptance criteria: no red badges, no guilt language, streak pauses rather than resets)
- [ ] Task persistence and history: all decomposed tasks are saved and accessible, with completion state preserved across sessions (acceptance criteria: tasks persist after app close and relaunch, completed micro-steps remain checked)
- [ ] Micro-step editing: user can edit step text, reorder steps via drag-and-drop, add new steps, remove steps, and re-decompose any step into sub-steps (acceptance criteria: all edits persist immediately, drag-and-drop is smooth on mobile)
- [ ] Progress dashboard: view showing completed tasks, total micro-steps finished today/this week/all time, and a celebration of recent accomplishments (acceptance criteria: defaults to showing achievements, not pending items)
- [ ] Free tier gating: 3 free decompositions per day, basic micro-step view and completion tracking; paywall for unlimited decompositions, energy matching, body-doubling, and streaks (acceptance criteria: free tier is genuinely useful to drive retention, paywall appears contextually and not intrusively)
- [ ] Guest mode: allow initial task decomposition without account creation, prompt for signup after second use to save progress (acceptance criteria: first decomposition works with zero friction, data from guest session migrates to account on signup)
- [ ] Push notification reminders: configurable gentle reminders for in-progress tasks, phrased encouragingly ("Your task 'clean kitchen' is waiting -- just the next step takes 3 minutes") (acceptance criteria: user controls frequency and quiet hours, language is always encouraging and never guilt-inducing)

### v2.0 -- Should Have
- [ ] Calendar integration (Google Calendar, Apple Calendar): export micro-steps as time-blocked calendar events
- [ ] Community decomposition templates: browse and use crowd-sourced task templates for common tasks (cleaning, cooking, homework, job applications) with ratings
- [ ] Time budget mode: user sets available time, app selects micro-steps that fit within that window
- [ ] Personalization engine: learn from user's completion patterns (which steps get skipped, which tasks take longer than estimated) and adjust future decompositions
- [ ] Daily focus intention: set one primary task for the day, featured prominently on the home screen
- [ ] Weekly reflection screen: accomplishment summary with a positive framing and a single reflection prompt
- [ ] Multiple body-doubling audio environments: expand from 3 to 8+ ambient sound options including nature, white noise, binaural beats, and user-uploaded audio
- [ ] Share task lists: send a decomposed task to another user (parent-to-teen, partner-to-partner) with shared completion tracking

### v3.0 -- Nice to Have
- [ ] Therapist/coach dashboard: create and assign decomposed tasks to clients, view completion analytics, generate session preparation reports
- [ ] Family plan: up to 3 linked accounts with shared task templates and completion celebrations
- [ ] Custom celebration sounds and animations: upload personal audio clips or choose from an expanded library
- [ ] Widget support (iOS/Android): home screen widget showing current micro-step and quick "Done" button
- [ ] Wearable integration (Apple Watch, Wear OS): receive micro-step prompts and tap-to-complete on wrist

## 5. Technical Architecture
- **Frontend**: React Native with Expo -- chosen for cross-platform mobile development (iOS and Android from a single codebase), critical because the ADHD audience primarily uses mobile devices for productivity apps. Expo simplifies push notifications, audio playback, and app store deployment. React Native Reanimated for smooth celebration animations. NativeWind (Tailwind for React Native) for consistent, rapid styling.
- **Backend**: Node.js with Express.js on Railway -- chosen for simplicity, fast deployment, and Railway's generous free/starter tiers that keep hosting costs below $100/month. TypeScript throughout. The backend is relatively thin: user auth, task CRUD, and an API gateway to OpenAI. Background jobs (reminders, streak calculations) handled by BullMQ on Redis.
- **Database**: PostgreSQL on Supabase -- chosen for relational integrity (users have tasks, tasks have micro-steps, micro-steps have completion states), Supabase's built-in auth (reduces development time), real-time subscriptions for live task updates, and row-level security for future multi-user features (therapist dashboard, family plans). Supabase's free tier supports up to 50,000 monthly active users.
- **Key APIs**:
  - OpenAI API (GPT-4o-mini) -- task decomposition engine, generating micro-steps from natural language task descriptions with time estimates and difficulty ratings. Chosen for quality and low cost ($0.003/decomposition)
  - Supabase Auth -- user authentication (email/password, Google OAuth, Apple Sign-In) with session management
  - Expo Push Notifications -- cross-platform push notification delivery for task reminders
  - Google Calendar API and Apple EventKit -- calendar integration for time-blocked micro-step scheduling (v2.0)
  - RevenueCat -- in-app subscription management for iOS and Android, handling receipts, trials, and cross-platform entitlement
  - Sentry -- error tracking and performance monitoring for React Native
- **Hosting**: Railway for backend API ($10-20/month at launch), Supabase for database and auth (free tier to $25/month Pro), Cloudflare R2 for audio file storage and CDN (~$5/month), Expo Application Services for app builds ($0 for free tier). Total infrastructure: ~$15-50/month at launch, scaling to ~$200/month at 10,000 users.

## 6. Data Model

### Users
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| email | String | Unique, indexed |
| name | String | Display name |
| auth_provider | Enum | email, google, apple |
| plan | Enum | free, paid, premium |
| streak_current | Integer | Current grace-based streak |
| streak_longest | Integer | All-time longest |
| last_active_date | Date | For streak calculation |
| preferences | JSONB | Audio environment, check-in frequency, quiet hours |
| created_at | Timestamp | |

### Tasks
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| title | String | Original task description |
| status | Enum | active, completed, archived |
| energy_level | Integer | 1-5, nullable (set when working) |
| total_estimated_minutes | Integer | Sum of micro-step estimates |
| total_completed_minutes | Integer | Sum of completed step estimates |
| created_at | Timestamp | |
| completed_at | Timestamp | Nullable |

### MicroSteps
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| task_id | UUID | FK to Tasks |
| parent_step_id | UUID | Nullable, FK to self (for sub-decomposition) |
| text | String | Step description |
| estimated_minutes | Integer | Time estimate |
| difficulty | Enum | easy, medium, hard |
| sort_order | Integer | Display order |
| is_completed | Boolean | Default false |
| completed_at | Timestamp | Nullable |

### BodyDoublingSessions
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| task_id | UUID | FK to Tasks, nullable |
| audio_environment | String | lofi, rain, coffee_shop, etc. |
| started_at | Timestamp | |
| ended_at | Timestamp | Nullable |
| duration_minutes | Integer | Calculated |
| steps_completed | Integer | Count during session |

### Celebrations
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| user_id | UUID | FK to Users |
| micro_step_id | UUID | FK to MicroSteps |
| celebration_type | String | confetti, fireworks, dance, etc. |
| shown_at | Timestamp | |

### CommunityTemplates (v2.0)
| Field | Type | Notes |
|-------|------|-------|
| id | UUID | Primary key |
| author_id | UUID | FK to Users |
| title | String | Template name |
| category | String | cleaning, cooking, work, etc. |
| steps | JSONB | Array of {text, estimated_minutes, difficulty} |
| use_count | Integer | Popularity metric |
| avg_rating | Decimal | 1-5 |

### Relationships
- A User has many Tasks
- A Task has many MicroSteps (ordered by sort_order)
- A MicroStep can have child MicroSteps (recursive sub-decomposition via parent_step_id)
- A User has many BodyDoublingSessions
- A BodyDoubling session is optionally linked to a Task
- Each MicroStep completion generates a Celebration record (for variety tracking)

## 7. Screen-by-Screen Wireframe Descriptions

### Screen 1: Home / Task Entry
The first screen users see after opening the app. Center of screen: a large, friendly text input field with placeholder text "What feels overwhelming right now?" and a pulsing cursor inviting interaction. The tone is warm and casual, not corporate. Below the input: a large "Break it down" button with a satisfying visual treatment (rounded, slightly animated). Below that: a "Recent tasks" section showing the last 3-5 tasks with completion progress indicators (soft progress rings, not harsh bars). No clutter, no sidebar, no menu -- just the invitation to start. A small settings gear icon in the top right.

### Screen 2: Decomposition Result
After entering a task, a brief loading animation plays (friendly, not clinical -- perhaps animated puzzle pieces assembling). Then the micro-steps appear in a vertical list, each showing: step number, step text, estimated time (pill-shaped tag: "3 min"), and a difficulty indicator (color-coded: green=easy, yellow=medium, orange=hard). At the top: the original task title and total estimated time. Below the list: two prominent buttons: "Just Start" (enters just-start mode) and "Start with Timer" (enters body-doubling mode). A secondary row of actions: "Edit Steps," "Set Energy Level," "Save for Later." If the user is on the free tier and has used their 3 daily decompositions, a gentle paywall appears instead of the fourth decomposition.

### Screen 3: Energy Level Selector
A full-screen overlay triggered by tapping "Set Energy Level" or automatically prompted when starting a task. Five large, colorful buttons arranged vertically, each with an emoji-like icon and label: 1 (Exhausted -- "I can barely lift my phone"), 2 (Low -- "I can do tiny things"), 3 (Medium -- "I've got some fuel"), 4 (Good -- "Let's do this"), 5 (Supercharged -- "I'm hyperfocusing, load me up"). After selection, the micro-step list visually reorders with a smooth animation -- easy steps float to the top at low energy, hard steps rise at high energy. A brief tooltip explains the reordering.

### Screen 4: Just Start Mode
A radically minimal screen. The background color is calming (soft blue or warm gray). Only three elements are visible: the current micro-step text in large, friendly typography centered on screen, the estimated time in smaller text below it, and a single "Done" button at the bottom. No task list, no progress indicator, no menu, no distractions. When the user taps "Done," a celebration animation plays (confetti, encouraging message like "One step down -- you're unstoppable"), and the next step slides in. If the user wants to exit, they swipe down or tap a subtle "X" in the corner. This screen is the product's signature experience -- built for the ADHD brain that needs to focus on exactly one thing.

### Screen 5: Body-Doubling Timer
A focus session screen combining ambient audio with task progress. The top section shows the current micro-step and a running timer. The middle section displays a large, calming audio visualizer (gentle wave animation) with the selected environment name (e.g., "Rainy Coffee Shop"). Controls: play/pause, volume, and environment switcher (4+ ambient sound options as horizontal cards). Every 5-15 minutes (configurable), a gentle check-in appears as an overlay: "Still going? You're doing amazing" or "Need a break? That's okay -- you can come back anytime." The bottom shows a minimal progress indicator (completed X of Y steps). The screen is designed to feel like a calm, supportive presence -- a virtual body double.

### Screen 6: Completion Celebration
Triggered when a task (all micro-steps) is completed. Full-screen celebration with varied animations (confetti shower, fireworks, dancing characters, high-five illustration). A large "You did it!" message with the task name. Below: stats for the completed task (total time, micro-steps completed, streak update). A "Share your win" button generates a shareable card ("I just conquered 'clean the apartment' -- 12 micro-steps in 47 minutes"). A "What's next?" button returns to the home screen. If the user has a streak going, the streak counter updates with its own mini-celebration.

### Screen 7: Progress Dashboard
Accessible from the home screen via a small trophy/star icon. Organized around accomplishments, not obligations. Top section: "This Week" showing total micro-steps completed, total minutes focused, and tasks completed -- all displayed as achievements with upward trend arrows. Middle section: a "streak garden" visualization where each active day grows a flower or plant (grace-based -- missing days show sleeping flowers, not dead ones). Bottom section: "Recent Wins" list showing the last 10 completed tasks with completion dates. No section shows overdue or pending tasks -- this is a celebration space. A "Weekly Reflection" card appears once per week with a prompt: "What felt good this week?"

### Screen 8: Task Library
A list view of all saved tasks, organized by status tabs: "In Progress," "Completed," "Saved for Later." Each task card shows the title, progress ring (micro-steps completed / total), date created, and estimated time remaining. Tap to open and continue working. Swipe to archive. A search bar at the top filters tasks by keyword. For completed tasks, a small "Re-do" button creates a fresh copy for recurring tasks (cleaning, weekly planning, etc.). The empty state for "In Progress" is encouraging: "Nothing here -- you're either caught up or ready to break something down!"

### Screen 9: Settings and Account
Clean settings screen organized in sections. Profile: name, email, subscription status (free/paid with upgrade button). Preferences: default energy level, body-doubling check-in frequency (every 5/10/15 minutes), preferred audio environment, notification schedule (quiet hours), celebration intensity (subtle/normal/extra). Subscription: current plan, manage subscription (links to App Store/Play Store), restore purchases. Support: FAQ, contact support, community Discord link. About: version, privacy policy, terms of service. Data: export my data, delete my account.

### Screen 10: Paywall / Upgrade Screen
Appears contextually when free users hit their 3-decomposition daily limit or try to access energy matching, body-doubling, or streaks. A warm, non-pressuring design -- no "you're missing out" shame language. Headline: "Unlock your full ADHD toolkit." Feature comparison: Free (3 decompositions/day, basic view) vs. Pro at $6.99/month (unlimited decompositions, energy matching, body-doubling timer, grace-based streaks, calendar integration). Social proof: "Join 2,500+ people who stopped fighting their ADHD brain." A 7-day free trial CTA. Option to continue on the free plan without dismissal guilt ("No thanks, I'll stick with free" -- not grayed out or hidden).

## 8. Monetization Implementation

### Paywall Placement
The free tier provides 3 task decompositions per day with basic micro-step view and completion tracking. This is enough to experience the core value (the "aha moment" of seeing an overwhelming task become manageable) and build a daily habit. The paywall activates when users try to access premium features: unlimited decompositions (hits the limit), energy-level matching, body-doubling timers, grace-based streaks, and calendar integration. The key insight is that the free tier must be genuinely useful -- ADHD users are highly sensitive to feeling "tricked" or manipulated, and a too-aggressive paywall will generate backlash in the ADHD community.

### Upgrade Triggers
- Hitting the 3-decomposition daily limit: "You've used your 3 free decompositions today. Upgrade to break down unlimited tasks." (Appears after the "aha moment" is established)
- Tapping "Set Energy Level" on the free tier: "Energy matching is a Pro feature. It reorders your steps so you can start even on low-energy days."
- Tapping the body-doubling timer: "Body-doubling helps you feel less alone while you work. Try it free for 7 days."
- After completing 5 total tasks: "You've completed 5 tasks! Imagine what you could do with energy matching and body-doubling." (Triggered by demonstrated engagement, not arbitrary timing)
- Weekly re-engagement email: "You decomposed 8 tasks this week on the free plan. Pro users complete 60% more micro-steps with energy matching."

### Pricing Psychology
- $6.99/month is positioned as "less than one therapy copay" -- familiar framing for the ADHD audience, many of whom pay for therapy, coaching, or medication
- The 7-day free trial de-risks the decision for a community that has been burned by productivity app subscriptions before
- Annual plan at $49.99/year ($4.17/month) offers a 40% discount, but monthly is the default because ADHD users are commitment-averse and respond better to "cancel anytime" flexibility
- No dark-pattern cancellation flow -- cancellation is one tap in settings, and the app sends a genuine "We'll miss you, but we get it" message with an option to pause instead

## 9. Analytics & KPIs

| Metric | Target (Month 1) | Target (Month 6) | Target (Month 12) |
|--------|-------------------|--------------------|--------------------|
| Daily active decompositions | 500 | 5,000/day | 15,000/day |
| Monthly active users (free) | 2,000 | 25,000 | 50,000 |
| Free-to-paid conversion rate | 3% | 5% | 6% |
| Paid subscribers (cumulative) | 60 | 1,250 | 2,500 |
| Monthly recurring revenue (MRR) | $420 | $8,750 | $17,500 |
| Task completion rate (% of decomposed micro-steps completed) | 45% | 55% | 65% |
| Day 7 retention (free users) | 30% | 40% | 45% |
| Day 30 retention (paid users) | 55% | 65% | 70% |
| Body-doubling sessions per paid user per week | 1.5 | 3.0 | 4.0 |
| NPS score | 40 | 50 | 60 |
| TikTok/Reddit organic mentions per month | 10 | 80 | 200 |
| Average decomposition quality rating (user feedback) | 3.8/5 | 4.2/5 | 4.5/5 |

## 10. 12-Week Launch Plan

| Week | Milestone |
|------|-----------|
| Week 1 | Initialize Expo/React Native project, set up Supabase (database schema, auth), configure Railway for backend API, integrate OpenAI API for task decomposition. Build the core decomposition endpoint and test with 50+ sample tasks across categories (work, home, school, personal). |
| Week 2 | Build the Home/Task Entry screen and Decomposition Result screen. Implement micro-step generation, display, and basic editing (reorder, edit text, add, remove). Build task persistence (save/load from Supabase). |
| Week 3 | Build the Energy Level Selector with animated reordering of micro-steps. Build "Just Start" mode -- the minimal, distraction-free single-step view with "Done" button and step transitions. |
| Week 4 | Build the Body-Doubling Timer: audio player with 4 ambient environments (lofi, rain, coffee shop, library), configurable check-in messages, and background audio support. Source or license ambient audio tracks. Build step-completion celebrations (10+ animation variants using React Native Reanimated). |
| Week 5 | Build the grace-based streak system, progress dashboard (accomplishments view, streak garden visualization, weekly reflection), and task library (in-progress, completed, saved tabs). Build push notification reminders with encouraging language. |
| Week 6 | Build the paywall and subscription system: integrate RevenueCat for iOS and Android in-app purchases, implement free tier limits (3 decompositions/day), build the upgrade screen, and test the full purchase flow in sandbox environments. |
| Week 7 | Polish, accessibility, and performance: audit all screens for ADHD-friendly design (no guilt language, no red badges, calming colors). Test on 5+ device sizes. Optimize decomposition speed (target under 3 seconds). Implement Sentry for error tracking. Build settings screen with all preference controls. |
| Week 8 | Beta testing: release TestFlight (iOS) and internal testing track (Android) to 30-50 beta users recruited from r/ADHD and ADHD TikTok creators. Collect feedback via in-app survey and a private Discord channel. Focus on decomposition quality, celebration variety, and body-doubling UX. |
| Week 9 | Iterate based on beta feedback: tune decomposition prompts for quality, adjust celebration frequency and variety, fix bugs, improve energy-level matching logic. Prepare App Store and Play Store listings (screenshots, description, keywords optimized for ADHD-related search terms). |
| Week 10 | Submit to App Store and Google Play for review. Prepare launch content: 3-5 TikTok videos partnered with ADHD micro-creators, Product Hunt listing, r/ADHD soft-launch post draft, App Store Optimization (ASO) for keywords like "ADHD task manager," "task decomposer," "ADHD productivity." |
| Week 11 | Public launch: release on iOS and Android app stores. Launch on Product Hunt (target Thursday for productivity category). Post on r/ADHD with an authentic story ("I built this because I have ADHD and nothing else worked"). Publish partner TikTok content. Begin engaging in ADHD TikTok comment sections. |
| Week 12 | Post-launch analysis: review Day 1/3/7 retention data, decomposition usage patterns, free-to-paid conversion funnel, and app store reviews. Prioritize the top 5 user-requested features for v1.1. Begin outreach to ADHD coaches and therapists (email 50 providers listed on Psychology Today and CHADD). Establish a weekly content cadence on TikTok and Reddit. |

## 11. Growth Loops

### ADHD Community Word-of-Mouth
The ADHD community is one of the most vocal and loyal user bases on the internet. When ADHD users find a tool that "gets" them, they share it relentlessly -- on r/ADHD (2.1M members), ADHD TikTok (billions of views), ADHD Twitter, and in group chats with their ADHD friends. The app's "no shame" design philosophy is specifically engineered to earn this word-of-mouth: every design decision that avoids guilt, embraces inconsistency, and celebrates progress becomes a talking point. Users do not just recommend the app -- they evangelize the philosophy.

### Shareable Wins
After completing a task, users can generate a shareable card showing their accomplishment ("I just conquered 'clean the apartment' -- 12 micro-steps in 47 minutes"). This is designed for ADHD social media, where celebrating mundane task completion is a powerful bonding moment. Each share includes a download link, driving organic installs from a highly qualified audience.

### Therapist and Coach Referral Network
ADHD therapists and coaches are a high-leverage distribution channel: each provider sees dozens of clients who need exactly this tool. By building a therapist dashboard (v2.0) and offering free premium accounts to providers, the app creates a referral loop where therapists recommend the app, clients use it, and client success reinforces the therapist's recommendation to future clients.

### Content-Driven Discovery
The app's decomposition engine generates inherently shareable content: "How to clean your apartment in 12 micro-steps," "How to do your taxes in 15 micro-steps." These decomposition examples can be published as TikTok videos, Reddit posts, and blog content, driving search and social traffic to the app. Each piece of content demonstrates the product's value without requiring the viewer to sign up first.

## 12. Regulatory & Compliance

### Health and Wellness App Classification
- The ADHD Task Decomposer is a productivity and wellness tool, not a medical device. It does not diagnose, treat, or claim to treat ADHD. All marketing and in-app language must avoid medical claims (e.g., "helps you manage tasks" is acceptable; "treats ADHD symptoms" is not).
- The app should include a disclaimer: "This app is a productivity tool designed for people who struggle with task initiation. It is not a substitute for professional medical advice, diagnosis, or treatment."
- If the therapist dashboard (v3.0) is built, it must not store protected health information (PHI) or connect to electronic health records. The therapist feature is a task management tool, not a clinical tool, and must be positioned accordingly to avoid HIPAA obligations.

### Data Privacy
- **COPPA compliance**: If the app is used by children under 13 (parent-to-teen task sharing feature), COPPA requires verifiable parental consent before collecting personal information from children. The v2.0 sharing feature must implement age verification and parental consent flows.
- **CCPA/CPRA**: California residents must have the right to know, delete, and opt out of sale of personal information.
- **GDPR**: If expanding to EU markets, full GDPR compliance is required -- consent management, data portability, right to erasure, Data Protection Officer designation if processing at scale.
- **App Store privacy requirements**: Both Apple and Google require privacy nutrition labels and data collection disclosures. The app collects email, task content, usage analytics, and (if enabled) calendar data. All must be disclosed.

### AI-Generated Content Liability
- Task decompositions are generated by OpenAI's GPT models. There is a risk of inappropriate, incorrect, or harmful suggestions (e.g., a task about "declutter medicine cabinet" generating steps that could be interpreted as medication instructions). Implement content filtering and safety guardrails on the AI output.
- Terms of service should state that AI-generated decompositions are suggestions and the user is responsible for evaluating their applicateness.

### Subscription and Auto-Renewal Laws
- Apple and Google require clear disclosure of subscription terms, free trial length, and auto-renewal behavior. The paywall screen must comply with App Store Review Guidelines Section 3.1.2 (subscription disclosures).
- US FTC guidelines on auto-renewal: must clearly disclose the full terms before purchase and provide an easy cancellation mechanism.

## 13. Risk Register

| Risk | Probability | Impact | Mitigation |
|------|------------|--------|------------|
| Novelty fatigue: ADHD users adopt the app enthusiastically but abandon it within 2-4 weeks as the dopamine of a new tool wears off (the "ADHD app graveyard" problem) | High | Critical | Design for inconsistency from day one: no punishment for missed days, "welcome back" flows, variable reward celebrations (surprise animations to maintain novelty), periodic UI micro-refreshes (new celebration types, seasonal themes), and the body-doubling feature which provides ongoing utility beyond novelty. Track Day 14 and Day 30 retention obsessively. |
| OpenAI API quality degrades, pricing increases significantly, or service becomes unreliable, impacting decomposition quality and cost structure | Medium | High | Fine-tune a smaller open-source model (Llama 3 or Mistral) on 50,000+ decomposition examples as a drop-in replacement. Cache the most common task decompositions (cleaning, taxes, meal prep, job applications) to reduce API calls by 30-40%. Build a fallback to a local rules-based decomposer for simple tasks. Monitor API cost per decomposition weekly. |
| Goblin Tools adds workflow features (persistence, timers, energy matching) and becomes a direct competitor with a massive existing user base | Medium | High | Move fast on features Goblin Tools does not have and would be hard to bolt on: body-doubling audio, grace-based streaks, community templates, and the therapist dashboard. Build community-driven decomposition templates that create a data moat. Establish brand identity as "the ADHD task app that gets you" versus Goblin Tools' utility-tool positioning. |
| Backlash from the ADHD community if the app is perceived as exploitative, not "truly ADHD-friendly," or engaging in predatory monetization | Medium | High | Hire ADHD advisors and beta testers from the community. Never use guilt, shame, or FOMO in marketing or in-app messaging. Make the free tier genuinely useful (not a crippled teaser). Be transparent about pricing and make cancellation easy. Participate authentically in ADHD communities (not just marketing). If criticism emerges, respond with humility and iterate. |
| App Store rejection or delays due to subscription compliance issues, content policy violations, or performance requirements | Low | Medium | Study Apple's App Store Review Guidelines and Google Play Developer Policies thoroughly before submission. Use RevenueCat (which handles Apple/Google compliance) for subscriptions. Test on minimum supported OS versions. Submit 2 weeks before planned launch to allow for review cycles. Have a web app fallback if app store launch is delayed. |
| Data privacy incident or security breach exposing user task data (which can be deeply personal -- therapy tasks, financial tasks, relationship tasks) | Low | Critical | Encrypt all user data at rest (Supabase handles this) and in transit (TLS 1.3). Implement row-level security in Supabase so users can only access their own data. Never log task content to application logs. Conduct a security audit before launch. Minimize data collection (do not store data you do not need). Have an incident response plan and carry cyber liability insurance. |

## 14. Success Criteria

- **6-month go/no-go**: 1,250 paid subscribers generating $8,750 MRR, with a free-to-paid conversion rate of 5%+, Day 7 free user retention of 40%+, Day 30 paid user retention of 65%+, task completion rate (micro-steps completed / total generated) of 55%+, and at least 50 organic mentions on TikTok or Reddit per month. If retention targets are not met, the primary investigation should focus on whether novelty fatigue is the cause (in which case, invest in variable rewards and UI refreshes) or whether decomposition quality is the cause (in which case, invest in AI prompt engineering and community templates).
- **12-month milestone**: 2,500 paid subscribers generating $17,500 MRR, with NPS of 55+, a viral coefficient of 0.4+ (each user drives 0.4 new users through organic sharing), Day 30 paid retention of 70%+, and community templates library exceeding 500 crowd-sourced templates. iOS App Store rating of 4.7+ with 1,000+ ratings. At least 5 ADHD therapists or coaches actively recommending the app to clients. Product mentioned in at least one ADHD-focused publication (ADDitude Magazine, CHADD, or equivalent).
