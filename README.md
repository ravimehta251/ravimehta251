<!--
  ravi-kumar.service — GitHub profile README
  theme : production backend · terminal green #20C20E on #0d1117
  note  : the mermaid diagrams render natively on GitHub (no images needed)
-->

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=venom&color=0d1117&height=220&section=header&text=RAVI%20KUMAR&fontSize=68&fontColor=20C20E&fontAlignY=38&desc=backend%20engineer%20%C2%B7%20distributed%20systems%20%C2%B7%20applied%20AI&descSize=18&descAlignY=60&animation=fadeIn" width="100%" alt="Ravi Kumar — backend engineer"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=2600&pause=900&color=20C20E&center=true&vCenter=true&width=720&height=40&lines=%3E+booting+ravi-kumar.service+...;Backend+Engineer+%C2%B7+Java+%C2%B7+Spring+Boot;Kafka+sagas+%C2%B7+Redis+locks+%C2%B7+pgvector+RAG;Building+systems+that+survive+production+%F0%9F%9A%80" alt="intro"/>
</p>

<p align="center">
  <a href="#about"><kbd>&nbsp;~/about&nbsp;</kbd></a>&nbsp;
  <a href="#stack"><kbd>&nbsp;~/stack&nbsp;</kbd></a>&nbsp;
  <a href="#services"><kbd>&nbsp;~/services&nbsp;</kbd></a>&nbsp;
  <a href="#decisions"><kbd>&nbsp;~/decisions&nbsp;</kbd></a>&nbsp;
  <a href="#metrics"><kbd>&nbsp;~/metrics&nbsp;</kbd></a>&nbsp;
  <a href="#connect"><kbd>&nbsp;~/connect&nbsp;</kbd></a>
</p>

```diff
@@  ravi-kumar.service · boot sequence  @@
+ [  OK  ]  Loaded      jvm.runtime ................ Java 17 · Java 21
+ [  OK  ]  Started     spring-boot.service ........ Security · Data JPA · Cloud Gateway
+ [  OK  ]  Mounted     postgres.volume ............ + pgvector · ivfflat index
+ [  OK  ]  Connected   kafka.cluster .............. event-driven saga · outbox
+ [  OK  ]  Acquired    redisson.lock .............. 0 conflicts @ 200 threads
+ [  OK  ]  Indexed     repolens.vectors ........... top-5 cosine · cited sources
+ [  OK  ]  Listening   :8080/api · /ws ............ REST + WebSocket (STOMP)
+ [  OK  ]  Passed      ci.pipeline ................ JUnit · Postgres + Redis containers
- [ WARN ]  Detected    coffee.level < 20% ......... auto-refill scheduled
@@  active (running) since 2023 · ready to accept requests  @@
```

## ~/about

```http
GET /api/v1/engineers/ravi-kumar HTTP/1.1
Host: github.com
Accept: application/json
```

<sub>⤷ <code>200 OK</code> · <code>Content-Type: application/json</code> · <code>X-Powered-By: Spring Boot</code></sub>

```json
{
  "name": "Ravi Kumar",
  "role": "Backend Software Engineer",
  "location": "Bengaluru, India",
  "education": {
    "degree": "B.E. Information Science & Engineering",
    "institute": "JSS Academy of Technical Education (VTU)",
    "batch": "2023 – 2027",
    "cgpa": 8.1
  },
  "primaryStack": ["Java", "Spring Boot", "PostgreSQL", "Kafka", "Redis"],
  "focus": [
    "distributed systems & event-driven architecture",
    "API security & real-time communication",
    "AI-integrated applications (RAG, vector search)",
    "clean architecture & backend performance"
  ],
  "motto": "I build backend systems that survive real-world usage."
}
```

## ~/stack

