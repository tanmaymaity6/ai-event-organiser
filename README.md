# 🎉 AI Event Organiser  
A full-stack event creation and discovery platform built with **Next.js**, **Convex**, **Clerk Auth**, **Shadcn UI**, **Tailwind**, and **Gemini AI**.

Create, manage, explore, and register for events with ease — powered by AI-assisted event generation.

---

## 🚀 Features

### 🔐 Authentication & User Management
- Secure authentication using **Clerk**
- Social login support (Google, GitHub, etc.)
- Automatic user sync into **Convex DB**
- Tracks:
  - Onboarding completion
  - Free vs Pro usage limits
  - Event creation history

---

### 🧭 Modern UI & UX
- Responsive design using **TailwindCSS**
- Styled with **Shadcn UI**
- Beautiful Mobbin-style layout
- Smooth onboarding flow
- Elegant theme-color based pages

---

### 🧠 AI-Powered Event Creator
- Generate event title, description, capacity, and ticket type using **Gemini AI**
- One-click auto-fill in Create Event page
- Reduces manual typing and improves quality

---

### 📍 Location-Aware Search
- Country → State → City based filtering
- Powered by `country-state-city` package
- Instant event search on Explore page

---

### 📸 Media & Customization
- Pick banners using **Unsplash API**
- Custom theme color selection
  - Free users → only default color  
  - Pro users → unlock all colors
- Rich event descriptions

---

### 🎫 Event Tickets & Registration
- Support for Free & Paid tickets
- Ticket capacity limits
- Auto confirmation
- QR code generation
- Organisers can check-in attendees at the venue

---

### 🧾 Event Dashboard
- Track registrations
- Viewer analytics
- QR-based attendee check-in
- Organiser-only management tools

---

### 👤 User Subscription (Free / Pro)
- Free users can create **1 event**
- Pro users can:
  - Create unlimited events
  - Use all t


ai-event-organiser/
│── app/
│── components/
│── convex/
│── hooks/
│── lib/
│── public/
│── .env.local
│── convex.json
│── package.json
│── README.md



---

## 🔧 Setup Instructions

### 1️⃣ Clone the repo
```bash
git clone https://github.com/tanmaymaity6/ai-event-organiser
cd ai-event-organiser

Install dependencies
npm install

Create .env.local

# Convex Deployment (created when you run `npx convex dev`)
CONVEX_DEPLOYMENT=

NEXT_PUBLIC_CONVEX_URL=

# Clerk Auth
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
CLERK_JWT_ISSUER_DOMAIN=

# Unsplash API
NEXT_PUBLIC_UNSPLASH_ACCESS_KEY=

# Gemini AI
GEMINI_API_KEY=
