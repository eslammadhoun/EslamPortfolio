# Portfolio Brief: Eslam R. Madhoun — Flutter Developer
# FOR CLAUDE CODE: Read this entire file before writing a single line of code.

---

## WHO YOU ARE BUILDING FOR

**Name:** Eslam R. Madhoun  
**Role:** Flutter Developer  
**Email:** eslammadhoun3@gmail.com  
**GitHub:** https://github.com/eslammadhoun  
**LinkedIn:** https://linkedin.com/in/eslam-madhoun-68210b355  
**Location:** Gaza, Palestine  
**Status:** Computer Science student at Al-Azhar University, Gaza. Started 2024.  
**Available for:** Remote freelance projects and full-time Flutter roles.

---

## THE GOAL

Build a **fully custom, professional Flutter developer portfolio website** as a single HTML file
(HTML + CSS + JS all in one file). It must:

- Look like it was designed by a senior Flutter developer, not generated from a template.
- Be visually distinctive — dark theme, technical aesthetic, clean and modern.
- Tell Eslam's story honestly: a self-taught developer from Gaza who learned production-level
  Flutter in under a year and built real, technically deep applications.
- Work perfectly on desktop and mobile (fully responsive).
- Have smooth scroll animations (subtle, not overdone).
- Be ready to deploy to GitHub Pages directly.

---

## DESIGN DIRECTION

**Aesthetic:** Dark, technical, precise. Like a senior developer's portfolio crossed with a
well-designed developer tool landing page. NOT a generic Tailwind template. NOT warm/cream
with serif fonts. This is a Flutter developer — the UI itself should demonstrate taste.

**Color Palette:**
- Background: #0D0F14 (near-black, not pure black)
- Surface/Cards: #151921
- Border: #1E2530
- Primary Accent: #5C6BC0 (indigo-blue — the Flutter brand color family)
- Accent Glow: #7986CB (lighter indigo for hover states)
- Text Primary: #E8EAF0
- Text Secondary: #8892A4
- Success/Highlight: #4CAF50 (used sparingly)
- Code accent: #64FFDA (mint — used only for inline code references)

**Typography:**
- Display/Headings: "Space Grotesk" (Google Fonts) — modern, technical, distinctive
- Body: "Inter" (Google Fonts) — clean and readable
- Code/Mono: "JetBrains Mono" (Google Fonts) — for code snippets and tech terms

**Signature element:** A subtle animated Flutter logo or widget tree diagram in the hero
section — something that immediately signals "Flutter developer" without being cheesy.
Use CSS/SVG animation, not a GIF.

**Layout:** Single-page, sections separated by generous whitespace. Sticky nav. Smooth
scroll. Cards with subtle border glow on hover.

---

## SECTIONS (IN ORDER)

### 1. NAV
- Logo: "EM" monogram, styled
- Links: About, Skills, Projects, Experience, Contact
- Sticky on scroll, slight blur background effect
- GitHub and LinkedIn icon links in the nav

---

### 2. HERO SECTION

**Headline (large, display font):**
"Flutter Developer."

**Sub-headline:**
"I build production-ready cross-platform apps with clean architecture,
BLoC state management, and obsessive attention to detail."

**Supporting line:**
"Based in Gaza, Palestine. Open to remote roles worldwide."

**CTAs:**
- Primary button: "View My Work" → scrolls to Projects
- Secondary button: "Get In Touch" → scrolls to Contact

**Visual element:**
An animated code snippet or abstract Flutter widget tree diagram using CSS/SVG.
Something like a simplified visual of:
```
MaterialApp
  └── Scaffold
        ├── AppBar
        └── BlocBuilder
              └── ListView
```
Rendered as a glowing, subtle animated diagram in the background or to the right.

---

### 3. ABOUT SECTION

**Section label:** "About"
**Headline:** "From Gaza to Global-Ready Flutter Dev"

**Story (write exactly this, in a warm but professional tone):**

I'm a Flutter developer based in Gaza, Palestine, currently studying Software Engineering
at Al-Azhar University. In less than a year, I've gone from learning Dart fundamentals
to building production-level applications with Clean Architecture, BLoC/Cubit state
management, Firebase, REST APIs, and Stripe payments.