| layer | tools | in practice |
|:--|:--:|:--|
| **core** | <img src="https://skillicons.dev/icons?i=java,spring,maven" height="36" alt="java spring maven"/> | Core & Advanced Java · Spring Boot · Spring Security · Spring Data JPA · Hibernate · Spring Cloud Gateway |
| **apis** | <img src="https://skillicons.dev/icons?i=postman" height="36" alt="postman"/> | RESTful APIs · JWT · RBAC · WebSocket (STOMP) · Swagger / OpenAPI |
| **data** | <img src="https://skillicons.dev/icons?i=postgres,mysql,mongodb,redis" height="36" alt="postgres mysql mongodb redis"/> | PostgreSQL + pgvector · MySQL · MongoDB · Redis · Flyway · JDBC |
| **messaging** | <img src="https://skillicons.dev/icons?i=kafka" height="36" alt="kafka"/> | Apache Kafka · event-driven architecture · transactional outbox · Redis Pub/Sub |
| **ai** | <img src="https://img.shields.io/badge/Gemini-0d1117?style=for-the-badge&logo=googlegemini&logoColor=20C20E" height="28" alt="gemini"/> | RAG · vector embeddings · semantic search · LLM API integration |
| **design** | 🏗️ | distributed systems · scalability · concurrency & multithreading · performance optimization · OOD |
| **infra** | <img src="https://skillicons.dev/icons?i=docker,aws,githubactions,nginx,linux" height="36" alt="docker aws github-actions nginx linux"/> | Docker & Docker Compose · AWS · GitHub Actions CI/CD · Nginx |
| **quality** | <img src="https://skillicons.dev/icons?i=git,github" height="36" alt="git github"/> | JUnit (unit + integration) · concurrency testing · Git |
| **frontend** <sub>supporting</sub> | <img src="https://skillicons.dev/icons?i=react,tailwind,html,css" height="36" alt="react tailwind html css"/> | React 18 · Tailwind CSS · clean, API-driven UIs |

## ~/services

```console
$ docker compose ps
NAME       STATUS         STACK                                HIGHLIGHT
repolens   Up (healthy)   Spring Boot 3 · pgvector · Gemini    top-5 retrieval · cited answers
bidly      Up (healthy)   STOMP · Redisson · Redis Pub/Sub     0 conflicts @ 200 threads
shopmesh   Up (healthy)   Kafka saga · Gateway · Eureka        5 services · 6 event types
```

### `01` RepoLens &nbsp;<sub>AI-powered Q&A over any GitHub repository</sub>

> Ask a codebase anything in plain English. Every answer is grounded in retrieved code and cited back to its source.
>
> <a href="https://github.com/ravimehta251/RepoLens"><img src="https://img.shields.io/badge/source-ravimehta251%2FRepoLens-20C20E?style=flat-square&logo=github&labelColor=0d1117" alt="RepoLens source"/></a>

<p>
  <img src="https://img.shields.io/badge/Java_17-0d1117?style=flat-square&logo=openjdk&logoColor=20C20E" alt="Java 17"/>
  <img src="https://img.shields.io/badge/Spring_Boot_3-0d1117?style=flat-square&logo=springboot&logoColor=20C20E" alt="Spring Boot 3"/>
  <img src="https://img.shields.io/badge/PostgreSQL_%2B_pgvector-0d1117?style=flat-square&logo=postgresql&logoColor=20C20E" alt="PostgreSQL + pgvector"/>
  <img src="https://img.shields.io/badge/Gemini_API-0d1117?style=flat-square&logo=googlegemini&logoColor=20C20E" alt="Gemini API"/>
  <img src="https://img.shields.io/badge/Docker_Compose-0d1117?style=flat-square&logo=docker&logoColor=20C20E" alt="Docker Compose"/>
  <img src="https://img.shields.io/badge/JUnit-0d1117?style=flat-square&logo=junit5&logoColor=20C20E" alt="JUnit"/>
</p>

