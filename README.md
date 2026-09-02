<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?size=30&duration=2800&color=20C20E&center=true&vCenter=true&width=800&lines=Hi%2C+I'm+Ravi+Kumar+👋;Backend+Software+Engineer;Spring+Boot+%7C+Distributed+Systems+%7C+RAG;Building+Scalable+Production+Systems+🚀" />
</p>

<img src="https://raw.githubusercontent.com/trinib/trinib/main/.github/wave.gif" width="100%" />

---

## 🧠 Terminal:

I'm **Ravi Kumar**, a **backend-focused software engineering student** who builds **secure, scalable, production-grade systems**.

I work primarily with **Java & Spring Boot**, focusing on:
- distributed systems & event-driven architecture
- API security & real-time communication
- AI-integrated applications (RAG, vector search)
- clean architecture & backend performance

🎓 **B.E. in Information Science and Engineering**
📍 JSS Academy of Technical Education, Bengaluru (VTU)
📅 09/2023 – 07/2027 | CGPA: 8.1 / 10

---

## ⚙️ System Capabilities

### 🧩 Backend & Core
<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,maven&perline=6" />
</p>

- Core & Advanced Java
- Spring Boot, Spring Security, Spring Data JPA, Hibernate
- Spring Cloud Gateway, Microservices, Event-Driven Architecture
- RESTful APIs, JWT Authentication, RBAC
- WebSocket (STOMP), Swagger/OpenAPI

---

### 🗄️ Databases & Messaging
<p align="center">
  <img src="https://skillicons.dev/icons?i=mysql,postgresql,mongodb,redis,kafka&perline=6" />
</p>

- PostgreSQL (+ pgvector), MySQL, MongoDB
- Redis, Apache Kafka
- Flyway, JDBC, Spring Data JPA, Hibernate

---

### 🤖 AI/ML Integration
- Retrieval-Augmented Generation (RAG)
- Vector Embeddings, Semantic Search
- LLM API Integration (Gemini)

---

### 🏗️ System Design
- Distributed Systems, Scalability
- Performance Optimization
- Concurrency & Multithreading
- Object-Oriented Design

---

### 🌐 Frontend (Supporting Role)
<p align="center">
  <img src="https://skillicons.dev/icons?i=react,html,css,tailwind&perline=6" />
</p>

- React 18 (functional, API-driven UI)
- Tailwind CSS
- Clean integration with backend APIs

---

### 🛠️ DevOps & Cloud
<p align="center">
  <img src="https://skillicons.dev/icons?i=git,github,docker,aws,linux,nginx,postman&perline=6" />
</p>

- Docker, Docker Compose
- AWS, GitHub Actions (CI/CD)
- Nginx, Maven
- JUnit, Postman

---

## 🚀 Production-Grade Projects

### 🔎 RepoLens — AI-Powered GitHub Repository Q&A (RAG)
**Tech:** Java 17 · Spring Boot 3 · PostgreSQL + pgvector · Gemini API · Docker Compose · REST APIs
🔗 [github.com/ravimehta251/RepoLens](https://github.com/ravimehta251/RepoLens)

- Built a RAG service that answers natural-language questions about GitHub repositories by embedding ~500-token code chunks via Gemini's `text-embedding-004` API
- Ran cosine-similarity vector search over PostgreSQL with pgvector (ivfflat index), retrieving the top-5 relevant chunks to ground each answer with cited sources
- Designed an asynchronous ingestion pipeline (`@Async`) tracking status through `PENDING → INDEXING → READY` across 4 REST endpoints
- Containerized the PostgreSQL + pgvector stack with Docker Compose; validated with a JUnit suite covering unit and integration tests

---

### 🔨 Bidly — Real-Time Auction & Bidding Platform
**Tech:** Java 21 · Spring Boot 3.3 · WebSocket (STOMP) · Redis (Redisson) · PostgreSQL · React 18 · Nginx · GitHub Actions
🔗 [github.com/ravimehta251/bidly](https://github.com/ravimehta251/bidly)

- Eliminated double-sell race conditions using Redisson distributed locks with JPA optimistic locking, validated by a 200-thread concurrency test with zero conflicting writes
- Broadcast live price updates over WebSocket (STOMP), using Redis Pub/Sub to fan out updates across app instances behind an Nginx load balancer
- Exposed 12 secured REST endpoints behind a React UI with server-authoritative countdown timers
- Gated every push with a GitHub Actions pipeline running the JUnit suite against PostgreSQL and Redis containers before building the Docker image

---

### 🛍️ ShopMesh — Distributed Event-Driven E-Commerce Microservices Platform
**Tech:** Java 21 · Spring Boot 3.3 · Spring Cloud Gateway · Eureka · Kafka · MySQL · React 18 · Docker Compose · GitHub Actions
🔗 [github.com/ravimehta251/ShopMesh](https://github.com/ravimehta251/ShopMesh)

- Decomposed checkout into 5 Spring Boot microservices routed via Spring Cloud Gateway with Eureka service discovery, orchestrated through Docker Compose
- Modeled checkout as an event-driven saga over 6 Kafka event types using the transactional outbox pattern, with compensating events releasing stock on payment failure
- Isolated 3 per-service MySQL schemas versioned with Flyway, enforcing stateless JWT authorization across 6 gateway-routed endpoints

---

## 🧠 Problem Solving & Achievements

- ✅ Solved **500+ DSA problems** on LeetCode across arrays, strings, graphs, and trees
- 🏆 **2nd Runner-Up – JSSATE Hackathon**: Built **Snap2Clean**, a civic-issue reporting platform (React, Google Maps API, MySQL), recognized for technical execution and social impact
- 🏆 **Runner-Up – HackAthena 2025** (National-level hackathon, 1,259 teams)

---

## 📬 Connect

- 📧 **Email:** ravi7481081raj@gmail.com
- 🐙 **GitHub:** https://github.com/ravimehta251
- 💼 **LinkedIn:** https://www.linkedin.com/in/ravi-mehta2511/
- 💻 **LeetCode:** https://leetcode.com/u/ravi_kumar_129

---

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=ravimehta251&color=20C20E&style=flat-square&label=PROFILE+VIEWS" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/System-Active-20C20E?style=for-the-badge&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/Backend-Focused-20C20E?style=for-the-badge&logo=spring&logoColor=black" />
</p>

<p align="center">
  <i>"I build backend systems that survive real-world usage."</i>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=20C20E&height=70&section=footer" width="100%"/>
</p>
