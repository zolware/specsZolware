================
The Signal Class
================

|

.. comments

:Author(s):
   Francois Roy

:Date Created: 03-12-2017

:Language: None

:Status: :red:`Draft`

-----------


Description
-----------

The signal class is used to manipulate a single time series. It contains the information about the timestamp, the values of the measured quantity, the type of sensor, the units, the location, and one or more labels.


Inheritance
-----------

This class is not inherited.


Constructor Arguments
---------------------

- The stored data from the sensor. This is a 2-by-:math:`N` ``Matrix`` where the first row represents the timesatmp data, and where the second row represents the measured values. The number of column :math:`N` is the number of measurements.
- The type of sensor. This could be a ``String`` or an ``Enum``. 
- The units for the time stamps and measured values. This could be an array of ``String`` or an array of ``Enum`` of length 2.
- The location. This is a ``String``.
- The labels. This could be an array of ``String`` of size 3 where the unused value are set to a certain character.


Members
-------

- Original data ``Matrix``.
- Initial number of measurement ``int``.
- Sensor type ``Enum`` or ``String``.
- Units array of ``Enum`` or ``String`` of length 2.
- Sensor location ``String``.
- data ``Matrix``, the updated data when used online. 


Methods
--------------

- get_dt()
- getSize()
- getOriginalData()
- getData()
- getNumberofNewMeasurements()
- getMax()
- getMin()
- getLocation()
- getUnits()
- getLabel()
- getSensorType()
- addMeasurement()



Third-Party Packages
--------------------



Deployment
----------



Testing
-------

Use raw data obatined from a real sensor 

References
----------

`Data from the Tamar bridge. <https://github.com/jamesgoulet/BDLM/tree/master/Config_files>`_

.. Definitions

.. |longtext| replace:: This is a very very long text to include by substitution.
