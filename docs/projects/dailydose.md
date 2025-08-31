---
title: DailyDose Web Application
layout: blog
icon: material/dev-to
tags: [python, flask, sqlalchemy, git]
description: Joined the fCC Hackathon as a backend developer
---
![Image](../assets/images/dd_dashboard.png)

## Project Overview  

> DailyDose — Mindfulness Web App Built for Hackathon Delivery

Developed a full-featured web application promoting emotional well-being through personalized affirmations and community features. Built during the freeCodeCamp Hackathon (July 2025) under a four-week delivery timeline, the platform includes core user flows and a robust admin system, delivered by a newly assembled international team working remotely.

---

## Team Composition & My Role  

| Role                     | Responsibility                                                  |
|--------------------------|------------------------------------------------------------------|
| **Project manager (Myself)** | Project management, Sprint planning, Product specification  |
| **Backend Developers (4, incl. myself)**  | Designed and implemented core server-side modules, ensured data integrity, and supported frontend integration                      |
| Frontend Developers (5)  | UI/UX implementation, template integration                      |

---
### Tech Stack  

| Category     | Technologies Used                                      |
|--------------|--------------------------------------------------------|
| **Backend**  | Flask, SQLAlchemy, SMTP, Bcrypt                        |
| **Frontend** | Jinja                                                  |
| **Database** | PostgreSQL                                             |
| **DevOps**   | Docker                                                 |

---

## Key Challenges & Solutions  

- **Remote Collaboration Under Pressure**：Aligned workflows across a distributed team with no prior collaboration history  
- **Rapid Scope & Codebase Management**：Delivered a scalable backend and admin system within four weeks, balancing speed and maintainability  

---

## Key Contributions & Impact  

- **Backend Module Delivery**：Built `user_settings.py`, `admin/user.py`, and `admin/dashboard.py` for account management and analytics  
- **User Operations**：Implemented core CRUD flows and partial password reset functionality  
- **Integration Testing**：Designed and executed backend–frontend integration tests to ensure seamless interaction  
- **Project Coordination**：Contributed to task breakdown, progress tracking, and technical issue resolution  
- **Scalable Architecture**：Helped design a modular Flask + SQLAlchemy backend for future extensibility  

---

## Software Development Lifecycle  

| Phase                   | Key Activities                                                                 |
|-------------------------|--------------------------------------------------------------------------------|
| **Initiation**          | - Defined MVP scope: affirmations, user management, analytics<br>- Assigned tasks and timeline |
| **Planning**            | - Selected Flask + PostgreSQL<br>- Designed modular architecture and API interfaces |
| **Development & Testing** | - Built backend controllers and business logic<br>- Resolved API inconsistencies and query optimizations |
| **Release & Deployment** | - Used Docker for environment setup<br>- Deployed collaboratively to cloud platform |
| **Iteration & Validation** | - Conducted internal testing and feature validation<br>- Designed for future scalability |

---

## Project Structure Overview  
Relevant backend components I contributed to:

```
indigo-class/
├── app/
│   ├── controllers/
│   │   ├── root.py          
│   │   ├── auth.py          
│   │   ├── affirmations.py  
│   │   ├── categories.py    
│   │   ├── user.py          # User routes  --> My Contribution
│   │   └── admin/                                        
│   │       ├── dashboard.py # Admin dashboard routes  --> My Contribution
│   │       └── user.html    # Admin user management routes  --> My Contribution
│   ├── static/               
│   └── templates/               
├── main.py                   
├── pyproject.toml           
├── Dockerfile                
├── docker-compose.yml        
└── README.md                 
```

**GitHub Repository**: [DailyDose – indigo-class](https://github.com/freeCodeCamp-2025-Summer-Hackathon/indigo-class)

---

<div class="card-grid">

  <a href="./" class="card-item-wrapper"> <div class="card-image">
      <img src="/cv/assets/images/app_view.png" alt="DailyDose App View">
      <div class="caption"> DailyDose App View</div>
      <div class="tags"> #user_view </div>
    </div>
  </a> <a href="./" class="card-item-wrapper"> <div class="card-image">
      <img src="/cv/assets/images/dd_us.png" alt="DailyDose user stories">
      <div class="caption">User Stories</div>
      <div class="tags">#ux </div>
    </div>
  </a> </div>