I trained through the Flutter Development Program at Gaza Sky Geeks, where I focused
on Dart fundamentals, Flutter UI, and state management. What I built afterward wasn't
tutorial projects — it was apps with real architecture decisions: feature-first folder
structures, Freezed sealed state unions, dual data source separation (REST + Firestore),
and documented performance optimizations.

I care deeply about the quality of what I ship. Not just whether it works, but whether
it's maintainable, testable, and understandable to another developer six months later.

**Quick stats (displayed as cards/grid):**
- "< 1 year" → "To production-level Flutter"
- "3+" → "Shipped Projects"
- "9 Sections" → "Formally assessed across 52+ interview questions"
- "Clean Architecture" → "Every project, no exceptions"

---

### 4. SKILLS SECTION

**Section label:** "Technical Skills"
**Headline:** "What I Work With"

Display skills in logical groups, NOT a flat tag cloud:

**Flutter & Dart**
Flutter, Dart 3.x, Flutter Web, Responsive UI, flutter_screenutil, flutter_native_splash

**State Management**
BLoC / Cubit, Freezed (sealed states), Provider (familiar)

**Architecture**
Clean Architecture, Feature-First Structure, SOLID Principles, MVVM, Repository Pattern

**Networking & APIs**
Retrofit + Dio, RESTful APIs, JWT Authentication, Interceptors, Token Refresh, Error Handling

**Backend & Services**
Firebase (Firestore, Auth, Cloud Functions), Stripe Payment Gateway, Google Maps

**Code Quality & DX**
GetIt (Dependency Injection), json_serializable, build_runner, flutter_secure_storage,
easy_localization, pretty_dio_logger

**Tools & Workflow**
Git / GitHub, GitHub Actions (CI), Android Studio, VS Code, Figma (design handoff),
Multi-flavor builds (dev/prod)

**Currently Learning**
Riverpod, GoRouter, Flutter Desktop, Unit & Widget Testing

---

### 5. PROJECTS SECTION

**Section label:** "Selected Work"
**Headline:** "Projects Built for Real Problems"

Display 3 project cards. Each card has: project image placeholder (or icon), title,
category tag, description, tech stack pills, and links.

---

#### PROJECT 1: Doc-doc — Medical Appointment Booking App
**Category tag:** Healthcare · Production-Ready
**GitHub:** https://github.com/eslammadhoun/Doc-doc
**Status badge:** "Most Complex Project"

**Description (write exactly this):**
A full-featured medical app connecting patients with doctors across 15+ specializations.
Patients can browse by specialty, search and filter doctors, view detailed profiles with
reviews, book appointments with real-time slot selection, and communicate via a real-time
Firebase Firestore chat inbox.

**What makes it technically serious:**
- Dual data architecture: REST API (via Retrofit + Dio) for medical data, Firebase
  Firestore for real-time messaging — cleanly separated through the repository pattern
- BLoC/Cubit with Freezed sealed state unions on every screen that fetches data
- Multi-flavor builds: separate dev and prod entry points with independent configurations
- Performance: RepaintBoundary on list items, BlocSelector scoping, memCacheWidth on
  cached images, ListView.builder everywhere, debounced search
- Secure JWT storage via flutter_secure_storage, never plain SharedPreferences
- Feature-first Clean Architecture with full layer separation (Presentation/Domain/Data/Core)

**Full tech stack:**
Flutter/Dart 3.x · BLoC/Cubit · Freezed · Retrofit + Dio · Firebase Firestore · GetIt ·
json_serializable · flutter_secure_storage · flutter_screenutil · easy_localization ·
GitHub Actions (CI) · Multi-flavor builds

**Honest trade-offs (show this — it signals maturity):**
"Chat messages use static sample data at the conversation level — Firestore message read/write
is wired but not complete. Three bottom nav tabs are placeholder screens. Test coverage is
minimal, though the architecture supports it through DI and repository abstraction."

---

#### PROJECT 2: Shopy — E-Commerce App with Maps & Payments
**Category tag:** E-Commerce · Full Stack
**GitHub:** https://github.com/eslammadhoun (link to the repo if available)

**Description:**
A complete e-commerce mobile application built to demonstrate the full purchase flow:
product browsing, cart management, Stripe payment integration, and Google Maps order
tracking. Built with Clean Architecture and Cubit state management.

