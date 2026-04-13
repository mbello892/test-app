# Test-app

## What This Project Is
This project is a SaaS application for hotel reservations. It will allow users to search for available hotel rooms, view detailed information about each property, and book their stays.

## Stack

| Layer | Technology | Reason |
| --- | --- | --- |
| Frontend | Next.js + TypeScript | Provides a robust and maintainable frontend with server-side rendering capabilities. TypeScript enhances code quality and developer productivity. |
| Styling | Tailwind CSS + shadcn/ui | Tailwind CSS is a utility-first CSS framework that enables efficient and customizable styling. The shadcn/ui library provides a set of high-quality, accessible UI components. |
| Build | Next.js (built-in) | Next.js's built-in build process is fast and lightweight, ensuring a smooth development experience. |
| Database | Supabase (PostgreSQL) | Supabase provides a scalable PostgreSQL database with a simple API, reducing backend complexity. |
| Auth | Supabase Auth | Supabase's built-in authentication system simplifies the implementation of user authentication. |
| Deployment | Vercel | Vercel offers seamless deployment and reliable performance for hosting the application. |

## First Time Setup
1. Check if `.env.local` exists. If not, copy from `.env.example`.
2. Fill in the required environment variables:
   - `NEXT_PUBLIC_SUPABASE_URL`: Get this from your Supabase project dashboard.
   - `NEXT_PUBLIC_SUPABASE_ANON_KEY`: Get this from your Supabase project dashboard.
3. Run `pnpm install`.
4. Run `pnpm dev`.
5. Verify the app loads at `localhost:3000`.

## Before You Start Coding
- **Ask the user what they want to build first. Don't assume.**
- If the user's description is vague, ask clarifying questions about: target audience, key features, design style, and priority.
- Always verify environment variables are configured before attempting to run or build the application.

## Project Structure
- `pages/`: Next.js pages and routes
- `components/`: Reusable UI components
- `lib/`: Utility functions, API clients, and other shared logic
- `styles/`: Global styles and Tailwind CSS configuration
- `types/`: TypeScript type definitions
- `public/`: Static assets like images and fonts

## Key Conventions
- TypeScript strict mode, no `any`
- All database queries through Supabase client
- Server components by default, 'use client' only when needed
- Mobile-first responsive design

## Common Commands
```bash
pnpm dev          # Start development server
pnpm build        # Production build
pnpm lint         # Run linter
```

## What NOT To Do
- Don't skip environment variable setup
- Don't use `any` in TypeScript
- Don't commit `.env.local`
- Don't modify files in `node_modules`
- Don't install packages without asking the user first
## Recommended Skills

Install these Claude Code skills for AI-assisted development:

```bash
npx skills add vercel-labs/agent-skills@vercel-react-best-practices -g -y  # React and Next.js patterns from Vercel Engineering
npx skills add tenequm/claude-plugins@shadcn-tailwind -g -y  # Tailwind CSS and shadcn/ui component patterns
npx skills add anthropics/skills@supabase -g -y  # Supabase best practices: RLS, auth, real-time
npx skills add binjuhor/shadcn-lar@frontend-design-pro -g -y  # Professional UI/UX design patterns
npx skills add anthropics/skills@testing-patterns -g -y  # Test writing patterns for frontend and backend
```

- **React Best Practices**: React and Next.js patterns from Vercel Engineering — Your project uses React/Next.js
- **Tailwind + shadcn/ui**: Tailwind CSS and shadcn/ui component patterns — Your project uses Tailwind + shadcn
- **Supabase Patterns**: Supabase best practices: RLS, auth, real-time — Your project uses Supabase
- **Frontend Design Pro**: Professional UI/UX design patterns — Helps create polished, professional interfaces
- **Testing Patterns**: Test writing patterns for frontend and backend — Every production app needs tests
