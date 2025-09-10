# Django + Django + PostgreSQL

## References

Django Girls のチュートリアル
https://tutorial.djangogirls.org/ja/

クィックスタート: Compose と Django
https://docs.docker.jp/compose/django.html


Python Anywhere
https://www.pythonanywhere.com/


WebSite
https://masarugotou.pythonanywhere.com/


## Build Container

```shell
docker compose build
```

## Create Project

django-admin startproject mysite .
<!-- docker-compose run web django-admin.py startproject mysite . -->

## Start Server
python manage.py runserver 0.0.0.0:8000

## Migration

python manage.py makemigrations blog
python manage.py migrate blog

## Create Admin User

python manage.py createsuperuser

## Deploy

pa_autoconfigure_django.py --python=3.12 https://github.com/marzg510/my-first-blog.git

or

git pull

## Command Shell

docker compose exec -it web python manage.py shell


#### Claude

apt install npm
npm install -g @anthropic-ai/claude-code


## Command Memo

pgsql
docker compose exec -it db psql mydb myuser

new project
docker-compose run web django-admin.py startproject composeexample .

Bootstrap
        <link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap.min.css">
        <link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap-theme.min.css">
