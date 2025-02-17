.. Copyright (c) 2011-2022 Keith O'Hara

   Distributed under the terms of the Apache License, Version 2.0.

   The full license is in the file LICENSE, distributed with this software.

Cauchy Distribution
===================

**Table of contents**

.. contents:: :local:

----

Density Function
----------------

The density function of the Cauchy distribution:

.. math::

   f(x; \mu, \sigma) = \dfrac{1}{\pi \sigma \left[ 1 + \left( \frac{x - \mu}{\sigma} \right)^2 \right]}

Methods for scalar input, as well as for vector/matrix input, are listed below.

Scalar Input
~~~~~~~~~~~~

.. _dcauchy-func-ref1:
.. doxygenfunction:: dcauchy(const T1, const T2, const T3, const bool)
   :project: statslib

Vector/Matrix Input
~~~~~~~~~~~~~~~~~~~

STL Containers
______________

.. _dcauchy-func-ref2:
.. doxygenfunction:: dcauchy(const std::vector<eT>&, const T1, const T2, const bool)
   :project: statslib

Armadillo
_________

.. _dcauchy-func-ref3:
.. doxygenfunction:: dcauchy(const ArmaMat<eT>&, const T1, const T2, const bool)
   :project: statslib

Blaze
_____

.. _dcauchy-func-ref4:
.. doxygenfunction:: dcauchy(const BlazeMat<eT, To>&, const T1, const T2, const bool)
   :project: statslib

Eigen
_____

.. _dcauchy-func-ref5:
.. doxygenfunction:: dcauchy(const EigenMat<eT, iTr, iTc>&, const T1, const T2, const bool)
   :project: statslib

----

Cumulative Distribution Function
--------------------------------

The cumulative distribution function of the Cauchy distribution:

.. math::

   F(x; \mu, \sigma) = \int_{-\infty}^x f(z; \mu, \sigma) dz = 0.5 + \dfrac{1}{\pi} \text{arctan}\left( \frac{x - \mu}{\sigma} \right)

Methods for scalar input, as well as for vector/matrix input, are listed below.

Scalar Input
~~~~~~~~~~~~

.. _pcauchy-func-ref1:
.. doxygenfunction:: pcauchy(const T1, const T2, const T3, const bool)
   :project: statslib

Vector/Matrix Input
~~~~~~~~~~~~~~~~~~~

STL Containers
______________

.. _pcauchy-func-ref2:
.. doxygenfunction:: pcauchy(const std::vector<eT>&, const T1, const T2, const bool)
   :project: statslib

Armadillo
_________

.. _pcauchy-func-ref3:
.. doxygenfunction:: pcauchy(const ArmaMat<eT>&, const T1, const T2, const bool)
   :project: statslib

Blaze
_____

.. _pcauchy-func-ref4:
.. doxygenfunction:: pcauchy(const BlazeMat<eT, To>&, const T1, const T2, const bool)
   :project: statslib

Eigen
_____

.. _pcauchy-func-ref5:
.. doxygenfunction:: pcauchy(const EigenMat<eT, iTr, iTc>&, const T1, const T2, const bool)
   :project: statslib

----

Quantile Function
-----------------

The quantile function of the Cauchy distribution:

.. math::

   q(p; \mu, \sigma) = \mu + \gamma \text{tan} \left( \pi (p - 0.5) \right)

Methods for scalar input, as well as for vector/matrix input, are listed below.

Scalar Input
~~~~~~~~~~~~

.. _qcauchy-func-ref1:
.. doxygenfunction:: qcauchy(const T1, const T2, const T3)
   :project: statslib

Vector/Matrix Input
~~~~~~~~~~~~~~~~~~~

STL Containers
______________

.. _qcauchy-func-ref2:
.. doxygenfunction:: qcauchy(const std::vector<eT>&, const T1, const T2)
   :project: statslib

Armadillo
_________

.. _qcauchy-func-ref3:
.. doxygenfunction:: qcauchy(const ArmaMat<eT>&, const T1, const T2)
   :project: statslib

Blaze
_____

.. _qcauchy-func-ref4:
.. doxygenfunction:: qcauchy(const BlazeMat<eT, To>&, const T1, const T2)
   :project: statslib

Eigen
_____

.. _qcauchy-func-ref5:
.. doxygenfunction:: qcauchy(const EigenMat<eT, iTr, iTc>&, const T1, const T2)
   :project: statslib

----

Random Sampling
---------------

Random sampling for the Cauchy distribution is achieved via the inverse probability integral transform.

Scalar Output
~~~~~~~~~~~~~

Random number engines
_____________________

.. _rcauchy-func-ref1:
.. doxygenfunction:: rcauchy(const T1, const T2, rand_engine_t&)
   :project: statslib

Seed values
___________

.. _rcauchy-func-ref2:
.. doxygenfunction:: rcauchy(const T1, const T2, const ullint_t)
   :project: statslib

Vector/Matrix Output
~~~~~~~~~~~~~~~~~~~~

1. Random number engines

.. _rcauchy-func-ref3:
.. doxygenfunction:: rcauchy(const ullint_t, const ullint_t, const T1, const T2, rand_engine_t&)
   :project: statslib

2. Seed values

.. _rcauchy-func-ref4:
.. doxygenfunction:: rcauchy(const ullint_t, const ullint_t, const T1, const T2, const ullint_t)
   :project: statslib
