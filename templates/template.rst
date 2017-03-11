Title
=====
.. _Title:

.. _table_Lambda:
.. csv-table::
   :header: "Boundary Type", ":math:`k_1`", ":math:`k_2`", ":math:`s_1`", ":math:`s_2`", ":math:`\\Lambda_1,~x=x_1`", ":math:`\\Lambda_2,~x=x_2`"
   :widths: 15, 2, 2, 2, 2, 9, 9

   "Temperature, Dirichlet", 1, 1, 0, 0, ":math:`\frac{\partial}{\partial \xi}G(x,\xi,t-\tau)`", ":math:`-\frac{\partial}{\partial \xi}G(x,\xi,t-\tau)`"
   "Heat Flux, Neumann", 0, 0, 1, 1, ":math:`-G(x,\xi,t-\tau)`", ":math:`G(x,\xi,t-\tau)`"
   "Convection, Robin ", <0, >0, 1, 1, ":math:`-G(x,\xi,t-\tau)`", ":math:`G(x,\xi,t-\tau)`"
   "Mixed I", 1, 0, 0, 1, ":math:`\frac{\partial}{\partial \xi}G(x,\xi,t-\tau)`", ":math:`G(x,\xi,t-\tau)`"
   "Mixed II", 0, 1, 1, 0, ":math:`-G(x,\xi,t-\tau)`", ":math:`-\frac{\partial}{\partial \xi}G(x,\xi,t-\tau)`"

.. _greensFcts:
Statement of the Problem
------------------------

:ref:`Table 1 <table_Lambda>`
:ref:`Title`

Eigenvalues and Eigenfunctions
""""""""""""""""""""""""""""""

.. _table_Lambda:
.. csv-table:: Table 1: :math:`\Lambda_i` for Different Homogeneous Boundary Type.
   :header: "Boundary Type", ":math:`k_1`", ":math:`k_2`", ":math:`s_1`", ":math:`s_2`", ":math:`\\Lambda_1,~x=x_1`", ":math:`\\Lambda_2,~x=x_2`"
   :widths: 15, 2, 2, 2, 2, 9, 9

   "Temperature, Dirichlet", 1, 1, 0, 0, ":math:`\frac{\partial}{\partial \xi}G(x,\xi,t-\tau)`", ":math:`-\frac{\partial}{\partial \xi}G(x,\xi,t-\tau)`"
   "Heat Flux, Neumann", 0, 0, 1, 1, ":math:`-G(x,\xi,t-\tau)`", ":math:`G(x,\xi,t-\tau)`"
   "Convection, Robin ", <0, >0, 1, 1, ":math:`-G(x,\xi,t-\tau)`", ":math:`G(x,\xi,t-\tau)`"
   "Mixed I", 1, 0, 0, 1, ":math:`\frac{\partial}{\partial \xi}G(x,\xi,t-\tau)`", ":math:`G(x,\xi,t-\tau)`"
   "Mixed II", 0, 1, 1, 0, ":math:`-G(x,\xi,t-\tau)`", ":math:`-\frac{\partial}{\partial \xi}G(x,\xi,t-\tau)`"

References
----------

.. [Polyanin2001] `Andrei D. Polyanin, Handbook of Linear Partial Differential Equations for Engineers and Scientists, Chapman and Hall/CRC 2001 <http://goo.gl/jVjUFX>`_
.. [MyintU2007] `Tyn Myint-U, and Lokenath Debnath, Linear Partial Differential Equations for Scientists and Engineers, 4th edition, Birkhauser 2007 <http://goo.gl/1YIGSz>`_


