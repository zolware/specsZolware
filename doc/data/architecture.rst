==============
Project Layout
==============

|

.. comments

:Author(s):
   Francois Roy

:Date Created: 03-12-2017

:Language: None

:Status: :red:`Draft`

-----------


Basic Directory Structure
-------------------------

The following directorystructure is considered based on the template cookiecutter-django.

.. code-block:: bash

   .
   ├── .coveragerc
   ├── .editorconfig
   ├── .env
   ├── .git
   ├── .gitattributes
   ├── .gitignore
   ├── .travis.yml
   ├── CMakeLists.txt
   ├── CONTRIBUTORS.txt
   ├── LICENSE
   ├── README.rst
   ├── zolwareCOM
   │   ├── __init__.py
   │   ├── data
   │   │   ├── admin.py
   │   │   ├── apps.py
   │   │   ├── forms.py
   │   │   ├── migrations
   │   │   ├── models.py
   │   │   ├── templatetags
   │   │   ├── tests
   │   │   ├── urls.py
   │   │   └── views.py
   │   ├── contrib
   │   └── market
   │   ├── media
   │   │   └── data
   │   ├── static
   │   │   ├── css
   │   │   ├── fonts
   │   │   ├── images
   │   │   ├── js
   │   │   └── sass
   │   ├── templates
   │   │   ├── 404.html
   │   │   ├── 500.html
   │   │   ├── account
   │   │   ├── base.html
   │   │   ├── data
   │   │   └── users
   │   ├── tests_functional
   │   └── users
   │       ├── adapters.py
   │       ├── admin.py
   │       ├── apps.py
   │       ├── migrations
   │       ├── models.py
   │       ├── tests
   │       ├── urls.py
   │       └── views.py
   ├── config
   │   ├── settings
   │   │   ├── citest.py
   │   │   ├── common.py
   │   │   ├── local.py
   │   │   ├── production.py
   │   │   └── staging.py
   │   ├── urls.py
   │   └── wsgi.py
   ├── docs
   │   ├── CMakeLists.txt
   │   ├── conf.py
   │   ├── deploy.rst
   │   ├── index.rst
   │   ├── install.rst
   │   └── make.bat
   ├── manage.py
   ├── publish-key.enc
   ├── pytest.ini
   ├── requirements
   │   ├── base.txt
   │   ├── citest.txt
   │   ├── local.txt
   │   ├── production.txt
   │   └── staging.txt
   └── setup.cfg

The different component are explained below:

.. todo::
  Comment the different components.

