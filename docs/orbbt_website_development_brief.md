# orbbt. Website Development Brief

Version: 1.0
Date: July 27, 2026
Prepared for: orbbt. / Zyntro web development team
Reference implementation: https://danish-shah-cyber.github.io/orbbt-landing-page/
Repository: https://github.com/Danish-Shah-Cyber/orbbt-landing-page

## 1. Project Summary

orbbt. is a job hunt companion for people who are actively applying to roles and need a calmer way to stay organized. The landing page should communicate that job hunting is already a job, and orbbt. reduces the mental load by keeping applications, company research, deadlines, contacts, notes, and follow-ups in one place.

The current sample site is a static HTML prototype. The production implementation can be rebuilt in any modern frontend stack, but the final experience should preserve the same product positioning, visual tone, page structure, interactions, and content hierarchy described in this document.

## 2. Product Positioning

### Core Promise

Your job hunt, organized.

### Supporting Message

Track applications, research companies, remember deadlines, and follow up from one calm place.

### One-Sentence Description

orbbt. is a job application tracker and job hunt organizer that helps job seekers track applications, research companies with AI, remember deadlines, manage contacts, and follow up without an overwhelming dashboard.

### Product Personality

orbbt. should feel calm, useful, organized, modern, and slightly alive. It should not feel like a noisy SaaS dashboard, a generic AI landing page, or a dense productivity tool. The emotional target is relief: users should feel that their messy job hunt can finally be held in one clear system.

### Primary Audience

- Students applying for internships or graduate roles.
- Recent graduates applying across many companies.
- Career switchers managing several application paths.
- Active job seekers who need a practical job application tracker.
- Future secondary audience: campuses, career teams, and small groups.

## 3. Strategic Goals

The website must:

- Explain what orbbt. does within five seconds.
- Make the product feel real through an early product screenshot.
- Separate the web app CTA from the mobile app waitlist CTA.
- Support SEO and AEO search phrases naturally.
- Present the site as calm and organized, not dense or overwhelming.
- Give visitors an immediate reason to sign up or join the mobile waitlist.
- Give developers a scalable structure for future product screenshots, testimonials, backend forms, analytics, and authentication.

## 4. Routes and Pages

### Home: `index.html`

Purpose: Main landing page and conversion surface.

Must include:

- Sticky top navigation.
- Centered hero with orbit animation.
- Floating draggable hero message banners.
- Product preview screenshot.
- Trust signal strip.
- Problem statement.
- Story section.
- Interactive feature tabs.
- How it works.
- Before and after orbbt. comparison.
- Pricing cards with CTAs.
- Contact section.
- Final CTA section.
- FAQ section.
- Footer.

### Auth: `auth.html`

Purpose: Demo sign up and log in page.

Current behavior:

- Contains Sign up and Log in tabs.
- Form submission is a demo-only local response.
- Production version should connect to actual authentication.

Primary CTA links:

- Top nav Log in.
- Top nav Sign up for free.
- Hero Try free on web.
- Pricing Try free.
- Pricing Go Pro.

### Waitlist: `waitlist.html`

Purpose: Mobile app waitlist page.

Current behavior:

- Collects name, email, and user type.
- Demo-only submission message.

Positioning:

- Waitlist is specifically for the mobile app on iOS and Android.
- Copy should reference App Store and Play Store early access.

### Privacy Policy: `privacy-policy.html`

Purpose: Legal/privacy route.

Access:

- Top nav Policies dropdown.
- Footer Resources.

### Terms and Conditions: `terms-and-conditions.html`

Purpose: Legal terms route.

Access:

- Top nav Policies dropdown.
- Footer Resources.

### Refund Policy: `refund-policy.html`

Purpose: Refund/billing route.

Access:

- Top nav Policies dropdown.
- Footer Resources.

## 5. Navigation Requirements

### Desktop Top Bar

Brand area:

- Logo image.
- Text: `orbbt.`
- Subtext: `by zyntro`

Center nav links:

- Features -> `#features`
- Pricing -> `#pricing`
- Contact -> `#contact`
- Waitlist (mobile app) -> `waitlist.html`
- Policies dropdown:
  - Privacy Policy -> `privacy-policy.html`
  - Terms and Conditions -> `terms-and-conditions.html`
  - Refund Policy -> `refund-policy.html`

Right-side actions:

- Log in -> `auth.html`
- Sign up / for free -> `auth.html`

Important:

