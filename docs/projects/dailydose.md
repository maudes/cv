---
title: DailyDose Web Application
layout: blog
icon: material/dev-to
tags: [backend, python, flask, sqlalchemy, git]
description: Joined the fCC Hackathon as a backend developer
---

## Project Overview

This is the project from freeCodeCamp Hackathon.

## Team Size

- Front-end developers: 4
- Back-end developers: 5 (*me)

## Challenges

- Need to deliver a well-functioned web application with memeber system within 4 weeks with strangers.
- We need to design, groom, validate our codes closely and figure out the best way (or a workaround) to deliver successfully. 

## Tech Stacks & My Contribution

- Virtual environment: uv
- Database: PostgreSQL (SQLlite for testing)
- Back-end: Flask, sqlalchemy
- Front-end: Jinja
- Others: Docker, Git

```
indigo-class/
├── app/
│   ├── __init__.py          # Flask app factory
│   ├── controllers/
│   │   ├── root.py          # Root blueprint and routes
│   │   ├── auth.py          # Authentication blueprint and routes
│   │   ├── affirmations.py  # Affirmation blueprint and routes
│   │   ├── user_settings.py    # User settings blueprint and routes
|   |   └── admin_user.py          # User blueprint and routes
│   ├── static/              # Static files (CSS, JS, images)
│   └── templates/           # HTML templates
│       ├── base.html a      # Base template
│       ├── _header.html     # Base template's header partial
│       ├── _footer.html     # Base template's footer partial
│       ├── home/
│       │   ├── index.html             # Home page template
│       │   └── dashboard.html         # User dashboard template
│       ├── auth/
│       │   ├── register.html                 # Account registration template
│       │   ├── login.html                    # Login template
│       │   ├── profile.html                  # User profile template
│       │   ├── reset_password_request.html   # Password reset request template
│       │   └── new_password.html             # New password input template
│       ├── affirmations/
│       │   ├── index.html   # Affirmation list template
│       │   ├── add.html     # Affirmation submission template
│       │   └── edit.html    # Affirmation edit template
│       ├── categories/
│       │   ├── list.html    # Affirmation categeries list template
│       │   ├── add.html     # Affirmation category submission template
│       │   └── edit.html    # Affirmation category edit template
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

### Contribution

- Delivered `contronllers/admin_user.py` and `contronllers/user_settings.py`
- Others: Project management, Integration tests

> [GitHub project: indigo-class/DailyDose ](https://github.com/freeCodeCamp-2025-Summer-Hackathon/indigo-class)

## Highlights

- Most proud of

<br>
