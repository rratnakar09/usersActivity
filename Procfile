release: python3 -m venv env
release: pip install -r requirements.txt
release: python manage.py makemigrations --no-input
release: python manage.py migrate --no-input

web: gunicorn activityTracker.wsgi.py
