============
Architecture
============

|

.. comments

:Author(s): Francois Roy

:Date Created: 03-12-2017

:Language: None

:Status: :red:`Draft`

-----------

Overview
--------

Simple graphviz diagram:

.. graphviz::

   digraph G {
      subgraph cluster_0 {
         label="API";
         /* size ="4,4"; */
         Cpp [shape=box, label="C++ templates"];   /* this is a comment */
         Python [shape=box];
         Cpp -> Cython -> Python;
         Python -> Cython -> Cpp;
         }
      rankdir=LR;
      User -> Python;
      Python -> User;
    }

.. Basic Directory Structure

.. -------------------------

.. code-block bash

..  .
..  ├── .coverage
..  ├── .coveragerc
..  ├── .git
..  ├── .gitignore
..  ├── .travis.yml
..  ├── CMakeLists.txt
..  ├── LICENSE
..  ├── MANIFEST.in
..  ├── README.rst
..  ├── cmake
..  │   ├── DownloadProject.cmake
..  │   ├── FindSphinx.cmake
..  │   └── ReplicatePythonSourceTree.cmake
..  ├── cmake.config
..  │   └── DownloadProject.CMakeLists.cmake.in
..  ├── include
..  │   ├── Misc.h
..  │   └── Model.h
..  ├── publish-key.enc
..  ├── pytest.ini
..  ├── requirements
..  │   ├── base.txt
..  │   └── development.txt
..  ├── setup.cfg
..  ├── setup.py
..  ├── src
..  │   └── Misc.cxx
..  ├── tests
..  │   ├── CMakeLists.txt
..  │   ├── test_Misc.cxx
..  │   ├── test_Model.cxx
..  │   ├── test_main.cxx
..  │   ├── test_model.py
..  │   ├── test_utils.py
..  │   └── test_wrapper.py
.. ├── tox.ini
..  └── zolwareAPI
..      ├── CMakeLists.txt
..      ├── __init__.py
..      ├── command_line.py
..      ├── model.py
..      ├── utils.py
..      ├── w.pxd
..      └── wrapper.pyx


Suggested Technology
--------------------

1. Build engine: `Cmake <https://cmake.org/>`_
2. C++ template library for numerics: `Eigen <http://eigen.tuxfamily.org/>`_
3. Scientific computing: `Numpy <http://www.numpy.org>`_
4. Static compiler: `Cython <http://cython.org>`_
5. Figures: `Bokeh <http://bokeh.pydata.org/en/latest/>`_
6. Helper: `Eigency <https://github.com/wouterboomsma/eigency>`_
7. Command line library: `Click <http://click.pocoo.org/5/>`_





