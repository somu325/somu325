```
╔══════════════════════════════════════════════════════════════╗
║   somasekhar-reddy / api                                      ║
║   Full Stack Developer · Hyderabad, IN                        ║
║   Status: 200 OK · Uptime: 2+ yrs · Zero unplanned downtime   ║
╚══════════════════════════════════════════════════════════════╝
```

**Base URL:** `https://github.com/somu325`
**Auth:** none required — I answer emails without a bearer token

---

### `GET /profile`

```json
{
  "name": "Somasekhar Reddy Irikireddy",
  "role": "Full Stack Developer",
  "experience_years": 2,
  "location": "Hyderabad, Telangana, India",
  "summary": "Ships production APIs in Node/Express and FastAPI. Comfortable owning a service end to end — schema design, auth, deployment, the 2am incident that follows.",
  "origin_story": "B.Tech in Mechanical Engineering, pivoted into software in 2023. Debugging a stress fracture and debugging a race condition turned out to require the same instinct.",
  "currently": "Building 30+ REST APIs for a multi-vendor e-commerce platform"
}
```

---

### `GET /skills`

```json
{
  "languages":  ["JavaScript (ES6+)", "TypeScript", "Python"],
  "frontend":   ["React.js", "Tailwind CSS", "HTML5/CSS3"],
  "backend":    ["Node.js", "Express.js", "FastAPI", "Socket.io", "JWT Auth + RBAC"],
  "data":       ["MongoDB (aggregation pipelines)", "PostgreSQL", "Redis", "Supabase"],
  "cloud_devops": ["AWS (EC2, S3)", "Docker", "GitHub Actions CI/CD", "Google Cloud Run", "Firebase"],
  "integrations": ["Razorpay", "Nodemailer", "OpenAI API", "Google Gemini API", "Passport.js"]
}
```

---

### `GET /experience` → CHANGELOG.md

```
## v3.0.0 — Software Developer @ Daksh Global Innovations (Oct 2025–Present)
  + Shipped 30+ REST APIs for multi-vendor e-commerce (onboarding, catalog, cart, orders)
  * Replaced Mongoose populate() with aggregation pipelines → cut response times
    on the platform's heaviest queries
  + Implemented JWT + RBAC across vendor / customer / admin dashboards
  + Integrated Razorpay, AWS S3, Nodemailer

## v2.0.0 — Full Stack Developer @ Corp-Astro, Freelance (Mar–Aug 2025)
  + Designed and built a private astrology platform solo — React, FastAPI,
    WebSocket real-time chat — architecture through production deploy
  + Shipped 20+ FastAPI endpoints, self-documenting via OpenAPI/Swagger
  + Configured Redis caching + normalized Postgres schema (Supabase)
  + Deployed and managed production on AWS EC2

## v1.0.0 — Software Developer @ Genamplify Solutions Hub (Mar 2024–Feb 2025)
  + Owned backend for a booking platform — 30+ services in Node/Express
  + Built validation + error-handling middleware from scratch
  + Added real-time booking notifications via Socket.io
  + Secured endpoints with JWT over indexed MongoDB schemas

## v0.1.0 — Mechanical Engineering (2020–2023)
  + Learned that every system fails somewhere — just wasn't APIs yet
```

---

### `GET /projects`

| Method | Endpoint | Description |
|---|---|---|
| `POST` | `/resonance/match` | AI resume-to-JD matcher — skill-gap % + fit verdict via OpenAI, auto-fallback to Gemini. Passport auth (email/Google/GitHub). Deployed on Cloud Run via Docker + GitHub Actions using Workload Identity Federation — no static keys in CI. |
| `POST` | `/booking/slots` | React calendar with drag-and-drop scheduling and real conflict detection. Node/Express + MongoDB aggregation for live availability. JWT-secured create/cancel, automated email + SMS confirmations. |
| `GET` | `/corp-astro/chat` | Private astrology platform, solo build — React + FastAPI + WebSocket chat, from architecture to production on EC2. |

---

### `GET /status-codes`

```
200 OK                 — actively employed, actively building
201 Created             — open to backend-heavy full stack roles
418 I'm a teapot        — mechanical engineer who now ships JavaScript
503 Unavailable         — mid-sprint, try again in a standup
```

---

### `POST /contact`

```bash
curl -X POST https://somasekhar.dev/contact \
  -H "Content-Type: application/json" \
  -d '{
        "email": "somureddyirikireddy@gmail.com",
        "linkedin": "linkedin.com/in/somureddy",
        "phone": "+91-9391556743",
        "message": "Let'\''s build something that needs to actually work in production."
      }'
```

```json
{ "response": "202 Accepted — I reply fast." }
```
