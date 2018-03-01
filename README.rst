=======================================
Fachschaftsempfaenger Production Config
=======================================

.. image:: https://img.shields.io/github/license/fsi-tue/fse-production.svg
    :target: https://github.com/fsi-tue/fse-production/blob/master/LICENSE.txt

.. image:: https://img.shields.io/badge/python-3-green.svg
    :target: https://www.python.org/

.. image:: https://img.shields.io/badge/django-2.0-green.svg
    :target: https://www.djangoproject.com/

This repository contains the nginx configuration files for running the
*fachschaftsempfaenger* application of the student union of Computer Science at
the university of Tuebingen in production.

Quickstart
==========

1. Install *fachschaftsempfaenger* via ``pip``:

.. code-block:: bash

    pip install git+https://github.com/fsi-tue/fachschaftsempfaenger

2. Make the migrations to adapt the database scheme locally:

.. code-block:: bash

    python manage.py migrate
    python manage.py makemigrations fachschaftsempfaenger
    python manage.py migrate fachschaftsempfaenger


3. Define a superuser to access the Django admin:

.. code-block:: bash

    python manage.py createsuperuser


4. Start a local server:

.. code-block:: bash

    python manage.py runserver

5. Open a browser and go to http://127.0.0.1:8000/