- Do not add another Log in link beside Policies. The login action already exists on the right side.
- The Sign up button should stack the text:
  - Main line: `Sign up`
  - Small line: `for free`

### Mobile Navigation

- Use a hamburger menu.
- The nav should open as a compact dropdown panel.
- Policies should remain accessible on mobile.
- Hide the extra Log in button on very small screens if needed to preserve space.
- Keep Sign up for free as the primary mobile action.

## 6. Homepage Section-by-Section Specification

### 6.1 Hero Section

Main headline:

`Your job hunt, organized.`

Eyebrow:

`Job application tracker and job hunt organizer`

Supporting sentence:

`Track applications, research companies, remember deadlines, and follow up from one calm place.`

Benefit labels:

- Job application tracker
- AI company research
- Deadline reminders
- Contact management

Hero CTAs:

- Primary: `Try free on web` -> `auth.html`
- Secondary: `Join mobile app waitlist` -> `waitlist.html`

Small note:

`Built by Zyntro for students, graduates, active job seekers, and career switchers.`

Visual behavior:

- Centered hero text.
- Subtle animated orbit background.
- The orbit should be visible enough to feel alive, but should not compete with the headline.
- Floating message banners should sit in the vacant hero areas and not overlap the central text.

Floating banners:

- Track applications
- Research companies
- Remember deadlines
- Follow up

Floating banner interaction:

- Banners should subtly float.
- Banners should glow slightly with the orbbt. theme color.
- On hover, glow should become slightly stronger.
- User should be able to drag banners.
- After dragging, banners should stay where the user moved them during the current page session.
- The banners may continue their subtle float animation after being moved.
- Hide floating banners on mobile to prevent clutter.

### 6.2 Product Preview

Purpose: Show that orbbt. is a real product interface, not just a concept.

Section label:

`Product preview`

Heading:

`A quiet place for a very busy search.`

Body:

`orbbt. keeps jobs, contacts, companies, deadlines, and job search tracking visible without making the workflow feel heavy.`

Asset:

- Current screenshot: `app-preview.png`
- Alt text: `orbbt. job application tracker dashboard preview`

Future requirement:

- Replace static screenshot with polished final product screenshots when available.
- Keep image visible early on the page, directly after the hero.

### 6.3 Trust Strip

Purpose: Add early-stage credibility without fake testimonials.

Cards:

1. Built by Zyntro
   - `A focused product team building practical tools for modern applicants.`

2. Early access opening soon
   - `Join the mobile app waitlist for App Store and Play Store access.`

3. Made for active job seekers
   - `Designed for students, graduates, career switchers, and repeat applicants.`

### 6.4 Problem Section

Label:

`Problem`

Heading:

`Your job search should not live in ten places.`

Body:

`Applications get scattered across tabs, emails, notes, calendars, and messages. orbbt. brings the important pieces together so your next step is always clear.`

### 6.5 Story Section

Label:

`Our story`

Heading:

`We wanted the job hunt to feel lighter.`

Body:

`orbbt. started from a simple frustration: the work around applying can become heavier than the application itself.`

`So the product is intentionally simple. Save the role. Understand the company. Track what happens next. Remember who matters.`

### 6.6 Features Section

Section ID:

`features`

Label:

`Features`

Heading:

`Just the parts that keep your job search moving.`

Body:

`No giant dashboard energy. orbbt. focuses on job application management, company research, deadline reminders, and contacts.`

Interaction:

- Feature section uses horizontal clickable tabs.
- On click, update:
  - Eyebrow
  - Feature title
  - Body text
  - Bullet points
  - Preview image
  - Image alt text

Current tabs:

1. Job Tracking
2. AI Research
3. Deadline Alerts
4. Contacts

Feature content:

Job Tracking:

- Eyebrow: `Feature 01`
- Title: `Track every role without losing the thread.`
- Body: `Keep companies, roles, statuses, locations, salary notes, deadlines, and next steps in one organized view.`
- Points:
  - See applied, saved, interviewed, and rejected roles at a glance.
  - Keep job links and notes attached to each application.
  - Use the same tracker across web, mobile, and extension.

AI Research:

- Eyebrow: `Feature 02`
- Title: `Know the company before you apply.`
- Body: `AI company research helps you understand what a company does, what is public on the web, and what to prepare before outreach or interviews.`
- Points:
  - Summarize company context before you spend hours searching.
  - Prepare better answers for applications and interviews.
  - Save research beside the role you are applying for.

