# Hey, I'm Albin Joseph 👋

> ⚠️ **Note:** My primary GitHub account is currently under review. This is my temporary account, and only my recent projects and contributions are being mirrored here while github support resolves it. The experience and projects below are real and actively maintained.

---

## About Me

Full stack Software Engineer with **3 years** building scalable, distributed systems in **Node.js , React & TypeScript**. I've re-architected monolithic platforms into microservices-based SaaS products, designed real-time systems, event-driven workflows, and full trip/ride lifecycle engines — both in production and as independent projects.

I enjoy owning backend modules end-to-end — from API design to deployment — with a strong interest in **system design and high-throughput API architecture**. Working knowledge of React for full-stack support in lean teams.

📍 Bengaluru, India &nbsp;|&nbsp; 📧 albiejosephs101@gmail.com &nbsp;|&nbsp; 💼 [LinkedIn](https://linkedin.com/in/) &nbsp;|&nbsp; ✍️ [Medium](https://medium.com/@albiejosephs101)

---

## 🛠 Tech Stack

| Layer | Technologies |
|---|---|
| **Languages** | JavaScript, TypeScript |
| **Backend** | Node.js, Express.js, NestJS, RESTful APIs, Microservices, Event-Driven Architecture |
| **Real-time** | WebSockets, Socket.IO, RabbitMQ |
| **Databases** | MongoDB (Geospatial), PostgreSQL, Redis |
| **Frontend** | React.js, Redux, Redux-Toolkit, Tailwind CSS, shadcn/ui |
| **DevOps** | Docker, Kubernetes, NGINX, AWS (S3, EC2), Git |
| **Integrations** | Stripe, Razorpay, Twilio, Google OAuth 2.0, WhatsApp Business API, ZegoCloud |

---

## 🚀 Featured Projects

### 🚗 RideFlow — Ride-Sharing Backend (Microservices)
> Production-grade distributed backend for a ride-hailing platform

A fully event-driven ride-hailing backend built as **7 independent NestJS microservices** — API Gateway, IAM, Driver, Geo, Matching, Trip, and Payment — each owning its own database and communicating via RabbitMQ.

**Key Engineering Highlights:**
- **Driver Matching Engine** — sequential and parallel offer modes, configurable 15s per-driver timeouts, automatic radius expansion on no-match, and short-lived geospatial candidate caching
- **Trip Lifecycle State Machine** — `REQUESTED → ASSIGNED → STARTED → COMPLETED/CANCELLED` with OTP-based pickup verification and atomic state transitions
- **Billing Saga** — event choreography where `trip.completed` triggers auto-invoicing; `payment.completed` updates trip state — with idempotent handlers and Dead-Letter Queue (DLQ) fallback
- **Geo Service** — MongoDB 2dsphere geospatial indexing for real-time nearby driver queries, synced via async `driver.went_online/offline` events
- **Surge Pricing** — TTL-based rule caching, demand/supply ratio sampling, and server-authoritative fare settlement to prevent client-side manipulation
- **Replay-resistant design** — JWT auth, idempotency keys on all mutation endpoints, request timestamp skew enforcement at the gateway

**Stack:** NestJS · RabbitMQ · MongoDB · PostgreSQL · Redis · Docker · TypeScript

🔗 [View RideFlow GitHub Organization](#) *(https://github.com/Rideflow-ride-sharing)*

---

### ☁️ CloudTrack — Multi-Tenant Logistics SaaS Platform
> Production system at Cloudesign Technology Services (Jul 2024 – May 2026)

Re-architected a legacy monolithic logistics platform into a scalable, **multi-tenant B2B SaaS product** — independently owning backend development across all major modules.

**Key Engineering Highlights:**
- **Trip Management System** — trip creation, driver assignment, OTP-based pickup verification, status lifecycle transitions, and integration with planning, billing, and agreement modules
- **Real-time Trip Tracking** — dual-mode location accuracy using WebSocket-based driver app integration and SIM-based GPS via Twilio for live truck location updates
- **Auction/Bidding Engine** — real-time WebSocket-based system enabling transporters to compete live for trip assignments with concurrent user participation
- **WhatsApp-native Auction Workflow** — automated bid notifications, bid submission via chat, and real-time rank/lowest-bid feedback for non-web transporter networks
- **Redis Caching** — integrated across high-frequency read paths, reducing API latency by **40–60%** on trip status, driver, and agreement data in production
- **Financial Workflows** — end-to-end Billing & Invoicing module and Agreement/Contract management covering the full logistics operational lifecycle

**Stack:** NestJS · Node.js · TypeScript · Redis · WebSockets · MongoDB · Twilio · Docker

---

### 🛍 Other Projects

| Project | Description | Stack |
|---|---|---|
| **Event Crest** | Vendor booking platform with real-time chat, payments, and live streaming | React, Node.js, MongoDB, Socket.IO, Stripe, ZegoCloud |
| **Denim Store** | Full-stack e-commerce platform with admin dashboard and payment integration | Node.js, Express, MongoDB, EJS, Razorpay |

---

## ✍️ Technical Writing

I write about backend engineering, system design, and software architecture on Medium.
👉 [medium.com/@albiejosephs101](https://medium.com/@albiejosephs101)

---

## 📚 Education

- **MERN Stack Development** — Brototype, Ernakulam (2023–2024)
- **BCA — Bachelor of Computer Application** — Mahatma Gandhi University (2017–2020)

---

*Primary account under review — this account is active while the issue is being resolved.*