- **Embedding pipeline:** splits code into ~500-token chunks and embeds them with Gemini `text-embedding-004`
- **Vector retrieval:** cosine-similarity search on PostgreSQL + pgvector (ivfflat index). The top-5 chunks ground every answer, with sources cited
- **Async ingestion:** an `@Async` pipeline tracks each repo through `PENDING → INDEXING → READY` across 4 REST endpoints
- **Shipped & tested:** the Postgres + pgvector stack is containerized with Docker Compose and validated by a JUnit suite (unit + integration)

```mermaid
flowchart TB
    subgraph ingest["⚙️ async ingestion · PENDING → INDEXING → READY"]
        direction LR
        R["GitHub repo"] --> CH["chunker<br/>~500 tokens"] --> EM["Gemini<br/>text-embedding-004"] --> PG[("PostgreSQL<br/>pgvector · ivfflat")]
    end
    subgraph query["💬 query path"]
        direction LR
        Q["question"] --> QE["embed query"] --> VS{"cosine search<br/>top-5 chunks"} --> LLM["Gemini LLM"] --> ANS["answer +<br/>cited sources"]
    end
    ingest -. "vectors" .-> query

    classDef box fill:#0d1117,stroke:#20C20E,color:#e6edf3,stroke-width:1px
    classDef hot fill:#20C20E,stroke:#20C20E,color:#0d1117
    class R,CH,EM,Q,QE,LLM box
    class PG,VS,ANS hot
    style ingest fill:transparent,stroke:#20C20E,stroke-dasharray:4 4
    style query fill:transparent,stroke:#20C20E,stroke-dasharray:4 4
```

### `02` Bidly &nbsp;<sub>real-time auction & bidding platform</sub>

> Live auctions where two people can never win the same item, even when they bid in the same millisecond.
>
> <a href="https://github.com/ravimehta251/bidly"><img src="https://img.shields.io/badge/source-ravimehta251%2Fbidly-20C20E?style=flat-square&logo=github&labelColor=0d1117" alt="Bidly source"/></a>

<p>
  <img src="https://img.shields.io/badge/Java_21-0d1117?style=flat-square&logo=openjdk&logoColor=20C20E" alt="Java 21"/>
  <img src="https://img.shields.io/badge/Spring_Boot_3.3-0d1117?style=flat-square&logo=springboot&logoColor=20C20E" alt="Spring Boot 3.3"/>
  <img src="https://img.shields.io/badge/WebSocket_%C2%B7_STOMP-0d1117?style=flat-square" alt="WebSocket STOMP"/>
  <img src="https://img.shields.io/badge/Redis_%C2%B7_Redisson-0d1117?style=flat-square&logo=redis&logoColor=20C20E" alt="Redis Redisson"/>
  <img src="https://img.shields.io/badge/PostgreSQL-0d1117?style=flat-square&logo=postgresql&logoColor=20C20E" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/React_18-0d1117?style=flat-square&logo=react&logoColor=20C20E" alt="React 18"/>
  <img src="https://img.shields.io/badge/Nginx-0d1117?style=flat-square&logo=nginx&logoColor=20C20E" alt="Nginx"/>
  <img src="https://img.shields.io/badge/GitHub_Actions-0d1117?style=flat-square&logo=githubactions&logoColor=20C20E" alt="GitHub Actions"/>
</p>

- **Zero double-sells:** Redisson distributed locks plus JPA optimistic locking. A 200-thread concurrency test produced **0 conflicting writes**
- **Live price fan-out:** WebSocket (STOMP) broadcasts, with Redis Pub/Sub carrying updates across app instances behind an Nginx load balancer
- **12 secured REST endpoints** behind a React 18 UI with server-authoritative countdown timers
- **Gated CI:** GitHub Actions runs the JUnit suite against real PostgreSQL & Redis containers before building the Docker image

