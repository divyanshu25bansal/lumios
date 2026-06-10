# Lumios Learning + Build Roadmap

## Rule #1

Never learn something without immediately using it.

### Bad

* [ ] Learn JWT for 3 days

### Good

* [ ] Learn JWT
* [ ] Build JWT Login
* [ ] Use JWT

Same day.

---

# Phase 0 — Foundation

## Goal

Understand Next.js App Router and project structure.

## Learn

* [ ] What is Next.js App Router
* [ ] page.jsx
* [ ] layout.jsx
* [ ] Link component
* [ ] useRouter()

## Build

* [ ] Create Next.js project
* [ ] Setup Tailwind
* [ ] Setup shadcn/ui
* [ ] Setup GitHub
* [ ] Create folder structure

## Deliverable

* [ ] Home page
* [ ] About page
* [ ] Navigation works

---

# Phase 1 — Learn JWT Authentication

## Goal

Understand how authentication actually works.

> IMPORTANT: This phase is for learning only. You will replace it with Supabase Auth later.

## Learn

* [ ] Password hashing
* [ ] bcrypt
* [ ] JWT
* [ ] Cookies
* [ ] Middleware

## Build

### Users Table

* [ ] id
* [ ] email
* [ ] password

### Backend

* [ ] Signup API
* [ ] Login API
* [ ] Logout API

### JWT

* [ ] Generate token
* [ ] Store token in cookie
* [ ] Verify token

### Frontend

* [ ] Login page
* [ ] Signup page

### Protected Routes

* [ ] Dashboard route

## Deliverable

* [ ] User can signup
* [ ] User can login
* [ ] User can logout
* [ ] Protected dashboard works

## Knowledge Gained

* [ ] How authentication works internally
* [ ] How JWT works
* [ ] How cookies work

### STOP HERE

Do not continue until JWT authentication is fully working.

---

# Phase 2 — Rebuild Using Supabase Auth

## Goal

Learn the industry-standard shortcut.

## Learn

* [ ] Supabase Auth
* [ ] Sessions
* [ ] User management

## Build

* [ ] Create Supabase project
* [ ] Enable Email Authentication
* [ ] Replace JWT signup
* [ ] Replace JWT login
* [ ] Create user_profiles table

## Git

* [ ] Create branch: jwt-learning
* [ ] Create branch: main

## Deliverable

* [ ] Same authentication system
* [ ] Less code
* [ ] Better security

## Knowledge Gained

* [ ] Why developers use auth providers
* [ ] Difference between JWT and Supabase Auth

---

# Phase 3 — User Profiles

## Goal

Learn databases properly.

## Learn

* [ ] Tables
* [ ] Relationships
* [ ] CRUD operations

## Build

### user_profiles

* [ ] name
* [ ] age
* [ ] gender
* [ ] weight
* [ ] height

### Pages

* [ ] Onboarding
* [ ] Profile

## Deliverable

* [ ] Save profile
* [ ] Fetch profile
* [ ] Update profile

## Knowledge Gained

* [ ] Database fundamentals
* [ ] CRUD operations

---

# Phase 4 — Hydration Module

## Goal

Build your first real feature.

## Learn

* [ ] Database queries
* [ ] User-specific data

## Build

### water_logs

* [ ] amount
* [ ] date
* [ ] user_id

### Features

* [ ] Add water
* [ ] Delete water
* [ ] View history
* [ ] Daily total

### Dashboard

* [ ] Progress bar
* [ ] Goal tracking

## Deliverable

* [ ] Complete hydration tracker

## Knowledge Gained

* [ ] Real-world CRUD
* [ ] Data filtering

---

# Phase 5 — Habits

## Goal

Learn relational databases.

## Tables

### habits

* [ ] id
* [ ] user_id
* [ ] title

### habit_logs

* [ ] habit_id
* [ ] completed_at

## Learn

* [ ] One-to-many relationships

## Build

* [ ] Create habit
* [ ] Complete habit
* [ ] Delete habit
* [ ] Habit streak

## Deliverable

* [ ] Habit tracker

## Knowledge Gained

* [ ] Relationships
* [ ] Foreign keys

---

# Phase 6 — Dashboard

## Goal

Learn aggregation and dashboard design.

## Build

* [ ] Welcome card
* [ ] Hydration card
* [ ] Habit card
* [ ] Quick actions section

## Learn

* [ ] Combining multiple datasets
* [ ] Dashboard UX

## Deliverable

* [ ] Functional dashboard

---

# Phase 7 — Gemini AI Chat

## Goal

Learn AI integration.

## Learn

* [ ] Prompts
* [ ] Context
* [ ] Chat history

## Build

* [ ] Chat page
* [ ] Message input
* [ ] Message history
* [ ] Gemini integration

## Deliverable

* [ ] AI companion chat

## Knowledge Gained

* [ ] AI fundamentals

---

# Phase 8 — Tool Calling

## Goal

Build a real AI agent.

## Learn

* [ ] Function calling
* [ ] Tool calling

## Tool 1 — Add Water

### User

"I drank 500ml water"

### AI

* [ ] Updates database

## Tool 2 — Create Habit

### User

"Create a reading habit"

### AI

* [ ] Creates habit

## Tool 3 — Dashboard Summary

### User

"How am I doing today?"

### AI

* [ ] Reads hydration data
* [ ] Reads habits data
* [ ] Generates summary

## Deliverable

* [ ] Real AI actions

## Knowledge Gained

* [ ] Agent architecture
* [ ] Tool calling

---

# Phase 9 — Voice

## Goal

Make the product feel magical.

## Learn

* [ ] Speech-to-Text
* [ ] Text-to-Speech

## Build

* [ ] Microphone button
* [ ] Voice input
* [ ] Voice response

## Deliverable

* [ ] Voice companion

---

# Phase 10 — AI Memory

## Goal

Make AI feel personal.

## Table

### agent_memories

* [ ] id
* [ ] user_id
* [ ] memory
* [ ] created_at

## Build

* [ ] Save memory
* [ ] Retrieve memory

## Examples

* [ ] User misses hydration goals
* [ ] User prefers morning habits

## Deliverable

* [ ] Personalized AI responses

---

# Phase 11 — Reports

## Goal

Visualize progress.

## Learn

* [ ] Recharts

## Build

### Hydration

* [ ] Weekly chart
* [ ] Monthly chart

### Habits

* [ ] Weekly completion chart
* [ ] Monthly completion chart

## Deliverable

* [ ] Analytics dashboard

---

# MVP Launch Checklist

## Must Have

* [ ] Supabase Auth
* [ ] Onboarding
* [ ] User Profile
* [ ] Hydration
* [ ] Habits
* [ ] Dashboard
* [ ] AI Chat
* [ ] Add Water Tool
* [ ] Create Habit Tool

## Nice To Have

* [ ] Voice
* [ ] Memory
* [ ] Reports

## Ignore Completely For Now

* [ ] Sleep Tracking
* [ ] Nutrition
* [ ] Notifications
* [ ] Achievements
* [ ] Social Features
* [ ] Premium Plans
* [ ] Mobile App

---

# Launch Rule

🚀 Launch as soon as all **Must Have** items are complete.

Do not wait for Voice, Memory, Reports, Sleep Tracking, Nutrition, or Premium features.