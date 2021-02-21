# Profiles REST API

docker-compose run --rm app sh -c "django-admin.py startproject app ."
docker-compose run --rm app sh -c "python manage.py startapp api"
docker-compose run --rm app sh -c "python manage.py makemigrations api"
docker-compose run --rm app sh -c "python manage.py migrate"
Add to settings.py:
    'rest_framework',
    'rest_framework.authtoken',
    'api',
docker-compose run app sh -c "python manage.py test && flake8"