Deadline Alerts:

- Eyebrow: `Feature 03`
- Title: `Never let the next step go quiet.`
- Body: `Add reminders for applications, assessments, interviews, and follow-ups so your search keeps moving.`
- Points:
  - Track upcoming due dates from one place.
  - Plan follow-ups after applications and recruiter chats.
  - Reduce the feeling that something important is slipping.

Contacts:

- Eyebrow: `Feature 04`
- Title: `Remember the people behind the process.`
- Body: `Save recruiters, referrals, alumni, and hiring managers so relationship building does not disappear into messages and notes.`
- Points:
  - Keep contact notes connected to companies and jobs.
  - Remember who to follow up with and when.
  - Build a network because a strong resume is not the whole game.

Future asset plan:

- Job Tracking tab: jobs dashboard screenshot.
- AI Research tab: AI company summary screenshot.
- Deadline Alerts tab: calendar/reminder screenshot.
- Contacts tab: contact profile or relationship notes screenshot.

### 6.7 How It Works

Label:

`How it works`

Heading:

`Save. Research. Follow up.`

Steps:

1. Save a role
   - `Add jobs from web, mobile, or the Chrome extension.`

2. Get the context
   - `Use orbbt. to understand the company before you make your move.`

3. Know what is next
   - `Track deadlines, contacts, follow-ups, and status without mental clutter.`

Platforms:

- Mobile app
- Web
- Chrome extension

### 6.8 Before and After Comparison

Label:

`Before and after orbbt.`

Heading:

`Spreadsheets track data. orbbt. tracks momentum.`

Body:

`A job hunt gets messy when every next step lives somewhere else. orbbt. turns scattered effort into one organized job search tracker.`

Visual requirement:

- Two-column comparison on desktop.
- Stack columns on mobile.
- Left side uses red/soft warning styling.
- Right side uses green/positive styling.

Left column heading:

`The old way`

Left column items:

- Jobs are scattered
  - `Applications sit across tabs, emails, notes, job boards, and spreadsheets.`
- Research gets repeated
  - `You search the same company context again before every application or interview.`
- Deadlines rely on memory
  - `Assessments, follow-ups, and interviews can slip when your calendar is not connected to your tracker.`
- Contacts disappear
  - `Recruiters, referrals, alumni, and hiring managers get buried inside messages.`

Right column heading:

`The orbbt. way`

Right column items:

- Every application has a home
  - `Track jobs, statuses, links, notes, salaries, deadlines, and next steps in one place.`
- Company context is ready
  - `Use AI company research to understand what matters before you apply or interview.`
- Follow-ups stay visible
  - `Deadline reminders help you know what needs attention before momentum fades.`
- Relationships stay organized
  - `Keep contact notes connected to companies and roles because a good resume is not the whole process.`

### 6.9 Pricing Section

Section ID:

`pricing`

Label:

`Pricing`

Heading:

`Free during early access.`

Body:

`Start with the job application tracker now. Pro features will open gradually as the product matures.`

Pricing cards:

#### Early Access

Description:

`For getting your job hunt organized.`

Price:

`$0 / month`

Included:

- Job application tracking
- Basic deadline reminders
- Contacts and notes
- Web access

CTA:

`Try free` -> `auth.html`

#### Planned Pro

Description:

`For active job seekers who need more power.`

Price:

`Soon`

Included:

- Unlimited jobs
- AI company research
- Advanced reminders
- Mobile app and Chrome extension

CTA:

`Go Pro` -> `auth.html`

Note:

- In production, if Pro is not available yet, this CTA can open signup and tag the user as interested in Pro.

#### Campus and Teams

Description:

`For career teams and small groups.`

Price:

`Custom`

Included:

- Shared workspace
- Member insights
- Priority support

CTA:

`Send enquiry` -> `#contact`

### 6.10 Contact Section

Section ID:

`contact`

Label:

`Contact`

Heading:

`Questions, feedback, or problems?`

Body:

`Reach us directly or connect on socials.`

Contact links:

- `hello@orbbt.co` - Contact
- `support@orbbt.co` - Support
- Instagram - `@orbbt`
- LinkedIn - `orbbt.`

Form fields:

- Name
- Email
- Message

CTA:

`Send message`

Production requirement:

- Connect form to backend, CRM, email workflow, or support inbox.
- Add validation and spam protection.
- Show a real success/error state.

### 6.11 Final CTA

Heading:

`Ease your mind. Focus on what matters.`

