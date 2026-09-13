# FitFlow_RE_Design

FitFlow is a modern fitness application engineered to deliver a seamless user experience across iOS, Android, and Web platforms. The system supports personalized workout plans, nutrition tracking, social sharing, real-time updates, and AI-powered recommendations.

---

## 📁 Repository Structure

```text
├── ai-service/     # Python & FastAPI service for AI-powered fitness insights
├── backend/        # Node.js & NestJS backend API with WebSockets & Redis
├── docs/           # Architectural Decision Records, matrices, and system diagrams
│   ├── architecture-decision-record.md
│   ├── architecture-diagram.png
│   ├── backend-database-auth-comparison.md
│   ├── frontend-comparison.md
│   └── technology-comparison-matrix.md
├── frontend/       # Flutter cross-platform client (iOS, Android, Web)
├── .gitignore
└── README.md
```

---

## 🏗️ Architecture Overview

The system follows a modern multi-tiered distributed architecture:

- **Frontend Client Layer:** [Flutter](https://flutter.dev/) for cross-platform iOS, Android, and Web support.
- **Application Layer (Backend):** [NestJS](https://nestjs.com/) (Node.js) handling core business logic, user management, and real-time WebSockets.
- **AI Microservice:** [FastAPI](https://fastapi.tiangolo.com/) (Python) providing dedicated AI/ML model inference and workout/nutrition recommendations.
- **Caching Layer:** [Redis](https://redis.io/) for session store, fast in-memory caching, and low-latency data access.
- **Database Layer:** [PostgreSQL](https://www.postgresql.org/) for persistent relational data management.
- **Authentication & Identity:** [Firebase Auth](https://firebase.google.com/docs/auth) for unified identity management across mobile and web.

For detailed documentation, refer to the documents inside the [`docs/`](./docs/) directory.