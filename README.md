# Django Polls App

Django polls app (parts 1–4), deployed to AWS EB; visit /polls.

## Quick Start

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

## EB Deploy

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
