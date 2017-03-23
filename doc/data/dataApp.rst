============
The data App
============

|

.. comments

:Author(s):
   Francois Roy

:Date Created: 03-18-2017

:Language: None

:Status: :red:`Draft`

-----------

Description
-----------

Models
------

.. csv-table:: The measurement model.
   :header: "Field", "Type", "Details"
   :widths: 10, 5, 15

    "name", "CharField", "unique=True"
    "project", "CharField", "blank=false"
    "isSimulated", "BooleanField", ""
    "index", "IntegerField", "unique=True"
    "xname", "CharField", "blank=false"
    "xunit", "CharField", "blank=true, validator for unit format"
    "yname", "CharField", "blank=false"
    "yunit", "CharField", "blank=true, validator for unit format"
    "sensorType", "CharField", "blank=true"
    "sensorLabel", "CharField", "blank=true"
    "sensorLocation", "CharField", "blank=true"
    "pubDate", "DateTimeField", "automatic (now)"
    "originator", "CharField", "automatic (user)"
    "reference", "CharField", "blank=true, validator or bibtex format"
    "details", "CharField", "blank=true"
    "filename", "FileField", "upload_to=generate_filename, storage=OverwriteStorage()"

.. todo::
   Define the fields. Index is position of the last measurement (the length) of the series.

Views
-----

Forms
-----

Templates
---------

Testing
-------

References
----------

