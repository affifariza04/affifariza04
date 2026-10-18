### Hi, I'm affifariza04 👋

**Full-stack developer & AI engineer.** I build complete digital products (web, mobile, real-time, and AI) and ship them measured, tested and deployable.

- 🧠 Focus: LLM applications (RAG, tool-using agents) and the products around them
- 🌐 End to end: database → API → web & mobile clients → CI/CD and Docker
- 🛠️ I care about correctness under real conditions: concurrency, retries, bad networks, untrusted input

---

### 🤖 AI & machine learning

| Project | What it is | Highlights |
|---|---|---|
| **[ragkit](https://github.com/affifariza04/ragkit)** · Python | Hybrid-search RAG service with cited answers | BM25 + vectors fused with RRF · heading-aware chunking · Hit@k / MRR eval in CI · FastAPI + Docker |
| **[agentloop](https://github.com/affifariza04/agentloop)** · TypeScript | Provider-agnostic AI agent runtime | Zod-typed tools · self-correcting validation errors · parallel calls, timeouts, step limits · Claude & Gemini · SSRF-safe tools |
| **[churnlab](https://github.com/affifariza04/churnlab)** · Python | Churn prediction, from data to decision | CV model selection · calibration · profit-optimal threshold (+41% vs 0.5) · FastAPI scoring API |
| **[bizchat](https://github.com/affifariza04/bizchat)** · JavaScript | Customer-service chatbot for small businesses | keyword KB → Gemini fallback → human escalation · staff dashboard |

### 🌐 Full-stack web

| Project | What it is | Highlights |
|---|---|---|
| **[storefront](https://github.com/affifariza04/storefront)** · Next.js | E-commerce app on Next.js 16 + PostgreSQL | oversell-safe checkout · HMAC-signed, idempotent payment webhooks · Server Actions · admin dashboard |
| **[taskflow](https://github.com/affifariza04/taskflow)** · React + Express | Kanban task manager | JWT + scrypt auth · rate limiting · drag-and-drop with fractional ordering · optimistic UI · Docker |
| **[pulse](https://github.com/affifariza04/pulse)** · WebSocket | Real-time chat rooms | presence & typing · reconnect-and-resume · exactly-once storage · rate limiting · origin checks |

### 📱 Mobile

| Project | What it is | Highlights |
|---|---|---|
| **[taskflow-mobile](https://github.com/affifariza04/taskflow-mobile)** · Flutter | Android / iOS client for the taskflow API | Material 3 · swipe gestures · optimistic updates with rollback · widget tests against a fake API |

### Toolbox

- **AI / ML:** LLM APIs (Claude, Gemini) · RAG · tool calling / agents · embeddings · scikit-learn · pandas · NumPy
- **Web:** TypeScript · React · Next.js · Node.js · Express · Python · FastAPI · WebSockets · REST design
- **Mobile:** Flutter · Dart
- **Data & Ops:** PostgreSQL · SQLite · Drizzle ORM · Docker · GitHub Actions · Vitest · pytest

### How I work

```text
1. Define what "good" means before building   →  eval sets, tests, business metric
2. Start with the simplest thing that can work →  let measurements justify complexity
3. Treat every input as untrusted               →  validate, bound, sandbox, sign
4. Write down trade-offs and limitations        →  every README has a "Design decisions" section
```
