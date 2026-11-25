# Hi, I'm Olamide 👋

### Full-Stack & Distributed Systems Engineer

I'm a Computer Engineering undergraduate at the University of Lagos, building web applications, reliable APIs, database-backed services, and distributed systems.

I enjoy working across the stack—from browser interfaces and API design to transactional data integrity, message processing, and infrastructure reliability.

## 🛠️ Engineering stack

| Area | Technologies |
| --- | --- |
| Frontend | React, JavaScript, HTML, CSS |
| Backend & systems | Python, FastAPI, C++17, REST APIs |
| Data | PostgreSQL, SQLite |
| Infrastructure | Docker, Apache Kafka, AWS, GitHub Actions |
| Practices | Automated testing, CI/CD, concurrency, authentication, fault tolerance |

## 🚀 Featured work

### [LedgerFlow — Full-Stack Financial Ledger](https://github.com/olabs123-hue/LedgerFlow.)
**React · FastAPI · PostgreSQL · Authentication · CI**

A fictional financial-ledger prototype investigating safe concurrent transfers, idempotency, double-entry journals, and browser session security.

- [Public React showcase](https://ledgerflow-showcase-olabs123.onrender.com) uses **browser-local demo data**, not a live transactional backend.
- A separate read-only API staging service exposes health/readiness endpoints.
- The interactive transfer experience is tested in isolated HTTPS CI; public transactions are **not enabled**.
- **Measured fictional-transfer benchmark:** [82.29 transfers/s with 4 workers](https://github.com/olabs123-hue/LedgerFlow./blob/main/PHASE3_REPORT.md), **68.17 ms p95** on 100 persisted transfers in a single runner-local FastAPI TestClient + PostgreSQL CI comparison; not public-service load testing.

### [InfraPulse — Full-Stack Infrastructure Monitoring](https://github.com/olabs123-hue/Infrapulse)
**React · TypeScript · FastAPI · SQLite · Docker**

A standalone observability lab with health samples, latency charts, token-protected metric ingestion, threshold-based incident detection, and a read-only dashboard. The [read-only dashboard is live on Render](https://infrapulse-readonly-olabs123.onrender.com); the frontend and Docker production builds passed during deployment. Public metric ingestion is disabled.

### [MarketStream — Real-Time Market Data Simulation](https://github.com/olabs123-hue/MarketStream)
**React · TypeScript · FastAPI · WebSockets · C++17**

A [live simulated trading terminal](https://marketstream-sim-olabs123.onrender.com) featuring fictional WebSocket prices, synthetic order-book depth, stateful C++17 order-book processing, sequence validation, normalized simulated sources, and bounded SQLite observation history. Backend/native tests and Docker builds run in CI.

- **Measured internal performance:** [138,388.83 in-process Python fanout enqueue calls/s](https://github.com/olabs123-hue/MarketStream/actions/runs/45190849808) at p95 **7.493 µs** (20 bounded subscriber queues; not network/WebSocket delivery latency).
- **Synthetic source-recovery test:** [200/200 successful simulated failover selections](https://github.com/olabs123-hue/MarketStream/actions/runs/45196355759), p95 **2.964 µs** for local synchronous selection (not external source recovery time).

### [SentinelAI — Explainable Security Monitoring](https://github.com/olabs123-hue/SentinelAI)
**Python · FastAPI · SQLite · Browser dashboard**

A defensive security monitoring MVP with event ingestion, rule-based incident detection, explainable summaries, and an incident triage dashboard. This is a local demo, not a production security platform or trained AI model.

### [Distributed Real-Time Event Processing](https://github.com/olabs123-hue/distributed-event-processing)
**C++17 · Kafka · PostgreSQL · Docker**

Message-driven event processing with Kafka consumers, idempotent persistence, observability, and failure-recovery testing. The repository distinguishes serialization benchmarks from end-to-end ingestion performance.

- **Measured batch scaling:** [5,000 synthetic events per configuration](https://github.com/olabs123-hue/distributed-event-processing/actions/runs/45601157117); **1,025 → 1,575 persisted events/s** from **1 to 3 active database-writing workers** (~**54% improvement**) in one GitHub Actions run (4 consumers configured, 3 partitions).
- **Measured event age at PostgreSQL insert (3 active writers):** **896 ms p50 / 1,438 ms p99**. Synthetic container benchmark; not client acknowledgment latency or production throughput.
- **Recovery evidence:** [10,000 unique IDs + 2,500 replayed IDs](https://github.com/olabs123-hue/distributed-event-processing/actions/runs/44302567380), with no missing or duplicate persisted rows after worker/database disruptions.

### [AtlasKV — Transactional Key-Value Store](https://github.com/olabs123-hue/AtlasKV-Transactional-Database)
**C++17 · MVCC · Transactions · Indexing**

An educational transactional storage engine with historical reads, optimistic validation, secondary indexing, and reproducible tests. Not a production distributed database.

### [Autonomous Network Reliability](https://github.com/olabs123-hue/autonomous-network-reliability)
**Python · FRRouting · Containerlab · Prometheus · Grafana**

A network reliability lab exploring dynamic routing, fault injection, observability, and automated recovery validation.

### [DSA Grind — Algorithm Practice](https://github.com/olabs123-hue/dsa-grind)
**Python · Data Structures · Algorithms**

- **27 publicly inspectable Python solution files** verified from the GitHub repository tree on 25 November 2026, covering hashing, arrays, two pointers, sliding windows, trees, graphs and dynamic programming.
- [Browse the solutions](https://github.com/olabs123-hue/dsa-grind/tree/main/python) · [Evidence and contest tracker](https://github.com/olabs123-hue/dsa-grind/blob/main/PROGRESS.md). Source-file count is **not** an accepted-online-judge submission count; no contest rating is claimed.

## 🔭 Current focus

- Building polished, accessible frontend experiences that connect to secure backend APIs
- Designing reliable data processing services and transactional systems
- Improving automated testing, observability, security, and deployment practices

## 📫 Connect

- [GitHub projects](https://github.com/olabs123-hue)

_I'm interested in software engineering internships and opportunities to collaborate on practical engineering projects._