Body:

`Your job hunt, organized in orbbt.`

CTAs:

- `Try free on web` -> `auth.html`
- `Join mobile app waitlist` -> `waitlist.html`

Alignment:

- Section must be centered.
- Buttons must be centered beneath body text.

### 6.12 FAQ Section

Section ID:

`faq`

Label:

`FAQ`

Heading:

`Frequently asked questions`

Body:

`Clear answers about orbbt., job tracking, mobile access, and getting started.`

FAQ items:

1. What is orbbt.?
   - `orbbt. is a job hunt companion that helps job seekers track applications, research companies with AI, remember deadlines, and manage contacts in one place.`

2. Is orbbt. a job tracker?
   - `Yes. orbbt. is a job application tracker and job hunt organizer for applications, statuses, deadlines, notes, contacts, and follow-ups.`

3. Does orbbt. have a mobile app?
   - `The orbbt. mobile app is planned for iOS and Android. Join the App Store and Play Store waitlist for early access.`

4. How is orbbt. different?
   - `orbbt. focuses on calm job hunt organization: applications, AI company research, deadlines, contacts, and next steps without an overwhelming dashboard.`

Interaction:

- FAQ items are accordions.
- First FAQ can open by default.
- Clicking an FAQ toggles the answer.

### 6.13 Footer

Footer layout:

- Three columns on desktop.
- Stack columns on mobile.
- Columns should align cleanly:
  - Product left.
  - Resources centered on desktop.
  - Connect right on desktop.
  - All left-aligned on mobile.

Product:

- Features -> `#features`
- Pricing -> `#pricing`
- Try it -> `auth.html`

Resources:

- Privacy -> `privacy-policy.html`
- Support -> `mailto:support@orbbt.co`
- Terms -> `terms-and-conditions.html`
- Refunds -> `refund-policy.html`

Connect:

- Instagram
- X (Twitter)
- LinkedIn
- YouTube

Footer bottom:

- orbbt. logo with `by zyntro`
- Copyright 2026 orbbt.

## 7. Visual Design System

### Overall Feel

The site should be minimal, calm, clean, and organized. It should not look crowded. Content should have enough whitespace so the visitor's eyes can settle on one idea at a time.

### Color Palette

Primary brand colors:

- Main violet: `#4D1FE8`
- Mint: `#B9F2CC`
- Pearl: `#FFF6DB`

Core UI colors:

- Background base: `#FBFAF6`
- Paper/card: `#FFFFFF`
- Ink: `#111111`
- Muted text: `#6D6A64`
- Soft text: `#A6A19A`
- Line/border: `#E8E2D8`
- Violet soft: `#F0EBFF`
- Mint soft: `#EFFCF4`

Semantic comparison colors:

- Green: `#168A45`
- Green soft: `#EFFAF1`
- Red: `#BD3F32`
- Red soft: `#FFF0ED`

### Background

The page background uses a soft animated wash, not a plain white background.

Requirements:

- Animated violet/mint/pearl gradient.
- Violet should have more visual space than mint.
- Mint should remain light and secondary.
- Pearl should soften the overall palette.
- Animation should be slow and subtle.
- Must not reduce text readability.

### Typography

Current font stack:

- Primary: Inter
- Utility/labels: Geist Mono
- Instrument Serif is loaded but not essential in the current sample.

Typography direction:

- Standard capitalization, not all lowercase.
- No negative letter spacing.
- Headings should be smaller and calmer than typical AI landing pages.
- Body text should be readable but not dense.
- Hero supporting sentence and benefit labels should remain compact.

### Spacing and Density

The site must avoid feeling claustrophobic.

Rules:

- Use generous vertical section spacing.
- Keep paragraphs short.
- Avoid large blocks of text in cards.
- Do not nest cards inside other cards.
- Use repeated cards only for trust signals, pricing, comparison, and footer groups.

### Cards and Borders

- Border radius should remain minimal or pill-shaped only for buttons/chips.
- Cards should be clean with light borders.
- Avoid heavy shadows.
- Use subtle shadows mainly around product screenshots and hero floating signals.

## 8. Interaction Requirements

### Reveal on Scroll

Sections use a subtle reveal animation:

- Initial: slight downward offset and transparent.
- Visible: opacity 1 and translateY 0.
- Trigger: IntersectionObserver around 12% threshold.

### Mobile Menu

- Hamburger toggles nav panel.
- `aria-expanded` should update.
- Clicking any nav link should close the menu.

