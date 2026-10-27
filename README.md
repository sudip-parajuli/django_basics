# Django Fundamentals Practice

An early Django learning project exploring URL routing, view functions,
templates, models and the admin interface. The application is named `polls`,
but the implemented pages are introductory home, about and contact exercises.

## Project layout

- `DjangoTutorial/` — project settings, root URL configuration, ASGI and WSGI.
- `polls/` — application views, models, migrations and templates.
- `manage.py` — Django's development commands.

## Run locally

The original project was generated with Django 5.1.4. To reproduce the historical
learning environment, use a virtual environment with Python 3.11:

```sh
python -m venv .venv
```

Activate `.venv\Scripts\Activate.ps1` in PowerShell or
`source .venv/bin/activate` on macOS/Linux, then:

```sh
python -m pip install Django==5.1.4
python manage.py migrate
python manage.py runserver
```

Open `http://127.0.0.1:8000/polls/`, `/polls/about/` or `/polls/contact/`.
Create an administrator with `python manage.py createsuperuser` to use `/admin/`.

## Scope

This is a historical local-development exercise. The settings contain development
defaults, and the original tree includes a SQLite database and generated cache
files. Back up or use a separate copy of the database before experimenting.
The placeholder test file is not an automated regression suite. Modernizing
dependencies, repository hygiene and deployment configuration remain future work.

My later [DRF internship project](https://github.com/sudip-parajuli/drftutorial)
demonstrates authentication, permissions and tested API examples.
