---
title: DailyDose Web Application
layout: blog
icon: material/dev-to
tags: [backend, python, flask, sqlalchemy, git]
description: Joined the fCC Hackathon as a backend developer
---

## Project Overview

This project was initiated as part of the freeCodeCamp Hackathon in July 2025, with a tight delivery timeline of just four weeks. Our team, composed of members from around the world, was tasked with building a fully functional web application from scratch.

We developed DailyDose, a platform designed to promote daily affirmations and positive self-talk—empowering users to cultivate mindfulness and emotional well-being through personalized content and community-driven features.

## Team Size

- Front-end developers: 4
- Back-end developers: 5 (*me)

## Challenges

- Delivered a fully functional web application with a built-in admin system in just 4 weeks, collaborating with an international team of newly assembled and unfamiliar members.
- Designing, grooming, and validating the project and codebase under tight timelines, while identifying optimal solutions or creative workarounds to ensure successful delivery.

## Tech Stacks & My Contribution

- **Virtual environment**: uv
- **Database**: PostgreSQL (SQLlite for testing)
- **Back-end**: Flask, sqlalchemy
- **Front-end**: Jinja, CSS, JS
- **Others**: Docker, Git

### Contribution

- Delivered `contronllers/admin_user.py` and `contronllers/user_settings.py`
    - Implemented core CRUD functionalities and partially developed the password reset flow to support essential user account operations.
- Others: Project management, Integration tests


```
indigo-class/
├── app/
│   ├── __init__.py          # Flask app factory
│   ├── controllers/
│   │   ├── root.py          # Root blueprint and routes
│   │   ├── auth.py          # Authentication blueprint and routes
│   │   ├── affirmations.py  # Affirmation blueprint and routes
│   │   ├── user_settings.py # User settings blueprint and routes
|   |   └── admin_user.py    # User blueprint and routes
│   ├── static/              # Static files (CSS, JS, images)
│   └── templates/           # HTML templates
│       ├── base.html a      # Base template
│       ├── _header.html     # Base template's header partial
│       ├── _footer.html     # Base template's footer partial
│       ├── home/
│       │   ├── index.html             # Home page template
│       ├── auth/
│       │   ├── register.html                 # Account registration template
│       │   ├── login.html                    # Login template
│       │   ├── profile.html                  # User profile template
│       │   ├── reset_password_request.html   # Password reset request template
│       │   └── new_password.html             # New password input template
│       ├── affirmations/*
│       ├── categories/*
│       └── admin/
│           ├── dashboard.html      # Admin dashboard template
│           ├── users.html          # Users management template
│           ├── affirmations.html   # Affirmation management template
│           ├── categories.html     # Categories management template
│           ├── analytics.html      # Analytics template
│           └── settings.html       # Admin settings template
├── main.py                  # Application entry point
├── pyproject.toml           # Project configuration
├── Dockerfile               # Instructions for building the Docker image
├── docker-compose.yml       # Requirements for building the Docker image
└── README.md                # This file
```

> [GitHub project: indigo-class/DailyDose ](https://github.com/freeCodeCamp-2025-Summer-Hackathon/indigo-class)


## Highlights

- Successfully delivered key backend modules—including admin user and user settings controllers—entirely from scratch, ensuring modularity and maintainability.
- Designed scalable backend architecture with Flask and SQLAlchemy, enabling smooth integration with front-end templates and future feature expansion.
- Coordinated backend development across a newly formed international team, aligning workflows and resolving blockers under tight deadlines.

<br>
