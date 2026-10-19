### Hi, I'm affifariza04 👋

**Software engineer: distributed systems, AI infrastructure, data, and the products on top of them.**

I like the parts of software that break in production: consensus under partitions, money under concurrency, LLM providers going down, data that arrives late and twice. My projects focus on *proving* correctness (simulation, invariants, mutation testing, equivalence tests) and on writing down the trade-offs.

---

### ⭐ Deep dives

| | |
|---|---|
| **[raft-kv](https://github.com/affifariza04/raft-kv)**<br>Distributed systems · TypeScript | Raft consensus from scratch and a linearizable KV store. **Deterministic simulation testing**: 500 fault schedules (1,168 crashes, 3,212 partitions, 7.7M messages) with TLA+-derived invariants. **Mutation testing** shows the checker catches injected bugs, and a scripted test reproduces the paper's Figure 8 bug, which random search can't reach. |
| **[llm-gateway](https://github.com/affifariza04/llm-gateway)**<br>AI infrastructure · Python | OpenAI-compatible gateway over Claude and Gemini: per-target **circuit breakers**, retry and failover policy, caching, **per-key USD budgets** and rate limits, SSE streaming, and Prometheus metrics. Measured at 0.6 ms p50 overhead. Design recorded in ADRs. |
| **[platform](https://github.com/affifariza04/platform)**<br>Infrastructure · Terraform/K8s | AWS (VPC, private EKS, Multi-AZ RDS) with Terraform. Kustomize, **GitOps with Argo CD**, and Pod Security `restricted` with default-deny networking. **SLO burn-rate alerts with promtool unit tests**, plus runbooks. Policy-as-code and Trivy run in CI. |
| **[order-analytics](https://github.com/affifariza04/order-analytics)**<br>Data engineering · dbt/DuckDB | Messy events (duplicates, late arrivals, schema drift) go into contracted marts, with SCD2 and point-in-time joins. The incremental pipeline is **proven equal to a full rebuild**, and handles 719k events in 72 s. |

### 🤖 AI & ML

| Project | Highlights |
|---|---|
| **[ragkit](https://github.com/affifariza04/ragkit)** · Python | Hybrid retrieval (BM25 + vectors, RRF), cited answers, and a Hit@k/MRR eval harness in CI |
| **[agentloop](https://github.com/affifariza04/agentloop)** · TypeScript | Provider-agnostic agent runtime: Zod-typed tools, self-correcting validation errors, timeouts and step limits, SSRF-safe tools |
| **[churnlab](https://github.com/affifariza04/churnlab)** · Python | Calibrated churn model with a profit-optimal decision threshold (+41% vs 0.5), served via FastAPI |
| **[bizchat](https://github.com/affifariza04/bizchat)** · JavaScript | Small-business support bot: keyword KB → Gemini → human escalation |

### 🌐 Product engineering

| Project | Highlights |
|---|---|
| **[storefront](https://github.com/affifariza04/storefront)** · Next.js + Postgres | Oversell-safe checkout, HMAC-signed idempotent payment webhooks, admin dashboard |
| **[pulse](https://github.com/affifariza04/pulse)** · WebSockets | Reconnect-and-resume and exactly-once message storage, rate limiting and origin checks |
| **[taskflow](https://github.com/affifariza04/taskflow)** · React + Express | Kanban with JWT auth, fractional ordering and optimistic UI |
| **[taskflow-mobile](https://github.com/affifariza04/taskflow-mobile)** · Flutter | Android/iOS client with optimistic updates and rollback, widget-tested against a fake API |

### Toolbox

- **Languages:** TypeScript · Python · SQL · Dart
- **Distributed systems & backend:** consensus (Raft) · deterministic simulation · WebSockets · REST · Node.js · FastAPI · Next.js
- **AI / ML:** LLM APIs (Claude, Gemini) · RAG · agents and tool calling · evaluation · scikit-learn
- **Data:** dbt · DuckDB · PostgreSQL · data contracts · SCD2 · incremental modelling
- **Infrastructure:** AWS · Terraform · Kubernetes · Argo CD · Prometheus/Grafana · SLOs · Docker · GitHub Actions · Trivy
- **Mobile & frontend:** Flutter · React

### How I work

```text
1. Define "correct" before building     →  invariants, eval sets, SLOs, business metrics
2. Prove it, don't assume it            →  simulation, mutation testing, equivalence tests
3. Simplest design that meets the bar   →  measure before adding complexity
4. Untrusted input, unreliable networks →  validate, bound, retry with jitter, fail closed
5. Write the decision down              →  ADRs, runbooks, honest "not yet" sections
```