```mermaid
sequenceDiagram
    autonumber
    actor U as Bidder
    participant LB as Nginx
    participant A as App instance A
    participant R as Redis · Redisson
    participant DB as PostgreSQL
    participant B as App instance B
    actor W as Watchers
    U->>LB: place bid
    LB->>A: route request
    A->>R: acquire lock on auction
    rect rgba(32, 194, 14, 0.12)
        Note over A,DB: critical section — one writer per auction
        A->>DB: write bid (JPA @Version check)
        DB-->>A: committed ✓
    end
    A->>R: release lock + publish new price
    R-->>B: Pub/Sub fan-out
    A-->>U: STOMP push · new price
    B-->>W: STOMP push · new price
```

### `03` ShopMesh &nbsp;<sub>distributed, event-driven e-commerce microservices</sub>

> Checkout as a distributed saga. Every service owns its own data, with no distributed transactions.
>
> <a href="https://github.com/ravimehta251/ShopMesh"><img src="https://img.shields.io/badge/source-ravimehta251%2FShopMesh-20C20E?style=flat-square&logo=github&labelColor=0d1117" alt="ShopMesh source"/></a>

<p>
  <img src="https://img.shields.io/badge/Java_21-0d1117?style=flat-square&logo=openjdk&logoColor=20C20E" alt="Java 21"/>
  <img src="https://img.shields.io/badge/Spring_Boot_3.3-0d1117?style=flat-square&logo=springboot&logoColor=20C20E" alt="Spring Boot 3.3"/>
  <img src="https://img.shields.io/badge/Spring_Cloud_Gateway-0d1117?style=flat-square&logo=spring&logoColor=20C20E" alt="Spring Cloud Gateway"/>
  <img src="https://img.shields.io/badge/Eureka-0d1117?style=flat-square" alt="Eureka"/>
  <img src="https://img.shields.io/badge/Apache_Kafka-0d1117?style=flat-square&logo=apachekafka&logoColor=20C20E" alt="Apache Kafka"/>
  <img src="https://img.shields.io/badge/MySQL_%C2%B7_Flyway-0d1117?style=flat-square&logo=mysql&logoColor=20C20E" alt="MySQL Flyway"/>
  <img src="https://img.shields.io/badge/React_18-0d1117?style=flat-square&logo=react&logoColor=20C20E" alt="React 18"/>
  <img src="https://img.shields.io/badge/Docker_Compose-0d1117?style=flat-square&logo=docker&logoColor=20C20E" alt="Docker Compose"/>
  <img src="https://img.shields.io/badge/GitHub_Actions-0d1117?style=flat-square&logo=githubactions&logoColor=20C20E" alt="GitHub Actions"/>
</p>

- **5 microservices** routed through Spring Cloud Gateway with Eureka service discovery, orchestrated via Docker Compose
- **Event-driven saga:** checkout runs over 6 Kafka event types using the transactional outbox pattern. Compensating events release stock when payment fails
- **Database-per-service:** 3 isolated MySQL schemas, each versioned with Flyway
- **Stateless JWT authorization** enforced across 6 gateway-routed endpoints

```mermaid
flowchart LR
    UI["React 18"] -->|JWT| GW["Spring Cloud<br/>Gateway"]
    GW -.->|discovery| EU["Eureka<br/>registry"]
    GW --> ORD["order<br/>service"]
    ORD -->|same transaction| OBX[("outbox")]
    OBX -->|publish| K{{"Apache Kafka<br/>6 event types"}}
    K --> INV["inventory<br/>service"]
    K --> PAY["payment<br/>service"]
    PAY -.->|payment failed| K
    K -.->|compensate · release stock| INV

    classDef box fill:#0d1117,stroke:#20C20E,color:#e6edf3,stroke-width:1px
    classDef hot fill:#20C20E,stroke:#20C20E,color:#0d1117
    class UI,GW,EU,ORD,INV,PAY box
    class OBX,K hot
```

## ~/decisions

<sub>Architecture Decision Records: the <i>why</i> behind the code, and the cost I chose to pay.</sub>

