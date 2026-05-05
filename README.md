<div align="center">

# 🚀 Sarvya Career OS

**The all-in-one engineering career platform for Indian students**

[![Next.js](https://img.shields.io/badge/Next.js-16-black?logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.7-blue?logo=typescript)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.4-38bdf8?logo=tailwindcss)](https://tailwindcss.com/)
[![Supabase](https://img.shields.io/badge/Supabase-Database-3ecf8e?logo=supabase)](https://supabase.com/)
[![Clerk](https://img.shields.io/badge/Clerk-Auth-6c47ff?logo=clerk)](https://clerk.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

[Live Demo](#) · [Report Bug](https://github.com/Sreejith-nair511/Sarvya-carrer/issues) · [Request Feature](https://github.com/Sreejith-nair511/Sarvya-carrer/issues)

</div>

---

## 📖 About

**Sarvya Career OS** is a comprehensive career platform built specifically for Indian engineering students aiming to land roles at top tech companies. It combines expert-led courses, AI-powered guidance, adaptive quizzes, learning analytics, and an ATS-optimized resume builder — all in one place.

> Built with the modern web stack: Next.js 16, TypeScript, Supabase, Clerk, and Groq AI.

---

## ✨ Features

### 🎓 Learning Platform
- **200+ Expert Courses** — Industry-aligned content curated by engineers from top tech companies
- **Structured Learning Paths** — Guided roadmaps from beginner to job-ready
- **Course Progress Tracking** — Resume where you left off, track completion per lesson
- **My Courses Dashboard** — Manage all enrolled courses in one view

### 🤖 AI-Powered Tools
- **AI Career Assistant** — Streaming chat interface powered by Groq (Llama 3.3 70B), acting as your personal engineering career coach
- **Adaptive Quiz Engine** — AI-generated quizzes that adjust difficulty based on your performance
- **AI Resume Analyzer** — Get structured ATS feedback and keyword suggestions on your resume

### 📊 Analytics & Insights
- **Learning Analytics** — Visual dashboards showing streaks, skill progress, and time spent
- **Learning Profile** — Personalized profile tracking your strengths and growth areas
- **Achievement System** — Badges and milestones to keep you motivated

### 📝 Resume Builder
- **ATS-Optimized Templates** — Professionally designed resume layouts
- **Real-Time Preview** — See changes instantly as you type
- **AI Feedback Integration** — One-click AI analysis with actionable improvement suggestions
- **Export Ready** — Download your resume in a clean, recruiter-friendly format

### 🎨 Premium UI/UX
- **5 Accent Color Themes** — Classic Blue, Royal Indigo, Ethereal Violet, Deep Rose, Vibrant Emerald
- **Dark / Light Mode** — Full theme support with smooth transitions
- **Glassmorphism Effects** — Adjustable intensity (Low / Medium / High)
- **Motion Controls** — Full, Subtle, or No animations — your choice
- **Fully Responsive** — Optimized for mobile and desktop

### 🔐 Authentication & Security
- **Clerk Auth** — Secure sign-in / sign-up with social login support
- **Protected Routes** — Middleware-based route protection
- **Role-based Access** — Dashboard and course content gated behind auth

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Framework** | [Next.js 16](https://nextjs.org/) (App Router) |
| **Language** | [TypeScript 5.7](https://www.typescriptlang.org/) |
| **Styling** | [Tailwind CSS 3.4](https://tailwindcss.com/) |
| **UI Components** | [shadcn/ui](https://ui.shadcn.com/) (Radix UI primitives) |
| **Database** | [Supabase](https://supabase.com/) (PostgreSQL) |
| **Authentication** | [Clerk](https://clerk.com/) |
| **AI / LLM** | [Groq SDK](https://console.groq.com/) — Llama 3.3 70B |
| **Charts** | [Recharts](https://recharts.org/) |
| **Icons** | [Lucide React](https://lucide.dev/) |
| **Forms** | [React Hook Form](https://react-hook-form.com/) + [Zod](https://zod.dev/) |
| **Package Manager** | [pnpm](https://pnpm.io/) |

---

## 📁 Project Structure

```
├── app/
│   ├── page.tsx                  # Landing page
│   ├── dashboard/                # Main user dashboard
│   ├── courses/                  # Course listing & detail pages
│   │   └── [id]/lesson/[lessonId]/ # Individual lesson viewer
│   ├── learning/
│   │   ├── path/                 # Learning path page
│   │   ├── quiz/                 # Adaptive quiz
│   │   └── analytics/            # Learning analytics
│   ├── ai-assistant/             # AI career chat
│   ├── resume-builder/           # Resume builder tool
│   ├── roadmaps/                 # Career roadmaps
│   ├── hackathons/               # Hackathon listings
│   ├── jobs/                     # Job board
│   ├── settings/                 # User settings & appearance
│   └── api/                      # API routes (chat, quiz, analytics, etc.)
├── components/
│   ├── dashboard/                # Dashboard-specific components
│   ├── landing/                  # Landing page sections
│   └── ui/                       # shadcn/ui component library (50+ components)
├── lib/
│   ├── actions/                  # Server actions
│   ├── supabase.ts               # Supabase client
│   ├── supabase-server.ts        # Supabase server client
│   └── utils.ts                  # Utility functions
├── hooks/                        # Custom React hooks
├── scripts/                      # Database seeding scripts
└── supabase_migration_*.sql      # Database migration files
```

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** — Latest LTS version
- **pnpm** — `npm install -g pnpm`
- **Supabase** account — [supabase.com](https://supabase.com)
- **Clerk** account — [clerk.com](https://clerk.com)
- **Groq** API key — [console.groq.com](https://console.groq.com)

### 1. Clone the repository

```bash
git clone https://github.com/Sreejith-nair511/Sarvya-carrer.git
cd Sarvya-carrer
```

### 2. Install dependencies

```bash
pnpm install
```

### 3. Set up environment variables

Copy the example env file and fill in your keys:

```bash
cp .env.example .env.local
```

```env
# Supabase
NEXT_PUBLIC_SUPABASE_URL=your_supabase_project_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_supabase_service_role_key

# Clerk
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/dashboard
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/dashboard

# AI
GROQ_API_KEY=your_groq_api_key

# Optional
YOUTUBE_API_KEY=your_youtube_api_key
```

### 4. Set up the database

Run the SQL migrations in your Supabase SQL Editor in this order:

```
supabase_migration_courses.sql   → Creates the courses table
supabase_migration_v2.sql        → Adds enrollments, progress, indexes
supabase_migration_ai_learning.sql → AI learning features schema
```

### 5. Run the development server

```bash
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### 6. Seed initial data (optional)

After signing in, visit:
```
http://localhost:3000/api/populate-courses
```

---

## 🌐 Deployment

The recommended deployment stack is **Vercel + Supabase + Clerk**.

See [DEPLOYMENT.md](DEPLOYMENT.md) for the full step-by-step guide including:
- Supabase project setup and migrations
- Clerk configuration and redirect URLs
- Vercel environment variable setup
- Post-deployment data seeding

---

## 📸 Screenshots

| Landing Page | Dashboard | AI Assistant |
|---|---|---|
| ![Landing](https://via.placeholder.com/300x200?text=Landing+Page) | ![Dashboard](https://via.placeholder.com/300x200?text=Dashboard) | ![AI Chat](https://via.placeholder.com/300x200?text=AI+Assistant) |

| Course View | Resume Builder | Learning Analytics |
|---|---|---|
| ![Courses](https://via.placeholder.com/300x200?text=Courses) | ![Resume](https://via.placeholder.com/300x200?text=Resume+Builder) | ![Analytics](https://via.placeholder.com/300x200?text=Analytics) |

---

## 🗺️ Roadmap

- [ ] Mobile app (React Native)
- [ ] Live coding interview practice
- [ ] Peer-to-peer mentorship matching
- [ ] Company-specific interview prep tracks
- [ ] Community forums and discussion boards
- [ ] Offline course downloads

---

## 🤝 Contributing

Contributions are welcome! Here's how to get started:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m 'feat: add your feature'`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Open a Pull Request

Please follow [Conventional Commits](https://www.conventionalcommits.org/) for commit messages.

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Sreejith Nair**
- GitHub: [@Sreejith-nair511](https://github.com/Sreejith-nair511)

---

<div align="center">
  <p>Built with ❤️ for Indian engineering students</p>
  <p>⭐ Star this repo if you find it helpful!</p>
</div>
