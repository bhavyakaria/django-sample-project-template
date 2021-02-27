# Django Sample Project Template

`mysite/`
* It's the root directory for our project.
* It's name doesn't matter to Django.

`manage.py`
* Command Line utility which helps to interact with Django project in various ways.

inner `mysite/`
* Actual Python package for our project.

`mysite/__init__.py`
* Empty file which tells Python that this directory should be considered a Python package.

`mysite/settings.py`
* Settings/configuration for this Django project.

`mysite/urls.py`
* URL declarations for this Django project.
* Kind of Index for your site.

`mysite/asgi.py`
* Entry point for ASGI-compatible web servers to serve your project.

`mysite/wsgi.py`
* Entry point for WSGI-compatible web servers to serve your project.

Pre-Installed Apps with Django
1. admin
2. auth
3. contenttypes
4. sessions
5. messages
6. staticfiles

### Some of the apps make use of at least one database table and for that reason we need to run below command.
```
python manage.py migrate
```

The above commands looks at the *INSTALLED_APPS* in `settings.py` and creates required databases.

Notes:
* By default, django comes with a pre configured database(sqlite)
* Django follows the DRY principle.
* 