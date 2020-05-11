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

Apply Database Migrations
> python manage.py migrate

> The migrate command looks at the INSTALLED_APPS setting and creates any necessary database tables according to the database settings in your mysite/settings.py file and the database migrations shipped with the app.


