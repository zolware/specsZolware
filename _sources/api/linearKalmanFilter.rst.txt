========================
The Linear Kalman Filter
========================

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

The model class contains all the information about the Bayesian network.


Theory
------

A typical equation:

.. math:: T(\mathbf{x},0)=T_0(\mathbf{x}),\qquad \textrm{at }t=0.
   :label: lkf_eq_1

Where :math:`T_0` is the initial temperature.

.. math::
  \int_{x_1}^{x_2} \varphi_n(x)\varphi_m(x)dx = \left\{
  \begin{array}{rl}
  1 & \text{if } m = n,\\
  0 & \text{if } m\neq n.
  \end{array} \right.
  :label: lkf_eq_2

Equation :eq:`lkf_eq_1` and :eq:`lkf_eq_2` have been used in to demonstrate...



.. note::
   This is a note.

A simple bokeh plot?

.. <iframe src="_static/example.html" height="300px" width="350px"></iframe>


.. plot::

   import matplotlib.pyplot as plt
   import numpy as np
   x = np.random.randn(1000)
   plt.hist( x, 20)
   plt.grid()
   plt.title(r'Normal: $\mu=%.2f, \sigma=%.2f$'%(x.mean(), x.std()))
   plt.show()

Sub-theory
~~~~~~~~~~

A basic table is presented in :numref:`lkf_table_label`.

.. _lkf_table_label:
.. csv-table:: :math:`\Lambda_i` for Different Homogeneous Boundary Type.
   :header: "Boundary Type", ":math:`k_1`", ":math:`k_2`", ":math:`s_1`", ":math:`s_2`", ":math:`\\Lambda_1,~x=x_1`", ":math:`\\Lambda_2,~x=x_2`"
   :widths: 15, 2, 2, 2, 2, 9, 9

   "Temperature, Dirichlet", 1, 1, 0, 0, ":math:`\frac{\partial}{\partial \xi}G(x,\xi,t-\tau)`", ":math:`-\frac{\partial}{\partial \xi}G(x,\xi,t-\tau)`"
   "Heat Flux, Neumann", 0, 0, 1, 1, ":math:`-G(x,\xi,t-\tau)`", ":math:`G(x,\xi,t-\tau)`"
   "Convection, Robin ", <0, >0, 1, 1, ":math:`-G(x,\xi,t-\tau)`", ":math:`G(x,\xi,t-\tau)`"
   "Mixed I", 1, 0, 0, 1, ":math:`\frac{\partial}{\partial \xi}G(x,\xi,t-\tau)`", ":math:`G(x,\xi,t-\tau)`"
   "Mixed II", 0, 1, 1, 0, ":math:`-G(x,\xi,t-\tau)`", ":math:`-\frac{\partial}{\partial \xi}G(x,\xi,t-\tau)`"

Third-Party Packages
--------------------



Architecture
------------



User Interface
--------------


Deployment
----------


Testing
-------



References
----------


.. Definitions

.. |longtext| replace:: This is a very very long text to include by substitution.
