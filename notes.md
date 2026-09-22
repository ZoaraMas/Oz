## Initialisation du projet
docker compose build

docker compose run --rm app django-admin startproject config .

docker compose exec app python manage.py migrate

docker compose exec app python manage.py createsuperuser (root, ozisadmin)

App de test:
docker compose exec app python manage.py startapp employes
docker compose exec app python manage.py makemigrations
docker compose exec app python manage.py migrate
- 

## Liens utilis
http://localhost:8000/
http://localhost:8000/admin