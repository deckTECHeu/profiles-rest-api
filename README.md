# Profiles REST API

docker-compose run app sh -c "django-admin.py startproject profiles_project ."
docker-compose run app sh -c "python manage.py startapp profiles_api"
docker-compose run app sh -c "python manage.py test && flake8"