### Policies Dropdown

- Desktop: open on hover and focus-within.
- Mobile: show policy links inside the mobile nav panel.

### Feature Tabs

On click:

- Update active state.
- Update `aria-selected`.
- Update feature text and image.

### FAQ Accordion

On click:

- Toggle `.open`.
- Update `aria-expanded`.

### Demo Forms

Current behavior:

- Prevent default submit.
- Show demo message: `Saved for demo. Connect this form to your backend later.`

Production behavior:

- Replace with real submission handling.
- Add loading, success, and error states.
- Validate required fields.
- Add spam protection where needed.

### Hero Floating Banners

Required behavior:

- Banners float subtly.
- Banners glow on hover.
- Banners can be dragged with pointer events.
- Banners should stay where the user drops them during the page session.
- Banners should be hidden on mobile.

## 9. Responsive Requirements

Breakpoints in sample:

- `860px`: tablet/mobile layout changes.
- `560px`: small mobile refinements.

Mobile requirements:

- Hero floating banners hidden.
- Multi-column grids stack into one column.
- Feature tabs become horizontally scrollable.
- Footer columns left-align.
- Top nav collapses to hamburger.
- Policy dropdown remains accessible.
- Pricing cards stack.
- Comparison table stacks.
- Contact section stacks.
- Text must not overlap.
- Buttons must remain tappable.

Potential mobile refinement:

- Hero benefit labels are currently very small. If QA shows they are too small on actual devices, raise mobile-only benefit label size to 11px or 12px.

## 10. SEO and AEO Requirements

### Primary SEO Phrase

`job application tracker`

### Secondary SEO/AEO Phrases

- job hunt organizer
- job search tracker
- job application management
- AI company research
- deadline reminders
- contact management
- job tracking app
- job hunt companion
- application status tracker
- follow-up reminders
- mobile job tracker
- Chrome extension job tracker

### Meta Description

`orbbt. is a calm job application tracker and job hunt organizer with AI company research, deadline reminders, contact notes, and job search tracking across web, mobile, and Chrome extension.`

### AEO Answer Phrases

Use these exact or close-answer phrases in FAQ and structured content:

- `orbbt. is a job hunt companion that helps job seekers track applications, research companies with AI, remember deadlines, and manage contacts in one place.`
- `Yes. orbbt. is a job application tracker and job hunt organizer for applications, statuses, deadlines, notes, contacts, and follow-ups.`
- `The orbbt. mobile app is planned for iOS and Android. Join the App Store and Play Store waitlist for early access.`
- `orbbt. focuses on calm job hunt organization: applications, AI company research, deadlines, contacts, and next steps without an overwhelming dashboard.`

### Recommended Structured Data

Production site should add:

- `Organization` schema for Zyntro/orbbt.
- `SoftwareApplication` schema for orbbt.
- `FAQPage` schema for FAQ section.
- `WebSite` schema for the site.

### Technical SEO

Production site should include:

- Unique title and description per route.
- Canonical URLs.
- Open Graph metadata.
- Twitter card metadata.
- Favicon and app icons.
- Sitemap XML.
- Robots.txt.
- Semantic heading order.
- Descriptive image alt text.

## 11. Accessibility Requirements

Minimum requirements:

- All interactive controls must be keyboard accessible.
- Buttons and links must have visible focus states.
- FAQ buttons should update `aria-expanded`.
- Feature tabs should use `role="tab"` and `aria-selected`.
- Mobile menu should update `aria-expanded`.
- Images need descriptive alt text.
- Text contrast must remain readable over animated backgrounds.
- Forms need labels connected to inputs.
- Avoid text overlap at all responsive widths.
- Motion should remain subtle. Consider `prefers-reduced-motion` in production.

Recommended improvement:

- Add `prefers-reduced-motion` CSS to reduce background, orbit, floating banners, and reveal animations for users who prefer less motion.

## 12. Assets

Current assets:

- `orbbt-logo.png`: primary logo.
- `app-preview.png`: current product screenshot.

Known untracked/draft files in local folder:

- `Frame 37 - Copy.png`
- `Untitled-1.html`
- `logo.png`
- `orbbt-9844ff.html`
- `orbbt-landing-page.zip`
- `output/`
- `tmp/`

Production recommendation:

- Move old drafts or unused files out of the production repository before final deployment.
- Keep only current site files and required assets.
- Use optimized screenshot sizes and modern formats where possible.

