---
title: Carepilot Dashboard
layout: blog
icon: material/dev-to
tags: [python, streamlit, fastapi, sqlalchemy, pytest]
description: CarePilot is a personal project designed to help users record and track their health data over time. 
---
![cover](../assets/images/CarePilot_dashboard.png)

## Project Overview  

> CarePilot — Personal Health Tracker & Backend Sandbox

CarePilot is a solo-developed web application for recording and tracking personal health data over time. It supports metric input, goal setting, trend visualization, and data export. Beyond its practical use, the project serves as a technical sandbox for exploring backend architecture, authentication flows, and health data standards such as FHIR.

---

## Role & Scope  
Sole developer and product owner of the project. Led the full lifecycle from architecture design and feature implementation to testing, deployment, and roadmap planning. The project was designed to validate backend patterns and health data interoperability in a modular, extensible environment.

---

### Tech Stack  

| Category     | Technologies Used                                      |
|--------------|--------------------------------------------------------|
| **Backend**  | FastAPI, SQLAlchemy, Pydantic, Redis, SMTP             |
| **Frontend** | Streamlit                                              |
| **Database** | PostgreSQL + Alembic                                   |
| **Data Analytics** | pandas (matplotlib)                              |
| **DevOps**   | Docker, multi-env configuration                        |
| **Testing**  | Pytest                                                 |

---

## Key Challenges & Solutions  

- **Health Data Modeling & Interoperability**：Designed a scalable FastAPI backend with SQLAlchemy ORM and Pydantic schema validation, with planned support for FHIR conversion  
- **Authentication & Security**：Implemented JWT and OTP-based authentication with multi-environment support, Redis-backed session management for secure access  
- **Scalability & Maintainability**：Built a modular backend architecture with Alembic migrations and Dockerized environments for long-term extensibility  
- **Testing & Reliability**：Used pytest for unit testing and validation of core modules

---

## Software Development Lifecycle  

| Phase                   | Key Activities                                                                 |
|-------------------------|--------------------------------------------------------------------------------|
| **Initiation**          | - Defined scope: health tracking, authentication, backend sandbox<br>- Outlined core features and architecture goals |
| **Planning**            | - Selected tech stack: FastAPI, PostgreSQL, Streamlit<br>- Designed modular backend and multi-env setup |
| **Development & Testing** | - Built core modules: CRUD, auth, goal tracking<br>- Implemented pytest-based unit tests |
| **Release & Deployment** | - Dockerized app for local and cloud deployment<br>- Published documentation and usage examples |
| **Iteration & Impact**   | - Planned FHIR integration and MQTT support<br>- Continued refinement based on usage and architectural goals |

---

## Project Structure
The tool follows a modular architecture for maintainability and extensibility:

```
carepilot-dashboard/
├── backend/                      # FastAPI backend
│   ├── alembic/                  # Alembic migration scripts
│   │   ├── versions/
│   │   ├── env.py
│   │   ├── script.py.mako
│   ├── config/                   # Configuration settings
│   │   └── settings.py
│   ├── models/                   # ORM models
│   │   ├── user.py
│   │   └── umixin.py
│   ├── routers/                  # API route definitions
│   ├── schemas/                  # Pydantic schemas
│   │   ├── dailylog.py
│   │   ├── user.py
│   │   ├── profile.py
│   │   ├── goal.py
│   │   └── vitalsign.py
│   ├── services/                 # Business logic
│   ├── alembic.ini
│   ├── db.py                     # DB session and engine setup
│   └── main.py                   # FastAPI entry point
├── dashboard/                    # Frontend dashboard
├── tests/                        # Backend test cases
├── .gitignore                    # Git ignore rules
├── README.md                     # Project documentation
├── docker-compose.yml            # Docker orchestration
├── pyproject.toml                # Python project configuration
├── pytest.ini                    # Pytest configuration
└── uv.lock                       # Dependency lock file

```

**GitHub Repository**: [CarePilot Dashboard](https://github.com/maudes/carepilot-dashboard)

---

## Demo Video

<iframe width="100%" height="400" src="https://www.youtube.com/embed/vUQTXPYX7bw" frameborder="0" allowfullscreen></iframe>

<br>
