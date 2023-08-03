Django-PostgreSQL Docker Training

This repository contains a simple Django application with PostgreSQL set up using Docker containers.

Setup

1. Clone the repository:

```bash
git clone https://github.com/khanZaki1/django-postgres-docker-training.git
```

2. Spin up the Docker containers:

```bash
docker-compose up -d --build
```
3. Connect to the Django container shell:
```bash
docker exec -it <container_name> /bin/sh
```
4. Run migrations to set up the database:
```bash
python manage.py makemigrations
python manage.py migrate
```
5. Create a superuser to access the Django admin panel:
```bash
python manage.py createsuperuser
```
6. Access the Django admin panel at:
```bash
http://localhost:8000/admin/
```