## 13. Development Implementation Notes

The current prototype is static HTML/CSS/JS. A production team may rebuild in:

- Plain static HTML/CSS/JS.
- Next.js.
- Astro.
- Vite/React.
- Any equivalent framework.

If rebuilding, preserve:

- Route structure.
- Content hierarchy.
- CTAs and destinations.
- Visual palette.
- Hero animation direction.
- Feature tab behavior.
- FAQ accordion behavior.
- Mobile responsiveness.

Recommended component breakdown:

- `Header`
- `PolicyDropdown`
- `Hero`
- `HeroOrbit`
- `FloatingHeroSignals`
- `ProductPreview`
- `TrustStrip`
- `ProblemSection`
- `StorySection`
- `FeatureTabs`
- `HowItWorks`
- `BeforeAfterComparison`
- `PricingCards`
- `ContactSection`
- `FinalCTA`
- `FAQAccordion`
- `Footer`
- `AuthPage`
- `WaitlistPage`
- `PolicyPage`

## 14. Backend and Integrations

### Authentication

Current auth page is demo-only.

Production needs:

- Sign up.
- Log in.
- Password handling or OAuth.
- Session management.
- Error states.
- Email verification if required.

### Waitlist

Current waitlist form is demo-only.

Production needs:

- Store waitlist entries.
- Capture platform interest if needed: iOS, Android, both.
- Send confirmation email if desired.
- Track source page and campaign.

### Contact Form

Production needs:

- Route contact messages to support or CRM.
- Basic spam protection.
- Confirmation message.
- Error handling.

### Analytics

Recommended events:

- Hero Try free click.
- Hero mobile waitlist click.
- Top nav sign up click.
- Pricing Try free click.
- Pricing Go Pro click.
- Pricing Send enquiry click.
- Waitlist form submit.
- Contact form submit.
- Feature tab click.
- FAQ open.

## 15. QA Checklist

Desktop QA:

- Hero text centered and readable.
- Floating banners do not overlap main hero copy by default.
- Floating banners drag and stay in place.
- Product screenshot loads.
- Feature tabs update content.
- Pricing CTAs work.
- Contact form aligns.
- Final CTA is centered.
- Footer columns align properly.
- Policy dropdown opens on hover/focus.

Mobile QA:

- Hamburger menu opens and closes.
- Policy links accessible.
- Hero floating banners hidden.
- Hero text does not overlap.
- Benefit labels remain readable.
- Product screenshot scales.
- Feature tabs scroll horizontally if needed.
- Pricing cards stack.
- Comparison columns stack.
- Contact section stacks.
- Footer stacks and left-aligns.

Accessibility QA:

- Tab through all links/buttons.
- Focus states visible.
- Accordions update `aria-expanded`.
- Feature tabs update `aria-selected`.
- Images have alt text.
- Form fields are labeled.

Performance QA:

- Optimize screenshots.
- Avoid blocking JavaScript.
- Keep animations CSS-based where possible.
- Avoid heavy decorative assets.

SEO QA:

- Page titles and descriptions present.
- Semantic headings.
- FAQ content indexable.
- Sitemap and robots added in production.
- Structured data added in production.

## 16. Acceptance Criteria

The implementation is acceptable when:

- The site communicates orbbt. as a calm job application tracker within five seconds.
- The hero, product preview, features, pricing, FAQ, and footer match the sample site's content intent.
- All routes are reachable.
- CTAs route correctly.
- Forms show functional production behavior or clearly defined demo states.
- Desktop and mobile layouts have no overlapping text.
- Animations are subtle and do not reduce usability.
- SEO/AEO phrases are naturally present.
- Accessibility basics are met.

## 17. Open Decisions for Product Team

The dev team should confirm:

- Final production domain.
- Real contact/support email addresses.
- Final social profile URLs.
- Whether Pro should be selectable before launch or waitlist-only.
- Whether Campus and Teams should route to email, contact form, or a separate enquiry page.
- Authentication provider.
- Waitlist storage provider.
- Analytics provider.
- Final product screenshots for each feature tab.
- Whether testimonials/reviews should be added later.

## 18. Current Deployment

Current sample deployment:

`https://danish-shah-cyber.github.io/orbbt-landing-page/`

Current source repository:

`https://github.com/Danish-Shah-Cyber/orbbt-landing-page`

Production deployment can use GitHub Pages, Netlify, Vercel, Cloudflare Pages, or another static hosting provider.
