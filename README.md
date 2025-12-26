# AI Chat Application

A production-ready, mobile-first AI chat application built with modern web technologies.  
This project started as a **case study** and is actively evolving into a **personal product**.

## 🔎 Overview

This application demonstrates how to build a polished AI-powered chat experience with:

- Real-time **streaming AI responses**
- Persistent chat history
- Multiple AI characters with distinct personalities
- Clean architecture and modern UI/UX patterns

The focus of this project is not only functionality, but also **code quality, scalability, and user experience**.

## ⚙️ Core Features

- Google Sign-In authentication (OAuth)
- Session persistence
- Multiple predefined AI characters
- Streaming chat responses (typewriter-style)
- Persistent chat history (database-backed)
- Switch between chat sessions
- Fully responsive UI
- Smooth animations and transitions
- Dark / Light mode support
- Markdown rendering for AI responses

## 🧰 Tech Stack

### Frontend
- ![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)
- ![Next.js](https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white)
- ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
- ![Tailwind](https://img.shields.io/badge/TailwindCSS-06B6D4?logo=tailwindcss&logoColor=white)
- ![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-000000?logo=vercel&logoColor=white)
- ![Framer Motion](https://img.shields.io/badge/Framer%20Motion-0055FF?logo=framer&logoColor=white)

### Backend & Services
- ![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?logo=supabase&logoColor=white)
- ![OpenRouter](https://img.shields.io/badge/OpenRouter-AI%20API-blueviolet)
- ![Google OAuth](https://img.shields.io/badge/Google%20OAuth-4285F4?logo=google&logoColor=white)

### Content & UX
- **react-markdown** ![react-markdown]
- **next-themes** ![next-themes]

## 📐 Architecture Overview

The project follows a clean and scalable architecture:

- `app/`  
  Contains routing, layouts, and page-level components using Next.js App Router.

- `src/features/`  
  Business logic grouped by domain:
  - authentication
  - chat
  - characters

- `src/components/`  
  Reusable UI components and layouts.

- `src/lib/`  
  External services and integrations:
  - Supabase client
  - OpenRouter client
  - Environment validation

- `src/hooks/`  
  Custom React hooks (streaming, auto-scroll, etc.).

This separation keeps UI, business logic, and infrastructure concerns isolated.

## 🎭 AI Characters

The application includes predefined AI characters.  
Each character has:

- A unique avatar
- A display name
- A dedicated system prompt

Characters are defined in a single configuration file, making them easy to extend or modify.

## 🔐 Authentication

- Google Sign-In via Supabase OAuth
- Secure session persistence
- Server-side session handling for protected routes

## 💬 Chat System

- Messages stream in real time from the AI (no full-response blocking)
- Messages are saved to the database as they arrive
- Conversations persist across page reloads
- Smooth auto-scroll behavior during streaming

## 🌗 Theme Support

- Dark and Light mode support
- Theme preference stored on the client
- Fully compatible with Tailwind and shadcn/ui

## 📦 Environment Variables

Create a `.env.local` file based on `.env.example`.

Example:

```env
NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=

OPENROUTER_API_KEY=
OPENROUTER_MODEL=
```

.env.local is intentionally ignored by Git and should never be committed.

## 🚀 Getting Started

Install dependencies

```
npm install
```

Run development server
```
npm dev
```

Open:
http://localhost:3000


## 🛸 Deployment

- Deployed on Vercel
- Optimized for edge-friendly streaming responses

Live Demo: (coming soon)
Demo Video: (coming soon)

## 🧭 Roadmap

- Chat title auto-generation
- Chat rename / delete
- Improved code block rendering
- Rate limiting and abuse protection
- Mobile-specific UX improvements

## 🧠 Project Philosophy

- Prefer clarity over cleverness
- Small, composable components
- Minimal but expressive UI
- Strong typing and predictable data flow
- Production mindset, even in a case study

## 📄 License

MIT
