# Gyan Uday - Education Management System

## Overview
Gyan Uday is a comprehensive Django-based web application for managing educational institutions. It handles students, courses, attendance, fees, results, and dashboard functionalities.

## Features
- **Students**: CRUD operations, departments, faculties
- **Courses**: Enrollment, lists, details
- **Attendance**: Bulk marking, reports, summaries
- **Fees**: Structures, payments, details
- **Results**: Exams, bulk entry, student cards, activity logs
- **Dashboard**: Home view with API docs

## Tech Stack
- Backend: Django (REST API support with serializers)
- Frontend: HTML templates, Bootstrap CSS, vanilla JS
- Database: SQLite (dev), likely PostgreSQL (prod)
- Deployment: Heroku-ready (Procfile)

## Quick Start
1. Clone the repo:
   ```
   git clone https://github.com/Mithleshyadavgithub/bbd-project.git
   cd bbd-project
   ```
2. Create virtual environment:
   ```
   python -m venv venv
   source venv/bin/activate  # macOS/Linux
   ```
3. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
4. Copy env:
   ```
   cp .env.example .env
   ```
5. Run migrations:
   ```
   python manage.py makemigrations
   python manage.py migrate
   ```
6. Create superuser:
   ```
   python manage.py createsuperuser
   ```
7. Start server:
   ```
   python manage.py runserver
   ```
8. Access: http://127.0.0.1:8000/

## API Docs
Available at `/api/docs/` (Swagger-like).

## Deployment
- Heroku: `git push heroku main`
- Ensure `SECRET_KEY` in `.env`

## Project Structure
```
gyan_uday/          # Main Django project
accounts/           # User accounts
students/           # Student management
courses/            # Course handling
attendance/         # Attendance tracking
fees/               # Fee management
results/            # Result entry & reports
dashboard/          # Admin dashboard
static/             # CSS/JS
templates/          # HTML templates
```

Built with ❤️ for educational management.
