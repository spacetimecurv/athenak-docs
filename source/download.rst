Download
========

Get a local AthenaK checkout with required submodules (especially Kokkos).

Recommended clone
-----------------

Use a recursive clone so Kokkos is fetched immediately:

.. code-block:: bash

   git clone --recursive https://github.com/IAS-Astrophysics/athenak.git
   cd athenak

Developer clone with token authentication
-----------------------------------------

If your workflow requires authenticated HTTPS operations from the start:

.. code-block:: bash

   git clone --recursive https://USERNAME:TOKEN@github.com/IAS-Astrophysics/athenak.git
   cd athenak

Replace ``TOKEN`` with a GitHub personal access token scoped appropriately for
your repository access.

If you already cloned without submodules
----------------------------------------

Initialize and update submodules (including Kokkos):

.. code-block:: bash

   git submodule init
   git submodule update

Verification
------------

Confirm the Kokkos submodule exists:

.. code-block:: bash

   ls kokkos

Next step
---------

Continue with :doc:`build`.
