=============================
The Data Service: zolware.com
=============================

Zolware Inc. provides a data service in the form of a set of web applications where registered users can:

- Define data sets from by loading a file, entering manually, or through Python functions.
- Store their data.
- Share their data with other registered users.
- Stream their data from our database to a remote server at a defined rate.
- Update their data on our database from a remote server at a defined rate.
- Sell or buy data to other registered user (digital market place).
- Vizualize and analyze their data.

The data service is accesible at https:\\zolware.com. Different pricing options can be considered.

1. Pay per use, e.g. per transaction on the market palce, per number of requests/hour, etc.
2. Subscription plans, e.g. pay per month with different pricing options defined by access to resources.

More details are provided in the business plan.

Overview
--------

The data service uses the Django web framework (Python) and is deployed on a multi-server architecture -- see Deployment. For the initial phase of the project, the data service is hosted on Heroku, a popular Platefrom as a Service (PaaS) provider in the Python community. The Django project has a Service-Oriented Architecture (SOA) and is broken up into isolated independent components (apps).

1. The *users* app (django-allauth), taking care of registration and authentication.
2. The *data* app for data generation, storage, and vizualization.
3. The *Market* app for the digital market place.

The project has different environments settings, i.e.

1. The *local* environment (settings for devlopement of the product).
2. The *test* environment (settings for continuous integration, tests, and coverage).
3. The *staging* environment (settings for a semi-private version of the site).
4. The *production* environment (settings for the live production servers).

These different settings use different third-party packages. The use of *pip* and *virtualenv* are needed to work on the different environments in an isolated manner. The coding style for the Python part of the project follows PEP 8. The JavaScript style still has to be defined.

.. toctree::
   :maxdepth: 1
   
   architecture
   usersApp
   dataApp
   marketApp
   security
   deployment
   logging
