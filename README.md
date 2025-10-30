# Django Polls App

[![Build Status](https://github.com/nicknikac/swe-app1/workflows/Django%20CI%2FCD/badge.svg)](https://github.com/nicknikac/swe-app1/actions)
[![Coverage Status](https://coveralls.io/repos/github/nicknikac/swe-app1/badge.svg?branch=main)](https://coveralls.io/github/nicknikac/swe-app1?branch=main)

Django polls app (parts 1–4), deployed to AWS EB.

## 🌐 Live URLs
- **Polls App:** https://swe-app1-env.eba-dpznhkqv.us-east-2.elasticbeanstalk.com/polls/
- **Admin Interface:** https://swe-app1-env.eba-dpznhkqv.us-east-2.elasticbeanstalk.com/admin/

## 👤 Admin Credentials
- **Username:** admin
- **Password:** adminpass123!

## Quick Start (Local Development)

1. Create virtual environment:
   ```bash
   python -m venv .venv
   # Windows PowerShell: .\.venv\Scripts\Activate
   # WSL/macOS: source .venv/bin/activate
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run migrations:
   ```bash
   python manage.py migrate
   ```

4. Create superuser:
   ```bash
   python manage.py createsuperuser
   ```

5. Run development server:
   ```bash
   python manage.py runserver
   ```

6. Visit http://127.0.0.1:8000/polls/

## 🚀 AWS Elastic Beanstalk Deployment

1. Configure AWS CLI:
   ```bash
   aws configure
   ```

2. Initialize EB:
   ```bash
   eb init
   ```

3. Create environment:
   ```bash
   eb create <env-name> --single
   ```

4. Deploy:
   ```bash
   eb deploy
   ```

5. Get URL:
   ```bash
   eb status
   ```

## 📝 Features
- Modern UI with animated progress bars
- Real-time vote counting
- Admin interface for managing polls
- Responsive design
- Secure deployment on AWS