**Technical highlights:**
- Stripe Payment Gateway integration with full checkout flow
- Google Maps for real-time order tracking
- Cubit state management with Clean Architecture
- Secure local data persistence

**Tech stack:**
Flutter · Cubit · Stripe · Google Maps · Clean Architecture · Firebase

---

#### PROJECT 3: Nectar-Groceries — Grocery Shopping App
**Category tag:** E-Commerce · Firebase
**GitHub:** https://github.com/eslammadhoun/Nectar-Groceries

**Description:**
A full-featured grocery shopping app built with Flutter and Firebase. Features real-time
product browsing, cart management, favorites, and location-based delivery. Built as a deep
dive into Firebase-first architecture.

**Tech stack:**
Flutter · Firebase · Firestore · Authentication · Location Services

---

### 6. EXPERIENCE / TIMELINE SECTION

**Section label:** "Journey"
**Headline:** "How I Got Here"

Display as a vertical timeline (not numbered — it's a real chronological journey):

**2024 — Started Software Engineering at Al-Azhar University, Gaza**
"Began my formal computer science education while simultaneously learning Flutter
independently — because I couldn't wait."

**Early 2025 — Gaza Sky Geeks Flutter Development Program**
"Completed an intensive Flutter training program focused on Dart fundamentals, Flutter UI
architecture, and state management. This was where I went from learning Flutter to
understanding it."

**2025 — First Production Role: Junior Flutter Developer**
"Joined as a Junior Flutter Developer. Responsible for implementing pixel-perfect
responsive UIs from Figma designs, applying SOLID Principles and Clean Architecture
from day one."

**2025 — Backend Integration Milestone**
"Integrated Firebase services (Firestore, Auth, Cloud Functions) and Stripe Payment
Gateway into production applications. First real experience with dual data source
architecture."

**2025 — Built Doc-doc (Flagship Project)**
"Built my most technically ambitious project: a medical appointment booking app with
real-time Firebase chat, multi-flavor builds, performance-optimized lists, and
dual-source architecture. The README documents the engineering decisions in full."

---

### 7. INTERVIEW SKILLS SECTION (IMPORTANT — THIS IS UNIQUE)

**Section label:** "Verified Skills"
**Headline:** "Assessed, Not Just Listed"

**Intro text:**
"Most developers list skills. I've had mine assessed through a comprehensive Flutter
developer evaluation — 9 sections, 52+ questions, covering exactly what interviewers
ask for mid-to-senior Flutter roles. Here's how I performed:"

Display as a GRID of skill cards (2 columns on desktop, 1 on mobile).
Each card shows: section name, level label, and a one-line description.
Use a visual indicator (colored dot or thin bar) — green for Expert/Senior, yellow for
actively improving. NO specific numeric scores.

**Card 1 — State Management (BLoC/Cubit)**
Level: "Expert"
Color: green
Description: "Sealed state unions with Freezed, BlocSelector scoping, BlocProvider
context rules, and every edge case that trips up mid-level developers."

**Card 2 — Architecture (Clean Architecture)**
Level: "Expert"
Color: green
Description: "Feature-first folder structure, SOLID principles, Repository pattern,
dependency injection with GetIt — applied in every project I build, not just described."

**Card 3 — Deployment & CI/CD**
Level: "Expert"
Color: green
Description: "APK vs AAB, app signing, Play Store publishing, GitHub Actions pipelines,
Firebase App Distribution, and staged rollouts. I've set this up in real projects."

**Card 4 — Networking & APIs**
Level: "Senior"
Color: green
Description: "Retrofit + Dio, interceptors, JWT token refresh flows, unified error
handling with ApiResult<T>, pagination, REST vs WebSocket — implemented in production."

**Card 5 — Performance Optimization**
Level: "Senior"
Color: green
Description: "RepaintBoundary, BlocSelector scoping, ListView.builder, memCacheWidth,
const constructors, and debounced inputs — I apply these by default, not as afterthoughts."

**Card 6 — Firebase**
Level: "Senior"
Color: green
Description: "Auth, Firestore (real-time streams), Cloud Functions, Security Rules,
Firebase App Distribution. I've integrated both Firebase and REST in the same app."

**Card 7 — Local Storage**
Level: "Senior"
Color: green
Description: "SharedPreferences for UI state, flutter_secure_storage for tokens,
SQLite/Drift for structured data — I know what to store where and why."

**Card 8 — Flutter Fundamentals**
Level: "Actively Sharpening"
Color: yellow
Description: "Strong on Widget/Element/Render trees and const optimization. Drilling
Keys and StatefulWidget lifecycle before interviews — I'd rather flag this than have
it surprise you in a technical screen."

**Section summary line (below the grid):**
"Overall assessment across all 9 sections: strong mid-to-senior level with exceptional
depth in architecture, state management, deployment, and performance optimization."

**Honest note (smaller text below):**
"Flutter Fundamentals is the one area I'm actively improving. Everything else I can
defend line by line in a technical interview."

**Why this section matters:** Almost no junior/mid developer puts this on their portfolio.
It signals honesty, self-awareness, and a commitment to real skill over fake confidence.
This is what makes a recruiter stop and read.

---

### 8. CONTACT SECTION

**Section label:** "Contact"
**Headline:** "Let's Build Something"

**Body text:**
"I'm currently open to remote Flutter roles and freelance projects. If you're looking for
a Flutter developer who writes clean code, thinks architecturally, and ships real apps —
let's talk."

**Contact methods:**
- Email: eslammadhoun3@gmail.com (large, clickable mailto link)
- GitHub: github.com/eslammadhoun
- LinkedIn: linkedin.com/in/eslam-madhoun-68210b355

**Availability note:**
"Available immediately. Time zone: GMT+3 (Gaza). Comfortable working async."

---

### 9. FOOTER

"Built with HTML, CSS, and JavaScript. © 2026 Eslam R. Madhoun."
Small note: "Designed to be as clean as the code inside my projects."

---

## TECHNICAL REQUIREMENTS FOR CLAUDE CODE

1. **Single HTML file** — all CSS and JS embedded. No external files except Google Fonts CDN.
2. **Google Fonts** — import Space Grotesk, Inter, JetBrains Mono from fonts.googleapis.com
3. **No frameworks** — pure HTML/CSS/JS only. No React, no Vue, no Tailwind.
4. **Animations:**
   - Hero section: subtle fade-in on load
   - Scroll-triggered: sections fade/slide in as they enter viewport (IntersectionObserver)
   - Hover: card border glow, button color transitions
   - Skill bars: animate width on scroll into view
   - Score rings in the interview section: animate stroke-dashoffset on scroll into view
5. **Responsive:** Works on mobile (320px+), tablet, and desktop. Mobile-first CSS.
6. **Sticky nav** with backdrop-filter blur on scroll
7. **Smooth scroll** for all anchor links
8. **Active nav link** highlights as user scrolls through sections
9. **No Lorem Ipsum** — use ALL the real content from this brief exactly as written
10. **Performance:** No unnecessary JS. CSS variables for all colors. Clean, commented code.
11. **Deploy-ready:** Can be saved as index.html and pushed to GitHub Pages immediately.

---

## TONE GUIDANCE

- Professional but human. Not corporate.
- Honest about limitations (the interview scores section proves this).
- Confident about strengths without overclaiming.
- Gaza context is part of the story — don't hide it, don't over-emphasize it.
  It's mentioned once in the About section, naturally.
- This portfolio should feel like it was written by a developer who knows exactly
  what they're doing, is honest about where they're still growing, and respects
  the recruiter's time.

---

## WHAT TO AVOID

- Do NOT use a light/cream background. Dark theme only.
- Do NOT use generic phrases like "passionate developer" or "love to code."
- Do NOT use numbered section markers (01, 02, 03) — they look template-generated.
- Do NOT make the hero a fullscreen image with text overlay.
- Do NOT use emoji in the portfolio itself (only in this brief for readability).
- Do NOT add a "Download CV" button unless you create the CV too.
- Do NOT use Bootstrap or any CSS framework.
- Do NOT make the interview scores section look like an infographic from 2018.
  Use clean, modern CSS rings or horizontal bars with labels.

---

## START HERE

Read this entire brief. Then build the complete index.html file.
Do not ask for clarification — all the content and direction is here.
Build it in full, top to bottom, production-ready.
