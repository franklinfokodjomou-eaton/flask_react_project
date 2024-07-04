python3 -m venv venv
source venv/bin/activate
pip install django
pip install djangorestframework
django-admin startproject admin .
cd admin
python3 manage.py runserver
django-admin startapp quickstart
cd ..

docker compose exec backend sh
  python manage.py startapp products
  python manage.py makemigrations
  python manage.py migrate