| id | problem | decision | trade-off accepted |
|:-:|:--|:--|:--|
| `ADR-01` | Two bids hit the same auction in the same millisecond | Redisson distributed lock **+** JPA optimistic locking (`@Version`) as a second line of defense | an extra Redis round-trip per bid: cheap insurance against double-sells |
| `ADR-02` | Checkout spans services that each own their data | Saga over Kafka with a **transactional outbox**, plus compensating events on failure | eventual consistency and compensation logic, instead of a 2PC that doesn't scale |
| `ADR-03` | Live prices must reach clients connected to *any* instance | Redis Pub/Sub fan-out behind Nginx, pushed to browsers over STOMP | Pub/Sub is fire-and-forget, with no replay for a subscriber that was offline |
| `ADR-04` | Semantic search over code without adding a new datastore | pgvector inside PostgreSQL with an ivfflat index | approximate nearest-neighbour search, giving up a little recall for speed |
| `ADR-05` | Indexing a whole repository is slow | `@Async` ingestion with an explicit `PENDING → INDEXING → READY` lifecycle | callers check status instead of getting one blocking response |

## ~/metrics

```sh
$ curl -s localhost:8080/actuator/prometheus | grep ravi_

# HELP ravi_dsa_problems_solved_total  LeetCode problems solved
ravi_dsa_problems_solved_total{topics="arrays,strings,graphs,trees"}               500

# HELP ravi_hackathon_podiums_total  Podium finishes at hackathons
ravi_hackathon_podiums_total{event="HackAthena 2025",level="national",teams="1259"}  1
ravi_hackathon_podiums_total{event="JSSATE Hackathon",project="Snap2Clean"}          1

# HELP ravi_conflicting_writes_total  Double-sells under a 200-thread load test
ravi_conflicting_writes_total{service="bidly",threads="200"}                       0

# HELP ravi_cgpa  Current CGPA on a 10-point scale
ravi_cgpa{program="B.E. ISE"}                                                      8.1
```

| | result | context |
|:-:|:--|:--|
| 🥈 | **Runner-Up · HackAthena 2025** | National-level hackathon, 1,259 teams |
| 🥉 | **2nd Runner-Up · JSSATE Hackathon** | Built **Snap2Clean**, a civic-issue reporting platform (React · Google Maps API · MySQL), recognized for technical execution & social impact |
| ⚡ | **500+ DSA problems** | LeetCode: arrays, strings, graphs, trees |

<p align="center">
  <img src="https://streak-stats.demolab.com?user=ravimehta251&background=0d1117&ring=20C20E&fire=20C20E&currStreakLabel=20C20E&currStreakNum=e6edf3&sideNums=e6edf3&sideLabels=8b949e&dates=8b949e&stroke=30363d&hide_border=true" height="170" alt="GitHub streak"/>
  <img src="https://leetcard.jacoblin.cool/ravi_kumar_129?theme=dark&font=JetBrains%20Mono" height="170" alt="LeetCode stats"/>
</p>

<p align="center">
  <img src="https://ghchart.rshah.org/20C20E/ravimehta251" width="100%" alt="GitHub contribution chart"/>
</p>

## ~/connect

| method | channel | endpoint |
|:--|:--|:--|
| `POST` | 📧 mail | [ravi7481081raj@gmail.com](mailto:ravi7481081raj@gmail.com) |
| `GET` | 💼 linkedin | [linkedin.com/in/ravi-mehta2511](https://www.linkedin.com/in/ravi-mehta2511/) |
| `GET` | 💻 leetcode | [leetcode.com/u/ravi_kumar_129](https://leetcode.com/u/ravi_kumar_129) |
| `GET` | 🐙 github | [github.com/ravimehta251](https://github.com/ravimehta251) |

<p align="center">
  <br/>
  <i>"I build backend systems that survive real-world usage."</i>
  <br/><br/>
  <img src="https://komarev.com/ghpvc/?username=ravimehta251&color=20C20E&style=flat-square&label=REQUESTS+SERVED" alt="profile views"/>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:20C20E&height=100&section=footer" width="100%" alt=""/>
</p>
