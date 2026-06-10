# Lumios - Scalable Next.js Folder Structure

```txt
src/
│
├── app/                              # Next.js App Router
│
│   ├── (marketing)/
│   │   ├── page.tsx
│   │   ├── pricing/
│   │   └── about/
│   │
│   ├── (auth)/
│   │   ├── login/
│   │   ├── signup/
│   │   ├── forgot-password/
│   │   └── reset-password/
│   │
│   ├── (protected)/
│   │   ├── dashboard/
│   │   ├── hydration/
│   │   ├── habits/
│   │   ├── sleep/
│   │   ├── nutrition/
│   │   ├── reports/
│   │   ├── companion/
│   │   └── settings/
│   │
│   ├── api/
│   │   ├── auth/
│   │   ├── hydration/
│   │   ├── habits/
│   │   ├── sleep/
│   │   ├── nutrition/
│   │   ├── reports/
│   │   └── ai/
│   │
│   ├── layout.tsx
│   └── page.tsx
│
├── features/                         # Business Domains
│
│   ├── auth/
│   │   ├── components/
│   │   ├── hooks/
│   │   ├── actions/
│   │   ├── validations/
│   │   ├── services/
│   │   ├── types.ts
│   │   └── constants.ts
│   │
│   ├── hydration/
│   │   ├── components/
│   │   ├── hooks/
│   │   ├── actions/
│   │   ├── services/
│   │   ├── queries/
│   │   ├── validations/
│   │   └── types.ts
│   │
│   ├── habits/
│   │   ├── components/
│   │   ├── hooks/
│   │   ├── actions/
│   │   ├── services/
│   │   ├── queries/
│   │   └── types.ts
│   │
│   ├── sleep/
│   ├── nutrition/
│   ├── reports/
│   │
│   └── ai/
│       ├── chat/
│       ├── memory/
│       ├── prompts/
│       ├── tools/
│       ├── voice/
│       ├── workflows/
│       └── services/
│
├── shared/                           # Reusable Code
│
│   ├── components/
│   │
│   │   ├── ui/                       # shadcn
│   │   ├── charts/
│   │   ├── forms/
│   │   ├── layout/
│   │   ├── modals/
│   │   └── loaders/
│   │
│   ├── hooks/
│   │
│   │   ├── use-mobile.ts
│   │   ├── use-local-storage.ts
│   │   └── use-debounce.ts
│   │
│   ├── utils/
│   │
│   │   ├── date.ts
│   │   ├── calculations.ts
│   │   ├── formatters.ts
│   │   └── validators.ts
│   │
│   ├── constants/
│   │
│   │   ├── routes.ts
│   │   ├── roles.ts
│   │   └── settings.ts
│   │
│   └── types/
│       ├── api.ts
│       ├── user.ts
│       └── common.ts
│
├── server/                           # Server Only Logic
│
│   ├── db/
│   │   ├── schema/
│   │   ├── migrations/
│   │   └── queries/
│   │
│   ├── auth/
│   │
│   ├── ai/
│   │
│   ├── notifications/
│   │
│   └── analytics/
│
├── lib/                              # External SDK Setup
│
│   ├── supabase/
│   ├── openai/
│   ├── gemini/
│   ├── resend/
│   └── logger/
│
├── store/
│
│   ├── auth.store.ts
│   ├── settings.store.ts
│   └── ui.store.ts
│
├── styles/
│   ├── globals.css
│   └── themes.css
│
├── middleware.ts
│
└── config/
    ├── env.ts
    ├── app.ts
    └── feature-flags.ts
```

# Folder Rules

app/
→ Routing only

features/
→ Business logic

shared/
→ Reusable code

server/
→ Backend-only code

lib/
→ SDK initialization

store/
→ Global state only

Never put business logic inside app/
Never put API calls inside components
Never put OpenAI calls inside React components

````

# Development Flow Chart

:::writing{variant="document" id="73482"}
```txt
┌────────────────────┐
│      USER          │
└─────────┬──────────┘
          │
          ▼
┌────────────────────┐
│     NEXT.JS UI     │
│  app/(protected)   │
└─────────┬──────────┘
          │
          ▼
┌────────────────────┐
│ FEATURE LAYER      │
│ hydration          │
│ habits             │
│ sleep              │
│ nutrition          │
│ ai                 │
└─────────┬──────────┘
          │
          ▼
┌────────────────────┐
│ ACTIONS / SERVICES │
└─────────┬──────────┘
          │
          ▼
┌────────────────────┐
│ SERVER LAYER       │
│ auth               │
│ db                 │
│ ai                 │
└─────────┬──────────┘
          │
          ▼
┌────────────────────┐
│ SUPABASE DATABASE  │
└─────────┬──────────┘
          │
          ▼
┌────────────────────┐
│  HEALTH DATA       │
│ habits             │
│ hydration          │
│ sleep              │
│ nutrition          │
└────────────────────┘


AI FLOW

User Voice
     │
     ▼
Speech To Text
     │
     ▼
AI Prompt
     │
     ▼
Tool Calling
     │
     ├── Add Water
     ├── Create Habit
     ├── Log Sleep
     └── Generate Insight
     │
     ▼
Database Update
     │
     ▼
AI Response
     │
     ▼
Text To Speech
     │
     ▼
User
````