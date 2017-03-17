=================
Glossary of Terms
=================

.. glossary::

    The *state-space transition matrix*, :math:`\mathbf{A}_k`
       This matrix represents how the state-spaces evolve with the process (the physical model). The matrix elements may change at each time step.

    The *state-to-measurement measurement matrix*, :math:`\mathbf{H}_k`
       This matrix represents the relation between the state-spaces and the measurements. The matrix elements may change at each time step. If the matrix is diagonal, the readings from the sensors are uncorelated. If off-diagonal terms are present the measurements are correlated.   

    The *process noise covariance matrix*, :math:`\mathbf{Q}_k`
       This matrix represents the uncertainty on the state-spaces as they evolve with the process. The matrix elements may change at each time step. If the matrix is diagonal, the state-spaces are uncorelated. If off-diagonal terms are present the state-spaces are correlated.

    The *measurement noise covariance matrix*, :math:`\mathbf{R}_k`
       This matrix represents the uncertainty on the measurements or the sensors noise. The matrix elements may change at each time step. If the matrix is diagonal, the readings from the sensors are uncorelated. If off-diagonal terms are present the measurements are correlated.