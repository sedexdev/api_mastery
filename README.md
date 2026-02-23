# 🚀 Modern API Mastery Roadmap (Tool-Agnostic, 2026)

**Primary Texts:**
- **The Design of Web APIs, 2nd Edition (Manning)**  
  https://www.manning.com/books/the-design-of-web-apis-second-edition
- **Hacking APIs (No Starch Press)**  
  https://nostarch.com/hacking-apis

Focus: REST, GraphQL, gRPC, security, OpenAPI, and real world architectural patterns — without relying on framework tutorials.

---

## 🧠 Phase 1 — HTTP Foundations (2–3 weeks)

**Canonical Written References**
- **MDN Web Docs — HTTP Overview**  
  https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview
- **MDN Web Docs — HTTP Messages**  
  https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages

**Video (Conceptual & Practical)**
- **HTTP Crash Course + Practical Guide** — freeCodeCamp (YouTube)  
  https://www.youtube.com/watch?v=iYM2zFP3Zn0

**Study Focus**
- Methods, status codes, headers
- Content negotiation, caching
- TLS/HTTPS basics
- CORS and preflight mechanisms

**Hands-On Practice**
- Use Postman or curl to craft requests
- Observe real API behavior (GitHub API, JSONPlaceholder)

---

## 📐 Phase 2 — REST & API Design (6–8 weeks)

**Primary Text**
- **The Design of Web APIs (Manning)**

**Important Specification**
- **OpenAPI 3.1 Specification**  
  https://spec.openapis.org/oas/latest.html

**Video (Supplemental)**
- **Designing RESTful APIs** — Pluralsight (requires account, high quality)  
  https://www.pluralsight.com/courses/restful-api-design

**Focus Areas**
- Resource modeling
- URI conventions
- HTTP verbs and safe/idempotent semantics
- Error modeling, pagination
- Versioning and deprecation policies
- API-first and contract-first development with OpenAPI

**Hands-On Practice**
- Create an OpenAPI spec from scratch
- Build a Postman collection from your spec
- Draft versioning guidance

---

## 🔁 Phase 3 — GraphQL (2–3 weeks)

**Official Docs**
- **GraphQL Learn**  
  https://graphql.org/learn/

**Structured Video**
- **GraphQL Full Course** — freeCodeCamp (YouTube, ~4 hrs)  
  https://www.youtube.com/watch?v=ed8SzALpx1Q

**Focus Areas**
- Queries, Mutations, Subscriptions
- Schema design fundamentals
- Authorization & error handling
- Cost limiting and complexity analysis

**Hands-On Practice**
- Build a small GraphQL API
- Add auth logic
- Explore schema stitching or federation basics

---

## 🛠️ Phase 4 — gRPC in Context (2–3 weeks)

### 🎥 Intro + Architecture

**Video — gRPC, HTTP/2 & API Architecture**
- **gRPC vs REST vs GraphQL** — InfoQ talk  
  https://www.youtube.com/watch?v=mZ4trNrkv14

**Article (Contextual Explanation)**
- **gRPC: A Closer Look** — DailyDev blog  
  https://daily.dev/blog/introduction-to-grpc

---

### 🧱 Practical Build

**Official Tutorial (Guided Code Example)**
- **gRPC Basics**  
  https://grpc.io/docs/languages/

Pick your language (Go / Python / Node / Java) and implement:
- A User service
- An Order service
- A REST gateway (gRPC → HTTP)

**Focus Building Blocks**
- `.proto` schema design
- Unary and Streaming RPC
- Client & server stubs
- HTTP/2 basics under the hood

---

### 📘 Schema Evolution (Text-Focused)

**Guidance on Protobuf**
- **Protocol Buffers Language Guide**  
  https://developers.google.com/protocol-buffers/docs/proto3

**Important Concepts**
- Field numbering & compatibility
- Reserved fields
- oneof and repeated fields
- Schema evolution best practices

---

### 🔒 Production Concerns

**Observability**
- Logging / tracing with gRPC metadata
- Deadlines, retries, timeouts

**Security**
- JWT metadata propagation
- Conceptual mTLS

**Service Mesh Integration**
- “Understanding gRPC with Istio” (Google Cloud docs)  
  https://cloud.google.com/istio/docs/concepts/grpc

---

### 📊 Trade-Off Reflection

After building:

- When is REST simpler and preferable?
- When does binary + HTTP/2 shine?
- How do you version a gRPC API?
- What are debugging challenges compared to HTTP/JSON?

This reflection embeds architectural mastery.

---

## 🔐 Phase 5 — API Security (6–8 weeks)

**Primary Book (Applied Security)**
- **Hacking APIs (No Starch Press)**

**Supplementary Free Resources**
- **OWASP API Security Top 10**  
  https://owasp.org/API-Security/
- **PortSwigger Web Security Academy — API Labs**  
  https://portswigger.net/web-security/api-testing
- **OWASP Juice Shop (self-hosted vulnerable app)**  
  https://owasp.org/projects/juice-shop/

**Core Focus Areas**
- Broken object level authorization
- OAuth 2.0 & JWT threats
- IDOR & business logic attacks
- Rate limiting bypass
- Fuzzing & automated attacks

**Hands-On Practice**
- Attack your own mini API
- Apply defense mechanisms
- Track vulnerabilities in a bug tracker (replicate real processes)

---

## 🔄 Phase 6 — API Lifecycle & Governance (3–4 weeks)

**Standards**
- **OpenAPI 3.1 Spec**
- **AsyncAPI Spec (Event APIs)**  
  https://www.asyncapi.com/docs/

**Core Topics**
- Contract-first API governance
- Versioning & backward compatibility
- API gateways & policy enforcement
- Deprecation scheduling
- Observability (metrics, tracing, logging)

**Practice**
- Publish an OpenAPI & AsyncAPI spec
- Create a versioning policy document
- Add gating rules (e.g., minimal schema changes for minor versions)

---

## 🎓 Capstone Project

Combine everything:

- REST API with OpenAPI spec  
- JWT auth and role-based authorization  
- Mini gRPC microservices layer  
- GraphQL endpoint  
- Documentation site (Notion / repos)  
- Tests & contract validation  
- Security testing sweep (OWASP Top 10 + Hacking APIs methods)

Optional: Deploy locally or on cloud (with logs/metrics).

---

## 📅 Estimated Timeline (Balanced)

| Phase | Duration |
|-------|----------|
| HTTP Foundations | 2–3 wks |
| REST & API Design | 6–8 wks |
| GraphQL | 2–3 wks |
| gRPC | 2–3 wks |
| API Security | 6–8 wks |
| Lifecycle & Governance | 3–4 wks |
| Capstone | 4 wks |

**Total:** ~6 months (5–8 hrs / week)

---

## 🎯 Final Outcome

You will be able to:

✔ Evaluate API style trade-offs  
✔ Design robust, versioned APIs  
✔ Document APIs with canonical specs  
✔ Integrate security by design  
✔ Build and defend API systems  
✔ Leverage REST, GraphQL, gRPC appropriately  

---
