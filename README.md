<div align="center">

```
██╗  ██╗██╗████████╗ ██████╗██╗  ██╗███████╗███╗   ██╗███████╗██╗      ██████╗ ██╗    ██╗
██║ ██╔╝██║╚══██╔══╝██╔════╝██║  ██║██╔════╝████╗  ██║██╔════╝██║     ██╔═══██╗██║    ██║
█████╔╝ ██║   ██║   ██║     ███████║█████╗  ██╔██╗ ██║█████╗  ██║     ██║   ██║██║ █╗ ██║
██╔═██╗ ██║   ██║   ██║     ██╔══██║██╔══╝  ██║╚██╗██║██╔══╝  ██║     ██║   ██║██║███╗██║
██║  ██╗██║   ██║   ╚██████╗██║  ██║███████╗██║ ╚████║██║     ███████╗╚██████╔╝╚███╔███╔╝
╚═╝  ╚═╝╚═╝   ╚═╝    ╚═════╝╚═╝  ╚═╝╚══════╝╚═╝  ╚═══╝╚═╝     ╚══════╝ ╚═════╝  ╚══╝╚══╝ 
```

### Andrea Peruzzetto · Full Stack & AI Developer
**Building intelligent, production-ready applications from Italy 🇮🇹**

[![Email](https://img.shields.io/badge/Email-peruzzetto.saas%40gmail.com-0d1117?style=flat-square&logo=gmail&logoColor=white&labelColor=EA4335)](mailto:peruzzetto77@gmail.com)
![Location](https://img.shields.io/badge/Italy-Venice_Area-0d1117?style=flat-square&logo=googlemaps&logoColor=white&labelColor=4285F4)
![Focus](https://img.shields.io/badge/Focus-Full_Stack_AI_Engineering-0d1117?style=flat-square&logo=openai&logoColor=white&labelColor=10a37f)

</div>

---

## 👋 About Me

I'm on a focused journey to become a **Full Stack AI Engineer** — building real-world projects that bridge modern web development with intelligent AI systems.

I believe the best way to learn is by shipping. Right now that means going deep on production architecture patterns: async backends, token-based auth, AI-powered data pipelines, and clean full-stack monorepos — all things I'm actively building in my main project **KitchenFlow**.

```python
andrea = {
    "role":     "Aspiring Full Stack AI Engineer",
    "focus":    ["Production-grade backends", "AI Agents", "RAG systems"],
    "learning": ["FastAPI", "Next.js", "LLM integrations", "AI Agent workflows"],
    "values":   ["Ship real things", "Understand the stack", "Build in public"],
}
```

---

## 🛠️ Tech Stack

**Frontend**

![Next.js](https://img.shields.io/badge/Next.js_14-000000?style=flat-square&logo=next.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

**Backend & AI**

![Python](https://img.shields.io/badge/Python_3.12-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logo=python&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=llama&logoColor=white)
![Anthropic](https://img.shields.io/badge/Anthropic_Claude-191919?style=flat-square&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)

**Database & Infrastructure**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-336791?style=flat-square&logo=postgresql&logoColor=white)
![Alembic](https://img.shields.io/badge/Alembic-6C3483?style=flat-square&logo=python&logoColor=white)

---

## 🚀 Featured Project — KitchenFlow

> **An AI-powered restaurant intelligence platform** — turns raw sales data, customer reviews, and reservation logs into actionable operational insights.

```
┌─────────────────────────────────────────────────────────────────┐
│  ⚡ KitchenFlow                                                  │
│                                                                  │
│  Upload CSV/PDF menu  ──►  AI parses & structures data          │
│  Upload sales history ──►  Matching against menu items          │
│  Photo of paper agenda──►  AI Vision extracts reservations      │
│  Google Maps reviews  ──►  Auto-sync + sentiment analysis       │
│                                ▼                                 │
│              AI Correlation Engine                               │
│      "Saturday peak + 'slow service' reviews → +1 waiter"       │
│      "Tiramisu: high margin + positive sentiment → promote"      │
│                                ▼                                 │
│         Dashboard  |  Problems  |  Opportunities  |  Forecast   │
└─────────────────────────────────────────────────────────────────┘
```

### Architecture at a Glance

The project is structured as a **monorepo** with a clean separation between frontend and backend:

```
kitchenflow/
├── apps/
│   ├── backend/          # Python · FastAPI · SQLAlchemy (async)
│   │   ├── app/api/      # HTTP layer — routes only, no business logic
│   │   ├── app/services/ # Business logic layer — orchestrates everything
│   │   ├── app/crud/     # DB queries — flush, never commit
│   │   └── app/core/     # AI client, scheduler, rate limiter
│   └── frontend/         # Next.js 14 · TypeScript · Tailwind CSS
│       └── src/
│           ├── app/(auth)/      # Public routes
│           ├── app/(app)/       # Protected routes with auth guard
│           └── lib/api/         # Typed API client with auto-refresh
└── docs/                 # Architecture docs, user flows, data models
```

### Key Features Built

| Area | What's implemented |
|------|-------------------|
| 🔐 **Auth** | JWT with refresh rotation · Google OAuth 2.0 · Magic link · Email verification · Password reset |
| 🍽️ **Menu** | Upload CSV or PDF → AI text parsing → human review & confirm |
| 💰 **Sales** | Upload CSV → fuzzy match against menu items → upsert with conflict handling |
| 📅 **Reservations** | Upload photo of paper agenda → **AI Vision** (LLaVA) extracts guest data |
| ⭐ **Reviews** | Auto-sync from Google Maps via SerpApi + AI sentiment classification |
| 🧠 **AI Insights** | Daily report · Top insight (last 30d) · Sales↔Reviews correlation · Demand forecast |
| 🛡️ **Reliability** | Circuit breaker · Retry logic · Rate limiting (slowapi) · Async job queue |
| 📧 **Notifications** | Transactional emails via Resend · Jinja2 templates · Daily digest |

### AI Integration

The platform supports a **provider-agnostic AI client** that works locally or in production:

```
Development  →  Ollama (llama3.1:8b + llava for vision) — fully local, zero cost
Production   →  Anthropic Claude or OpenAI GPT — configurable via env
```

The AI layer uses a **circuit breaker pattern** — if the model is unavailable or too slow, the system degrades gracefully rather than failing user requests.

### What I Learned Building This

- Designing a clean **3-layer backend architecture** (API → Service → CRUD) that scales
- Building async Python with `asyncpg` and `SQLAlchemy 2.0` on Supabase connection pooler
- Implementing **JWT refresh token rotation** with secure httpOnly cookies
- Integrating **AI vision models** for unstructured input (handwritten agendas → structured data)
- Writing **production-hardened AI calls**: timeouts, retries, circuit breakers, cost caps
- Next.js App Router patterns: route groups, auth guards, server/client component split

---

## 📚 Currently Learning

- [ ] Advanced AI Agent workflows (tool use, planning, memory)
- [ ] RAG over pgvector — semantic search on restaurant knowledge base
- [ ] Deeper TypeScript patterns & React architecture
- [ ] Containerization and deployment pipelines

---

## 📊 GitHub Stats

<div align="center">

![Andrea's GitHub Stats](https://github-readme-stats.vercel.app/api?username=andrepaeruzzetto&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=58a6ff)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=andreaeruzzetto&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff)

</div>

---

<div align="center">

*Building in public. Learning by shipping.*
**📧 peruzzetto.saas@gmail.com**

</div>
