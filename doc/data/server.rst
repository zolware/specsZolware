========================
Data Service Application
========================

|

.. comments

:Author(s): Francois Roy, Simon Clucas

:Date Created: 03-11-2017

:Language: C++

:Status: :red:`Draft`

-----------

Description
-----------

The signal emulator service is a web application with the following component:

- A home page with a menu bar
- A sign In/Sign Up interface
- An interface to connect to data streams sent by sensors
- A database containing users (static) data --> can be updated in real time
- A tool to manage dtabase storage (maximum size, download data, delete data) 
- A sensor emulator interface that simulates different type of sensors
- A profile page
- A space to connect with other users
- A User settings interface
- An web admin interface

Proposed Technology
-------------------

- Coding languages: Python and javascript (user interface)
- Back-end Framework: `Django <https://www.djangoproject.com>`_
- Web Servers: `Nginx <https://nginx.org/en/>`_
- WSGI Server: `Gunicorn <http://gunicorn.org>`_
- Hosting: TBD, `Heroku <https://www.heroku.com>`_ `Digital Ocean <https://www.digitalocean.com>`_  or `Amazon EC2 <https://aws.amazon.com/ec2/>`_
- Storage: `Amazon S3 <https://aws.amazon.com/s3/>`_
- Templating: `Jinja2 <http://jinja.pocoo.org>`_
- Front-end Framework: `Bootstrap <http://getbootstrap.com>`_ or `Semantic UI <https://semantic-ui.com>`_
- Email backend: `mailgun <https://www.mailgun.com>`_
- Database: `postgresql <https://www.postgresql.org>`_
- Unit Testing: `pytest <http://doc.pytest.org/en/latest/>`_ and `tox <https://tox.readthedocs.io/en/latest/>`_ 
- Integration testing: `selenium <http://www.seleniumhq.org>`_ + `phantomJS <http://phantomjs.org>`_
- Continuous integration: `Travis CI <https://travis-ci.org>`_
- Code coverage: `codecov <https://codecov.io>`_
- Countainer: `Docker <https://www.docker.com>`_ 
- SSL certificate: `DigiCert <https://www.digicert.com>`_ or another competitor.

Cost Estimation
---------------

Heroku (PaaS)

    Documentation is very good.
    Has built-in tools and architecture.
    Limited control over architecture while designing app.
    Heroku is best at what they provide.
    Deployment is taken care of (through git commands only).
    Good support.
    Not time consuming.

AWS EC2 (IaaS)

    AWS is versatile. They have many kinds of products. EC2, LAMBDA, EMR etc.,.
    You can go for Dedicated instance. You have more control over the architecture, like choosing OS, Version of the softwares, etc.
    Can use the automated deployment, or roll your own.
    Great support
  

User Interface
--------------

Deployment
----------

Testing
-------

References
----------

