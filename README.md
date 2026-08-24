# Hey, I'm Albin Joseph 👋

> ⚠️ **Note:** My primary GitHub account is currently under review. This is my temporary account, and only my recent projects and contributions are being mirrored here while GitHub Support resolves it. The experience and projects below are real and actively maintained.

---

## About Me

Full Stack Software Engineer with **3 years of experience** building scalable backend systems, distributed applications, real-time platforms, and AI-powered applications using **Node.js, TypeScript, React, Python, and modern AI tooling**.

I've worked on production systems involving **microservices, multi-tenant SaaS, event-driven architecture, WebSockets, concurrent workflows, real-time bidding, geospatial systems, caching, and asynchronous messaging**.

More recently, I've been building **AI-native applications**, including a production-oriented **AI Voice Receptionist** using streaming speech-to-text, LLM reasoning, text-to-speech, RAG, vector databases, tool calling, and LangGraph-based agent workflows.

I enjoy solving problems where the interesting part isn't just making an API work, but designing the system behind it — handling **concurrency, failures, real-time events, scalability, consistency, and performance**.

📍 Bengaluru, India  |  📧 [albiejosephs101@gmail.com](mailto:albiejosephs101@gmail.com)  |  💼 [LinkedIn](https://linkedin.com/in/)  |  ✍️ [Medium](https://medium.com/@albiejosephs101)

---

## 🛠 Tech Stack

| Layer              | Technologies                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------- |
| **Languages**      | JavaScript, TypeScript, Python                                                                    |
| **Backend**        | Node.js, Express.js, NestJS, FastAPI, REST APIs, Microservices                                    |
| **Architecture**   | Distributed Systems, Event-Driven Architecture, Saga Patterns, Async Workflows, Multi-Tenant SaaS |
| **Real-time**      | WebSockets, Socket.IO, RabbitMQ, Redis Pub/Sub                                                    |
| **Databases**      | MongoDB, PostgreSQL, Redis, ChromaDB                                                              |
| **AI / LLM**       | LangChain, LangGraph, RAG, Embeddings, Vector Search, Tool Calling, AI Agents                     |
| **Voice AI**       | Deepgram, ElevenLabs, Streaming STT/TTS, WebSockets                                               |
| **Frontend**       | React.js, Next.js, Redux, Redux Toolkit, Zustand, Tailwind CSS, shadcn/ui                         |
| **Cloud / DevOps** | Docker, Kubernetes, NGINX, AWS S3, AWS EC2, Git                                                   |
| **Integrations**   | Stripe, Razorpay, Twilio, Google OAuth 2.0, WhatsApp Business API, Google Maps API, ZegoCloud     |

---

# 🚀 Featured Projects

## ☁️ CloudTrack — Multi-Tenant Logistics SaaS Platform

> **Production system at Cloudesign Technology Services · Jul 2024 – May 2026**

CloudTrack is a multi-tenant B2B logistics platform that I worked on for approximately two years. I contributed across the backend architecture and independently owned multiple production modules.

The platform involved **microservices, asynchronous communication, real-time tracking, financial workflows, auctions, notifications, and high-frequency operational APIs**.

### Key Engineering Highlights

* **Microservices Architecture** — contributed to the migration/re-architecture of a legacy monolith into independently deployable services including Trip, IAM, Master, Billing, Communication, and API Gateway components.

* **Trip Management System** — designed and implemented APIs and workflows covering trip creation, driver/transporter assignment, status transitions, pickup verification, trip tracking, and operational dashboards.

* **Real-Time Trip Tracking** — implemented WebSocket-based communication for live driver/location updates and integrated external GPS tracking sources for truck location data.

* **Real-Time Auction Engine** — built a WebSocket-driven auction system where multiple transporters could participate and submit bids concurrently for the same trip.

* **Concurrency Handling** — designed auction workflows around concurrent bid submissions, real-time state updates, bid ranking, and consistent auction state while multiple users interacted with the system simultaneously.

* **WhatsApp Auction Workflow** — extended the auction system beyond the web application with automated WhatsApp notifications, bid submission, and real-time rank/lowest-bid feedback.

* **RabbitMQ Event-Driven Communication** — implemented asynchronous communication between services for workflows such as organization creation, notification generation, and cross-service operations.

* **Redis Caching** — introduced caching on frequently accessed read-heavy APIs and implemented cache invalidation on relevant mutations.

* **Performance Optimization** — optimized database queries, indexes, aggregation pipelines, and caching strategies, reducing latency on critical dashboard and trip APIs by approximately **40–60%**.

* **Communication Platform** — worked on a dedicated communication service supporting **WhatsApp, Email, SMS, and Push notifications**, including templates, channels, and communication logs.

* **Billing & Agreements** — implemented backend workflows for billing, invoicing, and agreement/contract management.

### Stack

**Node.js · NestJS · TypeScript · MongoDB · Redis · RabbitMQ · WebSockets · Twilio · AWS · Docker**

---

## 🤖 VoicePilot AI — Production-Oriented AI Voice Receptionist

> **AI-powered voice agent for real-time phone conversations**

VoicePilot AI is a production-oriented AI Voice Receptionist that I'm building to understand the architecture behind real-time voice agents rather than simply wrapping an LLM API.

The system processes conversations through a streaming pipeline:

**Speech → Speech-to-Text → Agent/LLM → Tools/RAG → Text-to-Speech → Voice**

### Key Engineering Highlights

* **Real-Time Voice Pipeline** — implemented streaming communication using WebSockets and Deepgram for speech transcription.

* **LangGraph Agent Architecture** — designed a stateful agent workflow with separate nodes for memory, routing, tools, and answer generation.

* **RAG Pipeline** — implemented document retrieval using embeddings and ChromaDB to provide the agent with relevant company knowledge.

* **Conversation Memory** — designed conversation state and memory handling so the agent can maintain context across multiple turns.

* **Tool Calling** — designed the architecture for agents to invoke external actions instead of relying only on generated text.

* **Vector Search** — integrated embeddings and semantic search for retrieving relevant knowledge before generating responses.

* **Streaming Architecture** — designed the system around low-latency, event-driven communication rather than traditional request/response AI APIs.

* **Observability** — working toward structured logging, metrics, Redis-backed state, and production monitoring using Prometheus.

### Planned / Integrated Components

**Python · FastAPI · LangGraph · LangChain · ChromaDB · Redis · WebSockets · Deepgram · ElevenLabs · Docker · Prometheus**

🔗 [View VoicePilot AI](https://github.com/albiejodev/VoicePilot-AI_Backend)

---

## 📝 Collaborative AI Document Editor

> **AI-native collaborative document platform**

Built a collaborative document editing application as a full-stack engineering project with an emphasis on **real-time collaboration, backend architecture, and AI-assisted workflows**.

### Key Engineering Highlights

* Designed a full-stack application with separate frontend and backend services.
* Implemented collaborative document workflows and real-time state synchronization.
* Added AI-assisted document operations and structured AI workflows.
* Designed the application architecture around clear separation between frontend, backend, AI workflows, and persistence.
* Documented system architecture and AI workflow decisions.
* Focused on building the application as an **AI-native product rather than simply adding an AI chatbot to an existing application**.

**Stack:** React · TypeScript · Node.js · MongoDB · AI/LLM APIs

---

## 🚗 RideFlow — Ride-Sharing Backend

> **Distributed ride-hailing backend inspired by Uber**

RideFlow is a microservices-based ride-sharing backend designed to explore **distributed systems, geospatial queries, service communication, concurrency, and transactional workflows**.

The system consists of independent services for:

**API Gateway · IAM · Driver · Geo · Matching · Trip · Payment**

### Key Engineering Highlights

* **Driver Matching Engine** — supports sequential and parallel driver offers, configurable timeouts, automatic radius expansion, and candidate caching.

* **Geospatial Matching** — uses MongoDB 2dsphere indexes to efficiently locate nearby drivers.

* **Trip State Machine** — handles lifecycle transitions such as `REQUESTED → ASSIGNED → STARTED → COMPLETED/CANCELLED`.

* **Payment Idempotency** — uses idempotency keys to prevent duplicate payment operations during retries or network failures.

* **Distributed Communication** — services communicate asynchronously using RabbitMQ.

* **Billing Saga** — trip completion triggers downstream billing and payment workflows through event-driven communication.

* **Concurrency & Consistency** — designed state transitions and payment operations to remain safe under retries and concurrent requests.

* **Surge Pricing** — demand/supply-based pricing with cached pricing rules and server-authoritative fare calculation.

### Stack

**NestJS · RabbitMQ · MongoDB · PostgreSQL · Redis · Docker · TypeScript**

🔗 [View RideFlow GitHub Organization](https://github.com/Rideflow-ride-sharing)

---

# ⚡ Systems I've Worked On

Some of the engineering problems I've worked with:

### Real-Time Systems

* WebSocket-based live tracking
* Real-time auctions and bidding
* Concurrent users submitting state-changing operations
* Live driver/location updates
* Real-time communication workflows

### Distributed Systems

* Microservice decomposition
* RabbitMQ-based asynchronous communication
* Event-driven architecture
* Service-to-service workflows
* Saga-style distributed transactions
* Retry and failure handling

### Concurrency

* Concurrent auction bidding
* Atomic state transitions
* Idempotent payment operations
* Duplicate event/request prevention
* Race-condition-aware workflows
* Consistent state across asynchronous operations

### Performance

* MongoDB indexing
* Aggregation pipeline optimization
* Redis caching
* Cache invalidation
* Read-heavy API optimization
* Reducing API latency by **40–60%** on critical production routes

### AI Engineering

* RAG pipelines
* Embeddings and vector search
* LangGraph agent workflows
* Tool calling
* Conversation memory
* Streaming AI pipelines
* Speech-to-text / text-to-speech
* Real-time voice agents

---

# 🛍 Other Projects

| Project         | Description                                                                 | Stack                                                 |
| --------------- | --------------------------------------------------------------------------- | ----------------------------------------------------- |
| **Event Crest** | Vendor booking platform with real-time chat, payments, and live streaming   | React, Node.js, MongoDB, Socket.IO, Stripe, ZegoCloud |
| **Denim Store** | Full-stack e-commerce platform with admin dashboard and payment integration | Node.js, Express, MongoDB, EJS, Razorpay              |

---

# ✍️ Technical Writing

I write about **backend engineering, system design, distributed systems, AI engineering, and software architecture** on Medium.

👉 [medium.com/@albiejosephs101](https://medium.com/@albiejosephs101)

---

# 📚 Education

* **MERN Stack Development** — Brototype, Ernakulam (2023–2024)
* **BCA — Bachelor of Computer Application** — Mahatma Gandhi University (2017–2020)

---

## 🎯 What I Like Building

```text
Distributed Systems
       ↓
Microservices + Event Driven Architecture
       ↓
Real-Time Systems + Concurrency
       ↓
Scalable APIs + Data Systems
       ↓
AI Agents + RAG + Voice AI
       ↓
Production-Grade AI Applications
```

I'm particularly interested in engineering problems at the intersection of **backend systems, distributed architecture, real-time applications, and AI**.

---

*Primary account under review — this account is active while the issue is being resolved.*
