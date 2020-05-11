# Sample Django Project

## Virtual Environment Setup

Install virtualenv command
> pip install virtualenv

Create virtual environment
> virtualenv -p python3 venv

Activate Virtualenv
> . venv/bin/activate

Install dependencies from requirements
> pip install -r requirements.txt

List dependencies
> pip freeze

To deactivate virtualenv
> deactivate 

## Starting with Django

Check Django Version
> python -m django --version

Initializing Django Project
> django-admin startproject mysite

Run the Project (Navigate to mysite directory)
> python manage.py runserver

Add a new app to the project
> python manage.py startapp app_name

Create Database Migrations
> python manage.py migrate

> The migrate command looks at the INSTALLED_APPS setting and creates any necessary database tables according to the database settings in your mysite/settings.py file and the database migrations shipped with the app.

Create Database Migrations for an App
> python manage.py makemigrations app_name

Apply Database Migrations
> python manage.py migrate

> The migrate command takes all the migrations that haven’t been applied (Django tracks which ones are applied using a special table in your database called django_migrations) and runs them against your database - essentially, synchronizing the changes you made to your models with the schema in the database.

