<h1 align="center">🦷 Dentwise – Dental Platform with AI Voice Agent 🦷</h1>

A scalable SaaS platform targeting dental practices, built to automate, assist, or enhance dental workflows using AI and cloud-native architecture.

📖 Project Overview

This project aims to deliver a Software-as-a-Service (SaaS) platform tailored for dental clinics, integrating AI-powered features along with standard SaaS functionalities (multi-tenant support, user roles, subscription billing, etc.). The platform enables dentists to manage patients, run diagnostics, and access analytics — while leveraging AI to support decision-making and workflow optimisation.


![Demo App](/public/screenshot-for-readme.png)


Highlights:

- 🏠 Modern Landing Page with gradients & images
- 🔐 Authentication via Clerk (Google, GitHub, Email & Password)
- 🔑 Email Verification (6-digit code)
- 📅 Appointment Booking System
- 🦷 3-Step Booking Flow (Dentist → Service & Time → Confirm)
- 📩 Email Notifications for Bookings (Resend)
- 📊 Admin Dashboard for Managing Appointments
- 🗣️ AI Voice Agent powered by Vapi (Pro Plans only)
- 💳 Subscription Payments with Clerk (Free + 2 Paid Plans)
- 🧾 Automatic Invoices via Email
- 💸 Smart Subscription Upgrades (pay only the difference)
- 📂 PostgreSQL for Data Persistence
- 🎨 Styling with Tailwind CSS + Shadcn
- ⚡ Data Fetching with TanStack Query
- 🤖 CodeRabbit for PR Optimizations
- 🧑‍💻 Git & GitHub Workflow (branches, PRs, merges)
- 🚀 Deployment on Sevalla (free-tier friendly)

🛠 Tech Stack & Skills

Backend: Node.js / Express (or similar), REST APIs, authentication & authorization

Frontend: React / Angular / Vue (or any SPA framework) + UI library

AI/ML: TensorFlow/PyTorch or ML-served models, image processing, inference pipelines

Database: Postgres/MySQL (relational) + possibly MongoDB for semi-structured data

Multi-tenant SaaS architecture: Tenant isolation, role-based access, subscription layering

Cloud & DevOps: Docker, Kubernetes, CI/CD pipelines, cloud deployment (AWS/GCP/Azure)

Data security & compliance: Encryption, audit trails, HIPAA/GDPR considerations

Version control & collaboration: Git, GitHub

UI/UX: Design of intuitive dashboards for dentists, staff & patients

Key Skills: SaaS architecture · Multi-tenancy · REST APIs · AI/ML integration · Dental domain knowledge · Full-stack web development · Cloud deployment · Security & compliance · Database design · Dashboards & analytics

📁 Suggested Folder Structure
AI-Dentist-SaaS-Platform/
│
├── backend/                     # Backend services (APIs, business logic)
│   ├── src/
│   ├── models/
│   ├── routes/
│   └── services/
│
├── frontend/                    # Frontend application (clinic staff & patient portals)
│   ├── src/
│   ├── components/
│   └── assets/
│
├── ai-models/                   # AI/ML modules & inference code
│   ├── training/
│   ├── inference/
│   └── utils/
│
├── infra/                       # Infrastructure as code, deployment scripts
│   ├── docker/
│   ├── k8s/
│   └── ci-cd/
│
├── docs/                        # Project documentation, architecture diagrams
│   └── architecture.md
│
├── tests/                       # Automated tests (unit, integration, e2e)
│
├── .env.example                 # Environment variable specs
├── README.md                    # This documentation
└── LICENSE                      # License file


---

## 🧪 .env Setup

```bash
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key

DATABASE_URL=your_postgres_database_url

NEXT_PUBLIC_VAPI_ASSISTANT_ID=your_vapi_assistant_id
NEXT_PUBLIC_VAPI_API_KEY=your_vapi_api_key

ADMIN_EMAIL=your_admin_email

RESEND_API_KEY=your_resend_api_key

NEXT_PUBLIC_APP_URL=your_app_url

```

## Run the app



🚀 Getting Started
Prerequisites

Node.js (v14+) and npm/yarn

Docker & docker-compose (optional, for local environment)

Access to AI model binaries or prepared inference service

Installation & Running Locally
# Clone repo
git clone https://github.com/yashuyouwaraj/AI-Dentist-Saas-Platform.git
cd AI-Dentist-Saas-Platform

# Setup environment variables
cp .env.example .env
# Edit .env to configure database, AI service endpoint, tenant settings

# Install backend & frontend
cd backend
npm install
cd ../frontend
npm install

# Run services
# Option A: run independently
cd backend && npm run dev
cd ../frontend && npm run start

# Option B: using Docker (if docker-compose provided)
docker-compose up --build

Deployment

Use Docker images for each service

Use Kubernetes, AWS ECS or similar for scaling

Use managed PostgreSQL or MySQL for persistence

Use object storage for images

Set up monitoring/logging (Prometheus, Grafana, ELK)

✅ What’s Complete & MVP Scope

Core user roles & authentication

Patient management & clinic onboarding

Basic dashboard UI for clinic staff

AI diagnostics stub/service integration

Multi-tenant setup and subscription workflow

🚧 Planned Improvements / Roadmap

Full patient portal with treatment tracking & alerts

Advanced AI: dental image segmentation, risk prediction, 3D modelling

Interoperability: DICOM/HL7 integration, EHR export

Mobile app for patients & dentists

Real-time chat/tele-dentistry feature

Compliance certifications (HIPAA, ISO 27001)

Enhanced analytics: predictive retention, revenue forecasting

White-label deployment option and marketplace apps

🤝 Contributing

Contributions are welcome!

Fork the repository

Create a feature branch (git checkout -b feature/YourFeature)

Commit your changes (git commit -m "Add monthly revenue dashboard")

Push to your branch (git push origin feature/YourFeature)

Open a pull request describing your change

Please ensure contributions follow existing code style, include tests, and maintain backward compatibility.

🪪 License

This project is licensed under the MIT License (or whichever you choose). See LICENSE for details.

👤 Author

Yashu Youwaraj

```bash
1- npm install
2- npm run dev
```
